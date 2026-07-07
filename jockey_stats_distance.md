# `/race-cards/jockey-stats-distance`

## Endpoint

```http id="8l3xqw"
GET /race-cards/jockey-stats-distance
```

## Description

Returns jockey statistics for the race distance of the current runner. Each item represents one runner and includes the jockey’s historical performance over the same distance/furlong range.

---

## Columns

| Column             | Example Value      | Explanation                                                          |
| ------------------ | ------------------ | -------------------------------------------------------------------- |
| `jockey_id`        | `"1154425"`        | Unique jockey ID.                                                    |
| `jockey_name`      | `"K Shoemark"`     | Name of the jockey.                                                  |
| `furlongs`         | `"6f"`             | Race distance used for the jockey statistics.                        |
| `m_cloth_number`   | `1`                | Cloth or saddlecloth number for the current runner.                  |
| `current_position` | `null`             | Current or finishing position, if available.                         |
| `runner_name`      | `"Poppy Foxy"`     | Name of the horse/runner.                                            |
| `commentary`       | `null`             | Race commentary, if available.                                       |
| `m_drawn_stall`    | `6`                | Stall draw number for the current runner.                            |
| `status`           | `null`             | Runner status, if available.                                         |
| `bred`             | `"IRE"`            | Country where the horse was bred.                                    |
| `age`              | `2`                | Horse age.                                                           |
| `weight`           | `"9 9"`            | Weight carried by the horse.                                         |
| `rating_offical`   | `65`               | Official rating. Field name appears as `offical` in API.             |
| `casualty_reason`  | `null`             | Reason for casualty, withdrawal, or non-runner status, if available. |
| `trainer_name`     | `"Charlie Clover"` | Name of the trainer.                                                 |
| `winnings_cur`     | `"GBP"`            | Currency used for winnings.                                          |
| `trainer_id`       | `"162239"`         | Unique trainer ID.                                                   |
| `race_country`     | `"England"`        | Country where the race is taking place.                              |
| `topSpeed`         | `null`             | Top speed value, if available.                                       |
| `price`            | `null`             | Betting price or odds, if available.                                 |
| `runs`             | `"964"`            | Number of jockey runs over this race distance.                       |
| `wins`             | `"107"`            | Number of jockey wins over this race distance.                       |
| `Win %`            | `"11%"`            | Jockey win percentage over this race distance.                       |
| `place`            | `"296"`            | Number of jockey places over this race distance.                     |
| `Place %`          | `"31%"`            | Jockey place percentage over this race distance.                     |
| `total_winnings`   | `"1661335"`        | Total winnings for the jockey over this race distance.               |

---

# Model Usage

## Model Version: `v1`

| Column             | Used in v1? | Why   |
| ------------------ | ----------- | ----- |
| `jockey_id`        | `Yes/No`    | `TBC` |
| `jockey_name`      | `Yes/No`    | `TBC` |
| `furlongs`         | `Yes/No`    | `TBC` |
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
