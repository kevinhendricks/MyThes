MyThes
======

Note: MyThes-1.0 has been subsumed by the Hunspell project.
This repo is here just to archive some older software I once wrote
back in the very early 2000's.


MyThes is a simple thesaurus that uses a structured
text data file and an index file with binary search
to lookup words and phrases and return information
on part of speech, meanings, and synonyms

MyThes was written to provide a thesaurus for the 
OpenOffice.org project 

The Main features of MyThes are:

1. written in C++ to make it easier to interface with 
   Pspell, OpenOffice, AbiWord, etc

2. it is stateless, uses no static variables and
   should be completely reentrant with no ifdefs  

3. it compiles with -ansi and -pedantic and -Wall
   with no warnigns so it shouldbe quite portable

4. it uses a simple perl program to read the structured
   text file and create the index needed for bianry
   searching

5. it is very simple with *lots* of comments.
   The main "smarts" are in the structure of the
   text file that makes up the thesaurus data

6. It comes with a ready-to-go structured thesaurus
   data file for en_US extracted from the WordNet-2.0 data.

   Please see WordNet_license.txt and WordNet_readme.txt
   for more information on the very useful project!
   

7. The source code has a BSD license (and  no advertising clause)


MyThes has the world's simplest Makefile and no 
configure support. It does come with a simple example 
program that looks up some words and returns meanings 
and synonyms.

To build it simply do the following:

unzip mythes.zip
cd mythes
make

To run the example program:
./example th_en_US_new.idx th_en_US_new.dat checkme.lst

Please play around with it and let me know
what you think.

Thanks,

Kevin Hendricks
kevin.b.hendricks@icloud.com (was kevin.hendricks@sympatico.ca)

   
