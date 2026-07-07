# `/race-cards/runner-stats-type`

## Endpoint

```http id="ruj3id"
GET /race-cards/runner-stats-type
```

## Description

Returns runner statistics based on the race type of the current race. Each item represents one horse/runner and includes the runner’s historical performance for the same race type.

---

## Columns

| Column                 | Example Value                   | Explanation                                                          |
| ---------------------- | ------------------------------- | -------------------------------------------------------------------- |
| `pa_horse_id`          | `"4344154"`                     | Horse ID from the racing data provider.                              |
| `runner_name`          | `"Poppy Foxy"`                  | Name of the horse/runner.                                            |
| `bred`                 | `"IRE"`                         | Country where the horse was bred.                                    |
| `m_cloth_number`       | `1`                             | Cloth or saddlecloth number for the runner.                          |
| `current_position`     | `null`                          | Current or finishing position, if available.                         |
| `casualty_reason`      | `null`                          | Reason for casualty, withdrawal, or non-runner status, if available. |
| `commentary`           | `null`                          | Race commentary, if available.                                       |
| `horse_age`            | `"2"`                           | Horse age.                                                           |
| `going_brief`          | `null`                          | Short going/ground description, if available.                        |
| `advanced_going`       | `"Good-good to firm in places"` | Advanced going/ground description.                                   |
| `going_brief_advanced` | `"Good-good to firm in places"` | Detailed going/ground description.                                   |
| `race_type`            | `"Flat"`                        | Race type used for the runner statistics.                            |
| `m_drawn_stall`        | `6`                             | Stall draw number for the runner.                                    |
| `status`               | `null`                          | Runner status, if available.                                         |
| `weight`               | `"9 9"`                         | Weight carried by the horse.                                         |
| `rating_offical`       | `65`                            | Official rating. Field name appears as `offical` in API.             |
| `topSpeed`             | `null`                          | Top speed value, if available.                                       |
| `trainer_name`         | `"Charlie Clover"`              | Name of the trainer.                                                 |
| `trainer_id`           | `"162239"`                      | Unique trainer ID.                                                   |
| `jockey_name`          | `"K Shoemark"`                  | Name of the jockey.                                                  |
| `jockey_id`            | `"1154425"`                     | Unique jockey ID.                                                    |
| `race_country`         | `"England"`                     | Country where the race is taking place.                              |
| `price`                | `null`                          | Betting price or odds, if available.                                 |
| `winnings_cur`         | `"GBP"`                         | Currency used for winnings.                                          |
| `runs`                 | `"5"`                           | Number of runner runs for this race type.                            |
| `wins`                 | `"2"`                           | Number of runner wins for this race type.                            |
| `Win %`                | `"40%"`                         | Runner win percentage for this race type.                            |
| `place`                | `"2"`                           | Number of runner places for this race type.                          |
| `Place %`              | `"40%"`                         | Runner place percentage for this race type.                          |
| `total_winnings`       | `"26676"`                       | Total winnings for the runner for this race type.                    |

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
| `race_type`            | `Yes/No`    | `TBC` |
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
