# EPAM - Elementary Perceiver and Memorizer

**Title**: An Information Processing Theory Of Verbal Learning  
**Author**: Edward A. Feigenbaum, The RAND Corporation, Mathematics
Division  
**Ref**: P-1817  
**Date**: 9 October 1959  
**Source**:
[Bitsavers](http://bitsavers.org/pdf/rand/ipl/P-1817_Feigenbaum_EPAM_Oct59.pdf)  

> This paper presents a theory of some elementary forms of human symbolic learning — memorization, discrimination, association, and attention direction. This theory is concerned with mental activity at the level of the processing of information symbols, which are the basic units manipulated.

> The precise statement of the theory is given in the language of a digital computer, specifically as a set of programs in IPL-V, called EPAM.

> The paper deals generally with information structures and processes for discrimination and association learning, and specifically with behavior in the standard rote learning task. A number of implications of the theory in rote learning situations are explored; comparisons are drawn between the behavior of human subjects in these situations and the behavior of the EPAM model.

## Code extraction

The code listing in the report on pages 142-70 has been extracted. It
is available in three formats:

- [EPAM.txt](./EPAM.txt) - original card image format
- [EPAM.liplv](./EPAM.liplv) - s-expressions, suitable for Jeff Shrager's IPL-V
  interpreter in Lisp at [jeffshrager/IPL-V/](https://github.com/jeffshrager/IPL-V/)
- [EPAM.tsv](./EPAM.tsv) - tab-separated columns for easier viewing in
 a spreadsheet

## Known issues

The following line in the source PDF

```
     ZERO INTEGER                        +N   0 01 0000  0000            N   01 
```

has a `+` in column 42, but the IPL-V specification says this column
should always be blank. This has been preserved in the card-image file
but has been removed from the tsv and liplv versions.
