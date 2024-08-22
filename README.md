# genomic-alignment-extraction

- A scalable large scale genomic fraction aligner and extractor for the large scale alignment of the genomes and the transcriptomes and process them over the cores for the extraction of the aligned regions.
- The aligned regions can also be mapped to the length plotter and can be machine trained for specific applications.
- This repository contains two codes one for the one-one genome alignment and extractions and it is used for one reference genome and one target genome and the other code in which you can have one target genome and as many as reference genomes you want.
- In case of the one genome one target, such as bacterial or the organell genome alignments, it provides the target genome start, end, reference genome start end and also corrdinates and reverse corrdinates and sequences.
- In case of the one 2 many genome, such as a specific transcript alignment to the larger database of the transcripts, or genome, it provides, the target start, end, cordinates, sequences and returns a list of lists with the named tuple as the referencename, sequenceextracted.

```
def genomeExtraction(alignmentgenome = FALSE,
                          reference_genome = FALSE,
                                 target_genome = FALSE,
                                    percent_match = FALSE):
    """
    Function: genomeExtraction
    Summary: this will take the genome alignment file in the format given below from
    the lastz or the blast alignments and then will extract the reference and the target
    genome regions. It will extract from both the positive and the negative strand and in
    the case of the negative strand it reverses the sequences. It also provides the option
    for the filtering according to the given percentage match and also writes all the coordinates
    and the sequences as tab delimited files.
    Examples:
        genome  query_size  aligned_start   aligned_end matches mismatches  %_aligned   %_matched   chromosome  strand  start   end
0   taeGut2 8000    1   8000    7788    60  100 97.35   chr1    +   5637454 5646796
1   taeGut2 8000    6295    7425    1095    22  14.14   96.82   chr1    +   5642077 5643357
2   taeGut2 8000    6332    6383    45  4   0.65    86.54   chr1    -   1365309 1365357
3   taeGut2 8000    6351    6387    34  1   0.46    91.89   chr1   +   2096236 2096628
4   taeGut2 8000    6351    6383    31  2   0.41    93.94   chr1    +   7208240 7208272
5   taeGut2 8000    6357    6383    26  1   0.34    96.3    chr1   -   3293331 3293357
6   taeGut2 8000    3498    3526    25  1   0.36    86.21   chr1   -   71676009    71676034
7   taeGut2 8000    3602    3624    22  1   0.29    95.65   chr1   +   12695042    12695064
    Attributes:
        @param (multilevelgenome) default=FALSE: InsertHere
        @param (splitgenome) default=FALSE: InsertHere
    Returns: InsertHere
```

Gaurav Sablok \
University of Potsdam \
Potsdam,Germany
