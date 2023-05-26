# Tibetan Translator GPT

version: 2023.05.26

author: PeterS

This repository is dedicate to the development of Tibetan tranlation machine through fine-tuning of GPT models.

### Samples

In the samples folder you can find results of translation from Tibetan to English from consecutive versions of our system.
In the samples, each line on Tibetan text is followed by original translation on https://www.lotsawahouse.org/ followed by translations provided by two versions of our system.

* version 1 - GPT-3 Babbage fine-tuned for 4 epochs on the dataset tib_small.jsonl which contains 19844 language pairs

* version 2 - GPT-3 Babbage fine-tuned for 4 epochs on the dataset tib_long.jsonl which contains 54080 language pairs

Samples are presented both as .txt and .html files.

### Datasets

Datasets folder contain datasets of Tibetan-English text as scraped from https://www.lotsawahouse.org/ with some edits by Peter. There are two datasets: tib_small and tib_long.
Both are uploaded in the original .txt version and converted into .jsonl fromat for GPT-3 fine-tuning.
