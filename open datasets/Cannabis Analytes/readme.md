Source: https://github.com/cannlytics/cannlytics/tree/main/datasets/cannabis_analytes

Accessed: Oct, 2023

Please note: This data currently includes only the Cannabinoids and Terpenes subsets. Additional data on Pesticides, Microbes, Heavy Metals, Residual Solvents, and other analytes will be available soon.

## Data Fields

Below is a non-exhaustive list of fields used to standardize the various data that are encountered. You may expect to find the following for each observation:

| Field                        | Example                                                | Description                                                                                                 |
| ---------------------------- | ------------------------------------------------------ | ----------------------------------------------------------------------------------------------------------- |
| `key`                        | `"thca"`                                               | A unique ID for each analyte.                                                                               |
| `description`                | `"Δ-9-Tetrahydrocannabinol is a cannabinoid..."`       | A brief description or summary about the analyte.                                                           |
| `name`                       | `"THC"`                                                | Common name of the analyte.                                                                                 |
| `scientific_name`            | `"\u0394-9-Tetrahydrocannabinol"`                      | The scientific name or IUPAC name of the analyte.                                                           |
| `type`                       | `"cannabinoid"`                                        | The type or classification of the analyte (e.g., terpene, cannabinoid).                                     |
| `wikipedia_url`              | `"https://en.wikipedia.org/wiki/Tetrahydrocannabinol"` | The Wikipedia URL where more detailed information can be found about the analyte.                           |
| `degrades_to`                | `["cannabinol"]`                                       | A list of chemicals or substances the analyte degrades to.                                                  |
| `precursors`                 | `["thca"]`                                             | A list of precursor chemicals or substances related to the analyte.                                         |
| `subtype`                    | `"psychoactive"`                                       | A sub-classification or additional details about the type of the analyte.                                   |
| `cas_number`                 | `"1972-08-3"`                                          | The Chemical Abstracts Service (CAS) registry number, which is a unique identifier for chemical substances. |
| `chemical_formula`           | `"C21H30O2"`                                           | The chemical formula of the analyte.                                                                        |
| `molar_mass`                 | `"314.5 g/mol"`                                        | The molar mass of the analyte.                                                                              |
| `density`                    | `"1.0±0.1 g/cm3"`                                      | The density of the analyte.                                                                                 |
| `boiling_point`              | `"383.5±42.0 °C"`                                      | The boiling point of the analyte.                                                                           |
| `image_url`                  | `"https://example.com/image.jpg"`                      | URL of an image representing the analyte.                                                                   |
| `chemical_formula_image_url` | `"https://example.com/formula_image.jpg"`              | URL of an image representing the chemical formula of the analyte.                                           |
