# `/race-cards/each-jockey-result`

## Endpoint

```http
GET /race-cards/each-jockey-result
```

## Description

Returns recent result history for a jockey. Each item in the response represents one jockey and contains a `last_6_results` list with the jockey’s recent race results.

---

## Columns

### Top-Level Columns

| Column           | Example Value      | Explanation                                                                          |
| ---------------- | ------------------ | ------------------------------------------------------------------------------------ |
| `jockey_name`    | `"K Shoemark"`     | Name of the jockey for whom recent results are returned.                             |
| `jockey_id`      | `"1154425"`        | Unique jockey ID.                                                                    |
| `last_6_results` | `[ {...}, {...} ]` | List of recent race results related to the jockey. Usually contains up to 6 records. |

---

### `last_6_results` Columns

| Column                          | Example Value                                          | Explanation                                                                             |
| ------------------------------- | ------------------------------------------------------ | --------------------------------------------------------------------------------------- |
| `date`                          | `"2026-07-04"`                                         | Date of the race.                                                                       |
| `venue`                         | `"Sandown"`                                            | Racecourse or venue name.                                                               |
| `distance`                      | `"1m 0f 0y"`                                           | Race distance in miles, furlongs, and yards.                                            |
| `sk_race_id`                    | `22088178`                                             | Unique race ID.                                                                         |
| `going`                         | `"Good to Firm (Good in places)"`                      | Official going/ground condition for the race.                                           |
| `status`                        | `"Runner"`                                             | Runner status in the race, for example `Runner` or `NonRunner`.                         |
| `race_group`                    | `"2026-07-04 14:25 Sandown"`                           | Combined race date, time, and venue label.                                              |
| `time_name`                     | `"14:25"`                                              | Race start time.                                                                        |
| `pa_horse_id`                   | `4200759`                                              | Horse ID from the racing data provider.                                                 |
| `handicap`                      | `"Yes"`                                                | Indicates whether the race was a handicap.                                              |
| `position`                      | `"13"`                                                 | Finishing position of the runner. Null if the horse was a non-runner or did not finish. |
| `class`                         | `"2"`                                                  | Race class.                                                                             |
| `commentary`                    | `"midfield, ridden over 2f out, weakened over 1f out"` | In-running race commentary for the runner.                                              |
| `sp`                            | `"14/1"`                                               | Starting price odds.                                                                    |
| `beaten_by`                     | `"4 1/2 lengths"`                                      | Distance the runner was beaten by. Null if the runner won or did not run.               |
| `weight`                        | `"9st 5lbs"`                                           | Weight carried by the horse.                                                            |
| `or_rating`                     | `103`                                                  | Official rating of the horse at the time of the race.                                   |
| `m_cloth_number`                | `4`                                                    | Cloth or saddlecloth number of the runner.                                              |
| `runner_name`                   | `"Excellent Believe"`                                  | Name of the horse/runner.                                                               |
| `bred`                          | `"GB"`                                                 | Country where the horse was bred.                                                       |
| `m_runner_count`                | `14`                                                   | Number of runners in the race.                                                          |
| `casualty_reason`               | `null`                                                 | Reason for casualty, withdrawal, or non-completion, if available.                       |
| `max_speed`                     | `38.84558`                                             | Maximum recorded speed for the runner in the race.                                      |
| `avg_speed`                     | `30.651615`                                            | Average recorded speed for the runner in the race.                                      |
| `jockey_name`                   | `"James Doyle"`                                        | Jockey name for this specific historical result record.                                 |
| `trainer_name`                  | `"J Channon"`                                          | Trainer name for this specific historical result record.                                |
| `race_type`                     | `"Flat"`                                               | Type of race.                                                                           |
| `race_name`                     | `"Coral Challenge (Handicap)"`                         | Full race name.                                                                         |
| `furlongs`                      | `"8f"`                                                 | Race distance expressed in furlongs.                                                    |
| `winning_horse`                 | `"Indalo"`                                             | Name of the winning horse in the race.                                                  |
| `winning_jockey`                | `"Ray Dawson"`                                         | Name of the winning jockey in the race.                                                 |
| `winning_trainer`               | `"R Varian"`                                           | Name of the winning trainer in the race.                                                |
| `win_horse_id`                  | `4079068`                                              | Horse ID of the winning horse.                                                          |
| `winning_bred`                  | `"IRE"`                                                | Country where the winning horse was bred.                                               |
| `winning_breeding_dam_bred`     | `"FR"`                                                 | Country where the winning horse’s dam was bred.                                         |
| `winning_breeding_sire_bred`    | `"IRE"`                                                | Country where the winning horse’s sire was bred.                                        |
| `winning_breeding_dam_name`     | `"Pearly Empress"`                                     | Dam name of the winning horse.                                                          |
| `winning_breeding_sire_name`    | `"Phoenix Of Spain"`                                   | Sire name of the winning horse.                                                         |
| `winning_breeding_damsire_name` | `"Holy Roman Emperor"`                                 | Damsire name of the winning horse.                                                      |
| `winning_breeding_damsire_bred` | `"IRE"`                                                | Country where the winning horse’s damsire was bred.                                     |

---

# Model Usage

## Model Version: `v1`

| Column                                         | Used in v1? | Why   |
| ---------------------------------------------- | ----------- | ----- |
| `jockey_name`                                  | `Yes/No`    | `TBC` |
| `jockey_id`                                    | `Yes/No`    | `TBC` |
| `last_6_results`                               | `Yes/No`    | `TBC` |
| `last_6_results.date`                          | `Yes/No`    | `TBC` |
| `last_6_results.venue`                         | `Yes/No`    | `TBC` |
| `last_6_results.distance`                      | `Yes/No`    | `TBC` |
| `last_6_results.sk_race_id`                    | `Yes/No`    | `TBC` |
| `last_6_results.going`                         | `Yes/No`    | `TBC` |
| `last_6_results.status`                        | `Yes/No`    | `TBC` |
| `last_6_results.race_group`                    | `Yes/No`    | `TBC` |
| `last_6_results.time_name`                     | `Yes/No`    | `TBC` |
| `last_6_results.pa_horse_id`                   | `Yes/No`    | `TBC` |
| `last_6_results.handicap`                      | `Yes/No`    | `TBC` |
| `last_6_results.position`                      | `Yes/No`    | `TBC` |
| `last_6_results.class`                         | `Yes/No`    | `TBC` |
| `last_6_results.commentary`                    | `Yes/No`    | `TBC` |
| `last_6_results.sp`                            | `Yes/No`    | `TBC` |
| `last_6_results.beaten_by`                     | `Yes/No`    | `TBC` |
| `last_6_results.weight`                        | `Yes/No`    | `TBC` |
| `last_6_results.or_rating`                     | `Yes/No`    | `TBC` |
| `last_6_results.m_cloth_number`                | `Yes/No`    | `TBC` |
| `last_6_results.runner_name`                   | `Yes/No`    | `TBC` |
| `last_6_results.bred`                          | `Yes/No`    | `TBC` |
| `last_6_results.m_runner_count`                | `Yes/No`    | `TBC` |
| `last_6_results.casualty_reason`               | `Yes/No`    | `TBC` |
| `last_6_results.max_speed`                     | `Yes/No`    | `TBC` |
| `last_6_results.avg_speed`                     | `Yes/No`    | `TBC` |
| `last_6_results.jockey_name`                   | `Yes/No`    | `TBC` |
| `last_6_results.trainer_name`                  | `Yes/No`    | `TBC` |
| `last_6_results.race_type`                     | `Yes/No`    | `TBC` |
| `last_6_results.race_name`                     | `Yes/No`    | `TBC` |
| `last_6_results.furlongs`                      | `Yes/No`    | `TBC` |
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
