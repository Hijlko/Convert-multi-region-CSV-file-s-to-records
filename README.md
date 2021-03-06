# Convert-multi-region-CSV-file-s-to-records
Modification of ConvertCSVtoRecords from ForcePanda/Narender Singh te be able to read multi region CSV files

I downloaded the package for converting CSV files to records created by Narender Singh
. I found it very usefull but had to change the apex code to be able to import CSV files of the European region. Standard US csv uses a comma as a field separator while most European csv's use a semicolon as a field seperator. There are more diferences between the regions.
Date: YYYY-MM-DD for US and SalesForce standard but DD-MM-YYYY for European standard
Thousand/decimal separator: In US the point is used as a decimal separator an a comma as a thousands separator.
In Europe a comma is used as a decimal separator and a point as thousands separator.

That's why I made some changes to the code/componet so you're able to set the

field separator
Thousand seperator
Decimal Separator and
Currency symbol
The code can now import muli region CSV files
Numbers/currency like 1,2345.56 (US) and 1.234,56 (EU) are converted to 1234.56
Date like YYYY-MM-DD and DD-MM-YYYY (and other separators like YYYY/MM/DD and DD/MM/YYYY) are always converted to YYYY-MM-DD

I'm very new to APEX coding so maybe it can be coded in a better way but it works for me. Maybe you can check it out.

[ConvertAllCSVToRecords.txt](https://github.com/Hijlko/Convert-multi-region-CSV-file-s-to-records/files/6096138/ConvertAllCSVToRecords.txt)
