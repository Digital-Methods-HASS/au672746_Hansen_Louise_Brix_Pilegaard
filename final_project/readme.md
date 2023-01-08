# Topic Modeling on Popular Music Lyrics From 1982-2022

This folder contains the code, data and report for the exam project "Topic Modeling on Popular Music Lyrics from 1982-2022". 

## File- and metadata descriptions
**billboard_scrape.Rmd**: This markdown contains the code to scrape data from the Billboard Hot 100 chart from several weeks of 1982, 2002 and 2022. It also containts the data to scrape the lyrics to these songs from genius.com. **NOTE**: running this script requires the creation of an API client to genius.com. An API client token is personal, and mine can therefore not be shared for this project. To run the code on your own machine, a personal token can be made at https://genius.com/api-clients. This token must be saved in an .Renviron file in the correct directory on your machine (see https://stackoverflow.com/questions/40788645/how-to-create-renviron-file for different solutions for Windows, Linux and Mac) and activated in the R-script (code is provided for this in the script)

**billboard_tm.Rmd**: This markdown contains the code to apply Topic Modeling to the data from the **billboard_scrape.Rmd** markdown.

**lyrics_1982.csv**, **lyrics_2002.csv**, and **lyrics_2022.csv**: CSV files containing the lyrics from the Billboard charts from 1982, 2002 and 2022. These files stem from running the .Rmd file “billboard_scrape.Rmd”. HOWEVER; using functions from the geniusr package resulted in some random errors (i.e., it was not always the same songs that resulted in errors). So, to replicate the exact findings of this project, you must run the Topic Modeling analysis found in the “billboard_tm.Rmd” script using these three CSV files. Furthermore, as obtaining the lyrics to all the songs is extremely time consuming, and it will take a long time to run **billboard_scrape.Rmd**, using these files is recommended.
