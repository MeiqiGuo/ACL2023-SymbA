# ACL2023-SymbA

Repo for our ACL 2023 paper: Decoding Symbolism in Language Models

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


