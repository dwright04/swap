SWAP
=========

Repository for the SWAP implementation used in:

A transient search using combined human and machine classiﬁcations


The main function is messy with tests and plots for the paper.
The SWAP object is probably most useful, but is currently tightly 
bound to my specific database and schema.  It should be fairly easy
to alter and substitute in the relavant calls to your own database
or loop through a csv.

## MATSWAP

The MATSWAP object implements SWAP to process this .mat file:

[SNHunters_classification_dump_20170109.mat](https://www.dropbox.com/s/0sjkfhbxocnkbbb/SNHunters_classification_dump_20170109.mat?dl=0)

## Usage Example

Process the .mat file:

```python
from swap import MATSWAP
swap = MATSWAP("SNHunters_classification_dump_20170109.mat")
swap.process()
swap.save("swap_SNHunters_classification_dump_20170109.mat")

``` 
