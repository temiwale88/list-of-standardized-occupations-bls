# Project overview

This project aims to normalize occupation data from the [U.S. BUREAU OF LABOR STATISTICS](https://www.bls.gov/emp/tables/emp-by-detailed-occupation.htm) (BLS). An initial review of their tool seems to display a pivoted list of employment occupations / industry, employment categories, and corresponding employment titles. What we might want is the employment titles (third level of detail), with their corresponding occupation categories (second level summary), and occupations / industries (first level summary). For some occupations, we will find additonal levels but a visual inspection of the file suggests that going down three levels is enough. ***#Inception***!

You can clone this folder to your workspace  
`git clone https://github.com/temiwale88/list-of-standardized-occupations-bls`

You project tree will most likely look like this: 
``` 
Employment
├─ employment_parser.ipynb
├─ README.md
└─ Resources
   ├─ Cleaned_BLS_Employment_Categories.csv
   └─ occupation.xlsx
```

The final output (and most likely what you need) is the `Cleaned_BLS_Employment_Categories.csv` file in the **Resources** folder.

*Optional*:  
See the `employment_parser.ipynb` for informative notebook on how this was created.  
Feel free to modify to code to make it cleaner and more meaningful where possible! Nonetheless, this should be a good starting point.

## Potential use cases

This might be useful for some tasks including:  

- Building an application with a form that requests employment title from end users. This allows you to standardize your employment database with nationally recognized titles and their respective industries or "occupations".
- Fuzzy matching existing job titles in your employment database with the BLS employment titles so as to categorize these into their respective recognized industries.