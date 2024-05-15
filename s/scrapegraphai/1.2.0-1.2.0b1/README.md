# Comparing `tmp/scrapegraphai-1.2.0.tar.gz` & `tmp/scrapegraphai-1.2.0b1.tar.gz`

## Comparing `scrapegraphai-1.2.0.tar` & `scrapegraphai-1.2.0b1.tar`

### file list

```diff
@@ -1,258 +1,258 @@
--rw-r--r--   0        0        0       66 2020-02-02 00:00:00.000000 scrapegraphai-1.2.0/.gitattributes
--rw-r--r--   0        0        0     1403 2020-02-02 00:00:00.000000 scrapegraphai-1.2.0/.releaserc.yml
--rw-r--r--   0        0        0    41033 2020-02-02 00:00:00.000000 scrapegraphai-1.2.0/CHANGELOG.md
--rw-r--r--   0        0        0     5221 2020-02-02 00:00:00.000000 scrapegraphai-1.2.0/CODE_OF_CONDUCT.md
--rw-r--r--   0        0        0     3496 2020-02-02 00:00:00.000000 scrapegraphai-1.2.0/CONTRIBUTING.md
--rw-r--r--   0        0        0      138 2020-02-02 00:00:00.000000 scrapegraphai-1.2.0/Dockerfile
--rw-r--r--   0        0        0      117 2020-02-02 00:00:00.000000 scrapegraphai-1.2.0/SECURITY.md
--rw-r--r--   0        0        0      398 2020-02-02 00:00:00.000000 scrapegraphai-1.2.0/citation.cff
--rw-r--r--   0        0        0      224 2020-02-02 00:00:00.000000 scrapegraphai-1.2.0/docker-compose.yml
--rw-r--r--   0        0        0     9317 2020-02-02 00:00:00.000000 scrapegraphai-1.2.0/html_structure
--rw-r--r--   0        0        0   494652 2020-02-02 00:00:00.000000 scrapegraphai-1.2.0/html_structure.png
--rw-r--r--   0        0        0      587 2020-02-02 00:00:00.000000 scrapegraphai-1.2.0/readthedocs.yml
--rw-r--r--   0        0        0       56 2020-02-02 00:00:00.000000 scrapegraphai-1.2.0/requirements-dev.txt
--rw-r--r--   0        0        0      426 2020-02-02 00:00:00.000000 scrapegraphai-1.2.0/requirements.txt
--rw-r--r--   0        0        0      834 2020-02-02 00:00:00.000000 scrapegraphai-1.2.0/.github/ISSUE_TEMPLATE/bug_report.md
--rw-r--r--   0        0        0      126 2020-02-02 00:00:00.000000 scrapegraphai-1.2.0/.github/ISSUE_TEMPLATE/custom.md
--rw-r--r--   0        0        0      595 2020-02-02 00:00:00.000000 scrapegraphai-1.2.0/.github/ISSUE_TEMPLATE/feature_request.md
--rw-r--r--   0        0        0     2593 2020-02-02 00:00:00.000000 scrapegraphai-1.2.0/.github/workflows/codeql.yml
--rw-r--r--   0        0        0     1729 2020-02-02 00:00:00.000000 scrapegraphai-1.2.0/.github/workflows/dependency-review.yml
--rw-r--r--   0        0        0     1067 2020-02-02 00:00:00.000000 scrapegraphai-1.2.0/.github/workflows/pylint.yml
--rw-r--r--   0        0        0      877 2020-02-02 00:00:00.000000 scrapegraphai-1.2.0/.github/workflows/python-publish.yml
--rw-r--r--   0        0        0     2360 2020-02-02 00:00:00.000000 scrapegraphai-1.2.0/.github/workflows/release.yml
--rw-r--r--   0        0        0      638 2020-02-02 00:00:00.000000 scrapegraphai-1.2.0/docs/Makefile
--rw-r--r--   0        0        0     2546 2020-02-02 00:00:00.000000 scrapegraphai-1.2.0/docs/README.md
--rw-r--r--   0        0        0      769 2020-02-02 00:00:00.000000 scrapegraphai-1.2.0/docs/make.bat
--rw-r--r--   0        0        0    60520 2020-02-02 00:00:00.000000 scrapegraphai-1.2.0/docs/assets/apikey_1.png
--rw-r--r--   0        0        0   123826 2020-02-02 00:00:00.000000 scrapegraphai-1.2.0/docs/assets/apikey_2.png
--rw-r--r--   0        0        0    60775 2020-02-02 00:00:00.000000 scrapegraphai-1.2.0/docs/assets/apikey_3.png
--rw-r--r--   0        0        0    86914 2020-02-02 00:00:00.000000 scrapegraphai-1.2.0/docs/assets/apikey_4.png
--rw-r--r--   0        0        0     3526 2020-02-02 00:00:00.000000 scrapegraphai-1.2.0/docs/assets/codespaces-badge.png
--rw-r--r--   0        0        0  1178826 2020-02-02 00:00:00.000000 scrapegraphai-1.2.0/docs/assets/logo_authors.png
--rw-r--r--   0        0        0    73949 2020-02-02 00:00:00.000000 scrapegraphai-1.2.0/docs/assets/omniscrapergraph.png
--rw-r--r--   0        0        0    58062 2020-02-02 00:00:00.000000 scrapegraphai-1.2.0/docs/assets/omnisearchgraph.png
--rw-r--r--   0        0        0    53007 2020-02-02 00:00:00.000000 scrapegraphai-1.2.0/docs/assets/project_overview_diagram.fig
--rw-r--r--   0        0        0    83949 2020-02-02 00:00:00.000000 scrapegraphai-1.2.0/docs/assets/project_overview_diagram.png
--rw-r--r--   0        0        0    33264 2020-02-02 00:00:00.000000 scrapegraphai-1.2.0/docs/assets/scrapegraphai_logo.png
--rw-r--r--   0        0        0    54611 2020-02-02 00:00:00.000000 scrapegraphai-1.2.0/docs/assets/searchgraph.png
--rw-r--r--   0        0        0    15508 2020-02-02 00:00:00.000000 scrapegraphai-1.2.0/docs/assets/serp_api_logo.png
--rw-r--r--   0        0        0    61095 2020-02-02 00:00:00.000000 scrapegraphai-1.2.0/docs/assets/smartscrapergraph.png
--rw-r--r--   0        0        0    49312 2020-02-02 00:00:00.000000 scrapegraphai-1.2.0/docs/assets/speechgraph.png
--rw-r--r--   0        0        0     1737 2020-02-02 00:00:00.000000 scrapegraphai-1.2.0/docs/source/conf.py
--rw-r--r--   0        0        0      753 2020-02-02 00:00:00.000000 scrapegraphai-1.2.0/docs/source/index.rst
--rw-r--r--   0        0        0     2843 2020-02-02 00:00:00.000000 scrapegraphai-1.2.0/docs/source/getting_started/examples.rst
--rw-r--r--   0        0        0     1213 2020-02-02 00:00:00.000000 scrapegraphai-1.2.0/docs/source/getting_started/installation.rst
--rw-r--r--   0        0        0      523 2020-02-02 00:00:00.000000 scrapegraphai-1.2.0/docs/source/introduction/contributing.rst
--rw-r--r--   0        0        0     1689 2020-02-02 00:00:00.000000 scrapegraphai-1.2.0/docs/source/introduction/overview.rst
--rw-r--r--   0        0        0       47 2020-02-02 00:00:00.000000 scrapegraphai-1.2.0/docs/source/modules/modules.rst
--rw-r--r--   0        0        0      603 2020-02-02 00:00:00.000000 scrapegraphai-1.2.0/docs/source/modules/scrapegraphai.graphs.rst
--rw-r--r--   0        0        0     1410 2020-02-02 00:00:00.000000 scrapegraphai-1.2.0/docs/source/modules/scrapegraphai.nodes.rst
--rw-r--r--   0        0        0     2137 2020-02-02 00:00:00.000000 scrapegraphai-1.2.0/docs/source/modules/scrapegraphai.rst
--rw-r--r--   0        0        0      532 2020-02-02 00:00:00.000000 scrapegraphai-1.2.0/docs/source/scrapers/benchmarks.rst
--rw-r--r--   0        0        0     1868 2020-02-02 00:00:00.000000 scrapegraphai-1.2.0/docs/source/scrapers/graph_config.rst
--rw-r--r--   0        0        0     5646 2020-02-02 00:00:00.000000 scrapegraphai-1.2.0/docs/source/scrapers/graphs.rst
--rw-r--r--   0        0        0     5568 2020-02-02 00:00:00.000000 scrapegraphai-1.2.0/docs/source/scrapers/llm.rst
--rw-r--r--   0        0        0     4500 2020-02-02 00:00:00.000000 scrapegraphai-1.2.0/examples/custom_graph_domtree.py
--rw-r--r--   0        0        0     4011 2020-02-02 00:00:00.000000 scrapegraphai-1.2.0/examples/domtree_example.py
--rw-r--r--   0        0        0     1032 2020-02-02 00:00:00.000000 scrapegraphai-1.2.0/examples/faiss_vector.py
--rw-r--r--   0        0        0     2360 2020-02-02 00:00:00.000000 scrapegraphai-1.2.0/examples/readme.md
--rw-r--r--   0        0        0     2051 2020-02-02 00:00:00.000000 scrapegraphai-1.2.0/examples/anthropic/smart_scraper_haiku.py
--rw-r--r--   0        0        0     2053 2020-02-02 00:00:00.000000 scrapegraphai-1.2.0/examples/azure/json_scraper_azure.py
--rw-r--r--   0        0        0     1929 2020-02-02 00:00:00.000000 scrapegraphai-1.2.0/examples/azure/search_graph_azure.py
--rw-r--r--   0        0        0     2164 2020-02-02 00:00:00.000000 scrapegraphai-1.2.0/examples/azure/smart_scraper_azure_openai.py
--rw-r--r--   0        0        0     2047 2020-02-02 00:00:00.000000 scrapegraphai-1.2.0/examples/azure/xml_scraper_azure.py
--rw-r--r--   0        0        0     4429 2020-02-02 00:00:00.000000 scrapegraphai-1.2.0/examples/azure/inputs/books.xml
--rw-r--r--   0        0        0     6455 2020-02-02 00:00:00.000000 scrapegraphai-1.2.0/examples/azure/inputs/example.json
--rw-r--r--   0        0        0      176 2020-02-02 00:00:00.000000 scrapegraphai-1.2.0/examples/azure/inputs/username.csv
--rw-r--r--   0        0        0      897 2020-02-02 00:00:00.000000 scrapegraphai-1.2.0/examples/bedrock/smart_scraper_bedrock.py
--rw-r--r--   0        0        0      265 2020-02-02 00:00:00.000000 scrapegraphai-1.2.0/examples/benchmarks/readme.md
--rw-r--r--   0        0        0       36 2020-02-02 00:00:00.000000 scrapegraphai-1.2.0/examples/benchmarks/GenerateScraper/.env.example
--rw-r--r--   0        0        0     2888 2020-02-02 00:00:00.000000 scrapegraphai-1.2.0/examples/benchmarks/GenerateScraper/Readme.md
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 scrapegraphai-1.2.0/examples/benchmarks/GenerateScraper/benchmark_docker.py
--rw-r--r--   0        0        0     1773 2020-02-02 00:00:00.000000 scrapegraphai-1.2.0/examples/benchmarks/GenerateScraper/benchmark_groq.py
--rw-r--r--   0        0        0     1770 2020-02-02 00:00:00.000000 scrapegraphai-1.2.0/examples/benchmarks/GenerateScraper/benchmark_llama3.py
--rw-r--r--   0        0        0     1862 2020-02-02 00:00:00.000000 scrapegraphai-1.2.0/examples/benchmarks/GenerateScraper/benchmark_mistral.py
--rw-r--r--   0        0        0     1554 2020-02-02 00:00:00.000000 scrapegraphai-1.2.0/examples/benchmarks/GenerateScraper/benchmark_openai_gpt35.py
--rw-r--r--   0        0        0     1563 2020-02-02 00:00:00.000000 scrapegraphai-1.2.0/examples/benchmarks/GenerateScraper/benchmark_openai_gpt4.py
--rw-r--r--   0        0        0     7305 2020-02-02 00:00:00.000000 scrapegraphai-1.2.0/examples/benchmarks/GenerateScraper/inputs/example_1.txt
--rw-r--r--   0        0        0  2590773 2020-02-02 00:00:00.000000 scrapegraphai-1.2.0/examples/benchmarks/GenerateScraper/inputs/example_2.txt
--rw-r--r--   0        0        0       36 2020-02-02 00:00:00.000000 scrapegraphai-1.2.0/examples/benchmarks/SmartScraper/.env.example
--rw-r--r--   0        0        0     2914 2020-02-02 00:00:00.000000 scrapegraphai-1.2.0/examples/benchmarks/SmartScraper/Readme.md
--rw-r--r--   0        0        0     1539 2020-02-02 00:00:00.000000 scrapegraphai-1.2.0/examples/benchmarks/SmartScraper/benchmark_docker.py
--rw-r--r--   0        0        0     1615 2020-02-02 00:00:00.000000 scrapegraphai-1.2.0/examples/benchmarks/SmartScraper/benchmark_groq.py
--rw-r--r--   0        0        0     1630 2020-02-02 00:00:00.000000 scrapegraphai-1.2.0/examples/benchmarks/SmartScraper/benchmark_llama3.py
--rw-r--r--   0        0        0     1641 2020-02-02 00:00:00.000000 scrapegraphai-1.2.0/examples/benchmarks/SmartScraper/benchmark_mistral.py
--rw-r--r--   0        0        0     1520 2020-02-02 00:00:00.000000 scrapegraphai-1.2.0/examples/benchmarks/SmartScraper/benchmark_openai_gpt35.py
--rw-r--r--   0        0        0     1519 2020-02-02 00:00:00.000000 scrapegraphai-1.2.0/examples/benchmarks/SmartScraper/benchmark_openai_gpt4.py
--rw-r--r--   0        0        0     7305 2020-02-02 00:00:00.000000 scrapegraphai-1.2.0/examples/benchmarks/SmartScraper/inputs/example_1.txt
--rw-r--r--   0        0        0  2590773 2020-02-02 00:00:00.000000 scrapegraphai-1.2.0/examples/benchmarks/SmartScraper/inputs/example_2.txt
--rw-r--r--   0        0        0       35 2020-02-02 00:00:00.000000 scrapegraphai-1.2.0/examples/deepseek/.env.example
--rw-r--r--   0        0        0     1665 2020-02-02 00:00:00.000000 scrapegraphai-1.2.0/examples/deepseek/csv_scraper_deepseek.py
--rw-r--r--   0        0        0     1723 2020-02-02 00:00:00.000000 scrapegraphai-1.2.0/examples/deepseek/json_scraper_deepseek.py
--rw-r--r--   0        0        0     1309 2020-02-02 00:00:00.000000 scrapegraphai-1.2.0/examples/deepseek/script_generator_deepseek.py
--rw-r--r--   0        0        0     1238 2020-02-02 00:00:00.000000 scrapegraphai-1.2.0/examples/deepseek/search_graph_deepseek.py
--rw-r--r--   0        0        0     1289 2020-02-02 00:00:00.000000 scrapegraphai-1.2.0/examples/deepseek/smart_scarper_deepseek.py
--rw-r--r--   0        0        0     1714 2020-02-02 00:00:00.000000 scrapegraphai-1.2.0/examples/deepseek/xml_scraper_deepseek.py
--rw-r--r--   0        0        0     4429 2020-02-02 00:00:00.000000 scrapegraphai-1.2.0/examples/deepseek/inputs/books.xml
--rw-r--r--   0        0        0     6455 2020-02-02 00:00:00.000000 scrapegraphai-1.2.0/examples/deepseek/inputs/example.json
--rw-r--r--   0        0        0      176 2020-02-02 00:00:00.000000 scrapegraphai-1.2.0/examples/deepseek/inputs/username.csv
--rw-r--r--   0        0        0       36 2020-02-02 00:00:00.000000 scrapegraphai-1.2.0/examples/gemini/.env.example
--rw-r--r--   0        0        0     1447 2020-02-02 00:00:00.000000 scrapegraphai-1.2.0/examples/gemini/csv_scraper_gemini.py
--rw-r--r--   0        0        0     2120 2020-02-02 00:00:00.000000 scrapegraphai-1.2.0/examples/gemini/custom_graph_gemini.py
--rw-r--r--   0        0        0     1629 2020-02-02 00:00:00.000000 scrapegraphai-1.2.0/examples/gemini/json_scraper_gemini.py
--rw-r--r--   0        0        0      211 2020-02-02 00:00:00.000000 scrapegraphai-1.2.0/examples/gemini/readme.md
--rw-r--r--   0        0        0     1556 2020-02-02 00:00:00.000000 scrapegraphai-1.2.0/examples/gemini/scrape_plain_text_gemini.py
--rw-r--r--   0        0        0     1557 2020-02-02 00:00:00.000000 scrapegraphai-1.2.0/examples/gemini/scrape_xml_gemini.py
--rw-r--r--   0        0        0     1230 2020-02-02 00:00:00.000000 scrapegraphai-1.2.0/examples/gemini/script_generator_gemini.py
--rw-r--r--   0        0        0      964 2020-02-02 00:00:00.000000 scrapegraphai-1.2.0/examples/gemini/search_graph_gemini.py
--rw-r--r--   0        0        0     1175 2020-02-02 00:00:00.000000 scrapegraphai-1.2.0/examples/gemini/smart_scraper_gemini.py
--rw-r--r--   0        0        0     1617 2020-02-02 00:00:00.000000 scrapegraphai-1.2.0/examples/gemini/xml_scraper_openai.py
--rw-r--r--   0        0        0     4429 2020-02-02 00:00:00.000000 scrapegraphai-1.2.0/examples/gemini/inputs/books.xml
--rw-r--r--   0        0        0     6455 2020-02-02 00:00:00.000000 scrapegraphai-1.2.0/examples/gemini/inputs/example.json
--rw-r--r--   0        0        0     7305 2020-02-02 00:00:00.000000 scrapegraphai-1.2.0/examples/gemini/inputs/plain_html_example.txt
--rw-r--r--   0        0        0      176 2020-02-02 00:00:00.000000 scrapegraphai-1.2.0/examples/gemini/inputs/username.csv
--rw-r--r--   0        0        0       64 2020-02-02 00:00:00.000000 scrapegraphai-1.2.0/examples/groq/.env.example
--rw-r--r--   0        0        0     1054 2020-02-02 00:00:00.000000 scrapegraphai-1.2.0/examples/groq/search_graph_groq_openai.py
--rw-r--r--   0        0        0     1414 2020-02-02 00:00:00.000000 scrapegraphai-1.2.0/examples/groq/smart_scraper_groq_ollama.py
--rw-r--r--   0        0        0     1366 2020-02-02 00:00:00.000000 scrapegraphai-1.2.0/examples/groq/smart_scraper_groq_openai.py
--rw-r--r--   0        0        0     2062 2020-02-02 00:00:00.000000 scrapegraphai-1.2.0/examples/huggingfacehub/smart_scraper_huggingfacehub.py
--rw-r--r--   0        0        0     1838 2020-02-02 00:00:00.000000 scrapegraphai-1.2.0/examples/local_models/csv_scraper_ollama.py
--rw-r--r--   0        0        0     1942 2020-02-02 00:00:00.000000 scrapegraphai-1.2.0/examples/local_models/json_scraper_ollama.py
--rw-r--r--   0        0        0     1752 2020-02-02 00:00:00.000000 scrapegraphai-1.2.0/examples/local_models/scrape_plain_text_ollama.py
--rw-r--r--   0        0        0     1832 2020-02-02 00:00:00.000000 scrapegraphai-1.2.0/examples/local_models/scrape_xml_ollama.py
--rw-r--r--   0        0        0     1465 2020-02-02 00:00:00.000000 scrapegraphai-1.2.0/examples/local_models/script_generator_ollama.py
--rw-r--r--   0        0        0     1401 2020-02-02 00:00:00.000000 scrapegraphai-1.2.0/examples/local_models/search_graph_ollama.py
--rw-r--r--   0        0        0     1407 2020-02-02 00:00:00.000000 scrapegraphai-1.2.0/examples/local_models/smart_scraper_ollama.py
--rw-r--r--   0        0        0     1929 2020-02-02 00:00:00.000000 scrapegraphai-1.2.0/examples/local_models/xml_scraper_ollama.py
--rw-r--r--   0        0        0     4429 2020-02-02 00:00:00.000000 scrapegraphai-1.2.0/examples/local_models/inputs/books.xml
--rw-r--r--   0        0        0     6455 2020-02-02 00:00:00.000000 scrapegraphai-1.2.0/examples/local_models/inputs/example.json
--rw-r--r--   0        0        0     7305 2020-02-02 00:00:00.000000 scrapegraphai-1.2.0/examples/local_models/inputs/plain_html_example.txt
--rw-r--r--   0        0        0      176 2020-02-02 00:00:00.000000 scrapegraphai-1.2.0/examples/local_models/inputs/username.csv
--rw-r--r--   0        0        0      208 2020-02-02 00:00:00.000000 scrapegraphai-1.2.0/examples/mixed_models/.env.example
--rw-r--r--   0        0        0      201 2020-02-02 00:00:00.000000 scrapegraphai-1.2.0/examples/mixed_models/readme.md
--rw-r--r--   0        0        0     1357 2020-02-02 00:00:00.000000 scrapegraphai-1.2.0/examples/mixed_models/search_graph_groq_ollama.py
--rw-r--r--   0        0        0     1448 2020-02-02 00:00:00.000000 scrapegraphai-1.2.0/examples/mixed_models/smart_scraper_mixed.py
--rw-r--r--   0        0        0     4429 2020-02-02 00:00:00.000000 scrapegraphai-1.2.0/examples/mixed_models/inputs/books.xml
--rw-r--r--   0        0        0     6455 2020-02-02 00:00:00.000000 scrapegraphai-1.2.0/examples/mixed_models/inputs/example.json
--rw-r--r--   0        0        0     7305 2020-02-02 00:00:00.000000 scrapegraphai-1.2.0/examples/mixed_models/inputs/plain_html_example.txt
--rw-r--r--   0        0        0       39 2020-02-02 00:00:00.000000 scrapegraphai-1.2.0/examples/openai/.env.example
--rw-r--r--   0        0        0     1574 2020-02-02 00:00:00.000000 scrapegraphai-1.2.0/examples/openai/csv_scraper_openai.py
--rw-r--r--   0        0        0     2688 2020-02-02 00:00:00.000000 scrapegraphai-1.2.0/examples/openai/custom_graph_openai.py
--rw-r--r--   0        0        0     1321 2020-02-02 00:00:00.000000 scrapegraphai-1.2.0/examples/openai/deep_scraper_openai.py
--rw-r--r--   0        0        0     1633 2020-02-02 00:00:00.000000 scrapegraphai-1.2.0/examples/openai/json_scraper_openai.py
--rw-r--r--   0        0        0     1307 2020-02-02 00:00:00.000000 scrapegraphai-1.2.0/examples/openai/omni_scraper_openai.py
--rw-r--r--   0        0        0     1142 2020-02-02 00:00:00.000000 scrapegraphai-1.2.0/examples/openai/omni_search_graph_openai.py
--rw-r--r--   0        0        0      203 2020-02-02 00:00:00.000000 scrapegraphai-1.2.0/examples/openai/readme.md
--rw-r--r--   0        0        0     1512 2020-02-02 00:00:00.000000 scrapegraphai-1.2.0/examples/openai/scrape_plain_text_openai.py
--rw-r--r--   0        0        0     1239 2020-02-02 00:00:00.000000 scrapegraphai-1.2.0/examples/openai/script_generator_openai.py
--rw-r--r--   0        0        0     1160 2020-02-02 00:00:00.000000 scrapegraphai-1.2.0/examples/openai/search_graph_openai.py
--rw-r--r--   0        0        0     1233 2020-02-02 00:00:00.000000 scrapegraphai-1.2.0/examples/openai/smart_scraper_openai.py
--rw-r--r--   0        0        0     1531 2020-02-02 00:00:00.000000 scrapegraphai-1.2.0/examples/openai/speech_graph_openai.py
--rw-r--r--   0        0        0     1642 2020-02-02 00:00:00.000000 scrapegraphai-1.2.0/examples/openai/xml_scraper_openai.py
--rw-r--r--   0        0        0     4429 2020-02-02 00:00:00.000000 scrapegraphai-1.2.0/examples/openai/inputs/books.xml
--rw-r--r--   0        0        0     6455 2020-02-02 00:00:00.000000 scrapegraphai-1.2.0/examples/openai/inputs/example.json
--rw-r--r--   0        0        0     7305 2020-02-02 00:00:00.000000 scrapegraphai-1.2.0/examples/openai/inputs/plain_html_example.txt
--rw-r--r--   0        0        0      176 2020-02-02 00:00:00.000000 scrapegraphai-1.2.0/examples/openai/inputs/username.csv
--rw-r--r--   0        0        0      567 2020-02-02 00:00:00.000000 scrapegraphai-1.2.0/examples/single_node/fetch_node.py
--rw-r--r--   0        0        0     1199 2020-02-02 00:00:00.000000 scrapegraphai-1.2.0/examples/single_node/image2text_node.py
--rw-r--r--   0        0        0      961 2020-02-02 00:00:00.000000 scrapegraphai-1.2.0/examples/single_node/robot_node.py
--rwxr-xr-x   0        0        0      986 2020-02-02 00:00:00.000000 scrapegraphai-1.2.0/manual deployment/commit_and_push.sh
--rwxr-xr-x   0        0        0      611 2020-02-02 00:00:00.000000 scrapegraphai-1.2.0/manual deployment/commit_and_push_with_tests.sh
--rwxr-xr-x   0        0        0      169 2020-02-02 00:00:00.000000 scrapegraphai-1.2.0/manual deployment/deploy_on_pip.sh
--rw-r--r--   0        0        0       90 2020-02-02 00:00:00.000000 scrapegraphai-1.2.0/manual deployment/rye_update.sh
--rw-r--r--   0        0        0       54 2020-02-02 00:00:00.000000 scrapegraphai-1.2.0/scrapegraphai/__init__.py
--rw-r--r--   0        0        0       77 2020-02-02 00:00:00.000000 scrapegraphai-1.2.0/scrapegraphai/asdt/__init__.py
--rw-r--r--   0        0        0     2009 2020-02-02 00:00:00.000000 scrapegraphai-1.2.0/scrapegraphai/asdt/dom_tree.py
--rw-r--r--   0        0        0     3658 2020-02-02 00:00:00.000000 scrapegraphai-1.2.0/scrapegraphai/asdt/tree.py
--rw-r--r--   0        0        0     4395 2020-02-02 00:00:00.000000 scrapegraphai-1.2.0/scrapegraphai/asdt/tree_node.py
--rw-r--r--   0        0        0       90 2020-02-02 00:00:00.000000 scrapegraphai-1.2.0/scrapegraphai/builders/__init__.py
--rw-r--r--   0        0        0     6653 2020-02-02 00:00:00.000000 scrapegraphai-1.2.0/scrapegraphai/builders/graph_builder.py
--rw-r--r--   0        0        0       83 2020-02-02 00:00:00.000000 scrapegraphai-1.2.0/scrapegraphai/docloaders/__init__.py
--rw-r--r--   0        0        0     4498 2020-02-02 00:00:00.000000 scrapegraphai-1.2.0/scrapegraphai/docloaders/chromium.py
--rw-r--r--   0        0        0      681 2020-02-02 00:00:00.000000 scrapegraphai-1.2.0/scrapegraphai/graphs/__init__.py
--rw-r--r--   0        0        0    13691 2020-02-02 00:00:00.000000 scrapegraphai-1.2.0/scrapegraphai/graphs/abstract_graph.py
--rw-r--r--   0        0        0     5378 2020-02-02 00:00:00.000000 scrapegraphai-1.2.0/scrapegraphai/graphs/base_graph.py
--rw-r--r--   0        0        0     2472 2020-02-02 00:00:00.000000 scrapegraphai-1.2.0/scrapegraphai/graphs/csv_scraper_graph.py
--rw-r--r--   0        0        0     3777 2020-02-02 00:00:00.000000 scrapegraphai-1.2.0/scrapegraphai/graphs/deep_scraper_graph.py
--rw-r--r--   0        0        0     3392 2020-02-02 00:00:00.000000 scrapegraphai-1.2.0/scrapegraphai/graphs/json_scraper_graph.py
--rw-r--r--   0        0        0     4295 2020-02-02 00:00:00.000000 scrapegraphai-1.2.0/scrapegraphai/graphs/omni_scraper_graph.py
--rw-r--r--   0        0        0     3714 2020-02-02 00:00:00.000000 scrapegraphai-1.2.0/scrapegraphai/graphs/omni_search_graph.py
--rw-r--r--   0        0        0     3538 2020-02-02 00:00:00.000000 scrapegraphai-1.2.0/scrapegraphai/graphs/pdf_scraper_graph.py
--rw-r--r--   0        0        0     3371 2020-02-02 00:00:00.000000 scrapegraphai-1.2.0/scrapegraphai/graphs/script_creator_graph.py
--rw-r--r--   0        0        0     3638 2020-02-02 00:00:00.000000 scrapegraphai-1.2.0/scrapegraphai/graphs/search_graph.py
--rw-r--r--   0        0        0     3651 2020-02-02 00:00:00.000000 scrapegraphai-1.2.0/scrapegraphai/graphs/smart_scraper_graph.py
--rw-r--r--   0        0        0     4322 2020-02-02 00:00:00.000000 scrapegraphai-1.2.0/scrapegraphai/graphs/speech_graph.py
--rw-r--r--   0        0        0     4486 2020-02-02 00:00:00.000000 scrapegraphai-1.2.0/scrapegraphai/graphs/turbo_scraper.py
--rw-r--r--   0        0        0     3534 2020-02-02 00:00:00.000000 scrapegraphai-1.2.0/scrapegraphai/graphs/xml_scraper_graph.py
--rw-r--r--   0        0        0      202 2020-02-02 00:00:00.000000 scrapegraphai-1.2.0/scrapegraphai/helpers/__init__.py
--rw-r--r--   0        0        0     4203 2020-02-02 00:00:00.000000 scrapegraphai-1.2.0/scrapegraphai/helpers/models_tokens.py
--rw-r--r--   0        0        0     3807 2020-02-02 00:00:00.000000 scrapegraphai-1.2.0/scrapegraphai/helpers/nodes_metadata.py
--rw-r--r--   0        0        0      310 2020-02-02 00:00:00.000000 scrapegraphai-1.2.0/scrapegraphai/helpers/robots.py
--rw-r--r--   0        0        0     2363 2020-02-02 00:00:00.000000 scrapegraphai-1.2.0/scrapegraphai/helpers/schemas.py
--rw-r--r--   0        0        0      406 2020-02-02 00:00:00.000000 scrapegraphai-1.2.0/scrapegraphai/models/__init__.py
--rw-r--r--   0        0        0      429 2020-02-02 00:00:00.000000 scrapegraphai-1.2.0/scrapegraphai/models/anthropic.py
--rw-r--r--   0        0        0      441 2020-02-02 00:00:00.000000 scrapegraphai-1.2.0/scrapegraphai/models/azure_openai.py
--rw-r--r--   0        0        0      579 2020-02-02 00:00:00.000000 scrapegraphai-1.2.0/scrapegraphai/models/bedrock.py
--rw-r--r--   0        0        0      455 2020-02-02 00:00:00.000000 scrapegraphai-1.2.0/scrapegraphai/models/deepseek.py
--rw-r--r--   0        0        0      606 2020-02-02 00:00:00.000000 scrapegraphai-1.2.0/scrapegraphai/models/gemini.py
--rw-r--r--   0        0        0      426 2020-02-02 00:00:00.000000 scrapegraphai-1.2.0/scrapegraphai/models/groq.py
--rw-r--r--   0        0        0      459 2020-02-02 00:00:00.000000 scrapegraphai-1.2.0/scrapegraphai/models/hugging_face.py
--rw-r--r--   0        0        0      427 2020-02-02 00:00:00.000000 scrapegraphai-1.2.0/scrapegraphai/models/ollama.py
--rw-r--r--   0        0        0      412 2020-02-02 00:00:00.000000 scrapegraphai-1.2.0/scrapegraphai/models/openai.py
--rw-r--r--   0        0        0     1367 2020-02-02 00:00:00.000000 scrapegraphai-1.2.0/scrapegraphai/models/openai_itt.py
--rw-r--r--   0        0        0     1221 2020-02-02 00:00:00.000000 scrapegraphai-1.2.0/scrapegraphai/models/openai_tts.py
--rw-r--r--   0        0        0      959 2020-02-02 00:00:00.000000 scrapegraphai-1.2.0/scrapegraphai/nodes/__init__.py
--rw-r--r--   0        0        0     8591 2020-02-02 00:00:00.000000 scrapegraphai-1.2.0/scrapegraphai/nodes/base_node.py
--rw-r--r--   0        0        0     2370 2020-02-02 00:00:00.000000 scrapegraphai-1.2.0/scrapegraphai/nodes/blocks_identifier.py
--rw-r--r--   0        0        0     2914 2020-02-02 00:00:00.000000 scrapegraphai-1.2.0/scrapegraphai/nodes/conditional_node.py
--rw-r--r--   0        0        0     6450 2020-02-02 00:00:00.000000 scrapegraphai-1.2.0/scrapegraphai/nodes/fetch_node.py
--rw-r--r--   0        0        0     7182 2020-02-02 00:00:00.000000 scrapegraphai-1.2.0/scrapegraphai/nodes/generate_answer_csv_node.py
--rw-r--r--   0        0        0     6612 2020-02-02 00:00:00.000000 scrapegraphai-1.2.0/scrapegraphai/nodes/generate_answer_node.py
--rw-r--r--   0        0        0     7064 2020-02-02 00:00:00.000000 scrapegraphai-1.2.0/scrapegraphai/nodes/generate_answer_omni_node.py
--rw-r--r--   0        0        0     7158 2020-02-02 00:00:00.000000 scrapegraphai-1.2.0/scrapegraphai/nodes/generate_answer_pdf_node.py
--rw-r--r--   0        0        0     4340 2020-02-02 00:00:00.000000 scrapegraphai-1.2.0/scrapegraphai/nodes/generate_scraper_node.py
--rw-r--r--   0        0        0     3537 2020-02-02 00:00:00.000000 scrapegraphai-1.2.0/scrapegraphai/nodes/get_probable_tags_node.py
--rw-r--r--   0        0        0     4395 2020-02-02 00:00:00.000000 scrapegraphai-1.2.0/scrapegraphai/nodes/graph_iterator_node.py
--rw-r--r--   0        0        0     2671 2020-02-02 00:00:00.000000 scrapegraphai-1.2.0/scrapegraphai/nodes/image_to_text_node.py
--rw-r--r--   0        0        0     3890 2020-02-02 00:00:00.000000 scrapegraphai-1.2.0/scrapegraphai/nodes/merge_answers_node.py
--rw-r--r--   0        0        0     2930 2020-02-02 00:00:00.000000 scrapegraphai-1.2.0/scrapegraphai/nodes/parse_node.py
--rw-r--r--   0        0        0     4496 2020-02-02 00:00:00.000000 scrapegraphai-1.2.0/scrapegraphai/nodes/rag_node.py
--rw-r--r--   0        0        0     6072 2020-02-02 00:00:00.000000 scrapegraphai-1.2.0/scrapegraphai/nodes/robots_node.py
--rw-r--r--   0        0        0     4185 2020-02-02 00:00:00.000000 scrapegraphai-1.2.0/scrapegraphai/nodes/search_internet_node.py
--rw-r--r--   0        0        0     4181 2020-02-02 00:00:00.000000 scrapegraphai-1.2.0/scrapegraphai/nodes/search_link_node.py
--rw-r--r--   0        0        0     4913 2020-02-02 00:00:00.000000 scrapegraphai-1.2.0/scrapegraphai/nodes/search_node_with_context.py
--rw-r--r--   0        0        0     2343 2020-02-02 00:00:00.000000 scrapegraphai-1.2.0/scrapegraphai/nodes/text_to_speech_node.py
--rw-r--r--   0        0        0      424 2020-02-02 00:00:00.000000 scrapegraphai-1.2.0/scrapegraphai/utils/__init__.py
--rw-r--r--   0        0        0     7705 2020-02-02 00:00:00.000000 scrapegraphai-1.2.0/scrapegraphai/utils/aaa.py
--rw-r--r--   0        0        0     5791 2020-02-02 00:00:00.000000 scrapegraphai-1.2.0/scrapegraphai/utils/asdt.py
--rw-r--r--   0        0        0     2330 2020-02-02 00:00:00.000000 scrapegraphai-1.2.0/scrapegraphai/utils/cleanup_html.py
--rw-r--r--   0        0        0     2141 2020-02-02 00:00:00.000000 scrapegraphai-1.2.0/scrapegraphai/utils/convert_to_csv.py
--rw-r--r--   0        0        0     1974 2020-02-02 00:00:00.000000 scrapegraphai-1.2.0/scrapegraphai/utils/convert_to_json.py
--rw-r--r--   0        0        0     4638 2020-02-02 00:00:00.000000 scrapegraphai-1.2.0/scrapegraphai/utils/parse_state_keys.py
--rw-r--r--   0        0        0      764 2020-02-02 00:00:00.000000 scrapegraphai-1.2.0/scrapegraphai/utils/prettify_exec_info.py
--rw-r--r--   0        0        0     6404 2020-02-02 00:00:00.000000 scrapegraphai-1.2.0/scrapegraphai/utils/proxy_rotation.py
--rw-r--r--   0        0        0     2140 2020-02-02 00:00:00.000000 scrapegraphai-1.2.0/scrapegraphai/utils/research_web.py
--rw-r--r--   0        0        0      836 2020-02-02 00:00:00.000000 scrapegraphai-1.2.0/scrapegraphai/utils/save_audio_from_bytes.py
--rw-r--r--   0        0        0     1702 2020-02-02 00:00:00.000000 scrapegraphai-1.2.0/scrapegraphai/utils/sys_dynamic_import.py
--rw-r--r--   0        0        0     1320 2020-02-02 00:00:00.000000 scrapegraphai-1.2.0/scrapegraphai/utils/token_calculator.py
--rw-r--r--   0        0        0     1997 2020-02-02 00:00:00.000000 scrapegraphai-1.2.0/scrapegraphai/utils/tree_base.py
--rw-r--r--   0        0        0      417 2020-02-02 00:00:00.000000 scrapegraphai-1.2.0/tests/Readme.md
--rw-r--r--   0        0        0     1220 2020-02-02 00:00:00.000000 scrapegraphai-1.2.0/tests/graphs/scrape_json_ollama.py
--rw-r--r--   0        0        0     1238 2020-02-02 00:00:00.000000 scrapegraphai-1.2.0/tests/graphs/scrape_plain_text_llama3_test.py
--rw-r--r--   0        0        0     1239 2020-02-02 00:00:00.000000 scrapegraphai-1.2.0/tests/graphs/scrape_plain_text_mistral_test.py
--rw-r--r--   0        0        0     1243 2020-02-02 00:00:00.000000 scrapegraphai-1.2.0/tests/graphs/scrape_xml_ollama_test.py
--rw-r--r--   0        0        0     1223 2020-02-02 00:00:00.000000 scrapegraphai-1.2.0/tests/graphs/script_generator_test.py
--rw-r--r--   0        0        0     1350 2020-02-02 00:00:00.000000 scrapegraphai-1.2.0/tests/graphs/smart_scraper_ollama_test.py
--rw-r--r--   0        0        0     4429 2020-02-02 00:00:00.000000 scrapegraphai-1.2.0/tests/graphs/inputs/books.xml
--rw-r--r--   0        0        0     6455 2020-02-02 00:00:00.000000 scrapegraphai-1.2.0/tests/graphs/inputs/example.json
--rw-r--r--   0        0        0     7305 2020-02-02 00:00:00.000000 scrapegraphai-1.2.0/tests/graphs/inputs/plain_html_example.txt
--rw-r--r--   0        0        0      176 2020-02-02 00:00:00.000000 scrapegraphai-1.2.0/tests/graphs/inputs/username.csv
--rw-r--r--   0        0        0      771 2020-02-02 00:00:00.000000 scrapegraphai-1.2.0/tests/nodes/fetch_node_test.py
--rw-r--r--   0        0        0     1207 2020-02-02 00:00:00.000000 scrapegraphai-1.2.0/tests/nodes/robot_node_test.py
--rw-r--r--   0        0        0     2961 2020-02-02 00:00:00.000000 scrapegraphai-1.2.0/tests/utils/test_proxy_rotation.py
--rw-r--r--   0        0        0     2203 2020-02-02 00:00:00.000000 scrapegraphai-1.2.0/tests/utils/test_sys_dynamic_import.py
--rw-r--r--   0        0        0      448 2020-02-02 00:00:00.000000 scrapegraphai-1.2.0/.gitignore
--rw-r--r--   0        0        0     1065 2020-02-02 00:00:00.000000 scrapegraphai-1.2.0/LICENSE
--rw-r--r--   0        0        0     8967 2020-02-02 00:00:00.000000 scrapegraphai-1.2.0/README.md
--rw-r--r--   0        0        0     2007 2020-02-02 00:00:00.000000 scrapegraphai-1.2.0/pyproject.toml
--rw-r--r--   0        0        0    10486 2020-02-02 00:00:00.000000 scrapegraphai-1.2.0/PKG-INFO
+-rw-r--r--   0        0        0       66 2020-02-02 00:00:00.000000 scrapegraphai-1.2.0b1/.gitattributes
+-rw-r--r--   0        0        0     1403 2020-02-02 00:00:00.000000 scrapegraphai-1.2.0b1/.releaserc.yml
+-rw-r--r--   0        0        0    41047 2020-02-02 00:00:00.000000 scrapegraphai-1.2.0b1/CHANGELOG.md
+-rw-r--r--   0        0        0     5221 2020-02-02 00:00:00.000000 scrapegraphai-1.2.0b1/CODE_OF_CONDUCT.md
+-rw-r--r--   0        0        0     3496 2020-02-02 00:00:00.000000 scrapegraphai-1.2.0b1/CONTRIBUTING.md
+-rw-r--r--   0        0        0      138 2020-02-02 00:00:00.000000 scrapegraphai-1.2.0b1/Dockerfile
+-rw-r--r--   0        0        0      117 2020-02-02 00:00:00.000000 scrapegraphai-1.2.0b1/SECURITY.md
+-rw-r--r--   0        0        0      398 2020-02-02 00:00:00.000000 scrapegraphai-1.2.0b1/citation.cff
+-rw-r--r--   0        0        0      224 2020-02-02 00:00:00.000000 scrapegraphai-1.2.0b1/docker-compose.yml
+-rw-r--r--   0        0        0     9317 2020-02-02 00:00:00.000000 scrapegraphai-1.2.0b1/html_structure
+-rw-r--r--   0        0        0   494652 2020-02-02 00:00:00.000000 scrapegraphai-1.2.0b1/html_structure.png
+-rw-r--r--   0        0        0      587 2020-02-02 00:00:00.000000 scrapegraphai-1.2.0b1/readthedocs.yml
+-rw-r--r--   0        0        0       56 2020-02-02 00:00:00.000000 scrapegraphai-1.2.0b1/requirements-dev.txt
+-rw-r--r--   0        0        0      426 2020-02-02 00:00:00.000000 scrapegraphai-1.2.0b1/requirements.txt
+-rw-r--r--   0        0        0      834 2020-02-02 00:00:00.000000 scrapegraphai-1.2.0b1/.github/ISSUE_TEMPLATE/bug_report.md
+-rw-r--r--   0        0        0      126 2020-02-02 00:00:00.000000 scrapegraphai-1.2.0b1/.github/ISSUE_TEMPLATE/custom.md
+-rw-r--r--   0        0        0      595 2020-02-02 00:00:00.000000 scrapegraphai-1.2.0b1/.github/ISSUE_TEMPLATE/feature_request.md
+-rw-r--r--   0        0        0     2593 2020-02-02 00:00:00.000000 scrapegraphai-1.2.0b1/.github/workflows/codeql.yml
+-rw-r--r--   0        0        0     1729 2020-02-02 00:00:00.000000 scrapegraphai-1.2.0b1/.github/workflows/dependency-review.yml
+-rw-r--r--   0        0        0     1067 2020-02-02 00:00:00.000000 scrapegraphai-1.2.0b1/.github/workflows/pylint.yml
+-rw-r--r--   0        0        0      877 2020-02-02 00:00:00.000000 scrapegraphai-1.2.0b1/.github/workflows/python-publish.yml
+-rw-r--r--   0        0        0     2360 2020-02-02 00:00:00.000000 scrapegraphai-1.2.0b1/.github/workflows/release.yml
+-rw-r--r--   0        0        0      638 2020-02-02 00:00:00.000000 scrapegraphai-1.2.0b1/docs/Makefile
+-rw-r--r--   0        0        0     2546 2020-02-02 00:00:00.000000 scrapegraphai-1.2.0b1/docs/README.md
+-rw-r--r--   0        0        0      769 2020-02-02 00:00:00.000000 scrapegraphai-1.2.0b1/docs/make.bat
+-rw-r--r--   0        0        0    60520 2020-02-02 00:00:00.000000 scrapegraphai-1.2.0b1/docs/assets/apikey_1.png
+-rw-r--r--   0        0        0   123826 2020-02-02 00:00:00.000000 scrapegraphai-1.2.0b1/docs/assets/apikey_2.png
+-rw-r--r--   0        0        0    60775 2020-02-02 00:00:00.000000 scrapegraphai-1.2.0b1/docs/assets/apikey_3.png
+-rw-r--r--   0        0        0    86914 2020-02-02 00:00:00.000000 scrapegraphai-1.2.0b1/docs/assets/apikey_4.png
+-rw-r--r--   0        0        0     3526 2020-02-02 00:00:00.000000 scrapegraphai-1.2.0b1/docs/assets/codespaces-badge.png
+-rw-r--r--   0        0        0  1178826 2020-02-02 00:00:00.000000 scrapegraphai-1.2.0b1/docs/assets/logo_authors.png
+-rw-r--r--   0        0        0    73949 2020-02-02 00:00:00.000000 scrapegraphai-1.2.0b1/docs/assets/omniscrapergraph.png
+-rw-r--r--   0        0        0    58062 2020-02-02 00:00:00.000000 scrapegraphai-1.2.0b1/docs/assets/omnisearchgraph.png
+-rw-r--r--   0        0        0    53007 2020-02-02 00:00:00.000000 scrapegraphai-1.2.0b1/docs/assets/project_overview_diagram.fig
+-rw-r--r--   0        0        0    83949 2020-02-02 00:00:00.000000 scrapegraphai-1.2.0b1/docs/assets/project_overview_diagram.png
+-rw-r--r--   0        0        0    33264 2020-02-02 00:00:00.000000 scrapegraphai-1.2.0b1/docs/assets/scrapegraphai_logo.png
+-rw-r--r--   0        0        0    54611 2020-02-02 00:00:00.000000 scrapegraphai-1.2.0b1/docs/assets/searchgraph.png
+-rw-r--r--   0        0        0    15508 2020-02-02 00:00:00.000000 scrapegraphai-1.2.0b1/docs/assets/serp_api_logo.png
+-rw-r--r--   0        0        0    61095 2020-02-02 00:00:00.000000 scrapegraphai-1.2.0b1/docs/assets/smartscrapergraph.png
+-rw-r--r--   0        0        0    49312 2020-02-02 00:00:00.000000 scrapegraphai-1.2.0b1/docs/assets/speechgraph.png
+-rw-r--r--   0        0        0     1737 2020-02-02 00:00:00.000000 scrapegraphai-1.2.0b1/docs/source/conf.py
+-rw-r--r--   0        0        0      753 2020-02-02 00:00:00.000000 scrapegraphai-1.2.0b1/docs/source/index.rst
+-rw-r--r--   0        0        0     2843 2020-02-02 00:00:00.000000 scrapegraphai-1.2.0b1/docs/source/getting_started/examples.rst
+-rw-r--r--   0        0        0     1213 2020-02-02 00:00:00.000000 scrapegraphai-1.2.0b1/docs/source/getting_started/installation.rst
+-rw-r--r--   0        0        0      523 2020-02-02 00:00:00.000000 scrapegraphai-1.2.0b1/docs/source/introduction/contributing.rst
+-rw-r--r--   0        0        0     1689 2020-02-02 00:00:00.000000 scrapegraphai-1.2.0b1/docs/source/introduction/overview.rst
+-rw-r--r--   0        0        0       47 2020-02-02 00:00:00.000000 scrapegraphai-1.2.0b1/docs/source/modules/modules.rst
+-rw-r--r--   0        0        0      603 2020-02-02 00:00:00.000000 scrapegraphai-1.2.0b1/docs/source/modules/scrapegraphai.graphs.rst
+-rw-r--r--   0        0        0     1410 2020-02-02 00:00:00.000000 scrapegraphai-1.2.0b1/docs/source/modules/scrapegraphai.nodes.rst
+-rw-r--r--   0        0        0     2137 2020-02-02 00:00:00.000000 scrapegraphai-1.2.0b1/docs/source/modules/scrapegraphai.rst
+-rw-r--r--   0        0        0      532 2020-02-02 00:00:00.000000 scrapegraphai-1.2.0b1/docs/source/scrapers/benchmarks.rst
+-rw-r--r--   0        0        0     1868 2020-02-02 00:00:00.000000 scrapegraphai-1.2.0b1/docs/source/scrapers/graph_config.rst
+-rw-r--r--   0        0        0     5646 2020-02-02 00:00:00.000000 scrapegraphai-1.2.0b1/docs/source/scrapers/graphs.rst
+-rw-r--r--   0        0        0     5568 2020-02-02 00:00:00.000000 scrapegraphai-1.2.0b1/docs/source/scrapers/llm.rst
+-rw-r--r--   0        0        0     4500 2020-02-02 00:00:00.000000 scrapegraphai-1.2.0b1/examples/custom_graph_domtree.py
+-rw-r--r--   0        0        0     4011 2020-02-02 00:00:00.000000 scrapegraphai-1.2.0b1/examples/domtree_example.py
+-rw-r--r--   0        0        0     1032 2020-02-02 00:00:00.000000 scrapegraphai-1.2.0b1/examples/faiss_vector.py
+-rw-r--r--   0        0        0     2360 2020-02-02 00:00:00.000000 scrapegraphai-1.2.0b1/examples/readme.md
+-rw-r--r--   0        0        0     2051 2020-02-02 00:00:00.000000 scrapegraphai-1.2.0b1/examples/anthropic/smart_scraper_haiku.py
+-rw-r--r--   0        0        0     2053 2020-02-02 00:00:00.000000 scrapegraphai-1.2.0b1/examples/azure/json_scraper_azure.py
+-rw-r--r--   0        0        0     1929 2020-02-02 00:00:00.000000 scrapegraphai-1.2.0b1/examples/azure/search_graph_azure.py
+-rw-r--r--   0        0        0     2164 2020-02-02 00:00:00.000000 scrapegraphai-1.2.0b1/examples/azure/smart_scraper_azure_openai.py
+-rw-r--r--   0        0        0     2047 2020-02-02 00:00:00.000000 scrapegraphai-1.2.0b1/examples/azure/xml_scraper_azure.py
+-rw-r--r--   0        0        0     4429 2020-02-02 00:00:00.000000 scrapegraphai-1.2.0b1/examples/azure/inputs/books.xml
+-rw-r--r--   0        0        0     6455 2020-02-02 00:00:00.000000 scrapegraphai-1.2.0b1/examples/azure/inputs/example.json
+-rw-r--r--   0        0        0      176 2020-02-02 00:00:00.000000 scrapegraphai-1.2.0b1/examples/azure/inputs/username.csv
+-rw-r--r--   0        0        0      897 2020-02-02 00:00:00.000000 scrapegraphai-1.2.0b1/examples/bedrock/smart_scraper_bedrock.py
+-rw-r--r--   0        0        0      265 2020-02-02 00:00:00.000000 scrapegraphai-1.2.0b1/examples/benchmarks/readme.md
+-rw-r--r--   0        0        0       36 2020-02-02 00:00:00.000000 scrapegraphai-1.2.0b1/examples/benchmarks/GenerateScraper/.env.example
+-rw-r--r--   0        0        0     2888 2020-02-02 00:00:00.000000 scrapegraphai-1.2.0b1/examples/benchmarks/GenerateScraper/Readme.md
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 scrapegraphai-1.2.0b1/examples/benchmarks/GenerateScraper/benchmark_docker.py
+-rw-r--r--   0        0        0     1773 2020-02-02 00:00:00.000000 scrapegraphai-1.2.0b1/examples/benchmarks/GenerateScraper/benchmark_groq.py
+-rw-r--r--   0        0        0     1770 2020-02-02 00:00:00.000000 scrapegraphai-1.2.0b1/examples/benchmarks/GenerateScraper/benchmark_llama3.py
+-rw-r--r--   0        0        0     1862 2020-02-02 00:00:00.000000 scrapegraphai-1.2.0b1/examples/benchmarks/GenerateScraper/benchmark_mistral.py
+-rw-r--r--   0        0        0     1554 2020-02-02 00:00:00.000000 scrapegraphai-1.2.0b1/examples/benchmarks/GenerateScraper/benchmark_openai_gpt35.py
+-rw-r--r--   0        0        0     1563 2020-02-02 00:00:00.000000 scrapegraphai-1.2.0b1/examples/benchmarks/GenerateScraper/benchmark_openai_gpt4.py
+-rw-r--r--   0        0        0     7305 2020-02-02 00:00:00.000000 scrapegraphai-1.2.0b1/examples/benchmarks/GenerateScraper/inputs/example_1.txt
+-rw-r--r--   0        0        0  2590773 2020-02-02 00:00:00.000000 scrapegraphai-1.2.0b1/examples/benchmarks/GenerateScraper/inputs/example_2.txt
+-rw-r--r--   0        0        0       36 2020-02-02 00:00:00.000000 scrapegraphai-1.2.0b1/examples/benchmarks/SmartScraper/.env.example
+-rw-r--r--   0        0        0     2914 2020-02-02 00:00:00.000000 scrapegraphai-1.2.0b1/examples/benchmarks/SmartScraper/Readme.md
+-rw-r--r--   0        0        0     1539 2020-02-02 00:00:00.000000 scrapegraphai-1.2.0b1/examples/benchmarks/SmartScraper/benchmark_docker.py
+-rw-r--r--   0        0        0     1615 2020-02-02 00:00:00.000000 scrapegraphai-1.2.0b1/examples/benchmarks/SmartScraper/benchmark_groq.py
+-rw-r--r--   0        0        0     1630 2020-02-02 00:00:00.000000 scrapegraphai-1.2.0b1/examples/benchmarks/SmartScraper/benchmark_llama3.py
+-rw-r--r--   0        0        0     1641 2020-02-02 00:00:00.000000 scrapegraphai-1.2.0b1/examples/benchmarks/SmartScraper/benchmark_mistral.py
+-rw-r--r--   0        0        0     1520 2020-02-02 00:00:00.000000 scrapegraphai-1.2.0b1/examples/benchmarks/SmartScraper/benchmark_openai_gpt35.py
+-rw-r--r--   0        0        0     1519 2020-02-02 00:00:00.000000 scrapegraphai-1.2.0b1/examples/benchmarks/SmartScraper/benchmark_openai_gpt4.py
+-rw-r--r--   0        0        0     7305 2020-02-02 00:00:00.000000 scrapegraphai-1.2.0b1/examples/benchmarks/SmartScraper/inputs/example_1.txt
+-rw-r--r--   0        0        0  2590773 2020-02-02 00:00:00.000000 scrapegraphai-1.2.0b1/examples/benchmarks/SmartScraper/inputs/example_2.txt
+-rw-r--r--   0        0        0       35 2020-02-02 00:00:00.000000 scrapegraphai-1.2.0b1/examples/deepseek/.env.example
+-rw-r--r--   0        0        0     1665 2020-02-02 00:00:00.000000 scrapegraphai-1.2.0b1/examples/deepseek/csv_scraper_deepseek.py
+-rw-r--r--   0        0        0     1723 2020-02-02 00:00:00.000000 scrapegraphai-1.2.0b1/examples/deepseek/json_scraper_deepseek.py
+-rw-r--r--   0        0        0     1309 2020-02-02 00:00:00.000000 scrapegraphai-1.2.0b1/examples/deepseek/script_generator_deepseek.py
+-rw-r--r--   0        0        0     1238 2020-02-02 00:00:00.000000 scrapegraphai-1.2.0b1/examples/deepseek/search_graph_deepseek.py
+-rw-r--r--   0        0        0     1289 2020-02-02 00:00:00.000000 scrapegraphai-1.2.0b1/examples/deepseek/smart_scarper_deepseek.py
+-rw-r--r--   0        0        0     1714 2020-02-02 00:00:00.000000 scrapegraphai-1.2.0b1/examples/deepseek/xml_scraper_deepseek.py
+-rw-r--r--   0        0        0     4429 2020-02-02 00:00:00.000000 scrapegraphai-1.2.0b1/examples/deepseek/inputs/books.xml
+-rw-r--r--   0        0        0     6455 2020-02-02 00:00:00.000000 scrapegraphai-1.2.0b1/examples/deepseek/inputs/example.json
+-rw-r--r--   0        0        0      176 2020-02-02 00:00:00.000000 scrapegraphai-1.2.0b1/examples/deepseek/inputs/username.csv
+-rw-r--r--   0        0        0       36 2020-02-02 00:00:00.000000 scrapegraphai-1.2.0b1/examples/gemini/.env.example
+-rw-r--r--   0        0        0     1447 2020-02-02 00:00:00.000000 scrapegraphai-1.2.0b1/examples/gemini/csv_scraper_gemini.py
+-rw-r--r--   0        0        0     2120 2020-02-02 00:00:00.000000 scrapegraphai-1.2.0b1/examples/gemini/custom_graph_gemini.py
+-rw-r--r--   0        0        0     1629 2020-02-02 00:00:00.000000 scrapegraphai-1.2.0b1/examples/gemini/json_scraper_gemini.py
+-rw-r--r--   0        0        0      211 2020-02-02 00:00:00.000000 scrapegraphai-1.2.0b1/examples/gemini/readme.md
+-rw-r--r--   0        0        0     1556 2020-02-02 00:00:00.000000 scrapegraphai-1.2.0b1/examples/gemini/scrape_plain_text_gemini.py
+-rw-r--r--   0        0        0     1557 2020-02-02 00:00:00.000000 scrapegraphai-1.2.0b1/examples/gemini/scrape_xml_gemini.py
+-rw-r--r--   0        0        0     1230 2020-02-02 00:00:00.000000 scrapegraphai-1.2.0b1/examples/gemini/script_generator_gemini.py
+-rw-r--r--   0        0        0      964 2020-02-02 00:00:00.000000 scrapegraphai-1.2.0b1/examples/gemini/search_graph_gemini.py
+-rw-r--r--   0        0        0     1175 2020-02-02 00:00:00.000000 scrapegraphai-1.2.0b1/examples/gemini/smart_scraper_gemini.py
+-rw-r--r--   0        0        0     1617 2020-02-02 00:00:00.000000 scrapegraphai-1.2.0b1/examples/gemini/xml_scraper_openai.py
+-rw-r--r--   0        0        0     4429 2020-02-02 00:00:00.000000 scrapegraphai-1.2.0b1/examples/gemini/inputs/books.xml
+-rw-r--r--   0        0        0     6455 2020-02-02 00:00:00.000000 scrapegraphai-1.2.0b1/examples/gemini/inputs/example.json
+-rw-r--r--   0        0        0     7305 2020-02-02 00:00:00.000000 scrapegraphai-1.2.0b1/examples/gemini/inputs/plain_html_example.txt
+-rw-r--r--   0        0        0      176 2020-02-02 00:00:00.000000 scrapegraphai-1.2.0b1/examples/gemini/inputs/username.csv
+-rw-r--r--   0        0        0       64 2020-02-02 00:00:00.000000 scrapegraphai-1.2.0b1/examples/groq/.env.example
+-rw-r--r--   0        0        0     1054 2020-02-02 00:00:00.000000 scrapegraphai-1.2.0b1/examples/groq/search_graph_groq_openai.py
+-rw-r--r--   0        0        0     1414 2020-02-02 00:00:00.000000 scrapegraphai-1.2.0b1/examples/groq/smart_scraper_groq_ollama.py
+-rw-r--r--   0        0        0     1366 2020-02-02 00:00:00.000000 scrapegraphai-1.2.0b1/examples/groq/smart_scraper_groq_openai.py
+-rw-r--r--   0        0        0     2062 2020-02-02 00:00:00.000000 scrapegraphai-1.2.0b1/examples/huggingfacehub/smart_scraper_huggingfacehub.py
+-rw-r--r--   0        0        0     1838 2020-02-02 00:00:00.000000 scrapegraphai-1.2.0b1/examples/local_models/csv_scraper_ollama.py
+-rw-r--r--   0        0        0     1942 2020-02-02 00:00:00.000000 scrapegraphai-1.2.0b1/examples/local_models/json_scraper_ollama.py
+-rw-r--r--   0        0        0     1752 2020-02-02 00:00:00.000000 scrapegraphai-1.2.0b1/examples/local_models/scrape_plain_text_ollama.py
+-rw-r--r--   0        0        0     1832 2020-02-02 00:00:00.000000 scrapegraphai-1.2.0b1/examples/local_models/scrape_xml_ollama.py
+-rw-r--r--   0        0        0     1465 2020-02-02 00:00:00.000000 scrapegraphai-1.2.0b1/examples/local_models/script_generator_ollama.py
+-rw-r--r--   0        0        0     1401 2020-02-02 00:00:00.000000 scrapegraphai-1.2.0b1/examples/local_models/search_graph_ollama.py
+-rw-r--r--   0        0        0     1407 2020-02-02 00:00:00.000000 scrapegraphai-1.2.0b1/examples/local_models/smart_scraper_ollama.py
+-rw-r--r--   0        0        0     1929 2020-02-02 00:00:00.000000 scrapegraphai-1.2.0b1/examples/local_models/xml_scraper_ollama.py
+-rw-r--r--   0        0        0     4429 2020-02-02 00:00:00.000000 scrapegraphai-1.2.0b1/examples/local_models/inputs/books.xml
+-rw-r--r--   0        0        0     6455 2020-02-02 00:00:00.000000 scrapegraphai-1.2.0b1/examples/local_models/inputs/example.json
+-rw-r--r--   0        0        0     7305 2020-02-02 00:00:00.000000 scrapegraphai-1.2.0b1/examples/local_models/inputs/plain_html_example.txt
+-rw-r--r--   0        0        0      176 2020-02-02 00:00:00.000000 scrapegraphai-1.2.0b1/examples/local_models/inputs/username.csv
+-rw-r--r--   0        0        0      208 2020-02-02 00:00:00.000000 scrapegraphai-1.2.0b1/examples/mixed_models/.env.example
+-rw-r--r--   0        0        0      201 2020-02-02 00:00:00.000000 scrapegraphai-1.2.0b1/examples/mixed_models/readme.md
+-rw-r--r--   0        0        0     1357 2020-02-02 00:00:00.000000 scrapegraphai-1.2.0b1/examples/mixed_models/search_graph_groq_ollama.py
+-rw-r--r--   0        0        0     1448 2020-02-02 00:00:00.000000 scrapegraphai-1.2.0b1/examples/mixed_models/smart_scraper_mixed.py
+-rw-r--r--   0        0        0     4429 2020-02-02 00:00:00.000000 scrapegraphai-1.2.0b1/examples/mixed_models/inputs/books.xml
+-rw-r--r--   0        0        0     6455 2020-02-02 00:00:00.000000 scrapegraphai-1.2.0b1/examples/mixed_models/inputs/example.json
+-rw-r--r--   0        0        0     7305 2020-02-02 00:00:00.000000 scrapegraphai-1.2.0b1/examples/mixed_models/inputs/plain_html_example.txt
+-rw-r--r--   0        0        0       39 2020-02-02 00:00:00.000000 scrapegraphai-1.2.0b1/examples/openai/.env.example
+-rw-r--r--   0        0        0     1574 2020-02-02 00:00:00.000000 scrapegraphai-1.2.0b1/examples/openai/csv_scraper_openai.py
+-rw-r--r--   0        0        0     2688 2020-02-02 00:00:00.000000 scrapegraphai-1.2.0b1/examples/openai/custom_graph_openai.py
+-rw-r--r--   0        0        0     1321 2020-02-02 00:00:00.000000 scrapegraphai-1.2.0b1/examples/openai/deep_scraper_openai.py
+-rw-r--r--   0        0        0     1633 2020-02-02 00:00:00.000000 scrapegraphai-1.2.0b1/examples/openai/json_scraper_openai.py
+-rw-r--r--   0        0        0     1307 2020-02-02 00:00:00.000000 scrapegraphai-1.2.0b1/examples/openai/omni_scraper_openai.py
+-rw-r--r--   0        0        0     1142 2020-02-02 00:00:00.000000 scrapegraphai-1.2.0b1/examples/openai/omni_search_graph_openai.py
+-rw-r--r--   0        0        0      203 2020-02-02 00:00:00.000000 scrapegraphai-1.2.0b1/examples/openai/readme.md
+-rw-r--r--   0        0        0     1512 2020-02-02 00:00:00.000000 scrapegraphai-1.2.0b1/examples/openai/scrape_plain_text_openai.py
+-rw-r--r--   0        0        0     1239 2020-02-02 00:00:00.000000 scrapegraphai-1.2.0b1/examples/openai/script_generator_openai.py
+-rw-r--r--   0        0        0     1160 2020-02-02 00:00:00.000000 scrapegraphai-1.2.0b1/examples/openai/search_graph_openai.py
+-rw-r--r--   0        0        0     1233 2020-02-02 00:00:00.000000 scrapegraphai-1.2.0b1/examples/openai/smart_scraper_openai.py
+-rw-r--r--   0        0        0     1531 2020-02-02 00:00:00.000000 scrapegraphai-1.2.0b1/examples/openai/speech_graph_openai.py
+-rw-r--r--   0        0        0     1642 2020-02-02 00:00:00.000000 scrapegraphai-1.2.0b1/examples/openai/xml_scraper_openai.py
+-rw-r--r--   0        0        0     4429 2020-02-02 00:00:00.000000 scrapegraphai-1.2.0b1/examples/openai/inputs/books.xml
+-rw-r--r--   0        0        0     6455 2020-02-02 00:00:00.000000 scrapegraphai-1.2.0b1/examples/openai/inputs/example.json
+-rw-r--r--   0        0        0     7305 2020-02-02 00:00:00.000000 scrapegraphai-1.2.0b1/examples/openai/inputs/plain_html_example.txt
+-rw-r--r--   0        0        0      176 2020-02-02 00:00:00.000000 scrapegraphai-1.2.0b1/examples/openai/inputs/username.csv
+-rw-r--r--   0        0        0      567 2020-02-02 00:00:00.000000 scrapegraphai-1.2.0b1/examples/single_node/fetch_node.py
+-rw-r--r--   0        0        0     1199 2020-02-02 00:00:00.000000 scrapegraphai-1.2.0b1/examples/single_node/image2text_node.py
+-rw-r--r--   0        0        0      961 2020-02-02 00:00:00.000000 scrapegraphai-1.2.0b1/examples/single_node/robot_node.py
+-rwxr-xr-x   0        0        0      986 2020-02-02 00:00:00.000000 scrapegraphai-1.2.0b1/manual deployment/commit_and_push.sh
+-rwxr-xr-x   0        0        0      611 2020-02-02 00:00:00.000000 scrapegraphai-1.2.0b1/manual deployment/commit_and_push_with_tests.sh
+-rwxr-xr-x   0        0        0      169 2020-02-02 00:00:00.000000 scrapegraphai-1.2.0b1/manual deployment/deploy_on_pip.sh
+-rw-r--r--   0        0        0       90 2020-02-02 00:00:00.000000 scrapegraphai-1.2.0b1/manual deployment/rye_update.sh
+-rw-r--r--   0        0        0       54 2020-02-02 00:00:00.000000 scrapegraphai-1.2.0b1/scrapegraphai/__init__.py
+-rw-r--r--   0        0        0       77 2020-02-02 00:00:00.000000 scrapegraphai-1.2.0b1/scrapegraphai/asdt/__init__.py
+-rw-r--r--   0        0        0     2009 2020-02-02 00:00:00.000000 scrapegraphai-1.2.0b1/scrapegraphai/asdt/dom_tree.py
+-rw-r--r--   0        0        0     3658 2020-02-02 00:00:00.000000 scrapegraphai-1.2.0b1/scrapegraphai/asdt/tree.py
+-rw-r--r--   0        0        0     4395 2020-02-02 00:00:00.000000 scrapegraphai-1.2.0b1/scrapegraphai/asdt/tree_node.py
+-rw-r--r--   0        0        0       90 2020-02-02 00:00:00.000000 scrapegraphai-1.2.0b1/scrapegraphai/builders/__init__.py
+-rw-r--r--   0        0        0     6653 2020-02-02 00:00:00.000000 scrapegraphai-1.2.0b1/scrapegraphai/builders/graph_builder.py
+-rw-r--r--   0        0        0       83 2020-02-02 00:00:00.000000 scrapegraphai-1.2.0b1/scrapegraphai/docloaders/__init__.py
+-rw-r--r--   0        0        0     4498 2020-02-02 00:00:00.000000 scrapegraphai-1.2.0b1/scrapegraphai/docloaders/chromium.py
+-rw-r--r--   0        0        0      681 2020-02-02 00:00:00.000000 scrapegraphai-1.2.0b1/scrapegraphai/graphs/__init__.py
+-rw-r--r--   0        0        0    13691 2020-02-02 00:00:00.000000 scrapegraphai-1.2.0b1/scrapegraphai/graphs/abstract_graph.py
+-rw-r--r--   0        0        0     6360 2020-02-02 00:00:00.000000 scrapegraphai-1.2.0b1/scrapegraphai/graphs/base_graph.py
+-rw-r--r--   0        0        0     2472 2020-02-02 00:00:00.000000 scrapegraphai-1.2.0b1/scrapegraphai/graphs/csv_scraper_graph.py
+-rw-r--r--   0        0        0     3777 2020-02-02 00:00:00.000000 scrapegraphai-1.2.0b1/scrapegraphai/graphs/deep_scraper_graph.py
+-rw-r--r--   0        0        0     3392 2020-02-02 00:00:00.000000 scrapegraphai-1.2.0b1/scrapegraphai/graphs/json_scraper_graph.py
+-rw-r--r--   0        0        0     4295 2020-02-02 00:00:00.000000 scrapegraphai-1.2.0b1/scrapegraphai/graphs/omni_scraper_graph.py
+-rw-r--r--   0        0        0     3714 2020-02-02 00:00:00.000000 scrapegraphai-1.2.0b1/scrapegraphai/graphs/omni_search_graph.py
+-rw-r--r--   0        0        0     3538 2020-02-02 00:00:00.000000 scrapegraphai-1.2.0b1/scrapegraphai/graphs/pdf_scraper_graph.py
+-rw-r--r--   0        0        0     3371 2020-02-02 00:00:00.000000 scrapegraphai-1.2.0b1/scrapegraphai/graphs/script_creator_graph.py
+-rw-r--r--   0        0        0     3638 2020-02-02 00:00:00.000000 scrapegraphai-1.2.0b1/scrapegraphai/graphs/search_graph.py
+-rw-r--r--   0        0        0     3651 2020-02-02 00:00:00.000000 scrapegraphai-1.2.0b1/scrapegraphai/graphs/smart_scraper_graph.py
+-rw-r--r--   0        0        0     4322 2020-02-02 00:00:00.000000 scrapegraphai-1.2.0b1/scrapegraphai/graphs/speech_graph.py
+-rw-r--r--   0        0        0     4486 2020-02-02 00:00:00.000000 scrapegraphai-1.2.0b1/scrapegraphai/graphs/turbo_scraper.py
+-rw-r--r--   0        0        0     3534 2020-02-02 00:00:00.000000 scrapegraphai-1.2.0b1/scrapegraphai/graphs/xml_scraper_graph.py
+-rw-r--r--   0        0        0      202 2020-02-02 00:00:00.000000 scrapegraphai-1.2.0b1/scrapegraphai/helpers/__init__.py
+-rw-r--r--   0        0        0     4203 2020-02-02 00:00:00.000000 scrapegraphai-1.2.0b1/scrapegraphai/helpers/models_tokens.py
+-rw-r--r--   0        0        0     3807 2020-02-02 00:00:00.000000 scrapegraphai-1.2.0b1/scrapegraphai/helpers/nodes_metadata.py
+-rw-r--r--   0        0        0      310 2020-02-02 00:00:00.000000 scrapegraphai-1.2.0b1/scrapegraphai/helpers/robots.py
+-rw-r--r--   0        0        0     2363 2020-02-02 00:00:00.000000 scrapegraphai-1.2.0b1/scrapegraphai/helpers/schemas.py
+-rw-r--r--   0        0        0      406 2020-02-02 00:00:00.000000 scrapegraphai-1.2.0b1/scrapegraphai/models/__init__.py
+-rw-r--r--   0        0        0      429 2020-02-02 00:00:00.000000 scrapegraphai-1.2.0b1/scrapegraphai/models/anthropic.py
+-rw-r--r--   0        0        0      441 2020-02-02 00:00:00.000000 scrapegraphai-1.2.0b1/scrapegraphai/models/azure_openai.py
+-rw-r--r--   0        0        0      579 2020-02-02 00:00:00.000000 scrapegraphai-1.2.0b1/scrapegraphai/models/bedrock.py
+-rw-r--r--   0        0        0      455 2020-02-02 00:00:00.000000 scrapegraphai-1.2.0b1/scrapegraphai/models/deepseek.py
+-rw-r--r--   0        0        0      606 2020-02-02 00:00:00.000000 scrapegraphai-1.2.0b1/scrapegraphai/models/gemini.py
+-rw-r--r--   0        0        0      426 2020-02-02 00:00:00.000000 scrapegraphai-1.2.0b1/scrapegraphai/models/groq.py
+-rw-r--r--   0        0        0      459 2020-02-02 00:00:00.000000 scrapegraphai-1.2.0b1/scrapegraphai/models/hugging_face.py
+-rw-r--r--   0        0        0      427 2020-02-02 00:00:00.000000 scrapegraphai-1.2.0b1/scrapegraphai/models/ollama.py
+-rw-r--r--   0        0        0      412 2020-02-02 00:00:00.000000 scrapegraphai-1.2.0b1/scrapegraphai/models/openai.py
+-rw-r--r--   0        0        0     1367 2020-02-02 00:00:00.000000 scrapegraphai-1.2.0b1/scrapegraphai/models/openai_itt.py
+-rw-r--r--   0        0        0     1221 2020-02-02 00:00:00.000000 scrapegraphai-1.2.0b1/scrapegraphai/models/openai_tts.py
+-rw-r--r--   0        0        0      959 2020-02-02 00:00:00.000000 scrapegraphai-1.2.0b1/scrapegraphai/nodes/__init__.py
+-rw-r--r--   0        0        0     8591 2020-02-02 00:00:00.000000 scrapegraphai-1.2.0b1/scrapegraphai/nodes/base_node.py
+-rw-r--r--   0        0        0     2370 2020-02-02 00:00:00.000000 scrapegraphai-1.2.0b1/scrapegraphai/nodes/blocks_identifier.py
+-rw-r--r--   0        0        0     2082 2020-02-02 00:00:00.000000 scrapegraphai-1.2.0b1/scrapegraphai/nodes/conditional_node.py
+-rw-r--r--   0        0        0     6450 2020-02-02 00:00:00.000000 scrapegraphai-1.2.0b1/scrapegraphai/nodes/fetch_node.py
+-rw-r--r--   0        0        0     7182 2020-02-02 00:00:00.000000 scrapegraphai-1.2.0b1/scrapegraphai/nodes/generate_answer_csv_node.py
+-rw-r--r--   0        0        0     6612 2020-02-02 00:00:00.000000 scrapegraphai-1.2.0b1/scrapegraphai/nodes/generate_answer_node.py
+-rw-r--r--   0        0        0     7064 2020-02-02 00:00:00.000000 scrapegraphai-1.2.0b1/scrapegraphai/nodes/generate_answer_omni_node.py
+-rw-r--r--   0        0        0     7158 2020-02-02 00:00:00.000000 scrapegraphai-1.2.0b1/scrapegraphai/nodes/generate_answer_pdf_node.py
+-rw-r--r--   0        0        0     4340 2020-02-02 00:00:00.000000 scrapegraphai-1.2.0b1/scrapegraphai/nodes/generate_scraper_node.py
+-rw-r--r--   0        0        0     3537 2020-02-02 00:00:00.000000 scrapegraphai-1.2.0b1/scrapegraphai/nodes/get_probable_tags_node.py
+-rw-r--r--   0        0        0     4395 2020-02-02 00:00:00.000000 scrapegraphai-1.2.0b1/scrapegraphai/nodes/graph_iterator_node.py
+-rw-r--r--   0        0        0     2671 2020-02-02 00:00:00.000000 scrapegraphai-1.2.0b1/scrapegraphai/nodes/image_to_text_node.py
+-rw-r--r--   0        0        0     3890 2020-02-02 00:00:00.000000 scrapegraphai-1.2.0b1/scrapegraphai/nodes/merge_answers_node.py
+-rw-r--r--   0        0        0     2930 2020-02-02 00:00:00.000000 scrapegraphai-1.2.0b1/scrapegraphai/nodes/parse_node.py
+-rw-r--r--   0        0        0     4496 2020-02-02 00:00:00.000000 scrapegraphai-1.2.0b1/scrapegraphai/nodes/rag_node.py
+-rw-r--r--   0        0        0     6072 2020-02-02 00:00:00.000000 scrapegraphai-1.2.0b1/scrapegraphai/nodes/robots_node.py
+-rw-r--r--   0        0        0     4185 2020-02-02 00:00:00.000000 scrapegraphai-1.2.0b1/scrapegraphai/nodes/search_internet_node.py
+-rw-r--r--   0        0        0     4181 2020-02-02 00:00:00.000000 scrapegraphai-1.2.0b1/scrapegraphai/nodes/search_link_node.py
+-rw-r--r--   0        0        0     4913 2020-02-02 00:00:00.000000 scrapegraphai-1.2.0b1/scrapegraphai/nodes/search_node_with_context.py
+-rw-r--r--   0        0        0     2343 2020-02-02 00:00:00.000000 scrapegraphai-1.2.0b1/scrapegraphai/nodes/text_to_speech_node.py
+-rw-r--r--   0        0        0      424 2020-02-02 00:00:00.000000 scrapegraphai-1.2.0b1/scrapegraphai/utils/__init__.py
+-rw-r--r--   0        0        0     7705 2020-02-02 00:00:00.000000 scrapegraphai-1.2.0b1/scrapegraphai/utils/aaa.py
+-rw-r--r--   0        0        0     5791 2020-02-02 00:00:00.000000 scrapegraphai-1.2.0b1/scrapegraphai/utils/asdt.py
+-rw-r--r--   0        0        0     2330 2020-02-02 00:00:00.000000 scrapegraphai-1.2.0b1/scrapegraphai/utils/cleanup_html.py
+-rw-r--r--   0        0        0     2141 2020-02-02 00:00:00.000000 scrapegraphai-1.2.0b1/scrapegraphai/utils/convert_to_csv.py
+-rw-r--r--   0        0        0     1974 2020-02-02 00:00:00.000000 scrapegraphai-1.2.0b1/scrapegraphai/utils/convert_to_json.py
+-rw-r--r--   0        0        0     4638 2020-02-02 00:00:00.000000 scrapegraphai-1.2.0b1/scrapegraphai/utils/parse_state_keys.py
+-rw-r--r--   0        0        0      764 2020-02-02 00:00:00.000000 scrapegraphai-1.2.0b1/scrapegraphai/utils/prettify_exec_info.py
+-rw-r--r--   0        0        0     6404 2020-02-02 00:00:00.000000 scrapegraphai-1.2.0b1/scrapegraphai/utils/proxy_rotation.py
+-rw-r--r--   0        0        0     2140 2020-02-02 00:00:00.000000 scrapegraphai-1.2.0b1/scrapegraphai/utils/research_web.py
+-rw-r--r--   0        0        0      836 2020-02-02 00:00:00.000000 scrapegraphai-1.2.0b1/scrapegraphai/utils/save_audio_from_bytes.py
+-rw-r--r--   0        0        0     1702 2020-02-02 00:00:00.000000 scrapegraphai-1.2.0b1/scrapegraphai/utils/sys_dynamic_import.py
+-rw-r--r--   0        0        0     1320 2020-02-02 00:00:00.000000 scrapegraphai-1.2.0b1/scrapegraphai/utils/token_calculator.py
+-rw-r--r--   0        0        0     1997 2020-02-02 00:00:00.000000 scrapegraphai-1.2.0b1/scrapegraphai/utils/tree_base.py
+-rw-r--r--   0        0        0      417 2020-02-02 00:00:00.000000 scrapegraphai-1.2.0b1/tests/Readme.md
+-rw-r--r--   0        0        0     1220 2020-02-02 00:00:00.000000 scrapegraphai-1.2.0b1/tests/graphs/scrape_json_ollama.py
+-rw-r--r--   0        0        0     1238 2020-02-02 00:00:00.000000 scrapegraphai-1.2.0b1/tests/graphs/scrape_plain_text_llama3_test.py
+-rw-r--r--   0        0        0     1239 2020-02-02 00:00:00.000000 scrapegraphai-1.2.0b1/tests/graphs/scrape_plain_text_mistral_test.py
+-rw-r--r--   0        0        0     1243 2020-02-02 00:00:00.000000 scrapegraphai-1.2.0b1/tests/graphs/scrape_xml_ollama_test.py
+-rw-r--r--   0        0        0     1223 2020-02-02 00:00:00.000000 scrapegraphai-1.2.0b1/tests/graphs/script_generator_test.py
+-rw-r--r--   0        0        0     1350 2020-02-02 00:00:00.000000 scrapegraphai-1.2.0b1/tests/graphs/smart_scraper_ollama_test.py
+-rw-r--r--   0        0        0     4429 2020-02-02 00:00:00.000000 scrapegraphai-1.2.0b1/tests/graphs/inputs/books.xml
+-rw-r--r--   0        0        0     6455 2020-02-02 00:00:00.000000 scrapegraphai-1.2.0b1/tests/graphs/inputs/example.json
+-rw-r--r--   0        0        0     7305 2020-02-02 00:00:00.000000 scrapegraphai-1.2.0b1/tests/graphs/inputs/plain_html_example.txt
+-rw-r--r--   0        0        0      176 2020-02-02 00:00:00.000000 scrapegraphai-1.2.0b1/tests/graphs/inputs/username.csv
+-rw-r--r--   0        0        0      771 2020-02-02 00:00:00.000000 scrapegraphai-1.2.0b1/tests/nodes/fetch_node_test.py
+-rw-r--r--   0        0        0     1207 2020-02-02 00:00:00.000000 scrapegraphai-1.2.0b1/tests/nodes/robot_node_test.py
+-rw-r--r--   0        0        0     2961 2020-02-02 00:00:00.000000 scrapegraphai-1.2.0b1/tests/utils/test_proxy_rotation.py
+-rw-r--r--   0        0        0     2203 2020-02-02 00:00:00.000000 scrapegraphai-1.2.0b1/tests/utils/test_sys_dynamic_import.py
+-rw-r--r--   0        0        0      448 2020-02-02 00:00:00.000000 scrapegraphai-1.2.0b1/.gitignore
+-rw-r--r--   0        0        0     1065 2020-02-02 00:00:00.000000 scrapegraphai-1.2.0b1/LICENSE
+-rw-r--r--   0        0        0     8967 2020-02-02 00:00:00.000000 scrapegraphai-1.2.0b1/README.md
+-rw-r--r--   0        0        0     2009 2020-02-02 00:00:00.000000 scrapegraphai-1.2.0b1/pyproject.toml
+-rw-r--r--   0        0        0    10488 2020-02-02 00:00:00.000000 scrapegraphai-1.2.0b1/PKG-INFO
```

### Comparing `scrapegraphai-1.2.0/.releaserc.yml` & `scrapegraphai-1.2.0b1/.releaserc.yml`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.2.0/CHANGELOG.md` & `scrapegraphai-1.2.0b1/CHANGELOG.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-## [1.2.0](https://github.com/VinciGit00/Scrapegraph-ai/compare/v1.1.0...v1.2.0) (2024-05-15)
+## [1.2.0-beta.1](https://github.com/VinciGit00/Scrapegraph-ai/compare/v1.1.0...v1.2.0-beta.1) (2024-05-15)
 
 
 ### Features
 
 * add finalize_node() ([6e7283e](https://github.com/VinciGit00/Scrapegraph-ai/commit/6e7283ed8fc42408d718e8776f9fd3856960ffdb))
 
 ## [1.1.0](https://github.com/VinciGit00/Scrapegraph-ai/compare/v1.0.1...v1.1.0) (2024-05-15)
```

### Comparing `scrapegraphai-1.2.0/CODE_OF_CONDUCT.md` & `scrapegraphai-1.2.0b1/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.2.0/CONTRIBUTING.md` & `scrapegraphai-1.2.0b1/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.2.0/html_structure` & `scrapegraphai-1.2.0b1/html_structure`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.2.0/html_structure.png` & `scrapegraphai-1.2.0b1/html_structure.png`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.2.0/readthedocs.yml` & `scrapegraphai-1.2.0b1/readthedocs.yml`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.2.0/.github/ISSUE_TEMPLATE/bug_report.md` & `scrapegraphai-1.2.0b1/.github/ISSUE_TEMPLATE/bug_report.md`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.2.0/.github/ISSUE_TEMPLATE/feature_request.md` & `scrapegraphai-1.2.0b1/.github/ISSUE_TEMPLATE/feature_request.md`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.2.0/.github/workflows/codeql.yml` & `scrapegraphai-1.2.0b1/.github/workflows/codeql.yml`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.2.0/.github/workflows/dependency-review.yml` & `scrapegraphai-1.2.0b1/.github/workflows/dependency-review.yml`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.2.0/.github/workflows/pylint.yml` & `scrapegraphai-1.2.0b1/.github/workflows/pylint.yml`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.2.0/.github/workflows/python-publish.yml` & `scrapegraphai-1.2.0b1/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.2.0/.github/workflows/release.yml` & `scrapegraphai-1.2.0b1/.github/workflows/release.yml`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.2.0/docs/Makefile` & `scrapegraphai-1.2.0b1/docs/Makefile`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.2.0/docs/README.md` & `scrapegraphai-1.2.0b1/docs/README.md`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.2.0/docs/make.bat` & `scrapegraphai-1.2.0b1/docs/make.bat`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.2.0/docs/assets/apikey_1.png` & `scrapegraphai-1.2.0b1/docs/assets/apikey_1.png`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.2.0/docs/assets/apikey_2.png` & `scrapegraphai-1.2.0b1/docs/assets/apikey_2.png`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.2.0/docs/assets/apikey_3.png` & `scrapegraphai-1.2.0b1/docs/assets/apikey_3.png`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.2.0/docs/assets/apikey_4.png` & `scrapegraphai-1.2.0b1/docs/assets/apikey_4.png`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.2.0/docs/assets/codespaces-badge.png` & `scrapegraphai-1.2.0b1/docs/assets/codespaces-badge.png`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.2.0/docs/assets/logo_authors.png` & `scrapegraphai-1.2.0b1/docs/assets/logo_authors.png`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.2.0/docs/assets/omniscrapergraph.png` & `scrapegraphai-1.2.0b1/docs/assets/omniscrapergraph.png`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.2.0/docs/assets/omnisearchgraph.png` & `scrapegraphai-1.2.0b1/docs/assets/omnisearchgraph.png`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.2.0/docs/assets/project_overview_diagram.fig` & `scrapegraphai-1.2.0b1/docs/assets/project_overview_diagram.fig`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.2.0/docs/assets/project_overview_diagram.png` & `scrapegraphai-1.2.0b1/docs/assets/project_overview_diagram.png`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.2.0/docs/assets/scrapegraphai_logo.png` & `scrapegraphai-1.2.0b1/docs/assets/scrapegraphai_logo.png`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.2.0/docs/assets/searchgraph.png` & `scrapegraphai-1.2.0b1/docs/assets/searchgraph.png`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.2.0/docs/assets/serp_api_logo.png` & `scrapegraphai-1.2.0b1/docs/assets/serp_api_logo.png`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.2.0/docs/assets/smartscrapergraph.png` & `scrapegraphai-1.2.0b1/docs/assets/smartscrapergraph.png`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.2.0/docs/assets/speechgraph.png` & `scrapegraphai-1.2.0b1/docs/assets/speechgraph.png`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.2.0/docs/source/conf.py` & `scrapegraphai-1.2.0b1/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.2.0/docs/source/index.rst` & `scrapegraphai-1.2.0b1/docs/source/index.rst`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.2.0/docs/source/getting_started/examples.rst` & `scrapegraphai-1.2.0b1/docs/source/getting_started/examples.rst`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.2.0/docs/source/getting_started/installation.rst` & `scrapegraphai-1.2.0b1/docs/source/getting_started/installation.rst`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.2.0/docs/source/introduction/contributing.rst` & `scrapegraphai-1.2.0b1/docs/source/introduction/contributing.rst`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.2.0/docs/source/introduction/overview.rst` & `scrapegraphai-1.2.0b1/docs/source/introduction/overview.rst`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.2.0/docs/source/modules/scrapegraphai.graphs.rst` & `scrapegraphai-1.2.0b1/docs/source/modules/scrapegraphai.graphs.rst`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.2.0/docs/source/modules/scrapegraphai.nodes.rst` & `scrapegraphai-1.2.0b1/docs/source/modules/scrapegraphai.nodes.rst`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.2.0/docs/source/modules/scrapegraphai.rst` & `scrapegraphai-1.2.0b1/docs/source/modules/scrapegraphai.rst`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.2.0/docs/source/scrapers/benchmarks.rst` & `scrapegraphai-1.2.0b1/docs/source/scrapers/benchmarks.rst`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.2.0/docs/source/scrapers/graph_config.rst` & `scrapegraphai-1.2.0b1/docs/source/scrapers/graph_config.rst`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.2.0/docs/source/scrapers/graphs.rst` & `scrapegraphai-1.2.0b1/docs/source/scrapers/graphs.rst`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.2.0/docs/source/scrapers/llm.rst` & `scrapegraphai-1.2.0b1/docs/source/scrapers/llm.rst`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.2.0/examples/custom_graph_domtree.py` & `scrapegraphai-1.2.0b1/examples/custom_graph_domtree.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.2.0/examples/domtree_example.py` & `scrapegraphai-1.2.0b1/examples/domtree_example.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.2.0/examples/faiss_vector.py` & `scrapegraphai-1.2.0b1/examples/faiss_vector.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.2.0/examples/readme.md` & `scrapegraphai-1.2.0b1/examples/readme.md`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.2.0/examples/anthropic/smart_scraper_haiku.py` & `scrapegraphai-1.2.0b1/examples/anthropic/smart_scraper_haiku.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.2.0/examples/azure/json_scraper_azure.py` & `scrapegraphai-1.2.0b1/examples/azure/json_scraper_azure.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.2.0/examples/azure/search_graph_azure.py` & `scrapegraphai-1.2.0b1/examples/azure/search_graph_azure.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.2.0/examples/azure/smart_scraper_azure_openai.py` & `scrapegraphai-1.2.0b1/examples/azure/smart_scraper_azure_openai.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.2.0/examples/azure/xml_scraper_azure.py` & `scrapegraphai-1.2.0b1/examples/azure/xml_scraper_azure.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.2.0/examples/azure/inputs/books.xml` & `scrapegraphai-1.2.0b1/examples/azure/inputs/books.xml`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.2.0/examples/azure/inputs/example.json` & `scrapegraphai-1.2.0b1/examples/azure/inputs/example.json`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.2.0/examples/bedrock/smart_scraper_bedrock.py` & `scrapegraphai-1.2.0b1/examples/bedrock/smart_scraper_bedrock.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.2.0/examples/benchmarks/GenerateScraper/Readme.md` & `scrapegraphai-1.2.0b1/examples/benchmarks/GenerateScraper/Readme.md`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.2.0/examples/benchmarks/GenerateScraper/benchmark_groq.py` & `scrapegraphai-1.2.0b1/examples/benchmarks/GenerateScraper/benchmark_groq.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.2.0/examples/benchmarks/GenerateScraper/benchmark_llama3.py` & `scrapegraphai-1.2.0b1/examples/benchmarks/GenerateScraper/benchmark_llama3.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.2.0/examples/benchmarks/GenerateScraper/benchmark_mistral.py` & `scrapegraphai-1.2.0b1/examples/benchmarks/GenerateScraper/benchmark_mistral.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.2.0/examples/benchmarks/GenerateScraper/benchmark_openai_gpt35.py` & `scrapegraphai-1.2.0b1/examples/benchmarks/GenerateScraper/benchmark_openai_gpt35.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.2.0/examples/benchmarks/GenerateScraper/benchmark_openai_gpt4.py` & `scrapegraphai-1.2.0b1/examples/benchmarks/GenerateScraper/benchmark_openai_gpt4.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.2.0/examples/benchmarks/GenerateScraper/inputs/example_1.txt` & `scrapegraphai-1.2.0b1/examples/benchmarks/GenerateScraper/inputs/example_1.txt`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.2.0/examples/benchmarks/GenerateScraper/inputs/example_2.txt` & `scrapegraphai-1.2.0b1/examples/benchmarks/GenerateScraper/inputs/example_2.txt`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.2.0/examples/benchmarks/SmartScraper/Readme.md` & `scrapegraphai-1.2.0b1/examples/benchmarks/SmartScraper/Readme.md`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.2.0/examples/benchmarks/SmartScraper/benchmark_docker.py` & `scrapegraphai-1.2.0b1/examples/benchmarks/SmartScraper/benchmark_docker.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.2.0/examples/benchmarks/SmartScraper/benchmark_groq.py` & `scrapegraphai-1.2.0b1/examples/benchmarks/SmartScraper/benchmark_groq.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.2.0/examples/benchmarks/SmartScraper/benchmark_llama3.py` & `scrapegraphai-1.2.0b1/examples/benchmarks/SmartScraper/benchmark_llama3.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.2.0/examples/benchmarks/SmartScraper/benchmark_mistral.py` & `scrapegraphai-1.2.0b1/examples/benchmarks/SmartScraper/benchmark_mistral.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.2.0/examples/benchmarks/SmartScraper/benchmark_openai_gpt35.py` & `scrapegraphai-1.2.0b1/examples/benchmarks/SmartScraper/benchmark_openai_gpt35.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.2.0/examples/benchmarks/SmartScraper/benchmark_openai_gpt4.py` & `scrapegraphai-1.2.0b1/examples/benchmarks/SmartScraper/benchmark_openai_gpt4.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.2.0/examples/benchmarks/SmartScraper/inputs/example_1.txt` & `scrapegraphai-1.2.0b1/examples/benchmarks/SmartScraper/inputs/example_1.txt`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.2.0/examples/benchmarks/SmartScraper/inputs/example_2.txt` & `scrapegraphai-1.2.0b1/examples/benchmarks/SmartScraper/inputs/example_2.txt`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.2.0/examples/deepseek/csv_scraper_deepseek.py` & `scrapegraphai-1.2.0b1/examples/deepseek/csv_scraper_deepseek.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.2.0/examples/deepseek/json_scraper_deepseek.py` & `scrapegraphai-1.2.0b1/examples/deepseek/json_scraper_deepseek.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.2.0/examples/deepseek/script_generator_deepseek.py` & `scrapegraphai-1.2.0b1/examples/deepseek/script_generator_deepseek.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.2.0/examples/deepseek/search_graph_deepseek.py` & `scrapegraphai-1.2.0b1/examples/deepseek/search_graph_deepseek.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.2.0/examples/deepseek/smart_scarper_deepseek.py` & `scrapegraphai-1.2.0b1/examples/deepseek/smart_scarper_deepseek.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.2.0/examples/deepseek/xml_scraper_deepseek.py` & `scrapegraphai-1.2.0b1/examples/deepseek/xml_scraper_deepseek.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.2.0/examples/deepseek/inputs/books.xml` & `scrapegraphai-1.2.0b1/examples/deepseek/inputs/books.xml`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.2.0/examples/deepseek/inputs/example.json` & `scrapegraphai-1.2.0b1/examples/deepseek/inputs/example.json`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.2.0/examples/gemini/csv_scraper_gemini.py` & `scrapegraphai-1.2.0b1/examples/gemini/csv_scraper_gemini.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.2.0/examples/gemini/custom_graph_gemini.py` & `scrapegraphai-1.2.0b1/examples/gemini/custom_graph_gemini.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.2.0/examples/gemini/json_scraper_gemini.py` & `scrapegraphai-1.2.0b1/examples/gemini/json_scraper_gemini.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.2.0/examples/gemini/scrape_plain_text_gemini.py` & `scrapegraphai-1.2.0b1/examples/gemini/scrape_plain_text_gemini.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.2.0/examples/gemini/scrape_xml_gemini.py` & `scrapegraphai-1.2.0b1/examples/gemini/scrape_xml_gemini.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.2.0/examples/gemini/script_generator_gemini.py` & `scrapegraphai-1.2.0b1/examples/gemini/script_generator_gemini.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.2.0/examples/gemini/search_graph_gemini.py` & `scrapegraphai-1.2.0b1/examples/gemini/search_graph_gemini.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.2.0/examples/gemini/smart_scraper_gemini.py` & `scrapegraphai-1.2.0b1/examples/gemini/smart_scraper_gemini.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.2.0/examples/gemini/xml_scraper_openai.py` & `scrapegraphai-1.2.0b1/examples/gemini/xml_scraper_openai.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.2.0/examples/gemini/inputs/books.xml` & `scrapegraphai-1.2.0b1/examples/gemini/inputs/books.xml`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.2.0/examples/gemini/inputs/example.json` & `scrapegraphai-1.2.0b1/examples/gemini/inputs/example.json`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.2.0/examples/gemini/inputs/plain_html_example.txt` & `scrapegraphai-1.2.0b1/examples/gemini/inputs/plain_html_example.txt`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.2.0/examples/groq/search_graph_groq_openai.py` & `scrapegraphai-1.2.0b1/examples/groq/search_graph_groq_openai.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.2.0/examples/groq/smart_scraper_groq_ollama.py` & `scrapegraphai-1.2.0b1/examples/groq/smart_scraper_groq_ollama.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.2.0/examples/groq/smart_scraper_groq_openai.py` & `scrapegraphai-1.2.0b1/examples/groq/smart_scraper_groq_openai.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.2.0/examples/huggingfacehub/smart_scraper_huggingfacehub.py` & `scrapegraphai-1.2.0b1/examples/huggingfacehub/smart_scraper_huggingfacehub.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.2.0/examples/local_models/csv_scraper_ollama.py` & `scrapegraphai-1.2.0b1/examples/local_models/csv_scraper_ollama.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.2.0/examples/local_models/json_scraper_ollama.py` & `scrapegraphai-1.2.0b1/examples/local_models/json_scraper_ollama.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.2.0/examples/local_models/scrape_plain_text_ollama.py` & `scrapegraphai-1.2.0b1/examples/local_models/scrape_plain_text_ollama.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.2.0/examples/local_models/scrape_xml_ollama.py` & `scrapegraphai-1.2.0b1/examples/local_models/scrape_xml_ollama.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.2.0/examples/local_models/script_generator_ollama.py` & `scrapegraphai-1.2.0b1/examples/local_models/script_generator_ollama.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.2.0/examples/local_models/search_graph_ollama.py` & `scrapegraphai-1.2.0b1/examples/local_models/search_graph_ollama.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.2.0/examples/local_models/smart_scraper_ollama.py` & `scrapegraphai-1.2.0b1/examples/local_models/smart_scraper_ollama.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.2.0/examples/local_models/xml_scraper_ollama.py` & `scrapegraphai-1.2.0b1/examples/local_models/xml_scraper_ollama.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.2.0/examples/local_models/inputs/books.xml` & `scrapegraphai-1.2.0b1/examples/local_models/inputs/books.xml`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.2.0/examples/local_models/inputs/example.json` & `scrapegraphai-1.2.0b1/examples/local_models/inputs/example.json`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.2.0/examples/local_models/inputs/plain_html_example.txt` & `scrapegraphai-1.2.0b1/examples/local_models/inputs/plain_html_example.txt`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.2.0/examples/mixed_models/search_graph_groq_ollama.py` & `scrapegraphai-1.2.0b1/examples/mixed_models/search_graph_groq_ollama.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.2.0/examples/mixed_models/smart_scraper_mixed.py` & `scrapegraphai-1.2.0b1/examples/mixed_models/smart_scraper_mixed.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.2.0/examples/mixed_models/inputs/books.xml` & `scrapegraphai-1.2.0b1/examples/mixed_models/inputs/books.xml`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.2.0/examples/mixed_models/inputs/example.json` & `scrapegraphai-1.2.0b1/examples/mixed_models/inputs/example.json`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.2.0/examples/mixed_models/inputs/plain_html_example.txt` & `scrapegraphai-1.2.0b1/examples/mixed_models/inputs/plain_html_example.txt`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.2.0/examples/openai/csv_scraper_openai.py` & `scrapegraphai-1.2.0b1/examples/openai/csv_scraper_openai.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.2.0/examples/openai/custom_graph_openai.py` & `scrapegraphai-1.2.0b1/examples/openai/custom_graph_openai.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.2.0/examples/openai/deep_scraper_openai.py` & `scrapegraphai-1.2.0b1/examples/openai/deep_scraper_openai.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.2.0/examples/openai/json_scraper_openai.py` & `scrapegraphai-1.2.0b1/examples/openai/json_scraper_openai.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.2.0/examples/openai/omni_scraper_openai.py` & `scrapegraphai-1.2.0b1/examples/openai/omni_scraper_openai.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.2.0/examples/openai/omni_search_graph_openai.py` & `scrapegraphai-1.2.0b1/examples/openai/omni_search_graph_openai.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.2.0/examples/openai/scrape_plain_text_openai.py` & `scrapegraphai-1.2.0b1/examples/openai/scrape_plain_text_openai.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.2.0/examples/openai/script_generator_openai.py` & `scrapegraphai-1.2.0b1/examples/openai/script_generator_openai.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.2.0/examples/openai/search_graph_openai.py` & `scrapegraphai-1.2.0b1/examples/openai/search_graph_openai.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.2.0/examples/openai/smart_scraper_openai.py` & `scrapegraphai-1.2.0b1/examples/openai/smart_scraper_openai.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.2.0/examples/openai/speech_graph_openai.py` & `scrapegraphai-1.2.0b1/examples/openai/speech_graph_openai.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.2.0/examples/openai/xml_scraper_openai.py` & `scrapegraphai-1.2.0b1/examples/openai/xml_scraper_openai.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.2.0/examples/openai/inputs/books.xml` & `scrapegraphai-1.2.0b1/examples/openai/inputs/books.xml`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.2.0/examples/openai/inputs/example.json` & `scrapegraphai-1.2.0b1/examples/openai/inputs/example.json`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.2.0/examples/openai/inputs/plain_html_example.txt` & `scrapegraphai-1.2.0b1/examples/openai/inputs/plain_html_example.txt`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.2.0/examples/single_node/fetch_node.py` & `scrapegraphai-1.2.0b1/examples/single_node/fetch_node.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.2.0/examples/single_node/image2text_node.py` & `scrapegraphai-1.2.0b1/examples/single_node/image2text_node.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.2.0/examples/single_node/robot_node.py` & `scrapegraphai-1.2.0b1/examples/single_node/robot_node.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.2.0/manual deployment/commit_and_push.sh` & `scrapegraphai-1.2.0b1/manual deployment/commit_and_push.sh`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.2.0/manual deployment/commit_and_push_with_tests.sh` & `scrapegraphai-1.2.0b1/manual deployment/commit_and_push_with_tests.sh`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.2.0/scrapegraphai/asdt/dom_tree.py` & `scrapegraphai-1.2.0b1/scrapegraphai/asdt/dom_tree.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.2.0/scrapegraphai/asdt/tree.py` & `scrapegraphai-1.2.0b1/scrapegraphai/asdt/tree.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.2.0/scrapegraphai/asdt/tree_node.py` & `scrapegraphai-1.2.0b1/scrapegraphai/asdt/tree_node.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.2.0/scrapegraphai/builders/graph_builder.py` & `scrapegraphai-1.2.0b1/scrapegraphai/builders/graph_builder.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.2.0/scrapegraphai/docloaders/chromium.py` & `scrapegraphai-1.2.0b1/scrapegraphai/docloaders/chromium.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.2.0/scrapegraphai/graphs/__init__.py` & `scrapegraphai-1.2.0b1/scrapegraphai/graphs/__init__.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.2.0/scrapegraphai/graphs/abstract_graph.py` & `scrapegraphai-1.2.0b1/scrapegraphai/graphs/abstract_graph.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.2.0/scrapegraphai/graphs/base_graph.py` & `scrapegraphai-1.2.0b1/scrapegraphai/graphs/base_graph.py`

 * *Files 18% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 BaseGraph Module
 """
 
 import time
 import warnings
 from langchain_community.callbacks import get_openai_callback
 from typing import Tuple
+from collections import deque
 
 
 class BaseGraph:
     """
     BaseGraph manages the execution flow of a graph composed of interconnected nodes.
 
     Attributes:
@@ -22,14 +23,16 @@
         nodes (iterable): An iterable of node instances that will be part of the graph.
         edges (iterable): An iterable of tuples where each tuple represents a directed edge
                           in the graph, defined by a pair of nodes (from_node, to_node).
         entry_point (BaseNode): The node instance that represents the entry point of the graph.
 
     Raises:
         Warning: If the entry point node is not the first node in the list.
+        ValueError: If conditional_node does not have exactly two outgoing edges
+
 
     Example:
         >>> BaseGraph(
         ...    nodes=[
         ...        fetch_node,
         ...        parse_node,
         ...        rag_node,
@@ -44,15 +47,15 @@
         ... )
     """
 
     def __init__(self, nodes: list, edges: list, entry_point: str):
 
         self.nodes = nodes
         self.edges = self._create_edges({e for e in edges})
-        self.entry_point = entry_point.node_name
+        self.entry_point = entry_point
 
         if nodes[0].node_name != entry_point.node_name:
             # raise a warning if the entry point is not the first node in the list
             warnings.warn(
                 "Careful! The entry point node is different from the first node if the graph.")
 
     def _create_edges(self, edges: list) -> dict:
@@ -64,85 +67,95 @@
 
         Returns:
             dict: A dictionary of edges with the from-node as keys and to-node as values.
         """
 
         edge_dict = {}
         for from_node, to_node in edges:
-            edge_dict[from_node.node_name] = to_node.node_name
+            if from_node in edge_dict:
+                edge_dict[from_node].append(to_node)
+            else:
+                edge_dict[from_node] = [to_node]
         return edge_dict
 
     def execute(self, initial_state: dict) -> Tuple[dict, list]:
         """
-        Executes the graph by traversing nodes starting from the entry point. The execution
-        follows the edges based on the result of each node's execution and continues until
+        Executes the graph by traversing nodes in breadth-first order starting from the entry point.
+        The execution follows the edges based on the result of each node's execution and continues until
         it reaches a node with no outgoing edges.
 
         Args:
             initial_state (dict): The initial state to pass to the entry point node.
 
         Returns:
             Tuple[dict, list]: A tuple containing the final state and a list of execution info.
         """
 
-        current_node_name = self.nodes[0]
         state = initial_state
 
         # variables for tracking execution info
         total_exec_time = 0.0
         exec_info = []
         cb_total = {
             "total_tokens": 0,
             "prompt_tokens": 0,
             "completion_tokens": 0,
             "successful_requests": 0,
             "total_cost_USD": 0.0,
         }
 
-        for index in self.nodes:
-
+        queue = deque([self.entry_point])
+        while queue:
+            current_node = queue.popleft()
             curr_time = time.time()
-            current_node = index
-
-            with get_openai_callback() as cb:
+            with get_openai_callback() as callback:
                 result = current_node.execute(state)
                 node_exec_time = time.time() - curr_time
                 total_exec_time += node_exec_time
 
                 cb = {
-                    "node_name": index.node_name,
-                    "total_tokens": cb.total_tokens,
-                    "prompt_tokens": cb.prompt_tokens,
-                    "completion_tokens": cb.completion_tokens,
-                    "successful_requests": cb.successful_requests,
-                    "total_cost_USD": cb.total_cost,
+                    "node_name": current_node.node_name,
+                    "total_tokens": callback.total_tokens,
+                    "prompt_tokens": callback.prompt_tokens,
+                    "completion_tokens": callback.completion_tokens,
+                    "successful_requests": callback.successful_requests,
+                    "total_cost_USD": callback.total_cost,
                     "exec_time": node_exec_time,
                 }
 
                 exec_info.append(
                     cb
                 )
 
                 cb_total["total_tokens"] += cb["total_tokens"]
                 cb_total["prompt_tokens"] += cb["prompt_tokens"]
                 cb_total["completion_tokens"] += cb["completion_tokens"]
                 cb_total["successful_requests"] += cb["successful_requests"]
                 cb_total["total_cost_USD"] += cb["total_cost_USD"]
 
-            if current_node.node_type == "conditional_node":
-                current_node_name = result
-            elif current_node_name in self.edges:
-                current_node_name = self.edges[current_node_name]
-            else:
-                current_node_name = None
-
-        exec_info.append({
-            "node_name": "TOTAL RESULT",
-            "total_tokens":  cb_total["total_tokens"],
-            "prompt_tokens":  cb_total["prompt_tokens"],
-            "completion_tokens": cb_total["completion_tokens"],
-            "successful_requests": cb_total["successful_requests"],
-            "total_cost_USD":   cb_total["total_cost_USD"],
-            "exec_time": total_exec_time,
-        })
+                if current_node in self.edges:
+                    current_node_connections = self.edges[current_node]
+                    if current_node.node_type == 'conditional_node':
+                        # Assert that there are exactly two out edges from the conditional node
+                        if len(current_node_connections) != 2:
+                            raise ValueError(f"Conditional node should have exactly two out connections {current_node_connections.node_name}")
+                        if result["next_node"] == 0:
+                            queue.append(current_node_connections[0])
+                        else:
+                            queue.append(current_node_connections[1])
+                        # remove the conditional node result
+                        del result["next_node"]
+                    else:
+                        queue.extend(node for node in current_node_connections)
+
+
+                exec_info.append({
+                    "node_name": "TOTAL RESULT",
+                    "total_tokens":  cb_total["total_tokens"],
+                    "prompt_tokens":  cb_total["prompt_tokens"],
+                    "completion_tokens": cb_total["completion_tokens"],
+                    "successful_requests": cb_total["successful_requests"],
+                    "total_cost_USD":   cb_total["total_cost_USD"],
+                    "exec_time": total_exec_time,
+                })
 
         return state, exec_info
```

### Comparing `scrapegraphai-1.2.0/scrapegraphai/graphs/csv_scraper_graph.py` & `scrapegraphai-1.2.0b1/scrapegraphai/graphs/csv_scraper_graph.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.2.0/scrapegraphai/graphs/deep_scraper_graph.py` & `scrapegraphai-1.2.0b1/scrapegraphai/graphs/deep_scraper_graph.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.2.0/scrapegraphai/graphs/json_scraper_graph.py` & `scrapegraphai-1.2.0b1/scrapegraphai/graphs/json_scraper_graph.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.2.0/scrapegraphai/graphs/omni_scraper_graph.py` & `scrapegraphai-1.2.0b1/scrapegraphai/graphs/omni_scraper_graph.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.2.0/scrapegraphai/graphs/omni_search_graph.py` & `scrapegraphai-1.2.0b1/scrapegraphai/graphs/omni_search_graph.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.2.0/scrapegraphai/graphs/pdf_scraper_graph.py` & `scrapegraphai-1.2.0b1/scrapegraphai/graphs/pdf_scraper_graph.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.2.0/scrapegraphai/graphs/script_creator_graph.py` & `scrapegraphai-1.2.0b1/scrapegraphai/graphs/script_creator_graph.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.2.0/scrapegraphai/graphs/search_graph.py` & `scrapegraphai-1.2.0b1/scrapegraphai/graphs/search_graph.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.2.0/scrapegraphai/graphs/smart_scraper_graph.py` & `scrapegraphai-1.2.0b1/scrapegraphai/graphs/smart_scraper_graph.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.2.0/scrapegraphai/graphs/speech_graph.py` & `scrapegraphai-1.2.0b1/scrapegraphai/graphs/speech_graph.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.2.0/scrapegraphai/graphs/turbo_scraper.py` & `scrapegraphai-1.2.0b1/scrapegraphai/graphs/turbo_scraper.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.2.0/scrapegraphai/graphs/xml_scraper_graph.py` & `scrapegraphai-1.2.0b1/scrapegraphai/graphs/xml_scraper_graph.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.2.0/scrapegraphai/helpers/models_tokens.py` & `scrapegraphai-1.2.0b1/scrapegraphai/helpers/models_tokens.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.2.0/scrapegraphai/helpers/nodes_metadata.py` & `scrapegraphai-1.2.0b1/scrapegraphai/helpers/nodes_metadata.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.2.0/scrapegraphai/helpers/schemas.py` & `scrapegraphai-1.2.0b1/scrapegraphai/helpers/schemas.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.2.0/scrapegraphai/models/bedrock.py` & `scrapegraphai-1.2.0b1/scrapegraphai/models/bedrock.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.2.0/scrapegraphai/models/gemini.py` & `scrapegraphai-1.2.0b1/scrapegraphai/models/gemini.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.2.0/scrapegraphai/models/openai_itt.py` & `scrapegraphai-1.2.0b1/scrapegraphai/models/openai_itt.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.2.0/scrapegraphai/models/openai_tts.py` & `scrapegraphai-1.2.0b1/scrapegraphai/models/openai_tts.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.2.0/scrapegraphai/nodes/__init__.py` & `scrapegraphai-1.2.0b1/scrapegraphai/nodes/__init__.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.2.0/scrapegraphai/nodes/base_node.py` & `scrapegraphai-1.2.0b1/scrapegraphai/nodes/base_node.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.2.0/scrapegraphai/nodes/blocks_identifier.py` & `scrapegraphai-1.2.0b1/scrapegraphai/nodes/blocks_identifier.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.2.0/scrapegraphai/nodes/conditional_node.py` & `scrapegraphai-1.2.0b1/scrapegraphai/nodes/conditional_node.py`

 * *Files 17% similar despite different names*

```diff
@@ -9,60 +9,49 @@
     A node that determines the next step in the graph's execution flow based on 
     the presence and content of a specified key in the graph's state. It extends 
     the BaseNode by adding condition-based logic to the execution process.
 
     This node type is used to implement branching logic within the graph, allowing 
     for dynamic paths based on the data available in the current state.
 
+    It is expected thar exactly two edges are created out of this node.
+    The first node is chosen for execution if the key exists and has a non-empty value,
+    and the second node is chosen if the key does not exist or is empty.
+
     Attributes:
         key_name (str): The name of the key in the state to check for its presence.
-        next_nodes (list): A list of two node instances. The first node is chosen 
-                           for execution if the key exists and has a non-empty value, 
-                           and the second node is chosen if the key does not exist or 
-                           is empty.
 
     Args:
         key_name (str): The name of the key to check in the graph's state. This is 
                         used to determine the path the graph's execution should take.
-        next_nodes (list): A list containing exactly two node instances, specifying 
-                           the next nodes to execute based on the condition's outcome.
         node_name (str, optional): The unique identifier name for the node. Defaults 
                                    to "ConditionalNode".
 
-    Raises:
-        ValueError: If next_nodes does not contain exactly two elements, indicating 
-                    a misconfiguration in specifying the conditional paths.
     """
 
-    def __init__(self, key_name: str, next_nodes: list, node_name="ConditionalNode"):
+    def __init__(self, key_name: str, node_name="ConditionalNode"):
         """
         Initializes the node with the key to check and the next node names based on the condition.
 
         Args:
             key_name (str): The name of the key to check in the state.
-            next_nodes (list): A list containing exactly two names of the next nodes.
-                               The first is used if the key exists, the second if it does not.
-
-        Raises:
-            ValueError: If next_nodes does not contain exactly two elements.
         """
 
         super().__init__(node_name, "conditional_node")
         self.key_name = key_name
-        if len(next_nodes) != 2:
-            raise ValueError("next_nodes must contain exactly two elements.")
-        self.next_nodes = next_nodes
 
-    def execute(self, state: dict) -> str:
+    def execute(self, state: dict) -> dict:
         """
         Checks if the specified key is present in the state and decides the next node accordingly.
 
         Args:
             state (dict): The current state of the graph.
 
         Returns:
             str: The name of the next node to execute based on the presence of the key.
         """
 
         if self.key_name in state and len(state[self.key_name]) > 0:
-            return self.next_nodes[0].node_name
-        return self.next_nodes[1].node_name
+            state["next_node"] = 0
+        else:
+            state["next_node"] = 1
+        return state
```

### Comparing `scrapegraphai-1.2.0/scrapegraphai/nodes/fetch_node.py` & `scrapegraphai-1.2.0b1/scrapegraphai/nodes/fetch_node.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.2.0/scrapegraphai/nodes/generate_answer_csv_node.py` & `scrapegraphai-1.2.0b1/scrapegraphai/nodes/generate_answer_csv_node.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.2.0/scrapegraphai/nodes/generate_answer_node.py` & `scrapegraphai-1.2.0b1/scrapegraphai/nodes/generate_answer_node.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.2.0/scrapegraphai/nodes/generate_answer_omni_node.py` & `scrapegraphai-1.2.0b1/scrapegraphai/nodes/generate_answer_omni_node.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.2.0/scrapegraphai/nodes/generate_answer_pdf_node.py` & `scrapegraphai-1.2.0b1/scrapegraphai/nodes/generate_answer_pdf_node.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.2.0/scrapegraphai/nodes/generate_scraper_node.py` & `scrapegraphai-1.2.0b1/scrapegraphai/nodes/generate_scraper_node.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.2.0/scrapegraphai/nodes/get_probable_tags_node.py` & `scrapegraphai-1.2.0b1/scrapegraphai/nodes/get_probable_tags_node.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.2.0/scrapegraphai/nodes/graph_iterator_node.py` & `scrapegraphai-1.2.0b1/scrapegraphai/nodes/graph_iterator_node.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.2.0/scrapegraphai/nodes/image_to_text_node.py` & `scrapegraphai-1.2.0b1/scrapegraphai/nodes/image_to_text_node.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.2.0/scrapegraphai/nodes/merge_answers_node.py` & `scrapegraphai-1.2.0b1/scrapegraphai/nodes/merge_answers_node.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.2.0/scrapegraphai/nodes/parse_node.py` & `scrapegraphai-1.2.0b1/scrapegraphai/nodes/parse_node.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.2.0/scrapegraphai/nodes/rag_node.py` & `scrapegraphai-1.2.0b1/scrapegraphai/nodes/rag_node.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.2.0/scrapegraphai/nodes/robots_node.py` & `scrapegraphai-1.2.0b1/scrapegraphai/nodes/robots_node.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.2.0/scrapegraphai/nodes/search_internet_node.py` & `scrapegraphai-1.2.0b1/scrapegraphai/nodes/search_internet_node.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.2.0/scrapegraphai/nodes/search_link_node.py` & `scrapegraphai-1.2.0b1/scrapegraphai/nodes/search_link_node.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.2.0/scrapegraphai/nodes/search_node_with_context.py` & `scrapegraphai-1.2.0b1/scrapegraphai/nodes/search_node_with_context.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.2.0/scrapegraphai/nodes/text_to_speech_node.py` & `scrapegraphai-1.2.0b1/scrapegraphai/nodes/text_to_speech_node.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.2.0/scrapegraphai/utils/aaa.py` & `scrapegraphai-1.2.0b1/scrapegraphai/utils/aaa.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.2.0/scrapegraphai/utils/asdt.py` & `scrapegraphai-1.2.0b1/scrapegraphai/utils/asdt.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.2.0/scrapegraphai/utils/cleanup_html.py` & `scrapegraphai-1.2.0b1/scrapegraphai/utils/cleanup_html.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.2.0/scrapegraphai/utils/convert_to_csv.py` & `scrapegraphai-1.2.0b1/scrapegraphai/utils/convert_to_csv.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.2.0/scrapegraphai/utils/convert_to_json.py` & `scrapegraphai-1.2.0b1/scrapegraphai/utils/convert_to_json.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.2.0/scrapegraphai/utils/parse_state_keys.py` & `scrapegraphai-1.2.0b1/scrapegraphai/utils/parse_state_keys.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.2.0/scrapegraphai/utils/prettify_exec_info.py` & `scrapegraphai-1.2.0b1/scrapegraphai/utils/prettify_exec_info.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.2.0/scrapegraphai/utils/proxy_rotation.py` & `scrapegraphai-1.2.0b1/scrapegraphai/utils/proxy_rotation.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.2.0/scrapegraphai/utils/research_web.py` & `scrapegraphai-1.2.0b1/scrapegraphai/utils/research_web.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.2.0/scrapegraphai/utils/save_audio_from_bytes.py` & `scrapegraphai-1.2.0b1/scrapegraphai/utils/save_audio_from_bytes.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.2.0/scrapegraphai/utils/sys_dynamic_import.py` & `scrapegraphai-1.2.0b1/scrapegraphai/utils/sys_dynamic_import.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.2.0/scrapegraphai/utils/token_calculator.py` & `scrapegraphai-1.2.0b1/scrapegraphai/utils/token_calculator.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.2.0/scrapegraphai/utils/tree_base.py` & `scrapegraphai-1.2.0b1/scrapegraphai/utils/tree_base.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.2.0/tests/graphs/scrape_json_ollama.py` & `scrapegraphai-1.2.0b1/tests/graphs/scrape_json_ollama.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.2.0/tests/graphs/scrape_plain_text_llama3_test.py` & `scrapegraphai-1.2.0b1/tests/graphs/scrape_plain_text_llama3_test.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.2.0/tests/graphs/scrape_plain_text_mistral_test.py` & `scrapegraphai-1.2.0b1/tests/graphs/scrape_plain_text_mistral_test.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.2.0/tests/graphs/scrape_xml_ollama_test.py` & `scrapegraphai-1.2.0b1/tests/graphs/scrape_xml_ollama_test.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.2.0/tests/graphs/script_generator_test.py` & `scrapegraphai-1.2.0b1/tests/graphs/script_generator_test.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.2.0/tests/graphs/smart_scraper_ollama_test.py` & `scrapegraphai-1.2.0b1/tests/graphs/smart_scraper_ollama_test.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.2.0/tests/graphs/inputs/books.xml` & `scrapegraphai-1.2.0b1/tests/graphs/inputs/books.xml`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.2.0/tests/graphs/inputs/example.json` & `scrapegraphai-1.2.0b1/tests/graphs/inputs/example.json`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.2.0/tests/graphs/inputs/plain_html_example.txt` & `scrapegraphai-1.2.0b1/tests/graphs/inputs/plain_html_example.txt`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.2.0/tests/nodes/fetch_node_test.py` & `scrapegraphai-1.2.0b1/tests/nodes/fetch_node_test.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.2.0/tests/nodes/robot_node_test.py` & `scrapegraphai-1.2.0b1/tests/nodes/robot_node_test.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.2.0/tests/utils/test_proxy_rotation.py` & `scrapegraphai-1.2.0b1/tests/utils/test_proxy_rotation.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.2.0/tests/utils/test_sys_dynamic_import.py` & `scrapegraphai-1.2.0b1/tests/utils/test_sys_dynamic_import.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.2.0/LICENSE` & `scrapegraphai-1.2.0b1/LICENSE`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.2.0/README.md` & `scrapegraphai-1.2.0b1/README.md`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.2.0/pyproject.toml` & `scrapegraphai-1.2.0b1/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [project]
 name = "scrapegraphai"
 
-version = "1.2.0"
+version = "1.2.0b1"
 
 description = "A web scraping library based on LangChain which uses LLM and direct graph logic to create scraping pipelines."
 authors = [
     { name = "Marco Vinciguerra", email = "mvincig11@gmail.com" },
     { name = "Marco Perini", email = "perinim.98@gmail.com" },
     { name = "Lorenzo Padoan", email = "lorenzo.padoan977@gmail.com" }
 ]
```

### Comparing `scrapegraphai-1.2.0/PKG-INFO` & `scrapegraphai-1.2.0b1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: scrapegraphai
-Version: 1.2.0
+Version: 1.2.0b1
 Summary: A web scraping library based on LangChain which uses LLM and direct graph logic to create scraping pipelines.
 Author-email: Marco Vinciguerra <mvincig11@gmail.com>, Marco Perini <perinim.98@gmail.com>, Lorenzo Padoan <lorenzo.padoan977@gmail.com>
 License-Expression: MIT
 License-File: LICENSE
 Keywords: ai,artificial intelligence,gpt,graph,langchain,machine learning,natural language processing,nlp,openai,rag,scrapegraph,scrapegraphai,scraping,web scraping,web scraping library,web scraping tool,webscraping
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
```

