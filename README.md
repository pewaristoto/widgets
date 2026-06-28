# Pewaris Widgets

Embed live football and togel data on any website with a single script tag.

**[Documentation](https://pewaristoto.github.io/widgets/)** · **[Demo](https://pewaristoto.github.io/widgets/demo.html)** · **[Widget Builder](https://widgets.pewaris.dev/widget/docs)**

---

## Getting started

Place a `div` where you want the widget, then include the script once per page.

```html
<div class="whistle-widget"
     data-type="standings"
     data-league="39"></div>

<script src="https://widgets.pewaris.dev/api/widget/script" async></script>
```

One script tag handles any number of widgets on the same page.

---

## Widget types

### Football

| `data-type` | Description |
|---|---|
| `standings` | League table |
| `league` | League table + fixtures |
| `games` | Fixture list |
| `game` | Single match — live score, lineups, stats |
| `team` | Team profile and recent fixtures |
| `player` | Player season stats |
| `prediction` | Upcoming match predictions |

### Togel

| `data-type` | Description |
|---|---|
| `result` | Latest draw result for one market |
| `board` | Result cards for multiple markets |
| `history` | Recent draw history |
| `prediksi` | Statistical number predictions |

---

## Attributes

| Attribute | Values | Description |
|---|---|---|
| `data-type` | see tables above | Required |
| `data-league` | e.g. `39`, `1` | League ID (football widgets) |
| `data-season` | e.g. `2026` | Optional — auto-detected if omitted |
| `data-id` | numeric ID | Match, team, or player ID |
| `data-market` | e.g. `macau`, `sg4d` | Togel market for result/history/prediksi |
| `data-markets` | e.g. `macau,sg4d,hkpools` | Markets for the board widget |
| `data-theme` | `light` · `dark` | Color scheme. Default: `light` |
| `data-accent` | hex color | Accent color |
| `data-layout` | `card` · `full` | `card` = vertical list. `full` = responsive grid |
| `data-lang` | `id` · `en` | Label language. Default: `id` for togel, `en` for football |
| `data-max` | number | Limit the number of rows shown |
| `data-max-width` | pixels | Max width for `card` layout. Default: 560 |
| `data-compact` | `true` | Tighter padding and font size |
| `data-groups` | e.g. `A,B,C,D` | Show specific groups in standings/league widgets |
| `data-show-logos` | `true` · `false` | Show or hide team/league logos |
| `data-show-form` | `true` · `false` | Show form column in standings |
| `data-show-venue` | `true` · `false` | Show venue in fixture lists |
| `data-show-footer` | `true` · `false` | Show attribution footer. Default: `true` |
| `data-schema` | `true` | Inject JSON-LD structured data (match widgets) |
| `data-refresh` | seconds | Auto-refresh interval for live match widget. `0` = off |

---

## League IDs

| League | `data-league` |
|---|---|
| FIFA World Cup 2026 | `1` |
| UEFA Champions League | `2` |
| UEFA Europa League | `3` |
| Premier League | `39` |
| La Liga | `140` |
| Serie A | `135` |
| Bundesliga | `78` |
| Ligue 1 | `61` |
| Liga 1 Indonesia | `253` |

---

## Togel markets

| Market | `data-market` |
|---|---|
| Toto Macau | `macau` |
| Singapore 4D | `sg4d` |
| Hongkong Pools | `hkpools` |
| Sydney Pools | `sdypools` |
| Singapore Toto | `sgtoto` |

70+ markets available. Full list at [pewaristotoprediksi.com](https://pewaristotoprediksi.com).

---

## Static HTML output

The [Widget Builder](https://widgets.pewaris.dev/widget/docs) can also export static HTML — no JavaScript required, search-engine readable. Use this for content that doesn't need to update in real time.

```html
<link rel="stylesheet" href="https://widgets.pewaris.dev/api/widget/style.css">
<div class="pw-w ..."> ... widget markup ... </div>
```

---

## About

This repository contains the public documentation and demo for Pewaris Widgets, part of the [Pewaristoto](https://pewaristotoprediksi.com) ecosystem, built by [Pewarisgroup](https://pewaris.dev).

- Football data: [API-Football](https://api-football.com)
- Togel data: Pewaristoto Live Draw API
- Live score app: [whistle.pewaris.dev](https://whistle.pewaris.dev)
