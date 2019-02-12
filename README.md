BioNLP-OST corpus pre-processing with AlvisNLP

## Preprocessing tools

* Tokenization and sentence splitting
* Abbreviations (Ab3P)
* POS-tagging and lemmatization (GeniaTagger)
* Stemming
* NER
  * Generic (Stanford)
  * Chemicals (Chemspot)
  * Genes and Proteins (GeniaTagger)
* Term extraction (YaTeA)
* Dependency parsing (CCG, Enju and Stanford)
* Ask for more, we may have something in store...

## Prerequisites

### Mandatory

* [AlvisNLP](https://github.com/Bibliome/alvisnlp)

### Optional tools (depending on which is necessary)

* [GeniaTagger](http://www.nactem.ac.uk/GENIA/tagger/)
* [CCG Parser](http://groups.inf.ed.ac.uk/ccg/software.html)
* [Enju Parser](http://www.nactem.ac.uk/enju/)
* [Chemspot](https://github.com/rockt/ChemSpot)
* [Ab3P](https://github.com/ncbi-nlp/Ab3P)
* [YaTeA](https://metacpan.org/pod/Lingua::YaTeA)

**Or**

You can use the all-included docker image.


## File formats

### Input

AlvisNLP supports [several input formats](https://bibliome.github.io/alvisnlp/reference/Module-reference#readers) including: text, BioNLP-ST, PubTator, I2B2.

Reading particular XML files require to write a connector with XSLT.

### Output

Tabular text files. We can also export in XML^*, RDF^*, PubAnnotation JSON.

^* requires to write a connector.
