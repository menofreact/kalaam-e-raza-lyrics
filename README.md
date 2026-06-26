# Kalaam E Raza — Complete Lyrics Archive

Islamic devotional poetry (Na'at, Hamd, Manqabat, Salaam) by **A'la Hazrat Imam Ahmed Raza Khan** & other poets — scraped from [kalaam-e-raza.in](https://www.kalaam-e-raza.in/)

---

## Stats

| Metric | Count |
|--------|-------|
| Total Kalaam | 244 |
| Total Lines | 5413 |
| Categories | 30 |

## Categories

| Category | Kalaam |
|----------|--------|
| A | 28 |
| B | 12 |
| C | 6 |
| D | 8 |
| E | 1 |
| F | 6 |
| G | 6 |
| H | 13 |
| Hamd | 5 |
| I | 2 |
| J | 7 |
| K | 21 |
| Kalaam E Noori | 12 |
| Kalaam E Raza | 52 |
| L | 5 |
| M | 33 |
| Manqabat | 37 |
| N | 7 |
| Other Naat Shareef | 126 |
| P | 7 |
| Q | 5 |
| R | 9 |
| S | 18 |
| Salaam | 12 |
| T | 15 |
| U | 2 |
| W | 7 |
| Y | 12 |
| Z | 5 |

## Structure

```
kalaam-e-raza/
├── kalaam-e-raza.json      # Full dataset (244 kalaam, 5413 lines)
├── INDEX.md                # Full alphabetical index
├── README.md               # This file
└── lyrics/                 # Individual files by first letter
    ├── A/
    │   ├── arsh-ka-dulha-aaya-hain.md
    │   ├── arzo-samaa-banay-hain.md
    │   └── ...
    └── Z/
```

## JSON Format

```json
{
  "title": "Kalaam Title",
  "url": "https://...",
  "categories": ["Hamd", "Kalaam E Raza"],
  "lyrics": ["Line 1", "Line 2", ...],
  "line_count": 42
}
```

## Usage

```bash
# Search across all lyrics
grep -i "muhammad" kalaam-e-raza.json

# Count by category
jq '.posts | group_by(.categories[0])[] | {"cat": .[0].categories[0], "count": length}' kalaam-e-raza.json
```

---

<p align="center">
<b>Kalaam E Raza</b> — <i>Dedicated to lovers of the Prophet ﷺ</i><br>
<a href="https://www.kalaam-e-raza.in/">kalaam-e-raza.in</a>
</p>
