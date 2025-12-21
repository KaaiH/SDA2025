# README
## Structure and content of project
The code of this project is housed in the accompanying .ipynb file called notebook.ipynb.
The notebook is split up in multiple sections, with the first being dedicated to the processing and readying of the data used in the research. The other sections contain the research that was done for this project.

## Development process and section responsibility.
The development of the notebook started a bit as 4 small islands of code, original in a Google Collab notebook. However, we soon hit some limitations of that doctrine of working, and resorted to local notebook files, that were shared between each other via WhatsApp. This was far from a high level and coordinated development process, but with the amount of meetings we held to discuss our progress in the project, it worked very well in the end. Most of the research after all isolated. A problem appeared with each of us writing our own code to clean the data we used for the project. Kaai then merged all the work and made a centralized data cleaning section at the start of the notebook, with each person having a code cell dedicated to then adapting this central dataset to each research (This consisted mostly of renaming some columns to match personal preferences). 

## Quick external links

There is a high chance the project folder already contains all the files required.
These should be in the data/processed/ directory.
### Download data
#### Crime
The crime data can be downloaded from the following link:
https://opendata.cbs.nl/#/CBS/nl/dataset/83648NED/table?ts=1766081140268

#### Elections
The election data can be acquired at the following link:
https://www.verkiezingsuitslagen.nl/verkiezingen?s=Tweede+Kamer&v=2010&t=2024


After downloading the data, extract all csv files from their compressed state and
place them in the following directory: /data/raw.

The current directory should look like this:
notebook.ipynb
data/
    raw/
        files.csv

After running the notebook, the directory will update to the following:
notebook.ipynb
data/
    raw/
        files.csv
    processed/
        crime_provincial.csv
        crime_municipal.csv
        votes_provincial.csv
        votes_municipal.csv