# NPS Mortality Data Analysis

This project explores deaths reported in U.S. National Park Service (NPS) units and compares them with visitation to understand whether higher death counts correlate with visitation, or whether certain parks are outliers and seemingly more dangerous.

## How to Use
1. Clone this repository.
2. Install the required Python packages:  
   pip install -r requirements.txt
3. Open `NPS_mini_project.ipynb` in Jupyter Notebook or JupyterLab.


## Example Output
The analysis shows that drowning is the most frequent cause of death and several NPS units have many more deaths compared to other parks. Lake Mead specificly is an outlier with more than double the deaths than the next highest, Cape Hatteras. 


## Data Sources
- **NPS Mortality Data:** Publicly reported incidents in NPS units https://www.nps.gov/aboutus/mortality-data.htm

- **Park info & visitation:** NPS developer resources https://www.nps.gov/subjects/developer/get-started.htm

- **AI Usage**-The `manual_crosswalk` table used in this notebook was generated with the assistance of ChatGPT to minimize copy/paste and encoding errors in character-specific strings (e.g., *Haleakalā*, *Hawaiʻi*, *Wrangell–St. Elias*, “&” vs “and”, etc.). This helped prevent merge failures when normalizing park names.

 After generation, I manually verified every entry by comparing each `fullName`/`parkCode` against the official NPS website for accuracy. Any mismatches were corrected in the crosswalk file before use in the analysis.

The resulting file is saved as `parkname_manual_crosswalk.csv` and versioned in the repository. If an NPS unit is renamed or redesignated in the future, the crosswalk should be reviewed and updated accordingly.

-The project’s color palette (hex codes and ordered list) was assisted by ChatGPT to ensure consistent formatting and to streamline selection and presentation.

After generation, I manually verified each hex code and palette entry by comparing them against the reference palette published here:  
<https://siegal.bio.nyu.edu/color-palette/>

No discrepencies were found.

## Author
Jessica Long - Data Analysis Student

## License
MIT License