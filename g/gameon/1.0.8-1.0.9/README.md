# Comparing `tmp/gameon-1.0.8.tar.gz` & `tmp/gameon-1.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gameon-1.0.8.tar", last modified: Mon May 13 13:49:03 2024, max compression
+gzip compressed data, was "gameon-1.0.9.tar", last modified: Mon May 13 20:06:41 2024, max compression
```

## Comparing `gameon-1.0.8.tar` & `gameon-1.0.9.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0        0        0        0 2024-05-13 13:49:03.654429 gameon-1.0.8/
--rw-rw-rw-   0        0        0      683 2024-05-13 13:48:41.000000 gameon-1.0.8/CHANGELOG.txt
--rw-rw-rw-   0        0        0     1060 2022-07-06 14:58:58.000000 gameon-1.0.8/LICENCE.txt
--rw-rw-rw-   0        0        0       25 2022-07-06 14:59:00.000000 gameon-1.0.8/MANIFEST.in
--rw-rw-rw-   0        0        0      262 2024-05-13 13:49:03.653427 gameon-1.0.8/PKG-INFO
--rw-rw-rw-   0        0        0      172 2022-07-06 14:47:52.000000 gameon-1.0.8/README.txt
-drwxrwxrwx   0        0        0        0 2024-05-13 13:49:03.642054 gameon-1.0.8/gameon/
--rw-rw-rw-   0        0        0    19206 2024-05-13 13:47:54.000000 gameon-1.0.8/gameon/__init__.py
--rw-rw-rw-   0        0        0    11661 2024-04-25 10:58:03.000000 gameon-1.0.8/gameon/icon.ico
-drwxrwxrwx   0        0        0        0 2024-05-13 13:49:03.652061 gameon-1.0.8/gameon.egg-info/
--rw-rw-rw-   0        0        0      262 2024-05-13 13:49:03.000000 gameon-1.0.8/gameon.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      241 2024-05-13 13:49:03.000000 gameon-1.0.8/gameon.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-13 13:49:03.000000 gameon-1.0.8/gameon.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       22 2024-05-13 13:49:03.000000 gameon-1.0.8/gameon.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2024-05-13 13:49:03.000000 gameon-1.0.8/gameon.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-13 13:49:03.654429 gameon-1.0.8/setup.cfg
--rw-rw-rw-   0        0        0      396 2024-05-13 13:48:48.000000 gameon-1.0.8/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-13 20:06:41.639101 gameon-1.0.9/
+-rw-rw-rw-   0        0        0      773 2024-05-13 20:06:12.000000 gameon-1.0.9/CHANGELOG.txt
+-rw-rw-rw-   0        0        0     1060 2022-07-06 14:58:58.000000 gameon-1.0.9/LICENCE.txt
+-rw-rw-rw-   0        0        0       25 2022-07-06 14:59:00.000000 gameon-1.0.9/MANIFEST.in
+-rw-rw-rw-   0        0        0      262 2024-05-13 20:06:41.637651 gameon-1.0.9/PKG-INFO
+-rw-rw-rw-   0        0        0      172 2022-07-06 14:47:52.000000 gameon-1.0.9/README.txt
+drwxrwxrwx   0        0        0        0 2024-05-13 20:06:41.609895 gameon-1.0.9/gameon/
+-rw-rw-rw-   0        0        0    18349 2024-05-13 20:05:40.000000 gameon-1.0.9/gameon/__init__.py
+-rw-rw-rw-   0        0        0    11661 2024-04-25 10:58:03.000000 gameon-1.0.9/gameon/icon.ico
+drwxrwxrwx   0        0        0        0 2024-05-13 20:06:41.635352 gameon-1.0.9/gameon.egg-info/
+-rw-rw-rw-   0        0        0      262 2024-05-13 20:06:41.000000 gameon-1.0.9/gameon.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      241 2024-05-13 20:06:41.000000 gameon-1.0.9/gameon.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-13 20:06:41.000000 gameon-1.0.9/gameon.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       22 2024-05-13 20:06:41.000000 gameon-1.0.9/gameon.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2024-05-13 20:06:41.000000 gameon-1.0.9/gameon.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-13 20:06:41.639101 gameon-1.0.9/setup.cfg
+-rw-rw-rw-   0        0        0      396 2024-05-13 20:06:25.000000 gameon-1.0.9/setup.py
```

### Comparing `gameon-1.0.8/CHANGELOG.txt` & `gameon-1.0.9/CHANGELOG.txt`

 * *Files 12% similar despite different names*

```diff
@@ -31,8 +31,12 @@
 
 1.0.7 (5/02/2024)
 -------------------
 - Added load() function to load images
 
 1.0.8 (5/13/2024)
 -------------------
-- Bug fixes
+- Bug fixes
+
+1.0.9 (5/13/2024)
+-------------------
+- Added Player() class to create a full player
```

### Comparing `gameon-1.0.8/LICENCE.txt` & `gameon-1.0.9/LICENCE.txt`

 * *Files identical despite different names*

### Comparing `gameon-1.0.8/gameon/__init__.py` & `gameon-1.0.9/gameon/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -51,28 +51,14 @@
 right_click = False
 
 #key_pressed
 keys = ['a','b','c','d','e','f','g','h','i','j','k','l','m','n','o','p','q','r','s','t','u','v','w','x','y','z','space','1','2','3','4','5','6','7','8','9','0']
 pygame_keys = [pygame.K_a,pygame.K_b,pygame.K_c,pygame.K_d,pygame.K_e,pygame.K_f,pygame.K_g,pygame.K_h,pygame.K_i,pygame.K_j,pygame.K_k,pygame.K_l,pygame.K_m,pygame.K_n,pygame.K_o,pygame.K_p,pygame.K_q,pygame.K_r,pygame.K_s,pygame.K_t,pygame.K_u,pygame.K_v,pygame.K_w,pygame.K_x,pygame.K_y,pygame.K_z,pygame.K_SPACE,pygame.K_1,pygame.K_2,pygame.K_3,pygame.K_4,pygame.K_5,pygame.K_6,pygame.K_7,pygame.K_8,pygame.K_9,pygame.K_0]
 keys_boolean = [False,False,False,False,False,False,False,False,False,False,False,False,False,False,False,False,False,False,False,False,False,False,False,False,False,False,False,False,False,False,False,False,False,False,False,False,False]
 
-#player
-# player_x = 0
-# player_y = 0
-# jumped = False
-# jump_velocity = 0
-# player_width = 0
-# player_height = 0
-# player_run_once = True
-# player_speed = 0
-# original_x = 0
-# original_y = 0
-# change_x = 0
-# change_y = 0
-
 def fill(color):
     global screen,screen_color
     if not isinstance(color,tuple):
         if color.lower() in color_map:
             screen_color = color_map[color.lower()]
     elif isinstance(color, tuple):
         screen_color = color
@@ -387,97 +373,83 @@
                             screen.blit(image, (x,y))
                             return click(button, one)
                     else:
                         screen.blit(image, (x,y))
                         return False
     pass
 
-# def player(image,x,y,left='a',right='d',up='w',down='s',jump='space',speed=3,jump_height=20, collide_sides=False):
-#     global original_x,original_y,change_x,change_y,player_speed,player_x,player_y,player_width,player_height,jump_velocity,jumped,player_run_once,screen
-#     if player_run_once:
-#         jump_velocity = jump_height
-#         player_x = x
-#         player_y = y
-#         if isinstance(image, str):
-#             player_width = pygame.image.load(image).get_width()
-#             player_height = pygame.image.load(image).get_height()
-#         elif isinstance(image, pygame.Surface):
-#             player_width = image.get_width()
-#             player_height = image.get_height()
-
-#         player_speed = speed
-#         original_x = x
-#         original_y = y
-#         player_run_once = False
-#     change_x = x
-#     change_y = y
-#     if change_x != original_x or change_y != original_y:
-#         player_x = change_x
-#         player_y = change_y
-#         player_run_once = True
-#     if jump != None:
-#         if jumped == False and kb.is_pressed(jump):
-#             jumped = True
-#     if not collide_sides:
-#         if left != None:
-#             if kb.is_pressed(left):
-#                 player_x -= speed
-#         if right != None:
-#             if kb.is_pressed(right):
-#                 player_x += speed
-#         if up != None:
-#             if kb.is_pressed(up):
-#                 player_y -= speed
-#         if down != None:
-#             if kb.is_pressed(down):
-#                     player_y += speed
-#         if jump != None:
-#             if jumped:
-#                 player_y -= jump_velocity
-#                 jump_velocity -= 1
-#                 if jump_velocity < -jump_height:
-#                     jumped = False
-#                     jump_velocity = jump_height
-#     if collide_sides:
-#         if left != None:
-#             if kb.is_pressed(left) and player_x > 0:
-#                 player_x -= speed
-#         if right != None:
-#             if kb.is_pressed(right) and player_x < screen.get_width() - player_width:
-#                 player_x += speed
-#         if up != None:
-#             if kb.is_pressed(up) and player_y > 0:
-#                 player_y -= speed
-#         if down != None:
-#             if kb.is_pressed(down) and player_y < screen.get_height() - player_height:
-#                 player_y += speed
-#         if jump != None:
-#             if jumped:
-#                 player_y -= jump_velocity
-#                 jump_velocity -= 1
-#                 if jump_velocity < -jump_height:
-#                     jumped = False
-#                     jump_velocity = jump_height
-#     if collide_sides:
-#         if player_x > screen.get_width() - player_width:
-#             player_x = screen.get_width() - player_width
-#         if player_x < 0:
-#             player_x = 0
-#         if player_y > screen.get_height() - player_height:
-#             player_y = screen.get_height() - player_height
-#         if player_y < 0:
-#             player_y = 0
-#         pass
-#     if isinstance(image, str):
-#         screen.blit(pygame.image.load(image).convert_alpha(), (player_x,player_y))
-#         return pygame.Rect(player_x,player_y,pygame.image.load(image).get_width(),pygame.image.load(image).get_height())
-#     elif isinstance(image, pygame.Surface):
-#         screen.blit(image.convert_alpha(), (player_x,player_y))
-#         return pygame.Rect(player_x,player_y,image.get_width(),image.get_height())
-#     pass
+class Player:
+    def __init__(self,image,x,y,left=None,right=None,up=None,down=None,jump=False,speed=3,height=20,sides=True):
+        self.image = image
+        self.x = x
+        self.y = y
+        self.left = left
+        self.right = right
+        self.up = up
+        self.down  = down
+        self.jump = jump
+        self.speed = speed
+        self.height = height
+        self.sides = sides
+        self.player_width = 0
+        self.player_width = 0
+        self.jumped = True
+        self.jump_velocity = self.height
+        pass
+    def move(self):
+        if not self.sides:
+            if self.left != None:
+                if kb.is_pressed(self.left):
+                    self.x -= self.speed
+            if self.right != None:
+                if kb.is_pressed(self.right):
+                    self.x += self.speed
+            if self.up != None:
+                if kb.is_pressed(self.up):
+                    self.y -= self.speed
+            if self.down != None:
+                if kb.is_pressed(self.down):
+                        self.y += self.speed
+            if self.jump != None:
+                if self.jumped:
+                    self.y -= self.jump_velocity
+                    self.jump_velocity -= 1
+                    if self.jump_velocity < -self.height:
+                        self.jumped = False
+                        self.jump_velocity = self.height
+        if self.sides:
+            if self.left != None:
+                if kb.is_pressed(self.left) and self.x > 0:
+                    self.x -= self.speed
+            if self.right != None:
+                if kb.is_pressed(self.right) and self.x < screen.get_width() - self.player_width:
+                    self.x += self.speed
+            if self.up != None:
+                if kb.is_pressed(self.up) and self.y > 0:
+                    self.y -= self.speed
+            if self.down != None:
+                if kb.is_pressed(self.down) and self.y < screen.get_height() - self.player_height:
+                    self.y += self.speed
+            if self.jump != None:
+                if self.jumped:
+                    self.y -= self.jump_velocity
+                    self.jump_velocity -= 1
+                    if self.jump_velocity < -self.height:
+                        self.jumped = False
+                        self.jump_velocity = self.height
+        if isinstance(self.image, str):
+            screen.blit(pygame.image.load(self.image).convert_alpha(), (self.x,self.y))
+            self.player_width = pygame.image.load(self.image).get_width()
+            self.player_height = pygame.image.load(self.image).get_height()
+        elif isinstance(self.image, pygame.Surface):
+            screen.blit(self.image.convert_alpha(), (self.x,self.y))
+            self.player_width = self.image.get_width()
+            self.player_height = self.image.get_height()
+        pass
+    pass
 
 def box(image,x,y,collision=True):
     global player_x,player_y,player_width,player_height,player_speed
     player_rect = pygame.Rect(player_x,player_y,player_width,player_height)
     col_box = pygame.Rect(x,y,image.get_width(),image.get_height())
     if collision:
         if player_rect.colliderect(col_box):
```

### Comparing `gameon-1.0.8/gameon/icon.ico` & `gameon-1.0.9/gameon/icon.ico`

 * *Files identical despite different names*

