# ElectionAnalysis

Analyzing data from 2014 Hungarian National Elections. Performed exploratory analysis with pandas, found districts with anomalous number of invalid votes. Verified validity of Benford’s law for distribution of digits, indicating the numbers are not human-generated.

Interesting results are in StatisticalAnalysis.ipynb: 

A. Checking independence of voter turnout and percentage of votes for certain parties: textbook-Gaussian for FIDESZ (winning party); minor elongation effects for rest of the parties, likely due to positive correlation between voter turnout and popularity of MSZP and LMP in urban areas

B. Checking fit of Benford's law on 3rd and 4th digits with chi-square testing: found good agreement between election numbers and theoretical distribution.

The other files are for:

1. DownloadData.ipynb: Script to download html files from public websites, requires minor interaction.

2. ExtractData.ipynb: Extracting key data from individual text files & saving it to a csv file (resulting csv file included: electoral.csv).

3. VisualizeData.ipynb: Doing sanity checks and initial analysis. Found minor signs of fraud in a few individual districts.


