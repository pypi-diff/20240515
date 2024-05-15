# Comparing `tmp/medroom_ai_dataengineer-0.0.5.tar.gz` & `tmp/medroom_ai_dataengineer-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "medroom_ai_dataengineer-0.0.5.tar", last modified: Sat Apr 20 22:19:46 2024, max compression
+gzip compressed data, was "medroom_ai_dataengineer-0.0.6.tar", last modified: Wed May 15 19:00:54 2024, max compression
```

## Comparing `medroom_ai_dataengineer-0.0.5.tar` & `medroom_ai_dataengineer-0.0.6.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxrwxrwx   0        0        0        0 2024-04-20 22:19:46.514792 medroom_ai_dataengineer-0.0.5/
--rw-rw-rw-   0        0        0    11558 2024-02-15 13:42:00.000000 medroom_ai_dataengineer-0.0.5/LICENSE
-drwxrwxrwx   0        0        0        0 2024-04-20 22:19:46.512741 medroom_ai_dataengineer-0.0.5/MedRoom.AI.DataEngineer.egg-info/
--rw-rw-rw-   0        0        0    13755 2024-04-20 22:19:46.000000 medroom_ai_dataengineer-0.0.5/MedRoom.AI.DataEngineer.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      578 2024-04-20 22:19:46.000000 medroom_ai_dataengineer-0.0.5/MedRoom.AI.DataEngineer.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0      115 2024-04-20 22:19:46.000000 medroom_ai_dataengineer-0.0.5/MedRoom.AI.DataEngineer.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2024-04-12 17:49:13.000000 medroom_ai_dataengineer-0.0.5/MedRoom.AI.DataEngineer.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0      139 2024-04-20 22:19:46.000000 medroom_ai_dataengineer-0.0.5/MedRoom.AI.DataEngineer.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2024-04-20 22:19:46.000000 medroom_ai_dataengineer-0.0.5/MedRoom.AI.DataEngineer.egg-info/top_level.txt
--rw-rw-rw-   0        0        0    13755 2024-04-20 22:19:46.513831 medroom_ai_dataengineer-0.0.5/PKG-INFO
--rw-rw-rw-   0        0        0     7190 2024-04-12 22:03:40.000000 medroom_ai_dataengineer-0.0.5/README.md
-drwxrwxrwx   0        0        0        0 2024-04-20 22:19:46.456509 medroom_ai_dataengineer-0.0.5/medroom/
-drwxrwxrwx   0        0        0        0 2024-04-20 22:19:46.457585 medroom_ai_dataengineer-0.0.5/medroom/dna/
-drwxrwxrwx   0        0        0        0 2024-04-20 22:19:46.508881 medroom_ai_dataengineer-0.0.5/medroom/dna/processors/
--rw-rw-rw-   0        0        0        0 2024-02-15 13:42:00.000000 medroom_ai_dataengineer-0.0.5/medroom/dna/processors/__init__.py
--rw-rw-rw-   0        0        0      663 2024-02-15 13:42:00.000000 medroom_ai_dataengineer-0.0.5/medroom/dna/processors/config.py
--rw-rw-rw-   0        0        0      606 2024-02-15 13:42:00.000000 medroom_ai_dataengineer-0.0.5/medroom/dna/processors/main.py
-drwxrwxrwx   0        0        0        0 2024-04-20 22:19:46.512613 medroom_ai_dataengineer-0.0.5/medroom/dna/processors/utils/
--rw-rw-rw-   0        0        0        0 2024-02-15 13:42:00.000000 medroom_ai_dataengineer-0.0.5/medroom/dna/processors/utils/__init__.py
--rw-rw-rw-   0        0        0     4385 2024-04-12 20:49:37.000000 medroom_ai_dataengineer-0.0.5/medroom/dna/processors/utils/evalmetrics.py
--rw-rw-rw-   0        0        0     4949 2024-04-20 21:31:01.000000 medroom_ai_dataengineer-0.0.5/medroom/dna/processors/utils/mlflow_helper.py
--rw-rw-rw-   0        0        0     2908 2024-04-12 22:02:34.000000 medroom_ai_dataengineer-0.0.5/medroom/dna/processors/utils/textclean.py
--rw-rw-rw-   0        0        0       42 2024-04-20 22:19:46.514792 medroom_ai_dataengineer-0.0.5/setup.cfg
--rw-rw-rw-   0        0        0     1298 2024-02-15 13:42:00.000000 medroom_ai_dataengineer-0.0.5/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-15 19:00:54.732989 medroom_ai_dataengineer-0.0.6/
+-rw-rw-rw-   0        0        0    11558 2024-02-15 13:42:00.000000 medroom_ai_dataengineer-0.0.6/LICENSE
+drwxrwxrwx   0        0        0        0 2024-05-15 19:00:54.730969 medroom_ai_dataengineer-0.0.6/MedRoom.AI.DataEngineer.egg-info/
+-rw-rw-rw-   0        0        0    13755 2024-05-15 19:00:54.000000 medroom_ai_dataengineer-0.0.6/MedRoom.AI.DataEngineer.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      578 2024-05-15 19:00:54.000000 medroom_ai_dataengineer-0.0.6/MedRoom.AI.DataEngineer.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0      115 2024-05-15 19:00:54.000000 medroom_ai_dataengineer-0.0.6/MedRoom.AI.DataEngineer.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2024-04-12 17:49:13.000000 medroom_ai_dataengineer-0.0.6/MedRoom.AI.DataEngineer.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0      139 2024-05-15 19:00:54.000000 medroom_ai_dataengineer-0.0.6/MedRoom.AI.DataEngineer.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2024-05-15 19:00:54.000000 medroom_ai_dataengineer-0.0.6/MedRoom.AI.DataEngineer.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0    13755 2024-05-15 19:00:54.731994 medroom_ai_dataengineer-0.0.6/PKG-INFO
+-rw-rw-rw-   0        0        0     8428 2024-05-15 18:52:35.000000 medroom_ai_dataengineer-0.0.6/README.md
+drwxrwxrwx   0        0        0        0 2024-05-15 19:00:54.659638 medroom_ai_dataengineer-0.0.6/medroom/
+drwxrwxrwx   0        0        0        0 2024-05-15 19:00:54.659638 medroom_ai_dataengineer-0.0.6/medroom/dna/
+drwxrwxrwx   0        0        0        0 2024-05-15 19:00:54.725872 medroom_ai_dataengineer-0.0.6/medroom/dna/processors/
+-rw-rw-rw-   0        0        0        0 2024-02-15 13:42:00.000000 medroom_ai_dataengineer-0.0.6/medroom/dna/processors/__init__.py
+-rw-rw-rw-   0        0        0      663 2024-02-15 13:42:00.000000 medroom_ai_dataengineer-0.0.6/medroom/dna/processors/config.py
+-rw-rw-rw-   0        0        0      606 2024-02-15 13:42:00.000000 medroom_ai_dataengineer-0.0.6/medroom/dna/processors/main.py
+drwxrwxrwx   0        0        0        0 2024-05-15 19:00:54.730913 medroom_ai_dataengineer-0.0.6/medroom/dna/processors/utils/
+-rw-rw-rw-   0        0        0        0 2024-02-15 13:42:00.000000 medroom_ai_dataengineer-0.0.6/medroom/dna/processors/utils/__init__.py
+-rw-rw-rw-   0        0        0     4385 2024-04-12 20:49:37.000000 medroom_ai_dataengineer-0.0.6/medroom/dna/processors/utils/evalmetrics.py
+-rw-rw-rw-   0        0        0     4949 2024-04-20 21:31:01.000000 medroom_ai_dataengineer-0.0.6/medroom/dna/processors/utils/mlflow_helper.py
+-rw-rw-rw-   0        0        0     2908 2024-04-12 22:02:34.000000 medroom_ai_dataengineer-0.0.6/medroom/dna/processors/utils/textclean.py
+-rw-rw-rw-   0        0        0       42 2024-05-15 19:00:54.732989 medroom_ai_dataengineer-0.0.6/setup.cfg
+-rw-rw-rw-   0        0        0     1298 2024-02-15 13:42:00.000000 medroom_ai_dataengineer-0.0.6/setup.py
```

### Comparing `medroom_ai_dataengineer-0.0.5/LICENSE` & `medroom_ai_dataengineer-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `medroom_ai_dataengineer-0.0.5/MedRoom.AI.DataEngineer.egg-info/PKG-INFO` & `medroom_ai_dataengineer-0.0.6/MedRoom.AI.DataEngineer.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: MedRoom.AI.DataEngineer
-Version: 0.0.5
+Version: 0.0.6
 Summary: A Natural Language Processing Data Engineer
 Home-page: https://github.com/MedRoomGitHub/MedRoom.AI.DataEngineer
 Author: Team IA
 Author-email: medroom@medroom.com.br
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
@@ -213,8 +213,8 @@
 Requires-Dist: spacy==3.7.1
 Requires-Dist: unidecode==1.3.7
 Requires-Dist: matplotlib==3.7.0
 Requires-Dist: pandas==2.1.1
 Requires-Dist: numpy==1.26.0
 Requires-Dist: seaborn==0.13.0
 Requires-Dist: scikit-learn==1.3.1
-Requires-Dist: mlflow==2.12.1
+Requires-Dist: mlflow==2.12.2
```

### Comparing `medroom_ai_dataengineer-0.0.5/MedRoom.AI.DataEngineer.egg-info/SOURCES.txt` & `medroom_ai_dataengineer-0.0.6/MedRoom.AI.DataEngineer.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `medroom_ai_dataengineer-0.0.5/PKG-INFO` & `medroom_ai_dataengineer-0.0.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: MedRoom.AI.DataEngineer
-Version: 0.0.5
+Version: 0.0.6
 Summary: A Natural Language Processing Data Engineer
 Home-page: https://github.com/MedRoomGitHub/MedRoom.AI.DataEngineer
 Author: Team IA
 Author-email: medroom@medroom.com.br
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
@@ -213,8 +213,8 @@
 Requires-Dist: spacy==3.7.1
 Requires-Dist: unidecode==1.3.7
 Requires-Dist: matplotlib==3.7.0
 Requires-Dist: pandas==2.1.1
 Requires-Dist: numpy==1.26.0
 Requires-Dist: seaborn==0.13.0
 Requires-Dist: scikit-learn==1.3.1
-Requires-Dist: mlflow==2.12.1
+Requires-Dist: mlflow==2.12.2
```

### Comparing `medroom_ai_dataengineer-0.0.5/README.md` & `medroom_ai_dataengineer-0.0.6/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 # MedRoom.AI.DataEngineer
 
-O `MedRoom.AI.DataEngineer` é um pacote que encapsula funções comuns e genéricas, proporcionando uma solução padronizada para o pré-processamento de texto e avaliação de modelos de Machine Learning.
+O `MedRoom.AI.DataEngineer` é um pacote que encapsula funções comuns e genéricas, proporcionando uma solução padronizada para o pré-processamento de texto, avaliação de modelos de Machine Learning e interação com MLFlow.
 
 ## :arrow_down: Instalação
 
 #### Instalar o Pacote
 ```bash
-!pip install MedRoom.AI.DataEngineer==0.0.4
+!pip install MedRoom.AI.DataEngineer==0.0.5
 ```
 
 ## :book: Uso 
 
-### :one: Pré-processamento de Texto 
+## :one: Pré-processamento de Texto 
 
 #### Importar Bibliotecas Necessárias
 ```python
 import nltk
 import spacy
 
 nltk.download('punkt')
@@ -36,15 +36,15 @@
 
 text = "1- Exemplo de código para pré-processamento de texto. Atenção, o boris vai te pegar se você não usar as libs que importar!"
 
 processed_text = x.preprocess_text(text)
 print(processed_text)
 ```
 
-### :two: Avaliação de Modelos de Machine Learning
+## :two: Avaliação de Modelos de Machine Learning
 
 #### Importar e Usar a Classe de Avaliação
 ```python
 from medroom.dna.processors.utils.evalmetrics import ModelEvaluator
 
 # Suponha que `predictions` e `y_test` são suas predições e rótulos reais, respectivamente.
 evalmetrics = ModelEvaluator()
@@ -105,14 +105,46 @@
   display(Image(confusion_matrix_img.getvalue()))
   ```
 
   Matriz normalizada
   ```python
   normalized_confusion_matrix
   ```
+## 3️⃣ Utilitários de MLFlow
+
+O arquivo `mlflow_helper.py` fornece uma interface simplificada para interagir com o MLflow, permitindo a criação e gerenciamento de experimentos, assim como o registro de parâmetros, métricas e artefatos de forma estruturada. 
+
+### :wrench: Funcionalidades
+
+- **Criação ou recuperação de experimentos**: Automatiza a verificação e criação de experimentos no MLflow.
+- **Registro de dados de corridas**: Permite o registro fácil de parâmetros, métricas, tags e artefatos.
+- **Manipulação de artefatos**: Inclui manipuladores específicos para diferentes tipos de artefatos como imagens, modelos e DataFrames.
+
+### :arrow_down: Como Usar
+
+#### Configuração Inicial
+
+```python
+from medroom.dna.processors.utils.mlflow_helper import MLFlowHelper
+```
+
+#### Configurar a URL do servidor e o nome do experimento
+```python
+helper = MLFlowHelper("http://ai-mlflow", "MedEmotions")
+```
+
+#### Carregar dados consolidados (Arquivo Pickle)
+```python
+consolidated_data = helper.load_data_pickle("dados_run.pkl")
+```
+
+#### Registrar todos os componentes: parâmetros, métricas, tags e artefatos
+```python
+helper.log_run(consolidated_data)
+```
   
 ## :notebook: Tutorial Interativo
 
 Para um aprendizado mais prático e interativo, oferecemos um tutorial em formato de Jupyter Notebook. Ele guia você através do uso prático das classes e funções disponíveis no `MedRoom.AI.DataEngineer`, abrangendo desde o pré-processamento de texto até a avaliação do modelo.
 
 - [Acesse o Tutorial Interativo](https://github.com/MedRoomGitHub/MedRoom.AI.Notebooks/blob/develop/Tutoriais/Sprint11_MedRoomAIDataEngineer.ipynb)
 
@@ -172,9 +204,9 @@
    twine upload dist/*
    ```
    Nota: Para fazer o upload no PyPI, é necessário fornecer um nome de usuário e senha. Se você tiver a autenticação de dois fatores (2FA) ativada para sua conta no PyPI, precisará usar um Token de API em vez de sua senha habitual. Para mais detalhes sobre as credenciais e outras informações relacionadas, consulte nossa [documentação no Notion](https://www.notion.so/MedRoom-AI-DataEngineer-5d3ea0613d0b411795496fbc8319fa09).
 
 ### 4. **Instalação a partir do PyPI**:
    Depois de publicar seu pacote no PyPI, ele pode ser instalado em qualquer ambiente usando:
    ```bash
-   !pip install MedRoom.AI.DataEngineer====0.0.4
+   !pip install MedRoom.AI.DataEngineer====0.0.5
    ```
```

### Comparing `medroom_ai_dataengineer-0.0.5/medroom/dna/processors/config.py` & `medroom_ai_dataengineer-0.0.6/medroom/dna/processors/config.py`

 * *Files identical despite different names*

### Comparing `medroom_ai_dataengineer-0.0.5/medroom/dna/processors/main.py` & `medroom_ai_dataengineer-0.0.6/medroom/dna/processors/main.py`

 * *Files identical despite different names*

### Comparing `medroom_ai_dataengineer-0.0.5/medroom/dna/processors/utils/evalmetrics.py` & `medroom_ai_dataengineer-0.0.6/medroom/dna/processors/utils/evalmetrics.py`

 * *Files identical despite different names*

### Comparing `medroom_ai_dataengineer-0.0.5/medroom/dna/processors/utils/mlflow_helper.py` & `medroom_ai_dataengineer-0.0.6/medroom/dna/processors/utils/mlflow_helper.py`

 * *Files identical despite different names*

### Comparing `medroom_ai_dataengineer-0.0.5/medroom/dna/processors/utils/textclean.py` & `medroom_ai_dataengineer-0.0.6/medroom/dna/processors/utils/textclean.py`

 * *Files identical despite different names*

### Comparing `medroom_ai_dataengineer-0.0.5/setup.py` & `medroom_ai_dataengineer-0.0.6/setup.py`

 * *Files identical despite different names*

