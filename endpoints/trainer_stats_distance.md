# `/race-cards/trainer-stats-distance`

## Endpoint

```http id="u97x0k"
GET /race-cards/trainer-stats-distance
```

## Description

Returns trainer statistics based on the race distance of the current race. Each item represents one horse/runner and includes the trainer’s historical performance over the same or matching race distance.

For example, if the current race distance is `6f`, the `runs`, `wins`, `Win %`, `place`, `Place %`, and `total_winnings` fields describe how the trainer has performed historically over 6 furlongs.

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
| `weight`           | `"9 9"`            | Weight carried by the horse.                                         |
| `casualty_reason`  | `null`             | Reason for casualty, withdrawal, or non-runner status, if available. |
| `rating_offical`   | `65`               | Official rating. Field name appears as `offical` in API.             |
| `m_cloth_number`   | `1`                | Cloth or saddlecloth number for the runner.                          |
| `winnings_cur`     | `"GBP"`            | Currency used for winnings.                                          |
| `current_position` | `null`             | Current or finishing position, if available.                         |
| `status`           | `null`             | Runner status, if available.                                         |
| `race_country`     | `"England"`        | Country where the race is taking place.                              |
| `furlongs`         | `"6f"`             | Race distance used for the trainer statistics.                       |
| `topSpeed`         | `null`             | Top speed value, if available.                                       |
| `price`            | `null`             | Betting price or odds, if available.                                 |
| `runs`             | `"48"`             | Number of trainer runs over this distance.                           |
| `wins`             | `"4"`              | Number of trainer wins over this distance.                           |
| `Win %`            | `"8%"`             | Trainer win percentage over this distance.                           |
| `place`            | `"12"`             | Number of trainer places over this distance.                         |
| `Place %`          | `"25%"`            | Trainer place percentage over this distance.                         |
| `total_winnings`   | `"40439"`          | Total trainer winnings over this distance.                           |

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
| `furlongs`         | `Yes/No`    | `TBC` |
| `topSpeed`         | `Yes/No`    | `TBC` |
| `price`            | `Yes/No`    | `TBC` |
| `runs`             | `Yes/No`    | `TBC` |
| `wins`             | `Yes/No`    | `TBC` |
| `Win %`            | `Yes/No`    | `TBC` |
| `place`            | `Yes/No`    | `TBC` |
| `Place %`          | `Yes/No`    | `TBC` |
| `total_winnings`   | `Yes/No`    | `TBC` |
