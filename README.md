# Defining an Open Platform
The Apperta Foundation is a not-for-profit community interest company supported by NHS England and NHS Digital (HSCIC) 

They produced a document called “Defining an Open Platform” to make the case for open platforms and lay out a blueprint for an open platform architecture at a level of detail that would allow any willing party to build a first generation implementation of an open platform that would be interoperable with any other.

## Goal

## Getting started

## References

[How to Convert a PDF File to Editable Text Using the Command Line in Linux](https://www.howtogeek.com/228531/how-to-convert-a-pdf-file-to-editable-text-using-the-command-line-in-linux/)

Extract text from each page to a file

`for i in {1..48}; do pdftotext -f $i -l $i Apperta_Defining_an_Open_Platform_SP.pdf Apperta_Defining_an_Open_Platform_SP-nolayout-p$i.txt; done`
