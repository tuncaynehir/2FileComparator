# 2FileComparator

## Functionality
Given f1.txt and f2.txt with words separated by lines makes a new file output.txt that contains all the matching words.


## Project Overview
This project implements a custom alphabetical hash table that efficiently stores, compares, and sorts words from text files by grouping them into buckets based on their first letter . Each bucket dynamically resizes using manual memory allocation, ensuring minimal initial memory use and efficient growth as words are added. 

After building the first hash table from one file, the program checks a second file and collects all words that appear in both, storing them in a separate hash table. To organize the common words, each bucket is sorted using heap sort, chosen for its consistent worst-case performance.

Finally, the sorted results are written to an output file, producing an alphabetically ordered list of all shared words.


## Features
- Custom alphabetical hash table with 26 buckets (A–Z)
- Manual dynamic memory allocation with automatic resizing
- Heap sort implemented per bucket for consistent performance
- Produces an alphabetized list of shared words

## How to Run?
g++ -std=c++11 filewordcomparator.cpp -o comparator
./comparator
