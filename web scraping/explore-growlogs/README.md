## Growlog Data Collector for Cannabis Cultivation

This project collects data from [cannabis growlogs](https://growithjane.com/explore-growlogs) using web scraping techniques. The collected data includes details about the strain, growing medium, and environmental conditions for each grow.

### Data Structure

Each growlog page returns data in the following format:

```json
{
    "title": "Dance World #1",
    "data": {
        "strain": {
            "seed_bank": "Royal Queen Seeds",
            "seed_type": "Dance World"
        },
        "medium": {
            "title": "Soil",
            "content": "BioBizz light"
        },
        "environment": [
            {
                "title": "Name",
                "content": "OfficeGrow"
            },
            {
                "title": "Type",
                "content": "Indoor"
            },
            {
                "title": "Exposure Time",
                "content": "18 Hours"
            },
            {
                "title": "Environment Size",
                "content": "120 cm x 180 cm x 90 cm"
            },
            {
                "title": "Lights",
                "content": "LED - 100 W"
            }
        ]
    }
}
```


### License

This project is licensed under the GPL-3.0 License. See the `LICENSE` file for details.


