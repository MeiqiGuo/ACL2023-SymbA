# ACL2023-SymbA

Repo for our ACL 2023 paper: [Decoding Symbolism in Language Models](https://aclanthology.org/2023.acl-long.186/)

## Annotated datasets

1) Conventional symbolism: "conventional_symbols.json"

Data structure:

- signifiers' group name
  - signifier
    - list of ground-truth signifieds

2) Situated advertising symbolism: "situated_ads_symbols.json"

Data structure:

- image_id
  - region: the bounding box of the symbolic region
  - label: the ground-truth signified
  - description: the annotated local description for the symbolic region, considered as the signifier with context
  - signifier: the signifier without context
  - relation_type: the fine-grained type of symbolic relationship

The advertising images can be downloaded at [page](https://people.cs.pitt.edu/~kovashka/ads/#image).

3) Advertising symbolism without context: "ads_symbols.json"

The file can also be obtained by grouping same signifiers from the above file.

## Citation

If you make use of this code, please kindly cite our paper:
```
@inproceedings{guo-etal-2023-decoding,
    title = "Decoding Symbolism in Language Models",
    author = "Guo, Meiqi  and
      Hwa, Rebecca  and
      Kovashka, Adriana",
    booktitle = "Proceedings of the 61st Annual Meeting of the Association for Computational Linguistics (Volume 1: Long Papers)",
    month = jul,
    year = "2023",
    address = "Toronto, Canada",
    publisher = "Association for Computational Linguistics",
    url = "https://aclanthology.org/2023.acl-long.186",
    pages = "3311--3324",
    abstract = "This work explores the feasibility of eliciting knowledge from language models (LMs) to decode symbolism, recognizing something (e.g.,roses) as a stand-in for another (e.g., love). We present our evaluative framework, Symbolism Analysis (SymbA), which compares LMs (e.g., RoBERTa, GPT-J) on different types of symbolism and analyze the outcomes along multiple metrics. Our findings suggest that conventional symbols are more reliably elicited from LMs while situated symbols are more challenging. Results also reveal the negative impact of the bias in pre-trained corpora. We further demonstrate that a simple re-ranking strategy can mitigate the bias and significantly improve model performances to be on par with human performances in some cases.",
}
```

