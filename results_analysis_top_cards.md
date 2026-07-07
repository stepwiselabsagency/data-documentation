# `/results-analysis/top-cards`

## Endpoint

```http id="75w7c2"
GET /results-analysis/top-cards
```

## Description

Returns top-level race card/result analysis details for a race. Each item represents one race and includes race metadata, prize money, distance, going, tote/betting result fields, and race conditions.

---

## Columns

| Column                  | Example Value                              | Explanation                                                                         |
| ----------------------- | ------------------------------------------ | ----------------------------------------------------------------------------------- |
| `sk_race_id`            | `"22110727"`                               | Unique race ID.                                                                     |
| `pa_horse_id`           | `"4344154"`                                | Horse ID from the racing data provider.                                             |
| `race_country`          | `"England"`                                | Country where the race is taking place.                                             |
| `max_runners`           | `17`                                       | Maximum number of runners allowed for the race.                                     |
| `winnings_cur`          | `"GBP"`                                    | Currency used for race winnings.                                                    |
| `race_venue`            | `"Pontefract"`                             | Racecourse or venue name.                                                           |
| `track`                 | `"Turf"`                                   | Track surface/type.                                                                 |
| `race_group`            | `"2026-07-07 13:48 Pontefract"`            | Combined race date, time, and venue label.                                          |
| `race_eligibility`      | `"2YO only"`                               | Race eligibility condition.                                                         |
| `race_distance_yards`   | `"1320"`                                   | Race distance in yards.                                                             |
| `race_time_name`        | `"13:48"`                                  | Race start time.                                                                    |
| `price_1`               | `3402`                                     | Prize money for first place.                                                        |
| `price_2`               | `1596`                                     | Prize money for second place.                                                       |
| `price_3`               | `798`                                      | Prize money for third place.                                                        |
| `race_date`             | `"2026-07-07T00:00:00.000Z"`               | Date of the race.                                                                   |
| `race_name`             | `"Wakefield Thornes Cricket Club Nursery"` | Full race name.                                                                     |
| `thumb_url`             | `null`                                     | Thumbnail image URL, if available.                                                  |
| `thumb_status`          | `null`                                     | Thumbnail status, if available.                                                     |
| `race_track`            | `"Turf"`                                   | Race track surface/type.                                                            |
| `distance_metres`       | `1207.0080003727`                          | Race distance in metres.                                                            |
| `race_distance`         | `"0m 6f 0y"`                               | Race distance in miles, furlongs, and yards.                                        |
| `distance`              | `6`                                        | Race distance expressed as a numeric distance value, usually furlongs.              |
| `tote_trifecta_cur`     | `null`                                     | Currency for tote trifecta value, if available.                                     |
| `tote_trifecta_val`     | `null`                                     | Tote trifecta dividend/value, if available.                                         |
| `tote_exata_cur`        | `null`                                     | Currency for tote exacta value, if available. Field name appears as `exata` in API. |
| `tote_exacta_val`       | `null`                                     | Tote exacta dividend/value, if available.                                           |
| `bet_csf_cur`           | `null`                                     | Currency for computer straight forecast value, if available.                        |
| `bet_csf_val`           | `null`                                     | Computer straight forecast value, if available.                                     |
| `tote_place_cur`        | `null`                                     | Currency for tote place value, if available.                                        |
| `tote_place_val`        | `null`                                     | Tote place dividend/value, if available.                                            |
| `tote_win_cur`          | `null`                                     | Currency for tote win value, if available.                                          |
| `tote_win_val`          | `null`                                     | Tote win dividend/value, if available.                                              |
| `tote_swinger_cur`      | `null`                                     | Currency for tote swinger value, if available.                                      |
| `tote_swinger_val`      | `null`                                     | Tote swinger dividend/value, if available.                                          |
| `tote_win_numbers`      | `null`                                     | Winning tote number, if available.                                                  |
| `tote_swinger_numbers`  | `null`                                     | Tote swinger numbers, if available.                                                 |
| `tote_place_numbers`    | `null`                                     | Tote place numbers, if available.                                                   |
| `tote_exacta_numbers`   | `null`                                     | Tote exacta numbers, if available.                                                  |
| `tote_trifecta_numbers` | `null`                                     | Tote trifecta numbers, if available.                                                |
| `bet_csf_numbers`       | `null`                                     | Computer straight forecast numbers, if available.                                   |
| `age_group`             | `"2YO ONLY"`                               | Race age group.                                                                     |
| `status`                | `null`                                     | Race or result status, if available.                                                |
| `race_class`            | `"6"`                                      | Race class.                                                                         |
| `m_places_paid`         | `null`                                     | Number of places paid, if available.                                                |
| `eligibility`           | `"2YO only"`                               | Eligibility condition for the race.                                                 |
| `handicap`              | `"Yes"`                                    | Indicates whether the race is a handicap.                                           |
| `race_type`             | `"Flat"`                                   | Type of race.                                                                       |
| `runners`               | `null`                                     | Number of runners, if available.                                                    |
| `win_time`              | `null`                                     | Winning time, if available after result.                                            |
| `going`                 | `"Good-good to firm in places"`            | Going/ground condition.                                                             |
| `going_brief`           | `null`                                     | Short going description, if available.                                              |
| `advanced_going`        | `"Good-good to firm in places"`            | Advanced going/ground description.                                                  |
| `going_brief_advanced`  | `"Good-good to firm in places"`            | Detailed going/ground description.                                                  |

---

# Model Usage

## Model Version: `v1`

| Column                  | Used in v1? | Why   |
| ----------------------- | ----------- | ----- |
| `sk_race_id`            | `Yes/No`    | `TBC` |
| `pa_horse_id`           | `Yes/No`    | `TBC` |
| `race_country`          | `Yes/No`    | `TBC` |
| `max_runners`           | `Yes/No`    | `TBC` |
| `winnings_cur`          | `Yes/No`    | `TBC` |
| `race_venue`            | `Yes/No`    | `TBC` |
| `track`                 | `Yes/No`    | `TBC` |
| `race_group`            | `Yes/No`    | `TBC` |
| `race_eligibility`      | `Yes/No`    | `TBC` |
| `race_distance_yards`   | `Yes/No`    | `TBC` |
| `race_time_name`        | `Yes/No`    | `TBC` |
| `price_1`               | `Yes/No`    | `TBC` |
| `price_2`               | `Yes/No`    | `TBC` |
| `price_3`               | `Yes/No`    | `TBC` |
| `race_date`             | `Yes/No`    | `TBC` |
| `race_name`             | `Yes/No`    | `TBC` |
| `thumb_url`             | `Yes/No`    | `TBC` |
| `thumb_status`          | `Yes/No`    | `TBC` |
| `race_track`            | `Yes/No`    | `TBC` |
| `distance_metres`       | `Yes/No`    | `TBC` |
| `race_distance`         | `Yes/No`    | `TBC` |
| `distance`              | `Yes/No`    | `TBC` |
| `tote_trifecta_cur`     | `Yes/No`    | `TBC` |
| `tote_trifecta_val`     | `Yes/No`    | `TBC` |
| `tote_exata_cur`        | `Yes/No`    | `TBC` |
| `tote_exacta_val`       | `Yes/No`    | `TBC` |
| `bet_csf_cur`           | `Yes/No`    | `TBC` |
| `bet_csf_val`           | `Yes/No`    | `TBC` |
| `tote_place_cur`        | `Yes/No`    | `TBC` |
| `tote_place_val`        | `Yes/No`    | `TBC` |
| `tote_win_cur`          | `Yes/No`    | `TBC` |
| `tote_win_val`          | `Yes/No`    | `TBC` |
| `tote_swinger_cur`      | `Yes/No`    | `TBC` |
| `tote_swinger_val`      | `Yes/No`    | `TBC` |
| `tote_win_numbers`      | `Yes/No`    | `TBC` |
| `tote_swinger_numbers`  | `Yes/No`    | `TBC` |
| `tote_place_numbers`    | `Yes/No`    | `TBC` |
| `tote_exacta_numbers`   | `Yes/No`    | `TBC` |
| `tote_trifecta_numbers` | `Yes/No`    | `TBC` |
| `bet_csf_numbers`       | `Yes/No`    | `TBC` |
| `age_group`             | `Yes/No`    | `TBC` |
| `status`                | `Yes/No`    | `TBC` |
| `race_class`            | `Yes/No`    | `TBC` |
| `m_places_paid`         | `Yes/No`    | `TBC` |
| `eligibility`           | `Yes/No`    | `TBC` |
| `handicap`              | `Yes/No`    | `TBC` |
| `race_type`             | `Yes/No`    | `TBC` |
| `runners`               | `Yes/No`    | `TBC` |
| `win_time`              | `Yes/No`    | `TBC` |
| `going`                 | `Yes/No`    | `TBC` |
| `going_brief`           | `Yes/No`    | `TBC` |
| `advanced_going`        | `Yes/No`    | `TBC` |
| `going_brief_advanced`  | `Yes/No`    | `TBC` |
