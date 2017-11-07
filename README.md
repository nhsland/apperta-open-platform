# apperta-open-platform

## Goal

## Getting started

## References

[How to Convert a PDF File to Editable Text Using the Command Line in Linux](https://www.howtogeek.com/228531/how-to-convert-a-pdf-file-to-editable-text-using-the-command-line-in-linux/)

Extract text from each page to a file

`for i in {1..48}; do pdftotext -f $i -l $i Apperta_Defining_an_Open_Platform_SP.pdf Apperta_Defining_an_Open_Platform_SP-nolayout-p$i.txt; done`
