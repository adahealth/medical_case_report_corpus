# Medical Case Report Corpus
This repository contains a corpus of medical case reports with entity and relation annotations in BioC format.

We present a new corpus comprising annotations of medical entities in case reports, originating from PubMed Central’s open access library. In the case reports, we annotate cases, conditions, findings, factors and negation modifiers. Moreover, where applicable, we annotate relations between these entities. As such, this is the first corpus of this kind made available to the scientific community in English. It enables the initial investigation of automatic information extraction from case reports through tasks like Named Entity Recognition, Relation Extraction and (sentence/paragraph) relevance detection. Additionally, we present four strong baseline systems for the detection of medical entities made available through the annotated dataset.

## Corpus Format

The release format is a pickled BioC Json collection. You can process it with one of the many BioC libraries out there. 
The collection contains individual documents in its document list. Each of the documents contains 1 passage with the text of one case report  and an annotation list and relation list each.  
The annotations contain the locations of the annotation in the text. Each annotation looks like this:

```
id: 25412
{'origin': 'manual', 'key': UUID('ace40f78-9327-4ad9-a2f9-d4ef3ab127b2'), 'type': 'AdaEntity', 'entityType': 'finding'}
locations: 4299:23
text: ventricular tachycardia
```
## Corpus Statistics

The corpus statistics are summarized in the following Table:
![statistics](https://github.com/adahealth/medical_case_report_corpus/blob/master/docs/corpus_stats.png "Corpus Statistics")


## Reference

You can find the complete paper discribing the dataset and example scenarios on how it can be used [here](https://github.com/adahealth/medical_case_report_corpus/blob/master/docs/Medical_Entities_in_Case_Reports.pdf).
The corpus can be used under Creative Common Licenses. If you use it, please cite our paper.
