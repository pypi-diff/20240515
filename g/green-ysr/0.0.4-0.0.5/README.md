# Comparing `tmp/green_ysr-0.0.4.tar.gz` & `tmp/green_ysr-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "green_ysr-0.0.4.tar", max compression
+gzip compressed data, was "green_ysr-0.0.5.tar", max compression
```

## Comparing `green_ysr-0.0.4.tar` & `green_ysr-0.0.5.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0       47 2024-03-27 16:55:40.900726 green_ysr-0.0.4/green_ysr/__init__.py
--rw-r--r--   0        0        0    14953 2024-03-27 16:10:55.986540 green_ysr-0.0.4/green_ysr/green_ysr.py
--rw-r--r--   0        0        0      421 2024-03-27 17:17:56.559731 green_ysr-0.0.4/pyproject.toml
--rw-r--r--   0        0        0      465 2024-03-27 17:13:49.003936 green_ysr-0.0.4/README.md
--rw-r--r--   0        0        0     1083 1970-01-01 00:00:00.000000 green_ysr-0.0.4/PKG-INFO
+-rw-r--r--   0        0        0       47 2024-03-27 16:55:40.900726 green_ysr-0.0.5/green_ysr/__init__.py
+-rw-r--r--   0        0        0    17576 2024-05-15 13:11:52.379210 green_ysr-0.0.5/green_ysr/green_ysr.py
+-rw-r--r--   0        0        0      421 2024-05-15 13:13:26.824840 green_ysr-0.0.5/pyproject.toml
+-rw-r--r--   0        0        0      465 2024-03-27 17:13:49.003936 green_ysr-0.0.5/README.md
+-rw-r--r--   0        0        0     1083 1970-01-01 00:00:00.000000 green_ysr-0.0.5/PKG-INFO
```

### Comparing `green_ysr-0.0.4/green_ysr/green_ysr.py` & `green_ysr-0.0.5/green_ysr/green_ysr.py`

 * *Files 20% similar despite different names*

```diff
@@ -119,14 +119,47 @@
             elif x1+x2<=0.00001 and x1-x2<=0.00001:
                 G1=(np.exp((m*w/pf)*(x1+x2))*(-1/x1-1/x2)*pf*np.sin(pf*(-x1-x2))+np.exp(-(m*w/pf)*(-x1+x2))*(-1/x1+1/x2)*pf*np.sin(pf*(-x1+x2)) )*(m/(2*np.pi*pf**2))*BCS
                 G2=(np.exp((m*w/pf)*(x1+x2))*(-1/x1-1/x2)*pf*np.cos(pf*(-x1-x2))+np.exp(-(m*w/pf)*(-x1+x2))*(-1/x1+1/x2)*pf*np.cos(pf*(-x1+x2)) +2*pf/x1)*(m/(2*np.pi*pf**2))*xi
             elif x1+x2<0.00001 and x1-x2>0.00001:
                 G1=(np.exp((m*w/pf)*(x1+x2))*(-1/x1-1/x2)*pf*np.sin(pf*(-x1-x2))+np.exp(-(m*w/pf)*(-x2+x1))*(-1/x2+1/x1)*pf*np.sin(pf*(-x2+x1)) )*(m/(2*np.pi*pf**2))*BCS
                 G2=(np.exp((m*w/pf)*(x1+x2))*(-1/x1-1/x2)*pf*np.cos(pf*(-x1-x2))+np.exp(-(m*w/pf)*(-x2+x1))*(-1/x2+1/x1)*pf*np.cos(pf*(-x2+x1)) +2*pf/x2)*(m/(2*np.pi*pf**2))*xi
             G0 = G1+G2
+        if self.mode==2:
+            ## mode=2 is for the hexagonal-shaped Fermi contour
+            ## x1=x and x2=y
+            x1=r1[0]-r2[0]
+            x2=r1[1]-r2[1]
+            k=0
+            R=[[-1/2,-np.sqrt(3)/2],[np.sqrt(3)/2,-1/2]]
+            Rr=[[-1/2,np.sqrt(3)/2],[-np.sqrt(3)/2,-1/2]]
+            if x2>=0 and x2>np.sqrt(3)*x1:
+                D=np.matmul(Rr,[x1,x2])
+                x1=D[0]
+                x2=D[1]
+            elif x2<=0 and x2<-np.sqrt(3)*x1:
+                D=np.matmul(R,[x1,x2])
+                x1=D[0]
+                x2=D[1]
+            chi=m*w/pf
+            a=np.divide(2,np.sqrt(3))*np.abs(x2)
+            b=x1-np.divide(1,np.sqrt(3))*np.abs(x2)
+            c=x1+np.divide(1,np.sqrt(3))*np.abs(x2)
+            if np.abs(x1) < 0.1 and np.abs(x2) < 0.1:
+                G1 = np.sqrt(3)
+                G2 = 0.0
+            elif np.abs(x2)<0.001:
+                G1=(2/(np.sqrt(3)*x1*pf))*np.exp(-chi*x1)*np.sin(pf*x1)+(np.cos(pf*x1)/np.sqrt(3))*np.exp(-chi*x1)
+                G2=(2/(np.sqrt(3)*x1*pf))*np.exp(-chi*x1)*np.cos(pf*x1)-(np.sin(pf*x1)/np.sqrt(3))*np.exp(-chi*x1)-2/(np.sqrt(3)*x1*pf)
+            elif np.abs(np.sqrt(3)*x1-np.abs(x2))<0.001*np.sqrt(3):
+                G1=(1/(np.sqrt(3)*x1*pf))*np.exp(-2*chi*x1)*np.sin(2*pf*x1)+(np.cos(2*pf*x1)/np.sqrt(3))*np.exp(-2*chi*x1)
+                G2=(1/(np.sqrt(3)*x1*pf))*np.exp(-2*chi*x1)*np.cos(2*pf*x1)-(np.sin(2*pf*x1)/np.sqrt(3))*np.exp(-2*chi*x1)-2/(2*np.sqrt(3)*x1*pf)
+            else:
+                G1=(np.exp(-chi*c)*np.sin(c*pf)*(1/(np.sqrt(3)*b)+1/(np.sqrt(3)*a))+np.exp(-chi*b)*np.sin(b*pf)*(-1/(np.sqrt(3)*a)+1/(np.sqrt(3)*c))+np.exp(-chi*a)*np.sin(a*pf)*(-1/(np.sqrt(3)*b)+1/(np.sqrt(3)*c)))/pf
+                G2=(np.exp(-chi*c)*np.cos(c*pf)*(-1/(np.sqrt(3)*b)-1/(np.sqrt(3)*a))+np.exp(-chi*b)*np.cos(b*pf)*(1/(np.sqrt(3)*a)-1/(np.sqrt(3)*c))+np.exp(-chi*a)*np.cos(a*pf)*(1/(np.sqrt(3)*b)-1/(np.sqrt(3)*c))+2/(np.sqrt(3)*c))/pf
+            G0=-(2*m/(np.sqrt(3)*np.pi))*G1*BCS-(2*m/(np.sqrt(3)*np.pi))*G2*xi
         return G0
     
     def V(self,theta,alpha,U):
         return alpha * np.cos(theta)*np.kron(self.s0,self.s3) + alpha*np.sin(theta)*np.kron(self.s0,self.s1) + U*np.kron(self.s3,self.s0)
     
     def M(self,E):
         n=self.N
@@ -160,17 +193,16 @@
 
     def ElecDOS(self,r_,E):
         return np.imag(np.trace(np.dot(self.G(r_,E),np.diag((1,1,0,0)))))
 
     def HoleDOS(self,r_,E):
         return np.imag(np.trace(np.dot(self.G(r_,E),np.diag((0,0,1,1)))))
 
-    
 
-    
+
 
 class lattice():
     def __init__(self,type='atom',N=1,coords=None,pitch_x=0,direction=(1,0),alpha=0.04,U=0,spiral = 0,mode=0,m=18.7,pf = 0.21,delta_s = 1e-3,gamma_s=50e-6,E_px=500,E_range=(-5,5),V_range=(-3,3),spin_texture = None,T=1.3) -> None:
         self.N = N
         self.mode = mode
         self.m=m
         self.pf=pf
@@ -237,17 +269,17 @@
         return coords
 
     def show_lattice(self):
         f,ax = plt.subplots(1)
         for i in self.coords:
             ax.scatter(i[0],i[1],color='C0')
 
-    def map_coord_gen(self,spac,resolution,size): # spac is the point spacing of the grid, resolution is the number of points in one line, size is the length in units of spacing 
+    def map_coord_gen(self,resolution,size): # resolution is the number of points in one line, size= side of the square defining the mapped area
         self.resolution = resolution
-        A = np.arange(-spac*size/2,spac*size/2+(spac*size)/resolution,(spac*size)/resolution)
+        A = np.arange(-size/2,size/2+(size)/resolution,(size)/resolution)
         Gx = np.meshgrid(A,A)[0]
         Gy = np.meshgrid(A,A)[1]
         self.map_coords = [Gx,Gy]
 
     def show_lattice_map(self):
         f,ax = plt.subplots(1)
         for i in range(len(self.map_coords[0])):
@@ -308,40 +340,55 @@
         for i in range(0,len(self.LSx)):
             self.LS.append(self.didv((self.LSx[i],self.LSy[i])))
         self.LS = np.array(self.LS)
 
         
     def LSconvolute(self,Delta_t,Gamma_t):
         self.LSC = np.zeros(self.LS.shape)
-        self.V = np.linspace(-self.delta_s*self.V_range,self.delta_s*self.V_range,self.E_px)
+        self.V = np.linspace(-self.delta_s*self.V_range[0],self.delta_s*self.V_range[1],self.E_px)
         for i in range(self.LS.shape[0]):
             self.LSC[i,:] = (dynesConvolute(self.V,self.E,self.LS[i,:],Delta_t,self.T,Gamma_t))
     
     def explorer(self):
-        self.figure = plt.figure(figsize=(6,6))
-        self.axMap = self.figure.add_subplot(1,1,1)
-        self.figure.subplots_adjust(bottom=0.35)
+        self.figure = plt.figure(figsize=(7,5))
+        self.axMap = self.figure.add_subplot(2,2,1)
+        self.axSpec = self.figure.add_subplot(2,2,2)
+        self.figure.subplots_adjust(bottom=0)
         self.ax1 = self.figure.add_axes([0.20, 0.10, 0.65, 0.03])
         self.ax2 = self.figure.add_axes([0.20, 0.15, 0.65, 0.03])
         self.ax3 = self.figure.add_axes([0.20, 0.20, 0.65, 0.03])
         self.energyCut_slider = Slider(self.ax1,'Energy cut',self.E.min()*1e3,self.E.max()*1e3,valinit=0, valstep=(0.01))
         self.smin_slider = Slider(self.ax2, 'Min', self.didv_map.min(), self.didv_map.max(), valinit =self.didv_map.min())
         self.smax_slider = Slider(self.ax3, 'Max', self.didv_map.min(), self.didv_map.max(), valinit =self.didv_map.max()*0.5)            
         self.energyCut_slider.on_changed(self.update_energy)
         self.smin_slider.on_changed(self.update_cscale)
         self.smax_slider.on_changed(self.update_cscale)
         self.didv_map_cut = self.didv_map[:,:,0]
         self.im1 = self.axMap.imshow(np.flipud(self.didv_map_cut),interpolation='nearest')
         #axis labels
         self.axMap.set_xlabel('x (nm)')
         self.axMap.set_ylabel('y (nm)')
+        self.axSpec.set_xlabel('Energy (meV)')
+        self.axSpec.set_xlabel('LDOS (GN)')
 
+
+        self.figure.canvas.mpl_connect('button_press_event', self.onclick)
     def update_energy(self,val):
         self.cutIdx = (abs(self.E-val*1e-3)).argmin()
         self.im1.set_data(np.flipud(self.didv_map[:,:,self.cutIdx]))
         self.im1.set_clim(self.didv_map[:,:,self.cutIdx].min(),self.didv_map[:,:,self.cutIdx].max())
         # self.label.set_text('{} mV'.format(np.round(val,2)))
         self.figure.canvas.draw()
 
     def update_cscale(self,val):
         self.im1.set_clim([self.smin_slider.val,self.smax_slider.val])
         self.figure.canvas.draw()
+
+    def onclick(self, event):
+        if event.inaxes == self.axMap:
+            self.axSpec.clear()
+            x = int(round(event.xdata))
+            y = int(round(event.ydata))
+            self.axSpec.plot(self.E*1e3,np.flipud(self.didv_map)[x,y,:])
+            self.axSpec.set_xlabel('Energy (meV)')
+            self.axSpec.set_ylabel('LDOS (GN)')
+            self.figure.canvas.draw()
```

### Comparing `green_ysr-0.0.4/PKG-INFO` & `green_ysr-0.0.5/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: green-ysr
-Version: 0.0.4
+Version: 0.0.5
 Summary: Green function model to calculate LDOS of multiple YSR impurites
 Home-page: https://github.com/nanogunecic09/green-ysr
 License: MIT
 Author: stefanotriv
 Author-email: s.trivini@nanogune.eu
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
```

