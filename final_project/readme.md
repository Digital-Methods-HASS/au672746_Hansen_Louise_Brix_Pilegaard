# Topic Modeling on Popular Music Lyrics From 1982-2022

This folder containts the code, data and report for the exam project "Topic Modeling on Popular Music Lyrics from 1982-2022". 

**billboard_scrape.Rmd**: This markdown containts the code to scrape data from the Billboard Hot 100 chart from several weeks of 1982, 2002 and 2022. It also containts the data to scrape the lyrics to these songs from genius.com

**billboard_tm.Rmd**: This markdown contains the code to apply Topic Modeling to the data from the **billboard_scrape.Rmd** markdown.

**lyrics_1982.csv**, **lyrics_2002.csv**, and **lyrics_2022.csv**: CSV files containing the lyrics from the Billboard charts from 1982, 2002 and 2022. These files stem from running the .Rmd file “billboard_scrape.Rmd”. HOWEVER; using functions from the geniusr package resulted in some random errors (i.e., it was not always the same songs that resulted in errors). So, to replicate the exact findings of this project, you must run the Topic Modeling analysis found in the “billboard_tm.Rmd” script using these three CSV files.
