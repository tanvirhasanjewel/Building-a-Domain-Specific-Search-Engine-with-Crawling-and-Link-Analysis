# Building a Domain-Specific Search Engine with Crawling and Link Analysis

## Project Overview

This project implements a basic domain-specific search engine by:
- Crawling webpages from a selected domain
- Building an inverted index and web connection graph
- Implementing a search mechanism using PageRank or HITS

The project was developed as part of the Data Mining Lab (CSE 426) course at the University of Information Technology and Sciences (UITS).

## Submitted By
- **Name:** MD. Tanvir Hasan Jewel
- **ID:** 2125051038
- **Section:** 8A
- **Batch:** 50th
- **Semester:** Spring 2025
- **Department:** CSE

**Supervised By:**  
Mrinmoy Biswas Akash  
Lecturer  
Department of Computer Science & Engineering  
University of Information Technology and Sciences (UITS)  

**Date:** 06 July, 2025

## Project Structure

The project consists of several key components:

1. **Web Crawler**: Crawls specified seed URLs to collect domain-specific content
2. **Text Processing**: Cleans and tokenizes the collected content
3. **Indexing**: Builds an inverted index for efficient searching
4. **Link Analysis**: Implements PageRank algorithm for ranking pages
5. **Search Interface**: Provides search functionality based on the index and rankings

## Implementation Details

### Web Crawling
The crawler starts from seed URLs (primarily football/soccer-related websites) and follows links within the same domain, collecting webpage content.

### Text Processing
- Removes punctuation and stopwords
- Converts text to lowercase
- Tokenizes content for indexing

### Indexing
- Builds an inverted index mapping words to the URLs where they appear
- Creates a web connection graph showing links between pages

### Link Analysis
Implements PageRank algorithm to determine the importance of pages based on link structure.

## Requirements

- Python 3.x
- Required libraries:
  - requests
  - BeautifulSoup (bs4)
  - nltk
  - networkx
  - numpy
  - pandas

## Usage

1. Set up the seed URLs in the `seed_urls` list
2. Run the crawler with specified limits:
   ```python
   crawl_roots(seed_urls, crawl_limit=100, visit_limit=100)
   ```
3. After crawling, the inverted index and web connections will be available for searching

## Results

The project demonstrates:
- Successful crawling of domain-specific content
- Creation of an inverted index for efficient searching
- Implementation of PageRank for ranking pages
- Basic search functionality based on the collected data

## Future Work

Potential improvements include:
- Enhancing the search interface
- Implementing more sophisticated ranking algorithms
- Expanding the domain coverage
- Improving performance and scalability

## License

This project is licensed under the MIT License `https://github.com/tanvirhasanjewel/Building-a-Domain-Specific-Search-Engine-with-Crawling-and-Link-Analysis.git`.
