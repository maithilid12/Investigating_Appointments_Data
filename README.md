# Investigating Patients Appointment Data

# Table of Contents
1. Introduction
2. Prerequisites
3. File Description
4. Dataset Overview
5. Results
6. Acknowledgements

# Introduction
In this project, a dataset consisting information from 100k medical appointments in public hospitals at Vitoria, Brazil is investigated. The reason why the patient did not show up to their appointment attracts my attention. This dataset contains records whether patients miss appointments, attributes of paients and information about apointments.After inital assessment of data, I have formulated set of questions to help identify factors that are vital to be known in order to predict if a patient will show up for their scheduled appointment:
1. Does sending a SMS reminder increase the attendance of the patient? Is it affected by Gender?
2. Is there a correlation between type of disease and attendance of patient for the appointment?
3. Which age group has secured most scholarships and does it affect the attendance at appointment?

![Appointments-Image](appointments_image.jpg)

# Prerequisites
1. Pandas (for data loading and analysis)
2. NumPy (for computing)
3. Matplotlib (for visualizations)
4. Seaborn (for visualizations)
5. Jupyter (to run notebooks)

# File Description
There are three folders:
1. Code
   - Appointments Data Analysis.ipynb- covers the entire analysis process performed to investigate the dataset as well as the documentation
2. Data
   - appointments_data.csv: Patients Appointment Dataset
3. Presentation
   - appointments_data_presentation.slides.html: Slideshow providing insights on questions constructed
   - presentation.gif: Preview of presentation
   ![Presentation-gif](Presentation/presentation.gif)
4. Images 
   - appointments_image.jpg

# Dataset Overview
- There are 14 attributes and 110527 observations of patient data
- The most important attribute is the `no_show` which mentions whether the patient attended the appointment or not
- **Feature Description**
   1. PatientId: Identification of a patient
   2. AppointmentID: Identification of each appointment
   3. Gender: Male or Female
   4. Scheduled Day: The day of the actual appointment.
   5. Appointment Day: The day someone called or registered the appointment
   6. Age: How old is the patient
   7. Neighbourhood: The location of the appointment takes place
   8. Scholarship: whether or not the patient is enrolled in Brasilian welfare program [Bolsa Família](https://en.wikipedia.org/wiki/Bolsa_Fam%C3%ADlia)
   9. Hyertension: Type of disease
   10. Diabetes: Type of disease
   11. Alcoholism: Type of disease
   12. Handicap: Disability
   13. SMS received: or more messages sent to the patient.
   14. no-show: Whether the person will show up at the appointment or not

# Results
1. Does sending a SMS reminder increase the attendance of the patient? Is it affected by Gender?
     - Receiving SMS reminders does not increase patient attendance and thus a suggestion can be made to discontinue this service to save cost of operation
2. Is there a correlation between type of disease and attendance of patient for the appointment?
     - The type of disease does not increase patient attendance and more number of patients experience Hypertension
3. Which age group has secured most scholarships and does it affect the attendance at appointment?
     - Having a scholarship increases the chances of a patient attending the appointment which is people with the age 35 and above

# Acknowledgements
The dataset can be found [here.](https://www.kaggle.com/joniarroba/noshowappointments)
