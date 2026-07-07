# `/race-cards/trainer-stats-going`

## Endpoint

```http id="r6z2kt"
GET /race-cards/trainer-stats-going
```

## Description

Returns trainer statistics based on the going/ground conditions of the current race. Each item represents one horse/runner and includes the trainer’s historical performance on the same or matching going.

For example, if the current going is `Good-good to firm in places`, the `runs`, `wins`, `Win %`, `place`, `Place %`, and `total_winnings` fields describe how the trainer has performed historically under similar going conditions.

---

## Columns

| Column                 | Example Value                   | Explanation                                                          |
| ---------------------- | ------------------------------- | -------------------------------------------------------------------- |
| `trainer_id`           | `"162239"`                      | Unique trainer ID.                                                   |
| `trainer_name`         | `"Charlie Clover"`              | Name of the trainer.                                                 |
| `jockey_id`            | `"1154425"`                     | Unique jockey ID.                                                    |
| `jockey_name`          | `"K Shoemark"`                  | Name of the jockey.                                                  |
| `pa_horse_id`          | `"4344154"`                     | Horse ID from the racing data provider.                              |
| `runner_name`          | `"Poppy Foxy"`                  | Name of the horse/runner.                                            |
| `bred`                 | `"IRE"`                         | Country where the horse was bred.                                    |
| `m_drawn_stall`        | `6`                             | Stall draw number for the runner.                                    |
| `commentary`           | `null`                          | Race commentary, if available.                                       |
| `age`                  | `2`                             | Horse age.                                                           |
| `weight`               | `"9 9"`                         | Weight carried by the horse.                                         |
| `casualty_reason`      | `null`                          | Reason for casualty, withdrawal, or non-runner status, if available. |
| `rating_offical`       | `65`                            | Official rating. Field name appears as `offical` in API.             |
| `m_cloth_number`       | `1`                             | Cloth or saddlecloth number for the runner.                          |
| `winnings_cur`         | `"GBP"`                         | Currency used for winnings.                                          |
| `current_position`     | `null`                          | Current or finishing position, if available.                         |
| `status`               | `null`                          | Runner status, if available.                                         |
| `race_country`         | `"England"`                     | Country where the race is taking place.                              |
| `going_brief_advanced` | `"Good-good to firm in places"` | Going/ground condition used for the trainer statistics.              |
| `topSpeed`             | `null`                          | Top speed value, if available.                                       |
| `price`                | `null`                          | Betting price or odds, if available.                                 |
| `runs`                 | `"1"`                           | Number of trainer runs under this going condition.                   |
| `wins`                 | `"0"`                           | Number of trainer wins under this going condition.                   |
| `Win %`                | `"0%"`                          | Trainer win percentage under this going condition.                   |
| `place`                | `"0"`                           | Number of trainer places under this going condition.                 |
| `Place %`              | `"0%"`                          | Trainer place percentage under this going condition.                 |
| `total_winnings`       | `"0"`                           | Total trainer winnings under this going condition.                   |

---

# Model Usage

## Model Version: `v1`

| Column                 | Used in v1? | Why   |
| ---------------------- | ----------- | ----- |
| `trainer_id`           | `Yes/No`    | `TBC` |
| `trainer_name`         | `Yes/No`    | `TBC` |
| `jockey_id`            | `Yes/No`    | `TBC` |
| `jockey_name`          | `Yes/No`    | `TBC` |
| `pa_horse_id`          | `Yes/No`    | `TBC` |
| `runner_name`          | `Yes/No`    | `TBC` |
| `bred`                 | `Yes/No`    | `TBC` |
| `m_drawn_stall`        | `Yes/No`    | `TBC` |
| `commentary`           | `Yes/No`    | `TBC` |
| `age`                  | `Yes/No`    | `TBC` |
| `weight`               | `Yes/No`    | `TBC` |
| `casualty_reason`      | `Yes/No`    | `TBC` |
| `rating_offical`       | `Yes/No`    | `TBC` |
| `m_cloth_number`       | `Yes/No`    | `TBC` |
| `winnings_cur`         | `Yes/No`    | `TBC` |
| `current_position`     | `Yes/No`    | `TBC` |
| `status`               | `Yes/No`    | `TBC` |
| `race_country`         | `Yes/No`    | `TBC` |
| `going_brief_advanced` | `Yes/No`    | `TBC` |
| `topSpeed`             | `Yes/No`    | `TBC` |
| `price`                | `Yes/No`    | `TBC` |
| `runs`                 | `Yes/No`    | `TBC` |
| `wins`                 | `Yes/No`    | `TBC` |
| `Win %`                | `Yes/No`    | `TBC` |
| `place`                | `Yes/No`    | `TBC` |
| `Place %`              | `Yes/No`    | `TBC` |
| `total_winnings`       | `Yes/No`    | `TBC` |
