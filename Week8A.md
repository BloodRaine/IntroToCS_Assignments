Rosalind: http://rosalind.info/problems/subs/

Given two strings *s* and *t*, where *t* is a substring of *s* **IF** *t* is contained as a contiguous collection of symbols in *s* (as a result, *t* must be no longer than *s*).

The position of a symbol in a string is the total number of symbols found to its left within the string, including itself. (e.g. the position of all occurances of 'U' in "AUGCUUCAGAAAGGUCUUACG" are 2, 5, 6, 15, 17, and 18). The symbol at position *i* of *s* is denoted by  *s[i]*

A substring of *s* can be represented as *s[j:k]*, where *j* and *k* represent the starting and ending positions of the substring in *s*; for example if *s* = "AUGCUUCAGAAAGGUCUUACG", then *s[2:5]* = "UGCU".

The location of a substring *s[j:k]* is its beginning position *j*; **note** that the substring *t* may occur multiple times within the string *s* and will therefore have multiple positions.

**Input:** Two DNA strings *s* and *t* (each of length at most 1000 characters long).

**Output:** Total number of substrings *t* within *s* and all Locations of *t* as a substring of *s*

**Additional Requirement** Use the **.format()** function we learned in ZyBooks to output your answer. (Section 20.5 if you need help finding it)

# Sample Input
```
INPUT> Enter a DNA String S : GATATATGCATATACTT
INPUT> Enter a substring t: ATAT
```
# sample Output
```
OUTPUT> Total number of substrings found: 3, Locations in s: 2 4 10
```

**Note** Location **!=** Index, Index is 0 based while a location within an array may be 1 based.
