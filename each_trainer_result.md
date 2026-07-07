# `/race-cards/each-trainer-result`

## Endpoint

```http id="bdh1w8"
GET /race-cards/each-trainer-result
```

## Description

Returns recent result history for a trainer. Each item in the response represents one trainer and contains a `last_6_results` list with recent race results linked to that trainer.

---

## Columns

### Top-Level Columns

| Column           | Example Value      | Explanation                                                                           |
| ---------------- | ------------------ | ------------------------------------------------------------------------------------- |
| `trainer_id`     | `"162239"`         | Unique trainer ID.                                                                    |
| `trainer_name`   | `"Charlie Clover"` | Name of the trainer.                                                                  |
| `last_6_results` | `[ {...}, {...} ]` | List of recent race results related to the trainer. Usually contains up to 6 records. |

---

### `last_6_results` Columns

| Column                          | Example Value                                                                                                                                                                | Explanation                                                       |
| ------------------------------- | ---------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | ----------------------------------------------------------------- |
| `date`                          | `"2026-07-04"`                                                                                                                                                               | Date of the historical race.                                      |
| `venue`                         | `"Nottingham"`                                                                                                                                                               | Racecourse or venue name.                                         |
| `distance`                      | `"1m 6f 0y"`                                                                                                                                                                 | Race distance in miles, furlongs, and yards.                      |
| `sk_race_id`                    | `22088149`                                                                                                                                                                   | Unique race ID for the historical race.                           |
| `going`                         | `"Good to Firm (Good in places)"`                                                                                                                                            | Official going/ground condition.                                  |
| `status`                        | `"Runner"`                                                                                                                                                                   | Runner status in that historical race.                            |
| `race_group`                    | `"2026-07-04 19:30 Nottingham"`                                                                                                                                              | Combined race date, time, and venue label.                        |
| `time_name`                     | `"19:30"`                                                                                                                                                                    | Race start time.                                                  |
| `pa_horse_id`                   | `4192139`                                                                                                                                                                    | Horse ID from the racing data provider.                           |
| `handicap`                      | `"Yes"`                                                                                                                                                                      | Indicates whether the race was a handicap.                        |
| `position`                      | `"2"`                                                                                                                                                                        | Finishing position of the runner.                                 |
| `class`                         | `"6"`                                                                                                                                                                        | Race class.                                                       |
| `commentary`                    | `"held up in rear, pushed along over 4f out, ridden and headway over 2f out, went second over 1f out, clear with winner inside final furlong, kept on, held towards finish"` | In-running commentary for the runner.                             |
| `sp`                            | `"10/11"`                                                                                                                                                                    | Starting price odds.                                              |
| `beaten_by`                     | `"Neck"`                                                                                                                                                                     | Distance the runner was beaten by. Null if the runner won.        |
| `weight`                        | `"9st 9lbs"`                                                                                                                                                                 | Weight carried by the horse.                                      |
| `or_rating`                     | `65`                                                                                                                                                                         | Official rating of the horse at the time of the race.             |
| `m_cloth_number`                | `1`                                                                                                                                                                          | Cloth or saddlecloth number of the runner.                        |
| `runner_name`                   | `"Jack Langley"`                                                                                                                                                             | Name of the horse/runner.                                         |
| `bred`                          | `"GB"`                                                                                                                                                                       | Country where the horse was bred.                                 |
| `m_runner_count`                | `6`                                                                                                                                                                          | Number of runners in the race.                                    |
| `casualty_reason`               | `null`                                                                                                                                                                       | Reason for casualty, withdrawal, or non-completion, if available. |
| `max_speed`                     | `38.4842`                                                                                                                                                                    | Maximum recorded speed for the runner in the race.                |
| `avg_speed`                     | `30.294043`                                                                                                                                                                  | Average recorded speed for the runner in the race.                |
| `jockey_name`                   | `"Rowan Scott"`                                                                                                                                                              | Jockey name for the historical race.                              |
| `trainer_name`                  | `"Charlie Clover"`                                                                                                                                                           | Trainer name for the historical race.                             |
| `race_type`                     | `"Flat"`                                                                                                                                                                     | Type of race.                                                     |
| `race_name`                     | `"Nottingham's Finest Ale Mile Handicap"`                                                                                                                                    | Full race name.                                                   |
| `furlongs`                      | `"14f"`                                                                                                                                                                      | Race distance expressed in furlongs.                              |
| `winning_horse`                 | `"Chambers"`                                                                                                                                                                 | Name of the winning horse.                                        |
| `winning_jockey`                | `"T Eaves"`                                                                                                                                                                  | Name of the winning jockey.                                       |
| `winning_trainer`               | `"Faye Bramley"`                                                                                                                                                             | Name of the winning trainer.                                      |
| `win_horse_id`                  | `4167655`                                                                                                                                                                    | Horse ID of the winning horse.                                    |
| `winning_bred`                  | `"IRE"`                                                                                                                                                                      | Country where the winning horse was bred.                         |
| `winning_breeding_dam_bred`     | `"IRE"`                                                                                                                                                                      | Country where the winning horse’s dam was bred.                   |
| `winning_breeding_sire_bred`    | `"IRE"`                                                                                                                                                                      | Country where the winning horse’s sire was bred.                  |
| `winning_breeding_dam_name`     | `"Estemaala"`                                                                                                                                                                | Dam name of the winning horse.                                    |
| `winning_breeding_sire_name`    | `"Inns Of Court"`                                                                                                                                                            | Sire name of the winning horse.                                   |
| `winning_breeding_damsire_name` | `"Cape Cross"`                                                                                                                                                               | Damsire name of the winning horse.                                |
| `winning_breeding_damsire_bred` | `"IRE"`                                                                                                                                                                      | Country where the winning horse’s damsire was bred.               |

---

# Model Usage

## Model Version: `v1`

| Column                                         | Used in v1? | Why   |
| ---------------------------------------------- | ----------- | ----- |
| `trainer_id`                                   | `Yes/No`    | `TBC` |
| `trainer_name`                                 | `Yes/No`    | `TBC` |
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
