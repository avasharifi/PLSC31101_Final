# PLSC31101_Final
Final project for Computational Methods for Social Science
## Short Description
This project analyzes news articles from the Islamic Republic of Iran Broadcasting news articles which mention the United States. My intention was to scrape all articles from 1/1/2020 to 6/30/2020 from IRIB news which mention the United States. I first scraped 148 pages of search results with 50 articles per page. The corpus was made up of 9876 documents. I then parsed the text into title, subtitle, date, and text. I then translated the content, except for the date, from Persian to English.

While I intended to produce a dataframe of all 9876 documents, this was not possible because of the size of the corpus. As a result, I tested my code with a sample of 50 documents and created code that should run for the remainder of the corpus as well. 
## Dependencies
This project utilized
1. R, 4.0.2
2. Packages: tidyverse, rvest, stringr, purrr, googleLanguageR, utf8
## Files
1. Narrative.Rmd: Provides a narrative of the project, main challenges, solutions, and results.
2. Narrative.pdf: A knitted pdf of Narrative.Rmd.
3. Slides.pptx: My lightening talk slides
### Code
01_collect-links.R: Collects document links from all IRIB news articles and exports data to the file irib_doc_links.csv
02_scrape-docs.R: Scrapes relevant information from all news articles and exports data to the file sample.csv 
03_translate.R: Translates content from Persian to English
### Data
1. irib_doc_links.csv: Links to all 9876 documents in corpus
2. sample.csv: Dataframe using the first 50 documents in corpus
3. clean_sample.csv: Cleaned version of sample.csv
### Results
1. tr_sample.csv: Translated version of sample dataframe
2. cloud.png: Word cloud based on English translation of sample data
## More Information

