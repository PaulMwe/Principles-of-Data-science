# Question 1 — Frailty Analysis

## Ingest
The raw ten-participant frailty table was saved as `data/frailty_raw.csv`.

## Process
Height was standardized from inches to meters using 0.0254 m/in. Weight was standardized from pounds to kilograms using 0.45359237 kg/lb. BMI was engineered as weight in kilograms divided by height in meters squared and rounded to two decimals. AgeGroup was created using the required categories `<30`, `30–45`, `46–60`, and `>60`. Frailty was binary encoded as Y=1 and N=0 using integer type int8, and AgeGroup was one-hot encoded into the four requested columns.

## Analyze
### Numeric summary
| Column        |   Mean | Median | Std  |
|---------------|--------|--------|------|
| Height_in     | 68.60  | 68.45  | 1.67 |
| Weight_lb     | 131.90 | 136.00 | 14.23|
| Age_yr        | 32.50  | 29.50  | 12.86|
| Grip_kg       | 26.00  | 27.00  | 4.52 |
| Height_m      | 1.74   | 1.74   | 0.04 |
| Weight_kg     | 59.83  | 61.69  | 6.46 |
| BMI           | 19.68  | 19.19  | 1.78 |
| Frailty_binary| 0.40   | 0.00   | 0.52 |
| AgeGroup_<30  | 0.50   | 0.50   | 0.53 |
| AgeGroup_30–45| 0.30   | 0.00   | 0.48 |
| AgeGroup_46–60| 0.20   | 0.00   | 0.42 |
| AgeGroup_>60  | 0.00   | 0.00   | 0.00 |

### Grip strength ↔ frailty
The Pearson correlation between `Grip_kg` and `Frailty_binary` is **-0.4759**. The negative value indicates that, in this small dataset, higher grip strength tends to be associated with the non-frail category (Frailty_binary=0), while lower grip strength tends to be associated with the frail category (Frailty_binary=1).
