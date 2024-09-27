# Hospital Emergency Room Visits

### Dashboard Link : https://public.tableau.com/app/profile/favour.oyibo/viz/HospitalEmergencyroomvisitDashboard/ERDashboard

## Problem Statement

The hospital emergency room visits dashboard provides a concise overview of various metrics related to visits to the emergency department of a hospital. It typically includes information such as the number of visits over a specific period, demographics of patients (age, gender), reasons for visits (chief complaints), average wait times, disposition of patients (admitted, discharged, transferred), and any relevant trends or patterns observed.

This dashboard serves as a valuable tool for hospital administrators, healthcare providers, and policymakers to monitor the utilization of emergency services, identify areas for improvement in patient care and resource allocation, track patient flow, and make informed decisions to enhance the efficiency and effectiveness of emergency care delivery.

### Steps followed 

- Step 1 : Write SQL query to get data needed for analysis from the database.
- Step 2 : Data Cleaning and validation was carried to ensure data quality and intergrity is kept.
- Step 3 :  Save the cleaned and filtered data to a csv file.
- Step 4 :  Load the dataset into Tableau for visualizations..
- Step 5 : Create a calculated field to share the various age into categorical group.
- Step 6 : Each graph was used as a filter for easy visualization and interaction. 
- Step 7 : Various  Visual like Heat map, line charts, bar charts ,and Area chart was used to show the various insights below;

  (a) Number of patients visiting the Emergency room by their Age category.

  (b) Patient wait time on average.
  
  (c) Number of patients visiting the Emergency room group by their Race.
  
  (d) Number of Patient referred to various department after visiting the Emergency room

  (e) Average Patient wait time across the days of the week
  

- Step 9 : In the report view, three text boxes were added to the canvas, to show the number of patients who visited the Emergency room, the average patient wait time , and rating of patient satisfaction on average.

- Step 10 : In the dashboard view, under the object tab, using using image option elements were added to the report design area. 

- Step 11 : A heatmap chart was created to visualize the average patient wait time at the Emergency room department across the various days in the week.
        
- Step 12 : New measure was created to 

i. categorize age into groups.
    

Following Tableau expression was written for the same,
        
        IF [Patient Age]>= 0 and [Patient Age] <= 18 
        then  '0-18yrs'
        ELSEIF [Patient Age]>= 19 and [Patient Age] <= 65 
        then  '19-65yrs'
        ELSE '66yrs+' 
        END


 - step 13:        
A card visual was used to represent the number of Emergency Room patients

![page_1](https://github.com/FaeyO/Hospital-Emergency-Room-Visits-/assets/118575325/78df292f-4c35-4fa6-b3a1-5178ae247c48)


A card visual was used to represent the average Patient wait time and average patient satisfaction

![page_1](https://github.com/FaeyO/Hospital-Emergency-Room-Visits-/assets/118575325/cf3785dc-b4e3-4134-92a7-45cb8e160736)

![page_1](https://github.com/FaeyO/Hospital-Emergency-Room-Visits-/assets/118575325/a153ef0e-e66a-42e6-ab2d-a0c8c4a8375b)


 - Step 14 : The report was uploaded to the Tableau public server.
 
# Insights

A single page report was created on Tabeau, and the following inferences can be drawn from the dashboard;

### [1] The average waiting time at the Emergency room was 35.26minutes

### [2] The average Patient satisfaction rating was 4.99 out of 10

### [3] White and African American were the two race who consisted majority of the patient visiting the Emergency Room.

### [4] Patients were mostly referred to the General practice department or Orthopedics from the Emergency room.
  
### [5] The highest average waiting time of patients in the emergency room was on monday at 11pm, while the lowest was at wednesday at about 1am.


### Dashboard view

![Dashboard 1](https://github.com/FaeyO/Hospital-Emergency-Room-Visits-/assets/118575325/d87eaad9-e3ab-41fc-9550-966abfec4eee)
