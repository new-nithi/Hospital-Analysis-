# Hospital-Analysis-

SQL-only project to analyze a hospital database (SQLite). This repo focuses on **Analysis** 



## Data / Schema


### `appointments`
| column | type | pk | not null | default |
|---|---|---|---|---|
| `appointment_id` | TEXT | ✅ |  |  |
| `patient_id` | TEXT | ✅ |  |  |
| `doctor_id` | TEXT | ✅ |  |  |
| `appointment_date` | TEXT |  |  |  |
| `appointment_time` | TEXT |  |  |  |
| `reason_for_visit` | TEXT |  |  |  |
| `status` | TEXT |  |  |  |

### `billing`
| column | type | pk | not null | default |
|---|---|---|---|---|
| `bill_id` | TEXT | ✅ |  |  |
| `patient_id` | TEXT | ✅ |  |  |
| `treatment_id` | TEXT | ✅ |  |  |
| `bill_date` | TEXT |  |  |  |
| `amount` | REAL |  |  |  |
| `payment_method` | TEXT |  |  |  |
| `payment_status` | TEXT |  |  |  |

### `doctors`
| column | type | pk | not null | default |
|---|---|---|---|---|
| `doctor_id` | TEXT | ✅ |  |  |
| `first_name` | TEXT |  |  |  |
| `last_name` | TEXT |  |  |  |
| `specialization` | TEXT |  |  |  |
| `phone_number` | INTEGER |  |  |  |
| `years_experience` | INTEGER |  |  |  |
| `hospital_branch` | TEXT |  |  |  |
| `email` | TEXT |  |  |  |

### `patients`
| column | type | pk | not null | default |
|---|---|---|---|---|
| `patient_id` | TEXT | ✅ |  |  |
| `first_name` | TEXT |  |  |  |
| `last_name` | TEXT |  |  |  |
| `gender` | TEXT |  |  |  |
| `date_of_birth` | TEXT |  |  |  |
| `contact_number` | INTEGER |  |  |  |
| `address` | TEXT |  |  |  |
| `registration_date` | TEXT |  |  |  |
| `insurance_provider` | TEXT |  |  |  |
| `insurance_number` | TEXT |  |  |  |
| `email` | TEXT |  |  |  |

### `treatments`
| column | type | pk |  not null | default |
|---|---|---|---|---|
| `treatment_id` | TEXT | ✅ | |  |
| `appointment_id` | TEXT | ✅ |  |  |
| `treatment_type` | TEXT |  | |  |
| `description` | TEXT |  | |  |
| `cost` | REAL |  |  |  | |  |
| `treatment_date` | TEXT |  |  |  |






## Insights 
- A small set of specialties accounts for most visits and costs.
- Revisit within 30 days suggests opportunities for follow‑up programs.

> Replace these with your actual findings once you load sample data.

## (SQL skills)
- SELECT , WHERE , JOIN ,  GROUP BY , ORDER BY
- KPI


