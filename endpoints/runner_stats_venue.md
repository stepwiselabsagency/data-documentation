# `/race-cards/runner-stats-venue`

## Endpoint

```http id="9i5yfc"
GET /race-cards/runner-stats-venue
```

## Description

Returns runner statistics based on the race venue of the current race. Each item represents one horse/runner and includes the runner’s historical performance at the same venue.

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
| `race_venue`           | `"Pontefract"`                  | Racecourse/venue used for the runner statistics.                     |
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
| `runs`                 | `"0"`                           | Number of runner runs at this venue.                                 |
| `wins`                 | `"0"`                           | Number of runner wins at this venue.                                 |
| `Win %`                | `"0%"`                          | Runner win percentage at this venue.                                 |
| `place`                | `"0"`                           | Number of runner places at this venue.                               |
| `Place %`              | `"0%"`                          | Runner place percentage at this venue.                               |
| `total_winnings`       | `"0"`                           | Total winnings for the runner at this venue.                         |

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
| `race_venue`           | `Yes/No`    | `TBC` |
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
