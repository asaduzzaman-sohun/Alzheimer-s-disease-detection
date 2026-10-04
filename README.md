# Alzheimer’s Disease Detection Dataset

This dataset contains patient-level records used for Alzheimer’s disease detection and prediction tasks. Each row represents a patient, and each column captures demographic, clinical, behavioral, and diagnostic information.

## 1. Patient Information

| Column | Description | Value Range / Encoding |
|---|---|---|
| `PatientID` | Unique identifier for each patient. | 4751 to 6900 |

## 2. Demographic Details

| Column | Description | Value Range / Encoding |
|---|---|---|
| `Age` | Patient age. | 60 to 90 |
| `Gender` | Patient gender. | `0 = Male`, `1 = Female` |
| `Ethnicity` | Patient ethnicity. | `0 = Caucasian`, `1 = African American`, `2 = Asian`, `3 = Other` |
| `EducationLevel` | Education level of the patient. | `0 = None`, `1 = High School`, `2 = Bachelor's`, `3 = Higher` |

## 3. Lifestyle Factors

| Column | Description | Value Range / Encoding |
|---|---|---|
| `BMI` | Body Mass Index. | 15 to 40 |
| `Smoking` | Smoking status. | `0 = No`, `1 = Yes` |
| `AlcoholConsumption` | Weekly alcohol consumption. | 0 to 20 units |
| `PhysicalActivity` | Weekly physical activity. | 0 to 10 hours |
| `DietQuality` | Diet quality score. | 0 to 10 |
| `SleepQuality` | Sleep quality score. | 4 to 10 |

## 4. Medical History

| Column | Description | Value Range / Encoding |
|---|---|---|
| `FamilyHistoryAlzheimers` | Family history of Alzheimer’s disease. | `0 = No`, `1 = Yes` |
| `CardiovascularDisease` | Presence of cardiovascular disease. | `0 = No`, `1 = Yes` |
| `Diabetes` | Presence of diabetes. | `0 = No`, `1 = Yes` |
| `Depression` | Presence of depression. | `0 = No`, `1 = Yes` |
| `HeadInjury` | History of head injury. | `0 = No`, `1 = Yes` |
| `Hypertension` | Presence of hypertension. | `0 = No`, `1 = Yes` |

## 5. Clinical Measurements

| Column | Description | Value Range / Encoding |
|---|---|---|
| `SystolicBP` | Systolic blood pressure. | 90 to 180 mmHg |
| `DiastolicBP` | Diastolic blood pressure. | 60 to 120 mmHg |
| `CholesterolTotal` | Total cholesterol. | 150 to 300 mg/dL |
| `CholesterolLDL` | Low-density lipoprotein cholesterol. | 50 to 200 mg/dL |
| `CholesterolHDL` | High-density lipoprotein cholesterol. | 20 to 100 mg/dL |
| `CholesterolTriglycerides` | Triglyceride level. | 50 to 400 mg/dL |

## 6. Cognitive and Functional Assessments

| Column | Description | Value Range / Encoding |
|---|---|---|
| `MMSE` | Mini-Mental State Examination score. Lower scores indicate greater cognitive impairment. | 0 to 30 |
| `FunctionalAssessment` | Functional assessment score. Lower values indicate greater impairment. | 0 to 10 |
| `MemoryComplaints` | Presence of memory complaints. | `0 = No`, `1 = Yes` |
| `BehavioralProblems` | Presence of behavioral issues. | `0 = No`, `1 = Yes` |
| `ADL` | Activities of Daily Living score. Lower scores indicate greater impairment. | 0 to 10 |

## 7. Symptoms

| Column | Description | Value Range / Encoding |
|---|---|---|
| `Confusion` | Confusion symptom. | `0 = No`, `1 = Yes` |
| `Disorientation` | Disorientation symptom. | `0 = No`, `1 = Yes` |
| `PersonalityChanges` | Personality changes. | `0 = No`, `1 = Yes` |
| `DifficultyCompletingTasks` | Difficulty completing tasks. | `0 = No`, `1 = Yes` |
| `Forgetfulness` | Forgetfulness symptom. | `0 = No`, `1 = Yes` |

## 8. Diagnosis Information

| Column | Description | Value Range / Encoding |
|---|---|---|
| `Diagnosis` | Final diagnosis status for Alzheimer’s disease. | `0 = No`, `1 = Yes` |

## 9. Confidential Information

| Column | Description |
|---|---|
| `DoctorInCharge` | Contains confidential doctor information. In this dataset, the value is the same for all patients: `XXXConfid`. |

## Notes

- `0` usually means “No / Negative / Absent” and `1` means “Yes / Positive / Present” unless otherwise specified.
- This dataset is suitable for binary classification tasks, where the target variable is `Diagnosis`.
- The `DoctorInCharge` field should be treated as sensitive and removed or anonymized before model training or public sharing.
