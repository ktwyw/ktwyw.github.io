# Start page

My browser homepage: the Astana clock, today's weather and air quality,
tenge exchange rates, working days left in the month and the next day off,
a "today's focus" note, and one-click links to every tool and directory I've
built, plus the public services I use most. Served at https://ktwyw.github.io/

Plain HTML, CSS and JavaScript in one file. Weather and air quality come from
Open-Meteo (no key), rates from open.er-api.com, and the holiday rules are the
same as in [kz-workdays](https://github.com/ktwyw/kz-workdays).

## Set it as your homepage

- **Chrome / Edge:** Settings → On startup → "Open a specific page" →
  `https://ktwyw.github.io/`. Also Settings → Appearance → "Show home button".
- **Firefox:** Settings → Home → Homepage and new windows → Custom URL.
- **Safari:** Settings → General → Homepage.

## Using it

- Typing in the search box filters the links; press Enter to open the first
  match, or, if nothing matches, to run a web search.
- The focus note and the "My links" section are saved in the browser only.
- Air quality uses the European AQI scale (0–20 good … 100+ extremely poor)
  with PM2.5 and PM10 shown underneath. The value is Open-Meteo's model
  estimate for Astana; it's a citywide picture, not a street-level sensor.
- "Next day off" is the first public holiday or moved day off on or after
  today, looking at this year and next. Holidays that fall on a weekend are
  shown by their moved day (e.g. Republic Day, Sun 25 Oct 2026 → Mon 26 Oct).

## Editing the links

The `LINKS` object near the top of the script has three groups (tools,
directories, public services). Each entry is `[name, url, note]`.

## Changelog

- 2026-09-21 — fixed "next day off" skipping past October and December
  holidays to New Year (the search didn't stop at the first match).
- 2026-09-20 — first version.

## Ideas for next steps

- Weekly view of upcoming days off
- Show the next three calendar events from an .ics feed
- Kazakh and Russian interface
