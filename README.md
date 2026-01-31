# Smalltime
Literate documentation that explains how to translate the IANA tz source rules into a single table that contains enough information to translate a GPS timestamp with microsecond precision to and from local time zone and daylight saving time rules. In addition, code is provided to:
* Create a comprehensive SQL database that wraps around the main **timely** table. Full SQL code is supplied, with a detailed explanation. 
* Perl code (_small.pl_) that allows you to set up, test and interrogate the database, using a command-line interface.
* A Perl module (_Timely.pm_) that can be called to perform the translation of times between proleptic (extends into the past) GPS time and wall timestamps in Gregorian format.

## Requirements
1. You must have a basic grasp of SQL, or you will struggle.
2. You must be familiar with the command line in your operating system (e.g. Linux, Windows, Mac)
3. Detailed requirements are provided in the documentation, but you will need Perl, MySQL (with MySQL connector).  You will also need:
    * My literate LaTeX extraction script, [Dogwagger 4.05](https://github.com/jvanschalkwyk/dogwagger).  The literate source is available there too. 
* A recent copy of the [IANA tz database](https://www.iana.org/time-zones) with the ability to unzip the tar.gz file.
_Literate documents_ like those provided contain both the required documentation and all of the source code. They can be turned into PDF documents or a variety of code files, as required. The Dogwagger documentation explains in more detail. 

## Limitations 
If your Perl version is out of date (specifically the DateTime module) then there will be discrepancies between this and any more up to date version of tz. 

##Extras
As a convenience, the repository also contains documents and files derived from the literate .lyx files. These include PDF files, LaTeX .tex files, and the two Perl files in their relevant places in the directory structure provided. 
-----

