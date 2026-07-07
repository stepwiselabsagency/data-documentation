# `/race-cards/historical-data`

## Endpoint

```http id="qg487o"
GET /race-cards/historical-data
```

## Description

Returns historical runner performance data, including race details, runner details, result information, speed metrics, efficiency metrics, and sectional/sector-level performance data.

---

## Columns

### Top-Level Columns


| Column                 | Example Value                                 | Explanation                                                       |
| ---------------------- | --------------------------------------------- | ----------------------------------------------------------------- |
| `rn`                   | `"1"`                                         | Row number or ranking/index value returned by the query.          |
| `sk_race_id`           | `"21927852"`                                  | Unique race ID.                                                   |
| `sk_runner_id`         | `"253265577998"`                              | Unique runner ID for the horse in this race.                      |
| `race_date`            | `"2026-06-12T00:00:00.000Z"`                  | Date of the race.                                                 |
| `race_group`           | `"2026-06-12 14:25 York"`                     | Combined race date, time, and venue label.                        |
| `no`                   | `13`                                          | Runner number on the racecard.                                    |
| `draw`                 | `7`                                           | Stall draw number.                                                |
| `m_runner_count`       | `"15"`                                        | Number of runners in the race.                                    |
| `pa_horse_id`          | `"4330822"`                                   | Horse ID from the racing data provider.                           |
| `jockey_id`            | `"41905"`                                     | Jockey ID.                                                        |
| `status`               | `"Runner"`                                    | Runner status in the race.                                        |
| `bred`                 | `"GB"`                                        | Country where the horse was bred.                                 |
| `weight`               | `"8st 13lbs"`                                 | Weight carried by the horse.                                      |
| `casualty_reason`      | `null`                                        | Reason for casualty, withdrawal, or non-completion, if available. |
| `runner_name`          | `"Baila Morena"`                              | Horse/runner name.                                                |
| `race_country`         | `"England"`                                   | Country where the race took place.                                |
| `country_code`         | `null`                                        | Country code, if available.                                       |
| `age`                  | `2`                                           | Horse age.                                                        |
| `position`             | `"12"`                                        | Final finishing position.                                         |
| `m_efficiency_3f_pct`  | `"126%"`                                      | Efficiency percentage over the final 3 furlongs.                  |
| `m_efficiency_4f_pct`  | `"123%"`                                      | Efficiency percentage over the final 4 furlongs.                  |
| `furlongs`             | `6`                                           | Race distance in furlongs.                                        |
| `going`                | `"Good"`                                      | Official going/ground condition.                                  |
| `rating_offical`       | `null`                                        | Official rating. Field name appears as `offical` in API.          |
| `rating_adjusted`      | `null`                                        | Adjusted rating, if available.                                    |
| `going_brief_advanced` | `"Good"`                                      | Detailed going/ground description.                                |
| `race_venue`           | `"York"`                                      | Racecourse or venue name.                                         |
| `topSpeed`             | `41.86324`                                    | Top speed recorded for the runner.                                |
| `price`                | `"4/1"`                                       | Betting price or odds.                                            |
| `bet_movements`        | `"op 7/1"`                                    | Betting market movement information.                              |
| `jockey_name`          | `"S De Sousa"`                                | Jockey name.                                                      |
| `trainer_name`         | `"Ollie Pears"`                               | Trainer name.                                                     |
| `comments`             | `"prominent, ridden 3f out, weakened 1f out"` | Race comment for the runner.                                      |
| `max`                  | `"41.86"`                                     | Maximum speed summary value.                                      |
| `avg`                  | `"37.44"`                                     | Average speed summary value.                                      |
| `rt`                   | `"60.21"`                                     | Race time or runner time summary value.                           |
| `avg_rank`             | `"7.00"`                                      | Average rank across the race/sections.                            |
| `avg_stride`           | `null`                                        | Average stride value, if available.                               |
| `sector_numbers`       | `[0, 1, 2, 3, 4]`                             | List of sector numbers available for this runner.                 |
| `sector_data`          | `[ {...}, {...} ]`                            | List of detailed sectional/sector-level performance records.      |


---



### `sector_data` Columns


| Column             | Example Value        | Explanation                                                             |
| ------------------ | -------------------- | ----------------------------------------------------------------------- |
| `sector`           | `0`                  | Sector number within the race.                                          |
| `max_speed`        | `34.561547503507136` | Maximum speed recorded in this sector.                                  |
| `avg_speed`        | `32.950661236817695` | Average speed recorded in this sector.                                  |
| `sector_duration`  | `13.650000095367432` | Time taken to complete the sector.                                      |
| `total_distance`   | `202.18714061069917` | Distance covered in the sector.                                         |
| `race_rank`        | `12`                 | Runner’s rank within the race for that sector.                          |
| `stride_length`    | `null`               | Stride length in the sector, if available.                              |
| `time_behind`      | `"00:00:00.4"`       | Time behind the next relevant runner or comparison point in the sector. |
| `time_behind_lead` | `"00:00:02.35"`      | Time behind the race leader in the sector.                              |
| `stride_count`     | `null`               | Number of strides in the sector, if available.                          |
| `stride_frequency` | `null`               | Stride frequency in the sector, if available.                           |


---



# Model Usage



## Model Version: `v1`


| Column                         | Used in v1? | Why   |
| ------------------------------ | ----------- | ----- |
| `rn`                           | `Yes/No`    | `TBC` |
| `sk_race_id`                   | `Yes/No`    | `TBC` |
| `sk_runner_id`                 | `Yes/No`    | `TBC` |
| `race_date`                    | `Yes/No`    | `TBC` |
| `race_group`                   | `Yes/No`    | `TBC` |
| `no`                           | `Yes/No`    | `TBC` |
| `draw`                         | `Yes/No`    | `TBC` |
| `m_runner_count`               | `Yes/No`    | `TBC` |
| `pa_horse_id`                  | `Yes/No`    | `TBC` |
| `jockey_id`                    | `Yes/No`    | `TBC` |
| `status`                       | `Yes/No`    | `TBC` |
| `bred`                         | `Yes/No`    | `TBC` |
| `weight`                       | `Yes/No`    | `TBC` |
| `casualty_reason`              | `Yes/No`    | `TBC` |
| `runner_name`                  | `Yes/No`    | `TBC` |
| `race_country`                 | `Yes/No`    | `TBC` |
| `country_code`                 | `Yes/No`    | `TBC` |
| `age`                          | `Yes/No`    | `TBC` |
| `position`                     | `Yes/No`    | `TBC` |
| `m_efficiency_3f_pct`          | `Yes/No`    | `TBC` |
| `m_efficiency_4f_pct`          | `Yes/No`    | `TBC` |
| `furlongs`                     | `Yes/No`    | `TBC` |
| `going`                        | `Yes/No`    | `TBC` |
| `rating_offical`               | `Yes/No`    | `TBC` |
| `rating_adjusted`              | `Yes/No`    | `TBC` |
| `going_brief_advanced`         | `Yes/No`    | `TBC` |
| `race_venue`                   | `Yes/No`    | `TBC` |
| `topSpeed`                     | `Yes/No`    | `TBC` |
| `price`                        | `Yes/No`    | `TBC` |
| `bet_movements`                | `Yes/No`    | `TBC` |
| `jockey_name`                  | `Yes/No`    | `TBC` |
| `trainer_name`                 | `Yes/No`    | `TBC` |
| `comments`                     | `Yes/No`    | `TBC` |
| `max`                          | `Yes/No`    | `TBC` |
| `avg`                          | `Yes/No`    | `TBC` |
| `rt`                           | `Yes/No`    | `TBC` |
| `avg_rank`                     | `Yes/No`    | `TBC` |
| `avg_stride`                   | `Yes/No`    | `TBC` |
| `sector_numbers`               | `Yes/No`    | `TBC` |
| `sector_data`                  | `Yes/No`    | `TBC` |
| `sector_data.sector`           | `Yes/No`    | `TBC` |
| `sector_data.max_speed`        | `Yes/No`    | `TBC` |
| `sector_data.avg_speed`        | `Yes/No`    | `TBC` |
| `sector_data.sector_duration`  | `Yes/No`    | `TBC` |
| `sector_data.total_distance`   | `Yes/No`    | `TBC` |
| `sector_data.race_rank`        | `Yes/No`    | `TBC` |
| `sector_data.stride_length`    | `Yes/No`    | `TBC` |
| `sector_data.time_behind`      | `Yes/No`    | `TBC` |
| `sector_data.time_behind_lead` | `Yes/No`    | `TBC` |
| `sector_data.stride_count`     | `Yes/No`    | `TBC` |
| `sector_data.stride_frequency` | `Yes/No`    | `TBC` |


