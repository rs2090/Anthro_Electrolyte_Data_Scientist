# Anthro Interview - Staff Battery Scientist 

## The repo consists of examples of topics discussed in the  points. 

### Natural Language processing 
 1. Scraping the internet for Journals and patents to understand trials conducted
 2. Using unpaywall to get a list of legally available pdfs
 3. Go through each pdf and split it into sections like formulation and metric
 4. Each PDF is then searched line by line looking for standard electrolyte formulation formats defined with the regex compiler
 5. Formulations arebroken up to meaningful bits
 6. Metrics are connected to formulations based on distances or alliase matches
 7. 4 tables are generated
    - Formulation
      - Solvent
      - Additives
      - Metrics
 8. These are then flattened and added to a single table and pivoted for whatever the user  needs. The system also insters these  tables to PSQL database which holds these results so repeated API calls need not be made.
 9. The flattened table  can also be used as input to Machine learning protocols. If the addtion of SMILES is made to vectorise each one of the components
 
