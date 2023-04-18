# DataCleaning_SharkAttack
  ![shark_attack_cover](https://raw.githubusercontent.com/vdechen/DataCleaning_SharkAttack/main/images/shark_attack_cover.png)
 
# Project Goal and Description
  This project aimed at cleaning the "Global Shark Attacks" dataset (https://www.kaggle.com/datasets/teajay/global-shark-attacks) in order to analyze the fatality incidence in the records and the profile of these fatal attacks considering the 'sex', 'age', 'country' and 'year' information provided. 
  
# Technologies 
  - Python
  - Pandas
  - Numpy

# Steps
  1. The original dataset was made of 25723 lines and 24 columns. After cleaning lines with over 22 null values in them, it was left with 6302 lines for the analysis.
  2. The 'fatal', 'sex' and 'age' columns were cleaned. Unwanted categories and specific errors that represented less than 1% of data were turned into nulls or replaced by a small correction.
  - The 'fatal' column was left with 'y', 'n' and null values.  
  - The 'sex' column was left with 'm', 'f' and null values. 
  - The 'age' column was left with float and null values. If there were uncertain age values for a single person, the average of the values was used. If the record contained ages for more than a victim, each age turned into a different line and information from other columns were duplicated. The dataset ended up with 6332 lines.
  - The 'age_groups' column was created to classify ages in the following intervals: 0-9, 10-19, 20-29, 30-39, 40-49, 50-59, 60-69, 70-79, 80-87.
  3. Data frames were created to analyze the total values and percentages of categories for these columns: 'fatal', 'sex', 'age_groups', 'fatal X sex', 'fatal X age_groups'.
  4. The 'country' and the 'year' columns were grouped by the 'fatal' column and the frequency of their values.   

# Conclusion
  From the lines of 6332 records: 
   - Most attacks are not fatal (75.6% from 90.16% not nulls)
   - Most fatal cases happen among males (22.44% from 82.83% not nulls)
   
   ![fatality_sex](https://raw.githubusercontent.com/vdechen/DataCleaning_SharkAttack/main/images/fatality_sex.png)
   
   (t% = total percentage, compared to all cases; r% = relative percentage, compared to cases from that group)
   
   - Most fatal cases happen among ages 10-29 (over 65% from 50.55% not nulls)
   
   ![fatality_age](https://raw.githubusercontent.com/vdechen/DataCleaning_SharkAttack/main/images/fatality_age.png)
   
   (t% = total percentage, compared to all cases; r% = relative percentage, compared to cases from that group)
   
   - The top 10 countries for fatal attacks are Australia, USA, South Africa, Papua New Guinea, Mexico, Brazil, Philippines, Reunion, New Zealand and Cuba
   
      ![top10_countries](https://raw.githubusercontent.com/vdechen/DataCleaning_SharkAttack/main/images/top10_countries.png)
      
       (country X total number of cases)
   
   - The top 10 years for fatal attacks since 1960 are 2000, 1944, 1993, 1942, 1964, 1962, 1966, 1963, 1954 and 1960
   
      ![top10_years](https://raw.githubusercontent.com/vdechen/DataCleaning_SharkAttack/main/images/top10_years.png)
   
# Contact
- LinkedIn: vanessadechen
- GitHub: /vdechen
- Email: vanessadechen@gmail.com
