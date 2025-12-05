
### Geographic Data
- **German Administrative Boundaries**
- Source: geoBoundaries Project
- File: `geoBoundariesSimplified-3_0_0-DEU-ADM2.shp`
- Used for mapping crime distribution across German cities and districts

## Data Format

### Crime Data Files
Each CSV file should contain the following columns:
- `Straftat`: Crime type/category (German legal descriptions)
- `Stadt`: City name
- `Total`: Total number of victims/cases
- Additional columns for specific crime subcategories

### Expected Crime Categories
The dashboard processes these main crime types:
- Sexual offenses (Vergewaltigung, sexuelle Nötigung)
- Robbery and extortion (Raub, räuberische Erpressung)
- Assault (Körperverletzung)
- Theft (Diebstahl)
- Property damage (Sachbeschädigung)
- Drug offenses (Rauschgiftdelikte)
- Homicide (Mord, Totschlag)

## Data Privacy & Usage

- All data is anonymized and aggregated
- Contains no personal identifying information
- Used for statistical analysis and visualization only
- Complies with German data protection laws

## How to Add New Data

1. Place new CSV files in the `raw/PKS/Opfer/` directory
2. Follow the naming convention: `YYYY Opfer.csv`
3. Ensure consistent column structure across years
4. Update the `years` list in the main notebook if adding new years

## Notes

- Original data files are not included in this repository due to size limitations
- Users must obtain the official PKS data from BKA sources
- The dashboard includes sample data generation for demonstration purposes

## Data Acquisition

Official crime statistics can be obtained from:
- [BKA PKS Publications](https://www.bka.de/DE/AktuelleInformationen/StatistikenLagebilder/PolizeilicheKriminalstatistik/pks_node.html)
- [German Federal Statistical Office](https://www.destatis.de)

For research purposes, contact the respective statistical offices for complete datasets.