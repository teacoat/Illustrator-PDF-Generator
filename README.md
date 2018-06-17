# Illustrator-PDF-Generator

A backup of the process to generate PDF's based on CSV data. I did not make this.

Instructions taken from: https://graphicdesign.stackexchange.com/questions/57751/adding-individual-guest-names-to-a-wedding-invitation-in-illustrator/57753

----

Load the data
First the hard part, reading the data from the excel file. Unfortunately, Adobe Illustrator does not support CSV files for a data source. They do, read XML though. Fortunately, Prepression has been kind enough to write a Illustrator script that does this for you. The script is called VariableImporter. With this tool at hand let us begin:

Save your excel table as a CSV or TSV file.
Read the data in with VariableImporter.
The script is a bit temperamental but test a few things first.

Make the image dynamic
Open the variables window from Window → Variables.
Select your text object that you want to change.
In variables window click the make text dynamic button with suitable data column selected.

Make text dynamic

Image 1: Make text dynamic on selected text.

You can now test the different record in action. Data in set

Image 2: Test dataset.

Repeats 1-3 steps until you have all you want to change.

Export each variable as a PDF.
To export the data sets into multiple pdf files do this:

Make a new action where you save a pdf document.
From the menu in Actions window corner, select Batch...

batch

Image 3: Export the data sets to individual PDF files.

Set the source to Data Sets, Override save commands, and a folder.
