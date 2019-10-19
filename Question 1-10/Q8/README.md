# Problem</br>

Supervin is a librarian handling an ancient book with N pages, numbered from 1 to N. Since the book is too old, unfortunately M pages are torn out: page number P1, P2, ..., PM.</br>

Today, there are Q lazy readers who are interested in reading the ancient book. Since they are lazy, each reader will not necessarily read all the pages. Instead, the i-th reader will only read the pages that are numbered multiples of Ri and not torn out. Supervin would like to know the sum of the number of pages read by each reader.</br>

## Input</br>

The first line of the input gives the number of test cases, T. T test cases follow. Each test case begins with a line containing the three integers N, M, and Q, the number of pages in the book, the number of torn out pages in the book, and the number of readers, respectively. The second line contains M integers, the i-th of which is Pi. The third line contains Q integers, the i-th of which is Ri.</br>

## Output</br>

For each test case, output one line containing Case #x: y, where x is the test case number (starting from 1) and y is the total number of pages that will be read by all readers.</br>

# Sample</br>

## Input</br>

3
11 1 2
8
2 3
11 11 11
1 2 3 4 5 6 7 8 9 10 11
1 2 3 4 5 6 7 8 9 10 11
1000 6 1
4 8 15 16 23 42
1

## Output</br>

Case #1: 7
Case #2: 0
Case #3: 994

## Explanation</br>

In sample case #1, the first reader will read the pages numbered 2, 4, 6, and 10. Note that the page numbered 8 will not be read since it is torn out. The second reader will read the pages numbered 3, 6, and 9. Therefore, the total number of pages that will be read by all readers is 4 + 3 = 7.</br>

In sample case #2, all pages are torn out so all readers will read 0 pages.</br>

In sample case #3, the first reader will read all the pages other than the six given pages.</br>