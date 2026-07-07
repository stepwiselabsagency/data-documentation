# `/race-cards/each-runner-result`

## Endpoint

```http id="i5syju"
GET /race-cards/each-runner-result
```

## Description

Returns recent result history for a runner/horse. Each item in the response represents one runner and contains a `last_6_results` list with recent race results for that runner.

---

## Columns

### Top-Level Columns

| Column           | Example Value      | Explanation                                                     |
| ---------------- | ------------------ | --------------------------------------------------------------- |
| `runner_name`    | `"Poppy Foxy"`     | Name of the horse/runner.                                       |
| `m_cloth_number` | `1`                | Cloth or saddlecloth number for the runner in the current race. |
| `horse_bred`     | `"IRE"`            | Country where the horse was bred.                               |
| `position`       | `null`             | Current or result position for the runner, if available.        |
| `pa_horse_id`    | `"4344154"`        | Horse ID from the racing data provider.                         |
| `last_6_results` | `[ {...}, {...} ]` | List of recent race results for this runner.                    |

---

### `last_6_results` Columns

| Column                          | Example Value                                                                             | Explanation                                                       |
| ------------------------------- | ----------------------------------------------------------------------------------------- | ----------------------------------------------------------------- |
| `date`                          | `"2026-06-30"`                                                                            | Date of the historical race.                                      |
| `venue`                         | `"Salisbury"`                                                                             | Racecourse or venue name.                                         |
| `distance`                      | `"0m 6f 0y"`                                                                              | Race distance in miles, furlongs, and yards.                      |
| `status`                        | `"Runner"`                                                                                | Runner status in that historical race.                            |
| `sk_race_id`                    | `22061732`                                                                                | Unique race ID for the historical race.                           |
| `going`                         | `"Good to Firm (Good in places)"`                                                         | Official going/ground condition.                                  |
| `finish_position`               | `0`                                                                                       | Numeric finish position field.                                    |
| `group`                         | `"2026-06-30 15:07 Salisbury"`                                                            | Combined date, time, and venue label.                             |
| `time_name`                     | `"15:07"`                                                                                 | Race start time.                                                  |
| `handicap`                      | `"No"`                                                                                    | Indicates whether the race was a handicap.                        |
| `race_eligibility`              | `"2YO only"`                                                                              | Eligibility condition for the race.                               |
| `commentary`                    | `"wore red hood to post, led, pushed along 2f out, headed 1f out, weakened final 110yds"` | In-running commentary for the runner.                             |
| `position`                      | `"5"`                                                                                     | Finishing position as shown in the result.                        |
| `race_group`                    | `"2026-06-30 15:07 Salisbury"`                                                            | Race date, time, and venue label.                                 |
| `m_runner_count`                | `11`                                                                                      | Number of runners in the race.                                    |
| `class`                         | `"2"`                                                                                     | Race class.                                                       |
| `going_brief_advanced`          | `"Good to Firm (Good in places)"`                                                         | Detailed going/ground description.                                |
| `sp`                            | `"16/1"`                                                                                  | Starting price odds.                                              |
| `beaten_by`                     | `"3/4 length"`                                                                            | Distance the runner was beaten by. Null if the runner won.        |
| `weight`                        | `"8st 13lbs"`                                                                             | Weight carried by the horse.                                      |
| `or_rating`                     | `66`                                                                                      | Official rating of the horse at the time of the race.             |
| `m_cloth_number`                | `10`                                                                                      | Cloth or saddlecloth number in the historical race.               |
| `bred`                          | `"IRE"`                                                                                   | Country where the horse was bred.                                 |
| `max_speed`                     | `39.468002`                                                                               | Maximum recorded speed for the runner in the race.                |
| `avg_speed`                     | `30.74415`                                                                                | Average recorded speed for the runner in the race.                |
| `trainer_id`                    | `162239`                                                                                  | Trainer ID.                                                       |
| `jockey_id`                     | `1188563`                                                                                 | Jockey ID.                                                        |
| `casualty_reason`               | `null`                                                                                    | Reason for casualty, withdrawal, or non-completion, if available. |
| `jockey_name`                   | `"Jack Doughty"`                                                                          | Jockey name for the historical race.                              |
| `trainer_name`                  | `"Charlie Clover"`                                                                        | Trainer name for the historical race.                             |
| `runner_name`                   | `"Poppy Foxy"`                                                                            | Horse/runner name in the historical race.                         |
| `race_type`                     | `"Flat"`                                                                                  | Type of race.                                                     |
| `race_name`                     | `"Juddmonte EBF Restricted Novice Stakes (GBB Race)"`                                     | Full race name.                                                   |
| `furlongs`                      | `"6f"`                                                                                    | Race distance expressed in furlongs.                              |
| `m_runner_winnings`             | `906`                                                                                     | Winnings earned by the runner in that race.                       |
| `winning_horse`                 | `"Treasurer"`                                                                             | Name of the winning horse.                                        |
| `winning_jockey`                | `"D Egan"`                                                                                | Name of the winning jockey.                                       |
| `winning_trainer`               | `"C Fellowes"`                                                                            | Name of the winning trainer.                                      |
| `win_horse_id`                  | `4352414`                                                                                 | Horse ID of the winning horse.                                    |
| `winning_bred`                  | `"IRE"`                                                                                   | Country where the winning horse was bred.                         |
| `winning_breeding_dam_bred`     | `"IRE"`                                                                                   | Country where the winning horse’s dam was bred.                   |
| `winning_breeding_sire_bred`    | `"IRE"`                                                                                   | Country where the winning horse’s sire was bred.                  |
| `winning_breeding_dam_name`     | `"Laureldean Lady"`                                                                       | Dam name of the winning horse.                                    |
| `winning_breeding_sire_name`    | `"Persian Force"`                                                                         | Sire name of the winning horse.                                   |
| `winning_breeding_damsire_name` | `"Statue Of Liberty"`                                                                     | Damsire name of the winning horse.                                |
| `winning_breeding_damsire_bred` | `"USA"`                                                                                   | Country where the winning horse’s damsire was bred.               |

---

# Model Usage

## Model Version: `v1`

| Column                                         | Used in v1? | Why   |
| ---------------------------------------------- | ----------- | ----- |
| `runner_name`                                  | `Yes/No`    | `TBC` |
| `m_cloth_number`                               | `Yes/No`    | `TBC` |
| `horse_bred`                                   | `Yes/No`    | `TBC` |
| `position`                                     | `Yes/No`    | `TBC` |
| `pa_horse_id`                                  | `Yes/No`    | `TBC` |
| `last_6_results`                               | `Yes/No`    | `TBC` |
| `last_6_results.date`                          | `Yes/No`    | `TBC` |
| `last_6_results.venue`                         | `Yes/No`    | `TBC` |
| `last_6_results.distance`                      | `Yes/No`    | `TBC` |
| `last_6_results.status`                        | `Yes/No`    | `TBC` |
| `last_6_results.sk_race_id`                    | `Yes/No`    | `TBC` |
| `last_6_results.going`                         | `Yes/No`    | `TBC` |
| `last_6_results.finish_position`               | `Yes/No`    | `TBC` |
| `last_6_results.group`                         | `Yes/No`    | `TBC` |
| `last_6_results.time_name`                     | `Yes/No`    | `TBC` |
| `last_6_results.handicap`                      | `Yes/No`    | `TBC` |
| `last_6_results.race_eligibility`              | `Yes/No`    | `TBC` |
| `last_6_results.commentary`                    | `Yes/No`    | `TBC` |
| `last_6_results.position`                      | `Yes/No`    | `TBC` |
| `last_6_results.race_group`                    | `Yes/No`    | `TBC` |
| `last_6_results.m_runner_count`                | `Yes/No`    | `TBC` |
| `last_6_results.class`                         | `Yes/No`    | `TBC` |
| `last_6_results.going_brief_advanced`          | `Yes/No`    | `TBC` |
| `last_6_results.sp`                            | `Yes/No`    | `TBC` |
| `last_6_results.beaten_by`                     | `Yes/No`    | `TBC` |
| `last_6_results.weight`                        | `Yes/No`    | `TBC` |
| `last_6_results.or_rating`                     | `Yes/No`    | `TBC` |
| `last_6_results.m_cloth_number`                | `Yes/No`    | `TBC` |
| `last_6_results.bred`                          | `Yes/No`    | `TBC` |
| `last_6_results.max_speed`                     | `Yes/No`    | `TBC` |
| `last_6_results.avg_speed`                     | `Yes/No`    | `TBC` |
| `last_6_results.trainer_id`                    | `Yes/No`    | `TBC` |
| `last_6_results.jockey_id`                     | `Yes/No`    | `TBC` |
| `last_6_results.casualty_reason`               | `Yes/No`    | `TBC` |
| `last_6_results.jockey_name`                   | `Yes/No`    | `TBC` |
| `last_6_results.trainer_name`                  | `Yes/No`    | `TBC` |
| `last_6_results.runner_name`                   | `Yes/No`    | `TBC` |
| `last_6_results.race_type`                     | `Yes/No`    | `TBC` |
| `last_6_results.race_name`                     | `Yes/No`    | `TBC` |
| `last_6_results.furlongs`                      | `Yes/No`    | `TBC` |
| `last_6_results.m_runner_winnings`             | `Yes/No`    | `TBC` |
| `last_6_results.winning_horse`                 | `Yes/No`    | `TBC` |
| `last_6_results.winning_jockey`                | `Yes/No`    | `TBC` |
| `last_6_results.winning_trainer`               | `Yes/No`    | `TBC` |
| `last_6_results.win_horse_id`                  | `Yes/No`    | `TBC` |
| `last_6_results.winning_bred`                  | `Yes/No`    | `TBC` |
| `last_6_results.winning_breeding_dam_bred`     | `Yes/No`    | `TBC` |
| `last_6_results.winning_breeding_sire_bred`    | `Yes/No`    | `TBC` |
| `last_6_results.winning_breeding_dam_name`     | `Yes/No`    | `TBC` |
| `last_6_results.winning_breeding_sire_name`    | `Yes/No`    | `TBC` |
| `last_6_results.winning_breeding_damsire_name` | `Yes/No`    | `TBC` |
| `last_6_results.winning_breeding_damsire_bred` | `Yes/No`    | `TBC` |
