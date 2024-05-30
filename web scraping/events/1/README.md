## Cannabis Events Scraper

This project is focused on web scraping to collect data from the Massachusetts Cannabis Control Commission's events calendar at [MassCannabisControl Calendar](https://masscannabiscontrol.com/calendar/). The script captures details about each event including titles, URLs, dates, times, and more.

### Data Structure

Each scraped event is structured as follows:

```json
{
  "title": "Cannabis Control Commission Public Meeting",
  "url": "https://masscannabiscontrol.com/events/cannabis-control-commission-public-meeting-9/?occurrence=2017-09-26",
  "date": "Sep 26 2017",
  "time": "10:30 am",
  "labels": ["Public Meetings"],
  "location": "One Ashburton Place\nAshburton Café Meeting Room\nLower Plaza Level\nBoston, MA 02108",
  "related_documents": [
    {
      "title": "Notice of Public Meeting",
      "url": "https://masscannabiscontrol.com/document/notice-of-public-meeting-9-26-2017-cannabis-control-commission/"
    },
    {
      "title": "Presentation from 9/26/17 Meeting",
      "url": "https://masscannabiscontrol.com/document/presentation/"
    },
    {
      "title": "Handout | Draft Executive Director Job Posting",
      "url": "https://masscannabisnonna.com/document/handout-draft-executive-director-job-posting/"
    },
    {
      "title": "Handout | Draft Mission Statement",
      "url": "https://masscannabiscontrol.com/document/handout-draft-mission-statement/"
    }
  ]
}
```

### License

This project is licensed under the GPL-3.0 License. See the `LICENSE` file for details.
