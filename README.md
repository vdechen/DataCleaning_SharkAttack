# DataCleaning_SharkAttack
  Project status(Active)
  
# Project Objective and Description
  This data analysis aimed at cleaning the "Global Shark Attacks" dataset (https://www.kaggle.com/datasets/teajay/global-shark-attacks) in order to analyse the fatality incidence in the records and the profile of these fatal attacks considering the 'sex', 'age', 'country' and 'year' information provided. 
  
# Technologies 
  - Python
  - Pandas
  - Numpy

# Steps
  1. The original dataset was made of 25723 lines and 24 columns. After cleaning lines with over 22 null values in them, it was left with 6302 lines for the analysis.
  2. The 'fatal', 'sex' and 'age' columns were cleaned. Unwanted categories and specific errors that represented less than 1% of data were turned into nulls or replaced by a small correction.
  - The 'fatal' column was left with 'y', 'n' and null values.  
  - The 'sex' column was left with 'm', 'f' and null values. 
  - The 'age' columns was left with float and null values. If there were uncertain age values for a single person, the average of the values was used. If the record contained ages for more than a victim, each age turned into a different line and information from other columns were duplicated. The dataset ended up with 6332 lines.
  - The 'age_groups' column was created to classify ages in the following intervals: 0-9, 10-19, 20-29, 30-39, 40-49, 50-59, 60-69, 70-79, 80-87.
  3. Data frames were created to analyse the total values and percentages of categories for these columns: 'fatal', 'sex', 'age_groups', 'fatal X sex', 'fatal X age_groups'.
  4. The 'country' and the 'year' columns were grouped by the 'fatal' colum and the frequency of their values.   

# Conclusion
  From the lines of 6332 records: 
   - Most attacks are not fatal (75.6% from 90.16% not nulls)
   - Most attacks involve male victims (88.9% from 90,95% not nulls)
   - The attacks frequency decreases with age increase, except for young children between 0-9 (from 54,4% not nulls)
   - The mean age of the attacks was 27.4 years old 
   - Most fatal cases happen among males (22.44% from 82,83% not nulls)
   - Most fatal cases happen among ages 10-29 (over 65% from 50,55% not nulls)
   - The top 10 countries for fatal attacks are Autralia, USA, South Africa, Papua New Guinea, Mexico, Brazil, Philippines, Reunion, New Zealand and Cuba
   - The top 10 years for fatal attacks since 1960 are 2000, 1944, 1993, 1942, 1964, 1962, 1966, 1963, 1954 and 1960
   
# Contact
- LinkedIn: vanessadechen
- GitHub: /vdechen
- Email: vanessadechen@gmail.com
