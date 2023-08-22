fetch-sans-ics: fetch calendars for SANS summits in a single ICS file

SANS summit schedules have ICS calendar entries available for
download, but as one file per talk, making it incredibly tedious to
try to import an entire event. This script parses the HTML file, finds
the iCal data, collects all events in a single calendar, and writes it
to standard output.

Run it as:

```
./fetch-sans-ics url > calendar.ics
```

With the URL for the summit agenda page.

Requires [Ruby](https://www.ruby-lang.org/en/) with
[Nokogiri](https://nokogiri.org/) and
[icalendar](https://github.com/icalendar/icalendar).
