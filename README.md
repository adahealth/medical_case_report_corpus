# Medical Case Report Corpus
This repository contains a corpus of medical case reports with entity and relation annotations in BioC format.

## Corpus Format

The release format is a pickled BioC Json collection. You can process it with one of the many BioC libraries out there. 
The collection contains individual documents in its documents list. Each of the documents contains 1 passage with all the text and an annotation and relation list each.  
The annotations contain the locations of the annotation in the text. Each annotation looks like this:

```
id: 25412
{'origin': 'manual', 'key': UUID('ace40f78-9327-4ad9-a2f9-d4ef3ab127b2'), 'type': 'AdaEntity', 'entityType': 'finding'}
locations: 4299:23
text: ventricular tachycardia
```
## Corpus Statistics

The corpus statistics are summarized in the following Table:


## Reference

You can find the complete paper discribing the dataset and example scenarios on how it can be used here.
