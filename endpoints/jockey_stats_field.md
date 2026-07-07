# `/race-cards/jockey-stats-field`

## Endpoint

```http
GET /race-cards/jockey-stats-field
```

## Description

Returns jockey statistics based on the field size of the current race. Each item represents one runner and includes the jockey’s historical performance in races with a similar runner count.

---

## Columns

| Column             | Example Value      | Explanation                                                                               |
| ------------------ | ------------------ | ----------------------------------------------------------------------------------------- |
| `jockey_id`        | `"1154425"`        | Unique jockey ID.                                                                         |
| `jockey_name`      | `"K Shoemark"`     | Name of the jockey.                                                                       |
| `m_runner_count`   | `"8"`              | Number of runners in the current race or field-size group used for the jockey statistics. |
| `m_cloth_number`   | `1`                | Cloth or saddlecloth number for the current runner.                                       |
| `current_position` | `null`             | Current or finishing position, if available.                                              |
| `runner_name`      | `"Poppy Foxy"`     | Name of the horse/runner.                                                                 |
| `commentary`       | `null`             | Race commentary, if available.                                                            |
| `m_drawn_stall`    | `6`                | Stall draw number for the current runner.                                                 |
| `status`           | `"Runner"`         | Runner status.                                                                            |
| `bred`             | `"IRE"`            | Country where the horse was bred.                                                         |
| `age`              | `2`                | Horse age.                                                                                |
| `weight`           | `"9st 9lbs"`       | Weight carried by the horse.                                                              |
| `rating_offical`   | `65`               | Official rating. Field name appears as `offical` in API.                                  |
| `casualty_reason`  | `null`             | Reason for casualty, withdrawal, or non-runner status, if available.                      |
| `trainer_name`     | `"Charlie Clover"` | Name of the trainer.                                                                      |
| `winnings_cur`     | `"GBP"`            | Currency used for winnings.                                                               |
| `trainer_id`       | `"162239"`         | Unique trainer ID.                                                                        |
| `race_country`     | `"England"`        | Country where the race is taking place.                                                   |
| `topSpeed`         | `null`             | Top speed value, if available.                                                            |
| `price`            | `null`             | Betting price or odds, if available.                                                      |
| `runs`             | `"732"`            | Number of jockey runs in this field-size group.                                           |
| `wins`             | `"90"`             | Number of jockey wins in this field-size group.                                           |
| `Win %`            | `"12%"`            | Jockey win percentage in this field-size group.                                           |
| `place`            | `"269"`            | Number of jockey places in this field-size group.                                         |
| `Place %`          | `"37%"`            | Jockey place percentage in this field-size group.                                         |
| `total_winnings`   | `"2012572"`        | Total winnings for the jockey in this field-size group.                                   |

---

# Model Usage

## Model Version: `v1`

| Column             | Used in v1? | Why   |
| ------------------ | ----------- | ----- |
| `jockey_id`        | `Yes/No`    | `TBC` |
| `jockey_name`      | `Yes/No`    | `TBC` |
| `m_runner_count`   | `Yes/No`    | `TBC` |
| `m_cloth_number`   | `Yes/No`    | `TBC` |
| `current_position` | `Yes/No`    | `TBC` |
| `runner_name`      | `Yes/No`    | `TBC` |
| `commentary`       | `Yes/No`    | `TBC` |
| `m_drawn_stall`    | `Yes/No`    | `TBC` |
| `status`           | `Yes/No`    | `TBC` |
| `bred`             | `Yes/No`    | `TBC` |
| `age`              | `Yes/No`    | `TBC` |
| `weight`           | `Yes/No`    | `TBC` |
| `rating_offical`   | `Yes/No`    | `TBC` |
| `casualty_reason`  | `Yes/No`    | `TBC` |
| `trainer_name`     | `Yes/No`    | `TBC` |
| `winnings_cur`     | `Yes/No`    | `TBC` |
| `trainer_id`       | `Yes/No`    | `TBC` |
| `race_country`     | `Yes/No`    | `TBC` |
| `topSpeed`         | `Yes/No`    | `TBC` |
| `price`            | `Yes/No`    | `TBC` |
| `runs`             | `Yes/No`    | `TBC` |
| `wins`             | `Yes/No`    | `TBC` |
| `Win %`            | `Yes/No`    | `TBC` |
| `place`            | `Yes/No`    | `TBC` |
| `Place %`          | `Yes/No`    | `TBC` |
| `total_winnings`   | `Yes/No`    | `TBC` |
