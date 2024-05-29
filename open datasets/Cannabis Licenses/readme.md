Source: https://github.com/cannlytics/cannlytics/tree/main/datasets/cannabis_licenses

Accessed: Sep, 2023

Please note: License data is currently not available in all states. It is expected to be widely available by 2024.

### Data Fields

Below is a non-exhaustive list of fields, used to standardize the various data that are encountered, that you may expect to find for each observation.

| Field                    | Example                              | Description                                                            |
| ------------------------ | ------------------------------------ | ---------------------------------------------------------------------- |
| `id`                     | `"1046"`                             | A state-unique ID for the license.                                     |
| `license_number`         | `"C10-0000423-LIC"`                  | A unique license number.                                               |
| `license_status`         | `"Active"`                           | The status of the license. Only licenses that are active are included. |
| `license_status_date`    | `"2022-04-20T00:00"`                 | The date the status was assigned, an ISO-formatted date if present.    |
| `license_term`           | `"Provisional"`                      | The term for the license.                                              |
| `license_type`           | `"Commercial - Retailer"`            | The type of business license.                                          |
| `license_designation`    | `"Adult-Use and Medicinal"`          | A state-specific classification for the license.                       |
| `issue_date`             | `"2019-07-15T00:00:00"`              | An issue date for the license, an ISO-formatted date if present.       |
| `expiration_date`        | `"2023-07-14T00:00:00"`              | An expiration date for the license, an ISO-formatted date if present.  |
| `licensing_authority_id` | `"BCC"`                              | A unique ID for the state licensing authority.                         |
| `licensing_authority`    | `"Bureau of Cannabis Control (BCC)"` | The state licensing authority.                                         |
| `business_legal_name`    | `"Movocan"`                          | The legal name of the business that owns the license.                  |
| `business_dba_name`      | `"Movocan"`                          | The name the license is doing business as.                             |
| `business_owner_name`    | `"redacted"`                         | The name of the owner of the license.                                  |
| `business_structure`     | `"Corporation"`                      | The structure of the business that owns the license.                   |
| `activity`               | `"Pending Inspection"`               | Any relevant license activity.                                         |
| `premise_street_address` | `"1632 Gateway Rd"`                  | The street address of the business.                                    |
| `premise_city`           | `"Calexico"`                         | The city of the business.                                              |
| `premise_state`          | `"CA"`                               | The state abbreviation of the business.                                |
| `premise_county`         | `"Imperial"`                         | The county of the business.                                            |
| `premise_zip_code`       | `"92231"`                            | The zip code of the business.                                          |
| `business_email`         | `"redacted@gmail.com"`               | The business email of the license.                                     |
| `business_phone`         | `"(555) 555-5555"`                   | The business phone of the license.                                     |
| `business_website`       | `"cannlytics.com"`                   | The business website of the license.                                   |
| `parcel_number`          | `"A42"`                              | An ID for the business location.                                       |
| `premise_latitude`       | `32.69035693`                        | The latitude of the business.                                          |
| `premise_longitude`      | `-115.38987552`                      | The longitude of the business.                                         |
| `data_refreshed_date`    | `"2022-09-21T12:16:33.3866667"`      | An ISO-formatted time when the license data was updated.               |
