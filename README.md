# Lexicon of Polarity Shifting Directions
[![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.3545947.svg)](https://doi.org/10.5281/zenodo.3545947)


This repository contains the data presented in:

[Schulder, Marc](http://marc.schulder.info) and [Wiegand, Michael](http://www.coli.uni-saarland.de/~miwieg/) and [Ruppenhofer, Josef](http://ruppenhofer.de/) (2020). [**"Enhancing a Lexicon of Polarity Shifters through the Supervised Classification of Shifting Directions"**](https://www.aclweb.org/anthology/2020.lrec-1.616/). _Proceedings of the 12th Conference on Language Resources and Evaluation (LREC 2018)_, pages 5010–5016, Marseille, France, 11–16 May 2020.

## Content
We provide information on the shifting direction of polarity shifters.
Shifting directions specify whether a polarity shifter can affect __only positive__ polar expressions, __only negative__ ones or shift in __both__ directions.

We cover all shifters found in the [shifter lexicon](https://github.com/uds-lsv/bootstrapped-lexicon-of-english-polarity-shifters) of [Schulder, Wiegand and Ruppenhofer (JNLE 2020)](https://doi.org/10.1017/S135132492000039X), which contains verbs, noun and adjectives.

### Resources
- **Paper:** [ACL Anthology](https://www.aclweb.org/anthology/2020.lrec-1.616/)
- **Data:** See content of this repository

#### Related Resources
- **[Polarity Shifter Resources](https://github.com/uds-lsv/polarity-shifter-resources)**
  - **[IJCNLP 2017](https://github.com/uds-lsv/bootstrapped-lexicon-of-english-verbal-polarity-shifters):** Lexicon of English Verbal Shifters (bootstrapped, lemma-level)
  - **[LREC 2018](https://github.com/uds-lsv/lexicon-of-english-verbal-polarity-shifters):** Lexicon of English Verbal Shifters (manual, sense-level)
  - **[COLING 2018](https://github.com/uds-lsv/bootstrapped-lexicon-of-german-verbal-polarity-shifters):** Lexicon of German Verbal Shifters (bootstrapped, lemma-level)
  - **[JNLE 2020](https://github.com/uds-lsv/bootstrapped-lexicon-of-english-polarity-shifters):** General Lexicon of English Shifters (bootstrapped, lemma-level).
- **[Word Embedding of Amazon Product Review Corpus](https://doi.org/10.5281/zenodo.3370051):** Word2Vec word embedding used to create this data.

## Data
A list of 2521 polarity shifters, labeled for their shifting direction. Contains 863 shifters that affect only positive polar expressions, 288 shifters that affect only negative polar expressions and 1370 shifters that can shift in both directions.

- File: `shifting_directions.txt`
- The lexicon is a comma-separated value (CSV) table
- Each line follows the format `POS,LEMMA,DIRECTION_LABEL,SOURCE`.
  - `POS`: The part of speech of the word (`verb`, `noun`, `adj`)
  - `LEMMA`: The lemma representation of the word in question. Multiword expressions are separated by an underscore (`WORD_WORD`).
  - `DIRECTION_LABEL`: Whether the shifter affects only positive polarities (`AFFECTS_POSITIVE`), only negative polarities (`AFFECTS_NEGATIVE`) or can shift in both directions (`AFFECTS_BOTH`).
  - `SOURCE`: Whether the word was part of the gold standard (`GOLD_STANDARD`) or was labeled automatically (`AUTOMATIC`).

## Attribution
This data set is published under [Creative Commons Attribution 4.0](https://github.com/uds-lsv/lexicon-of-english-verbal-polarity-shifters/blob/master/LICENSE).

If you use it in your research or work, please cite the publication (see above).

### BibTex
```
@InProceedings{schulder2020shiftingdirections,
  author = {Schulder, Marc and Wiegand, Michael and Ruppenhofer, Josef},
  title = {Enhancing a Lexicon of Polarity Shifters through the Supervised Classification of Shifting Directions},
  booktitle = {Proceedings of the Twelfth International Conference on Language Resources and Evaluation (LREC 2020)},
  volume={1},
  year = {2020},
  month = {May},
  day = {11-16},
  address = {Marseille, France},
  publisher = {European Language Resources Association (ELRA)},
  language = {English}
}
```

## Acknowledgements
This work was partially supported by the German Research Foundation (DFG) under grants RU 1873/2-1 and WI4204/2-1.
