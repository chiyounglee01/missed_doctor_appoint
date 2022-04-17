# missed_doctor_appoint

# Brazilian Healthcare Appointment No Show Visual Analysis 

## Introduction

**A person makes a doctor appointment in advance, but misses it in the end.**

**What factors are common amongst patients who do not show up for doctor appointments?**
**Can text messages help patients not miss appointments?**
**Does the number of wait days influence missed appointments?**

**We try to answer these two questions by analyzing a 2016 brazilian healthcare dataset.
Data of appointments was combined from more than 45 clinics and hospitals at municipallevel in Brazil betweeen 04/29/2016 and 6/8/2016.**

**The link to the dataset is below.**

https://www.kaggle.com/joniarroba/noshowappointments

**Below are notes on the dataset.**

* **Scholarship variable means this concept** = https://en.wikipedia.org/wiki/Bolsa_Fam%C3%ADlia

## Data Wrangling

The dataset was relatively clean. There were no null values or duplicated rows in this dataset.
Most of the data wrangling was done in changing the "ScheduledDay" and "AppointmentDay" row from 
an object into datetime format so we could make Date, Month and DayofWeek columns out of them.

Using the describe() function, there were odd min values in the dataset. There was a row where
the Age was -1 and there were a few rows were the wait days were below 0. These rows were deleted.

## Conclusions

* **Overall, 20.2 percent of patients did not show up at their appointment.**
* **Patients from ages 20 - 30 are more likely to miss appointments.**
* **Patients receiving the scholarship are more likely to miss appointments.**
* **Patients receiving text messages(SMS) are more likely to miss appointments.**
* **Patients with alcoholism are more likely to miss appointments.**
* **Patients with hypertension are less likely to miss appointments.**
* **Patients who scheduled the appointment on the same day (0 wait days) are less likely to miss appointments.**
* **The dataset is limited in that the no show appointments were only gathered for three months from 04/29/2016 and 6/8/2016. Some segments have few appointments so one or two no-shows have a large effect on the no-show rate.**

