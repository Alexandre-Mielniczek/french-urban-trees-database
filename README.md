# french-urban-trees-database
This repository provides a database for french urban trees based on open data.

# Database creation methodology
The database was built in May 2025 by compiling 11 open datasets from data.gouv.fr, representing more than 305,000 urban trees provided mainly by French cities and metropolitan areas (e.g., Paris, Lyon, Bordeaux, Nantes).

Processing steps:

Selection of attributes: relevant fields were identified (planting date/age, height, trunk diameter, species, location).

Standardization: units were harmonized (meters for height, centimeters for trunk diameter).

Age calculation: when only the planting date was available, age was estimated assuming trees are 1 year old at planting.

Cleaning: outliers and inconsistent values (e.g., negative ages, unrealistic diameters, null heights) were removed.

Taxonomy harmonization: species and genus names were normalized despite variations, typos, or mixed French/Latin naming; analysis was conducted at genus level to reduce uncertainty.

Location harmonization: spelling errors were corrected and locations were grouped into 13 standardized categories.


Coverage:

After filtering and cleaning, the database provides complete records (age, height, diameter) for 144,563 trees, nearly 10 times more than the McPherson reference database (~15,000 trees).

A subset of 71,281 trees includes all six key variables.

The dataset includes trees up to 400 years old, compared with 100 years in McPherson, expanding the temporal scope of allometric models.

This methodology ensures a robust and reproducible compilation of French urban tree data, suitable for calibrating and contextualizing growth models in LCA applications.

# french-urban-trees-database.xlsx
This file is a tabular export in Excel format.

The file has been cleaned as described in the methodology section above.
