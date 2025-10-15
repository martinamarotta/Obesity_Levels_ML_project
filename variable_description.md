## Variables description
**The table below maps each variable from the original survey to its representation in the dataset and how it was used in the project.**

| Variable | Original Survey Options | Dataset Representation | Notes |
|---|---|---|---|
| **Gender** | Female, Male | Nominal: 0 = Female, 1 = Male |
  | **Age** | Numeric (years) | Continuous (years) |
| **Height** | Numeric (meters) | Continuous (m) | **Excluded from modeling** (leakage risk with BMI-based target) |
| **Weight** | Numeric (kg) | Continuous (kg) | **Excluded from modeling** (leakage risk with BMI-based target) |
| **family_history_with_overweight** | Yes, No | Binary: 1 = Yes, 0 = No |
| **FAVC** (Frequent consumption of high-caloric food) | Yes, No | Binary: 1 = Yes, 0 = No | 
| **FCVC** (Frequency of consumption of vegetables) | Never, Sometimes, Always | Ordinal: 1 = Never, 2 = Sometimes, 3 = Always | 
| **NCP** (Number of main meals) | 1–2, Three, > Three | Ordinal: 1 = 1–2, 2 = 3, 3 = ≥4 | 
| **CAEC** (Consumption of food between meals) | No, Sometimes, Frequently, Always | Nominal: 0 = No, 1 = Sometimes, 2 = Frequently, 3 = Always | 
| **SMOKE** | Yes, No | Binary: 1 = Yes, 0 = No | 
| **CH2O** (Consumption of water daily) | <1 L, 1–2 L, >2 L | Ordinal: 1 = <1L, 2 = 1–2L, 3 = >2L | 
| **SCC** (Calories consumption monitoring) | Yes, No | Binary: 1 = Yes, 0 = No |
| **FAF** (Physical activity frequency)** | *I do not have, 1–2 days, 2–4 days, 4–5 days* | **Observed as continuous/inconsistent numeric values in the dataset** | **Dropped** |
| **TUE** (Time using technological devices)** | *0–2 h, 3–5 h, >5 h* | **Observed as continuous/inconsistent numeric values in the dataset** | **Dropped** |
| **CALC** (Consumption of alcohol) | I do not drink, Sometimes, Frequently, Always | Nominal: 0 = No drink, 1 = Sometimes, 2 = Frequently, 3 = Always | 
| **MTRANS** (Transportation used) | Automobile, Motorbike, Bike, Public Transport, Walking | Nominal: 0 = Car, 1 = Motorbike, 2 = Bike, 3 = Public Transport, 4 = Walking |


