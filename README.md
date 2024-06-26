# InferBR

This repository contains InferBR, a NLI dataset accepted in the LREC/COLING 2024 (https://lrec-coling-2024.org/).

There are three CSV files: train (8399 instances), val (646), and test (1758). 

Below the description of each column in the files:

* **premise**:	the premise sentence.
* **hypothesis**:	the hypothesis sentence. 
* **label**:	The generated label for the hypothesis considering the premise: 
  * 0 –Contradiction
  * 1 –Entailment
  * 2 –Neutral
* **reviwers_output**: 	
  * “Disagreement”: the two reviewers assigned different labels for the pair of sentences and none of them flagged the instance as dubious or confusing text.
  * “Confusing”: at least one reviewer flagged the premise or the hypothesis of the instance as “confusing text”. The flag was reviewed by a third reviewer, who also confirmed that the text was confusing.
  * “Contradiction”, “Entailment”or “Neutral”: the label annotated by the reviewers.
* **confuse_sentence**: 	
  * “P” means the premise has a confusing sentence.“H” means the hypothesis is confusing. “OK” means the text was not flagged as confusing.
* **low_quality**:	
  * “S” means the instance is flagged as low quality because one of the reasons:
    * disagreement between the labels each reviewer annotated;
    * reviewers agreed on the label, but it is different from the generated one,
    * at least one reviewer flagged the premise or hypothesis as confusing.
  * “N” means the instance is not low quality.


# Citation
If you use our dataset please cite us.

```bibtex
@inproceedings{bencke-etal-2024-inferbr-natural,
    title = "{I}nfer{BR}: A Natural Language Inference Dataset in {P}ortuguese",
    author = "Bencke, Luciana  and
      Pereira, Francielle Vasconcellos  and
      Santos, Moniele Kunrath  and
      Moreira, Viviane",
    editor = "Calzolari, Nicoletta  and
      Kan, Min-Yen  and
      Hoste, Veronique  and
      Lenci, Alessandro  and
      Sakti, Sakriani  and
      Xue, Nianwen",
    booktitle = "Proceedings of the 2024 Joint International Conference on Computational Linguistics, Language Resources and Evaluation (LREC-COLING 2024)",
    month = may,
    year = "2024",
    address = "Torino, Italy",
    publisher = "ELRA and ICCL",
    url = "https://aclanthology.org/2024.lrec-main.793",
    pages = "9050--9060",
    
}
```
