# `/race-cards/runner-stats-field`

## Endpoint

```http id="wnnij4"
GET /race-cards/runner-stats-field
```

## Description

Returns runner statistics based on the field size of the current race. Each item represents one horse/runner and includes the runner’s historical performance in races with the same or similar runner count.

---

## Columns

| Column                 | Example Value                     | Explanation                                                                               |
| ---------------------- | --------------------------------- | ----------------------------------------------------------------------------------------- |
| `pa_horse_id`          | `"4344154"`                       | Horse ID from the racing data provider.                                                   |
| `runner_name`          | `"Poppy Foxy"`                    | Name of the horse/runner.                                                                 |
| `bred`                 | `"IRE"`                           | Country where the horse was bred.                                                         |
| `m_cloth_number`       | `1`                               | Cloth or saddlecloth number for the runner.                                               |
| `current_position`     | `null`                            | Current or finishing position, if available.                                              |
| `casualty_reason`      | `null`                            | Reason for casualty, withdrawal, or non-runner status, if available.                      |
| `commentary`           | `null`                            | Race commentary, if available.                                                            |
| `horse_age`            | `"2"`                             | Horse age.                                                                                |
| `going_brief`          | `"Good"`                          | Short going/ground description.                                                           |
| `advanced_going`       | `"Good-good to firm in places"`   | Advanced going/ground description.                                                        |
| `going_brief_advanced` | `"Good (Good to Firm in places)"` | Detailed going/ground description.                                                        |
| `m_runner_count`       | `"8"`                             | Number of runners in the current race or field-size group used for the runner statistics. |
| `m_drawn_stall`        | `6`                               | Stall draw number for the runner.                                                         |
| `status`               | `"Runner"`                        | Runner status.                                                                            |
| `weight`               | `"9st 9lbs"`                      | Weight carried by the horse.                                                              |
| `rating_offical`       | `65`                              | Official rating. Field name appears as `offical` in API.                                  |
| `topSpeed`             | `null`                            | Top speed value, if available.                                                            |
| `trainer_name`         | `"Charlie Clover"`                | Name of the trainer.                                                                      |
| `trainer_id`           | `"162239"`                        | Unique trainer ID.                                                                        |
| `jockey_name`          | `"K Shoemark"`                    | Name of the jockey.                                                                       |
| `jockey_id`            | `"1154425"`                       | Unique jockey ID.                                                                         |
| `race_country`         | `"England"`                       | Country where the race is taking place.                                                   |
| `price`                | `null`                            | Betting price or odds, if available.                                                      |
| `winnings_cur`         | `"GBP"`                           | Currency used for winnings.                                                               |
| `runs`                 | `"1"`                             | Number of runner runs in this field-size group.                                           |
| `wins`                 | `"0"`                             | Number of runner wins in this field-size group.                                           |
| `Win %`                | `"0%"`                            | Runner win percentage in this field-size group.                                           |
| `place`                | `"0"`                             | Number of runner places in this field-size group.                                         |
| `Place %`              | `"0%"`                            | Runner place percentage in this field-size group.                                         |
| `total_winnings`       | `"0"`                             | Total winnings for the runner in this field-size group.                                   |

---

# Model Usage

## Model Version: `v1`

| Column                 | Used in v1? | Why   |
| ---------------------- | ----------- | ----- |
| `pa_horse_id`          | `Yes/No`    | `TBC` |
| `runner_name`          | `Yes/No`    | `TBC` |
| `bred`                 | `Yes/No`    | `TBC` |
| `m_cloth_number`       | `Yes/No`    | `TBC` |
| `current_position`     | `Yes/No`    | `TBC` |
| `casualty_reason`      | `Yes/No`    | `TBC` |
| `commentary`           | `Yes/No`    | `TBC` |
| `horse_age`            | `Yes/No`    | `TBC` |
| `going_brief`          | `Yes/No`    | `TBC` |
| `advanced_going`       | `Yes/No`    | `TBC` |
| `going_brief_advanced` | `Yes/No`    | `TBC` |
| `m_runner_count`       | `Yes/No`    | `TBC` |
| `m_drawn_stall`        | `Yes/No`    | `TBC` |
| `status`               | `Yes/No`    | `TBC` |
| `weight`               | `Yes/No`    | `TBC` |
| `rating_offical`       | `Yes/No`    | `TBC` |
| `topSpeed`             | `Yes/No`    | `TBC` |
| `trainer_name`         | `Yes/No`    | `TBC` |
| `trainer_id`           | `Yes/No`    | `TBC` |
| `jockey_name`          | `Yes/No`    | `TBC` |
| `jockey_id`            | `Yes/No`    | `TBC` |
| `race_country`         | `Yes/No`    | `TBC` |
| `price`                | `Yes/No`    | `TBC` |
| `winnings_cur`         | `Yes/No`    | `TBC` |
| `runs`                 | `Yes/No`    | `TBC` |
| `wins`                 | `Yes/No`    | `TBC` |
| `Win %`                | `Yes/No`    | `TBC` |
| `place`                | `Yes/No`    | `TBC` |
| `Place %`              | `Yes/No`    | `TBC` |
| `total_winnings`       | `Yes/No`    | `TBC` |
