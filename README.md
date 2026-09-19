# Start page

My browser home page: the Astana clock, today's weather and air quality,
tenge exchange rates, working days left in the month and the next day off,
a "today's focus" note, and one-click links to every tool and directory I've
built, plus the public services I use most. Served at https://ktwyw.github.io/

Plain HTML, CSS and JavaScript in one file. Weather and air quality come from
Open-Meteo (no key), rates from open.er-api.com, and the holiday rules are the
same as in [kz-workdays](https://github.com/ktwyw/kz-workdays).

## Set it as your home page

- **Chrome / Edge:** Settings → On startup → "Open a specific page" →
  `https://ktwyw.github.io/`. Also Settings → Appearance → "Show home button".
- **Firefox:** Settings → Home → Homepage and new windows → Custom URL.
- **Safari:** Settings → General → Homepage.

## Using it

- Typing in the search box filters the links; press Enter to open the first
  match, or, if nothing matches, to run a web search.
- The focus note and the "My links" section are saved in the browser only.
- Air quality uses the European AQI scale (0–20 good … 100+ extremely poor)
  with PM2.5 and PM10 shown underneath.

## Editing the links

The `LINKS` object near the top of the script has three groups (tools,
directories, public services). Each entry is `[name, url, note]`.

## Ideas for next steps

- Weekly view of upcoming days off
- Show the next three calendar events from an .ics feed
- Kazakh and Russian interface
