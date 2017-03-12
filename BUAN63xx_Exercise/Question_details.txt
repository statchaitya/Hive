Enter your code into the placeholder files provided in the scripts directory. Please do not create additional files. You must do everything in the files provided.
I will grade each one by running 'hive -f filename.hive' and checking the results, in the sandbox.
Triple check that your queries execute successfully with 'hive -f' from the command-line. 
If they don't execute, they'll get a 0.
Don't modify the filenames, files, or directory structure.

Part 1 - Table Creation
Use the 3 provided csv files in the data directory to create 6 hive-managed tables.
total_pop_text (Populate hive table with zip_totpop.csv; hive table stored as text file format)
female_pop_text (Populate hive table with zip_femalepop.csv; hive table stored as text file format)
male_pop_text (Populate hive table with zip_malepop.csv; hive table stored as text file format)

total_pop_orc (total population data stored as ORC file format)
female_pop_orc (female population data stored as ORC file format)
male_pop_orc (male population data stored as ORC file format)

1. Which zip codes are missing from the male population table, compared to the total population table?
2. Which zip codes are missing from the female population table, compared to the total population table?
3. What are the 3 zip codes with the largest total population, sorted from lowest to highest?
4. What are the 3 zip codes with the smallest male population, sorted from lowest to highest? 
5. What are the 3 zip codes with the smallest female population, sorted from lowest to highest?
6. What is the average total population across all zip codes?
7. What is the average female population across all zip codes?
8. What is the average male population across all zip codes?
9. Which 5 zip codes have the greatest difference between the male and female populations? List the zip code and difference for each of the 5.
10. What is the average total population for zip codes that start with 75?
11. What is the average male population for zip codes that start with 75?
12. What is the average female population for zip codes that start with 75?
13. Write a query that prints the total population for each zip code that starts with 2, 8, and 9, from lowest total population to highest total population.
The results should look like this, but not necessarily in the exact same order:
FirstNumber     TotalPop
2               <your results here>
8               <your results here>
9               <your results here>
Make sure you get the column names exactly as listed (FirstNumber, TotalPop). Only for 2, 8, 9.

14. Create a VIEW that has zip, totalpop, malepop, and femalepop as the columns.

15. Create a VIEW exactly like 14, except it will never show data for counties that start with a 7 or a 9.

16. Build a script just like you did for 13, but let me pass in, from the command-line, the number that I want data for. 
For example, if I pass in 8, it will print out the total population of all counties that start with the number 8. And only for 8 (or whichever number I pass in).

17. Write a query that prints the total number of records for the two starting characters of each zip code.
The results should look like the following, except it should include a line for each unique 2-letter start to a zip code.:
FirstTwo            NumberOfZipCodes
75                  <number of zips that start with 75>
90                  <number of zips that start with 90>
99                  <number of zips that start with 99>>
Make sure you get the column names exactly as listed.

5 pt bonus: When you do a join to find rows that don't exist (as in 1 & 2), instead of NULL have the missing values replaced with "NOT FOUND". There is still only a max of 100, but you can attempt to recover other possibly lost points with this bonus.

Enter your code into the placeholder files provided in the scripts directory. Please do not create additional files. You must do everything in the files provided.
