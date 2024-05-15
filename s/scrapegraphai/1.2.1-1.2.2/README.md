# Comparing `tmp/scrapegraphai-1.2.1.tar.gz` & `tmp/scrapegraphai-1.2.2.tar.gz`

## Comparing `scrapegraphai-1.2.1.tar` & `scrapegraphai-1.2.2.tar`

### file list

```diff
@@ -1,248 +1,242 @@
--rw-r--r--   0        0        0       66 2020-02-02 00:00:00.000000 scrapegraphai-1.2.1/.gitattributes
--rw-r--r--   0        0        0     1403 2020-02-02 00:00:00.000000 scrapegraphai-1.2.1/.releaserc.yml
--rw-r--r--   0        0        0    41268 2020-02-02 00:00:00.000000 scrapegraphai-1.2.1/CHANGELOG.md
--rw-r--r--   0        0        0     5221 2020-02-02 00:00:00.000000 scrapegraphai-1.2.1/CODE_OF_CONDUCT.md
--rw-r--r--   0        0        0     3496 2020-02-02 00:00:00.000000 scrapegraphai-1.2.1/CONTRIBUTING.md
--rw-r--r--   0        0        0      138 2020-02-02 00:00:00.000000 scrapegraphai-1.2.1/Dockerfile
--rw-r--r--   0        0        0      117 2020-02-02 00:00:00.000000 scrapegraphai-1.2.1/SECURITY.md
--rw-r--r--   0        0        0      398 2020-02-02 00:00:00.000000 scrapegraphai-1.2.1/citation.cff
--rw-r--r--   0        0        0      224 2020-02-02 00:00:00.000000 scrapegraphai-1.2.1/docker-compose.yml
--rw-r--r--   0        0        0     9317 2020-02-02 00:00:00.000000 scrapegraphai-1.2.1/html_structure
--rw-r--r--   0        0        0   494652 2020-02-02 00:00:00.000000 scrapegraphai-1.2.1/html_structure.png
--rw-r--r--   0        0        0      587 2020-02-02 00:00:00.000000 scrapegraphai-1.2.1/readthedocs.yml
--rw-r--r--   0        0        0       56 2020-02-02 00:00:00.000000 scrapegraphai-1.2.1/requirements-dev.txt
--rw-r--r--   0        0        0      426 2020-02-02 00:00:00.000000 scrapegraphai-1.2.1/requirements.txt
--rw-r--r--   0        0        0      834 2020-02-02 00:00:00.000000 scrapegraphai-1.2.1/.github/ISSUE_TEMPLATE/bug_report.md
--rw-r--r--   0        0        0      126 2020-02-02 00:00:00.000000 scrapegraphai-1.2.1/.github/ISSUE_TEMPLATE/custom.md
--rw-r--r--   0        0        0      595 2020-02-02 00:00:00.000000 scrapegraphai-1.2.1/.github/ISSUE_TEMPLATE/feature_request.md
--rw-r--r--   0        0        0     2593 2020-02-02 00:00:00.000000 scrapegraphai-1.2.1/.github/workflows/codeql.yml
--rw-r--r--   0        0        0     1729 2020-02-02 00:00:00.000000 scrapegraphai-1.2.1/.github/workflows/dependency-review.yml
--rw-r--r--   0        0        0     1067 2020-02-02 00:00:00.000000 scrapegraphai-1.2.1/.github/workflows/pylint.yml
--rw-r--r--   0        0        0      877 2020-02-02 00:00:00.000000 scrapegraphai-1.2.1/.github/workflows/python-publish.yml
--rw-r--r--   0        0        0     2360 2020-02-02 00:00:00.000000 scrapegraphai-1.2.1/.github/workflows/release.yml
--rw-r--r--   0        0        0      638 2020-02-02 00:00:00.000000 scrapegraphai-1.2.1/docs/Makefile
--rw-r--r--   0        0        0     2546 2020-02-02 00:00:00.000000 scrapegraphai-1.2.1/docs/README.md
--rw-r--r--   0        0        0      769 2020-02-02 00:00:00.000000 scrapegraphai-1.2.1/docs/make.bat
--rw-r--r--   0        0        0    60520 2020-02-02 00:00:00.000000 scrapegraphai-1.2.1/docs/assets/apikey_1.png
--rw-r--r--   0        0        0   123826 2020-02-02 00:00:00.000000 scrapegraphai-1.2.1/docs/assets/apikey_2.png
--rw-r--r--   0        0        0    60775 2020-02-02 00:00:00.000000 scrapegraphai-1.2.1/docs/assets/apikey_3.png
--rw-r--r--   0        0        0    86914 2020-02-02 00:00:00.000000 scrapegraphai-1.2.1/docs/assets/apikey_4.png
--rw-r--r--   0        0        0     3526 2020-02-02 00:00:00.000000 scrapegraphai-1.2.1/docs/assets/codespaces-badge.png
--rw-r--r--   0        0        0  1178826 2020-02-02 00:00:00.000000 scrapegraphai-1.2.1/docs/assets/logo_authors.png
--rw-r--r--   0        0        0    73949 2020-02-02 00:00:00.000000 scrapegraphai-1.2.1/docs/assets/omniscrapergraph.png
--rw-r--r--   0        0        0    58062 2020-02-02 00:00:00.000000 scrapegraphai-1.2.1/docs/assets/omnisearchgraph.png
--rw-r--r--   0        0        0    53007 2020-02-02 00:00:00.000000 scrapegraphai-1.2.1/docs/assets/project_overview_diagram.fig
--rw-r--r--   0        0        0    83949 2020-02-02 00:00:00.000000 scrapegraphai-1.2.1/docs/assets/project_overview_diagram.png
--rw-r--r--   0        0        0    33264 2020-02-02 00:00:00.000000 scrapegraphai-1.2.1/docs/assets/scrapegraphai_logo.png
--rw-r--r--   0        0        0    54611 2020-02-02 00:00:00.000000 scrapegraphai-1.2.1/docs/assets/searchgraph.png
--rw-r--r--   0        0        0    15508 2020-02-02 00:00:00.000000 scrapegraphai-1.2.1/docs/assets/serp_api_logo.png
--rw-r--r--   0        0        0    61095 2020-02-02 00:00:00.000000 scrapegraphai-1.2.1/docs/assets/smartscrapergraph.png
--rw-r--r--   0        0        0    49312 2020-02-02 00:00:00.000000 scrapegraphai-1.2.1/docs/assets/speechgraph.png
--rw-r--r--   0        0        0     1737 2020-02-02 00:00:00.000000 scrapegraphai-1.2.1/docs/source/conf.py
--rw-r--r--   0        0        0      753 2020-02-02 00:00:00.000000 scrapegraphai-1.2.1/docs/source/index.rst
--rw-r--r--   0        0        0     2843 2020-02-02 00:00:00.000000 scrapegraphai-1.2.1/docs/source/getting_started/examples.rst
--rw-r--r--   0        0        0     1213 2020-02-02 00:00:00.000000 scrapegraphai-1.2.1/docs/source/getting_started/installation.rst
--rw-r--r--   0        0        0      523 2020-02-02 00:00:00.000000 scrapegraphai-1.2.1/docs/source/introduction/contributing.rst
--rw-r--r--   0        0        0     1689 2020-02-02 00:00:00.000000 scrapegraphai-1.2.1/docs/source/introduction/overview.rst
--rw-r--r--   0        0        0       47 2020-02-02 00:00:00.000000 scrapegraphai-1.2.1/docs/source/modules/modules.rst
--rw-r--r--   0        0        0      603 2020-02-02 00:00:00.000000 scrapegraphai-1.2.1/docs/source/modules/scrapegraphai.graphs.rst
--rw-r--r--   0        0        0     1410 2020-02-02 00:00:00.000000 scrapegraphai-1.2.1/docs/source/modules/scrapegraphai.nodes.rst
--rw-r--r--   0        0        0     2137 2020-02-02 00:00:00.000000 scrapegraphai-1.2.1/docs/source/modules/scrapegraphai.rst
--rw-r--r--   0        0        0      532 2020-02-02 00:00:00.000000 scrapegraphai-1.2.1/docs/source/scrapers/benchmarks.rst
--rw-r--r--   0        0        0     1868 2020-02-02 00:00:00.000000 scrapegraphai-1.2.1/docs/source/scrapers/graph_config.rst
--rw-r--r--   0        0        0     5646 2020-02-02 00:00:00.000000 scrapegraphai-1.2.1/docs/source/scrapers/graphs.rst
--rw-r--r--   0        0        0     5568 2020-02-02 00:00:00.000000 scrapegraphai-1.2.1/docs/source/scrapers/llm.rst
--rw-r--r--   0        0        0     4500 2020-02-02 00:00:00.000000 scrapegraphai-1.2.1/examples/custom_graph_domtree.py
--rw-r--r--   0        0        0     4011 2020-02-02 00:00:00.000000 scrapegraphai-1.2.1/examples/domtree_example.py
--rw-r--r--   0        0        0     1032 2020-02-02 00:00:00.000000 scrapegraphai-1.2.1/examples/faiss_vector.py
--rw-r--r--   0        0        0     2360 2020-02-02 00:00:00.000000 scrapegraphai-1.2.1/examples/readme.md
--rw-r--r--   0        0        0     2051 2020-02-02 00:00:00.000000 scrapegraphai-1.2.1/examples/anthropic/smart_scraper_haiku.py
--rw-r--r--   0        0        0     2053 2020-02-02 00:00:00.000000 scrapegraphai-1.2.1/examples/azure/json_scraper_azure.py
--rw-r--r--   0        0        0     1929 2020-02-02 00:00:00.000000 scrapegraphai-1.2.1/examples/azure/search_graph_azure.py
--rw-r--r--   0        0        0     2164 2020-02-02 00:00:00.000000 scrapegraphai-1.2.1/examples/azure/smart_scraper_azure_openai.py
--rw-r--r--   0        0        0     2047 2020-02-02 00:00:00.000000 scrapegraphai-1.2.1/examples/azure/xml_scraper_azure.py
--rw-r--r--   0        0        0     4429 2020-02-02 00:00:00.000000 scrapegraphai-1.2.1/examples/azure/inputs/books.xml
--rw-r--r--   0        0        0     6455 2020-02-02 00:00:00.000000 scrapegraphai-1.2.1/examples/azure/inputs/example.json
--rw-r--r--   0        0        0      176 2020-02-02 00:00:00.000000 scrapegraphai-1.2.1/examples/azure/inputs/username.csv
--rw-r--r--   0        0        0      897 2020-02-02 00:00:00.000000 scrapegraphai-1.2.1/examples/bedrock/smart_scraper_bedrock.py
--rw-r--r--   0        0        0      265 2020-02-02 00:00:00.000000 scrapegraphai-1.2.1/examples/benchmarks/readme.md
--rw-r--r--   0        0        0       36 2020-02-02 00:00:00.000000 scrapegraphai-1.2.1/examples/benchmarks/GenerateScraper/.env.example
--rw-r--r--   0        0        0     2888 2020-02-02 00:00:00.000000 scrapegraphai-1.2.1/examples/benchmarks/GenerateScraper/Readme.md
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 scrapegraphai-1.2.1/examples/benchmarks/GenerateScraper/benchmark_docker.py
--rw-r--r--   0        0        0     1773 2020-02-02 00:00:00.000000 scrapegraphai-1.2.1/examples/benchmarks/GenerateScraper/benchmark_groq.py
--rw-r--r--   0        0        0     1770 2020-02-02 00:00:00.000000 scrapegraphai-1.2.1/examples/benchmarks/GenerateScraper/benchmark_llama3.py
--rw-r--r--   0        0        0     1862 2020-02-02 00:00:00.000000 scrapegraphai-1.2.1/examples/benchmarks/GenerateScraper/benchmark_mistral.py
--rw-r--r--   0        0        0     1554 2020-02-02 00:00:00.000000 scrapegraphai-1.2.1/examples/benchmarks/GenerateScraper/benchmark_openai_gpt35.py
--rw-r--r--   0        0        0     1563 2020-02-02 00:00:00.000000 scrapegraphai-1.2.1/examples/benchmarks/GenerateScraper/benchmark_openai_gpt4.py
--rw-r--r--   0        0        0     7305 2020-02-02 00:00:00.000000 scrapegraphai-1.2.1/examples/benchmarks/GenerateScraper/inputs/example_1.txt
--rw-r--r--   0        0        0  2590773 2020-02-02 00:00:00.000000 scrapegraphai-1.2.1/examples/benchmarks/GenerateScraper/inputs/example_2.txt
--rw-r--r--   0        0        0       36 2020-02-02 00:00:00.000000 scrapegraphai-1.2.1/examples/benchmarks/SmartScraper/.env.example
--rw-r--r--   0        0        0     2914 2020-02-02 00:00:00.000000 scrapegraphai-1.2.1/examples/benchmarks/SmartScraper/Readme.md
--rw-r--r--   0        0        0     1539 2020-02-02 00:00:00.000000 scrapegraphai-1.2.1/examples/benchmarks/SmartScraper/benchmark_docker.py
--rw-r--r--   0        0        0     1615 2020-02-02 00:00:00.000000 scrapegraphai-1.2.1/examples/benchmarks/SmartScraper/benchmark_groq.py
--rw-r--r--   0        0        0     1630 2020-02-02 00:00:00.000000 scrapegraphai-1.2.1/examples/benchmarks/SmartScraper/benchmark_llama3.py
--rw-r--r--   0        0        0     1641 2020-02-02 00:00:00.000000 scrapegraphai-1.2.1/examples/benchmarks/SmartScraper/benchmark_mistral.py
--rw-r--r--   0        0        0     1520 2020-02-02 00:00:00.000000 scrapegraphai-1.2.1/examples/benchmarks/SmartScraper/benchmark_openai_gpt35.py
--rw-r--r--   0        0        0     1519 2020-02-02 00:00:00.000000 scrapegraphai-1.2.1/examples/benchmarks/SmartScraper/benchmark_openai_gpt4.py
--rw-r--r--   0        0        0     7305 2020-02-02 00:00:00.000000 scrapegraphai-1.2.1/examples/benchmarks/SmartScraper/inputs/example_1.txt
--rw-r--r--   0        0        0  2590773 2020-02-02 00:00:00.000000 scrapegraphai-1.2.1/examples/benchmarks/SmartScraper/inputs/example_2.txt
--rw-r--r--   0        0        0       35 2020-02-02 00:00:00.000000 scrapegraphai-1.2.1/examples/deepseek/.env.example
--rw-r--r--   0        0        0     1665 2020-02-02 00:00:00.000000 scrapegraphai-1.2.1/examples/deepseek/csv_scraper_deepseek.py
--rw-r--r--   0        0        0     1723 2020-02-02 00:00:00.000000 scrapegraphai-1.2.1/examples/deepseek/json_scraper_deepseek.py
--rw-r--r--   0        0        0     1309 2020-02-02 00:00:00.000000 scrapegraphai-1.2.1/examples/deepseek/script_generator_deepseek.py
--rw-r--r--   0        0        0     1238 2020-02-02 00:00:00.000000 scrapegraphai-1.2.1/examples/deepseek/search_graph_deepseek.py
--rw-r--r--   0        0        0     1289 2020-02-02 00:00:00.000000 scrapegraphai-1.2.1/examples/deepseek/smart_scarper_deepseek.py
--rw-r--r--   0        0        0     1714 2020-02-02 00:00:00.000000 scrapegraphai-1.2.1/examples/deepseek/xml_scraper_deepseek.py
--rw-r--r--   0        0        0     4429 2020-02-02 00:00:00.000000 scrapegraphai-1.2.1/examples/deepseek/inputs/books.xml
--rw-r--r--   0        0        0     6455 2020-02-02 00:00:00.000000 scrapegraphai-1.2.1/examples/deepseek/inputs/example.json
--rw-r--r--   0        0        0      176 2020-02-02 00:00:00.000000 scrapegraphai-1.2.1/examples/deepseek/inputs/username.csv
--rw-r--r--   0        0        0       36 2020-02-02 00:00:00.000000 scrapegraphai-1.2.1/examples/gemini/.env.example
--rw-r--r--   0        0        0     1447 2020-02-02 00:00:00.000000 scrapegraphai-1.2.1/examples/gemini/csv_scraper_gemini.py
--rw-r--r--   0        0        0     2120 2020-02-02 00:00:00.000000 scrapegraphai-1.2.1/examples/gemini/custom_graph_gemini.py
--rw-r--r--   0        0        0     1629 2020-02-02 00:00:00.000000 scrapegraphai-1.2.1/examples/gemini/json_scraper_gemini.py
--rw-r--r--   0        0        0      211 2020-02-02 00:00:00.000000 scrapegraphai-1.2.1/examples/gemini/readme.md
--rw-r--r--   0        0        0     1556 2020-02-02 00:00:00.000000 scrapegraphai-1.2.1/examples/gemini/scrape_plain_text_gemini.py
--rw-r--r--   0        0        0     1557 2020-02-02 00:00:00.000000 scrapegraphai-1.2.1/examples/gemini/scrape_xml_gemini.py
--rw-r--r--   0        0        0     1230 2020-02-02 00:00:00.000000 scrapegraphai-1.2.1/examples/gemini/script_generator_gemini.py
--rw-r--r--   0        0        0      964 2020-02-02 00:00:00.000000 scrapegraphai-1.2.1/examples/gemini/search_graph_gemini.py
--rw-r--r--   0        0        0     1175 2020-02-02 00:00:00.000000 scrapegraphai-1.2.1/examples/gemini/smart_scraper_gemini.py
--rw-r--r--   0        0        0     1617 2020-02-02 00:00:00.000000 scrapegraphai-1.2.1/examples/gemini/xml_scraper_openai.py
--rw-r--r--   0        0        0     4429 2020-02-02 00:00:00.000000 scrapegraphai-1.2.1/examples/gemini/inputs/books.xml
--rw-r--r--   0        0        0     6455 2020-02-02 00:00:00.000000 scrapegraphai-1.2.1/examples/gemini/inputs/example.json
--rw-r--r--   0        0        0     7305 2020-02-02 00:00:00.000000 scrapegraphai-1.2.1/examples/gemini/inputs/plain_html_example.txt
--rw-r--r--   0        0        0      176 2020-02-02 00:00:00.000000 scrapegraphai-1.2.1/examples/gemini/inputs/username.csv
--rw-r--r--   0        0        0       64 2020-02-02 00:00:00.000000 scrapegraphai-1.2.1/examples/groq/.env.example
--rw-r--r--   0        0        0     1054 2020-02-02 00:00:00.000000 scrapegraphai-1.2.1/examples/groq/search_graph_groq_openai.py
--rw-r--r--   0        0        0     1414 2020-02-02 00:00:00.000000 scrapegraphai-1.2.1/examples/groq/smart_scraper_groq_ollama.py
--rw-r--r--   0        0        0     1366 2020-02-02 00:00:00.000000 scrapegraphai-1.2.1/examples/groq/smart_scraper_groq_openai.py
--rw-r--r--   0        0        0     2062 2020-02-02 00:00:00.000000 scrapegraphai-1.2.1/examples/huggingfacehub/smart_scraper_huggingfacehub.py
--rw-r--r--   0        0        0     1838 2020-02-02 00:00:00.000000 scrapegraphai-1.2.1/examples/local_models/csv_scraper_ollama.py
--rw-r--r--   0        0        0     1942 2020-02-02 00:00:00.000000 scrapegraphai-1.2.1/examples/local_models/json_scraper_ollama.py
--rw-r--r--   0        0        0     1752 2020-02-02 00:00:00.000000 scrapegraphai-1.2.1/examples/local_models/scrape_plain_text_ollama.py
--rw-r--r--   0        0        0     1832 2020-02-02 00:00:00.000000 scrapegraphai-1.2.1/examples/local_models/scrape_xml_ollama.py
--rw-r--r--   0        0        0     1465 2020-02-02 00:00:00.000000 scrapegraphai-1.2.1/examples/local_models/script_generator_ollama.py
--rw-r--r--   0        0        0     1401 2020-02-02 00:00:00.000000 scrapegraphai-1.2.1/examples/local_models/search_graph_ollama.py
--rw-r--r--   0        0        0     1407 2020-02-02 00:00:00.000000 scrapegraphai-1.2.1/examples/local_models/smart_scraper_ollama.py
--rw-r--r--   0        0        0     1929 2020-02-02 00:00:00.000000 scrapegraphai-1.2.1/examples/local_models/xml_scraper_ollama.py
--rw-r--r--   0        0        0     4429 2020-02-02 00:00:00.000000 scrapegraphai-1.2.1/examples/local_models/inputs/books.xml
--rw-r--r--   0        0        0     6455 2020-02-02 00:00:00.000000 scrapegraphai-1.2.1/examples/local_models/inputs/example.json
--rw-r--r--   0        0        0     7305 2020-02-02 00:00:00.000000 scrapegraphai-1.2.1/examples/local_models/inputs/plain_html_example.txt
--rw-r--r--   0        0        0      176 2020-02-02 00:00:00.000000 scrapegraphai-1.2.1/examples/local_models/inputs/username.csv
--rw-r--r--   0        0        0      208 2020-02-02 00:00:00.000000 scrapegraphai-1.2.1/examples/mixed_models/.env.example
--rw-r--r--   0        0        0      201 2020-02-02 00:00:00.000000 scrapegraphai-1.2.1/examples/mixed_models/readme.md
--rw-r--r--   0        0        0     1357 2020-02-02 00:00:00.000000 scrapegraphai-1.2.1/examples/mixed_models/search_graph_groq_ollama.py
--rw-r--r--   0        0        0     1448 2020-02-02 00:00:00.000000 scrapegraphai-1.2.1/examples/mixed_models/smart_scraper_mixed.py
--rw-r--r--   0        0        0     4429 2020-02-02 00:00:00.000000 scrapegraphai-1.2.1/examples/mixed_models/inputs/books.xml
--rw-r--r--   0        0        0     6455 2020-02-02 00:00:00.000000 scrapegraphai-1.2.1/examples/mixed_models/inputs/example.json
--rw-r--r--   0        0        0     7305 2020-02-02 00:00:00.000000 scrapegraphai-1.2.1/examples/mixed_models/inputs/plain_html_example.txt
--rw-r--r--   0        0        0       39 2020-02-02 00:00:00.000000 scrapegraphai-1.2.1/examples/openai/.env.example
--rw-r--r--   0        0        0     1574 2020-02-02 00:00:00.000000 scrapegraphai-1.2.1/examples/openai/csv_scraper_openai.py
--rw-r--r--   0        0        0     2688 2020-02-02 00:00:00.000000 scrapegraphai-1.2.1/examples/openai/custom_graph_openai.py
--rw-r--r--   0        0        0     1321 2020-02-02 00:00:00.000000 scrapegraphai-1.2.1/examples/openai/deep_scraper_openai.py
--rw-r--r--   0        0        0     1633 2020-02-02 00:00:00.000000 scrapegraphai-1.2.1/examples/openai/json_scraper_openai.py
--rw-r--r--   0        0        0     1307 2020-02-02 00:00:00.000000 scrapegraphai-1.2.1/examples/openai/omni_scraper_openai.py
--rw-r--r--   0        0        0     1142 2020-02-02 00:00:00.000000 scrapegraphai-1.2.1/examples/openai/omni_search_graph_openai.py
--rw-r--r--   0        0        0      203 2020-02-02 00:00:00.000000 scrapegraphai-1.2.1/examples/openai/readme.md
--rw-r--r--   0        0        0     1512 2020-02-02 00:00:00.000000 scrapegraphai-1.2.1/examples/openai/scrape_plain_text_openai.py
--rw-r--r--   0        0        0     1239 2020-02-02 00:00:00.000000 scrapegraphai-1.2.1/examples/openai/script_generator_openai.py
--rw-r--r--   0        0        0     1160 2020-02-02 00:00:00.000000 scrapegraphai-1.2.1/examples/openai/search_graph_openai.py
--rw-r--r--   0        0        0     1233 2020-02-02 00:00:00.000000 scrapegraphai-1.2.1/examples/openai/smart_scraper_openai.py
--rw-r--r--   0        0        0     1531 2020-02-02 00:00:00.000000 scrapegraphai-1.2.1/examples/openai/speech_graph_openai.py
--rw-r--r--   0        0        0     1642 2020-02-02 00:00:00.000000 scrapegraphai-1.2.1/examples/openai/xml_scraper_openai.py
--rw-r--r--   0        0        0     4429 2020-02-02 00:00:00.000000 scrapegraphai-1.2.1/examples/openai/inputs/books.xml
--rw-r--r--   0        0        0     6455 2020-02-02 00:00:00.000000 scrapegraphai-1.2.1/examples/openai/inputs/example.json
--rw-r--r--   0        0        0     7305 2020-02-02 00:00:00.000000 scrapegraphai-1.2.1/examples/openai/inputs/plain_html_example.txt
--rw-r--r--   0        0        0      176 2020-02-02 00:00:00.000000 scrapegraphai-1.2.1/examples/openai/inputs/username.csv
--rw-r--r--   0        0        0      567 2020-02-02 00:00:00.000000 scrapegraphai-1.2.1/examples/single_node/fetch_node.py
--rw-r--r--   0        0        0     1199 2020-02-02 00:00:00.000000 scrapegraphai-1.2.1/examples/single_node/image2text_node.py
--rw-r--r--   0        0        0      961 2020-02-02 00:00:00.000000 scrapegraphai-1.2.1/examples/single_node/robot_node.py
--rwxr-xr-x   0        0        0      986 2020-02-02 00:00:00.000000 scrapegraphai-1.2.1/manual deployment/commit_and_push.sh
--rwxr-xr-x   0        0        0      611 2020-02-02 00:00:00.000000 scrapegraphai-1.2.1/manual deployment/commit_and_push_with_tests.sh
--rwxr-xr-x   0        0        0      169 2020-02-02 00:00:00.000000 scrapegraphai-1.2.1/manual deployment/deploy_on_pip.sh
--rw-r--r--   0        0        0       90 2020-02-02 00:00:00.000000 scrapegraphai-1.2.1/manual deployment/rye_update.sh
--rw-r--r--   0        0        0       54 2020-02-02 00:00:00.000000 scrapegraphai-1.2.1/scrapegraphai/__init__.py
--rw-r--r--   0        0        0      587 2020-02-02 00:00:00.000000 scrapegraphai-1.2.1/scrapegraphai/graphs/__init__.py
--rw-r--r--   0        0        0    13691 2020-02-02 00:00:00.000000 scrapegraphai-1.2.1/scrapegraphai/graphs/abstract_graph.py
--rw-r--r--   0        0        0     5378 2020-02-02 00:00:00.000000 scrapegraphai-1.2.1/scrapegraphai/graphs/base_graph.py
--rw-r--r--   0        0        0     2472 2020-02-02 00:00:00.000000 scrapegraphai-1.2.1/scrapegraphai/graphs/csv_scraper_graph.py
--rw-r--r--   0        0        0     3392 2020-02-02 00:00:00.000000 scrapegraphai-1.2.1/scrapegraphai/graphs/json_scraper_graph.py
--rw-r--r--   0        0        0     4295 2020-02-02 00:00:00.000000 scrapegraphai-1.2.1/scrapegraphai/graphs/omni_scraper_graph.py
--rw-r--r--   0        0        0     3714 2020-02-02 00:00:00.000000 scrapegraphai-1.2.1/scrapegraphai/graphs/omni_search_graph.py
--rw-r--r--   0        0        0     3538 2020-02-02 00:00:00.000000 scrapegraphai-1.2.1/scrapegraphai/graphs/pdf_scraper_graph.py
--rw-r--r--   0        0        0     3371 2020-02-02 00:00:00.000000 scrapegraphai-1.2.1/scrapegraphai/graphs/script_creator_graph.py
--rw-r--r--   0        0        0     3638 2020-02-02 00:00:00.000000 scrapegraphai-1.2.1/scrapegraphai/graphs/search_graph.py
--rw-r--r--   0        0        0     3651 2020-02-02 00:00:00.000000 scrapegraphai-1.2.1/scrapegraphai/graphs/smart_scraper_graph.py
--rw-r--r--   0        0        0     4322 2020-02-02 00:00:00.000000 scrapegraphai-1.2.1/scrapegraphai/graphs/speech_graph.py
--rw-r--r--   0        0        0     3534 2020-02-02 00:00:00.000000 scrapegraphai-1.2.1/scrapegraphai/graphs/xml_scraper_graph.py
--rw-r--r--   0        0        0      202 2020-02-02 00:00:00.000000 scrapegraphai-1.2.1/scrapegraphai/helpers/__init__.py
--rw-r--r--   0        0        0     4203 2020-02-02 00:00:00.000000 scrapegraphai-1.2.1/scrapegraphai/helpers/models_tokens.py
--rw-r--r--   0        0        0     3807 2020-02-02 00:00:00.000000 scrapegraphai-1.2.1/scrapegraphai/helpers/nodes_metadata.py
--rw-r--r--   0        0        0      310 2020-02-02 00:00:00.000000 scrapegraphai-1.2.1/scrapegraphai/helpers/robots.py
--rw-r--r--   0        0        0     2363 2020-02-02 00:00:00.000000 scrapegraphai-1.2.1/scrapegraphai/helpers/schemas.py
--rw-r--r--   0        0        0      406 2020-02-02 00:00:00.000000 scrapegraphai-1.2.1/scrapegraphai/models/__init__.py
--rw-r--r--   0        0        0      429 2020-02-02 00:00:00.000000 scrapegraphai-1.2.1/scrapegraphai/models/anthropic.py
--rw-r--r--   0        0        0      441 2020-02-02 00:00:00.000000 scrapegraphai-1.2.1/scrapegraphai/models/azure_openai.py
--rw-r--r--   0        0        0      579 2020-02-02 00:00:00.000000 scrapegraphai-1.2.1/scrapegraphai/models/bedrock.py
--rw-r--r--   0        0        0      455 2020-02-02 00:00:00.000000 scrapegraphai-1.2.1/scrapegraphai/models/deepseek.py
--rw-r--r--   0        0        0      606 2020-02-02 00:00:00.000000 scrapegraphai-1.2.1/scrapegraphai/models/gemini.py
--rw-r--r--   0        0        0      426 2020-02-02 00:00:00.000000 scrapegraphai-1.2.1/scrapegraphai/models/groq.py
--rw-r--r--   0        0        0      459 2020-02-02 00:00:00.000000 scrapegraphai-1.2.1/scrapegraphai/models/hugging_face.py
--rw-r--r--   0        0        0      427 2020-02-02 00:00:00.000000 scrapegraphai-1.2.1/scrapegraphai/models/ollama.py
--rw-r--r--   0        0        0      412 2020-02-02 00:00:00.000000 scrapegraphai-1.2.1/scrapegraphai/models/openai.py
--rw-r--r--   0        0        0     1367 2020-02-02 00:00:00.000000 scrapegraphai-1.2.1/scrapegraphai/models/openai_itt.py
--rw-r--r--   0        0        0     1221 2020-02-02 00:00:00.000000 scrapegraphai-1.2.1/scrapegraphai/models/openai_tts.py
--rw-r--r--   0        0        0      959 2020-02-02 00:00:00.000000 scrapegraphai-1.2.1/scrapegraphai/nodes/__init__.py
--rw-r--r--   0        0        0     8591 2020-02-02 00:00:00.000000 scrapegraphai-1.2.1/scrapegraphai/nodes/base_node.py
--rw-r--r--   0        0        0     2370 2020-02-02 00:00:00.000000 scrapegraphai-1.2.1/scrapegraphai/nodes/blocks_identifier.py
--rw-r--r--   0        0        0     2914 2020-02-02 00:00:00.000000 scrapegraphai-1.2.1/scrapegraphai/nodes/conditional_node.py
--rw-r--r--   0        0        0     6450 2020-02-02 00:00:00.000000 scrapegraphai-1.2.1/scrapegraphai/nodes/fetch_node.py
--rw-r--r--   0        0        0     7182 2020-02-02 00:00:00.000000 scrapegraphai-1.2.1/scrapegraphai/nodes/generate_answer_csv_node.py
--rw-r--r--   0        0        0     6612 2020-02-02 00:00:00.000000 scrapegraphai-1.2.1/scrapegraphai/nodes/generate_answer_node.py
--rw-r--r--   0        0        0     7064 2020-02-02 00:00:00.000000 scrapegraphai-1.2.1/scrapegraphai/nodes/generate_answer_omni_node.py
--rw-r--r--   0        0        0     7158 2020-02-02 00:00:00.000000 scrapegraphai-1.2.1/scrapegraphai/nodes/generate_answer_pdf_node.py
--rw-r--r--   0        0        0     4340 2020-02-02 00:00:00.000000 scrapegraphai-1.2.1/scrapegraphai/nodes/generate_scraper_node.py
--rw-r--r--   0        0        0     3537 2020-02-02 00:00:00.000000 scrapegraphai-1.2.1/scrapegraphai/nodes/get_probable_tags_node.py
--rw-r--r--   0        0        0     4395 2020-02-02 00:00:00.000000 scrapegraphai-1.2.1/scrapegraphai/nodes/graph_iterator_node.py
--rw-r--r--   0        0        0     2671 2020-02-02 00:00:00.000000 scrapegraphai-1.2.1/scrapegraphai/nodes/image_to_text_node.py
--rw-r--r--   0        0        0     3890 2020-02-02 00:00:00.000000 scrapegraphai-1.2.1/scrapegraphai/nodes/merge_answers_node.py
--rw-r--r--   0        0        0     2930 2020-02-02 00:00:00.000000 scrapegraphai-1.2.1/scrapegraphai/nodes/parse_node.py
--rw-r--r--   0        0        0     4496 2020-02-02 00:00:00.000000 scrapegraphai-1.2.1/scrapegraphai/nodes/rag_node.py
--rw-r--r--   0        0        0     6072 2020-02-02 00:00:00.000000 scrapegraphai-1.2.1/scrapegraphai/nodes/robots_node.py
--rw-r--r--   0        0        0     4185 2020-02-02 00:00:00.000000 scrapegraphai-1.2.1/scrapegraphai/nodes/search_internet_node.py
--rw-r--r--   0        0        0     4181 2020-02-02 00:00:00.000000 scrapegraphai-1.2.1/scrapegraphai/nodes/search_link_node.py
--rw-r--r--   0        0        0     4913 2020-02-02 00:00:00.000000 scrapegraphai-1.2.1/scrapegraphai/nodes/search_node_with_context.py
--rw-r--r--   0        0        0     2343 2020-02-02 00:00:00.000000 scrapegraphai-1.2.1/scrapegraphai/nodes/text_to_speech_node.py
--rw-r--r--   0        0        0      424 2020-02-02 00:00:00.000000 scrapegraphai-1.2.1/scrapegraphai/utils/__init__.py
--rw-r--r--   0        0        0     7705 2020-02-02 00:00:00.000000 scrapegraphai-1.2.1/scrapegraphai/utils/aaa.py
--rw-r--r--   0        0        0     5791 2020-02-02 00:00:00.000000 scrapegraphai-1.2.1/scrapegraphai/utils/asdt.py
--rw-r--r--   0        0        0     2330 2020-02-02 00:00:00.000000 scrapegraphai-1.2.1/scrapegraphai/utils/cleanup_html.py
--rw-r--r--   0        0        0     2141 2020-02-02 00:00:00.000000 scrapegraphai-1.2.1/scrapegraphai/utils/convert_to_csv.py
--rw-r--r--   0        0        0     1974 2020-02-02 00:00:00.000000 scrapegraphai-1.2.1/scrapegraphai/utils/convert_to_json.py
--rw-r--r--   0        0        0     4638 2020-02-02 00:00:00.000000 scrapegraphai-1.2.1/scrapegraphai/utils/parse_state_keys.py
--rw-r--r--   0        0        0      764 2020-02-02 00:00:00.000000 scrapegraphai-1.2.1/scrapegraphai/utils/prettify_exec_info.py
--rw-r--r--   0        0        0     6404 2020-02-02 00:00:00.000000 scrapegraphai-1.2.1/scrapegraphai/utils/proxy_rotation.py
--rw-r--r--   0        0        0     2140 2020-02-02 00:00:00.000000 scrapegraphai-1.2.1/scrapegraphai/utils/research_web.py
--rw-r--r--   0        0        0      836 2020-02-02 00:00:00.000000 scrapegraphai-1.2.1/scrapegraphai/utils/save_audio_from_bytes.py
--rw-r--r--   0        0        0     1702 2020-02-02 00:00:00.000000 scrapegraphai-1.2.1/scrapegraphai/utils/sys_dynamic_import.py
--rw-r--r--   0        0        0     1320 2020-02-02 00:00:00.000000 scrapegraphai-1.2.1/scrapegraphai/utils/token_calculator.py
--rw-r--r--   0        0        0     1997 2020-02-02 00:00:00.000000 scrapegraphai-1.2.1/scrapegraphai/utils/tree_base.py
--rw-r--r--   0        0        0      417 2020-02-02 00:00:00.000000 scrapegraphai-1.2.1/tests/Readme.md
--rw-r--r--   0        0        0     1220 2020-02-02 00:00:00.000000 scrapegraphai-1.2.1/tests/graphs/scrape_json_ollama.py
--rw-r--r--   0        0        0     1238 2020-02-02 00:00:00.000000 scrapegraphai-1.2.1/tests/graphs/scrape_plain_text_llama3_test.py
--rw-r--r--   0        0        0     1239 2020-02-02 00:00:00.000000 scrapegraphai-1.2.1/tests/graphs/scrape_plain_text_mistral_test.py
--rw-r--r--   0        0        0     1243 2020-02-02 00:00:00.000000 scrapegraphai-1.2.1/tests/graphs/scrape_xml_ollama_test.py
--rw-r--r--   0        0        0     1223 2020-02-02 00:00:00.000000 scrapegraphai-1.2.1/tests/graphs/script_generator_test.py
--rw-r--r--   0        0        0     1350 2020-02-02 00:00:00.000000 scrapegraphai-1.2.1/tests/graphs/smart_scraper_ollama_test.py
--rw-r--r--   0        0        0     4429 2020-02-02 00:00:00.000000 scrapegraphai-1.2.1/tests/graphs/inputs/books.xml
--rw-r--r--   0        0        0     6455 2020-02-02 00:00:00.000000 scrapegraphai-1.2.1/tests/graphs/inputs/example.json
--rw-r--r--   0        0        0     7305 2020-02-02 00:00:00.000000 scrapegraphai-1.2.1/tests/graphs/inputs/plain_html_example.txt
--rw-r--r--   0        0        0      176 2020-02-02 00:00:00.000000 scrapegraphai-1.2.1/tests/graphs/inputs/username.csv
--rw-r--r--   0        0        0      771 2020-02-02 00:00:00.000000 scrapegraphai-1.2.1/tests/nodes/fetch_node_test.py
--rw-r--r--   0        0        0     1207 2020-02-02 00:00:00.000000 scrapegraphai-1.2.1/tests/nodes/robot_node_test.py
--rw-r--r--   0        0        0     2961 2020-02-02 00:00:00.000000 scrapegraphai-1.2.1/tests/utils/test_proxy_rotation.py
--rw-r--r--   0        0        0     2203 2020-02-02 00:00:00.000000 scrapegraphai-1.2.1/tests/utils/test_sys_dynamic_import.py
--rw-r--r--   0        0        0      448 2020-02-02 00:00:00.000000 scrapegraphai-1.2.1/.gitignore
--rw-r--r--   0        0        0     1065 2020-02-02 00:00:00.000000 scrapegraphai-1.2.1/LICENSE
--rw-r--r--   0        0        0     8967 2020-02-02 00:00:00.000000 scrapegraphai-1.2.1/README.md
--rw-r--r--   0        0        0     2007 2020-02-02 00:00:00.000000 scrapegraphai-1.2.1/pyproject.toml
--rw-r--r--   0        0        0    10486 2020-02-02 00:00:00.000000 scrapegraphai-1.2.1/PKG-INFO
+-rw-r--r--   0        0        0       66 2020-02-02 00:00:00.000000 scrapegraphai-1.2.2/.gitattributes
+-rw-r--r--   0        0        0     1403 2020-02-02 00:00:00.000000 scrapegraphai-1.2.2/.releaserc.yml
+-rw-r--r--   0        0        0    41517 2020-02-02 00:00:00.000000 scrapegraphai-1.2.2/CHANGELOG.md
+-rw-r--r--   0        0        0     5221 2020-02-02 00:00:00.000000 scrapegraphai-1.2.2/CODE_OF_CONDUCT.md
+-rw-r--r--   0        0        0     3496 2020-02-02 00:00:00.000000 scrapegraphai-1.2.2/CONTRIBUTING.md
+-rw-r--r--   0        0        0      138 2020-02-02 00:00:00.000000 scrapegraphai-1.2.2/Dockerfile
+-rw-r--r--   0        0        0      117 2020-02-02 00:00:00.000000 scrapegraphai-1.2.2/SECURITY.md
+-rw-r--r--   0        0        0      398 2020-02-02 00:00:00.000000 scrapegraphai-1.2.2/citation.cff
+-rw-r--r--   0        0        0      224 2020-02-02 00:00:00.000000 scrapegraphai-1.2.2/docker-compose.yml
+-rw-r--r--   0        0        0      587 2020-02-02 00:00:00.000000 scrapegraphai-1.2.2/readthedocs.yml
+-rw-r--r--   0        0        0       56 2020-02-02 00:00:00.000000 scrapegraphai-1.2.2/requirements-dev.txt
+-rw-r--r--   0        0        0      426 2020-02-02 00:00:00.000000 scrapegraphai-1.2.2/requirements.txt
+-rw-r--r--   0        0        0      834 2020-02-02 00:00:00.000000 scrapegraphai-1.2.2/.github/ISSUE_TEMPLATE/bug_report.md
+-rw-r--r--   0        0        0      126 2020-02-02 00:00:00.000000 scrapegraphai-1.2.2/.github/ISSUE_TEMPLATE/custom.md
+-rw-r--r--   0        0        0      595 2020-02-02 00:00:00.000000 scrapegraphai-1.2.2/.github/ISSUE_TEMPLATE/feature_request.md
+-rw-r--r--   0        0        0     2593 2020-02-02 00:00:00.000000 scrapegraphai-1.2.2/.github/workflows/codeql.yml
+-rw-r--r--   0        0        0     1729 2020-02-02 00:00:00.000000 scrapegraphai-1.2.2/.github/workflows/dependency-review.yml
+-rw-r--r--   0        0        0     1067 2020-02-02 00:00:00.000000 scrapegraphai-1.2.2/.github/workflows/pylint.yml
+-rw-r--r--   0        0        0      877 2020-02-02 00:00:00.000000 scrapegraphai-1.2.2/.github/workflows/python-publish.yml
+-rw-r--r--   0        0        0     2360 2020-02-02 00:00:00.000000 scrapegraphai-1.2.2/.github/workflows/release.yml
+-rw-r--r--   0        0        0      638 2020-02-02 00:00:00.000000 scrapegraphai-1.2.2/docs/Makefile
+-rw-r--r--   0        0        0     2546 2020-02-02 00:00:00.000000 scrapegraphai-1.2.2/docs/README.md
+-rw-r--r--   0        0        0      769 2020-02-02 00:00:00.000000 scrapegraphai-1.2.2/docs/make.bat
+-rw-r--r--   0        0        0    60520 2020-02-02 00:00:00.000000 scrapegraphai-1.2.2/docs/assets/apikey_1.png
+-rw-r--r--   0        0        0   123826 2020-02-02 00:00:00.000000 scrapegraphai-1.2.2/docs/assets/apikey_2.png
+-rw-r--r--   0        0        0    60775 2020-02-02 00:00:00.000000 scrapegraphai-1.2.2/docs/assets/apikey_3.png
+-rw-r--r--   0        0        0    86914 2020-02-02 00:00:00.000000 scrapegraphai-1.2.2/docs/assets/apikey_4.png
+-rw-r--r--   0        0        0     3526 2020-02-02 00:00:00.000000 scrapegraphai-1.2.2/docs/assets/codespaces-badge.png
+-rw-r--r--   0        0        0  1178826 2020-02-02 00:00:00.000000 scrapegraphai-1.2.2/docs/assets/logo_authors.png
+-rw-r--r--   0        0        0    73949 2020-02-02 00:00:00.000000 scrapegraphai-1.2.2/docs/assets/omniscrapergraph.png
+-rw-r--r--   0        0        0    58062 2020-02-02 00:00:00.000000 scrapegraphai-1.2.2/docs/assets/omnisearchgraph.png
+-rw-r--r--   0        0        0    53007 2020-02-02 00:00:00.000000 scrapegraphai-1.2.2/docs/assets/project_overview_diagram.fig
+-rw-r--r--   0        0        0    83949 2020-02-02 00:00:00.000000 scrapegraphai-1.2.2/docs/assets/project_overview_diagram.png
+-rw-r--r--   0        0        0    33264 2020-02-02 00:00:00.000000 scrapegraphai-1.2.2/docs/assets/scrapegraphai_logo.png
+-rw-r--r--   0        0        0    54611 2020-02-02 00:00:00.000000 scrapegraphai-1.2.2/docs/assets/searchgraph.png
+-rw-r--r--   0        0        0    15508 2020-02-02 00:00:00.000000 scrapegraphai-1.2.2/docs/assets/serp_api_logo.png
+-rw-r--r--   0        0        0    61095 2020-02-02 00:00:00.000000 scrapegraphai-1.2.2/docs/assets/smartscrapergraph.png
+-rw-r--r--   0        0        0    49312 2020-02-02 00:00:00.000000 scrapegraphai-1.2.2/docs/assets/speechgraph.png
+-rw-r--r--   0        0        0     1737 2020-02-02 00:00:00.000000 scrapegraphai-1.2.2/docs/source/conf.py
+-rw-r--r--   0        0        0      753 2020-02-02 00:00:00.000000 scrapegraphai-1.2.2/docs/source/index.rst
+-rw-r--r--   0        0        0     2843 2020-02-02 00:00:00.000000 scrapegraphai-1.2.2/docs/source/getting_started/examples.rst
+-rw-r--r--   0        0        0     1139 2020-02-02 00:00:00.000000 scrapegraphai-1.2.2/docs/source/getting_started/installation.rst
+-rw-r--r--   0        0        0      523 2020-02-02 00:00:00.000000 scrapegraphai-1.2.2/docs/source/introduction/contributing.rst
+-rw-r--r--   0        0        0     1689 2020-02-02 00:00:00.000000 scrapegraphai-1.2.2/docs/source/introduction/overview.rst
+-rw-r--r--   0        0        0       47 2020-02-02 00:00:00.000000 scrapegraphai-1.2.2/docs/source/modules/modules.rst
+-rw-r--r--   0        0        0      603 2020-02-02 00:00:00.000000 scrapegraphai-1.2.2/docs/source/modules/scrapegraphai.graphs.rst
+-rw-r--r--   0        0        0     1410 2020-02-02 00:00:00.000000 scrapegraphai-1.2.2/docs/source/modules/scrapegraphai.nodes.rst
+-rw-r--r--   0        0        0     2137 2020-02-02 00:00:00.000000 scrapegraphai-1.2.2/docs/source/modules/scrapegraphai.rst
+-rw-r--r--   0        0        0      532 2020-02-02 00:00:00.000000 scrapegraphai-1.2.2/docs/source/scrapers/benchmarks.rst
+-rw-r--r--   0        0        0     1868 2020-02-02 00:00:00.000000 scrapegraphai-1.2.2/docs/source/scrapers/graph_config.rst
+-rw-r--r--   0        0        0     5646 2020-02-02 00:00:00.000000 scrapegraphai-1.2.2/docs/source/scrapers/graphs.rst
+-rw-r--r--   0        0        0     5568 2020-02-02 00:00:00.000000 scrapegraphai-1.2.2/docs/source/scrapers/llm.rst
+-rw-r--r--   0        0        0     2360 2020-02-02 00:00:00.000000 scrapegraphai-1.2.2/examples/readme.md
+-rw-r--r--   0        0        0     2051 2020-02-02 00:00:00.000000 scrapegraphai-1.2.2/examples/anthropic/smart_scraper_haiku.py
+-rw-r--r--   0        0        0     2053 2020-02-02 00:00:00.000000 scrapegraphai-1.2.2/examples/azure/json_scraper_azure.py
+-rw-r--r--   0        0        0     1929 2020-02-02 00:00:00.000000 scrapegraphai-1.2.2/examples/azure/search_graph_azure.py
+-rw-r--r--   0        0        0     2164 2020-02-02 00:00:00.000000 scrapegraphai-1.2.2/examples/azure/smart_scraper_azure_openai.py
+-rw-r--r--   0        0        0     2047 2020-02-02 00:00:00.000000 scrapegraphai-1.2.2/examples/azure/xml_scraper_azure.py
+-rw-r--r--   0        0        0     4429 2020-02-02 00:00:00.000000 scrapegraphai-1.2.2/examples/azure/inputs/books.xml
+-rw-r--r--   0        0        0     6455 2020-02-02 00:00:00.000000 scrapegraphai-1.2.2/examples/azure/inputs/example.json
+-rw-r--r--   0        0        0      176 2020-02-02 00:00:00.000000 scrapegraphai-1.2.2/examples/azure/inputs/username.csv
+-rw-r--r--   0        0        0      897 2020-02-02 00:00:00.000000 scrapegraphai-1.2.2/examples/bedrock/smart_scraper_bedrock.py
+-rw-r--r--   0        0        0      265 2020-02-02 00:00:00.000000 scrapegraphai-1.2.2/examples/benchmarks/readme.md
+-rw-r--r--   0        0        0       36 2020-02-02 00:00:00.000000 scrapegraphai-1.2.2/examples/benchmarks/GenerateScraper/.env.example
+-rw-r--r--   0        0        0     2888 2020-02-02 00:00:00.000000 scrapegraphai-1.2.2/examples/benchmarks/GenerateScraper/Readme.md
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 scrapegraphai-1.2.2/examples/benchmarks/GenerateScraper/benchmark_docker.py
+-rw-r--r--   0        0        0     1773 2020-02-02 00:00:00.000000 scrapegraphai-1.2.2/examples/benchmarks/GenerateScraper/benchmark_groq.py
+-rw-r--r--   0        0        0     1770 2020-02-02 00:00:00.000000 scrapegraphai-1.2.2/examples/benchmarks/GenerateScraper/benchmark_llama3.py
+-rw-r--r--   0        0        0     1862 2020-02-02 00:00:00.000000 scrapegraphai-1.2.2/examples/benchmarks/GenerateScraper/benchmark_mistral.py
+-rw-r--r--   0        0        0     1554 2020-02-02 00:00:00.000000 scrapegraphai-1.2.2/examples/benchmarks/GenerateScraper/benchmark_openai_gpt35.py
+-rw-r--r--   0        0        0     1563 2020-02-02 00:00:00.000000 scrapegraphai-1.2.2/examples/benchmarks/GenerateScraper/benchmark_openai_gpt4.py
+-rw-r--r--   0        0        0     7305 2020-02-02 00:00:00.000000 scrapegraphai-1.2.2/examples/benchmarks/GenerateScraper/inputs/example_1.txt
+-rw-r--r--   0        0        0  2590773 2020-02-02 00:00:00.000000 scrapegraphai-1.2.2/examples/benchmarks/GenerateScraper/inputs/example_2.txt
+-rw-r--r--   0        0        0       36 2020-02-02 00:00:00.000000 scrapegraphai-1.2.2/examples/benchmarks/SmartScraper/.env.example
+-rw-r--r--   0        0        0     2914 2020-02-02 00:00:00.000000 scrapegraphai-1.2.2/examples/benchmarks/SmartScraper/Readme.md
+-rw-r--r--   0        0        0     1539 2020-02-02 00:00:00.000000 scrapegraphai-1.2.2/examples/benchmarks/SmartScraper/benchmark_docker.py
+-rw-r--r--   0        0        0     1615 2020-02-02 00:00:00.000000 scrapegraphai-1.2.2/examples/benchmarks/SmartScraper/benchmark_groq.py
+-rw-r--r--   0        0        0     1630 2020-02-02 00:00:00.000000 scrapegraphai-1.2.2/examples/benchmarks/SmartScraper/benchmark_llama3.py
+-rw-r--r--   0        0        0     1641 2020-02-02 00:00:00.000000 scrapegraphai-1.2.2/examples/benchmarks/SmartScraper/benchmark_mistral.py
+-rw-r--r--   0        0        0     1520 2020-02-02 00:00:00.000000 scrapegraphai-1.2.2/examples/benchmarks/SmartScraper/benchmark_openai_gpt35.py
+-rw-r--r--   0        0        0     1519 2020-02-02 00:00:00.000000 scrapegraphai-1.2.2/examples/benchmarks/SmartScraper/benchmark_openai_gpt4.py
+-rw-r--r--   0        0        0     7305 2020-02-02 00:00:00.000000 scrapegraphai-1.2.2/examples/benchmarks/SmartScraper/inputs/example_1.txt
+-rw-r--r--   0        0        0  2590773 2020-02-02 00:00:00.000000 scrapegraphai-1.2.2/examples/benchmarks/SmartScraper/inputs/example_2.txt
+-rw-r--r--   0        0        0       35 2020-02-02 00:00:00.000000 scrapegraphai-1.2.2/examples/deepseek/.env.example
+-rw-r--r--   0        0        0     1665 2020-02-02 00:00:00.000000 scrapegraphai-1.2.2/examples/deepseek/csv_scraper_deepseek.py
+-rw-r--r--   0        0        0     1723 2020-02-02 00:00:00.000000 scrapegraphai-1.2.2/examples/deepseek/json_scraper_deepseek.py
+-rw-r--r--   0        0        0     1309 2020-02-02 00:00:00.000000 scrapegraphai-1.2.2/examples/deepseek/script_generator_deepseek.py
+-rw-r--r--   0        0        0     1238 2020-02-02 00:00:00.000000 scrapegraphai-1.2.2/examples/deepseek/search_graph_deepseek.py
+-rw-r--r--   0        0        0     1289 2020-02-02 00:00:00.000000 scrapegraphai-1.2.2/examples/deepseek/smart_scarper_deepseek.py
+-rw-r--r--   0        0        0     1714 2020-02-02 00:00:00.000000 scrapegraphai-1.2.2/examples/deepseek/xml_scraper_deepseek.py
+-rw-r--r--   0        0        0     4429 2020-02-02 00:00:00.000000 scrapegraphai-1.2.2/examples/deepseek/inputs/books.xml
+-rw-r--r--   0        0        0     6455 2020-02-02 00:00:00.000000 scrapegraphai-1.2.2/examples/deepseek/inputs/example.json
+-rw-r--r--   0        0        0      176 2020-02-02 00:00:00.000000 scrapegraphai-1.2.2/examples/deepseek/inputs/username.csv
+-rw-r--r--   0        0        0       36 2020-02-02 00:00:00.000000 scrapegraphai-1.2.2/examples/gemini/.env.example
+-rw-r--r--   0        0        0     1447 2020-02-02 00:00:00.000000 scrapegraphai-1.2.2/examples/gemini/csv_scraper_gemini.py
+-rw-r--r--   0        0        0     2120 2020-02-02 00:00:00.000000 scrapegraphai-1.2.2/examples/gemini/custom_graph_gemini.py
+-rw-r--r--   0        0        0     1629 2020-02-02 00:00:00.000000 scrapegraphai-1.2.2/examples/gemini/json_scraper_gemini.py
+-rw-r--r--   0        0        0      211 2020-02-02 00:00:00.000000 scrapegraphai-1.2.2/examples/gemini/readme.md
+-rw-r--r--   0        0        0     1556 2020-02-02 00:00:00.000000 scrapegraphai-1.2.2/examples/gemini/scrape_plain_text_gemini.py
+-rw-r--r--   0        0        0     1557 2020-02-02 00:00:00.000000 scrapegraphai-1.2.2/examples/gemini/scrape_xml_gemini.py
+-rw-r--r--   0        0        0     1230 2020-02-02 00:00:00.000000 scrapegraphai-1.2.2/examples/gemini/script_generator_gemini.py
+-rw-r--r--   0        0        0      964 2020-02-02 00:00:00.000000 scrapegraphai-1.2.2/examples/gemini/search_graph_gemini.py
+-rw-r--r--   0        0        0     1175 2020-02-02 00:00:00.000000 scrapegraphai-1.2.2/examples/gemini/smart_scraper_gemini.py
+-rw-r--r--   0        0        0     1617 2020-02-02 00:00:00.000000 scrapegraphai-1.2.2/examples/gemini/xml_scraper_openai.py
+-rw-r--r--   0        0        0     4429 2020-02-02 00:00:00.000000 scrapegraphai-1.2.2/examples/gemini/inputs/books.xml
+-rw-r--r--   0        0        0     6455 2020-02-02 00:00:00.000000 scrapegraphai-1.2.2/examples/gemini/inputs/example.json
+-rw-r--r--   0        0        0     7305 2020-02-02 00:00:00.000000 scrapegraphai-1.2.2/examples/gemini/inputs/plain_html_example.txt
+-rw-r--r--   0        0        0      176 2020-02-02 00:00:00.000000 scrapegraphai-1.2.2/examples/gemini/inputs/username.csv
+-rw-r--r--   0        0        0       64 2020-02-02 00:00:00.000000 scrapegraphai-1.2.2/examples/groq/.env.example
+-rw-r--r--   0        0        0     1054 2020-02-02 00:00:00.000000 scrapegraphai-1.2.2/examples/groq/search_graph_groq_openai.py
+-rw-r--r--   0        0        0     1414 2020-02-02 00:00:00.000000 scrapegraphai-1.2.2/examples/groq/smart_scraper_groq_ollama.py
+-rw-r--r--   0        0        0     1366 2020-02-02 00:00:00.000000 scrapegraphai-1.2.2/examples/groq/smart_scraper_groq_openai.py
+-rw-r--r--   0        0        0     2062 2020-02-02 00:00:00.000000 scrapegraphai-1.2.2/examples/huggingfacehub/smart_scraper_huggingfacehub.py
+-rw-r--r--   0        0        0     1838 2020-02-02 00:00:00.000000 scrapegraphai-1.2.2/examples/local_models/csv_scraper_ollama.py
+-rw-r--r--   0        0        0     1942 2020-02-02 00:00:00.000000 scrapegraphai-1.2.2/examples/local_models/json_scraper_ollama.py
+-rw-r--r--   0        0        0     1752 2020-02-02 00:00:00.000000 scrapegraphai-1.2.2/examples/local_models/scrape_plain_text_ollama.py
+-rw-r--r--   0        0        0     1832 2020-02-02 00:00:00.000000 scrapegraphai-1.2.2/examples/local_models/scrape_xml_ollama.py
+-rw-r--r--   0        0        0     1465 2020-02-02 00:00:00.000000 scrapegraphai-1.2.2/examples/local_models/script_generator_ollama.py
+-rw-r--r--   0        0        0     1401 2020-02-02 00:00:00.000000 scrapegraphai-1.2.2/examples/local_models/search_graph_ollama.py
+-rw-r--r--   0        0        0     1407 2020-02-02 00:00:00.000000 scrapegraphai-1.2.2/examples/local_models/smart_scraper_ollama.py
+-rw-r--r--   0        0        0     1929 2020-02-02 00:00:00.000000 scrapegraphai-1.2.2/examples/local_models/xml_scraper_ollama.py
+-rw-r--r--   0        0        0     4429 2020-02-02 00:00:00.000000 scrapegraphai-1.2.2/examples/local_models/inputs/books.xml
+-rw-r--r--   0        0        0     6455 2020-02-02 00:00:00.000000 scrapegraphai-1.2.2/examples/local_models/inputs/example.json
+-rw-r--r--   0        0        0     7305 2020-02-02 00:00:00.000000 scrapegraphai-1.2.2/examples/local_models/inputs/plain_html_example.txt
+-rw-r--r--   0        0        0      176 2020-02-02 00:00:00.000000 scrapegraphai-1.2.2/examples/local_models/inputs/username.csv
+-rw-r--r--   0        0        0      208 2020-02-02 00:00:00.000000 scrapegraphai-1.2.2/examples/mixed_models/.env.example
+-rw-r--r--   0        0        0      201 2020-02-02 00:00:00.000000 scrapegraphai-1.2.2/examples/mixed_models/readme.md
+-rw-r--r--   0        0        0     1357 2020-02-02 00:00:00.000000 scrapegraphai-1.2.2/examples/mixed_models/search_graph_groq_ollama.py
+-rw-r--r--   0        0        0     1448 2020-02-02 00:00:00.000000 scrapegraphai-1.2.2/examples/mixed_models/smart_scraper_mixed.py
+-rw-r--r--   0        0        0     4429 2020-02-02 00:00:00.000000 scrapegraphai-1.2.2/examples/mixed_models/inputs/books.xml
+-rw-r--r--   0        0        0     6455 2020-02-02 00:00:00.000000 scrapegraphai-1.2.2/examples/mixed_models/inputs/example.json
+-rw-r--r--   0        0        0     7305 2020-02-02 00:00:00.000000 scrapegraphai-1.2.2/examples/mixed_models/inputs/plain_html_example.txt
+-rw-r--r--   0        0        0       39 2020-02-02 00:00:00.000000 scrapegraphai-1.2.2/examples/openai/.env.example
+-rw-r--r--   0        0        0     1574 2020-02-02 00:00:00.000000 scrapegraphai-1.2.2/examples/openai/csv_scraper_openai.py
+-rw-r--r--   0        0        0     2688 2020-02-02 00:00:00.000000 scrapegraphai-1.2.2/examples/openai/custom_graph_openai.py
+-rw-r--r--   0        0        0     1321 2020-02-02 00:00:00.000000 scrapegraphai-1.2.2/examples/openai/deep_scraper_openai.py
+-rw-r--r--   0        0        0     1633 2020-02-02 00:00:00.000000 scrapegraphai-1.2.2/examples/openai/json_scraper_openai.py
+-rw-r--r--   0        0        0     1307 2020-02-02 00:00:00.000000 scrapegraphai-1.2.2/examples/openai/omni_scraper_openai.py
+-rw-r--r--   0        0        0     1142 2020-02-02 00:00:00.000000 scrapegraphai-1.2.2/examples/openai/omni_search_graph_openai.py
+-rw-r--r--   0        0        0      203 2020-02-02 00:00:00.000000 scrapegraphai-1.2.2/examples/openai/readme.md
+-rw-r--r--   0        0        0     1512 2020-02-02 00:00:00.000000 scrapegraphai-1.2.2/examples/openai/scrape_plain_text_openai.py
+-rw-r--r--   0        0        0     1239 2020-02-02 00:00:00.000000 scrapegraphai-1.2.2/examples/openai/script_generator_openai.py
+-rw-r--r--   0        0        0     1160 2020-02-02 00:00:00.000000 scrapegraphai-1.2.2/examples/openai/search_graph_openai.py
+-rw-r--r--   0        0        0     1233 2020-02-02 00:00:00.000000 scrapegraphai-1.2.2/examples/openai/smart_scraper_openai.py
+-rw-r--r--   0        0        0     1531 2020-02-02 00:00:00.000000 scrapegraphai-1.2.2/examples/openai/speech_graph_openai.py
+-rw-r--r--   0        0        0     1642 2020-02-02 00:00:00.000000 scrapegraphai-1.2.2/examples/openai/xml_scraper_openai.py
+-rw-r--r--   0        0        0     4429 2020-02-02 00:00:00.000000 scrapegraphai-1.2.2/examples/openai/inputs/books.xml
+-rw-r--r--   0        0        0     6455 2020-02-02 00:00:00.000000 scrapegraphai-1.2.2/examples/openai/inputs/example.json
+-rw-r--r--   0        0        0     7305 2020-02-02 00:00:00.000000 scrapegraphai-1.2.2/examples/openai/inputs/plain_html_example.txt
+-rw-r--r--   0        0        0      176 2020-02-02 00:00:00.000000 scrapegraphai-1.2.2/examples/openai/inputs/username.csv
+-rw-r--r--   0        0        0      567 2020-02-02 00:00:00.000000 scrapegraphai-1.2.2/examples/single_node/fetch_node.py
+-rw-r--r--   0        0        0     1199 2020-02-02 00:00:00.000000 scrapegraphai-1.2.2/examples/single_node/image2text_node.py
+-rw-r--r--   0        0        0      961 2020-02-02 00:00:00.000000 scrapegraphai-1.2.2/examples/single_node/robot_node.py
+-rwxr-xr-x   0        0        0      986 2020-02-02 00:00:00.000000 scrapegraphai-1.2.2/manual deployment/commit_and_push.sh
+-rwxr-xr-x   0        0        0      611 2020-02-02 00:00:00.000000 scrapegraphai-1.2.2/manual deployment/commit_and_push_with_tests.sh
+-rwxr-xr-x   0        0        0      154 2020-02-02 00:00:00.000000 scrapegraphai-1.2.2/manual deployment/deploy_on_pip.sh
+-rw-r--r--   0        0        0       54 2020-02-02 00:00:00.000000 scrapegraphai-1.2.2/scrapegraphai/__init__.py
+-rw-r--r--   0        0        0       90 2020-02-02 00:00:00.000000 scrapegraphai-1.2.2/scrapegraphai/builders/__init__.py
+-rw-r--r--   0        0        0     6653 2020-02-02 00:00:00.000000 scrapegraphai-1.2.2/scrapegraphai/builders/graph_builder.py
+-rw-r--r--   0        0        0       83 2020-02-02 00:00:00.000000 scrapegraphai-1.2.2/scrapegraphai/docloaders/__init__.py
+-rw-r--r--   0        0        0     4498 2020-02-02 00:00:00.000000 scrapegraphai-1.2.2/scrapegraphai/docloaders/chromium.py
+-rw-r--r--   0        0        0      636 2020-02-02 00:00:00.000000 scrapegraphai-1.2.2/scrapegraphai/graphs/__init__.py
+-rw-r--r--   0        0        0    13691 2020-02-02 00:00:00.000000 scrapegraphai-1.2.2/scrapegraphai/graphs/abstract_graph.py
+-rw-r--r--   0        0        0     5378 2020-02-02 00:00:00.000000 scrapegraphai-1.2.2/scrapegraphai/graphs/base_graph.py
+-rw-r--r--   0        0        0     2472 2020-02-02 00:00:00.000000 scrapegraphai-1.2.2/scrapegraphai/graphs/csv_scraper_graph.py
+-rw-r--r--   0        0        0     3777 2020-02-02 00:00:00.000000 scrapegraphai-1.2.2/scrapegraphai/graphs/deep_scraper_graph.py
+-rw-r--r--   0        0        0     3392 2020-02-02 00:00:00.000000 scrapegraphai-1.2.2/scrapegraphai/graphs/json_scraper_graph.py
+-rw-r--r--   0        0        0     4295 2020-02-02 00:00:00.000000 scrapegraphai-1.2.2/scrapegraphai/graphs/omni_scraper_graph.py
+-rw-r--r--   0        0        0     3722 2020-02-02 00:00:00.000000 scrapegraphai-1.2.2/scrapegraphai/graphs/omni_search_graph.py
+-rw-r--r--   0        0        0     3538 2020-02-02 00:00:00.000000 scrapegraphai-1.2.2/scrapegraphai/graphs/pdf_scraper_graph.py
+-rw-r--r--   0        0        0     3371 2020-02-02 00:00:00.000000 scrapegraphai-1.2.2/scrapegraphai/graphs/script_creator_graph.py
+-rw-r--r--   0        0        0     3646 2020-02-02 00:00:00.000000 scrapegraphai-1.2.2/scrapegraphai/graphs/search_graph.py
+-rw-r--r--   0        0        0     3650 2020-02-02 00:00:00.000000 scrapegraphai-1.2.2/scrapegraphai/graphs/smart_scraper_graph.py
+-rw-r--r--   0        0        0     4322 2020-02-02 00:00:00.000000 scrapegraphai-1.2.2/scrapegraphai/graphs/speech_graph.py
+-rw-r--r--   0        0        0     3534 2020-02-02 00:00:00.000000 scrapegraphai-1.2.2/scrapegraphai/graphs/xml_scraper_graph.py
+-rw-r--r--   0        0        0      202 2020-02-02 00:00:00.000000 scrapegraphai-1.2.2/scrapegraphai/helpers/__init__.py
+-rw-r--r--   0        0        0     4203 2020-02-02 00:00:00.000000 scrapegraphai-1.2.2/scrapegraphai/helpers/models_tokens.py
+-rw-r--r--   0        0        0     3807 2020-02-02 00:00:00.000000 scrapegraphai-1.2.2/scrapegraphai/helpers/nodes_metadata.py
+-rw-r--r--   0        0        0      310 2020-02-02 00:00:00.000000 scrapegraphai-1.2.2/scrapegraphai/helpers/robots.py
+-rw-r--r--   0        0        0     2363 2020-02-02 00:00:00.000000 scrapegraphai-1.2.2/scrapegraphai/helpers/schemas.py
+-rw-r--r--   0        0        0      406 2020-02-02 00:00:00.000000 scrapegraphai-1.2.2/scrapegraphai/models/__init__.py
+-rw-r--r--   0        0        0      429 2020-02-02 00:00:00.000000 scrapegraphai-1.2.2/scrapegraphai/models/anthropic.py
+-rw-r--r--   0        0        0      441 2020-02-02 00:00:00.000000 scrapegraphai-1.2.2/scrapegraphai/models/azure_openai.py
+-rw-r--r--   0        0        0      579 2020-02-02 00:00:00.000000 scrapegraphai-1.2.2/scrapegraphai/models/bedrock.py
+-rw-r--r--   0        0        0      455 2020-02-02 00:00:00.000000 scrapegraphai-1.2.2/scrapegraphai/models/deepseek.py
+-rw-r--r--   0        0        0      606 2020-02-02 00:00:00.000000 scrapegraphai-1.2.2/scrapegraphai/models/gemini.py
+-rw-r--r--   0        0        0      426 2020-02-02 00:00:00.000000 scrapegraphai-1.2.2/scrapegraphai/models/groq.py
+-rw-r--r--   0        0        0      459 2020-02-02 00:00:00.000000 scrapegraphai-1.2.2/scrapegraphai/models/hugging_face.py
+-rw-r--r--   0        0        0      427 2020-02-02 00:00:00.000000 scrapegraphai-1.2.2/scrapegraphai/models/ollama.py
+-rw-r--r--   0        0        0      412 2020-02-02 00:00:00.000000 scrapegraphai-1.2.2/scrapegraphai/models/openai.py
+-rw-r--r--   0        0        0     1367 2020-02-02 00:00:00.000000 scrapegraphai-1.2.2/scrapegraphai/models/openai_itt.py
+-rw-r--r--   0        0        0     1221 2020-02-02 00:00:00.000000 scrapegraphai-1.2.2/scrapegraphai/models/openai_tts.py
+-rw-r--r--   0        0        0      897 2020-02-02 00:00:00.000000 scrapegraphai-1.2.2/scrapegraphai/nodes/__init__.py
+-rw-r--r--   0        0        0     8591 2020-02-02 00:00:00.000000 scrapegraphai-1.2.2/scrapegraphai/nodes/base_node.py
+-rw-r--r--   0        0        0     2914 2020-02-02 00:00:00.000000 scrapegraphai-1.2.2/scrapegraphai/nodes/conditional_node.py
+-rw-r--r--   0        0        0     6449 2020-02-02 00:00:00.000000 scrapegraphai-1.2.2/scrapegraphai/nodes/fetch_node.py
+-rw-r--r--   0        0        0     7182 2020-02-02 00:00:00.000000 scrapegraphai-1.2.2/scrapegraphai/nodes/generate_answer_csv_node.py
+-rw-r--r--   0        0        0     6613 2020-02-02 00:00:00.000000 scrapegraphai-1.2.2/scrapegraphai/nodes/generate_answer_node.py
+-rw-r--r--   0        0        0     7064 2020-02-02 00:00:00.000000 scrapegraphai-1.2.2/scrapegraphai/nodes/generate_answer_omni_node.py
+-rw-r--r--   0        0        0     7158 2020-02-02 00:00:00.000000 scrapegraphai-1.2.2/scrapegraphai/nodes/generate_answer_pdf_node.py
+-rw-r--r--   0        0        0     4340 2020-02-02 00:00:00.000000 scrapegraphai-1.2.2/scrapegraphai/nodes/generate_scraper_node.py
+-rw-r--r--   0        0        0     3537 2020-02-02 00:00:00.000000 scrapegraphai-1.2.2/scrapegraphai/nodes/get_probable_tags_node.py
+-rw-r--r--   0        0        0     4395 2020-02-02 00:00:00.000000 scrapegraphai-1.2.2/scrapegraphai/nodes/graph_iterator_node.py
+-rw-r--r--   0        0        0     2671 2020-02-02 00:00:00.000000 scrapegraphai-1.2.2/scrapegraphai/nodes/image_to_text_node.py
+-rw-r--r--   0        0        0     3903 2020-02-02 00:00:00.000000 scrapegraphai-1.2.2/scrapegraphai/nodes/merge_answers_node.py
+-rw-r--r--   0        0        0     2930 2020-02-02 00:00:00.000000 scrapegraphai-1.2.2/scrapegraphai/nodes/parse_node.py
+-rw-r--r--   0        0        0     4496 2020-02-02 00:00:00.000000 scrapegraphai-1.2.2/scrapegraphai/nodes/rag_node.py
+-rw-r--r--   0        0        0     6117 2020-02-02 00:00:00.000000 scrapegraphai-1.2.2/scrapegraphai/nodes/robots_node.py
+-rw-r--r--   0        0        0     4185 2020-02-02 00:00:00.000000 scrapegraphai-1.2.2/scrapegraphai/nodes/search_internet_node.py
+-rw-r--r--   0        0        0     4181 2020-02-02 00:00:00.000000 scrapegraphai-1.2.2/scrapegraphai/nodes/search_link_node.py
+-rw-r--r--   0        0        0     2343 2020-02-02 00:00:00.000000 scrapegraphai-1.2.2/scrapegraphai/nodes/text_to_speech_node.py
+-rw-r--r--   0        0        0      424 2020-02-02 00:00:00.000000 scrapegraphai-1.2.2/scrapegraphai/utils/__init__.py
+-rw-r--r--   0        0        0     2330 2020-02-02 00:00:00.000000 scrapegraphai-1.2.2/scrapegraphai/utils/cleanup_html.py
+-rw-r--r--   0        0        0     2141 2020-02-02 00:00:00.000000 scrapegraphai-1.2.2/scrapegraphai/utils/convert_to_csv.py
+-rw-r--r--   0        0        0     1974 2020-02-02 00:00:00.000000 scrapegraphai-1.2.2/scrapegraphai/utils/convert_to_json.py
+-rw-r--r--   0        0        0     4638 2020-02-02 00:00:00.000000 scrapegraphai-1.2.2/scrapegraphai/utils/parse_state_keys.py
+-rw-r--r--   0        0        0      764 2020-02-02 00:00:00.000000 scrapegraphai-1.2.2/scrapegraphai/utils/prettify_exec_info.py
+-rw-r--r--   0        0        0     6404 2020-02-02 00:00:00.000000 scrapegraphai-1.2.2/scrapegraphai/utils/proxy_rotation.py
+-rw-r--r--   0        0        0     2140 2020-02-02 00:00:00.000000 scrapegraphai-1.2.2/scrapegraphai/utils/research_web.py
+-rw-r--r--   0        0        0      836 2020-02-02 00:00:00.000000 scrapegraphai-1.2.2/scrapegraphai/utils/save_audio_from_bytes.py
+-rw-r--r--   0        0        0     1702 2020-02-02 00:00:00.000000 scrapegraphai-1.2.2/scrapegraphai/utils/sys_dynamic_import.py
+-rw-r--r--   0        0        0     1320 2020-02-02 00:00:00.000000 scrapegraphai-1.2.2/scrapegraphai/utils/token_calculator.py
+-rw-r--r--   0        0        0      417 2020-02-02 00:00:00.000000 scrapegraphai-1.2.2/tests/Readme.md
+-rw-r--r--   0        0        0     1220 2020-02-02 00:00:00.000000 scrapegraphai-1.2.2/tests/graphs/scrape_json_ollama.py
+-rw-r--r--   0        0        0     1238 2020-02-02 00:00:00.000000 scrapegraphai-1.2.2/tests/graphs/scrape_plain_text_llama3_test.py
+-rw-r--r--   0        0        0     1239 2020-02-02 00:00:00.000000 scrapegraphai-1.2.2/tests/graphs/scrape_plain_text_mistral_test.py
+-rw-r--r--   0        0        0     1243 2020-02-02 00:00:00.000000 scrapegraphai-1.2.2/tests/graphs/scrape_xml_ollama_test.py
+-rw-r--r--   0        0        0     1223 2020-02-02 00:00:00.000000 scrapegraphai-1.2.2/tests/graphs/script_generator_test.py
+-rw-r--r--   0        0        0     1350 2020-02-02 00:00:00.000000 scrapegraphai-1.2.2/tests/graphs/smart_scraper_ollama_test.py
+-rw-r--r--   0        0        0     4429 2020-02-02 00:00:00.000000 scrapegraphai-1.2.2/tests/graphs/inputs/books.xml
+-rw-r--r--   0        0        0     6455 2020-02-02 00:00:00.000000 scrapegraphai-1.2.2/tests/graphs/inputs/example.json
+-rw-r--r--   0        0        0     7305 2020-02-02 00:00:00.000000 scrapegraphai-1.2.2/tests/graphs/inputs/plain_html_example.txt
+-rw-r--r--   0        0        0      176 2020-02-02 00:00:00.000000 scrapegraphai-1.2.2/tests/graphs/inputs/username.csv
+-rw-r--r--   0        0        0      771 2020-02-02 00:00:00.000000 scrapegraphai-1.2.2/tests/nodes/fetch_node_test.py
+-rw-r--r--   0        0        0     1207 2020-02-02 00:00:00.000000 scrapegraphai-1.2.2/tests/nodes/robot_node_test.py
+-rw-r--r--   0        0        0     2961 2020-02-02 00:00:00.000000 scrapegraphai-1.2.2/tests/utils/test_proxy_rotation.py
+-rw-r--r--   0        0        0     2203 2020-02-02 00:00:00.000000 scrapegraphai-1.2.2/tests/utils/test_sys_dynamic_import.py
+-rw-r--r--   0        0        0      448 2020-02-02 00:00:00.000000 scrapegraphai-1.2.2/.gitignore
+-rw-r--r--   0        0        0     1065 2020-02-02 00:00:00.000000 scrapegraphai-1.2.2/LICENSE
+-rw-r--r--   0        0        0     8967 2020-02-02 00:00:00.000000 scrapegraphai-1.2.2/README.md
+-rw-r--r--   0        0        0     2027 2020-02-02 00:00:00.000000 scrapegraphai-1.2.2/pyproject.toml
+-rw-r--r--   0        0        0    10480 2020-02-02 00:00:00.000000 scrapegraphai-1.2.2/PKG-INFO
```

### Comparing `scrapegraphai-1.2.1/.releaserc.yml` & `scrapegraphai-1.2.2/.releaserc.yml`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.2.1/CHANGELOG.md` & `scrapegraphai-1.2.2/CHANGELOG.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,7 +1,14 @@
+## [1.2.2](https://github.com/VinciGit00/Scrapegraph-ai/compare/v1.2.1...v1.2.2) (2024-05-15)
+
+
+### Bug Fixes
+
+* come back to the old version ([cc5adef](https://github.com/VinciGit00/Scrapegraph-ai/commit/cc5adefd29eb2d0d7127515c4a4a72eabbc7eaa8))
+
 ## [1.2.1](https://github.com/VinciGit00/Scrapegraph-ai/compare/v1.2.0...v1.2.1) (2024-05-15)
 
 
 ### Bug Fixes
 
 * removed unused ([5587a64](https://github.com/VinciGit00/Scrapegraph-ai/commit/5587a64d23451a6a216000fe83b2ce1cc8f7141b))
```

### Comparing `scrapegraphai-1.2.1/CODE_OF_CONDUCT.md` & `scrapegraphai-1.2.2/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.2.1/CONTRIBUTING.md` & `scrapegraphai-1.2.2/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.2.1/readthedocs.yml` & `scrapegraphai-1.2.2/readthedocs.yml`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.2.1/.github/ISSUE_TEMPLATE/bug_report.md` & `scrapegraphai-1.2.2/.github/ISSUE_TEMPLATE/bug_report.md`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.2.1/.github/ISSUE_TEMPLATE/feature_request.md` & `scrapegraphai-1.2.2/.github/ISSUE_TEMPLATE/feature_request.md`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.2.1/.github/workflows/codeql.yml` & `scrapegraphai-1.2.2/.github/workflows/codeql.yml`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.2.1/.github/workflows/dependency-review.yml` & `scrapegraphai-1.2.2/.github/workflows/dependency-review.yml`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.2.1/.github/workflows/pylint.yml` & `scrapegraphai-1.2.2/.github/workflows/pylint.yml`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.2.1/.github/workflows/python-publish.yml` & `scrapegraphai-1.2.2/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.2.1/.github/workflows/release.yml` & `scrapegraphai-1.2.2/.github/workflows/release.yml`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.2.1/docs/Makefile` & `scrapegraphai-1.2.2/docs/Makefile`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.2.1/docs/README.md` & `scrapegraphai-1.2.2/docs/README.md`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.2.1/docs/make.bat` & `scrapegraphai-1.2.2/docs/make.bat`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.2.1/docs/assets/apikey_1.png` & `scrapegraphai-1.2.2/docs/assets/apikey_1.png`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.2.1/docs/assets/apikey_2.png` & `scrapegraphai-1.2.2/docs/assets/apikey_2.png`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.2.1/docs/assets/apikey_3.png` & `scrapegraphai-1.2.2/docs/assets/apikey_3.png`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.2.1/docs/assets/apikey_4.png` & `scrapegraphai-1.2.2/docs/assets/apikey_4.png`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.2.1/docs/assets/codespaces-badge.png` & `scrapegraphai-1.2.2/docs/assets/codespaces-badge.png`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.2.1/docs/assets/logo_authors.png` & `scrapegraphai-1.2.2/docs/assets/logo_authors.png`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.2.1/docs/assets/omniscrapergraph.png` & `scrapegraphai-1.2.2/docs/assets/omniscrapergraph.png`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.2.1/docs/assets/omnisearchgraph.png` & `scrapegraphai-1.2.2/docs/assets/omnisearchgraph.png`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.2.1/docs/assets/project_overview_diagram.fig` & `scrapegraphai-1.2.2/docs/assets/project_overview_diagram.fig`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.2.1/docs/assets/project_overview_diagram.png` & `scrapegraphai-1.2.2/docs/assets/project_overview_diagram.png`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.2.1/docs/assets/scrapegraphai_logo.png` & `scrapegraphai-1.2.2/docs/assets/scrapegraphai_logo.png`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.2.1/docs/assets/searchgraph.png` & `scrapegraphai-1.2.2/docs/assets/searchgraph.png`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.2.1/docs/assets/serp_api_logo.png` & `scrapegraphai-1.2.2/docs/assets/serp_api_logo.png`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.2.1/docs/assets/smartscrapergraph.png` & `scrapegraphai-1.2.2/docs/assets/smartscrapergraph.png`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.2.1/docs/assets/speechgraph.png` & `scrapegraphai-1.2.2/docs/assets/speechgraph.png`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.2.1/docs/source/conf.py` & `scrapegraphai-1.2.2/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.2.1/docs/source/index.rst` & `scrapegraphai-1.2.2/docs/source/index.rst`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.2.1/docs/source/getting_started/examples.rst` & `scrapegraphai-1.2.2/docs/source/getting_started/examples.rst`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.2.1/docs/source/getting_started/installation.rst` & `scrapegraphai-1.2.2/docs/source/getting_started/installation.rst`

 * *Files 20% similar despite different names*

```diff
@@ -21,21 +21,19 @@
 
    pip install scrapegraphai
 
 .. important::
    
    It is higly recommended to install the library in a virtual environment (conda, venv, etc.)
 
-If you clone the repository, you can install the library using `rye <https://rye-up.com/>`_. Follow the installation instruction from the website and then run:
+If your clone the repository, you can install the library using `poetry <https://python-poetry.org/docs/>`_:
 
 .. code-block:: bash
 
-   rye pin 3.10
-   rye sync
-   rye build
+   poetry install
 
 Additionally on Windows when using WSL
 ^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
 
 If you are using Windows Subsystem for Linux (WSL) and you are facing issues with the installation of the library, you might need to install the following packages:
 
 .. code-block:: bash
```

### Comparing `scrapegraphai-1.2.1/docs/source/introduction/contributing.rst` & `scrapegraphai-1.2.2/docs/source/introduction/contributing.rst`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.2.1/docs/source/introduction/overview.rst` & `scrapegraphai-1.2.2/docs/source/introduction/overview.rst`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.2.1/docs/source/modules/scrapegraphai.graphs.rst` & `scrapegraphai-1.2.2/docs/source/modules/scrapegraphai.graphs.rst`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.2.1/docs/source/modules/scrapegraphai.nodes.rst` & `scrapegraphai-1.2.2/docs/source/modules/scrapegraphai.nodes.rst`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.2.1/docs/source/modules/scrapegraphai.rst` & `scrapegraphai-1.2.2/docs/source/modules/scrapegraphai.rst`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.2.1/docs/source/scrapers/benchmarks.rst` & `scrapegraphai-1.2.2/docs/source/scrapers/benchmarks.rst`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.2.1/docs/source/scrapers/graph_config.rst` & `scrapegraphai-1.2.2/docs/source/scrapers/graph_config.rst`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.2.1/docs/source/scrapers/graphs.rst` & `scrapegraphai-1.2.2/docs/source/scrapers/graphs.rst`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.2.1/docs/source/scrapers/llm.rst` & `scrapegraphai-1.2.2/docs/source/scrapers/llm.rst`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.2.1/examples/readme.md` & `scrapegraphai-1.2.2/examples/readme.md`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.2.1/examples/anthropic/smart_scraper_haiku.py` & `scrapegraphai-1.2.2/examples/anthropic/smart_scraper_haiku.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.2.1/examples/azure/json_scraper_azure.py` & `scrapegraphai-1.2.2/examples/azure/json_scraper_azure.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.2.1/examples/azure/search_graph_azure.py` & `scrapegraphai-1.2.2/examples/azure/search_graph_azure.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.2.1/examples/azure/smart_scraper_azure_openai.py` & `scrapegraphai-1.2.2/examples/azure/smart_scraper_azure_openai.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.2.1/examples/azure/xml_scraper_azure.py` & `scrapegraphai-1.2.2/examples/azure/xml_scraper_azure.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.2.1/examples/azure/inputs/books.xml` & `scrapegraphai-1.2.2/examples/azure/inputs/books.xml`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.2.1/examples/azure/inputs/example.json` & `scrapegraphai-1.2.2/examples/azure/inputs/example.json`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.2.1/examples/bedrock/smart_scraper_bedrock.py` & `scrapegraphai-1.2.2/examples/bedrock/smart_scraper_bedrock.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.2.1/examples/benchmarks/GenerateScraper/Readme.md` & `scrapegraphai-1.2.2/examples/benchmarks/GenerateScraper/Readme.md`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.2.1/examples/benchmarks/GenerateScraper/benchmark_groq.py` & `scrapegraphai-1.2.2/examples/benchmarks/GenerateScraper/benchmark_groq.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.2.1/examples/benchmarks/GenerateScraper/benchmark_llama3.py` & `scrapegraphai-1.2.2/examples/benchmarks/GenerateScraper/benchmark_llama3.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.2.1/examples/benchmarks/GenerateScraper/benchmark_mistral.py` & `scrapegraphai-1.2.2/examples/benchmarks/GenerateScraper/benchmark_mistral.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.2.1/examples/benchmarks/GenerateScraper/benchmark_openai_gpt35.py` & `scrapegraphai-1.2.2/examples/benchmarks/GenerateScraper/benchmark_openai_gpt35.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.2.1/examples/benchmarks/GenerateScraper/benchmark_openai_gpt4.py` & `scrapegraphai-1.2.2/examples/benchmarks/GenerateScraper/benchmark_openai_gpt4.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.2.1/examples/benchmarks/GenerateScraper/inputs/example_1.txt` & `scrapegraphai-1.2.2/examples/benchmarks/GenerateScraper/inputs/example_1.txt`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.2.1/examples/benchmarks/GenerateScraper/inputs/example_2.txt` & `scrapegraphai-1.2.2/examples/benchmarks/GenerateScraper/inputs/example_2.txt`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.2.1/examples/benchmarks/SmartScraper/Readme.md` & `scrapegraphai-1.2.2/examples/benchmarks/SmartScraper/Readme.md`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.2.1/examples/benchmarks/SmartScraper/benchmark_docker.py` & `scrapegraphai-1.2.2/examples/benchmarks/SmartScraper/benchmark_docker.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.2.1/examples/benchmarks/SmartScraper/benchmark_groq.py` & `scrapegraphai-1.2.2/examples/benchmarks/SmartScraper/benchmark_groq.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.2.1/examples/benchmarks/SmartScraper/benchmark_llama3.py` & `scrapegraphai-1.2.2/examples/benchmarks/SmartScraper/benchmark_llama3.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.2.1/examples/benchmarks/SmartScraper/benchmark_mistral.py` & `scrapegraphai-1.2.2/examples/benchmarks/SmartScraper/benchmark_mistral.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.2.1/examples/benchmarks/SmartScraper/benchmark_openai_gpt35.py` & `scrapegraphai-1.2.2/examples/benchmarks/SmartScraper/benchmark_openai_gpt35.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.2.1/examples/benchmarks/SmartScraper/benchmark_openai_gpt4.py` & `scrapegraphai-1.2.2/examples/benchmarks/SmartScraper/benchmark_openai_gpt4.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.2.1/examples/benchmarks/SmartScraper/inputs/example_1.txt` & `scrapegraphai-1.2.2/examples/benchmarks/SmartScraper/inputs/example_1.txt`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.2.1/examples/benchmarks/SmartScraper/inputs/example_2.txt` & `scrapegraphai-1.2.2/examples/benchmarks/SmartScraper/inputs/example_2.txt`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.2.1/examples/deepseek/csv_scraper_deepseek.py` & `scrapegraphai-1.2.2/examples/deepseek/csv_scraper_deepseek.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.2.1/examples/deepseek/json_scraper_deepseek.py` & `scrapegraphai-1.2.2/examples/deepseek/json_scraper_deepseek.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.2.1/examples/deepseek/script_generator_deepseek.py` & `scrapegraphai-1.2.2/examples/deepseek/script_generator_deepseek.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.2.1/examples/deepseek/search_graph_deepseek.py` & `scrapegraphai-1.2.2/examples/deepseek/search_graph_deepseek.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.2.1/examples/deepseek/smart_scarper_deepseek.py` & `scrapegraphai-1.2.2/examples/deepseek/smart_scarper_deepseek.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.2.1/examples/deepseek/xml_scraper_deepseek.py` & `scrapegraphai-1.2.2/examples/deepseek/xml_scraper_deepseek.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.2.1/examples/deepseek/inputs/books.xml` & `scrapegraphai-1.2.2/examples/deepseek/inputs/books.xml`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.2.1/examples/deepseek/inputs/example.json` & `scrapegraphai-1.2.2/examples/deepseek/inputs/example.json`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.2.1/examples/gemini/csv_scraper_gemini.py` & `scrapegraphai-1.2.2/examples/gemini/csv_scraper_gemini.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.2.1/examples/gemini/custom_graph_gemini.py` & `scrapegraphai-1.2.2/examples/gemini/custom_graph_gemini.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.2.1/examples/gemini/json_scraper_gemini.py` & `scrapegraphai-1.2.2/examples/gemini/json_scraper_gemini.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.2.1/examples/gemini/scrape_plain_text_gemini.py` & `scrapegraphai-1.2.2/examples/gemini/scrape_plain_text_gemini.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.2.1/examples/gemini/scrape_xml_gemini.py` & `scrapegraphai-1.2.2/examples/gemini/scrape_xml_gemini.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.2.1/examples/gemini/script_generator_gemini.py` & `scrapegraphai-1.2.2/examples/gemini/script_generator_gemini.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.2.1/examples/gemini/search_graph_gemini.py` & `scrapegraphai-1.2.2/examples/gemini/search_graph_gemini.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.2.1/examples/gemini/smart_scraper_gemini.py` & `scrapegraphai-1.2.2/examples/gemini/smart_scraper_gemini.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.2.1/examples/gemini/xml_scraper_openai.py` & `scrapegraphai-1.2.2/examples/gemini/xml_scraper_openai.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.2.1/examples/gemini/inputs/books.xml` & `scrapegraphai-1.2.2/examples/gemini/inputs/books.xml`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.2.1/examples/gemini/inputs/example.json` & `scrapegraphai-1.2.2/examples/gemini/inputs/example.json`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.2.1/examples/gemini/inputs/plain_html_example.txt` & `scrapegraphai-1.2.2/examples/gemini/inputs/plain_html_example.txt`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.2.1/examples/groq/search_graph_groq_openai.py` & `scrapegraphai-1.2.2/examples/groq/search_graph_groq_openai.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.2.1/examples/groq/smart_scraper_groq_ollama.py` & `scrapegraphai-1.2.2/examples/groq/smart_scraper_groq_ollama.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.2.1/examples/groq/smart_scraper_groq_openai.py` & `scrapegraphai-1.2.2/examples/groq/smart_scraper_groq_openai.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.2.1/examples/huggingfacehub/smart_scraper_huggingfacehub.py` & `scrapegraphai-1.2.2/examples/huggingfacehub/smart_scraper_huggingfacehub.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.2.1/examples/local_models/csv_scraper_ollama.py` & `scrapegraphai-1.2.2/examples/local_models/csv_scraper_ollama.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.2.1/examples/local_models/json_scraper_ollama.py` & `scrapegraphai-1.2.2/examples/local_models/json_scraper_ollama.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.2.1/examples/local_models/scrape_plain_text_ollama.py` & `scrapegraphai-1.2.2/examples/local_models/scrape_plain_text_ollama.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.2.1/examples/local_models/scrape_xml_ollama.py` & `scrapegraphai-1.2.2/examples/local_models/scrape_xml_ollama.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.2.1/examples/local_models/script_generator_ollama.py` & `scrapegraphai-1.2.2/examples/local_models/script_generator_ollama.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.2.1/examples/local_models/search_graph_ollama.py` & `scrapegraphai-1.2.2/examples/local_models/search_graph_ollama.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.2.1/examples/local_models/smart_scraper_ollama.py` & `scrapegraphai-1.2.2/examples/local_models/smart_scraper_ollama.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.2.1/examples/local_models/xml_scraper_ollama.py` & `scrapegraphai-1.2.2/examples/local_models/xml_scraper_ollama.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.2.1/examples/local_models/inputs/books.xml` & `scrapegraphai-1.2.2/examples/local_models/inputs/books.xml`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.2.1/examples/local_models/inputs/example.json` & `scrapegraphai-1.2.2/examples/local_models/inputs/example.json`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.2.1/examples/local_models/inputs/plain_html_example.txt` & `scrapegraphai-1.2.2/examples/local_models/inputs/plain_html_example.txt`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.2.1/examples/mixed_models/search_graph_groq_ollama.py` & `scrapegraphai-1.2.2/examples/mixed_models/search_graph_groq_ollama.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.2.1/examples/mixed_models/smart_scraper_mixed.py` & `scrapegraphai-1.2.2/examples/mixed_models/smart_scraper_mixed.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.2.1/examples/mixed_models/inputs/books.xml` & `scrapegraphai-1.2.2/examples/mixed_models/inputs/books.xml`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.2.1/examples/mixed_models/inputs/example.json` & `scrapegraphai-1.2.2/examples/mixed_models/inputs/example.json`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.2.1/examples/mixed_models/inputs/plain_html_example.txt` & `scrapegraphai-1.2.2/examples/mixed_models/inputs/plain_html_example.txt`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.2.1/examples/openai/csv_scraper_openai.py` & `scrapegraphai-1.2.2/examples/openai/csv_scraper_openai.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.2.1/examples/openai/custom_graph_openai.py` & `scrapegraphai-1.2.2/examples/openai/custom_graph_openai.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.2.1/examples/openai/deep_scraper_openai.py` & `scrapegraphai-1.2.2/examples/openai/deep_scraper_openai.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.2.1/examples/openai/json_scraper_openai.py` & `scrapegraphai-1.2.2/examples/openai/json_scraper_openai.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.2.1/examples/openai/omni_scraper_openai.py` & `scrapegraphai-1.2.2/examples/openai/omni_scraper_openai.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.2.1/examples/openai/omni_search_graph_openai.py` & `scrapegraphai-1.2.2/examples/openai/omni_search_graph_openai.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.2.1/examples/openai/scrape_plain_text_openai.py` & `scrapegraphai-1.2.2/examples/openai/scrape_plain_text_openai.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.2.1/examples/openai/script_generator_openai.py` & `scrapegraphai-1.2.2/examples/openai/script_generator_openai.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.2.1/examples/openai/search_graph_openai.py` & `scrapegraphai-1.2.2/examples/openai/search_graph_openai.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.2.1/examples/openai/smart_scraper_openai.py` & `scrapegraphai-1.2.2/examples/openai/smart_scraper_openai.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.2.1/examples/openai/speech_graph_openai.py` & `scrapegraphai-1.2.2/examples/openai/speech_graph_openai.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.2.1/examples/openai/xml_scraper_openai.py` & `scrapegraphai-1.2.2/examples/openai/xml_scraper_openai.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.2.1/examples/openai/inputs/books.xml` & `scrapegraphai-1.2.2/examples/openai/inputs/books.xml`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.2.1/examples/openai/inputs/example.json` & `scrapegraphai-1.2.2/examples/openai/inputs/example.json`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.2.1/examples/openai/inputs/plain_html_example.txt` & `scrapegraphai-1.2.2/examples/openai/inputs/plain_html_example.txt`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.2.1/examples/single_node/fetch_node.py` & `scrapegraphai-1.2.2/examples/single_node/fetch_node.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.2.1/examples/single_node/image2text_node.py` & `scrapegraphai-1.2.2/examples/single_node/image2text_node.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.2.1/examples/single_node/robot_node.py` & `scrapegraphai-1.2.2/examples/single_node/robot_node.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.2.1/manual deployment/commit_and_push.sh` & `scrapegraphai-1.2.2/manual deployment/commit_and_push.sh`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.2.1/manual deployment/commit_and_push_with_tests.sh` & `scrapegraphai-1.2.2/manual deployment/commit_and_push_with_tests.sh`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.2.1/scrapegraphai/graphs/__init__.py` & `scrapegraphai-1.2.2/scrapegraphai/graphs/__init__.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 """ 
 __init__.py file for graphs folder
 """
 
 from .abstract_graph import AbstractGraph
 from .base_graph import BaseGraph
 from .smart_scraper_graph import SmartScraperGraph
+from .deep_scraper_graph import DeepScraperGraph
 from .speech_graph import SpeechGraph
 from .search_graph import SearchGraph
 from .script_creator_graph import ScriptCreatorGraph
 from .xml_scraper_graph import XMLScraperGraph
 from .json_scraper_graph import JSONScraperGraph
 from .csv_scraper_graph import CSVScraperGraph
 from .pdf_scraper_graph import PDFScraperGraph
```

### Comparing `scrapegraphai-1.2.1/scrapegraphai/graphs/abstract_graph.py` & `scrapegraphai-1.2.2/scrapegraphai/graphs/abstract_graph.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.2.1/scrapegraphai/graphs/base_graph.py` & `scrapegraphai-1.2.2/scrapegraphai/graphs/base_graph.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.2.1/scrapegraphai/graphs/csv_scraper_graph.py` & `scrapegraphai-1.2.2/scrapegraphai/graphs/csv_scraper_graph.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.2.1/scrapegraphai/graphs/json_scraper_graph.py` & `scrapegraphai-1.2.2/scrapegraphai/graphs/json_scraper_graph.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.2.1/scrapegraphai/graphs/omni_scraper_graph.py` & `scrapegraphai-1.2.2/scrapegraphai/graphs/omni_scraper_graph.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.2.1/scrapegraphai/graphs/omni_search_graph.py` & `scrapegraphai-1.2.2/scrapegraphai/graphs/omni_search_graph.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 """ 
 OmniSearchGraph Module
 """
 
-from copy import copy
+from copy import deepcopy
 
 from .base_graph import BaseGraph
 from ..nodes import (
     SearchInternetNode,
     GraphIteratorNode,
     MergeAnswersNode
 )
@@ -39,15 +39,15 @@
         ... )
         >>> result = search_graph.run()
     """
 
     def __init__(self, prompt: str, config: dict):
 
         self.max_results = config.get("max_results", 3)
-        self.copy_config = copy(config)
+        self.copy_config = deepcopy(config)
 
         super().__init__(prompt, config)
 
     def _create_graph(self) -> BaseGraph:
         """
         Creates the graph of nodes representing the workflow for web scraping and searching.
```

### Comparing `scrapegraphai-1.2.1/scrapegraphai/graphs/pdf_scraper_graph.py` & `scrapegraphai-1.2.2/scrapegraphai/graphs/pdf_scraper_graph.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.2.1/scrapegraphai/graphs/script_creator_graph.py` & `scrapegraphai-1.2.2/scrapegraphai/graphs/script_creator_graph.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.2.1/scrapegraphai/graphs/search_graph.py` & `scrapegraphai-1.2.2/scrapegraphai/graphs/search_graph.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 """ 
 SearchGraph Module
 """
 
-from copy import copy
+from copy import deepcopy
 
 from .base_graph import BaseGraph
 from ..nodes import (
     SearchInternetNode,
     GraphIteratorNode,
     MergeAnswersNode
 )
@@ -38,15 +38,15 @@
         ... )
         >>> result = search_graph.run()
     """
 
     def __init__(self, prompt: str, config: dict):
 
         self.max_results = config.get("max_results", 3)
-        self.copy_config = copy(config)
+        self.copy_config = deepcopy(config)
 
         super().__init__(prompt, config)
 
     def _create_graph(self) -> BaseGraph:
         """
         Creates the graph of nodes representing the workflow for web scraping and searching.
```

### Comparing `scrapegraphai-1.2.1/scrapegraphai/graphs/smart_scraper_graph.py` & `scrapegraphai-1.2.2/scrapegraphai/graphs/smart_scraper_graph.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -107,8 +107,8 @@
         Returns:
             str: The answer to the prompt.
         """
 
         inputs = {"user_prompt": self.prompt, self.input_key: self.source}
         self.final_state, self.execution_info = self.graph.execute(inputs)
 
-        return self.final_state.get("answer", "No answer found.")
+        return self.final_state.get("answer", "No answer found.")
```

### Comparing `scrapegraphai-1.2.1/scrapegraphai/graphs/speech_graph.py` & `scrapegraphai-1.2.2/scrapegraphai/graphs/speech_graph.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.2.1/scrapegraphai/graphs/xml_scraper_graph.py` & `scrapegraphai-1.2.2/scrapegraphai/graphs/xml_scraper_graph.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.2.1/scrapegraphai/helpers/models_tokens.py` & `scrapegraphai-1.2.2/scrapegraphai/helpers/models_tokens.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.2.1/scrapegraphai/helpers/nodes_metadata.py` & `scrapegraphai-1.2.2/scrapegraphai/helpers/nodes_metadata.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.2.1/scrapegraphai/helpers/schemas.py` & `scrapegraphai-1.2.2/scrapegraphai/helpers/schemas.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.2.1/scrapegraphai/models/bedrock.py` & `scrapegraphai-1.2.2/scrapegraphai/models/bedrock.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.2.1/scrapegraphai/models/gemini.py` & `scrapegraphai-1.2.2/scrapegraphai/models/gemini.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.2.1/scrapegraphai/models/openai_itt.py` & `scrapegraphai-1.2.2/scrapegraphai/models/openai_itt.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.2.1/scrapegraphai/models/openai_tts.py` & `scrapegraphai-1.2.2/scrapegraphai/models/openai_tts.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.2.1/scrapegraphai/nodes/__init__.py` & `scrapegraphai-1.2.2/scrapegraphai/nodes/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -15,9 +15,8 @@
 from .generate_scraper_node import GenerateScraperNode
 from .search_link_node import SearchLinkNode
 from .robots_node import RobotsNode
 from .generate_answer_csv_node import GenerateAnswerCSVNode
 from .generate_answer_pdf_node import GenerateAnswerPDFNode
 from .graph_iterator_node import GraphIteratorNode
 from .merge_answers_node import MergeAnswersNode
-from .generate_answer_omni_node import GenerateAnswerOmniNode
-from .search_node_with_context import SearchLinksWithContext
+from .generate_answer_omni_node import GenerateAnswerOmniNode
```

### Comparing `scrapegraphai-1.2.1/scrapegraphai/nodes/base_node.py` & `scrapegraphai-1.2.2/scrapegraphai/nodes/base_node.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.2.1/scrapegraphai/nodes/conditional_node.py` & `scrapegraphai-1.2.2/scrapegraphai/nodes/conditional_node.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.2.1/scrapegraphai/nodes/fetch_node.py` & `scrapegraphai-1.2.2/scrapegraphai/nodes/fetch_node.py`

 * *Files 0% similar despite different names*

```diff
@@ -158,9 +158,8 @@
             parsed_content = f"Title: {title}, Body: {minimized_body}, Links: {link_urls}, Images: {image_urls}"
             
             compressed_document = [
                 Document(page_content=parsed_content, metadata={"source": source})
             ]
 
         state.update({self.output[0]: compressed_document, self.output[1]: link_urls, self.output[2]: image_urls})
-
         return state
```

### Comparing `scrapegraphai-1.2.1/scrapegraphai/nodes/generate_answer_csv_node.py` & `scrapegraphai-1.2.2/scrapegraphai/nodes/generate_answer_csv_node.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.2.1/scrapegraphai/nodes/generate_answer_node.py` & `scrapegraphai-1.2.2/scrapegraphai/nodes/generate_answer_node.py`

 * *Files 1% similar despite different names*

```diff
@@ -34,15 +34,15 @@
     """
 
     def __init__(self, input: str, output: List[str], node_config: Optional[dict] = None,
                  node_name: str = "GenerateAnswer"):
         super().__init__(node_name, "node", input, output, 2, node_config)
 
         self.llm_model = node_config["llm_model"]
-        self.verbose = True if node_config is None else node_config.get(
+        self.verbose = False if node_config is None else node_config.get(
             "verbose", False)
 
     def execute(self, state: dict) -> dict:
         """
         Generates an answer by constructing a prompt from the user's input and the scraped
         content, querying the language model, and parsing its response.
```

### Comparing `scrapegraphai-1.2.1/scrapegraphai/nodes/generate_answer_omni_node.py` & `scrapegraphai-1.2.2/scrapegraphai/nodes/generate_answer_omni_node.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.2.1/scrapegraphai/nodes/generate_answer_pdf_node.py` & `scrapegraphai-1.2.2/scrapegraphai/nodes/generate_answer_pdf_node.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.2.1/scrapegraphai/nodes/generate_scraper_node.py` & `scrapegraphai-1.2.2/scrapegraphai/nodes/generate_scraper_node.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.2.1/scrapegraphai/nodes/get_probable_tags_node.py` & `scrapegraphai-1.2.2/scrapegraphai/nodes/get_probable_tags_node.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.2.1/scrapegraphai/nodes/graph_iterator_node.py` & `scrapegraphai-1.2.2/scrapegraphai/nodes/graph_iterator_node.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.2.1/scrapegraphai/nodes/image_to_text_node.py` & `scrapegraphai-1.2.2/scrapegraphai/nodes/image_to_text_node.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.2.1/scrapegraphai/nodes/merge_answers_node.py` & `scrapegraphai-1.2.2/scrapegraphai/nodes/merge_answers_node.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 """
 MergeAnswersNode Module
 """
 
 # Imports from standard library
 from typing import List, Optional
+from tqdm import tqdm
 
 # Imports from Langchain
 from langchain.prompts import PromptTemplate
 from langchain_core.output_parsers import JsonOutputParser
 
 # Imports from the library
 from .base_node import BaseNode
@@ -34,16 +35,15 @@
 
         self.llm_model = node_config["llm_model"]
         self.verbose = False if node_config is None else node_config.get(
             "verbose", False)
 
     def execute(self, state: dict) -> dict:
         """
-        Executes the node's logic to merge the answers from multiple graph instances into a 
-        single answer.
+        Executes the node's logic to merge the answers from multiple graph instances into a single answer.
 
         Args:
             state (dict): The current state of the graph. The input keys will be used
                             to fetch the correct data from the state.
 
         Returns:
             dict: The updated state with the output key containing the generated answer.
```

### Comparing `scrapegraphai-1.2.1/scrapegraphai/nodes/parse_node.py` & `scrapegraphai-1.2.2/scrapegraphai/nodes/parse_node.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.2.1/scrapegraphai/nodes/rag_node.py` & `scrapegraphai-1.2.2/scrapegraphai/nodes/rag_node.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.2.1/scrapegraphai/nodes/robots_node.py` & `scrapegraphai-1.2.2/scrapegraphai/nodes/robots_node.py`

 * *Files 5% similar despite different names*

```diff
@@ -31,23 +31,20 @@
         node_config (dict): Additional configuration for the node.
         force_scraping (bool): A flag indicating whether scraping should be enforced even
                                  if disallowed by robots.txt. Defaults to True.
         node_name (str): The unique identifier name for the node, defaulting to "Robots".
     """
 
     def __init__(self, input: str, output: List[str],  node_config: Optional[dict]=None,
-
                  node_name: str = "Robots"):
         super().__init__(node_name, "node", input, output, 1)
 
         self.llm_model = node_config["llm_model"]
-
-        self.force_scraping = force_scraping
-        self.verbose = True if node_config is None else node_config.get(
-            "verbose", False)
+        self.force_scraping = False if node_config is None else node_config.get("force_scraping", False)
+        self.verbose = False if node_config is None else node_config.get("verbose", False)
 
     def execute(self, state: dict) -> dict:
         """
         Checks if a website is scrapeable based on the robots.txt file and updates the state
         with the scrapeability status. The method constructs a prompt for the language model,
         submits it, and parses the output to determine if scraping is allowed.
 
@@ -96,16 +93,15 @@
 
         else:
             parsed_url = urlparse(source)
             base_url = f"{parsed_url.scheme}://{parsed_url.netloc}"
             loader = AsyncChromiumLoader(f"{base_url}/robots.txt")
             document = loader.load()
             if "ollama" in self.llm_model.model_name:
-                self.llm_model.model_name = self.llm_model.model_name.split(
-                    "/")[-1]
+                self.llm_model.model_name = self.llm_model.model_name.split("/")[-1]
                 model = self.llm_model.model_name.split("/")[-1]
 
             else:
                 model = self.llm_model.model_name
             try:
                 agent = robots_dictionary[model]
 
@@ -122,15 +118,15 @@
 
             chain = prompt | self.llm_model | output_parser
             is_scrapable = chain.invoke({"path": source})[0]
 
             if "no" in is_scrapable:
                 if self.verbose:
                     print("\033[31m(Scraping this website is not allowed)\033[0m")
-
+                    
                 if not self.force_scraping:
                     raise ValueError(
                         'The website you selected is not scrapable')
                 else:
                     if self.verbose:
                         print("\033[33m(WARNING: Scraping this website is not allowed but you decided to force it)\033[0m")
             else:
```

### Comparing `scrapegraphai-1.2.1/scrapegraphai/nodes/search_internet_node.py` & `scrapegraphai-1.2.2/scrapegraphai/nodes/search_internet_node.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.2.1/scrapegraphai/nodes/search_link_node.py` & `scrapegraphai-1.2.2/scrapegraphai/nodes/search_link_node.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.2.1/scrapegraphai/nodes/text_to_speech_node.py` & `scrapegraphai-1.2.2/scrapegraphai/nodes/text_to_speech_node.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.2.1/scrapegraphai/utils/cleanup_html.py` & `scrapegraphai-1.2.2/scrapegraphai/utils/cleanup_html.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.2.1/scrapegraphai/utils/convert_to_csv.py` & `scrapegraphai-1.2.2/scrapegraphai/utils/convert_to_csv.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.2.1/scrapegraphai/utils/convert_to_json.py` & `scrapegraphai-1.2.2/scrapegraphai/utils/convert_to_json.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.2.1/scrapegraphai/utils/parse_state_keys.py` & `scrapegraphai-1.2.2/scrapegraphai/utils/parse_state_keys.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.2.1/scrapegraphai/utils/prettify_exec_info.py` & `scrapegraphai-1.2.2/scrapegraphai/utils/prettify_exec_info.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.2.1/scrapegraphai/utils/proxy_rotation.py` & `scrapegraphai-1.2.2/scrapegraphai/utils/proxy_rotation.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.2.1/scrapegraphai/utils/research_web.py` & `scrapegraphai-1.2.2/scrapegraphai/utils/research_web.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.2.1/scrapegraphai/utils/save_audio_from_bytes.py` & `scrapegraphai-1.2.2/scrapegraphai/utils/save_audio_from_bytes.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.2.1/scrapegraphai/utils/sys_dynamic_import.py` & `scrapegraphai-1.2.2/scrapegraphai/utils/sys_dynamic_import.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.2.1/scrapegraphai/utils/token_calculator.py` & `scrapegraphai-1.2.2/scrapegraphai/utils/token_calculator.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.2.1/tests/graphs/scrape_json_ollama.py` & `scrapegraphai-1.2.2/tests/graphs/scrape_json_ollama.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.2.1/tests/graphs/scrape_plain_text_llama3_test.py` & `scrapegraphai-1.2.2/tests/graphs/scrape_plain_text_llama3_test.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.2.1/tests/graphs/scrape_plain_text_mistral_test.py` & `scrapegraphai-1.2.2/tests/graphs/scrape_plain_text_mistral_test.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.2.1/tests/graphs/scrape_xml_ollama_test.py` & `scrapegraphai-1.2.2/tests/graphs/scrape_xml_ollama_test.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.2.1/tests/graphs/script_generator_test.py` & `scrapegraphai-1.2.2/tests/graphs/script_generator_test.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.2.1/tests/graphs/smart_scraper_ollama_test.py` & `scrapegraphai-1.2.2/tests/graphs/smart_scraper_ollama_test.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.2.1/tests/graphs/inputs/books.xml` & `scrapegraphai-1.2.2/tests/graphs/inputs/books.xml`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.2.1/tests/graphs/inputs/example.json` & `scrapegraphai-1.2.2/tests/graphs/inputs/example.json`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.2.1/tests/graphs/inputs/plain_html_example.txt` & `scrapegraphai-1.2.2/tests/graphs/inputs/plain_html_example.txt`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.2.1/tests/nodes/fetch_node_test.py` & `scrapegraphai-1.2.2/tests/nodes/fetch_node_test.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.2.1/tests/nodes/robot_node_test.py` & `scrapegraphai-1.2.2/tests/nodes/robot_node_test.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.2.1/tests/utils/test_proxy_rotation.py` & `scrapegraphai-1.2.2/tests/utils/test_proxy_rotation.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.2.1/tests/utils/test_sys_dynamic_import.py` & `scrapegraphai-1.2.2/tests/utils/test_sys_dynamic_import.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.2.1/LICENSE` & `scrapegraphai-1.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.2.1/README.md` & `scrapegraphai-1.2.2/README.md`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.2.1/pyproject.toml` & `scrapegraphai-1.2.2/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 [project]
 name = "scrapegraphai"
 
-version = "1.2.1"
+version = "1.2.2"
 
 description = "A web scraping library based on LangChain which uses LLM and direct graph logic to create scraping pipelines."
 authors = [
     { name = "Marco Vinciguerra", email = "mvincig11@gmail.com" },
     { name = "Marco Perini", email = "perinim.98@gmail.com" },
     { name = "Lorenzo Padoan", email = "lorenzo.padoan977@gmail.com" }
 ]
 dependencies = [
+    # python = ">=3.9, <3.12"
     "langchain==0.1.15",
     "langchain-openai==0.1.6",
     "langchain-google-genai==1.0.3",
     "langchain-groq==0.1.3",
     "langchain-aws==0.1.3",
     "langchain-anthropic==0.1.11",
     "html2text==2024.2.26",
@@ -57,22 +58,20 @@
 ]
 classifiers = [
     "Intended Audience :: Developers",
     "Topic :: Software Development :: Libraries :: Python Modules",
     "Programming Language :: Python :: 3",
     "Operating System :: OS Independent",
 ]
-requires-python = ">= 3.9, < 3.12"
-
+requires-python = ">= 3.9"
 
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
-
 [tool.rye]
 managed = true
 dev-dependencies = [
     "pytest==8.0.0",
     "pytest-mock==3.14.0"
 ]
```

### Comparing `scrapegraphai-1.2.1/PKG-INFO` & `scrapegraphai-1.2.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 Metadata-Version: 2.3
 Name: scrapegraphai
-Version: 1.2.1
+Version: 1.2.2
 Summary: A web scraping library based on LangChain which uses LLM and direct graph logic to create scraping pipelines.
 Author-email: Marco Vinciguerra <mvincig11@gmail.com>, Marco Perini <perinim.98@gmail.com>, Lorenzo Padoan <lorenzo.padoan977@gmail.com>
 License-Expression: MIT
 License-File: LICENSE
 Keywords: ai,artificial intelligence,gpt,graph,langchain,machine learning,natural language processing,nlp,openai,rag,scrapegraph,scrapegraphai,scraping,web scraping,web scraping library,web scraping tool,webscraping
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
-Requires-Python: <3.12,>=3.9
+Requires-Python: >=3.9
 Requires-Dist: beautifulsoup4==4.12.3
 Requires-Dist: faiss-cpu==1.8.0
 Requires-Dist: free-proxy==1.1.1
 Requires-Dist: google==3.0.0
 Requires-Dist: graphviz==0.20.3
 Requires-Dist: html2text==2024.2.26
 Requires-Dist: langchain-anthropic==0.1.11
```

