# Comparing `tmp/korean_regex-0.0.3.tar.gz` & `tmp/korean_regex-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "korean_regex-0.0.3.tar", last modified: Sat Jun 10 03:24:36 2023, max compression
+gzip compressed data
```

## Comparing `korean_regex-0.0.3.tar` & `korean_regex-0.1.0.tar`

### file list

```diff
@@ -1,16 +1,13 @@
-drwxrwxrwx   0        0        0        0 2023-06-10 03:24:36.752951 korean_regex-0.0.3/
--rw-rw-rw-   0        0        0     1089 2023-05-15 00:16:47.000000 korean_regex-0.0.3/LICENSE
--rw-rw-rw-   0        0        0       34 2023-06-10 02:05:20.000000 korean_regex-0.0.3/MANIFEST.in
--rw-rw-rw-   0        0        0     8853 2023-06-10 03:24:36.751952 korean_regex-0.0.3/PKG-INFO
--rw-rw-rw-   0        0        0     7914 2023-06-10 03:22:20.000000 korean_regex-0.0.3/README.md
-drwxrwxrwx   0        0        0        0 2023-06-10 03:24:36.736201 korean_regex-0.0.3/ko_re/
--rw-rw-rw-   0        0        0       84 2023-06-10 02:35:30.000000 korean_regex-0.0.3/ko_re/__init__.py
--rw-rw-rw-   0        0        0    10476 2023-06-10 02:06:52.000000 korean_regex-0.0.3/ko_re/ko_re.py
-drwxrwxrwx   0        0        0        0 2023-06-10 03:24:36.750946 korean_regex-0.0.3/korean_regex.egg-info/
--rw-rw-rw-   0        0        0     8853 2023-06-10 03:24:36.000000 korean_regex-0.0.3/korean_regex.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      250 2023-06-10 03:24:36.000000 korean_regex-0.0.3/korean_regex.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-10 03:24:36.000000 korean_regex-0.0.3/korean_regex.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2023-06-10 02:31:17.000000 korean_regex-0.0.3/korean_regex.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0        6 2023-06-10 03:24:36.000000 korean_regex-0.0.3/korean_regex.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-10 03:24:36.752951 korean_regex-0.0.3/setup.cfg
--rw-rw-rw-   0        0        0     1287 2023-06-10 02:42:09.000000 korean_regex-0.0.3/setup.py
+-rw-r--r--   0        0        0      272 1970-01-01 00:00:00.000000 korean_regex-0.1.0/Cargo.toml
+-rw-r--r--   0        0        0     3526 2024-05-11 00:26:10.000000 korean_regex-0.1.0/.github/workflows/CI.yml
+-rw-r--r--   0        0        0     1692 2024-05-15 03:23:18.000000 korean_regex-0.1.0/.gitignore
+-rw-r--r--   0        0        0     1089 2024-05-15 03:23:54.000000 korean_regex-0.1.0/LICENSE
+-rw-r--r--   0        0        0     7071 2024-05-15 03:27:43.000000 korean_regex-0.1.0/README.md
+-rw-r--r--   0        0        0     1070 2024-05-15 03:25:48.000000 korean_regex-0.1.0/python/kre/__init__.py
+-rw-r--r--   0        0        0      263 2024-05-14 15:23:51.000000 korean_regex-0.1.0/python/kre/_core.pyi
+-rw-r--r--   0        0        0     4723 2024-05-15 03:10:39.000000 korean_regex-0.1.0/python/kre/_regex.py
+-rw-r--r--   0        0        0     1345 2024-05-15 02:42:14.000000 korean_regex-0.1.0/src/lib.rs
+-rw-r--r--   0        0        0     1402 2024-05-15 03:26:12.000000 korean_regex-0.1.0/tests/kre_test.py
+-rw-r--r--   0        0        0     9483 2024-05-15 02:41:58.000000 korean_regex-0.1.0/Cargo.lock
+-rw-r--r--   0        0        0      496 2024-05-15 03:26:08.000000 korean_regex-0.1.0/pyproject.toml
+-rw-r--r--   0        0        0     7424 1970-01-01 00:00:00.000000 korean_regex-0.1.0/PKG-INFO
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive
+POSIX tar archive (GNU)
```

### Comparing `korean_regex-0.0.3/LICENSE` & `korean_regex-0.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `korean_regex-0.0.3/README.md` & `korean_regex-0.1.0/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,99 +1,122 @@
-# ko_re: regex for Korean - Being free from ord/chr in Hangeul analysis.
+Metadata-Version: 2.3
+Name: korean-regex
+Version: 0.1.0
+Classifier: Programming Language :: Rust
+Classifier: Programming Language :: Python :: Implementation :: CPython
+Classifier: Programming Language :: Python :: Implementation :: PyPy
+License-File: LICENSE
+Requires-Python: >=3.8
+Description-Content-Type: text/markdown; charset=UTF-8; variant=GFM
+
+# korean-regex: Regex for Korean
 
 ## 소개
 
-ko_re는 한국어(한글)을 분석하기 위해 regex(정규표현식)에 문법을 추가한 패키지입니다. ko_re로는 한글과 관련한 많은 추가 기능을 사용할 수 있습니다.
+korean-regex는 한국어(한글)을 분석하기 위해 regex(정규표현식)에 문법을 추가한 패키지입니다. korean-regex로는 한글과 관련한 많은 추가 기능을 사용할 수 있습니다.
+
+Rust 바인딩을 사용하여 매우 성능이 좋습니다.
 
 ```python
-import ko_re
-regex = ko_re.compile(r'\b[^ ]+(?=[::^0]).\b')
+import kre
+regex = kre.compile(r'\b[^ ]+(?=[::^0]).\b')
 print(regex.findall('ko_re는 한국어(한글)을 분석하기 위해 regex(정규표현식)에 문법을 추가한 패키지입니다. ko_re로는 한글과 관련한 많은 추가 기능을 사용할 수 있습니다.')) # ['ko_re는', '한국어(한글)을', 'regex(정규표현식', '문법을', '추가한', 'ko_re로는', '관련한', '많은', '기능을', '사용할']
 ```
 
 ## 설치
 
-ko_re는 pip를 통해 설치하실 수 있습니다. ko_re를 설치하는 것이 **아닌** korean_regex를 설치해야 한다는 점에 주의하세요.
+korean-regex는 pip를 통해 설치하실 수 있습니다. kre를 설치하는 것이 **아닌** `korean-regex`를 설치해야 한다는 점에 주의하세요.
 
 ```python
-pip install -U korean_regex
+pip install -U korean-regex
 ```
 
 ## 상세
 
-기본적으로 ko_re는 bracket expression에서 특정한 조건을 발생시켰을 때 작동하는 추가적인 기능을 가미한 것입니다. 해당 조건을 제외한 나머지 상황에서는 파이썬의 기본 re 라이브러리와 동작이 완전히 같습니다.
+이 프로젝트는 [동명의 러스트 프로젝트](https://github.com/ilotoki0804/korean-regex-rust)를 파이썬으로 바인딩한 것입니다. 기본적인 작동 방식은 완전히 같으니 조금 더 자세한 설명이 필요하다면 [이 링크](https://docs.rs/korean_regex/latest/korean_regex/)를 참고하세요.
+
+기본적으로 korean-regex는 bracket expression에서 특정한 조건을 발생시켰을 때 작동하는 추가적인 기능을 가미한 것입니다. 해당 조건을 제외한 나머지 상황에서는 파이썬의 기본 re 라이브러리와 동작이 완전히 같습니다.
 
-우선 ko_re를 불러오려면 ko_re.compile()을 사용합니다. ko_re는 현재로선 compile만 지원합니다. 나머지는 compile로 re 객체를 만든 뒤 사용하세요.
+우선 korean-regex를 불러오려면 kre.compile()을 사용합니다. compile외에도 `kre.sub`나 `kre.search`, `kre.match`와 같이 바로 사용하는 것도 가능합니다.
 
-ko_re에서 처리되는 구문은 다음과 같습니다: `[초성:중성]`(`가`와 같은 종성이 없는 글자의 경우) 또는 `[초성:중성:종성]`, 또한 이는 regex의 bracket expression처럼 글자를 죽 이어서 쓰거나 `-`을 처리하는 것으로 여러 음소(소리의 최소 단위로, 자음과 모음을 의미합니다.)를 선택합니다.
+korean-regex에서 처리되는 구문은 다음과 같습니다: `[초성:중성]`(`가`와 같은 종성이 없는 글자의 경우) 또는 `[초성:중성:종성]`, 또한 이는 regex의 bracket expression처럼 글자를 죽 이어서 쓰거나 `-`을 처리하는 것으로 여러 음소(소리의 최소 단위로, 자음과 모음을 의미합니다.)를 선택합니다.
 
 예를 들어 `[ㄱㄴ:ㅏ]`는 regex구문에서 `[가나]`를 의미하고, `[ㄹㅎ:ㅗ:ㄶㅈ]`은 `[롢롲혾홎]`을 의미합니다. 또한 `[ㄱ-ㄹ:ㅏ]`는 `[가까나다따라]`를 의미합니다(`[가나다라]`가 아님에 주의하세요!).
 
 ```python
 # 예시 코드
-import ko_re
-some_regex = ko_re.compile('[ㄱㄴ:ㅏㅓㅣ:ㄶㄷㄹㅊ]')
+import kre
+some_regex = kre.compile('[ㄱㄴ:ㅏㅓㅣ:ㄶㄷㄹㅊ]')
 print(some_regex) # re.compile('[갆갇갈갗걶걷걸겇긶긷길깇낞낟날낯넎넏널넟닎닏닐닟]')
 print(some_regex.findall('길을 걷는 사람을 보았다. 그는 날 볼 낯이 없어서 멀리멀리 떠났다.')) # ['길', '걷', '날', '낯']
 ```
 
 또한 regex구문처럼 `^`도 지원합니다. 예를 들어 `[^ㄷㄹㅉㅎ:ㅏ]`는 `[가까나따마바빠사싸아자차카타파]`(`ㅏ` 조합 중 `다,라,짜,하` 없음.)입니다.
 
-만약 해당 자리에 모든 구문을 일치시키고 싶다면 해당 자리를 비워두거나 .으로 나타낼 수도 있습니다. 예를 들어 `[.:ㅏ]`는 가능한 모든 `ㅏ` 조합을 의미하고, `[:ㅗ:ㄴ]`은 `[곤꼰논돈똔...혼]`을 의미합니다. 비워두는 경우와 .으로 나타내는 경우는 완전히 동일하며 바꿔쓸 수 있습니다(단, 한 칸이 .으로 채워져 있다면 그 칸에는 다른 문자가 있어서는 안 됩니다.). 이를 응용하여 모든 한글 조합을 알아낼 수 있습니다. `[::]`(혹은 `[.:.:.])`이 바로 그 경우입니다.
+만약 해당 자리에 모든 구문을 일치시키고 싶다면 해당 자리를 비워놓으면 됩니다. 예를 들어 `[:ㅏ]`는 가능한 모든 `ㅏ` 조합을 의미하고, `[:ㅗ:ㄴ]`은 `[곤꼰논돈똔...혼]`을 의미합니다.
 
 ## 고급
 
 ### 조합의 사용
 
 된소리를 제외한 조합형 음소는 괄호를 이용해서 표현할 수 있습니다. 예를 들어 `ㅚ`는 `(ㅗㅣ)`와 완전히 같은 구문이고, `ㄶ`은 `(ㄴㅎ)`과 완전히 같습니다. 예를 들어 `[:ㅞㅢ:ㄶㄼ]`은 `[:(ㅜㅔ)ㅢ:ㄶ(ㄹㅂ)]`과 같습니다.
 
 ### `0`의 사용
 
 `0`은 해당 자리에 음소가 없다는 의미입니다. 예를 들어 `[ㄱ:ㅏ:0ㄴㅎ]`은 `[가간갛]`와 같습니다. 초성과 중성에는 기본적으로는 `0`을 사용하는 것이 금지되지만 특별한 경우, 한 음소를 나타내고 싶을 때, 사용됩니다. 예를 들어 `[0:ㅏ-ㅜ]` 혹은 `[0:ㅏ-ㅜ:0]`은 `[ㅏㅐㅑㅒㅓㅔㅕㅖㅗㅘㅙㅚㅛㅜ]`를 의미합니다. 또한 `[ㄱ-ㄹ:0]` 또는 `[ㄱ-ㄹ:0:0]`은 `[ㄱㄲㄴㄷㄸㄹ]`를 의미합니다. 하지만 초성과 중성에 `0`이 들어가는 경우는 몇 가지 제약이 있는데요, 우선 `0`이 들어가면 그 자리에는 `0` 외에 다른 음소를 작성할 수 없습니다. 다음은 몇 가지 조합은 `0`을 사용할 수 없다는 것입니다. 예를 들어 `[ㄱ:0:ㅎ]`을 생각해 봅시다. 이런 한글은 곰곰히 생각해도 사용할 수 있는 형태는 아닙니다. 이것 뿐만 아니라 `[0:ㅏ:ㅎ]`나 `[0:0:0]`도 금지됩니다.
 
-### compilestr 사용 및 응용
+<!-- ### compilestr 및 make_korean 사용 및 응용
+
+기본적으로 compile은 단순히 compilestr()을 거친 문자열을 re.complie()에 감싸는 것에 불과합니다.
 
-기본적으로 compile은 단순히 compilestr()을 거친 문자열을 re.complie()에 감싸는 것에 불과합니다. 
 ```python
-# compile의 내부 구현
 def compile(pattern, flags=0):
     return re.compile(compilestr(pattern), flags)
 ```
+
 따라서 처리 전 상태의 구문을 알고 싶다면 compilestr을 사용할 수 있습니다.
 
-만약 regex 구문이 궁금한 것이 아니라 그냥 가능한 모든 한글 조합을 알고 싶은 경우엔 compilestr의 기능을 응용할 수 있습니다.
+만약 regex 구문이 궁금한 것이 아니라 그냥 가능한 모든 한글 조합을 알고 싶은 경우엔 make_korean의 기능을 응용할 수 있습니다.
+
 ```python
 # 받침이 ㄴ인 글자 모두 뽑기
-import ko_re
-print(ko_re.compilestr('[::ㄴ]'))
-# [간갠갼걘건겐견곈곤관괜괸굔군권궨귄균근긘긴깐깬꺈꺤껀껜껸꼔꼰꽌꽨꾄꾠꾼꿘꿴뀐뀬끈끤낀난낸냔냰넌넨년녠논놘놴뇐뇬눈눤뉀뉜뉸는늰닌단댄댠댼던덴뎐뎬돈돤됀된됸둔둰뒌뒨듄든듼딘딴땐땬떈떤뗀뗜뗸똔똰뙌뙨뚄뚠뚼뛘뛴뜐뜬띈띤란랜랸럔런렌련롄론롼뢘뢴룐룬뤈뤤륀륜른릔린만맨먄먠먼멘면몐몬뫈뫤묀묜문뭔뭰뮌뮨믄믠민반밴뱐뱬번벤변볜본봔봰뵌뵨분붠붼뷘뷴븐븬빈빤뺀뺜뺸뻔뻰뼌뼨뽄뽠뽼뾘뾴뿐뿬쀈쀤쁀쁜쁸삔산샌샨섄선센션셴손솬쇈쇤숀순숸쉔쉰슌슨싄신싼쌘쌴썐썬쎈쎤쏀쏜쏸쐔쐰쑌쑨쒄쒠쒼쓘쓴씐씬안앤얀얜언엔연옌온완왠왼욘운원웬윈윤은읜인잔잰쟌쟨전젠젼졘존좐좬죈죤준줜줸쥔쥰즌즨진짠짼쨘쨴쩐쩬쪈쪤쫀쫜쫸쬔쬰쭌쭨쮄쮠쮼쯘쯴찐찬챈챤첀천첸쳔쳰촌촨쵄쵠쵼춘춴췐췬츈츤칀친칸캔캰컌컨켄켠켼콘콴쾐쾬쿈쿤퀀퀜퀸큔큰킌킨탄탠탼턘턴텐텬톈톤퇀퇜퇸툔툰퉌퉨튄튠튼틘틴판팬퍈퍤펀펜편폔폰퐌퐨푄푠푼풘풴퓐퓬픈픤핀한핸햔햰헌헨현혠혼환홴횐횬훈훤휀휜휸흔흰힌]
-```
+import kre
+print(kre.make_korean('[::ㄴ]'))
+# 간갠갼걘...휸흔흰힌
+``` -->
 
-## 정규 음운 후행 자모순
+## 정규 음운 선행 자모순
 
-`regular_first` 자모순('정규 음운 후행 자모순' 이하 '후행 자모순')은 된소리나 자음군, 합용자들이 뒤로 보내진 순서입니다.
+`regular_first` 자모순('정규 음운 선행 자모순' 이하 '선행 자모순')은 된소리나 자음군, 합용자들이 뒤로 보내진 순서입니다.
 
-비교하면 기본 순서(유니코드 순서 또는 사전순)은 다음과 같습니다:
+기본 순서(유니코드 순서 또는 사전순)은 다음과 같습니다:
 
-초성: ㄱㄲㄴㄷㄸㄹㅁㅂㅃㅅㅆㅇㅈㅉㅊㅋㅌㅍㅎ
+* 초성: ㄱㄲㄴㄷㄸㄹㅁㅂㅃㅅㅆㅇㅈㅉㅊㅋㅌㅍㅎ
+* 중성: ㅏㅐㅑㅒㅓㅔㅕㅖㅗㅘㅙㅚㅛㅜㅝㅞㅟㅠㅡㅢㅣ
+* 종성: ㄱㄲㄳㄴㄵㄶㄷㄹㄺㄻㄼㄽㄾㄿㅀㅁㅂㅄㅅㅆㅇㅈㅊㅋㅌㅍㅎ
 
-중성: ㅏㅐㅑㅒㅓㅔㅕㅖㅗㅘㅙㅚㅛㅜㅝㅞㅟㅠㅡㅢㅣ
+하지만 선행 자모순은 다음과 같습니다:
 
-종성: ㄱㄲㄳㄴㄵㄶㄷㄹㄺㄻㄼㄽㄾㄿㅀㅁㅂㅄㅅㅆㅇㅈㅊㅋㅌㅍㅎ
+* 초성: ㄱㄴㄷㄹㅁㅂㅅㅇㅈㅊㅋㅌㅍㅎㄲㄸㅃㅆㅉ
+* 중성: ㅏㅑㅓㅕㅗㅛㅜㅠㅡㅣㅐㅒㅔㅖㅘㅙㅚㅝㅞㅟㅢ
+* 종성: ㄱㄴㄷㄹㅁㅂㅅㅇㅈㅊㅋㅌㅍㅎㄲㄳㄵㄶㄺㄻㄼㄽㄾㄿㅀㅄㅆ
 
-하지만 후행 자모순은 다음과 같습니다:
-
-초성: ㄱㄴㄷㄹㅁㅂㅅㅇㅈㅊㅋㅌㅍㅎㄲㄸㅃㅆㅉ
-
-중성: ㅏㅑㅓㅕㅗㅛㅜㅠㅡㅣㅐㅒㅔㅖㅘㅙㅚㅝㅞㅟㅢ
+이 순서는 `-`를 통해 값에 접근할 때 사용되지만, 정렬은 일반적인 유니코드 순서(사전 순서)대로 정렬됩니다.
 
-종성: ㄱㄴㄷㄹㅁㅂㅅㅇㅈㅊㅋㅌㅍㅎㄲㄳㄵㄶㄺㄻㄼㄽㄾㄿㅀㅄㅆ
+예를 들어 `[ㄱ-ㅎ:0:0]`은 기본 순서에서는 모든 초성을 포함하는 `[ㄱㄲㄴㄷㄸㄹㅁㅂㅃㅅㅆㅇㅈㅉㅊㅋㅌㅍㅎ]`이지만, 선행 자모순에서는 `[ㄱㄴㄷㄹㅁㅂㅅㅇㅈㅊㅋㅌㅍㅎ]`입니다.
 
-이 순서는 `-`를 통해 값에 접근할 때 사용되지만, 정렬은 일반적인 유니코드 순서(사전 순서)대로 정렬됩니다.
+다음과 같은 방식으로 선행 자모순을 사용할 수 있습니다.
 
-예를 들어 `[ㄱ-ㅎ:0:0]`은 기본 순서에서는 모든 초성을 포함하는 `[ㄱㄲㄴㄷㄸㄹㅁㅂㅃㅅㅆㅇㅈㅉㅊㅋㅌㅍㅎ]`이지만, 후행 자모순에서는 `[ㄱㄴㄷㄹㅁㅂㅅㅇㅈㅊㅋㅌㅍㅎ]`입니다.
+```python
+import kre
 
-이 자모순은 특히 된소리가 아닌 일반적으로 알고 있는 순서를 사용하고 싶을 때 유용하게 사용할 수 있습니다.
+kre.compile("[ㄱ-ㅎ:ㅏ]", "regular_first") # 선행 자모순
+kre.compile("[ㄱ-ㅎ:ㅏ]", "default") # 기본값(사전순)
+```
 
 ## release note
 
-0.0.3(첫 안정화 버전): ko_re 시작.
+* 0.1.0: 러스트 바인딩으로 완전히 처음부터 재제작, 기존 버전과 완전히 다름.
+* 0.0.5: make_korean 추가, 이름 변경, 타입 추가, 리팩토링, 검사 추가
+* 0.0.4: readme 보강, 리팩토링
+* 0.0.3(첫 안정화 버전): 시작
+
```

