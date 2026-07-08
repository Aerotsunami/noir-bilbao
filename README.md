# NOIR BILBAO — Crime Atlas

**Live:** https://aerotsunami.github.io/noir-bilbao/

An interactive crime map of Greater Bilbao (Gran Bilbao), built as an installable PWA
in a true-crime / *Sin City* aesthetic — graphite, blood red, white. Bilingual **EN / RU**.

## What it does

- **Neighbourhood map** — a real dark basemap with ~35 zones across Bilbao's districts and the estuary towns, coloured by night-risk or by crime volume. Tap a zone for its full file.
- **Night safety** — each neighbourhood is rated *OK / with care / avoid at night*, with plain-language guidance on where it's fine to walk after dark and where it isn't.
- **Neighbourhood files** — reported crimes per year, share of the city, violent-crime share, 12-month trend, crime mix by type, typical offenders, and a mini trend chart.
- **Rolling summary** — estimated reported crimes for the last **24 hours / 3 days / 7 days**; tap a card to break it down by neighbourhood.
- **Monthly dynamics** — a year of reported-crime totals for the city, with the seasonal peak highlighted.
- **Character of crime** — city-wide crime mix and a breakdown of who commits it, including the origin of those detained.
- **Recent incidents** — a live news feed (24h / 3 days / week) of crime and policing headlines in Bilbao, each linking to its source.
- **Most dangerous zones** — a ranked list that expands into full stats on tap.

## О чём это

Интерактивная карта преступности Большого Бильбао в виде устанавливаемого PWA, в стилистике
тру-крайм / «Города грехов». Показывает районы по уровню ночного риска, безопасность прогулок
ночью, статистику по каждому кварталу, сводку за 24 часа / 3 дня / 7 дней с разбивкой по районам,
динамику по месяцам, структуру и характер преступности, происхождение задержанных и живую ленту
происшествий со ссылками на источники. Языки — русский и английский.

## Data & method

City-wide 2025 figures are anchored to the official **Ertzaintza** and **Bilbao Municipal Police**
balance (29,696 reported crimes; theft 55.5%; violent robbery −8.85%; cybercrime +10.5%; 3,155
arrests), with detainee-origin data from the Ertzaintza's first origin report (Jan–Sep 2025).
**Neighbourhood-level and month-by-month figures are a transparent model** distributing those
official totals by known hotspots and seasonality — they are illustrative, not exact official
counts. Zones are proportional markers at real coordinates, not official boundaries. The live
feed is Google News, not an official police log. Basemap © OpenStreetMap contributors, © CARTO.

*Not affiliated with the Ertzaintza or any public authority. For decisions, consult the official
[Ertzaintza statistics portal](https://www.ertzaintza.euskadi.eus/lfr/web/ertzaintza/estadisticas-delictivas).*

## Tech

Single-file `index.html` (Leaflet + vanilla JS), PWA manifest + service worker for offline app
shell, noir SVG icon. No build step — just static files on GitHub Pages.
