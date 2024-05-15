# Comparing `tmp/oj_tools-0.0.3.tar.gz` & `tmp/oj_tools-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "oj_tools-0.0.3.tar", last modified: Tue May 14 15:00:44 2024, max compression
+gzip compressed data, was "oj_tools-0.0.4.tar", last modified: Wed May 15 20:28:30 2024, max compression
```

## Comparing `oj_tools-0.0.3.tar` & `oj_tools-0.0.4.tar`

### file list

```diff
@@ -1,12 +1,14 @@
-drwxr-xr-x   0 hepheir    (501) staff       (20)        0 2024-05-14 15:00:44.739927 oj_tools-0.0.3/
--rw-r--r--   0 hepheir    (501) staff       (20)     1870 2024-05-14 15:00:44.739741 oj_tools-0.0.3/PKG-INFO
--rw-r--r--   0 hepheir    (501) staff       (20)     1383 2024-05-14 11:57:20.000000 oj_tools-0.0.3/README.md
--rw-r--r--   0 hepheir    (501) staff       (20)      489 2024-05-14 15:00:33.000000 oj_tools-0.0.3/pyproject.toml
--rw-r--r--   0 hepheir    (501) staff       (20)       38 2024-05-14 15:00:44.739969 oj_tools-0.0.3/setup.cfg
-drwxr-xr-x   0 hepheir    (501) staff       (20)        0 2024-05-14 15:00:44.738583 oj_tools-0.0.3/src/
--rw-r--r--   0 hepheir    (501) staff       (20)     3446 2024-05-14 14:59:04.000000 oj_tools-0.0.3/src/oj.py
-drwxr-xr-x   0 hepheir    (501) staff       (20)        0 2024-05-14 15:00:44.739580 oj_tools-0.0.3/src/oj_tools.egg-info/
--rw-r--r--   0 hepheir    (501) staff       (20)     1870 2024-05-14 15:00:44.000000 oj_tools-0.0.3/src/oj_tools.egg-info/PKG-INFO
--rw-r--r--   0 hepheir    (501) staff       (20)      178 2024-05-14 15:00:44.000000 oj_tools-0.0.3/src/oj_tools.egg-info/SOURCES.txt
--rw-r--r--   0 hepheir    (501) staff       (20)        1 2024-05-14 15:00:44.000000 oj_tools-0.0.3/src/oj_tools.egg-info/dependency_links.txt
--rw-r--r--   0 hepheir    (501) staff       (20)        3 2024-05-14 15:00:44.000000 oj_tools-0.0.3/src/oj_tools.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 20:28:30.267180 oj_tools-0.0.4/
+-rw-r--r--   0 runner    (1001) docker     (127)     2301 2024-05-15 20:28:30.267180 oj_tools-0.0.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1815 2024-05-15 20:28:20.000000 oj_tools-0.0.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      489 2024-05-15 20:28:20.000000 oj_tools-0.0.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-15 20:28:30.267180 oj_tools-0.0.4/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 20:28:30.267180 oj_tools-0.0.4/src/
+-rw-r--r--   0 runner    (1001) docker     (127)      282 2024-05-15 20:28:20.000000 oj_tools-0.0.4/src/oj.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 20:28:30.267180 oj_tools-0.0.4/src/oj_tools.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2301 2024-05-15 20:28:30.000000 oj_tools-0.0.4/src/oj_tools.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      209 2024-05-15 20:28:30.000000 oj_tools-0.0.4/src/oj_tools.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-15 20:28:30.000000 oj_tools-0.0.4/src/oj_tools.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       20 2024-05-15 20:28:30.000000 oj_tools-0.0.4/src/oj_tools.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2238 2024-05-15 20:28:20.000000 oj_tools-0.0.4/src/problem.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2297 2024-05-15 20:28:20.000000 oj_tools-0.0.4/src/testcase.py
```

### Comparing `oj_tools-0.0.3/PKG-INFO` & `oj_tools-0.0.4/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: oj-tools
-Version: 0.0.3
+Version: 0.0.4
 Summary: tools for Online Judge management
 Author-email: hepheir <hepheir@gmail.com>
 Project-URL: Homepage, https://https://github.com/hepheir/oj-tools
 Project-URL: Issues, https://https://github.com/hepheir/oj-tools/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -21,55 +21,51 @@
 ```shell
 pip install --upgrade oj-tools
 ```
 
 
 ## Example
 
-아래는 100 보다 작거나 같은 '소수'를 구하는 문제의 테스트 케이스를 생성하는 예시 입니다.
+아래는 $N \leq 100$ 인 $N$ 번째 소수를 구하는 문제의 테스트 케이스를 생성하는 예시 입니다.
 
 ```python
-def primes(n):
+def prime_generator(hi):
     # Sieve of Eratosthenes
     # https://en.wikipedia.org/wiki/Sieve_of_Eratosthenes
-    sieve = [True] * (n+1)
-    for p in range(2, n+1):
+    sieve = [True] * (hi+1)
+    for p in range(2, hi+1):
         if sieve[p]:
-            for j in range(2*p, n+1, p):
+            for j in range(2*p, hi+1, p):
                 sieve[j] = False
             yield p
 
 
 if __name__ == '__main__':
-    import oj
+    # 100번째 소수들까지 사전에 구해둡니다.
+    # 100번째 소수는 541 입니다. (https://prime-numbers.info/number/100th-prime)
+    primes = list(prime_generator(hi=541))
+
+    # 1. Problem 객체를 생성합니다.
+    problem = Problem('prime_numbers')
+
+    # 입력 데이터로는 1이상 100 이하의 정수를 일부 사용하며, 테스트케이스 번호는 1부터 세어봅니다.
+    for testcase_no, x in enumerate(range(1, 101, 3), start=1):
+        # 2-1. input_data에 대한 올바른 output_data를 구합니다.
+        y = primes[x-1] # 1-base에서 0-base로 보정
+
+        # 2-2. TestCase 객체를 생성합니다.
+        tc = TestCase()
+
+        # 2-3. TestCase 객체에 입출력 데이터를 삽입합니다.
+        tc.input.from_args(x)
+        tc.output.from_args(y)
+        # tc.input.from_file('./sample.txt')
+        # tc.input.from_text("""
+        #     1 2
+        # """, dedent=True)
 
-    # 1. 문제를 생성합니다.
-    problem = oj.Problem('prime_numbers')
-
-    for id, prime in enumerate(primes(100), start=1):
-        # 2-1. 테스트케이스를 생성합니다.
-        tc = oj.TestCase(
-            id=str(id),
-            input=str(prime),
-            output=str(fib(prime))
-        )
-
-        if int(tc.output) > oj.INTEGER_SIZE:
-            print('MAX_INTEGER_SIZE EXCEEDED')
-            print(tc.output)
-            break
-
-        # 2-2. 테스트케이스를 문제에 추가합니다.
+        # 2-4. 테스트케이스를 문제에 추가합니다.
         problem.add_testcase(tc)
 
-    # 3. 문제의 정보와 테스트케이스를 .zip 파일로 출력합니다.
-    problem.extract_as_zip()
+    # 3. 문제의 정보와 테스트케이스를 prime_numbers.zip 파일로 출력합니다.
+    problem.extract_as_dir()
 ```
-
-
-## Documentation
-
-### Problem
-
-#### .title
-
-문제를 구분하는
```

### Comparing `oj_tools-0.0.3/README.md` & `oj_tools-0.0.4/README.md`

 * *Files 27% similar despite different names*

```diff
@@ -8,55 +8,51 @@
 ```shell
 pip install --upgrade oj-tools
 ```
 
 
 ## Example
 
-아래는 100 보다 작거나 같은 '소수'를 구하는 문제의 테스트 케이스를 생성하는 예시 입니다.
+아래는 $N \leq 100$ 인 $N$ 번째 소수를 구하는 문제의 테스트 케이스를 생성하는 예시 입니다.
 
 ```python
-def primes(n):
+def prime_generator(hi):
     # Sieve of Eratosthenes
     # https://en.wikipedia.org/wiki/Sieve_of_Eratosthenes
-    sieve = [True] * (n+1)
-    for p in range(2, n+1):
+    sieve = [True] * (hi+1)
+    for p in range(2, hi+1):
         if sieve[p]:
-            for j in range(2*p, n+1, p):
+            for j in range(2*p, hi+1, p):
                 sieve[j] = False
             yield p
 
 
 if __name__ == '__main__':
-    import oj
+    # 100번째 소수들까지 사전에 구해둡니다.
+    # 100번째 소수는 541 입니다. (https://prime-numbers.info/number/100th-prime)
+    primes = list(prime_generator(hi=541))
+
+    # 1. Problem 객체를 생성합니다.
+    problem = Problem('prime_numbers')
+
+    # 입력 데이터로는 1이상 100 이하의 정수를 일부 사용하며, 테스트케이스 번호는 1부터 세어봅니다.
+    for testcase_no, x in enumerate(range(1, 101, 3), start=1):
+        # 2-1. input_data에 대한 올바른 output_data를 구합니다.
+        y = primes[x-1] # 1-base에서 0-base로 보정
+
+        # 2-2. TestCase 객체를 생성합니다.
+        tc = TestCase()
+
+        # 2-3. TestCase 객체에 입출력 데이터를 삽입합니다.
+        tc.input.from_args(x)
+        tc.output.from_args(y)
+        # tc.input.from_file('./sample.txt')
+        # tc.input.from_text("""
+        #     1 2
+        # """, dedent=True)
 
-    # 1. 문제를 생성합니다.
-    problem = oj.Problem('prime_numbers')
-
-    for id, prime in enumerate(primes(100), start=1):
-        # 2-1. 테스트케이스를 생성합니다.
-        tc = oj.TestCase(
-            id=str(id),
-            input=str(prime),
-            output=str(fib(prime))
-        )
-
-        if int(tc.output) > oj.INTEGER_SIZE:
-            print('MAX_INTEGER_SIZE EXCEEDED')
-            print(tc.output)
-            break
-
-        # 2-2. 테스트케이스를 문제에 추가합니다.
+        # 2-4. 테스트케이스를 문제에 추가합니다.
         problem.add_testcase(tc)
 
-    # 3. 문제의 정보와 테스트케이스를 .zip 파일로 출력합니다.
-    problem.extract_as_zip()
+    # 3. 문제의 정보와 테스트케이스를 prime_numbers.zip 파일로 출력합니다.
+    problem.extract_as_dir()
 ```
-
-
-## Documentation
-
-### Problem
-
-#### .title
-
-문제를 구분하는
```

### Comparing `oj_tools-0.0.3/src/oj.py` & `oj_tools-0.0.4/src/problem.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,115 +1,58 @@
-import hashlib
+from pathlib import Path
 import json
 import os
-import pathlib
 import tempfile
 import typing
 import zipfile
 
-
-__all__ = [
-    'LONG_LONG_SIZE',
-    'INTEGER_SIZE',
-    'TestCase',
-    'Problem'
-]
-
-
-LONG_LONG_SIZE = 2305843009213693952
-INTEGER_SIZE = 2147483648
-
-
-class TestCase:
-    def __init__(self, id: str, input: str, output: str, strip=True) -> None:
-        self.id = id
-        self.input = input.strip() if strip else input
-        self.output = output.strip() if strip else output
-
-    @property
-    def input_size(self) -> int:
-        """Length of input data."""
-        return len(self.input)
-
-    @property
-    def output_size(self) -> int:
-        """Length of output data."""
-        return len(self.output)
-
-    @property
-    def input_name(self) -> str:
-        """A filename for the input."""
-        return f'{self.id}.in'
-
-    @property
-    def output_name(self) -> str:
-        """A filename for the output."""
-        return f'{self.id}.out'
-
-    @property
-    def stripped_output_md5(self) -> str:
-        md5 = hashlib.md5()
-        md5.update(self.output.strip().encode())
-        return md5.hexdigest()
-
-    def as_dict(self) -> dict:
-        return {
-            "stripped_output_md5": self.stripped_output_md5,
-            "input_size": self.input_size,
-            "output_size": self.output_size,
-            "input_name": self.input_name,
-            "output_name": self.output_name,
-        }
-
-    def extract_as_file(self, dir='./') -> None:
-        """Save testcase as `input_name` and `output_name` in a specific directory."""
-        dir_path = pathlib.Path(dir)
-        with open(dir_path / self.input_name, 'w') as f:
-            f.write(self.input)
-        with open(dir_path / self.output_name, 'w') as f:
-            f.write(self.output)
+from testcase import TestCase
 
 
 class Problem:
     def __init__(self, title: str) -> None:
         self.title = title
         self.spj = False
         self.testcases: typing.Dict[str, TestCase] = {}
 
     def add_testcase(self, testcase: TestCase):
         """Add a testcase for this problem."""
-        self.testcases[testcase.id] = testcase
+        self.testcases[testcase] = testcase
 
-    def as_dict(self) -> dict:
-        return {
-            "spj": self.spj,
-            "testcases": {
-                key: val.as_dict() for key, val in self.testcases.items()
-            },
-        }
-
-    @property
-    def default_zip_path(self) -> pathlib.Path:
-        return pathlib.Path(f'./{self.title}.zip')
+    def extract_as_dir(self, dirname: typing.Optional[str]=None, in_ext='.in', out_ext='.out') -> None:
+        """Save problem in a directory.
 
+        dirname: default is `./PROBLEM_TITLE`
+        """
+        dir_path = Path(dirname) if dirname is not None else Path(f'./{self.title}')
+        info_filename = 'info'
+        if not os.path.exists(dir_path):
+            os.makedirs(dir_path)
+        for testcase in self.testcases.values():
+            testcase.input.extract_as_file(dir_path / (testcase.id+in_ext))
+            testcase.output.extract_as_file(dir_path / (testcase.id+out_ext))
+        with open(dir_path / info_filename, 'w') as f:
+            json.dump({
+                "spj": self.spj,
+                "testcases": {
+                    testcase.id: {
+                        "stripped_output_md5": testcase.stripped_output_md5,
+                        "input_size": testcase.input_size,
+                        "output_size": testcase.output_size,
+                        "input_name": (testcase.id+in_ext),
+                        "output_name": (testcase.id+out_ext),
+                    } for testcase in self.testcases.values()
+                },
+            }, f, ensure_ascii=True)
 
     def extract_as_zip(self, filename: typing.Optional[str]=None) -> None:
         """Save problem as .zip file
 
         filename: default is `./PROBLEM_TITLE.zip`
         """
         with tempfile.TemporaryDirectory() as tmp_dir:
-            zip_path = pathlib.Path(filename) if filename is not None else self.default_zip_path
-            dir_path = pathlib.Path(tmp_dir)
-            info_filename = 'info'
-
-            for testcase in self.testcases.values():
-                testcase.extract_as_file(dir=dir_path)
-
-            with open(dir_path / info_filename, 'w') as f:
-                json.dump(self.as_dict(), f, ensure_ascii=True)
-
+            zip_path = Path(filename) if filename is not None else Path(f'./{self.title}.zip')
+            dir_path = Path(tmp_dir)
+            self.extract_as_dir(dir_path)
             with zipfile.ZipFile(zip_path, 'w') as fzip:
-                for testcase in self.testcases.values():
-                    fzip.write(filename=dir_path / testcase.input_name, arcname=testcase.input_name)
-                    fzip.write(filename=dir_path / testcase.output_name, arcname=testcase.output_name)
-                fzip.write(filename=dir_path / info_filename, arcname=info_filename)
+                for basename in os.listdir(dir_path):
+                    fzip.write(filename=dir_path/basename, arcname=basename)
```

### Comparing `oj_tools-0.0.3/src/oj_tools.egg-info/PKG-INFO` & `oj_tools-0.0.4/src/oj_tools.egg-info/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: oj-tools
-Version: 0.0.3
+Version: 0.0.4
 Summary: tools for Online Judge management
 Author-email: hepheir <hepheir@gmail.com>
 Project-URL: Homepage, https://https://github.com/hepheir/oj-tools
 Project-URL: Issues, https://https://github.com/hepheir/oj-tools/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -21,55 +21,51 @@
 ```shell
 pip install --upgrade oj-tools
 ```
 
 
 ## Example
 
-아래는 100 보다 작거나 같은 '소수'를 구하는 문제의 테스트 케이스를 생성하는 예시 입니다.
+아래는 $N \leq 100$ 인 $N$ 번째 소수를 구하는 문제의 테스트 케이스를 생성하는 예시 입니다.
 
 ```python
-def primes(n):
+def prime_generator(hi):
     # Sieve of Eratosthenes
     # https://en.wikipedia.org/wiki/Sieve_of_Eratosthenes
-    sieve = [True] * (n+1)
-    for p in range(2, n+1):
+    sieve = [True] * (hi+1)
+    for p in range(2, hi+1):
         if sieve[p]:
-            for j in range(2*p, n+1, p):
+            for j in range(2*p, hi+1, p):
                 sieve[j] = False
             yield p
 
 
 if __name__ == '__main__':
-    import oj
+    # 100번째 소수들까지 사전에 구해둡니다.
+    # 100번째 소수는 541 입니다. (https://prime-numbers.info/number/100th-prime)
+    primes = list(prime_generator(hi=541))
+
+    # 1. Problem 객체를 생성합니다.
+    problem = Problem('prime_numbers')
+
+    # 입력 데이터로는 1이상 100 이하의 정수를 일부 사용하며, 테스트케이스 번호는 1부터 세어봅니다.
+    for testcase_no, x in enumerate(range(1, 101, 3), start=1):
+        # 2-1. input_data에 대한 올바른 output_data를 구합니다.
+        y = primes[x-1] # 1-base에서 0-base로 보정
+
+        # 2-2. TestCase 객체를 생성합니다.
+        tc = TestCase()
+
+        # 2-3. TestCase 객체에 입출력 데이터를 삽입합니다.
+        tc.input.from_args(x)
+        tc.output.from_args(y)
+        # tc.input.from_file('./sample.txt')
+        # tc.input.from_text("""
+        #     1 2
+        # """, dedent=True)
 
-    # 1. 문제를 생성합니다.
-    problem = oj.Problem('prime_numbers')
-
-    for id, prime in enumerate(primes(100), start=1):
-        # 2-1. 테스트케이스를 생성합니다.
-        tc = oj.TestCase(
-            id=str(id),
-            input=str(prime),
-            output=str(fib(prime))
-        )
-
-        if int(tc.output) > oj.INTEGER_SIZE:
-            print('MAX_INTEGER_SIZE EXCEEDED')
-            print(tc.output)
-            break
-
-        # 2-2. 테스트케이스를 문제에 추가합니다.
+        # 2-4. 테스트케이스를 문제에 추가합니다.
         problem.add_testcase(tc)
 
-    # 3. 문제의 정보와 테스트케이스를 .zip 파일로 출력합니다.
-    problem.extract_as_zip()
+    # 3. 문제의 정보와 테스트케이스를 prime_numbers.zip 파일로 출력합니다.
+    problem.extract_as_dir()
 ```
-
-
-## Documentation
-
-### Problem
-
-#### .title
-
-문제를 구분하는
```

