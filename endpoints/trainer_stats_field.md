# `/race-cards/trainer-stats-field`

## Endpoint

```http id="kf7m2d"
GET /race-cards/trainer-stats-field
```

## Description

Returns trainer statistics based on the field size of the current race. Each item represents one horse/runner and includes the trainer’s historical performance in races with the same or matching number of runners.

For example, if the current race has `8` runners, the `runs`, `wins`, `Win %`, `place`, `Place %`, and `total_winnings` fields describe how the trainer has performed historically in races with an 8-runner field.

---

## Columns

| Column             | Example Value      | Explanation                                                          |
| ------------------ | ------------------ | -------------------------------------------------------------------- |
| `trainer_id`       | `"162239"`         | Unique trainer ID.                                                   |
| `trainer_name`     | `"Charlie Clover"` | Name of the trainer.                                                 |
| `jockey_id`        | `"1154425"`        | Unique jockey ID.                                                    |
| `jockey_name`      | `"K Shoemark"`     | Name of the jockey.                                                  |
| `pa_horse_id`      | `"4344154"`        | Horse ID from the racing data provider.                              |
| `runner_name`      | `"Poppy Foxy"`     | Name of the horse/runner.                                            |
| `bred`             | `"IRE"`            | Country where the horse was bred.                                    |
| `m_drawn_stall`    | `6`                | Stall draw number for the runner.                                    |
| `commentary`       | `null`             | Race commentary, if available.                                       |
| `age`              | `2`                | Horse age.                                                           |
| `weight`           | `"9st 9lbs"`       | Weight carried by the horse.                                         |
| `casualty_reason`  | `null`             | Reason for casualty, withdrawal, or non-runner status, if available. |
| `rating_offical`   | `65`               | Official rating. Field name appears as `offical` in API.             |
| `m_cloth_number`   | `1`                | Cloth or saddlecloth number for the runner.                          |
| `winnings_cur`     | `"GBP"`            | Currency used for winnings.                                          |
| `current_position` | `null`             | Current or finishing position, if available.                         |
| `status`           | `"Runner"`         | Runner status, if available.                                         |
| `race_country`     | `"England"`        | Country where the race is taking place.                              |
| `m_runner_count`   | `"8"`              | Number of runners in the race, used for the trainer statistics.      |
| `topSpeed`         | `null`             | Top speed value, if available.                                       |
| `price`            | `null`             | Betting price or odds, if available.                                 |
| `runs`             | `"30"`             | Number of trainer runs in races with this field size.                |
| `wins`             | `"7"`              | Number of trainer wins in races with this field size.                |
| `Win %`            | `"23%"`            | Trainer win percentage in races with this field size.                |
| `place`            | `"12"`             | Number of trainer places in races with this field size.              |
| `Place %`          | `"40%"`            | Trainer place percentage in races with this field size.              |
| `total_winnings`   | `"45908"`          | Total trainer winnings in races with this field size.                |

---

# Model Usage

## Model Version: `v1`

| Column             | Used in v1? | Why   |
| ------------------ | ----------- | ----- |
| `trainer_id`       | `Yes/No`    | `TBC` |
| `trainer_name`     | `Yes/No`    | `TBC` |
| `jockey_id`        | `Yes/No`    | `TBC` |
| `jockey_name`      | `Yes/No`    | `TBC` |
| `pa_horse_id`      | `Yes/No`    | `TBC` |
| `runner_name`      | `Yes/No`    | `TBC` |
| `bred`             | `Yes/No`    | `TBC` |
| `m_drawn_stall`    | `Yes/No`    | `TBC` |
| `commentary`       | `Yes/No`    | `TBC` |
| `age`              | `Yes/No`    | `TBC` |
| `weight`           | `Yes/No`    | `TBC` |
| `casualty_reason`  | `Yes/No`    | `TBC` |
| `rating_offical`   | `Yes/No`    | `TBC` |
| `m_cloth_number`   | `Yes/No`    | `TBC` |
| `winnings_cur`     | `Yes/No`    | `TBC` |
| `current_position` | `Yes/No`    | `TBC` |
| `status`           | `Yes/No`    | `TBC` |
| `race_country`     | `Yes/No`    | `TBC` |
| `m_runner_count`   | `Yes/No`    | `TBC` |
| `topSpeed`         | `Yes/No`    | `TBC` |
| `price`            | `Yes/No`    | `TBC` |
| `runs`             | `Yes/No`    | `TBC` |
| `wins`             | `Yes/No`    | `TBC` |
| `Win %`            | `Yes/No`    | `TBC` |
| `place`            | `Yes/No`    | `TBC` |
| `Place %`          | `Yes/No`    | `TBC` |
| `total_winnings`   | `Yes/No`    | `TBC` |
