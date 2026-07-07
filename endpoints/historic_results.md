# `/race-cards/historic-results`

## Endpoint

```http
GET /race-cards/historic-results
```

## Description

Returns historical race result records. Each item represents one runner/horse result from a past race, including race details, runner details, betting/tote values, form, jockey/trainer details, and final result information.

---

## Columns

| Column                      | Example Value                                                 | Explanation                                                           |
| --------------------------- | ------------------------------------------------------------- | --------------------------------------------------------------------- |
| `sk_race_id`                | `"22052975"`                                                  | Unique race ID.                                                       |
| `pa_horse_id`               | `"3832414"`                                                   | Horse ID from the racing data provider.                               |
| `race_country`              | `"England"`                                                   | Country where the race took place.                                    |
| `country_code`              | `null`                                                        | Country code, if available.                                           |
| `race_date`                 | `"2026-06-29T00:00:00.000Z"`                                  | Date of the race.                                                     |
| `race_name`                 | `"Wilfred Underwood Memorial Handicap"`                       | Full race name.                                                       |
| `race_distance`             | `"0m 6f 0y"`                                                  | Race distance in miles, furlongs, and yards.                          |
| `race_class`                | `"6"`                                                         | Race class.                                                           |
| `race_type`                 | `"Flat"`                                                      | Type of race.                                                         |
| `winnings_cur`              | `"GBP"`                                                       | Currency used for race winnings.                                      |
| `race_group`                | `"2026-06-29 17:00 Pontefract"`                               | Combined race date, time, and venue label.                            |
| `race_track`                | `"Turf"`                                                      | Race track surface/type.                                              |
| `race_venue`                | `"Pontefract"`                                                | Racecourse or venue name.                                             |
| `furlongs`                  | `"6f"`                                                        | Race distance expressed in furlongs.                                  |
| `runners`                   | `"8"`                                                         | Number of runners in the race.                                        |
| `max_runners`               | `17`                                                          | Maximum allowed runners for the race.                                 |
| `going`                     | `"Good (Good to Firm in places)"`                             | Official going/ground condition.                                      |
| `status`                    | `"Runner"`                                                    | Runner status in the race.                                            |
| `casualty_reason`           | `null`                                                        | Reason for casualty, withdrawal, or non-completion, if available.     |
| `win_time`                  | `"0116.14"`                                                   | Winning time for the race.                                            |
| `m_winnings_1`              | `3402`                                                        | Prize money for first place.                                          |
| `m_winnings_2`              | `1596`                                                        | Prize money for second place.                                         |
| `m_winnings_3`              | `798`                                                         | Prize money for third place.                                          |
| `race_handicap`             | `"Yes"`                                                       | Indicates whether the race was a handicap.                            |
| `no`                        | `2`                                                           | Runner number on the racecard.                                        |
| `draw`                      | `8`                                                           | Stall draw number.                                                    |
| `position`                  | `"1"`                                                         | Final finishing position of the runner.                               |
| `race_eligibility`          | `"3YO plus"`                                                  | Race eligibility condition.                                           |
| `Horse`                     | `"Ideal Guest"`                                               | Horse name.                                                           |
| `sire`                      | `"Shalaa"`                                                    | Horse’s sire.                                                         |
| `dam`                       | `"Rue Renan"`                                                 | Horse’s dam.                                                          |
| `beaten_distance`           | `null`                                                        | Distance the runner was beaten by. Null if the runner won.            |
| `bred`                      | `"FR"`                                                        | Country where the horse was bred.                                     |
| `tote_trifecta_cur`         | `"GBP"`                                                       | Currency for tote trifecta value.                                     |
| `tote_trifecta_val`         | `46.1`                                                        | Tote trifecta dividend/value.                                         |
| `tote_exata_cur`            | `"GBP"`                                                       | Currency for tote exacta value. Field name appears as `exata` in API. |
| `tote_exacta_val`           | `8.6`                                                         | Tote exacta dividend/value.                                           |
| `tote_place_cur`            | `"GBP"`                                                       | Currency for tote place value.                                        |
| `tote_place_val`            | `1.1`                                                         | Tote place dividend/value.                                            |
| `tote_win_cur`              | `"GBP"`                                                       | Currency for tote win value.                                          |
| `tote_win_val`              | `2.63`                                                        | Tote win dividend/value.                                              |
| `m_places_paid`             | `3`                                                           | Number of places paid.                                                |
| `going_brief_advanced`      | `"Good (Good to Firm in places)"`                             | Detailed going/ground description.                                    |
| `age`                       | `7`                                                           | Horse age.                                                            |
| `weight`                    | `"9st 12lbs"`                                                 | Weight carried by the horse.                                          |
| `jwp`                       | `"5"`                                                         | JWP value, if available.                                              |
| `rating_offical`            | `56`                                                          | Official rating. Field name appears as `offical` in API.              |
| `topSpeed`                  | `"39.217674 mph"`                                             | Top speed value.                                                      |
| `price`                     | `"13/8"`                                                      | Betting price or odds.                                                |
| `bet_movements`             | `"op 9/4"`                                                    | Betting market movement information.                                  |
| `last_6_finish_positions_h` | `"4_3_5324552___81_3133475.8761252"`                          | Encoded recent finishing position history for the horse.              |
| `m_last_rundays_flat`       | `8`                                                           | Days since the horse last ran on flat.                                |
| `tackle_type`               | `"Hood"`                                                      | Tack/headgear/equipment used by the horse.                            |
| `formfigures_flatsix`       | `"350-304"`                                                   | Recent flat-race form figures.                                        |
| `formfigures_jumpsix`       | `null`                                                        | Recent jumps-race form figures, if available.                         |
| `jockey_id`                 | `"1182945"`                                                   | Jockey ID.                                                            |
| `jockey_name`               | `"Ethan Tindall"`                                             | Jockey name.                                                          |
| `m_tg_runner`               | `"6"`                                                         | Number of trainer-jockey runners/races.                               |
| `sire_bred`                 | `"IRE"`                                                       | Country where the sire was bred.                                      |
| `dam_bred`                  | `"IRE"`                                                       | Country where the dam was bred.                                       |
| `m_finpos_1`                | `1`                                                           | Indicates/counts first-place finish for this result.                  |
| `m_tg_placed`               | `"4"`                                                         | Number of trainer-jockey placed runs.                                 |
| `jockey_form`               | `"545597"`                                                    | Recent jockey form.                                                   |
| `trainer_form`              | `"148954"`                                                    | Recent trainer form.                                                  |
| `trainer_name`              | `"H Bethell"`                                                 | Trainer name.                                                         |
| `jt_form`                   | `"354111"`                                                    | Recent jockey-trainer form.                                           |
| `m_tg_finpos_1`             | `"3"`                                                         | Number of trainer-jockey wins.                                        |
| `trainerjockeyraceswins`    | `"6 races, 3 wins"`                                           | Trainer-jockey race and win summary.                                  |
| `trainer_jockey_places`     | `"4Placed"`                                                   | Trainer-jockey places summary.                                        |
| `comments`                  | `"went early to post, made all, ridden over 1f out, kept on"` | Race comment for the runner.                                          |
| `m_beaten_favourite`        | `0`                                                           | Indicates whether the horse was a beaten favourite.                   |
| `bet_csf_val`               | `7.53`                                                        | Computer straight forecast value.                                     |
| `bet_csf_cur`               | `"GBP"`                                                       | Currency for computer straight forecast value.                        |
| `tote_win_numbers`          | `"2"`                                                         | Winning tote number.                                                  |
| `tote_place_numbers`        | `"2, 1, 7"`                                                   | Tote place numbers.                                                   |
| `tote_exata_numbers`        | `"2-1"`                                                       | Tote exacta numbers. Field name appears as `exata` in API.            |
| `tote_trifecta_numbers`     | `"2-1-7"`                                                     | Tote trifecta numbers.                                                |
| `bet_csf_numbers`           | `"2-1"`                                                       | Computer straight forecast numbers.                                   |
| `c_win`                     | `"C"`                                                         | Course win indicator.                                                 |
| `d_win`                     | `"D"`                                                         | Distance win indicator.                                               |
| `cd_win`                    | `"CD"`                                                        | Course-and-distance win indicator.                                    |

---

# Model Usage

## Model Version: `v1`

| Column                      | Used in v1? | Why   |
| --------------------------- | ----------- | ----- |
| `sk_race_id`                | `Yes/No`    | `TBC` |
| `pa_horse_id`               | `Yes/No`    | `TBC` |
| `race_country`              | `Yes/No`    | `TBC` |
| `country_code`              | `Yes/No`    | `TBC` |
| `race_date`                 | `Yes/No`    | `TBC` |
| `race_name`                 | `Yes/No`    | `TBC` |
| `race_distance`             | `Yes/No`    | `TBC` |
| `race_class`                | `Yes/No`    | `TBC` |
| `race_type`                 | `Yes/No`    | `TBC` |
| `winnings_cur`              | `Yes/No`    | `TBC` |
| `race_group`                | `Yes/No`    | `TBC` |
| `race_track`                | `Yes/No`    | `TBC` |
| `race_venue`                | `Yes/No`    | `TBC` |
| `furlongs`                  | `Yes/No`    | `TBC` |
| `runners`                   | `Yes/No`    | `TBC` |
| `max_runners`               | `Yes/No`    | `TBC` |
| `going`                     | `Yes/No`    | `TBC` |
| `status`                    | `Yes/No`    | `TBC` |
| `casualty_reason`           | `Yes/No`    | `TBC` |
| `win_time`                  | `Yes/No`    | `TBC` |
| `m_winnings_1`              | `Yes/No`    | `TBC` |
| `m_winnings_2`              | `Yes/No`    | `TBC` |
| `m_winnings_3`              | `Yes/No`    | `TBC` |
| `race_handicap`             | `Yes/No`    | `TBC` |
| `no`                        | `Yes/No`    | `TBC` |
| `draw`                      | `Yes/No`    | `TBC` |
| `position`                  | `Yes/No`    | `TBC` |
| `race_eligibility`          | `Yes/No`    | `TBC` |
| `Horse`                     | `Yes/No`    | `TBC` |
| `sire`                      | `Yes/No`    | `TBC` |
| `dam`                       | `Yes/No`    | `TBC` |
| `beaten_distance`           | `Yes/No`    | `TBC` |
| `bred`                      | `Yes/No`    | `TBC` |
| `tote_trifecta_cur`         | `Yes/No`    | `TBC` |
| `tote_trifecta_val`         | `Yes/No`    | `TBC` |
| `tote_exata_cur`            | `Yes/No`    | `TBC` |
| `tote_exacta_val`           | `Yes/No`    | `TBC` |
| `tote_place_cur`            | `Yes/No`    | `TBC` |
| `tote_place_val`            | `Yes/No`    | `TBC` |
| `tote_win_cur`              | `Yes/No`    | `TBC` |
| `tote_win_val`              | `Yes/No`    | `TBC` |
| `m_places_paid`             | `Yes/No`    | `TBC` |
| `going_brief_advanced`      | `Yes/No`    | `TBC` |
| `age`                       | `Yes/No`    | `TBC` |
| `weight`                    | `Yes/No`    | `TBC` |
| `jwp`                       | `Yes/No`    | `TBC` |
| `rating_offical`            | `Yes/No`    | `TBC` |
| `topSpeed`                  | `Yes/No`    | `TBC` |
| `price`                     | `Yes/No`    | `TBC` |
| `bet_movements`             | `Yes/No`    | `TBC` |
| `last_6_finish_positions_h` | `Yes/No`    | `TBC` |
| `m_last_rundays_flat`       | `Yes/No`    | `TBC` |
| `tackle_type`               | `Yes/No`    | `TBC` |
| `formfigures_flatsix`       | `Yes/No`    | `TBC` |
| `formfigures_jumpsix`       | `Yes/No`    | `TBC` |
| `jockey_id`                 | `Yes/No`    | `TBC` |
| `jockey_name`               | `Yes/No`    | `TBC` |
| `m_tg_runner`               | `Yes/No`    | `TBC` |
| `sire_bred`                 | `Yes/No`    | `TBC` |
| `dam_bred`                  | `Yes/No`    | `TBC` |
| `m_finpos_1`                | `Yes/No`    | `TBC` |
| `m_tg_placed`               | `Yes/No`    | `TBC` |
| `jockey_form`               | `Yes/No`    | `TBC` |
| `trainer_form`              | `Yes/No`    | `TBC` |
| `trainer_name`              | `Yes/No`    | `TBC` |
| `jt_form`                   | `Yes/No`    | `TBC` |
| `m_tg_finpos_1`             | `Yes/No`    | `TBC` |
| `trainerjockeyraceswins`    | `Yes/No`    | `TBC` |
| `trainer_jockey_places`     | `Yes/No`    | `TBC` |
| `comments`                  | `Yes/No`    | `TBC` |
| `m_beaten_favourite`        | `Yes/No`    | `TBC` |
| `bet_csf_val`               | `Yes/No`    | `TBC` |
| `bet_csf_cur`               | `Yes/No`    | `TBC` |
| `tote_win_numbers`          | `Yes/No`    | `TBC` |
| `tote_place_numbers`        | `Yes/No`    | `TBC` |
| `tote_exata_numbers`        | `Yes/No`    | `TBC` |
| `tote_trifecta_numbers`     | `Yes/No`    | `TBC` |
| `bet_csf_numbers`           | `Yes/No`    | `TBC` |
| `c_win`                     | `Yes/No`    | `TBC` |
| `d_win`                     | `Yes/No`    | `TBC` |
| `cd_win`                    | `Yes/No`    | `TBC` |
