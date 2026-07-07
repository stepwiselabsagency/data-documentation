# `/race-cards/runner-form`

## Endpoint

```http
GET /race-cards/runner-form
```

## Description

Returns form-related information for each runner in a race. Each item represents one horse/runner and includes recent horse form, jockey form, trainer form, and basic runner details.

---

## Columns

| Column             | Example Value                | Explanation                                                          |
| ------------------ | ---------------------------- | -------------------------------------------------------------------- |
| `pa_horse_id`      | `"4344154"`                  | Horse ID from the racing data provider.                              |
| `runner_name`      | `"Poppy Foxy"`               | Name of the horse/runner.                                            |
| `bred`             | `"IRE"`                      | Country where the horse was bred.                                    |
| `m_drawn_stall`    | `6`                          | Stall draw number for the runner.                                    |
| `m_cloth_number`   | `1`                          | Cloth or saddlecloth number for the runner.                          |
| `current_position` | `null`                       | Current or finishing position, if available.                         |
| `casualty_reason`  | `null`                       | Reason for casualty, withdrawal, or non-runner status, if available. |
| `status`           | `null`                       | Runner status, if available.                                         |
| `age`              | `"2"`                        | Horse age.                                                           |
| `weight`           | `"9 9"`                      | Weight carried by the horse.                                         |
| `rating_offical`   | `65`                         | Official rating. Field name appears as `offical` in API.             |
| `trainer_name`     | `"Charlie Clover"`           | Name of the trainer.                                                 |
| `jockey_name`      | `"K Shoemark"`               | Name of the jockey.                                                  |
| `price`            | `null`                       | Betting price or odds, if available.                                 |
| `race_date`        | `"2026-07-07T00:00:00.000Z"` | Date of the race.                                                    |
| `Form`             | `"5.16"`                     | Recent form for the horse/runner.                                    |
| `Jockey Form`      | `"241647"`                   | Recent form for the jockey.                                          |
| `Trainer Form`     | `"248641"`                   | Recent form for the trainer.                                         |
| `topSpeed`         | `"0 mph"`                    | Top speed value, if available.                                       |

---

# Model Usage

## Model Version: `v1`

| Column             | Used in v1? | Why   |
| ------------------ | ----------- | ----- |
| `pa_horse_id`      | `Yes/No`    | `TBC` |
| `runner_name`      | `Yes/No`    | `TBC` |
| `bred`             | `Yes/No`    | `TBC` |
| `m_drawn_stall`    | `Yes/No`    | `TBC` |
| `m_cloth_number`   | `Yes/No`    | `TBC` |
| `current_position` | `Yes/No`    | `TBC` |
| `casualty_reason`  | `Yes/No`    | `TBC` |
| `status`           | `Yes/No`    | `TBC` |
| `age`              | `Yes/No`    | `TBC` |
| `weight`           | `Yes/No`    | `TBC` |
| `rating_offical`   | `Yes/No`    | `TBC` |
| `trainer_name`     | `Yes/No`    | `TBC` |
| `jockey_name`      | `Yes/No`    | `TBC` |
| `price`            | `Yes/No`    | `TBC` |
| `race_date`        | `Yes/No`    | `TBC` |
| `Form`             | `Yes/No`    | `TBC` |
| `Jockey Form`      | `Yes/No`    | `TBC` |
| `Trainer Form`     | `Yes/No`    | `TBC` |
| `topSpeed`         | `Yes/No`    | `TBC` |
