# Calculate and visualise a score of how resourceful it is for 350+ regions in Greater Sydney

**Co-contributor:** Myra Rebecca Jia Min Wong

Australia is formally defined by more than $2000$ ”Statistical Area Level 2” (SA2) distinct geographical regions, designed to represent communities of between $3000-25000$ people ”that interact together socially and economically”. This project focuses on the $350+$ SA2s within the Greater Sydney area, aiming to calculate and visualised a score for how ”well-resourced” each region is by spatially integrating several datasets of various formats.

## Tasks

1. Wraggled $9$ data sets of various formats (txt, json, csv, etc.) including shapefile (geo-spatial data) using Python in Jupyter Notebook; 
2. Imported all datasets into PostgreSQL server using a well-defined data schema;
3. Using SQL queries to incorporate and spatially join all datasets, computed the "resourceful" score for $350+$ SA2 regions:
   $$\text{Score} = S(z_{retail} + z_{health} + z_{stops} + z_{polls} + z_{schools}- z_{homeless} + z_{internet})$$
   where $S$ is the [sigmoid function](https://en.wikipedia.org/wiki/Sigmoid_function).
5. Summarised the results and visualized them using overlay maps;
6. Investigated the correlation between calculated "resourceful" score and SA2 regions' median incomes.
