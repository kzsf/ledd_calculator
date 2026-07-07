##### Last Updated: July 7, 2026
---



# ledd calculator 
Calculates ledd from `PD Medications - LED Calculation` instrument in the Z1XADRCNACC Database.
### Instructions:

1.  Export the instrument `PD Medications - LED Calculation` from Z1XADRCNACC Database as a CSV file (raw labels).
2.  Update paths.yaml file with your desired calculator input (location of your saved PD Medications export) and calculator output (calculated ledd data) file paths.
3.  Run each code chunk. Output ledd csv will be saved under the path name specified in step 2.
---
# ledd cleaner
Subsets and cleans ledd output from calculator based on your subject list.
### Instructions:

1.  Use ledd calculator and obtain output ledd data.
2.  Update paths.yaml with your cleaner output file path.

- required input files:
  - `calculator_output_file`: ledd output data from ledd_calculator.qmd
  - `subj_list`: subject list of adrc_id's of interest
- output:
  - `cleaner_output_file`: cleaned ledd dataframe with only subjects of interest

3.  Run each code chunk. Output will be saved under `cleaner_output_file` path specified in step 2.
