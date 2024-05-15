# Comparing `tmp/hezar-0.36.1.tar.gz` & `tmp/hezar-0.37.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hezar-0.36.1.tar", max compression
+gzip compressed data, was "hezar-0.37.0.tar", max compression
```

## Comparing `hezar-0.36.1.tar` & `hezar-0.37.0.tar`

### file list

```diff
@@ -1,136 +1,136 @@
--rw-r--r--   0        0        0    11337 2024-04-25 07:35:04.374585 hezar-0.36.1/LICENSE
--rw-r--r--   0        0        0    14442 2024-04-25 07:35:04.374585 hezar-0.36.1/README.md
--rw-r--r--   0        0        0      623 2024-04-25 07:35:04.378585 hezar-0.36.1/hezar/__init__.py
--rw-r--r--   0        0        0     5651 2024-04-25 07:35:04.378585 hezar-0.36.1/hezar/builders.py
--rw-r--r--   0        0        0    16908 2024-04-25 07:35:04.378585 hezar-0.36.1/hezar/configs.py
--rw-r--r--   0        0        0     4712 2024-04-25 07:35:04.378585 hezar-0.36.1/hezar/constants.py
--rw-r--r--   0        0        0       54 2024-04-25 07:35:04.378585 hezar-0.36.1/hezar/data/__init__.py
--rw-r--r--   0        0        0    13746 2024-04-25 07:35:04.378585 hezar-0.36.1/hezar/data/data_collators.py
--rw-r--r--   0        0        0      634 2024-04-25 07:35:04.378585 hezar-0.36.1/hezar/data/datasets/__init__.py
--rw-r--r--   0        0        0     3279 2024-04-25 07:35:04.378585 hezar-0.36.1/hezar/data/datasets/dataset.py
--rw-r--r--   0        0        0     3727 2024-04-25 07:35:04.378585 hezar-0.36.1/hezar/data/datasets/image_captioning_dataset.py
--rw-r--r--   0        0        0     7384 2024-04-25 07:35:04.378585 hezar-0.36.1/hezar/data/datasets/ocr_dataset.py
--rw-r--r--   0        0        0     5923 2024-04-25 07:35:04.378585 hezar-0.36.1/hezar/data/datasets/sequence_labeling_dataset.py
--rw-r--r--   0        0        0     3030 2024-04-25 07:35:04.378585 hezar-0.36.1/hezar/data/datasets/speech_recognition_dataset.py
--rw-r--r--   0        0        0     4498 2024-04-25 07:35:04.378585 hezar-0.36.1/hezar/data/datasets/text_classification_dataset.py
--rw-r--r--   0        0        0     4820 2024-04-25 07:35:04.378585 hezar-0.36.1/hezar/data/datasets/text_summarization_dataset.py
--rw-r--r--   0        0        0      202 2024-04-25 07:35:04.378585 hezar-0.36.1/hezar/embeddings/__init__.py
--rw-r--r--   0        0        0    11544 2024-04-25 07:35:04.378585 hezar-0.36.1/hezar/embeddings/embedding.py
--rw-r--r--   0        0        0     7171 2024-04-25 07:35:04.378585 hezar-0.36.1/hezar/embeddings/fasttext.py
--rw-r--r--   0        0        0     7668 2024-04-25 07:35:04.378585 hezar-0.36.1/hezar/embeddings/word2vec.py
--rw-r--r--   0        0        0      444 2024-04-25 07:35:04.378585 hezar-0.36.1/hezar/metrics/__init__.py
--rw-r--r--   0        0        0     2285 2024-04-25 07:35:04.378585 hezar-0.36.1/hezar/metrics/accuracy.py
--rw-r--r--   0        0        0     2484 2024-04-25 07:35:04.378585 hezar-0.36.1/hezar/metrics/bleu.py
--rw-r--r--   0        0        0     3711 2024-04-25 07:35:04.378585 hezar-0.36.1/hezar/metrics/cer.py
--rw-r--r--   0        0        0     3209 2024-04-25 07:35:04.378585 hezar-0.36.1/hezar/metrics/f1.py
--rw-r--r--   0        0        0     1302 2024-04-25 07:35:04.378585 hezar-0.36.1/hezar/metrics/metric.py
--rw-r--r--   0        0        0     3566 2024-04-25 07:35:04.378585 hezar-0.36.1/hezar/metrics/precision.py
--rw-r--r--   0        0        0     3509 2024-04-25 07:35:04.378585 hezar-0.36.1/hezar/metrics/recall.py
--rw-r--r--   0        0        0     3155 2024-04-25 07:35:04.378585 hezar-0.36.1/hezar/metrics/rouge.py
--rw-r--r--   0        0        0     4029 2024-04-25 07:35:04.378585 hezar-0.36.1/hezar/metrics/seqeval.py
--rw-r--r--   0        0        0     2950 2024-04-25 07:35:04.378585 hezar-0.36.1/hezar/metrics/wer.py
--rw-r--r--   0        0        0      333 2024-04-25 07:35:04.378585 hezar-0.36.1/hezar/models/__init__.py
--rw-r--r--   0        0        0       88 2024-04-25 07:35:04.378585 hezar-0.36.1/hezar/models/backbone/__init__.py
--rw-r--r--   0        0        0       35 2024-04-25 07:35:04.378585 hezar-0.36.1/hezar/models/backbone/bert/__init__.py
--rw-r--r--   0        0        0     2787 2024-04-25 07:35:04.378585 hezar-0.36.1/hezar/models/backbone/bert/bert.py
--rw-r--r--   0        0        0      743 2024-04-25 07:35:04.378585 hezar-0.36.1/hezar/models/backbone/bert/bert_config.py
--rw-r--r--   0        0        0       53 2024-04-25 07:35:04.378585 hezar-0.36.1/hezar/models/backbone/distilbert/__init__.py
--rw-r--r--   0        0        0     2288 2024-04-25 07:35:04.378585 hezar-0.36.1/hezar/models/backbone/distilbert/distilbert.py
--rw-r--r--   0        0        0      618 2024-04-25 07:35:04.378585 hezar-0.36.1/hezar/models/backbone/distilbert/distilbert_config.py
--rw-r--r--   0        0        0       44 2024-04-25 07:35:04.378585 hezar-0.36.1/hezar/models/backbone/roberta/__init__.py
--rw-r--r--   0        0        0     2788 2024-04-25 07:35:04.378585 hezar-0.36.1/hezar/models/backbone/roberta/roberta.py
--rw-r--r--   0        0        0      812 2024-04-25 07:35:04.378585 hezar-0.36.1/hezar/models/backbone/roberta/roberta_config.py
--rw-r--r--   0        0        0       55 2024-04-25 07:35:04.378585 hezar-0.36.1/hezar/models/backbone/vit/__init__.py
--rw-r--r--   0        0        0     2172 2024-04-25 07:35:04.378585 hezar-0.36.1/hezar/models/backbone/vit/vit.py
--rw-r--r--   0        0        0      572 2024-04-25 07:35:04.378585 hezar-0.36.1/hezar/models/backbone/vit/vit_config.py
--rw-r--r--   0        0        0      120 2024-04-25 07:35:04.378585 hezar-0.36.1/hezar/models/image2text/__init__.py
--rw-r--r--   0        0        0      131 2024-04-25 07:35:04.378585 hezar-0.36.1/hezar/models/image2text/beit_roberta/__init__.py
--rw-r--r--   0        0        0     3493 2024-04-25 07:35:04.378585 hezar-0.36.1/hezar/models/image2text/beit_roberta/beit_roberta_image2text.py
--rw-r--r--   0        0        0     2376 2024-04-25 07:35:04.378585 hezar-0.36.1/hezar/models/image2text/beit_roberta/beit_roberta_image2text_config.py
--rw-r--r--   0        0        0      101 2024-04-25 07:35:04.378585 hezar-0.36.1/hezar/models/image2text/crnn/__init__.py
--rw-r--r--   0        0        0     1106 2024-04-25 07:35:04.378585 hezar-0.36.1/hezar/models/image2text/crnn/crnn_decode_utils.py
--rw-r--r--   0        0        0     4649 2024-04-25 07:35:04.378585 hezar-0.36.1/hezar/models/image2text/crnn/crnn_image2text.py
--rw-r--r--   0        0        0      478 2024-04-25 07:35:04.378585 hezar-0.36.1/hezar/models/image2text/crnn/crnn_image2text_config.py
--rw-r--r--   0        0        0      105 2024-04-25 07:35:04.378585 hezar-0.36.1/hezar/models/image2text/trocr/__init__.py
--rw-r--r--   0        0        0     3430 2024-04-25 07:35:04.378585 hezar-0.36.1/hezar/models/image2text/trocr/trocr_image2text.py
--rw-r--r--   0        0        0     1899 2024-04-25 07:35:04.378585 hezar-0.36.1/hezar/models/image2text/trocr/trocr_image2text_config.py
--rw-r--r--   0        0        0      115 2024-04-25 07:35:04.378585 hezar-0.36.1/hezar/models/image2text/vit_gpt2/__init__.py
--rw-r--r--   0        0        0     3463 2024-04-25 07:35:04.378585 hezar-0.36.1/hezar/models/image2text/vit_gpt2/vit_gpt2_image2text.py
--rw-r--r--   0        0        0     1872 2024-04-25 07:35:04.378585 hezar-0.36.1/hezar/models/image2text/vit_gpt2/vit_gpt2_image2text_config.py
--rw-r--r--   0        0        0      127 2024-04-25 07:35:04.378585 hezar-0.36.1/hezar/models/image2text/vit_roberta/__init__.py
--rw-r--r--   0        0        0     3864 2024-04-25 07:35:04.378585 hezar-0.36.1/hezar/models/image2text/vit_roberta/vit_roberta_image2text.py
--rw-r--r--   0        0        0     1952 2024-04-25 07:35:04.378585 hezar-0.36.1/hezar/models/image2text/vit_roberta/vit_roberta_image2text_config.py
--rw-r--r--   0        0        0       69 2024-04-25 07:35:04.378585 hezar-0.36.1/hezar/models/mask_filling/__init__.py
--rw-r--r--   0        0        0      107 2024-04-25 07:35:04.378585 hezar-0.36.1/hezar/models/mask_filling/bert/__init__.py
--rw-r--r--   0        0        0     4320 2024-04-25 07:35:04.382585 hezar-0.36.1/hezar/models/mask_filling/bert/bert_mask_filling.py
--rw-r--r--   0        0        0      771 2024-04-25 07:35:04.382585 hezar-0.36.1/hezar/models/mask_filling/bert/bert_mask_filling_config.py
--rw-r--r--   0        0        0      131 2024-04-25 07:35:04.382585 hezar-0.36.1/hezar/models/mask_filling/distilbert/__init__.py
--rw-r--r--   0        0        0     3921 2024-04-25 07:35:04.382585 hezar-0.36.1/hezar/models/mask_filling/distilbert/distilbert_mask_filling.py
--rw-r--r--   0        0        0      637 2024-04-25 07:35:04.382585 hezar-0.36.1/hezar/models/mask_filling/distilbert/distilbert_mask_filling_config.py
--rw-r--r--   0        0        0      119 2024-04-25 07:35:04.382585 hezar-0.36.1/hezar/models/mask_filling/roberta/__init__.py
--rw-r--r--   0        0        0     4384 2024-04-25 07:35:04.382585 hezar-0.36.1/hezar/models/mask_filling/roberta/roberta_mask_filling.py
--rw-r--r--   0        0        0      831 2024-04-25 07:35:04.382585 hezar-0.36.1/hezar/models/mask_filling/roberta/roberta_mask_filling_config.py
--rw-r--r--   0        0        0    20158 2024-04-25 07:35:04.382585 hezar-0.36.1/hezar/models/model.py
--rw-r--r--   0        0        0     2141 2024-04-25 07:35:04.382585 hezar-0.36.1/hezar/models/model_outputs.py
--rw-r--r--   0        0        0       69 2024-04-25 07:35:04.382585 hezar-0.36.1/hezar/models/sequence_labeling/__init__.py
--rw-r--r--   0        0        0      127 2024-04-25 07:35:04.382585 hezar-0.36.1/hezar/models/sequence_labeling/bert/__init__.py
--rw-r--r--   0        0        0     5118 2024-04-25 07:35:04.382585 hezar-0.36.1/hezar/models/sequence_labeling/bert/bert_sequence_labeling.py
--rw-r--r--   0        0        0      931 2024-04-25 07:35:04.382585 hezar-0.36.1/hezar/models/sequence_labeling/bert/bert_sequence_labeling_config.py
--rw-r--r--   0        0        0      151 2024-04-25 07:35:04.382585 hezar-0.36.1/hezar/models/sequence_labeling/distilbert/__init__.py
--rw-r--r--   0        0        0     5172 2024-04-25 07:35:04.382585 hezar-0.36.1/hezar/models/sequence_labeling/distilbert/distilbert_sequence_labeling.py
--rw-r--r--   0        0        0      872 2024-04-25 07:35:04.382585 hezar-0.36.1/hezar/models/sequence_labeling/distilbert/distilbert_sequence_labeling_config.py
--rw-r--r--   0        0        0      139 2024-04-25 07:35:04.382585 hezar-0.36.1/hezar/models/sequence_labeling/roberta/__init__.py
--rw-r--r--   0        0        0     5821 2024-04-25 07:35:04.382585 hezar-0.36.1/hezar/models/sequence_labeling/roberta/roberta_sequence_labeling.py
--rw-r--r--   0        0        0     1025 2024-04-25 07:35:04.382585 hezar-0.36.1/hezar/models/sequence_labeling/roberta/roberta_sequence_labeling_config.py
--rw-r--r--   0        0        0       23 2024-04-25 07:35:04.382585 hezar-0.36.1/hezar/models/speech_recognition/__init__.py
--rw-r--r--   0        0        0      306 2024-04-25 07:35:04.382585 hezar-0.36.1/hezar/models/speech_recognition/whisper/__init__.py
--rw-r--r--   0        0        0     7713 2024-04-25 07:35:04.382585 hezar-0.36.1/hezar/models/speech_recognition/whisper/whisper_feature_extractor.py
--rw-r--r--   0        0        0     6197 2024-04-25 07:35:04.382585 hezar-0.36.1/hezar/models/speech_recognition/whisper/whisper_speech_recognition.py
--rw-r--r--   0        0        0     1572 2024-04-25 07:35:04.382585 hezar-0.36.1/hezar/models/speech_recognition/whisper/whisper_speech_recognition_config.py
--rw-r--r--   0        0        0    26128 2024-04-25 07:35:04.382585 hezar-0.36.1/hezar/models/speech_recognition/whisper/whisper_tokenizer.py
--rw-r--r--   0        0        0       69 2024-04-25 07:35:04.382585 hezar-0.36.1/hezar/models/text_classification/__init__.py
--rw-r--r--   0        0        0      135 2024-04-25 07:35:04.382585 hezar-0.36.1/hezar/models/text_classification/bert/__init__.py
--rw-r--r--   0        0        0     4796 2024-04-25 07:35:04.382585 hezar-0.36.1/hezar/models/text_classification/bert/bert_text_classification.py
--rw-r--r--   0        0        0      845 2024-04-25 07:35:04.382585 hezar-0.36.1/hezar/models/text_classification/bert/bert_text_classification_config.py
--rw-r--r--   0        0        0      159 2024-04-25 07:35:04.382585 hezar-0.36.1/hezar/models/text_classification/distilbert/__init__.py
--rw-r--r--   0        0        0     4357 2024-04-25 07:35:04.382585 hezar-0.36.1/hezar/models/text_classification/distilbert/distilbert_text_classification.py
--rw-r--r--   0        0        0      748 2024-04-25 07:35:04.382585 hezar-0.36.1/hezar/models/text_classification/distilbert/distilbert_text_classification_config.py
--rw-r--r--   0        0        0      147 2024-04-25 07:35:04.382585 hezar-0.36.1/hezar/models/text_classification/roberta/__init__.py
--rw-r--r--   0        0        0     4963 2024-04-25 07:35:04.382585 hezar-0.36.1/hezar/models/text_classification/roberta/roberta_text_classification.py
--rw-r--r--   0        0        0      942 2024-04-25 07:35:04.382585 hezar-0.36.1/hezar/models/text_classification/roberta/roberta_text_classification_config.py
--rw-r--r--   0        0        0        0 2024-04-25 07:35:04.382585 hezar-0.36.1/hezar/models/text_embedding/__init__.py
--rw-r--r--   0        0        0       38 2024-04-25 07:35:04.382585 hezar-0.36.1/hezar/models/text_generation/__init__.py
--rw-r--r--   0        0        0      119 2024-04-25 07:35:04.382585 hezar-0.36.1/hezar/models/text_generation/gpt2/__init__.py
--rw-r--r--   0        0        0     3324 2024-04-25 07:35:04.382585 hezar-0.36.1/hezar/models/text_generation/gpt2/gpt2_text_generation.py
--rw-r--r--   0        0        0     1148 2024-04-25 07:35:04.382585 hezar-0.36.1/hezar/models/text_generation/gpt2/gpt2_text_generation_config.py
--rw-r--r--   0        0        0      111 2024-04-25 07:35:04.382585 hezar-0.36.1/hezar/models/text_generation/t5/__init__.py
--rw-r--r--   0        0        0     4053 2024-04-25 07:35:04.382585 hezar-0.36.1/hezar/models/text_generation/t5/t5_text_generation.py
--rw-r--r--   0        0        0      837 2024-04-25 07:35:04.382585 hezar-0.36.1/hezar/models/text_generation/t5/t5_text_generation_config.py
--rw-r--r--   0        0        0      390 2024-04-25 07:35:04.382585 hezar-0.36.1/hezar/preprocessors/__init__.py
--rw-r--r--   0        0        0    13309 2024-04-25 07:35:04.382585 hezar-0.36.1/hezar/preprocessors/audio_feature_extractor.py
--rw-r--r--   0        0        0     8292 2024-04-25 07:35:04.382585 hezar-0.36.1/hezar/preprocessors/image_processor.py
--rw-r--r--   0        0        0     5043 2024-04-25 07:35:04.382585 hezar-0.36.1/hezar/preprocessors/preprocessor.py
--rw-r--r--   0        0        0     4635 2024-04-25 07:35:04.382585 hezar-0.36.1/hezar/preprocessors/text_normalizer.py
--rw-r--r--   0        0        0      337 2024-04-25 07:35:04.382585 hezar-0.36.1/hezar/preprocessors/tokenizers/__init__.py
--rw-r--r--   0        0        0     3973 2024-04-25 07:35:04.382585 hezar-0.36.1/hezar/preprocessors/tokenizers/bpe.py
--rw-r--r--   0        0        0     4181 2024-04-25 07:35:04.382585 hezar-0.36.1/hezar/preprocessors/tokenizers/sentencepiece_bpe.py
--rw-r--r--   0        0        0     4102 2024-04-25 07:35:04.382585 hezar-0.36.1/hezar/preprocessors/tokenizers/sentencepiece_unigram.py
--rw-r--r--   0        0        0    27637 2024-04-25 07:35:04.382585 hezar-0.36.1/hezar/preprocessors/tokenizers/tokenizer.py
--rw-r--r--   0        0        0     3537 2024-04-25 07:35:04.382585 hezar-0.36.1/hezar/preprocessors/tokenizers/wordpiece.py
--rw-r--r--   0        0        0     6584 2024-04-25 07:35:04.382585 hezar-0.36.1/hezar/registry.py
--rw-r--r--   0        0        0      113 2024-04-25 07:35:04.382585 hezar-0.36.1/hezar/trainer/__init__.py
--rw-r--r--   0        0        0     7097 2024-04-25 07:35:04.382585 hezar-0.36.1/hezar/trainer/metrics_handlers.py
--rw-r--r--   0        0        0    30740 2024-04-25 07:35:04.382585 hezar-0.36.1/hezar/trainer/trainer.py
--rw-r--r--   0        0        0     4963 2024-04-25 07:35:04.382585 hezar-0.36.1/hezar/trainer/trainer_utils.py
--rw-r--r--   0        0        0      245 2024-04-25 07:35:04.382585 hezar-0.36.1/hezar/utils/__init__.py
--rw-r--r--   0        0        0    23979 2024-04-25 07:35:04.382585 hezar-0.36.1/hezar/utils/audio_utils.py
--rw-r--r--   0        0        0     3955 2024-04-25 07:35:04.382585 hezar-0.36.1/hezar/utils/common_utils.py
--rw-r--r--   0        0        0     6884 2024-04-25 07:35:04.382585 hezar-0.36.1/hezar/utils/data_utils.py
--rw-r--r--   0        0        0      976 2024-04-25 07:35:04.382585 hezar-0.36.1/hezar/utils/file_utils.py
--rw-r--r--   0        0        0     4903 2024-04-25 07:35:04.382585 hezar-0.36.1/hezar/utils/hub_utils.py
--rw-r--r--   0        0        0     7352 2024-04-25 07:35:04.382585 hezar-0.36.1/hezar/utils/image_utils.py
--rw-r--r--   0        0        0     1376 2024-04-25 07:35:04.382585 hezar-0.36.1/hezar/utils/integration_utils.py
--rw-r--r--   0        0        0      622 2024-04-25 07:35:04.382585 hezar-0.36.1/hezar/utils/logging.py
--rw-r--r--   0        0        0     4498 2024-04-25 07:35:04.382585 hezar-0.36.1/hezar/utils/registry_utils.py
--rw-r--r--   0        0        0     2632 2024-04-25 07:35:04.386585 hezar-0.36.1/pyproject.toml
--rw-r--r--   0        0        0    17058 1970-01-01 00:00:00.000000 hezar-0.36.1/PKG-INFO
+-rw-r--r--   0        0        0    11337 2024-05-15 19:20:22.371938 hezar-0.37.0/LICENSE
+-rw-r--r--   0        0        0    14442 2024-05-15 19:20:22.371938 hezar-0.37.0/README.md
+-rw-r--r--   0        0        0      623 2024-05-15 19:20:22.371938 hezar-0.37.0/hezar/__init__.py
+-rw-r--r--   0        0        0     5651 2024-05-15 19:20:22.371938 hezar-0.37.0/hezar/builders.py
+-rw-r--r--   0        0        0    18042 2024-05-15 19:20:22.371938 hezar-0.37.0/hezar/configs.py
+-rw-r--r--   0        0        0     4712 2024-05-15 19:20:22.371938 hezar-0.37.0/hezar/constants.py
+-rw-r--r--   0        0        0       54 2024-05-15 19:20:22.371938 hezar-0.37.0/hezar/data/__init__.py
+-rw-r--r--   0        0        0    13756 2024-05-15 19:20:22.375938 hezar-0.37.0/hezar/data/data_collators.py
+-rw-r--r--   0        0        0      634 2024-05-15 19:20:22.375938 hezar-0.37.0/hezar/data/datasets/__init__.py
+-rw-r--r--   0        0        0     3760 2024-05-15 19:20:22.375938 hezar-0.37.0/hezar/data/datasets/dataset.py
+-rw-r--r--   0        0        0     3727 2024-05-15 19:20:22.375938 hezar-0.37.0/hezar/data/datasets/image_captioning_dataset.py
+-rw-r--r--   0        0        0     7384 2024-05-15 19:20:22.375938 hezar-0.37.0/hezar/data/datasets/ocr_dataset.py
+-rw-r--r--   0        0        0     5923 2024-05-15 19:20:22.375938 hezar-0.37.0/hezar/data/datasets/sequence_labeling_dataset.py
+-rw-r--r--   0        0        0     3079 2024-05-15 19:20:22.375938 hezar-0.37.0/hezar/data/datasets/speech_recognition_dataset.py
+-rw-r--r--   0        0        0     4498 2024-05-15 19:20:22.375938 hezar-0.37.0/hezar/data/datasets/text_classification_dataset.py
+-rw-r--r--   0        0        0     4820 2024-05-15 19:20:22.375938 hezar-0.37.0/hezar/data/datasets/text_summarization_dataset.py
+-rw-r--r--   0        0        0      202 2024-05-15 19:20:22.375938 hezar-0.37.0/hezar/embeddings/__init__.py
+-rw-r--r--   0        0        0    11544 2024-05-15 19:20:22.375938 hezar-0.37.0/hezar/embeddings/embedding.py
+-rw-r--r--   0        0        0     7171 2024-05-15 19:20:22.375938 hezar-0.37.0/hezar/embeddings/fasttext.py
+-rw-r--r--   0        0        0     7668 2024-05-15 19:20:22.375938 hezar-0.37.0/hezar/embeddings/word2vec.py
+-rw-r--r--   0        0        0      444 2024-05-15 19:20:22.375938 hezar-0.37.0/hezar/metrics/__init__.py
+-rw-r--r--   0        0        0     2285 2024-05-15 19:20:22.375938 hezar-0.37.0/hezar/metrics/accuracy.py
+-rw-r--r--   0        0        0     2484 2024-05-15 19:20:22.375938 hezar-0.37.0/hezar/metrics/bleu.py
+-rw-r--r--   0        0        0     3711 2024-05-15 19:20:22.375938 hezar-0.37.0/hezar/metrics/cer.py
+-rw-r--r--   0        0        0     3209 2024-05-15 19:20:22.375938 hezar-0.37.0/hezar/metrics/f1.py
+-rw-r--r--   0        0        0     1302 2024-05-15 19:20:22.375938 hezar-0.37.0/hezar/metrics/metric.py
+-rw-r--r--   0        0        0     3566 2024-05-15 19:20:22.375938 hezar-0.37.0/hezar/metrics/precision.py
+-rw-r--r--   0        0        0     3509 2024-05-15 19:20:22.375938 hezar-0.37.0/hezar/metrics/recall.py
+-rw-r--r--   0        0        0     3155 2024-05-15 19:20:22.375938 hezar-0.37.0/hezar/metrics/rouge.py
+-rw-r--r--   0        0        0     4029 2024-05-15 19:20:22.375938 hezar-0.37.0/hezar/metrics/seqeval.py
+-rw-r--r--   0        0        0     2950 2024-05-15 19:20:22.375938 hezar-0.37.0/hezar/metrics/wer.py
+-rw-r--r--   0        0        0      333 2024-05-15 19:20:22.375938 hezar-0.37.0/hezar/models/__init__.py
+-rw-r--r--   0        0        0       88 2024-05-15 19:20:22.375938 hezar-0.37.0/hezar/models/backbone/__init__.py
+-rw-r--r--   0        0        0       35 2024-05-15 19:20:22.375938 hezar-0.37.0/hezar/models/backbone/bert/__init__.py
+-rw-r--r--   0        0        0     2787 2024-05-15 19:20:22.375938 hezar-0.37.0/hezar/models/backbone/bert/bert.py
+-rw-r--r--   0        0        0      743 2024-05-15 19:20:22.375938 hezar-0.37.0/hezar/models/backbone/bert/bert_config.py
+-rw-r--r--   0        0        0       53 2024-05-15 19:20:22.375938 hezar-0.37.0/hezar/models/backbone/distilbert/__init__.py
+-rw-r--r--   0        0        0     2288 2024-05-15 19:20:22.375938 hezar-0.37.0/hezar/models/backbone/distilbert/distilbert.py
+-rw-r--r--   0        0        0      618 2024-05-15 19:20:22.375938 hezar-0.37.0/hezar/models/backbone/distilbert/distilbert_config.py
+-rw-r--r--   0        0        0       44 2024-05-15 19:20:22.375938 hezar-0.37.0/hezar/models/backbone/roberta/__init__.py
+-rw-r--r--   0        0        0     2788 2024-05-15 19:20:22.375938 hezar-0.37.0/hezar/models/backbone/roberta/roberta.py
+-rw-r--r--   0        0        0      812 2024-05-15 19:20:22.375938 hezar-0.37.0/hezar/models/backbone/roberta/roberta_config.py
+-rw-r--r--   0        0        0       55 2024-05-15 19:20:22.375938 hezar-0.37.0/hezar/models/backbone/vit/__init__.py
+-rw-r--r--   0        0        0     2172 2024-05-15 19:20:22.375938 hezar-0.37.0/hezar/models/backbone/vit/vit.py
+-rw-r--r--   0        0        0      572 2024-05-15 19:20:22.375938 hezar-0.37.0/hezar/models/backbone/vit/vit_config.py
+-rw-r--r--   0        0        0      120 2024-05-15 19:20:22.375938 hezar-0.37.0/hezar/models/image2text/__init__.py
+-rw-r--r--   0        0        0      131 2024-05-15 19:20:22.375938 hezar-0.37.0/hezar/models/image2text/beit_roberta/__init__.py
+-rw-r--r--   0        0        0     3493 2024-05-15 19:20:22.375938 hezar-0.37.0/hezar/models/image2text/beit_roberta/beit_roberta_image2text.py
+-rw-r--r--   0        0        0     2376 2024-05-15 19:20:22.375938 hezar-0.37.0/hezar/models/image2text/beit_roberta/beit_roberta_image2text_config.py
+-rw-r--r--   0        0        0      101 2024-05-15 19:20:22.375938 hezar-0.37.0/hezar/models/image2text/crnn/__init__.py
+-rw-r--r--   0        0        0     1106 2024-05-15 19:20:22.375938 hezar-0.37.0/hezar/models/image2text/crnn/crnn_decode_utils.py
+-rw-r--r--   0        0        0     4649 2024-05-15 19:20:22.375938 hezar-0.37.0/hezar/models/image2text/crnn/crnn_image2text.py
+-rw-r--r--   0        0        0      478 2024-05-15 19:20:22.375938 hezar-0.37.0/hezar/models/image2text/crnn/crnn_image2text_config.py
+-rw-r--r--   0        0        0      105 2024-05-15 19:20:22.375938 hezar-0.37.0/hezar/models/image2text/trocr/__init__.py
+-rw-r--r--   0        0        0     3430 2024-05-15 19:20:22.375938 hezar-0.37.0/hezar/models/image2text/trocr/trocr_image2text.py
+-rw-r--r--   0        0        0     1899 2024-05-15 19:20:22.375938 hezar-0.37.0/hezar/models/image2text/trocr/trocr_image2text_config.py
+-rw-r--r--   0        0        0      115 2024-05-15 19:20:22.375938 hezar-0.37.0/hezar/models/image2text/vit_gpt2/__init__.py
+-rw-r--r--   0        0        0     3463 2024-05-15 19:20:22.375938 hezar-0.37.0/hezar/models/image2text/vit_gpt2/vit_gpt2_image2text.py
+-rw-r--r--   0        0        0     1872 2024-05-15 19:20:22.375938 hezar-0.37.0/hezar/models/image2text/vit_gpt2/vit_gpt2_image2text_config.py
+-rw-r--r--   0        0        0      127 2024-05-15 19:20:22.375938 hezar-0.37.0/hezar/models/image2text/vit_roberta/__init__.py
+-rw-r--r--   0        0        0     3864 2024-05-15 19:20:22.375938 hezar-0.37.0/hezar/models/image2text/vit_roberta/vit_roberta_image2text.py
+-rw-r--r--   0        0        0     1952 2024-05-15 19:20:22.375938 hezar-0.37.0/hezar/models/image2text/vit_roberta/vit_roberta_image2text_config.py
+-rw-r--r--   0        0        0       69 2024-05-15 19:20:22.375938 hezar-0.37.0/hezar/models/mask_filling/__init__.py
+-rw-r--r--   0        0        0      107 2024-05-15 19:20:22.375938 hezar-0.37.0/hezar/models/mask_filling/bert/__init__.py
+-rw-r--r--   0        0        0     4320 2024-05-15 19:20:22.375938 hezar-0.37.0/hezar/models/mask_filling/bert/bert_mask_filling.py
+-rw-r--r--   0        0        0      771 2024-05-15 19:20:22.375938 hezar-0.37.0/hezar/models/mask_filling/bert/bert_mask_filling_config.py
+-rw-r--r--   0        0        0      131 2024-05-15 19:20:22.375938 hezar-0.37.0/hezar/models/mask_filling/distilbert/__init__.py
+-rw-r--r--   0        0        0     3921 2024-05-15 19:20:22.375938 hezar-0.37.0/hezar/models/mask_filling/distilbert/distilbert_mask_filling.py
+-rw-r--r--   0        0        0      637 2024-05-15 19:20:22.375938 hezar-0.37.0/hezar/models/mask_filling/distilbert/distilbert_mask_filling_config.py
+-rw-r--r--   0        0        0      119 2024-05-15 19:20:22.375938 hezar-0.37.0/hezar/models/mask_filling/roberta/__init__.py
+-rw-r--r--   0        0        0     4384 2024-05-15 19:20:22.375938 hezar-0.37.0/hezar/models/mask_filling/roberta/roberta_mask_filling.py
+-rw-r--r--   0        0        0      831 2024-05-15 19:20:22.375938 hezar-0.37.0/hezar/models/mask_filling/roberta/roberta_mask_filling_config.py
+-rw-r--r--   0        0        0    20158 2024-05-15 19:20:22.375938 hezar-0.37.0/hezar/models/model.py
+-rw-r--r--   0        0        0     2141 2024-05-15 19:20:22.375938 hezar-0.37.0/hezar/models/model_outputs.py
+-rw-r--r--   0        0        0       69 2024-05-15 19:20:22.375938 hezar-0.37.0/hezar/models/sequence_labeling/__init__.py
+-rw-r--r--   0        0        0      127 2024-05-15 19:20:22.375938 hezar-0.37.0/hezar/models/sequence_labeling/bert/__init__.py
+-rw-r--r--   0        0        0     5118 2024-05-15 19:20:22.375938 hezar-0.37.0/hezar/models/sequence_labeling/bert/bert_sequence_labeling.py
+-rw-r--r--   0        0        0      931 2024-05-15 19:20:22.375938 hezar-0.37.0/hezar/models/sequence_labeling/bert/bert_sequence_labeling_config.py
+-rw-r--r--   0        0        0      151 2024-05-15 19:20:22.375938 hezar-0.37.0/hezar/models/sequence_labeling/distilbert/__init__.py
+-rw-r--r--   0        0        0     5172 2024-05-15 19:20:22.375938 hezar-0.37.0/hezar/models/sequence_labeling/distilbert/distilbert_sequence_labeling.py
+-rw-r--r--   0        0        0      872 2024-05-15 19:20:22.375938 hezar-0.37.0/hezar/models/sequence_labeling/distilbert/distilbert_sequence_labeling_config.py
+-rw-r--r--   0        0        0      139 2024-05-15 19:20:22.375938 hezar-0.37.0/hezar/models/sequence_labeling/roberta/__init__.py
+-rw-r--r--   0        0        0     5821 2024-05-15 19:20:22.375938 hezar-0.37.0/hezar/models/sequence_labeling/roberta/roberta_sequence_labeling.py
+-rw-r--r--   0        0        0     1025 2024-05-15 19:20:22.375938 hezar-0.37.0/hezar/models/sequence_labeling/roberta/roberta_sequence_labeling_config.py
+-rw-r--r--   0        0        0       23 2024-05-15 19:20:22.375938 hezar-0.37.0/hezar/models/speech_recognition/__init__.py
+-rw-r--r--   0        0        0      306 2024-05-15 19:20:22.375938 hezar-0.37.0/hezar/models/speech_recognition/whisper/__init__.py
+-rw-r--r--   0        0        0     7713 2024-05-15 19:20:22.379938 hezar-0.37.0/hezar/models/speech_recognition/whisper/whisper_feature_extractor.py
+-rw-r--r--   0        0        0     7059 2024-05-15 19:20:22.379938 hezar-0.37.0/hezar/models/speech_recognition/whisper/whisper_speech_recognition.py
+-rw-r--r--   0        0        0     2777 2024-05-15 19:20:22.379938 hezar-0.37.0/hezar/models/speech_recognition/whisper/whisper_speech_recognition_config.py
+-rw-r--r--   0        0        0    27594 2024-05-15 19:20:22.379938 hezar-0.37.0/hezar/models/speech_recognition/whisper/whisper_tokenizer.py
+-rw-r--r--   0        0        0       69 2024-05-15 19:20:22.379938 hezar-0.37.0/hezar/models/text_classification/__init__.py
+-rw-r--r--   0        0        0      135 2024-05-15 19:20:22.379938 hezar-0.37.0/hezar/models/text_classification/bert/__init__.py
+-rw-r--r--   0        0        0     4796 2024-05-15 19:20:22.379938 hezar-0.37.0/hezar/models/text_classification/bert/bert_text_classification.py
+-rw-r--r--   0        0        0      845 2024-05-15 19:20:22.379938 hezar-0.37.0/hezar/models/text_classification/bert/bert_text_classification_config.py
+-rw-r--r--   0        0        0      159 2024-05-15 19:20:22.379938 hezar-0.37.0/hezar/models/text_classification/distilbert/__init__.py
+-rw-r--r--   0        0        0     4357 2024-05-15 19:20:22.379938 hezar-0.37.0/hezar/models/text_classification/distilbert/distilbert_text_classification.py
+-rw-r--r--   0        0        0      748 2024-05-15 19:20:22.379938 hezar-0.37.0/hezar/models/text_classification/distilbert/distilbert_text_classification_config.py
+-rw-r--r--   0        0        0      147 2024-05-15 19:20:22.379938 hezar-0.37.0/hezar/models/text_classification/roberta/__init__.py
+-rw-r--r--   0        0        0     4963 2024-05-15 19:20:22.379938 hezar-0.37.0/hezar/models/text_classification/roberta/roberta_text_classification.py
+-rw-r--r--   0        0        0      942 2024-05-15 19:20:22.379938 hezar-0.37.0/hezar/models/text_classification/roberta/roberta_text_classification_config.py
+-rw-r--r--   0        0        0        0 2024-05-15 19:20:22.379938 hezar-0.37.0/hezar/models/text_embedding/__init__.py
+-rw-r--r--   0        0        0       38 2024-05-15 19:20:22.379938 hezar-0.37.0/hezar/models/text_generation/__init__.py
+-rw-r--r--   0        0        0      119 2024-05-15 19:20:22.379938 hezar-0.37.0/hezar/models/text_generation/gpt2/__init__.py
+-rw-r--r--   0        0        0     3324 2024-05-15 19:20:22.379938 hezar-0.37.0/hezar/models/text_generation/gpt2/gpt2_text_generation.py
+-rw-r--r--   0        0        0     1148 2024-05-15 19:20:22.379938 hezar-0.37.0/hezar/models/text_generation/gpt2/gpt2_text_generation_config.py
+-rw-r--r--   0        0        0      111 2024-05-15 19:20:22.379938 hezar-0.37.0/hezar/models/text_generation/t5/__init__.py
+-rw-r--r--   0        0        0     4053 2024-05-15 19:20:22.379938 hezar-0.37.0/hezar/models/text_generation/t5/t5_text_generation.py
+-rw-r--r--   0        0        0      837 2024-05-15 19:20:22.379938 hezar-0.37.0/hezar/models/text_generation/t5/t5_text_generation_config.py
+-rw-r--r--   0        0        0      390 2024-05-15 19:20:22.379938 hezar-0.37.0/hezar/preprocessors/__init__.py
+-rw-r--r--   0        0        0    13303 2024-05-15 19:20:22.379938 hezar-0.37.0/hezar/preprocessors/audio_feature_extractor.py
+-rw-r--r--   0        0        0     8292 2024-05-15 19:20:22.379938 hezar-0.37.0/hezar/preprocessors/image_processor.py
+-rw-r--r--   0        0        0     5043 2024-05-15 19:20:22.379938 hezar-0.37.0/hezar/preprocessors/preprocessor.py
+-rw-r--r--   0        0        0     4635 2024-05-15 19:20:22.379938 hezar-0.37.0/hezar/preprocessors/text_normalizer.py
+-rw-r--r--   0        0        0      337 2024-05-15 19:20:22.379938 hezar-0.37.0/hezar/preprocessors/tokenizers/__init__.py
+-rw-r--r--   0        0        0     3973 2024-05-15 19:20:22.379938 hezar-0.37.0/hezar/preprocessors/tokenizers/bpe.py
+-rw-r--r--   0        0        0     4181 2024-05-15 19:20:22.379938 hezar-0.37.0/hezar/preprocessors/tokenizers/sentencepiece_bpe.py
+-rw-r--r--   0        0        0     4102 2024-05-15 19:20:22.379938 hezar-0.37.0/hezar/preprocessors/tokenizers/sentencepiece_unigram.py
+-rw-r--r--   0        0        0    27637 2024-05-15 19:20:22.379938 hezar-0.37.0/hezar/preprocessors/tokenizers/tokenizer.py
+-rw-r--r--   0        0        0     3537 2024-05-15 19:20:22.379938 hezar-0.37.0/hezar/preprocessors/tokenizers/wordpiece.py
+-rw-r--r--   0        0        0     6584 2024-05-15 19:20:22.379938 hezar-0.37.0/hezar/registry.py
+-rw-r--r--   0        0        0      113 2024-05-15 19:20:22.379938 hezar-0.37.0/hezar/trainer/__init__.py
+-rw-r--r--   0        0        0     7345 2024-05-15 19:20:22.379938 hezar-0.37.0/hezar/trainer/metrics_handlers.py
+-rw-r--r--   0        0        0    31550 2024-05-15 19:20:22.379938 hezar-0.37.0/hezar/trainer/trainer.py
+-rw-r--r--   0        0        0     5624 2024-05-15 19:20:22.379938 hezar-0.37.0/hezar/trainer/trainer_utils.py
+-rw-r--r--   0        0        0      245 2024-05-15 19:20:22.379938 hezar-0.37.0/hezar/utils/__init__.py
+-rw-r--r--   0        0        0    23979 2024-05-15 19:20:22.379938 hezar-0.37.0/hezar/utils/audio_utils.py
+-rw-r--r--   0        0        0     3955 2024-05-15 19:20:22.379938 hezar-0.37.0/hezar/utils/common_utils.py
+-rw-r--r--   0        0        0     7676 2024-05-15 19:20:22.379938 hezar-0.37.0/hezar/utils/data_utils.py
+-rw-r--r--   0        0        0      976 2024-05-15 19:20:22.379938 hezar-0.37.0/hezar/utils/file_utils.py
+-rw-r--r--   0        0        0     4145 2024-05-15 19:20:22.379938 hezar-0.37.0/hezar/utils/hub_utils.py
+-rw-r--r--   0        0        0     7352 2024-05-15 19:20:22.379938 hezar-0.37.0/hezar/utils/image_utils.py
+-rw-r--r--   0        0        0     1376 2024-05-15 19:20:22.379938 hezar-0.37.0/hezar/utils/integration_utils.py
+-rw-r--r--   0        0        0      622 2024-05-15 19:20:22.379938 hezar-0.37.0/hezar/utils/logging.py
+-rw-r--r--   0        0        0     4498 2024-05-15 19:20:22.379938 hezar-0.37.0/hezar/utils/registry_utils.py
+-rw-r--r--   0        0        0     2600 2024-05-15 19:20:22.379938 hezar-0.37.0/pyproject.toml
+-rw-r--r--   0        0        0    17052 1970-01-01 00:00:00.000000 hezar-0.37.0/PKG-INFO
```

### Comparing `hezar-0.36.1/LICENSE` & `hezar-0.37.0/LICENSE`

 * *Files identical despite different names*

### Comparing `hezar-0.36.1/README.md` & `hezar-0.37.0/README.md`

 * *Files identical despite different names*

### Comparing `hezar-0.36.1/hezar/__init__.py` & `hezar-0.37.0/hezar/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,8 +8,8 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-__version__ = "0.36.1"
+__version__ = "0.37.0"
```

### Comparing `hezar-0.36.1/hezar/builders.py` & `hezar-0.37.0/hezar/builders.py`

 * *Files identical despite different names*

### Comparing `hezar-0.36.1/hezar/configs.py` & `hezar-0.37.0/hezar/configs.py`

 * *Files 2% similar despite different names*

```diff
@@ -392,27 +392,29 @@
         batch_size (int):
             Training batch size.
         eval_batch_size (int):
             Evaluation batch size, defaults to `batch_size` if None.
         gradient_accumulation_steps (int):
             Number of updates steps to accumulate before performing a backward/update pass, defaults to 1.
         distributed (bool):
-            Whether to use distributed training or not (via the `accelerate` package)
+            Whether to use distributed training (via the `accelerate` package)
         mixed_precision (PrecisionType | str):
             Mixed precision type e.g, fp16, bf16, etc. (disabled by default)
         evaluate_with_generate (bool):
             Whether to use `generate()` in the evaluation step or not. (only applicable for generative models).
         metrics (List[str | MetricConfig]):
             A list of metrics. Depending on the `valid_metrics` in the specific MetricsHandler of the Trainer.
         metric_for_best_model (str):
             Reference metric key to watch for determining the best model. Recommended to have a {train. | evaluation.}
             prefix (e.g, evaluation.f1, train.accuracy, etc.) but if not, defaults to
             `evaluation.{metric_for_best_model}`.
-        save_freq (int):
-            Save the trainer stats and everything every `save_freq` epochs.
+        save_freq (int) (DEPRECATED):
+            Deprecated and renamed to `save_steps`.
+        save_steps (int):
+            Save the trainer outputs every `save_steps` steps. Leave as `0` to ignore saving between training steps.
         checkpoints_dir (str):
             Path to the checkpoints' folder. The actual files will be saved under `{output_dir}/{checkpoints_dir}`.
         logs_dir (str):
             Path to the logs' folder. The actual log files will be saved under `{output_dir}/{logs_dir}`.
     """
 
     name: str = field(init=False, default="trainer")
@@ -430,35 +432,56 @@
     learning_rate: float = 2e-5
     weight_decay: float = 0.0
     lr_scheduler: str | LRSchedulerType = None
     lr_scheduler_kwargs: Dict[str, Any] = None
     batch_size: int = None
     eval_batch_size: int = None
     gradient_accumulation_steps: int = 1
-    distributed: bool = field(
-        init=False,
-        default=False,
-        metadata={"help": "Distributed training isn't supported yet! We're working hard to solve some bugs rn :("}
-    )
+    distributed: bool = False
     mixed_precision: PrecisionType | str | None = None
     use_cpu: bool = False
     evaluate_with_generate: bool = True
     metrics: List[str | MetricConfig] = None
     metric_for_best_model: str = "evaluation.loss"
-    save_freq: int = 1
+    save_enabled: bool = True
+    save_freq: int = None
+    save_steps: int = None
     checkpoints_dir: str = "checkpoints"
     logs_dir: str = "logs"
 
     def __post_init__(self):
         """
         Perform some argument sanitization and filtering here to avoid unexpected behavior in the trainer.
         The need for having this method is that some fields in the Trainer's config have correlations with each other
         and not controlling them can lead to conflicts.
         """
         super().__post_init__()
+        # Validate `task`
         if self.task not in list(TaskType):
             raise ValueError(
                 f"Invalid task `{self.task}` passed to `TrainerConfig`. "
                 f"Available options are {TaskType.list()}",
             )
+        # Validate `metric_for_best_model`
         if not (self.metric_for_best_model.startswith("evaluation") or self.metric_for_best_model.startswith("train")):
             self.metric_for_best_model = f"evaluation.{self.metric_for_best_model}"
+
+        # Validate steps
+        if self.save_steps is not None and self.save_steps % self.gradient_accumulation_steps != 0:
+            logger.warning(
+                f"It's recommended to set a `save_steps` dividable by `gradient_accumulation_steps`, "
+                f"otherwise, the saved model will have non-updated weights!\n"
+                f"`save_steps={self.save_steps}`, `gradient_accumulation_steps={self.gradient_accumulation_steps}`"
+            )
+
+        # Validate deprecated fields
+        if self.save_freq is not None:
+            logger.warning(
+                "Trainer argument `save_freq` is deprecated! Use `save_steps` (number of training steps per save)."
+                "Note that saving is also done at the end of each epoch unless you set `save_enabled` to `False` !"
+            )
+
+        # Distributed mode
+        if self.distributed:
+            logger.warning(
+                "Distributed mode is experimental and might have bugs. Use with caution and don't forget to submit your issues!"
+            )
```

### Comparing `hezar-0.36.1/hezar/constants.py` & `hezar-0.37.0/hezar/constants.py`

 * *Files identical despite different names*

### Comparing `hezar-0.36.1/hezar/data/data_collators.py` & `hezar-0.37.0/hezar/data/data_collators.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import numpy as np
 import torch
 
-from ..preprocessors import Tokenizer, AudioFeatureExtractor
+from ..preprocessors import AudioFeatureExtractor, Tokenizer
 from ..utils import Logger, convert_batch_dict_dtype
 
 
 __all__ = [
     "TextPaddingDataCollator",
     "TextGenerationDataCollator",
     "ImageCaptioningDataCollator",
@@ -225,17 +225,17 @@
 
 
 class SpeechRecognitionDataCollator:
     def __init__(
         self,
         feature_extractor: AudioFeatureExtractor,
         tokenizer: Tokenizer,
-        inputs_padding_type: str = None,
+        inputs_padding_type: str = "longest",
         inputs_max_length: int = None,
-        labels_padding_type: str = None,
+        labels_padding_type: str = "longest",
         labels_max_length: int = None,
     ):
         self.feature_extractor = feature_extractor
         self.tokenizer = tokenizer
         self.inputs_padding_type = inputs_padding_type
         self.inputs_max_length = inputs_max_length
         self.labels_padding_type = labels_padding_type
```

### Comparing `hezar-0.36.1/hezar/data/datasets/__init__.py` & `hezar-0.37.0/hezar/data/datasets/__init__.py`

 * *Files identical despite different names*

### Comparing `hezar-0.36.1/hezar/data/datasets/dataset.py` & `hezar-0.37.0/hezar/data/datasets/dataset.py`

 * *Files 11% similar despite different names*

```diff
@@ -70,39 +70,50 @@
         """
         raise NotImplementedError
 
     @classmethod
     def load(
         cls,
         hub_path: str | os.PathLike,
+        config: DatasetConfig = None,
         config_filename: Optional[str] = None,
         split: Optional[str | SplitType] = None,
         cache_dir: str = None,
         **kwargs,
     ) -> "Dataset":
         """
         Load the dataset from a hub path.
 
         Args:
-            hub_path (str | os.PathLike): Path to dataset from hub or locally.
-            config_filename (Optional[str]): Dataset config file name.
-            split (Optional[str | SplitType]): Dataset split, defaults to "train".
-            cache_dir (str): Path to cache directory
-            **kwargs: Config parameters as keyword arguments.
+            hub_path (str | os.PathLike):
+                Path to dataset from hub or locally.
+            config: (DatasetConfig):
+                A config object to ignore the config in the repo or in case the repo has no `dataset_config.yaml` file
+            config_filename (Optional[str]):
+                Dataset config file name. Falls back to `dataset_config.yaml` if not given.
+            split (Optional[str | SplitType]):
+                Dataset split, defaults to "train".
+            cache_dir (str):
+                Path to cache directory, defaults to Hezar's cache directory
+            **kwargs:
+                Config parameters as keyword arguments.
 
         Returns:
             Dataset: An instance of the loaded dataset.
 
         """
         split = split or "train"
         config_filename = config_filename or cls.config_filename
         if cache_dir is not None:
             cls.cache_dir = cache_dir
-        dataset_config = DatasetConfig.load(
-            hub_path,
-            filename=config_filename,
-            repo_type=RepoType.DATASET,
-            cache_dir=cls.cache_dir,
-        )
+        if config is not None:
+            dataset_config = config.update(kwargs)
+        else:
+            dataset_config = DatasetConfig.load(
+                hub_path,
+                filename=config_filename,
+                repo_type=RepoType.DATASET,
+                cache_dir=cls.cache_dir,
+            )
         dataset_config.path = hub_path
         dataset = build_dataset(dataset_config.name, config=dataset_config, split=split, **kwargs)
         return dataset
```

### Comparing `hezar-0.36.1/hezar/data/datasets/image_captioning_dataset.py` & `hezar-0.37.0/hezar/data/datasets/image_captioning_dataset.py`

 * *Files identical despite different names*

### Comparing `hezar-0.36.1/hezar/data/datasets/ocr_dataset.py` & `hezar-0.37.0/hezar/data/datasets/ocr_dataset.py`

 * *Files identical despite different names*

### Comparing `hezar-0.36.1/hezar/data/datasets/sequence_labeling_dataset.py` & `hezar-0.37.0/hezar/data/datasets/sequence_labeling_dataset.py`

 * *Files identical despite different names*

### Comparing `hezar-0.36.1/hezar/data/datasets/speech_recognition_dataset.py` & `hezar-0.37.0/hezar/data/datasets/speech_recognition_dataset.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,34 +1,35 @@
 from __future__ import annotations
 
 from dataclasses import dataclass
 
 from datasets import Audio, load_dataset
 
-from .dataset import Dataset
-from ..data_collators import SpeechRecognitionDataCollator
 from ...configs import DatasetConfig
-from ...constants import TaskType, Backends, PaddingType
-from ...preprocessors import Tokenizer, AudioFeatureExtractor
+from ...constants import Backends, PaddingType, TaskType
+from ...preprocessors import AudioFeatureExtractor, Tokenizer
 from ...registry import register_dataset
+from ..data_collators import SpeechRecognitionDataCollator
+from .dataset import Dataset
+
 
 _required_backends = [Backends.LIBROSA, Backends.DATASETS]
 
 
 @dataclass
 class SpeechRecognitionDatasetConfig(DatasetConfig):
     name = "speech_recognition"
     task = TaskType.SPEECH_RECOGNITION
     path: str = None
     feature_extractor_path: str = None
     tokenizer_path: str = None
     sampling_rate: int = 16000
-    audio_array_padding_type: bool | str | PaddingType = None
+    audio_array_padding_type: bool | str | PaddingType = "longest"
     max_audio_array_length: int = None
-    labels_padding_type: bool | str | PaddingType = None
+    labels_padding_type: bool | str | PaddingType = "longest"
     labels_max_length: int = None
     audio_file_path_column: str = "path"
     audio_column: str = "audio"
     audio_array_column: str = "array"
     transcript_column: str = "sentence"
 
 
@@ -40,17 +41,17 @@
         super().__init__(config, split, **kwargs)
         self.data = self._load(split)
         self.feature_extractor = AudioFeatureExtractor.load(self.config.feature_extractor_path)
         self.tokenizer = Tokenizer.load(self.config.tokenizer_path)
         self.data_collator = SpeechRecognitionDataCollator(
             self.feature_extractor,
             self.tokenizer,
-            inputs_padding_type="max_length" if self.config.max_audio_array_length is not None else "longest",
+            inputs_padding_type=self.config.audio_array_padding_type,
             inputs_max_length=self.config.max_audio_array_length,
-            labels_padding_type="max_length" if self.config.labels_max_length is not None else "longest",
+            labels_padding_type=self.config.labels_padding_type,
             labels_max_length=self.config.labels_max_length,
         )
 
     def _load(self, split):
         data = load_dataset(self.config.path, split=split, cache_dir=self.cache_dir)
         data = data.cast_column(self.config.audio_column, Audio(sampling_rate=self.config.sampling_rate))
         return data
@@ -67,15 +68,17 @@
             audio_array,
             sampling_rate=self.config.sampling_rate,
             return_tensors="pt"
         )["input_features"]
 
         labels = self.tokenizer(
             transcript,
+            padding_strategy=self.config.labels_padding_type,
             max_length=self.config.labels_max_length,
-            return_tensors="pt"
-        )["token_ids"]
+            return_tensors="pt",
+        )
 
         return {
             "input_features": input_features,
-            "labels": labels
+            "labels": labels["token_ids"],
+            "attention_mask": labels["attention_mask"],
         }
```

### Comparing `hezar-0.36.1/hezar/data/datasets/text_classification_dataset.py` & `hezar-0.37.0/hezar/data/datasets/text_classification_dataset.py`

 * *Files identical despite different names*

### Comparing `hezar-0.36.1/hezar/data/datasets/text_summarization_dataset.py` & `hezar-0.37.0/hezar/data/datasets/text_summarization_dataset.py`

 * *Files identical despite different names*

### Comparing `hezar-0.36.1/hezar/embeddings/embedding.py` & `hezar-0.37.0/hezar/embeddings/embedding.py`

 * *Files identical despite different names*

### Comparing `hezar-0.36.1/hezar/embeddings/fasttext.py` & `hezar-0.37.0/hezar/embeddings/fasttext.py`

 * *Files identical despite different names*

### Comparing `hezar-0.36.1/hezar/embeddings/word2vec.py` & `hezar-0.37.0/hezar/embeddings/word2vec.py`

 * *Files identical despite different names*

### Comparing `hezar-0.36.1/hezar/metrics/accuracy.py` & `hezar-0.37.0/hezar/metrics/accuracy.py`

 * *Files identical despite different names*

### Comparing `hezar-0.36.1/hezar/metrics/bleu.py` & `hezar-0.37.0/hezar/metrics/bleu.py`

 * *Files identical despite different names*

### Comparing `hezar-0.36.1/hezar/metrics/cer.py` & `hezar-0.37.0/hezar/metrics/cer.py`

 * *Files identical despite different names*

### Comparing `hezar-0.36.1/hezar/metrics/f1.py` & `hezar-0.37.0/hezar/metrics/f1.py`

 * *Files identical despite different names*

### Comparing `hezar-0.36.1/hezar/metrics/metric.py` & `hezar-0.37.0/hezar/metrics/metric.py`

 * *Files identical despite different names*

### Comparing `hezar-0.36.1/hezar/metrics/precision.py` & `hezar-0.37.0/hezar/metrics/precision.py`

 * *Files identical despite different names*

### Comparing `hezar-0.36.1/hezar/metrics/recall.py` & `hezar-0.37.0/hezar/metrics/recall.py`

 * *Files identical despite different names*

### Comparing `hezar-0.36.1/hezar/metrics/rouge.py` & `hezar-0.37.0/hezar/metrics/rouge.py`

 * *Files identical despite different names*

### Comparing `hezar-0.36.1/hezar/metrics/seqeval.py` & `hezar-0.37.0/hezar/metrics/seqeval.py`

 * *Files identical despite different names*

### Comparing `hezar-0.36.1/hezar/metrics/wer.py` & `hezar-0.37.0/hezar/metrics/wer.py`

 * *Files identical despite different names*

### Comparing `hezar-0.36.1/hezar/models/backbone/bert/bert.py` & `hezar-0.37.0/hezar/models/backbone/bert/bert.py`

 * *Files identical despite different names*

### Comparing `hezar-0.36.1/hezar/models/backbone/bert/bert_config.py` & `hezar-0.37.0/hezar/models/backbone/bert/bert_config.py`

 * *Files identical despite different names*

### Comparing `hezar-0.36.1/hezar/models/backbone/distilbert/distilbert.py` & `hezar-0.37.0/hezar/models/backbone/distilbert/distilbert.py`

 * *Files identical despite different names*

### Comparing `hezar-0.36.1/hezar/models/backbone/distilbert/distilbert_config.py` & `hezar-0.37.0/hezar/models/backbone/distilbert/distilbert_config.py`

 * *Files identical despite different names*

### Comparing `hezar-0.36.1/hezar/models/backbone/roberta/roberta.py` & `hezar-0.37.0/hezar/models/backbone/roberta/roberta.py`

 * *Files identical despite different names*

### Comparing `hezar-0.36.1/hezar/models/backbone/roberta/roberta_config.py` & `hezar-0.37.0/hezar/models/backbone/roberta/roberta_config.py`

 * *Files identical despite different names*

### Comparing `hezar-0.36.1/hezar/models/backbone/vit/vit.py` & `hezar-0.37.0/hezar/models/backbone/vit/vit.py`

 * *Files identical despite different names*

### Comparing `hezar-0.36.1/hezar/models/backbone/vit/vit_config.py` & `hezar-0.37.0/hezar/models/backbone/vit/vit_config.py`

 * *Files identical despite different names*

### Comparing `hezar-0.36.1/hezar/models/image2text/beit_roberta/beit_roberta_image2text.py` & `hezar-0.37.0/hezar/models/image2text/beit_roberta/beit_roberta_image2text.py`

 * *Files identical despite different names*

### Comparing `hezar-0.36.1/hezar/models/image2text/beit_roberta/beit_roberta_image2text_config.py` & `hezar-0.37.0/hezar/models/image2text/beit_roberta/beit_roberta_image2text_config.py`

 * *Files identical despite different names*

### Comparing `hezar-0.36.1/hezar/models/image2text/crnn/crnn_decode_utils.py` & `hezar-0.37.0/hezar/models/image2text/crnn/crnn_decode_utils.py`

 * *Files identical despite different names*

### Comparing `hezar-0.36.1/hezar/models/image2text/crnn/crnn_image2text.py` & `hezar-0.37.0/hezar/models/image2text/crnn/crnn_image2text.py`

 * *Files identical despite different names*

### Comparing `hezar-0.36.1/hezar/models/image2text/trocr/trocr_image2text.py` & `hezar-0.37.0/hezar/models/image2text/trocr/trocr_image2text.py`

 * *Files identical despite different names*

### Comparing `hezar-0.36.1/hezar/models/image2text/trocr/trocr_image2text_config.py` & `hezar-0.37.0/hezar/models/image2text/trocr/trocr_image2text_config.py`

 * *Files identical despite different names*

### Comparing `hezar-0.36.1/hezar/models/image2text/vit_gpt2/vit_gpt2_image2text.py` & `hezar-0.37.0/hezar/models/image2text/vit_gpt2/vit_gpt2_image2text.py`

 * *Files identical despite different names*

### Comparing `hezar-0.36.1/hezar/models/image2text/vit_gpt2/vit_gpt2_image2text_config.py` & `hezar-0.37.0/hezar/models/image2text/vit_gpt2/vit_gpt2_image2text_config.py`

 * *Files identical despite different names*

### Comparing `hezar-0.36.1/hezar/models/image2text/vit_roberta/vit_roberta_image2text.py` & `hezar-0.37.0/hezar/models/image2text/vit_roberta/vit_roberta_image2text.py`

 * *Files identical despite different names*

### Comparing `hezar-0.36.1/hezar/models/image2text/vit_roberta/vit_roberta_image2text_config.py` & `hezar-0.37.0/hezar/models/image2text/vit_roberta/vit_roberta_image2text_config.py`

 * *Files identical despite different names*

### Comparing `hezar-0.36.1/hezar/models/mask_filling/bert/bert_mask_filling.py` & `hezar-0.37.0/hezar/models/mask_filling/bert/bert_mask_filling.py`

 * *Files identical despite different names*

### Comparing `hezar-0.36.1/hezar/models/mask_filling/bert/bert_mask_filling_config.py` & `hezar-0.37.0/hezar/models/mask_filling/bert/bert_mask_filling_config.py`

 * *Files identical despite different names*

### Comparing `hezar-0.36.1/hezar/models/mask_filling/distilbert/distilbert_mask_filling.py` & `hezar-0.37.0/hezar/models/mask_filling/distilbert/distilbert_mask_filling.py`

 * *Files identical despite different names*

### Comparing `hezar-0.36.1/hezar/models/mask_filling/distilbert/distilbert_mask_filling_config.py` & `hezar-0.37.0/hezar/models/mask_filling/distilbert/distilbert_mask_filling_config.py`

 * *Files identical despite different names*

### Comparing `hezar-0.36.1/hezar/models/mask_filling/roberta/roberta_mask_filling.py` & `hezar-0.37.0/hezar/models/mask_filling/roberta/roberta_mask_filling.py`

 * *Files identical despite different names*

### Comparing `hezar-0.36.1/hezar/models/mask_filling/roberta/roberta_mask_filling_config.py` & `hezar-0.37.0/hezar/models/mask_filling/roberta/roberta_mask_filling_config.py`

 * *Files identical despite different names*

### Comparing `hezar-0.36.1/hezar/models/model.py` & `hezar-0.37.0/hezar/models/model.py`

 * *Files identical despite different names*

### Comparing `hezar-0.36.1/hezar/models/model_outputs.py` & `hezar-0.37.0/hezar/models/model_outputs.py`

 * *Files identical despite different names*

### Comparing `hezar-0.36.1/hezar/models/sequence_labeling/bert/bert_sequence_labeling.py` & `hezar-0.37.0/hezar/models/sequence_labeling/bert/bert_sequence_labeling.py`

 * *Files identical despite different names*

### Comparing `hezar-0.36.1/hezar/models/sequence_labeling/bert/bert_sequence_labeling_config.py` & `hezar-0.37.0/hezar/models/sequence_labeling/bert/bert_sequence_labeling_config.py`

 * *Files identical despite different names*

### Comparing `hezar-0.36.1/hezar/models/sequence_labeling/distilbert/distilbert_sequence_labeling.py` & `hezar-0.37.0/hezar/models/sequence_labeling/distilbert/distilbert_sequence_labeling.py`

 * *Files identical despite different names*

### Comparing `hezar-0.36.1/hezar/models/sequence_labeling/distilbert/distilbert_sequence_labeling_config.py` & `hezar-0.37.0/hezar/models/sequence_labeling/distilbert/distilbert_sequence_labeling_config.py`

 * *Files identical despite different names*

### Comparing `hezar-0.36.1/hezar/models/sequence_labeling/roberta/roberta_sequence_labeling.py` & `hezar-0.37.0/hezar/models/sequence_labeling/roberta/roberta_sequence_labeling.py`

 * *Files identical despite different names*

### Comparing `hezar-0.36.1/hezar/models/sequence_labeling/roberta/roberta_sequence_labeling_config.py` & `hezar-0.37.0/hezar/models/sequence_labeling/roberta/roberta_sequence_labeling_config.py`

 * *Files identical despite different names*

### Comparing `hezar-0.36.1/hezar/models/speech_recognition/whisper/whisper_feature_extractor.py` & `hezar-0.37.0/hezar/models/speech_recognition/whisper/whisper_feature_extractor.py`

 * *Files identical despite different names*

### Comparing `hezar-0.36.1/hezar/models/speech_recognition/whisper/whisper_speech_recognition.py` & `hezar-0.37.0/hezar/models/speech_recognition/whisper/whisper_speech_recognition.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,26 +1,25 @@
 from __future__ import annotations
 
 import copy
 from typing import List
 
+import librosa
 import numpy as np
 import torch
 
 from ....constants import Backends
 from ....registry import register_model
 from ....utils import is_backend_available, load_audio_files, shift_tokens_right
 from ...model import Model
 from ...model_outputs import SpeechRecognitionOutput
 from .whisper_speech_recognition_config import WhisperSpeechRecognitionConfig
 
-
 if is_backend_available(Backends.TRANSFORMERS):
-    from transformers import WhisperConfig, WhisperForConditionalGeneration
-
+    from transformers import WhisperConfig, WhisperForConditionalGeneration, GenerationConfig
 
 _required_backends = [
     Backends.TRANSFORMERS,
     Backends.TOKENIZERS,
     Backends.LIBROSA,
 ]
 
@@ -77,17 +76,18 @@
             use_cache=use_cache,
             output_attentions=output_attentions,
             output_hidden_states=output_hidden_states,
         )
 
         return dict(outputs)
 
-    def compute_loss(self, logits: torch.Tensor, labels: torch.Tensor) -> torch.Tensor:
+    def compute_loss(self, logits: torch.Tensor, labels: torch.Tensor, attention_mask: torch.Tensor = None):
         labels = copy.deepcopy(labels)
-        labels[labels == self.config.pad_token_id] = -100
+        if attention_mask is not None:
+            labels = labels.masked_fill(attention_mask.ne(1), -100)
         loss = self.loss_func(logits.view(-1, self.config.vocab_size), labels.view(-1))
         return loss
 
     def generate(
         self,
         input_features,
         forced_decoder_ids=None,
@@ -99,14 +99,19 @@
         return_timestamps=None,
         task=None,
         language=None,
         is_multilingual=None,
         prompt_ids=None,
         **kwargs,
     ):
+        if generation_config is not None:
+            self.config.generation_config.update(**generation_config)
+
+        generation_config = GenerationConfig(**self.config.generation_config)
+
         generation_outputs = self.whisper.generate(
             input_features=input_features,
             generation_config=generation_config,
             logits_processor=logits_processor,
             stopping_criteria=stopping_criteria,
             prefix_allowed_tokens_fn=prefix_allowed_tokens_fn,
             synced_gpus=synced_gpus,
@@ -159,21 +164,37 @@
 
     def freeze_encoder(self):
         self.whisper.freeze_encoder()
 
     def preprocess(self, inputs: str | np.ndarray | List[np.ndarray] | List[str], **kwargs):
         if isinstance(inputs, str) or (isinstance(inputs, List) and isinstance(inputs[0], str)):
             inputs = load_audio_files(inputs)
+        elif isinstance(inputs, List) and isinstance(inputs[0], np.ndarray):
+            inputs = [librosa.to_mono(x.transpose()) for x in inputs if isinstance(x, np.ndarray) and len(x.shape) > 1]
 
         tokenizer = self.preprocessor[self.tokenizer_name]
         feature_extractor = self.preprocessor[self.feature_extractor_name]
 
         forced_decoder_ids = tokenizer.get_decoder_prompt_ids(language="persian", task="transcribe")
         inputs = feature_extractor(inputs, sampling_rate=self.config.sampling_rate, return_tensors="pt")
         inputs["forced_decoder_ids"] = forced_decoder_ids
         return inputs
 
-    def post_process(self, model_outputs, **kwargs):
+    def post_process(
+        self,
+        model_outputs,
+        skip_special_tokens=True,
+        decode_with_timestamps=True,
+        output_offsets=False,
+        **kwargs,
+    ):
         tokenizer = self.preprocessor[self.tokenizer_name]
-        transcripts = tokenizer.decode(model_outputs, decode_with_timestamps=True, skip_special_tokens=True)
+        if isinstance(model_outputs, torch.Tensor):
+            model_outputs = model_outputs.cpu().numpy().tolist()
+        transcripts = tokenizer.decode(
+            model_outputs,
+            decode_with_timestamps=decode_with_timestamps,
+            skip_special_tokens=skip_special_tokens,
+            output_offsets=output_offsets,
+        )
         outputs = [SpeechRecognitionOutput(text=transcript) for transcript in transcripts]
         return outputs
```

### Comparing `hezar-0.36.1/hezar/models/speech_recognition/whisper/whisper_speech_recognition_config.py` & `hezar-0.37.0/hezar/models/text_generation/gpt2/gpt2_text_generation_config.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,49 +1,42 @@
 from dataclasses import dataclass, field
-from typing import List
 
 from ....configs import ModelConfig
 
 
 @dataclass
-class WhisperSpeechRecognitionConfig(ModelConfig):
-    name = "whisper_speech_recognition"
-    vocab_size: int = 51865
-    num_mel_bins: int = 80
-    encoder_layers: int = 6
-    encoder_attention_heads: int = 4
-    decoder_layers: int = 6
-    decoder_attention_heads: int = 4
-    num_hidden_layers: int = 12
-    decoder_ffn_dim: int = 1536
-    encoder_ffn_dim: int = 1536
-    encoder_layerdrop: float = 0.0
-    decoder_layerdrop: float = 0.0
-    decoder_start_token_id: int = 50257
+class GenerationConfig(ModelConfig):
+    bos_token_id: int = 0
+    decoder_start_token_id: int = 0
+    early_stopping: bool = True
+    eos_token_id: int = 2
+    length_penalty: float = 2.0
+    max_new_tokens: int = 50
+    no_repeat_ngram_size: int = 3
+    num_beams: int = 4
+    pad_token_id: int = 1
+
+
+@dataclass
+class GPT2TextGenerationConfig(ModelConfig):
+    name = "gpt2_text_generation"
+    add_cross_attention: bool = False
+    vocab_size: int = 42001
+    attn_pdrop: float = 0.1
+    bos_token_id: int = 5
+    embd_pdrop: float = 0.1
+    eos_token_id: int = 5
+    gradient_checkpointing: bool = False
+    initializer_range: float = 0.02
+    layer_norm_epsilon: float = 1e-05
+    model_type: str = "gpt2"
+    n_ctx: int = 1024
+    n_embd: int = 768
+    n_head: int = 12
+    n_inner: int = None
+    n_layer: int = 12
+    n_positions: int = 1024
+    resid_pdrop: float = 0.1
+    summary_activation: bool = False
+    summary_first_dropout: float = 0.1
     use_cache: bool = True
-    sampling_rate: int = 16000
-    is_encoder_decoder: bool = True
-    activation_function: str = "gelu"
-    d_model: int = 256
-    dropout: float = 0.0
-    torch_dtype: str = "float32"
-    attention_dropout: float = 0.0
-    activation_dropout: float = 0.0
-    init_std: float = 0.02
-    scale_embedding: bool = False
-    max_source_positions: int = 1500
-    max_target_positions: int = 448
-    pad_token_id: int = 50256
-    bos_token_id: int = 50257
-    eos_token_id: int = 50256
-    suppress_tokens: List[int] = None
-    begin_suppress_tokens: List[int] = field(default_factory=lambda: [220, 50256])
-    use_weighted_layer_sum: bool = False
-    classifier_proj_size: int = 256
-    apply_spec_augment: bool = False
-    mask_time_prob: float = 0.05
-    mask_time_length: int = 10
-    mask_time_min_masks: int = 2
-    mask_feature_prob: float = 0.0
-    mask_feature_length: int = 10
-    mask_feature_min_masks: int = 0
-    max_new_tokens: int = 448
+    generation: GenerationConfig = field(default_factory=GenerationConfig)
```

### Comparing `hezar-0.36.1/hezar/models/speech_recognition/whisper/whisper_tokenizer.py` & `hezar-0.37.0/hezar/models/speech_recognition/whisper/whisper_tokenizer.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+import re
 from dataclasses import dataclass, field
 from typing import List
 
 import numpy as np
 
 from ....constants import Backends
 from ....preprocessors import BPEConfig, BPETokenizer
@@ -295,45 +296,59 @@
         time_precision=0.02,
         decode_with_timestamps: bool = False,
         **kwargs,
     ):
         """
         Override decode method to enable timestamps and offsets.
         """
-        text = super().decode(token_ids, skip_special_tokens=skip_special_tokens, **kwargs)
+        filtered_ids = self._preprocess_token_ids(token_ids, skip_special_tokens=skip_special_tokens)
+        text = super().decode(filtered_ids, skip_special_tokens=skip_special_tokens, **kwargs)
         if decode_with_timestamps:
             text = [
                 self._decode_with_timestamps(
-                    token_id,
+                    ids,
                     time_precision=time_precision,
                     skip_special_tokens=skip_special_tokens,
                 )
-                for token_id in token_ids
+                for ids in filtered_ids
             ]
+        else:
+            text = [re.sub(re.compile(r"<\|(\d+\.\d+)\|>"), "", t) for t in text]
         # retrieve offsets
         if output_offsets:
             offsets = self._compute_offsets(token_ids, time_precision=time_precision)
             return {"text": text, "offsets": offsets}
         return text
 
     def _decode_with_timestamps(self, token_ids, skip_special_tokens=False, time_precision=0.02) -> str:
         """
         Timestamp tokens are above the special tokens' id range and are ignored by `decode()`. This method decodes
         given tokens with timestamps tokens annotated, e.g. "<|1.08|>".
         """
-        timestamp_begin = self.token_to_id(self.config.notimestamps_token) + 1
+        timestamp_begin = self.special_ids[-1] + 1
         outputs = [[]]
+
+        cur_max_timestamp = 0.0
+        prev_segments_len = 0.0
+
         for token in token_ids:
             if token >= timestamp_begin:
-                timestamp = f"<|{(token - timestamp_begin) * time_precision:.2f}|>"
-                outputs.append(timestamp)
+                timestamp = float((token - timestamp_begin) * time_precision)
+
+                if timestamp < cur_max_timestamp:
+                    # next segment has started
+                    prev_segments_len += cur_max_timestamp
+
+                cur_max_timestamp = timestamp
+
+                outputs.append(f"<|{(timestamp + prev_segments_len):.2f}|>")
                 outputs.append([])
             else:
                 outputs[-1].append(token)
-        outputs = self.decode(outputs, skip_special_tokens=skip_special_tokens)
+        outputs = [s if isinstance(s, str) else self.decode(s, skip_special_tokens=skip_special_tokens)[0] for s in outputs]  # noqa
         return "".join(outputs)
 
     def _compute_offsets(self, token_ids, time_precision=0.02):
         """
         Compute offsets for a given tokenized input
 
         Args:
@@ -372,14 +387,31 @@
                         ),
                     }
                 )
             last_slice = current_slice
 
         return offsets
 
+    def _preprocess_token_ids(self, token_ids, skip_special_tokens: bool = False):
+        """
+        Pre-process the token ids for decoding by removing the prompt tokens ids and timestamp token ids.
+
+        Args:
+            token_ids (`Union[int, List[int], np.ndarray, torch.Tensor, tf.Tensor]`):
+                List of tokenized input ids. Typically, obtained using the `__call__` method of the tokenizer.
+            skip_special_tokens (`bool`, *optional*, defaults to `False`):
+                Whether to remove special tokens from the token ids. If `True`, the prompt token ids will be removed.
+        """
+        if skip_special_tokens:
+            prompt_token_id = self.convert_tokens_to_ids("<|startofprev|>")
+            decoder_start_token_id = self.convert_tokens_to_ids("<|startoftranscript|>")
+            token_ids = self._strip_prompt(token_ids, prompt_token_id, decoder_start_token_id)
+
+        return token_ids
+
     def get_prompt_ids(self, text: str, return_tensors="np"):
         """Converts prompt text to IDs that can be passed to [`~WhisperForConditionalGeneration.generate`]."""
         batch_encoding = self([("<|startofprev|>", " " + text.strip())], add_special_tokens=False)
 
         # Check for special tokens
         prompt_text_ids = batch_encoding["input_ids"][1:]
         special_token_id = next((x for x in prompt_text_ids if x >= self.special_ids[0]), None)
```

### Comparing `hezar-0.36.1/hezar/models/text_classification/bert/bert_text_classification.py` & `hezar-0.37.0/hezar/models/text_classification/bert/bert_text_classification.py`

 * *Files identical despite different names*

### Comparing `hezar-0.36.1/hezar/models/text_classification/bert/bert_text_classification_config.py` & `hezar-0.37.0/hezar/models/text_classification/bert/bert_text_classification_config.py`

 * *Files identical despite different names*

### Comparing `hezar-0.36.1/hezar/models/text_classification/distilbert/distilbert_text_classification.py` & `hezar-0.37.0/hezar/models/text_classification/distilbert/distilbert_text_classification.py`

 * *Files identical despite different names*

### Comparing `hezar-0.36.1/hezar/models/text_classification/distilbert/distilbert_text_classification_config.py` & `hezar-0.37.0/hezar/models/text_classification/distilbert/distilbert_text_classification_config.py`

 * *Files identical despite different names*

### Comparing `hezar-0.36.1/hezar/models/text_classification/roberta/roberta_text_classification.py` & `hezar-0.37.0/hezar/models/text_classification/roberta/roberta_text_classification.py`

 * *Files identical despite different names*

### Comparing `hezar-0.36.1/hezar/models/text_classification/roberta/roberta_text_classification_config.py` & `hezar-0.37.0/hezar/models/text_classification/roberta/roberta_text_classification_config.py`

 * *Files identical despite different names*

### Comparing `hezar-0.36.1/hezar/models/text_generation/gpt2/gpt2_text_generation.py` & `hezar-0.37.0/hezar/models/text_generation/gpt2/gpt2_text_generation.py`

 * *Files identical despite different names*

### Comparing `hezar-0.36.1/hezar/models/text_generation/t5/t5_text_generation.py` & `hezar-0.37.0/hezar/models/text_generation/t5/t5_text_generation.py`

 * *Files identical despite different names*

### Comparing `hezar-0.36.1/hezar/models/text_generation/t5/t5_text_generation_config.py` & `hezar-0.37.0/hezar/models/text_generation/t5/t5_text_generation_config.py`

 * *Files identical despite different names*

### Comparing `hezar-0.36.1/hezar/preprocessors/audio_feature_extractor.py` & `hezar-0.37.0/hezar/preprocessors/audio_feature_extractor.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from __future__ import annotations
 
 from dataclasses import dataclass
-from typing import List, Mapping
+from typing import Mapping
 
 import numpy as np
 
 from ..builders import build_preprocessor
 from ..configs import PreprocessorConfig
 from ..constants import DEFAULT_FEATURE_EXTRACTOR_CONFIG_FILE, PaddingType
 from ..utils import convert_batch_dict_dtype
```

### Comparing `hezar-0.36.1/hezar/preprocessors/image_processor.py` & `hezar-0.37.0/hezar/preprocessors/image_processor.py`

 * *Files identical despite different names*

### Comparing `hezar-0.36.1/hezar/preprocessors/preprocessor.py` & `hezar-0.37.0/hezar/preprocessors/preprocessor.py`

 * *Files identical despite different names*

### Comparing `hezar-0.36.1/hezar/preprocessors/text_normalizer.py` & `hezar-0.37.0/hezar/preprocessors/text_normalizer.py`

 * *Files identical despite different names*

### Comparing `hezar-0.36.1/hezar/preprocessors/tokenizers/bpe.py` & `hezar-0.37.0/hezar/preprocessors/tokenizers/bpe.py`

 * *Files identical despite different names*

### Comparing `hezar-0.36.1/hezar/preprocessors/tokenizers/sentencepiece_bpe.py` & `hezar-0.37.0/hezar/preprocessors/tokenizers/sentencepiece_bpe.py`

 * *Files identical despite different names*

### Comparing `hezar-0.36.1/hezar/preprocessors/tokenizers/sentencepiece_unigram.py` & `hezar-0.37.0/hezar/preprocessors/tokenizers/sentencepiece_unigram.py`

 * *Files identical despite different names*

### Comparing `hezar-0.36.1/hezar/preprocessors/tokenizers/tokenizer.py` & `hezar-0.37.0/hezar/preprocessors/tokenizers/tokenizer.py`

 * *Files identical despite different names*

### Comparing `hezar-0.36.1/hezar/preprocessors/tokenizers/wordpiece.py` & `hezar-0.37.0/hezar/preprocessors/tokenizers/wordpiece.py`

 * *Files identical despite different names*

### Comparing `hezar-0.36.1/hezar/registry.py` & `hezar-0.37.0/hezar/registry.py`

 * *Files identical despite different names*

### Comparing `hezar-0.36.1/hezar/trainer/metrics_handlers.py` & `hezar-0.37.0/hezar/trainer/metrics_handlers.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 from __future__ import annotations
 
 from typing import List
 
 import numpy as np
-import torch
 
 from ..builders import build_metric
 from ..configs import MetricConfig
 from ..constants import MetricType
 from ..metrics import Metric
 from .trainer_utils import MetricsTracker
 
@@ -37,28 +36,39 @@
     def __init__(self, metrics: List[str | MetricType | Metric | MetricConfig], trainer=None, **kwargs):
         self.metrics = self._setup_metrics(metrics)
         self.trainer = trainer
         self.tracker = MetricsTracker(self.metrics)
         self.objective = self._configure_objective()
 
     def _configure_objective(self):
+        """
+        Figure out if the objective of the metric is to `minimize` or `maximize`
+        """
         target_metric = self.trainer.config.metric_for_best_model
         objective_metric = target_metric.split(".")[1] if "." in target_metric else target_metric
         if "loss" in objective_metric:
             objective = "minimize"
         else:
             if objective_metric not in self.metrics:
                 raise ValueError(
                     f"{objective_metric} is not a valid metric for this task, "
                     f"available metrics: {list(self.tracker.trackers.values())}"
                 )
             objective = self.metrics[objective_metric].config.objective
         return objective
 
     def _setup_metrics(self, metrics):
+        """
+        Prepare a dictionary of metric names and their instances mappings.
+        Args:
+            metrics: A list of either names, configs or metric instances. Defaults to `self.valid_metrics`.
+
+        Returns:
+
+        """
         metrics_dict = {}
         metrics = metrics or []
         if not len(metrics):
             return metrics_dict
         for metric in metrics:
             if isinstance(metric, str):
                 if metric not in self.valid_metrics:
@@ -132,16 +142,16 @@
 class Image2TextMetricHandler(MetricsHandler):
     valid_metrics = [MetricType.CER, MetricType.WER]
 
     def __init__(self, metrics: List[str | MetricType | Metric | MetricConfig], trainer=None):
         super().__init__(metrics=metrics, trainer=trainer)
 
     def compute_metrics(self, predictions, labels, **kwargs):
-        predictions = self.trainer.model.post_process(torch.tensor(predictions))
-        labels = self.trainer.model.post_process(torch.tensor(labels))
+        predictions = self.trainer.model.post_process(predictions)
+        labels = self.trainer.model.post_process(labels)
         predictions = [x["text"] for x in predictions]
         labels = [x["text"] for x in labels]
         results = {}
         for metric_name, metric in self.metrics.items():
             x = metric.compute(predictions, labels)
             results.update(x)
         return results
@@ -150,16 +160,16 @@
 class SpeechRecognitionMetricsHandler(MetricsHandler):
     valid_metrics = [MetricType.CER, MetricType.WER]
 
     def __init__(self, metrics: List[str | MetricType | Metric | MetricConfig], trainer=None):
         super().__init__(metrics=metrics, trainer=trainer)
 
     def compute_metrics(self, predictions, labels, **kwargs):
-        predictions = self.trainer.model.post_process(torch.tensor(predictions))
-        labels = self.trainer.model.post_process(torch.tensor(labels))
+        predictions = self.trainer.model.post_process(predictions)
+        labels = self.trainer.model.post_process(labels)
         predictions = [x["text"] for x in predictions]
         labels = [x["text"] for x in labels]
         results = {}
         for metric_name, metric in self.metrics.items():
             x = metric.compute(predictions, labels)
             results.update(x)
         return results
@@ -168,16 +178,16 @@
 class TextGenerationMetricsHandler(MetricsHandler):
     valid_metrics = [MetricType.ROUGE, MetricType.BLEU]
 
     def __init__(self, metrics: List[str | MetricType | Metric | MetricConfig], trainer=None):
         super().__init__(metrics=metrics, trainer=trainer)
 
     def compute_metrics(self, predictions, labels, **kwargs):
-        predictions = self.trainer.model.post_process(torch.tensor(predictions))
-        labels = self.trainer.model.post_process(torch.tensor(labels))
+        predictions = self.trainer.model.post_process(predictions)
+        labels = self.trainer.model.post_process(labels)
         predictions = [x["text"] for x in predictions]
         labels = [x["text"] for x in labels]
         results = {}
         for metric_name, metric in self.metrics.items():
             x = metric.compute(predictions, labels)
             results.update(x)
         return results
```

### Comparing `hezar-0.36.1/hezar/trainer/trainer.py` & `hezar-0.37.0/hezar/trainer/trainer.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,30 +1,22 @@
 from __future__ import annotations
 
+import math
 import os
 import random
-from typing import TYPE_CHECKING, Any, Callable, Dict, Tuple
+from typing import Any, Callable, Dict, Tuple
 
 import numpy as np
 import pandas as pd
 import torch
 from huggingface_hub import create_repo, hf_hub_download, upload_file
 from torch.utils.data import DataLoader
 from torch.utils.tensorboard import SummaryWriter
-from tqdm import tqdm
+from tqdm.auto import tqdm
 
-from .metrics_handlers import (
-    Image2TextMetricHandler,
-    MetricsHandler,
-    SequenceLabelingMetricsHandler,
-    SpeechRecognitionMetricsHandler,
-    TextClassificationMetricsHandler,
-    TextGenerationMetricsHandler,
-)
-from .trainer_utils import CSVLogger, TrainerState, resolve_logdir, write_to_tensorboard
 from ..configs import TrainerConfig
 from ..constants import (
     DEFAULT_DATASET_CONFIG_FILE,
     DEFAULT_TRAINER_CONFIG_FILE,
     DEFAULT_TRAINER_CSV_LOG_FILE,
     DEFAULT_TRAINER_STATE_FILE,
     DEFAULT_TRAINER_SUBFOLDER,
@@ -34,18 +26,37 @@
     LRSchedulerType,
     OptimizerType,
     TaskType,
 )
 from ..data.datasets import Dataset
 from ..models import Model
 from ..preprocessors import Preprocessor, PreprocessorsContainer
-from ..utils import Logger, colorize_text, is_backend_available, sanitize_function_parameters, verify_dependencies
+from ..utils import (
+    Logger,
+    colorize_text,
+    is_backend_available,
+    sanitize_function_parameters,
+    verify_dependencies,
+    set_seed,
+)
+from .metrics_handlers import (
+    Image2TextMetricHandler,
+    MetricsHandler,
+    SequenceLabelingMetricsHandler,
+    SpeechRecognitionMetricsHandler,
+    TextClassificationMetricsHandler,
+    TextGenerationMetricsHandler,
+)
+from .trainer_utils import CSVLogger, TrainerState, get_distributed_logger, resolve_logdir, write_to_tensorboard
+
 
-if TYPE_CHECKING:
+if is_backend_available(Backends.ACCELERATE):
     from accelerate import Accelerator
+else:
+    raise ImportError("The package `accelerate` needs to be installed to use `Trainer`!")
 
 logger = Logger(__name__)
 
 optimizers = {
     OptimizerType.ADAM: torch.optim.Adam,
     OptimizerType.ADAMW: torch.optim.AdamW,
     OptimizerType.SDG: torch.optim.SGD,
@@ -93,15 +104,15 @@
     trainer_subfolder = DEFAULT_TRAINER_SUBFOLDER
     trainer_config_file = DEFAULT_TRAINER_CONFIG_FILE
     trainer_csv_log_file = DEFAULT_TRAINER_CSV_LOG_FILE
     dataset_config_file = DEFAULT_DATASET_CONFIG_FILE
     trainer_state_file = DEFAULT_TRAINER_STATE_FILE
     default_optimizer = OptimizerType.ADAM
     default_lr_scheduler = None
-    _required_backends = []
+    _required_backends = [Backends.ACCELERATE]
 
     def __init__(
         self,
         model: Model = None,
         config: TrainerConfig = None,
         train_dataset: Dataset = None,
         eval_dataset: Dataset = None,
@@ -111,19 +122,23 @@
         optimizer: torch.optim.Optimizer = None,
         lr_scheduler=None,
         accelerator: "Accelerator" = None,
     ):
         # Check if all required dependencies are installed
         verify_dependencies(self._required_backends)
 
+        # Setup logger
+        self.logger = get_distributed_logger(__name__)
+
+        # Configuration
         self.config = config
         self.device = "cuda" if torch.cuda.is_available() and not self.config.use_cpu else "cpu"
 
         # Set determinism
-        self._set_seed(self.config.seed)
+        set_seed(self.config.seed)
 
         # Setup model and preprocessor(s)
         self.model = self._setup_model(model)
         if self.model.preprocessor is None:
             if preprocessor is not None:
                 self.model.preprocessor = preprocessor
             else:
@@ -132,57 +147,60 @@
                 )
 
         # Configure datasets and data loaders
         self.train_dataset = train_dataset
         self.eval_dataset = eval_dataset
         self.data_collator = data_collator or self.train_dataset.data_collator
         self.train_dataloader, self.eval_dataloader = self._setup_dataloaders()
+        self.total_steps = len(self.train_dataloader) * self.config.num_epochs
+        self.config.save_steps = len(self.train_dataloader) if not self.config.save_steps else self.config.save_steps
+        self.save_steps_per_epoch = math.ceil(len(self.train_dataloader) / self.config.save_steps)
 
         # Setup optimizer and (optionally) lr scheduler
         self.optimizer, self.lr_scheduler = self._setup_optimizers(optimizer, lr_scheduler)
 
         # Setup accelerated objects if possible
-        if accelerator is None and self.config.distributed and not self.config.use_cpu:
-            self.accelerator = self._setup_accelerator()
-            self.scaler = self.accelerator.scaler
-            self.device = self.accelerator.device
-        else:
-            self.accelerator = accelerator
-            enabled = True if (
-                self.config.mixed_precision is not None and not (self.config.use_cpu or self.device == "cpu")
-            ) else False
-            self.scaler = torch.cuda.amp.GradScaler(enabled=enabled)
+        self.accelerator = accelerator
+        if self.accelerator is None:
+            self.accelerator = Accelerator(
+                mixed_precision=self.config.mixed_precision,
+                cpu=True if self.device == "cpu" else False,
+                step_scheduler_with_optimizer=True if self.lr_scheduler is not None else False,
+                gradient_accumulation_steps=self.config.gradient_accumulation_steps,
+            )
+
+        self.model, self.optimizer, self.lr_scheduler, self.train_dataloader, self.eval_dataloader = (
+            self.accelerator.prepare(
+                self.model,
+                self.optimizer,
+                self.lr_scheduler,
+                self.train_dataloader,
+                self.eval_dataloader,
+            )
+        )
 
         # Setup metrics handler and inner trackers for the trainer
         self.metrics_handler = metrics_handler or self._setup_metrics_handler()
 
         # Configure checkpoints and logging directories
         self.logs_dir = resolve_logdir(os.path.join(self.config.output_dir, self.config.logs_dir))
         self.checkpoints_dir = os.path.join(self.config.output_dir, self.config.checkpoints_dir)
 
         # Setup logging properties
         self.tensorboard = SummaryWriter(log_dir=self.logs_dir)
         self.csv_logger = CSVLogger(logs_dir=self.logs_dir, csv_filename=self.trainer_csv_log_file)
 
-        self.current_epoch = 1
-
         # Configure trainer state
         self.state = TrainerState(
-            epoch=self.current_epoch,
+            epoch=1,
             total_epochs=self.config.num_epochs,
             metric_for_best_checkpoint=self.config.metric_for_best_model,
-            logs_dir=self.tensorboard.log_dir,
+            logs_dir=self.logs_dir,
         )
 
-    @staticmethod
-    def _set_seed(seed):
-        torch.manual_seed(seed)
-        np.random.seed(seed)
-        random.seed(seed)
-
     def _setup_model(self, model: Model) -> Model:
         """
         Download the model from HuggingFace Hub if `init_weights_from` is given in the config. Load the model to the
         device and return it.
         """
         if model is None:
             raise ValueError("`model` must be given to the Trainer!")
@@ -193,16 +211,15 @@
             else:
                 model_path = hf_hub_download(
                     hub_path,
                     filename=model.model_filename,
                     cache_dir=HEZAR_CACHE_DIR,
                     resume_download=True,
                 )
-            model.load_state_dict(torch.load(model_path, map_location="cpu"))
-        model.to(self.device)
+            model.load_state_dict(torch.load(model_path))
         return model
 
     def _setup_dataloaders(self) -> Tuple[DataLoader, DataLoader | None]:
         """
         Set up data loaders (train/eval) and return them.
 
         Returns:
@@ -225,15 +242,15 @@
                 batch_size=self.config.eval_batch_size or self.config.batch_size,
                 collate_fn=self.data_collator,
                 num_workers=self.config.num_dataloader_workers,
                 drop_last=self.config.dataloader_drop_last,
                 shuffle=self.config.dataloader_shuffle,
             )
         else:
-            logger.warning(
+            self.logger.warning(
                 "Cannot create eval dataloader because `eval_dataset` is not given to the Trainer! "
                 "Setting eval_dataloader to None..."
             )
             eval_dataloader = None
 
         return train_dataloader, eval_dataloader
 
@@ -261,39 +278,14 @@
                 scheduler_kwargs = self.config.lr_scheduler_kwargs or {}
                 if scheduler_name is None:
                     lr_scheduler = None
                 else:
                     lr_scheduler = lr_schedulers[scheduler_name](optimizer, **scheduler_kwargs, verbose=True)
         return optimizer, lr_scheduler
 
-    def _setup_accelerator(self):
-        if is_backend_available(Backends.ACCELERATE):
-            from accelerate import Accelerator
-
-            accelerator = Accelerator(
-                mixed_precision=self.config.mixed_precision,
-                step_scheduler_with_optimizer=True if self.lr_scheduler is not None else False,
-            )
-            self.model, self.optimizer, self.lr_scheduler, self.train_dataloader, self.eval_dataloader = (
-                accelerator.prepare(
-                    self.model,
-                    self.optimizer,
-                    self.lr_scheduler,
-                    self.train_dataloader,
-                    self.eval_dataloader,
-                )
-            )
-        else:
-            raise ValueError(
-                "The configuration for this trainer requires the package `accelerate` to be installed! "
-                "(config.distributed=True)"
-            )
-
-        return accelerator
-
     def _setup_metrics_handler(self):
         """
         Setup MetricsHandler instance for the trainer
 
         Returns:
             A MetricsHandler subclass instance based on self.config.task
         """
@@ -306,43 +298,59 @@
         Load trainer states like model weights, optimizer, etc. from a checkpoint
 
         Args:
             checkpoint: Path to checkpoint directory
             load_best: Whether to load the best checkpoint or not, if False, loads the latest checkpoint
         """
         if os.path.isdir(checkpoint) and load_best:
-            logger.warning("The `load_best` parameter has no effect when `checkpoint` is a path!")
+            self.logger.warning("The `load_best` parameter has no effect when `checkpoint` is a path!")
 
-        self.state = TrainerState.load(os.path.join(self.checkpoints_dir, self.trainer_state_file))
+        # Load trainer state file if available
+        state_path = os.path.join(self.checkpoints_dir, self.trainer_state_file)
+        if os.path.isfile(state_path):
+            self.state = TrainerState.load(state_path)
+
+        # If checkpoint is True instead of a path to the checkpoint, load the latest of the best checkpoint
         if isinstance(checkpoint, bool):
             if load_best:
                 checkpoint = os.path.join(self.checkpoints_dir, str(self.state.best_checkpoint))
             else:
-                checkpoint = os.path.join(self.checkpoints_dir, str(self.state.epoch))
+                # Get the most recent checkpoint based on global step
+                checkpoint = os.path.join(
+                    self.checkpoints_dir,
+                    str(self.state.global_step).zfill(len(str(self.total_steps))),
+                )
+
+        # Load checkpoint file and update trainer state based on the checkpoint file
         if os.path.isdir(checkpoint):
-            # Figure out the epoch number
-            epoch = os.path.basename(checkpoint) if os.path.basename(checkpoint).isdigit() else self.state.epoch
-            if str(epoch).isdigit():
-                self.state.epoch = int(epoch)
+            # Figure out the step and epoch number
+            step = os.path.basename(checkpoint)
+            self.state.global_step = int(step) if step.isdigit() else self.state.global_step
+            self.state.epoch = math.ceil(self.state.global_step / len(self.train_dataloader)) - 1
+            self.state.epoch_step = self.state.global_step % len(self.train_dataloader)
+            if self.state.epoch_step == 0:
+                self.state.epoch += 1
             # Load model's state dict
             model_path = os.path.join(checkpoint, self.model.model_filename)
             if os.path.isfile(model_path):
                 self.model.load_state_dict(torch.load(model_path))
-                if self.accelerator is not None:
-                    self.model = self.accelerator.prepare(self.model)
-                logger.info(f"Successfully loaded checkpoint from `{checkpoint}` ")
+                self.model = self.accelerator.prepare(self.model)
+                self.logger.info(f"Successfully loaded checkpoint from `{checkpoint}` ")
             else:
                 raise FileNotFoundError(
                     f"Could not find `{self.model.model_filename}` at `{os.path.dirname(model_path)}`!\n"
                 )
         else:
-            logger.warning(
+            self.logger.warning(
                 f"{checkpoint} does not seem to be a valid checkpoint!"
             )
 
+        if self.state.global_step >= self.total_steps:
+            self.logger.warning(f"The checkpoint at `{checkpoint}` belongs to the last training step!")
+
     def load_csv_logs(self, logs_dir=None):
         """
         Load the CSV log file
         Args:
             logs_dir: Path to logs directory, defaults to self.config.logs_dir
 
         Returns:
@@ -365,34 +373,14 @@
         """
         # Put inputs on device manually if accelerator is not available, otherwise it's taken care of by the accelerator
         if self.accelerator is None:
             input_batch = {k: v.to(self.device) if isinstance(v, torch.Tensor) else v for k, v in input_batch.items()}
 
         return input_batch
 
-    def amp_context_manager(self):
-        """
-        An auto context manager for mixed precision.
-
-        Returns:
-            A torch autocast context manager
-        """
-        if self.accelerator is not None:
-            context_manager = self.accelerator.autocast()
-        else:
-            device_type = "cuda" if "cuda" in self.device else "cpu"
-            dtype = torch.bfloat16 if self.config.mixed_precision == "bf16" or device_type == "cpu" else torch.float16
-            enabled = self.config.mixed_precision is not None or self.config.mixed_precision == "no"
-            context_manager = torch.autocast(
-                device_type=device_type,
-                dtype=dtype,
-                enabled=enabled
-            )
-        return context_manager
-
     def forward(self, input_batch):
         """
         Perform model forward on the input batch
 
         In special cases, one can override this method in their desired trainer.
 
         Args:
@@ -434,20 +422,15 @@
 
         return loss
 
     def optimization_step(self):
         """
         Perform optimization step
         """
-        if self.accelerator is not None:
-            self.optimizer.step()
-        else:
-            self.scaler.step(self.optimizer)
-            self.scaler.update()
-
+        self.optimizer.step()
         self.optimizer.zero_grad()
 
     def lr_scheduler_step(self, metrics=None):
         """
         Perform the learning rate scheduling step
 
         Args:
@@ -466,23 +449,20 @@
 
         Args:
             input_batch: A batch of inputs to train
 
         Returns:
             Train step outputs including loss, logits, etc.
         """
-        with self.amp_context_manager():
+        with self.accelerator.autocast():
             outputs = self.forward(input_batch)
 
-        loss = self.compute_loss(outputs, **input_batch) / self.config.gradient_accumulation_steps
+        loss = self.compute_loss(outputs, **input_batch)
 
-        if self.accelerator is not None:
-            self.accelerator.backward(loss)
-        else:
-            self.scaler.scale(loss).backward()
+        self.accelerator.backward(loss)
 
         outputs["loss"] = loss
 
         return outputs
 
     def evaluation_step(self, input_batch: Dict[str, torch.Tensor]) -> Dict[str, Any]:
         """
@@ -490,15 +470,15 @@
 
         Args:
             input_batch: A batch of inputs to evaluate
 
         Returns:
             Evaluation step outputs including loss, logits, etc.
         """
-        with self.amp_context_manager():
+        with self.accelerator.autocast():
             outputs = self.forward(input_batch)
 
         loss = self.compute_loss(outputs, **input_batch)
 
         if self.model.is_generative and self.config.evaluate_with_generate:
             generate_inputs = sanitize_function_parameters(self.model.generate, input_batch)
             generated_ids = self.model.generate(**generate_inputs)
@@ -514,35 +494,62 @@
 
         Args:
             epoch_num: Number of the current epoch
 
         Returns:
             Metrics averages through the full iteration
         """
-        losses_sum = 0.0
+        losses_sum = 0
         self.model.train()
         with tqdm(
             self.train_dataloader,
             unit="batch",
             desc=f"Epoch: {epoch_num}/{self.config.num_epochs} ",
             bar_format=TQDM_BAR_FORMAT,
             ascii=" #",
+            disable=not self.accelerator.is_local_main_process,
         ) as iterator:
             for step, input_batch in enumerate(iterator):
+                # TODO make this more efficient in a way that the data loader skips batches without iterating them
+                # Skip the first batches to reach `epoch_step`
+                if step < self.state.epoch_step:
+                    iterator.set_description(desc="Skipping already trained batches...")
+                    continue
+                elif step == self.state.epoch_step:
+                    iterator.set_description(desc=f"Epoch: {epoch_num}/{self.config.num_epochs} ")
+
+                # Prepare inputs
                 input_batch = self.prepare_input_batch(input_batch)
+
                 # Training on one batch
-                outputs = self.training_step(input_batch)
-                # Optimization step
-                if (step + 1) % self.config.gradient_accumulation_steps == 0 or step == len(iterator):
+                with self.accelerator.accumulate(self.model):
+                    outputs = self.training_step(input_batch)
+                    # Optimization step
                     self.optimization_step()
+
                 # Gather outputs for metrics
                 losses_sum += outputs["loss"].item()
                 avg_loss = losses_sum / (step + 1)
                 iterator.set_postfix(loss=avg_loss)
+
+                # Update steps states
                 self.state.global_step += 1
+                self.state.epoch_step += 1
+
+                # Save trainer outputs if `save_steps` is hit
+                if self.config.save_steps and self.state.global_step % self.config.save_steps == 0:
+                    ckpt_path_name = str(self.state.global_step).zfill(len(str(self.total_steps)))
+                    self.save(os.path.join(self.checkpoints_dir, ckpt_path_name))
+                    # Save Trainer state
+                    self.state.save(
+                        os.path.join(
+                            self.checkpoints_dir,
+                            self.trainer_state_file,
+                        )
+                    )
 
         return {"loss": avg_loss}
 
     def evaluate(self):
         """
         Evaluates the model on the whole eval dataset and verbose live metric values in the progress bar
 
@@ -553,133 +560,136 @@
         self.model.eval()
         with tqdm(
             self.eval_dataloader,
             unit="batch",
             desc="Evaluating... ",
             bar_format=TQDM_BAR_FORMAT,
             ascii=" #",
+            disable=not self.accelerator.is_local_main_process,
         ) as iterator:
             with torch.inference_mode():
                 for step, input_batch in enumerate(iterator):
                     input_batch = self.prepare_input_batch(input_batch)
                     # Evaluation on one batch
                     outputs = self.evaluation_step(input_batch)
-                    logits = outputs["logits"].detach().cpu().numpy()
-                    labels = input_batch["labels"].detach().cpu().numpy()
+                    logits, labels = self.accelerator.gather_for_metrics((outputs["logits"], input_batch["labels"]))
                     # Compute metrics
-                    evaluation_results = self.metrics_handler.compute_metrics(logits, labels)
-                    evaluation_results["loss"] = outputs["loss"].item()
+                    evaluation_results = self.metrics_handler.compute_metrics(
+                        logits.clone().detach().cpu(),
+                        labels.clone().detach().cpu(),
+                    )
+                    evaluation_results["loss"] = self.accelerator.gather_for_metrics(outputs["loss"]).item()
                     # Gather outputs for metrics
                     self.metrics_handler.tracker.update(evaluation_results)
                     iterator.set_postfix(**self.metrics_handler.tracker.avg())
 
         return self.metrics_handler.tracker.avg()
 
     def print_info(self):
         """
         Print training info
         """
 
         def _print_info_line(key, value):
-            line = f"  {colorize_text(key, 'bold')}: `{colorize_text(str(value), 'italic')}`"
-            print(line)
+            line = f"  {colorize_text(key, 'bold')}: {colorize_text(str(value), 'italic')}"
+            self.accelerator.print(line)
 
         header = f"{'*' * 20} Training Info {'*' * 20}"
         footer = "*" * len(header)
         info = {
             "Output Directory": self.config.output_dir,
             "Task": self.config.task,
             "Model": type(self.model).__name__,
             "Init Weights": self.config.init_weights_from or "N/A",
             "Device(s)": self.device,
             "Batch Size": self.config.batch_size,
             "Epochs": self.config.num_epochs,
+            "Total Steps": self.total_steps,
             "Training Dataset": self.train_dataset,
             "Evaluation Dataset": self.eval_dataset,
             "Optimizer": self.config.optimizer or self.default_optimizer,
             "Scheduler": self.config.lr_scheduler,
             "Initial Learning Rate": self.config.learning_rate,
             "Learning Rate Decay": self.config.weight_decay,
             "Number of Parameters": self.model.num_parameters,
             "Number of Trainable Parameters": self.model.num_trainable_parameters,
             "Mixed Precision": self.config.mixed_precision or "Full (fp32)",
+            "Gradient Accumulation Steps": self.config.gradient_accumulation_steps,
             "Metrics": list(self.metrics_handler.metrics.keys()),
+            "Save Steps": self.config.save_steps,
             "Checkpoints Path": self.checkpoints_dir,
             "Logs Path": self.logs_dir,
         }
 
         # Header
-        print(f"\n{colorize_text(header, 'bold')}\n")
+        self.accelerator.print(f"\n{colorize_text(header, 'bold')}\n")
         # Info
         [_print_info_line(k, v) for k, v in info.items()]
         # Footer
-        print(f"\n{colorize_text(footer, 'bold')}\n")
+        self.accelerator.print(f"\n{colorize_text(footer, 'bold')}\n")
 
     def train(self, resume_from_checkpoint: str | bool = None):
         """
         The full training process like training, evaluation, logging and saving model checkpoints.
 
         Args:
             resume_from_checkpoint: Resume from checkpoint path (if value is a path) or automatically load from the
             latest checkpoint (if value is True)
         """
         if resume_from_checkpoint:
             self.load_from_checkpoint(resume_from_checkpoint)
-            if self.current_epoch >= self.config.num_epochs:
-                logger.info(
-                    f"Unable to resume from `{os.path.join(self.checkpoints_dir, str(self.state.epoch))}` "
-                    f"since it belongs to the ending epoch!"
-                )
-            self.current_epoch = self.state.epoch + 1
 
         self.print_info()
 
-        for epoch in range(self.current_epoch, self.config.num_epochs + 1):
-            print()
+        for epoch in range(self.state.epoch, self.config.num_epochs + 1):
+            self.accelerator.print()
 
-            # Train on the whole train data
+            # Train on the whole training set
             training_results = self.inner_training_loop(epoch)
-            # Evaluate the model on eval data
+
+            # Save checkpoint
+            if self.accelerator.is_local_main_process:
+                if self.config.save_enabled:
+                    ckpt_path_name = str(self.state.global_step).zfill(len(str(self.total_steps)))
+                    self.save(os.path.join(self.checkpoints_dir, ckpt_path_name))
+
+            # Evaluate the model on the evaluation set
             evaluation_results = self.evaluate()
 
             # LR scheduler step
             self.lr_scheduler_step(evaluation_results["loss"])
 
             # Metrics gathering
             train_logs = {f"train.{metric_name}": value for metric_name, value in training_results.items()}
             evaluation_logs = {f"evaluation.{metric_name}": value for metric_name, value in evaluation_results.items()}
             all_logs = {**train_logs, **evaluation_logs}
 
             # Update trainer state
             self.state.epoch = epoch
+            self.state.epoch_step = 0
             self.state.update_best_results(
                 metric_value=all_logs[self.config.metric_for_best_model],
                 objective=self.metrics_handler.objective,
                 step=epoch,
             )
 
-            # maybe save checkpoint
-            if epoch % self.config.save_freq == 0:
-                ckpt_save_path = os.path.join(self.checkpoints_dir, str(epoch))
-                self.save(ckpt_save_path)
-
-            self.log(train_logs, evaluation_logs, epoch)
+            # Log everything
+            self.log(all_logs, epoch)
 
-        logger.info("Training done!")
+        self.logger.info("Training done!")
 
-    def log(self, train_logs: Dict[str, Any], evaluation_logs: Dict[str, Any], step: int):
+    def log(self, logs: Dict[str, Any], step: int):
         """
         Log metrics results
         """
         # Log to tensorboard
-        write_to_tensorboard(self.tensorboard, train_logs, step)
-        write_to_tensorboard(self.tensorboard, evaluation_logs, step)
+        write_to_tensorboard(self.tensorboard, logs, step)
 
         # Log to CSV
-        self.csv_logger.write({**train_logs, **evaluation_logs}, step)
+        self.csv_logger.write(logs, step)
 
         # Save trainer state
         self.state.save(
             os.path.join(
                 self.checkpoints_dir,
                 self.trainer_state_file,
             )
@@ -712,17 +722,17 @@
         dataset_config_file = dataset_config_file or self.dataset_config_file
 
         self.config.save(path, filename=config_filename, subfolder=subfolder)
         self.model.save(path, filename=model_filename, config_filename=model_config_filename)
         if isinstance(self.train_dataset, Dataset):
             self.train_dataset.config.save(path, filename=dataset_config_file, subfolder=subfolder)
         else:
-            logger.warning(
-                f"The dataset passed to the Trainer is not a `hezar.data.Dataset` instance so that no dataset config"
-                f" will be saved!"
+            self.logger.warning(
+                "The dataset passed to the Trainer is not a `hezar.data.Dataset` instance so that no dataset config"
+                " will be saved!"
             )
 
     def push_to_hub(
         self,
         repo_id: str,
         config_filename: str = None,
         push_model: bool = True,
```

### Comparing `hezar-0.36.1/hezar/trainer/trainer_utils.py` & `hezar-0.37.0/hezar/trainer/trainer_utils.py`

 * *Files 20% similar despite different names*

```diff
@@ -10,35 +10,38 @@
 __all__ = [
     "TrainerState",
     "AverageMeter",
     "MetricsTracker",
     "CSVLogger",
     "write_to_tensorboard",
     "resolve_logdir",
+    "get_distributed_logger",
 ]
 
 
 @dataclass
 class TrainerState:
     """
     A Trainer state is a container for holding specific updating values in the training process and is saved when
     checkpointing.
 
     Args:
         epoch: Current epoch number
         total_epochs: Total epochs to train the model
         global_step: Number of the update steps so far, one step is a full training step (one batch)
+        epoch_step: Number of the update steps in the current epoch
         metric_for_best_checkpoint: The metric key for choosing the best checkpoint (Also given in the TrainerConfig)
         best_metric_value: The value of the best checkpoint saved so far
         best_checkpoint: Path to the best model checkpoint so far
         logs_dir: Path to the logs directory
     """
     epoch: int = 1
     total_epochs: int = None
     global_step: int = 0
+    epoch_step: int = 0
     metric_for_best_checkpoint: str = None
     best_metric_value: float = None
     best_checkpoint: str = None
     logs_dir: str = None
 
     def update(self, items: dict, **kwargs):
         items.update(kwargs)
@@ -159,7 +162,26 @@
 
 def resolve_logdir(log_dir) -> str:
     import socket
     from datetime import datetime
 
     current_time = datetime.now().strftime("%b%d_%H-%M-%S")
     return os.path.join(log_dir, current_time + "_" + socket.gethostname())
+
+
+def get_distributed_logger(name: str, level: str = None, fmt: str = None):
+    """
+    Distributed logger is responsible for handling logging on multiple processes/machines
+    """
+    import logging
+
+    from accelerate.logging import get_logger
+
+    fmt = fmt or "Hezar (%(levelname)s): %(message)s"
+    level = level or "INFO"
+    logger = get_logger(name, level)
+    handler = logging.StreamHandler()
+    formatter = logging.Formatter(fmt)
+    handler.setFormatter(formatter)
+    logger.logger.addHandler(handler)
+
+    return logger
```

### Comparing `hezar-0.36.1/hezar/utils/audio_utils.py` & `hezar-0.37.0/hezar/utils/audio_utils.py`

 * *Files identical despite different names*

### Comparing `hezar-0.36.1/hezar/utils/common_utils.py` & `hezar-0.37.0/hezar/utils/common_utils.py`

 * *Files identical despite different names*

### Comparing `hezar-0.36.1/hezar/utils/data_utils.py` & `hezar-0.37.0/hezar/utils/data_utils.py`

 * *Files 6% similar despite different names*

```diff
@@ -3,26 +3,26 @@
 from typing import TYPE_CHECKING, Any, Dict, List, Literal, Optional
 
 from omegaconf import DictConfig
 
 from ..constants import PaddingType
 from .logging import Logger
 
-
 if TYPE_CHECKING:
     import torch
 
-
 __all__ = [
     "convert_batch_dict_dtype",
     "resolve_inputs_length_for_padding",
     "pad_batch_items",
     "shift_tokens_right",
+    "torch2numpy",
     "get_non_numeric_keys",
     "flatten_dict",
+    "set_seed",
 ]
 
 logger = Logger(__name__)
 
 
 # TODO: This code might be able to be written in a cleaner way, but be careful, any change might break a lot of things!
 def convert_batch_dict_dtype(batch_dict: Dict[str, Any], dtype: str = None, skip_keys: list = None):
@@ -86,21 +86,26 @@
         if max_length is not None:
             padding_type = "max_length"
         else:
             padding_type = "longest"
 
     # Now lets resolve any conflicts
     if padding_type == "longest":
-        if max_length is not None:
-            logger.warning(
-                "Setting padding='longest' and max_length is not valid. You must set one of them"
-                " and leave the other as None. Falling back to padding='longest'"
-            )
-
-        inputs_length = inputs_max_length
+        if max_length is not None and max_length < inputs_max_length:
+            if not truncation:
+                logger.warning(
+                    f"Setting padding_type to `longest` and a max_length={max_length} which is below the "
+                    f"inputs longest value {inputs_max_length} requires truncation to be True, "
+                    f"got truncation={truncation}. Falling back to truncating inputs to max_length={max_length}."
+                )
+                inputs_length = max_length
+            else:
+                inputs_length = max_length
+        else:
+            inputs_length = inputs_max_length
 
     elif padding_type == "max_length":
         if max_length is None:
             logger.warning(
                 "Setting padding='max_length' but no max_length value is provided! Falling back to padding='longest'"
             )
             inputs_length = inputs_max_length
@@ -172,14 +177,27 @@
 
     # replace possible -100 values in labels by `pad_token_id`
     shifted_input_ids.masked_fill_(shifted_input_ids == -100, pad_token_id)
 
     return shifted_input_ids
 
 
+def torch2numpy(*args):
+    """
+    Cast tensors to numpy
+
+    Args:
+        *args: Any number of torch.Tensor objects
+
+    Returns:
+        The same inputs cast to numpy
+    """
+    return [arg.cpu().numpy() if isinstance(arg, torch.Tensor) else arg for arg in args]
+
+
 def get_non_numeric_keys(d: Dict, batched=True):
     """
     Get keys that have string values in a dictionary
 
     Args:
         d: The dict
         batched: Are the input dict values batched or not
@@ -212,7 +230,17 @@
     for k, v in dict_config.items():
         if isinstance(v, (Dict, DictConfig)):
             config.update(flatten_dict(v))
         else:
             config[k] = v
 
     return config
+
+
+def set_seed(seed):
+    import torch
+    import numpy as np
+    import random
+
+    torch.manual_seed(seed)
+    np.random.seed(seed)
+    random.seed(seed)
```

### Comparing `hezar-0.36.1/hezar/utils/file_utils.py` & `hezar-0.37.0/hezar/utils/file_utils.py`

 * *Files identical despite different names*

### Comparing `hezar-0.36.1/hezar/utils/hub_utils.py` & `hezar-0.37.0/hezar/utils/hub_utils.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,49 +1,28 @@
 import os
 
 from huggingface_hub import HfApi, Repository
 
-from ..constants import HEZAR_CACHE_DIR, HEZAR_HUB_ID, RepoType
+from ..constants import HEZAR_CACHE_DIR, RepoType
 from ..utils.logging import Logger
 
 
 __all__ = [
-    "resolve_pretrained_path",
     "get_local_cache_path",
     "exists_in_cache",
     "exists_on_hub",
     "clone_repo",
     "list_repo_files",
     "get_state_dict_from_hub",
     "clean_cache",
 ]
 
 logger = Logger(__name__)
 
 
-def resolve_pretrained_path(hub_or_local_path):
-    """
-    **DEPRECATED**
-
-    Resolve a local or Hub path. If path exists locally it just returns the input, otherwise tries to resolve
-    hub_or_local_path. If it contains the namespace (author/org) leave it as is, otherwise change to hezarai/{hub_path}
-
-    Args:
-        hub_or_local_path: Repo name or id
-
-    Returns:
-        A proper pretrained path
-    """
-    logger.warning("`resolve_pretrained_path` is deprecated! Use the raw `hub_or_local_path`!")
-    if os.path.isdir(hub_or_local_path):
-        return hub_or_local_path
-    repo_id = f"{HEZAR_HUB_ID}/{hub_or_local_path}" if "/" not in hub_or_local_path else hub_or_local_path
-    return repo_id
-
-
 def get_local_cache_path(repo_id, repo_type):
     """
     Given the hub path and repo type, configure the local path to save everything e.g, ~/.hezar/models/<repo_name>
 
     Args:
         repo_id: Repo name or id
         repo_type: Repo type e.g, model, dataset, etc
```

### Comparing `hezar-0.36.1/hezar/utils/image_utils.py` & `hezar-0.37.0/hezar/utils/image_utils.py`

 * *Files identical despite different names*

### Comparing `hezar-0.36.1/hezar/utils/integration_utils.py` & `hezar-0.37.0/hezar/utils/integration_utils.py`

 * *Files identical despite different names*

### Comparing `hezar-0.36.1/hezar/utils/logging.py` & `hezar-0.37.0/hezar/utils/logging.py`

 * *Files identical despite different names*

### Comparing `hezar-0.36.1/hezar/utils/registry_utils.py` & `hezar-0.37.0/hezar/utils/registry_utils.py`

 * *Files identical despite different names*

### Comparing `hezar-0.36.1/pyproject.toml` & `hezar-0.37.0/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "hezar"
-version = "0.36.1"
+version = "0.37.0"
 packages = [{ include = "hezar" }]
 description = "Hezar: The all-in-one AI library for Persian, supporting a wide variety of tasks and modalities!"
 license = "Apache-2.0"
 authors = ["Aryan Shekarlaban <arxyzan@gmail.com>"]
 maintainers = ["Aryan Shekarlaban <arxyzan@gmail.com>"]
 repository = "https://github.com/hezarai/hezar"
 homepage = "https://github.com/hezarai"
@@ -37,15 +37,15 @@
 omegaconf = ">=2.3.0"
 transformers = ">=4.28.0"
 tokenizers = ">=0.13.0"
 datasets = ">=2.9.0"
 huggingface_hub = ">=0.12.0"
 tensorboard = ">=2.10.0"
 scikit-learn = ">=1.0.0"
-accelerate = {version="*", optional=true}
+accelerate = ">=0.27.0"
 numpy = {version="1.24.*", optional=true}
 scipy = {version="1.11.4", optional=true}
 gensim = {version="4.3.2", optional=true}
 seqeval = {version=">=1.2.0", optional=true}
 jiwer = {version=">=3.*", optional=true}
 soundfile = {version=">=0.12.0", optional=true}
 librosa = {version=">=0.10.0", optional=true}
@@ -55,15 +55,15 @@
 
 [tool.poetry.extras]
 nlp = ["seqeval", "jiwer", "nltk", "rouge_score"]
 audio = ["soundfile", "librosa", "jiwer"]
 vision = ["pillow"]
 embeddings = ["gensim", "numpy", "scipy"]
 dev = ["pytest", "ruff", "sphinx", "myst-parser", "furo", "sphinx-copybutton"]
-all = ["numpy", "gensim", "accelerate", "seqeval", "jiwer", "soundfile", "librosa", "pillow", "nltk", "rouge_score", "scipy"]
+all = ["numpy", "gensim", "seqeval", "jiwer", "soundfile", "librosa", "pillow", "nltk", "rouge_score", "scipy"]
 
 [tool.black]
 line-length = 120
 target-version = ['py39', 'py310', 'py311']
 
 [tool.ruff]
 ignore = ["C901", "E501", "E741", "W605", "F403", "F405"]
```

### Comparing `hezar-0.36.1/PKG-INFO` & `hezar-0.37.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hezar
-Version: 0.36.1
+Version: 0.37.0
 Summary: Hezar: The all-in-one AI library for Persian, supporting a wide variety of tasks and modalities!
 Home-page: https://github.com/hezarai
 License: Apache-2.0
 Keywords: packaging,poetry
 Author: Aryan Shekarlaban
 Author-email: arxyzan@gmail.com
 Maintainer: Aryan Shekarlaban
@@ -28,15 +28,15 @@
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Provides-Extra: all
 Provides-Extra: audio
 Provides-Extra: dev
 Provides-Extra: embeddings
 Provides-Extra: nlp
 Provides-Extra: vision
-Requires-Dist: accelerate ; extra == "all"
+Requires-Dist: accelerate (>=0.27.0)
 Requires-Dist: datasets (>=2.9.0)
 Requires-Dist: gensim (==4.3.2) ; extra == "embeddings" or extra == "all"
 Requires-Dist: huggingface_hub (>=0.12.0)
 Requires-Dist: jiwer (>=3) ; extra == "nlp" or extra == "audio" or extra == "all"
 Requires-Dist: librosa (>=0.10.0) ; extra == "audio" or extra == "all"
 Requires-Dist: nltk (>=3.8.0) ; extra == "nlp" or extra == "all"
 Requires-Dist: numpy (==1.24.*) ; extra == "embeddings" or extra == "all"
```

