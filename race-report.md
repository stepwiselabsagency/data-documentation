# `/race-cards/race-report`

## Endpoint

```http
GET /race-cards/race-report
```

## Description

Returns a list of runner-level race report records. Each item in the response represents one horse/runner in a race.

---

## Columns

| Column                      | Example Value                   | Explanation                                                                    |
| --------------------------- | ------------------------------- | ------------------------------------------------------------------------------ |
| `sk_race_id`                | `"22110727"`                    | Unique race ID. Used to identify the race.                                     |
| `race_country`              | `"England"`                     | Country where the race is taking place.                                        |
| `sk_runner_id`              | `"253267350210"`                | Unique runner ID for the horse in this race.                                   |
| `race_status`               | `"Dormant"`                     | Current status of the race.                                                    |
| `country_code`              | `null`                          | Country code, if available.                                                    |
| `pa_horse_id`               | `"4344154"`                     | Horse ID from the racing data provider.                                        |
| `race_date`                 | `"2026-07-07T00:00:00.000Z"`    | Date of the race.                                                              |
| `race_group`                | `"2026-07-07 13:48 Pontefract"` | Combined race date, time, and venue label.                                     |
| `race_time_name`            | `"13:48"`                       | Race start time.                                                               |
| `status`                    | `null`                          | Runner status, if available.                                                   |
| `jockeycolours_filename`    | `"20260707pfr134801.png"`       | Jockey colours image filename.                                                 |
| `jockey_color`              | `"20260707pfr134801.png"`       | Jockey colour image filename.                                                  |
| `no`                        | `1`                             | Runner number on the racecard.                                                 |
| `draw`                      | `6`                             | Stall draw number.                                                             |
| `Horse`                     | `"Poppy Foxy"`                  | Horse name.                                                                    |
| `sire`                      | `"Bungle Inthejungle"`          | Horse’s sire.                                                                  |
| `dam`                       | `"Hayyel"`                      | Horse’s dam.                                                                   |
| `beaten_distance`           | `null`                          | Distance the horse was beaten by, usually available after the race.            |
| `tote_trifecta_cur`         | `null`                          | Tote trifecta current value, if available.                                     |
| `race_distance_yards`       | `"1320"`                        | Race distance in yards.                                                        |
| `tote_trifecta_val`         | `null`                          | Tote trifecta value, if available.                                             |
| `tote_exata_cur`            | `null`                          | Tote exacta current value, if available. Field name appears as `exata` in API. |
| `tote_exacta_val`           | `null`                          | Tote exacta value, if available.                                               |
| `tote_place_cur`            | `null`                          | Tote place current value, if available.                                        |
| `tote_place_val`            | `null`                          | Tote place value, if available.                                                |
| `tote_win_cur`              | `null`                          | Tote win current value, if available.                                          |
| `tote_win_val`              | `null`                          | Tote win value, if available.                                                  |
| `bred`                      | `"IRE"`                         | Country where the horse was bred.                                              |
| `casualty_reason`           | `null`                          | Reason for casualty, withdrawal, or non-runner status, if available.           |
| `age`                       | `"2"`                           | Horse age.                                                                     |
| `weight`                    | `"9 9"`                         | Weight carried by the horse. Usually stones and pounds.                        |
| `rating_offical`            | `65`                            | Official rating. Field name appears as `offical` in API.                       |
| `topSpeed`                  | `"0 mph"`                       | Top speed value, if available.                                                 |
| `jwp`                       | `null`                          | JWP value, if available.                                                       |
| `price`                     | `"9/4"`                         | Betting price or odds.                                                         |
| `bet_movements`             | `null`                          | Betting market movements, if available.                                        |
| `last_6_finish_positions_h` | `"5.16"`                        | Horse’s recent finishing position history.                                     |
| `m_last_rundays_flat`       | `7`                             | Days since the horse last ran on flat.                                         |
| `formfigures_flatsix`       | `"615"`                         | Recent flat-race form figures.                                                 |
| `formfigures_jumpsix`       | `null`                          | Recent jumps-race form figures.                                                |
| `tackle_type`               | `null`                          | Tack or equipment type, if available.                                          |
| `tackle_count`              | `null`                          | Tack or equipment count, if available.                                         |
| `jockey_id`                 | `"1154425"`                     | Jockey ID.                                                                     |
| `jockey_name`               | `"K Shoemark"`                  | Jockey name.                                                                   |
| `m_beaten_favourite`        | `0`                             | Indicates whether the horse was a beaten favourite.                            |
| `race_venue`                | `"Pontefract"`                  | Racecourse or venue name.                                                      |
| `m_tg_runner`               | `"14"`                          | Number of trainer-jockey runners/races.                                        |
| `race_type`                 | `"Flat"`                        | Type of race.                                                                  |
| `sire_bred`                 | `"UK"`                          | Country where the sire was bred.                                               |
| `dam_bred`                  | `"IRE"`                         | Country where the dam was bred.                                                |
| `m_tg_placed`               | `"6"`                           | Number of trainer-jockey placed runs.                                          |
| `jockey_form`               | `"241647"`                      | Recent jockey form.                                                            |
| `trainer_form`              | `"248641"`                      | Recent trainer form.                                                           |
| `trainer_id`                | `"162239"`                      | Trainer ID.                                                                    |
| `trainer_name`              | `"Charlie Clover"`              | Trainer name.                                                                  |
| `jt_form`                   | `"861211"`                      | Recent jockey-trainer form.                                                    |
| `m_tg_finpos_1`             | `"3"`                           | Number of trainer-jockey wins.                                                 |
| `trainerjockeyraceswins`    | `"14 races, 3 wins"`            | Trainer-jockey race and win summary.                                           |
| `trainer_jockey_places`     | `"6Placed"`                     | Trainer-jockey places summary.                                                 |
| `c_win`                     | `"-"`                           | Course win indicator.                                                          |
| `d_win`                     | `"-"`                           | Distance win indicator.                                                        |
| `cd_win`                    | `"-"`                           | Course-and-distance win indicator.                                             |
| `comments`                  | `null`                          | Additional comments, if available.                                             |

---

# Model Usage

## Model Version: `v1`

| Column                      | Used in v1? | Why   |
| --------------------------- | ----------- | ----- |
| `sk_race_id`                | `Yes/No`    | `TBC` |
| `race_country`              | `Yes/No`    | `TBC` |
| `sk_runner_id`              | `Yes/No`    | `TBC` |
| `race_status`               | `Yes/No`    | `TBC` |
| `country_code`              | `Yes/No`    | `TBC` |
| `pa_horse_id`               | `Yes/No`    | `TBC` |
| `race_date`                 | `Yes/No`    | `TBC` |
| `race_group`                | `Yes/No`    | `TBC` |
| `race_time_name`            | `Yes/No`    | `TBC` |
| `status`                    | `Yes/No`    | `TBC` |
| `jockeycolours_filename`    | `Yes/No`    | `TBC` |
| `jockey_color`              | `Yes/No`    | `TBC` |
| `no`                        | `Yes/No`    | `TBC` |
| `draw`                      | `Yes/No`    | `TBC` |
| `Horse`                     | `Yes/No`    | `TBC` |
| `sire`                      | `Yes/No`    | `TBC` |
| `dam`                       | `Yes/No`    | `TBC` |
| `beaten_distance`           | `Yes/No`    | `TBC` |
| `tote_trifecta_cur`         | `Yes/No`    | `TBC` |
| `race_distance_yards`       | `Yes/No`    | `TBC` |
| `tote_trifecta_val`         | `Yes/No`    | `TBC` |
| `tote_exata_cur`            | `Yes/No`    | `TBC` |
| `tote_exacta_val`           | `Yes/No`    | `TBC` |
| `tote_place_cur`            | `Yes/No`    | `TBC` |
| `tote_place_val`            | `Yes/No`    | `TBC` |
| `tote_win_cur`              | `Yes/No`    | `TBC` |
| `tote_win_val`              | `Yes/No`    | `TBC` |
| `bred`                      | `Yes/No`    | `TBC` |
| `casualty_reason`           | `Yes/No`    | `TBC` |
| `age`                       | `Yes/No`    | `TBC` |
| `weight`                    | `Yes/No`    | `TBC` |
| `rating_offical`            | `Yes/No`    | `TBC` |
| `topSpeed`                  | `Yes/No`    | `TBC` |
| `jwp`                       | `Yes/No`    | `TBC` |
| `price`                     | `Yes/No`    | `TBC` |
| `bet_movements`             | `Yes/No`    | `TBC` |
| `last_6_finish_positions_h` | `Yes/No`    | `TBC` |
| `m_last_rundays_flat`       | `Yes/No`    | `TBC` |
| `formfigures_flatsix`       | `Yes/No`    | `TBC` |
| `formfigures_jumpsix`       | `Yes/No`    | `TBC` |
| `tackle_type`               | `Yes/No`    | `TBC` |
| `tackle_count`              | `Yes/No`    | `TBC` |
| `jockey_id`                 | `Yes/No`    | `TBC` |
| `jockey_name`               | `Yes/No`    | `TBC` |
| `m_beaten_favourite`        | `Yes/No`    | `TBC` |
| `race_venue`                | `Yes/No`    | `TBC` |
| `m_tg_runner`               | `Yes/No`    | `TBC` |
| `race_type`                 | `Yes/No`    | `TBC` |
| `sire_bred`                 | `Yes/No`    | `TBC` |
| `dam_bred`                  | `Yes/No`    | `TBC` |
| `m_tg_placed`               | `Yes/No`    | `TBC` |
| `jockey_form`               | `Yes/No`    | `TBC` |
| `trainer_form`              | `Yes/No`    | `TBC` |
| `trainer_id`                | `Yes/No`    | `TBC` |
| `trainer_name`              | `Yes/No`    | `TBC` |
| `jt_form`                   | `Yes/No`    | `TBC` |
| `m_tg_finpos_1`             | `Yes/No`    | `TBC` |
| `trainerjockeyraceswins`    | `Yes/No`    | `TBC` |
| `trainer_jockey_places`     | `Yes/No`    | `TBC` |
| `c_win`                     | `Yes/No`    | `TBC` |
| `d_win`                     | `Yes/No`    | `TBC` |
| `cd_win`                    | `Yes/No`    | `TBC` |
| `comments`                  | `Yes/No`    | `TBC` |
