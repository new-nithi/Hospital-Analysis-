# Hospital-Analysis-
SQL queries for analyzing hospital database

## Tables in this database
- `appointments` — appointment_id, patient_id, doctor_id, appointment_date, appointment_time, reason_for_visit, status
- `patients` — patient_id, first_name, last_name, gender, date_of_birth, insurance_provider
- `doctors` — doctor_id, first_name, last_name
- `treatments` — treatment_id, appointment_id, treatment_type, description, cost, treatment_date
- `billing` 

</div>

## ประเด็นที่วิเคราะห์ด้วย SQL
- 1.`show a doctor who have an exps more than 5 years_experienc `
- 2.`Show patient name and doctor name make an appointment_date `
- 3.`Summarize how many tines,each of appointment in each type `
- 4.`Total cost any treatment type`
- 5.`Total revenue from each doctor`
- 6.`patient who have most appointment`
- 7.`For patient who did appointment but not showing up`
- 8.`KPI : income per doctor and time of appointments`
  
</div>

flowchart LR
  A[Inspect schema<br/>ดูตาราง/คอลัมน์ใน SS.db] --> B[Standardize Views<br/>sql/views/01_base_views.sql]
  B --> C[Performance Basics<br/>sql/indexes/01_recommended.sql]
  C --> D[Analytics Reports (CTE/Window)<br/>sql/reports/*.sql]
  D --> E[Export CSV via CLI<br/>sql/scripts/run_all.sql → docs/outputs/*.csv]
  E --> F[Summarize Findings in README/ONE-PAGER]

