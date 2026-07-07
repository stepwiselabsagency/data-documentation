# `/race-cards/jockey-stats-going`

## Endpoint

```http id="2x8ng6"
GET /race-cards/jockey-stats-going
```

## Description

Returns jockey statistics based on the going/ground condition of the current race. Each item represents one runner and includes the jockey’s historical performance on the same or similar going.

---

## Columns

| Column                 | Example Value                   | Explanation                                                          |
| ---------------------- | ------------------------------- | -------------------------------------------------------------------- |
| `jockey_id`            | `"1154425"`                     | Unique jockey ID.                                                    |
| `jockey_name`          | `"K Shoemark"`                  | Name of the jockey.                                                  |
| `going_brief_advanced` | `"Good-good to firm in places"` | Going/ground condition used for the jockey statistics.               |
| `m_cloth_number`       | `1`                             | Cloth or saddlecloth number for the current runner.                  |
| `current_position`     | `null`                          | Current or finishing position, if available.                         |
| `runner_name`          | `"Poppy Foxy"`                  | Name of the horse/runner.                                            |
| `commentary`           | `null`                          | Race commentary, if available.                                       |
| `m_drawn_stall`        | `6`                             | Stall draw number for the current runner.                            |
| `status`               | `null`                          | Runner status, if available.                                         |
| `bred`                 | `"IRE"`                         | Country where the horse was bred.                                    |
| `age`                  | `2`                             | Horse age.                                                           |
| `weight`               | `"9 9"`                         | Weight carried by the horse.                                         |
| `rating_offical`       | `65`                            | Official rating. Field name appears as `offical` in API.             |
| `casualty_reason`      | `null`                          | Reason for casualty, withdrawal, or non-runner status, if available. |
| `trainer_name`         | `"Charlie Clover"`              | Name of the trainer.                                                 |
| `winnings_cur`         | `"GBP"`                         | Currency used for winnings.                                          |
| `trainer_id`           | `"162239"`                      | Unique trainer ID.                                                   |
| `race_country`         | `"England"`                     | Country where the race is taking place.                              |
| `topSpeed`             | `null`                          | Top speed value, if available.                                       |
| `price`                | `null`                          | Betting price or odds, if available.                                 |
| `runs`                 | `"132"`                         | Number of jockey runs on this going/ground condition.                |
| `wins`                 | `"13"`                          | Number of jockey wins on this going/ground condition.                |
| `Win %`                | `"10%"`                         | Jockey win percentage on this going/ground condition.                |
| `place`                | `"42"`                          | Number of jockey places on this going/ground condition.              |
| `Place %`              | `"32%"`                         | Jockey place percentage on this going/ground condition.              |
| `total_winnings`       | `"249658"`                      | Total winnings for the jockey on this going/ground condition.        |

---

# Model Usage

## Model Version: `v1`

| Column                 | Used in v1? | Why   |
| ---------------------- | ----------- | ----- |
| `jockey_id`            | `Yes/No`    | `TBC` |
| `jockey_name`          | `Yes/No`    | `TBC` |
| `going_brief_advanced` | `Yes/No`    | `TBC` |
| `m_cloth_number`       | `Yes/No`    | `TBC` |
| `current_position`     | `Yes/No`    | `TBC` |
| `runner_name`          | `Yes/No`    | `TBC` |
| `commentary`           | `Yes/No`    | `TBC` |
| `m_drawn_stall`        | `Yes/No`    | `TBC` |
| `status`               | `Yes/No`    | `TBC` |
| `bred`                 | `Yes/No`    | `TBC` |
| `age`                  | `Yes/No`    | `TBC` |
| `weight`               | `Yes/No`    | `TBC` |
| `rating_offical`       | `Yes/No`    | `TBC` |
| `casualty_reason`      | `Yes/No`    | `TBC` |
| `trainer_name`         | `Yes/No`    | `TBC` |
| `winnings_cur`         | `Yes/No`    | `TBC` |
| `trainer_id`           | `Yes/No`    | `TBC` |
| `race_country`         | `Yes/No`    | `TBC` |
| `topSpeed`             | `Yes/No`    | `TBC` |
| `price`                | `Yes/No`    | `TBC` |
| `runs`                 | `Yes/No`    | `TBC` |
| `wins`                 | `Yes/No`    | `TBC` |
| `Win %`                | `Yes/No`    | `TBC` |
| `place`                | `Yes/No`    | `TBC` |
| `Place %`              | `Yes/No`    | `TBC` |
| `total_winnings`       | `Yes/No`    | `TBC` |
