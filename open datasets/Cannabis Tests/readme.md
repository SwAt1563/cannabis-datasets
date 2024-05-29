Source: https://github.com/cannlytics/cannlytics/tree/main/datasets/cannabis_tests

Accessed: Feb, 2023

Please note: These test results are currently sourced only from Raw Gardens. Additional data from MCR Labs, PSI Labs, SC Labs, and Washington State will be available soon.

### Data Fields

Below is a non-exhaustive list of fields, used to standardize the various data that are encountered, that you may expect encounter in the parsed COA data.

| Field                        | Example                          | Description                                                                                    |
| ---------------------------- | -------------------------------- | ---------------------------------------------------------------------------------------------- |
| `analyses`                   | ["cannabinoids"]                 | A list of analyses performed on a given sample.                                                |
| `{analysis}_method`          | "HPLC"                           | The method used for each analysis.                                                             |
| `{analysis}_status`          | "pass"                           | The pass, fail, or N/A status for pass / fail analyses.                                        |
| `coa_urls`                   | [{"url": "", "filename": ""}]    | A list of certificate of analysis (CoA) URLs.                                                  |
| `date_collected`             | 2022-04-20T04:20                 | An ISO-formatted time when the sample was collected.                                           |
| `date_tested`                | 2022-04-20T16:20                 | An ISO-formatted time when the sample was tested.                                              |
| `date_received`              | 2022-04-20T12:20                 | An ISO-formatted time when the sample was received.                                            |
| `distributor`                | "Your Favorite Dispo"            | The name of the product distributor, if applicable.                                            |
| `distributor_address`        | "Under the Bridge, SF, CA 55555" | The distributor address, if applicable.                                                        |
| `distributor_street`         | "Under the Bridge"               | The distributor street, if applicable.                                                         |
| `distributor_city`           | "SF"                             | The distributor city, if applicable.                                                           |
| `distributor_state`          | "CA"                             | The distributor state, if applicable.                                                          |
| `distributor_zipcode`        | "55555"                          | The distributor zip code, if applicable.                                                       |
| `distributor_license_number` | "L2Stat"                         | The distributor license number, if applicable.                                                 |
| `images`                     | [{"url": "", "filename": ""}]    | A list of image URLs for the sample.                                                           |
| `lab_results_url`            | "https://cannlytics.com/results" | A URL to the sample results online.                                                            |
| `producer`                   | "Grow Tent"                      | The producer of the sampled product.                                                           |
| `producer_address`           | "3rd & Army, SF, CA 55555"       | The producer's address.                                                                        |
| `producer_street`            | "3rd & Army"                     | The producer's street.                                                                         |
| `producer_city`              | "SF"                             | The producer's city.                                                                           |
| `producer_state`             | "CA"                             | The producer's state.                                                                          |
| `producer_zipcode`           | "55555"                          | The producer's zipcode.                                                                        |
| `producer_license_number`    | "L2Calc"                         | The producer's license number.                                                                 |
| `product_name`               | "Blue Rhino Pre-Roll"            | The name of the product.                                                                       |
| `lab_id`                     | "Sample-0001"                    | A lab-specific ID for the sample.                                                              |
| `product_type`               | "flower"                         | The type of product.                                                                           |
| `batch_number`               | "Order-0001"                     | A batch number for the sample or product.                                                      |
| `metrc_ids`                  | ["1A4060300002199000003445"]     | A list of relevant Metrc IDs.                                                                  |
| `metrc_lab_id`               | "1A4060300002199000003445"       | The Metrc ID associated with the lab sample.                                                   |
| `metrc_source_id`            | "1A4060300002199000003445"       | The Metrc ID associated with the sampled product.                                              |
| `product_size`               | 2000                             | The size of the product in milligrams.                                                         |
| `serving_size`               | 1000                             | An estimated serving size in milligrams.                                                       |
| `servings_per_package`       | 2                                | The number of servings per package.                                                            |
| `sample_weight`              | 1                                | The weight of the product sample in grams.                                                     |
| `results`                    | [{...},...]                      | A list of results, see below for result-specific fields.                                       |
| `status`                     | "pass"                           | The overall pass / fail status for all contaminant screening analyses.                         |
| `total_cannabinoids`         | 14.20                            | The analytical total of all cannabinoids measured.                                             |
| `total_thc`                  | 14.00                            | The analytical total of THC and THCA.                                                          |
| `total_cbd`                  | 0.20                             | The analytical total of CBD and CBDA.                                                          |
| `total_terpenes`             | 0.42                             | The sum of all terpenes measured.                                                              |
| `results_hash`               | "{sha256-hash}"                  | An HMAC of the sample's `results` JSON signed with Cannlytics' public key, `"cannlytics.eth"`. |
| `sample_id`                  | "{sha256-hash}"                  | A generated ID to uniquely identify the `producer`, `product_name`, and `results`.             |
| `sample_hash`                | "{sha256-hash}"                  | An HMAC of the entire sample JSON signed with Cannlytics' public key, `"cannlytics.eth"`.      |
| `strain_name`                | "Blue Rhino"                     | A strain name, if specified. Otherwise, can be attempted to be parsed from the `product_name`. |

Each result can contain the following fields.

| Field      | Example      | Description                                                                                                                      |
| ---------- | ------------ | -------------------------------------------------------------------------------------------------------------------------------- |
| `analysis` | "pesticides" | The analysis used to obtain the result.                                                                                          |
| `key`      | "pyrethrins" | A standardized key for the result analyte.                                                                                       |
| `name`     | "Pyrethrins" | The lab's internal name for the result analyte                                                                                   |
| `value`    | 0.42         | The value of the result.                                                                                                         |
| `mg_g`     | 0.00000042   | The value of the result in milligrams per gram.                                                                                  |
| `units`    | "ug/g"       | The units for the result `value`, `limit`, `lod`, and `loq`.                                                                     |
| `limit`    | 0.5          | A pass / fail threshold for contaminant screening analyses.                                                                      |
| `lod`      | 0.01         | The limit of detection for the result analyte. Values below the `lod` are typically reported as `ND`.                            |
| `loq`      | 0.1          | The limit of quantification for the result analyte. Values above the `lod` but below the `loq` are typically reported as `<LOQ`. |
| `status`   | "pass"       | The pass / fail status for contaminant screening analyses.                                                                       |
