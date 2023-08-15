# Tibetan Translator GPT

version: 2023.05.30

author: PeterS

This repository is dedicated to the development of a Tibetan translation machine through fine-tuning of GPT models.

### Samples

In the samples folder, you can find results of translations (25 + 1) from Tibetan to English from consecutive versions of our system. In the samples, each line of Tibetan text is followed by the original translation on https://www.lotsawahouse.org/ followed by translations provided by two versions of our system.

* version 1 - GPT-3 Babbage fine-tuned for 4 epochs on the dataset tib_small.jsonl, which contains 19794 language pairs

* version 2 - GPT-3 Babbage fine-tuned for 4 epochs on the dataset tib_long_train.jsonl, which contains 53158 language pairs

Samples are presented both as .txt and .html files. The text that were translated were removed from the training dataset.

### Datasets

The datasets folder contains datasets of Tibetan-English text as scraped from https://www.lotsawahouse.org/ with some edits by PeterS. There are two datasets: tib_small and tib_long. Both are uploaded in the original .txt version and converted into .jsonl format for GPT-3 fine-tuning. There is an additional tib_long_train.json, from which the 25 texts used for validation were removed.

### Updates

2023.05.26 - Version 2 of our system already outperforms GPT-4 in Tibetan-to-English translation, despite being a much smaller model. However, the quality of translations is still not satisfactory, therefore, we don't recommend fine-tuning your models on our dataset just yet. The problem we are facing now is that line-by-line text in our dataset is, in many places, not matching. Also, English translations in many places are adding words that do not appear in the Tibetan text. While for the human reader it does not matter, for machine learning this presents a problem. Currently, we are working on improving the dataset. Expect an update soon.


