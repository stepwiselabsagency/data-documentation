# Data Documentation

Documentation for race-cards and results-analysis API endpoints. Each endpoint has its own markdown file in [`endpoints/`](endpoints/) with column definitions, example values, and model variable selection.

## Who this is for

### Documenting columns and variables

Use this when you need to explain what an endpoint returns — field names, example values, and what each column means.

1. Open the endpoint file from the [index below](#endpoint-index).
2. Work in the **Columns** section at the top of the file.
3. Add or update the `Explanation` column for any field that needs clarification.
4. For nested objects (e.g. `last_6_results`, `sector_data`), document each sub-table separately.

### Selecting variables for a model version

Use this when you are choosing which fields feed a specific model version and documenting why.

1. Open the endpoint file from the [index below](#endpoint-index).
2. Scroll to the **Model Usage** section at the bottom of the file.
3. For each model version (currently `v1`), set **Used in v1?** to `Yes` or `No`.
4. Fill in **Why** with a short rationale (predictive value, data quality, leakage risk, etc.).
5. Add a new `## Model Version: \`v2\`` block when a new model version is introduced.

## Endpoint index

### Race cards — core

| Endpoint | Documentation | Description |
| -------- | ------------- | ----------- |
| `GET /race-cards/race-report` | [race_report.md](endpoints/race_report.md) | Runner-level race report records for a racecard |
| `GET /race-cards/runner-form` | [runner_form.md](endpoints/runner_form.md) | Form data for each runner (horse, jockey, trainer) |
| `GET /race-cards/historical-data` | [historical_data.md](endpoints/historical_data.md) | Historical runner performance with sectional/sector data |
| `GET /race-cards/historic-results` | [historic_results.md](endpoints/historic_results.md) | Historic race results |

### Race cards — entity result history

| Endpoint | Documentation | Description |
| -------- | ------------- | ----------- |
| `GET /race-cards/each-runner-result` | [each_runner_result.md](endpoints/each_runner_result.md) | Recent result history per runner (`last_6_results`) |
| `GET /race-cards/each-jockey-result` | [each_jockey_result.md](endpoints/each_jockey_result.md) | Recent result history per jockey |
| `GET /race-cards/each-trainer-result` | [each_trainer_result.md](endpoints/each_trainer_result.md) | Recent result history per trainer |

### Race cards — runner stats

| Endpoint | Documentation | Description |
| -------- | ------------- | ----------- |
| `GET /race-cards/runner-stats-venue` | [runner_stats_venue.md](endpoints/runner_stats_venue.md) | Runner performance at the current race venue |
| `GET /race-cards/runner-stats-type` | [runner_stats_type.md](endpoints/runner_stats_type.md) | Runner performance by race type |
| `GET /race-cards/runner-stats-going` | [runner_stats_going.md](endpoints/runner_stats_going.md) | Runner performance by going/ground condition |
| `GET /race-cards/runner-stats-field` | [runner_stats_field.md](endpoints/runner_stats_field.md) | Runner performance by field size |
| `GET /race-cards/runner-stats-distance` | [runner_stats_distance.md](endpoints/runner_stats_distance.md) | Runner performance by distance |
| `GET /race-cards/runner-stats-class` | [runner_stats_class.md](endpoints/runner_stats_class.md) | Runner performance by race class |

### Race cards — jockey stats

| Endpoint | Documentation | Description |
| -------- | ------------- | ----------- |
| `GET /race-cards/jockey-stats-venue` | [jockey_stats_venue.md](endpoints/jockey_stats_venue.md) | Jockey performance at the current race venue |
| `GET /race-cards/jockey-stats-type` | [jockey_stats_type.md](endpoints/jockey_stats_type.md) | Jockey performance by race type |
| `GET /race-cards/jockey-stats-going` | [jockey_stats_going.md](endpoints/jockey_stats_going.md) | Jockey performance by going/ground condition |
| `GET /race-cards/jockey-stats-field` | [jockey_stats_field.md](endpoints/jockey_stats_field.md) | Jockey performance by field size |
| `GET /race-cards/jockey-stats-distance` | [jockey_stats_distance.md](endpoints/jockey_stats_distance.md) | Jockey performance by distance |
| `GET /race-cards/jockey-stats-class` | [jockey_stats_class.md](endpoints/jockey_stats_class.md) | Jockey performance by race class |

### Race cards — trainer stats

| Endpoint | Documentation | Description |
| -------- | ------------- | ----------- |
| `GET /race-cards/trainer-stats-venue` | [trainer_stats_venue.md](endpoints/trainer_stats_venue.md) | Trainer performance at the current race venue |
| `GET /race-cards/trainer-stats-type` | [trainer_stats_type.md](endpoints/trainer_stats_type.md) | Trainer performance by race type |
| `GET /race-cards/trainer-stats-going` | [trainer_stats_going.md](endpoints/trainer_stats_going.md) | Trainer performance by going/ground condition |
| `GET /race-cards/trainer-stats-field` | [trainer_stats_field.md](endpoints/trainer_stats_field.md) | Trainer performance by field size |
| `GET /race-cards/trainer-stats-distance` | [trainer_stats_distance.md](endpoints/trainer_stats_distance.md) | Trainer performance by distance |
| `GET /race-cards/trainer-stats-class` | [trainer_stats_class.md](endpoints/trainer_stats_class.md) | Trainer performance by race class |

### Results analysis

| Endpoint | Documentation | Description |
| -------- | ------------- | ----------- |
| `GET /results-analysis/top-cards` | [results_analysis_top_cards.md](endpoints/results_analysis_top_cards.md) | Top-level race card/result analysis for a race |

## File structure

Each file in `endpoints/` follows the same layout:

```
# `/path/to/endpoint`

## Endpoint          ← HTTP method and path
## Description       ← what the endpoint returns
## Columns           ← field table(s) with Example Value and Explanation
# Model Usage        ← per-model-version variable selection (Yes/No + Why)
```

## Contributing

- Keep column explanations factual and tied to the API response shape.
- When marking a variable as used in a model, always fill in the **Why** column — do not leave `TBC` once a decision is made.
- Add new endpoint docs as `{endpoint_name}.md` in `endpoints/` and link them from this README.
