# BratMerger #


## Introduction

This project is about merging the annotations in BRAT and 

This script was used to merge the annnotations 


## Directory structure

- [**`Script/`**](Script/): 

  - [**`merger.py`**](Script/merger.py): Merge the annotations ([Annotated section headers](root/documents/ANN_SECTION) that generated by [Header Detector](https://github.com/siabar/EHR-HeaderDetector-AnnotationAnalyser) with
    [pre-annotated variables](documents/ANN_VARIABLE) that generated by [SpaCTeS tool](https://github.com/siabar/SpaCTeS)) in BRAT format.
    Output of this script is in [ANN_FINAL](documents/ANN_FINAL) directory.

- [**`documents/`**](documents/)
  - [**`ANN_SECTION/`**](documents/ANN_SECTION/): Output of [Header Detector](https://github.com/siabar/EHR-HeaderDetector-AnnotationAnalyser) project and input for merger.py script.
  - [**`ANN_VARIABLE/`**](documents/ANN_VARIABLE/): Output of [SpaCTeS tool](https://github.com/siabar/SpaCTeS), which is ANN files and input for merger.py script.
  - [**`ANN_FINAL/`**](documents/ANN_FINAL/): Outout of concatenate.py script.

## Usage

**For merging the annotations in BRAT, use follwoing command:**

    python3 merger.py [options] 

Options:
<pre>
--set       Number of bunch [For example: 01]
</pre>


## Contact

Siamak Barzegar (siamak.barzegar@bsc.es)