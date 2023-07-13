# CrowdnessVerifier

 In this project the jetson nano is using imagenet to asses and verify the crowdness of an area, benificial for collecting data in medical and scientific enviroments as well as an aid for indivuals whom are visually impaired. 

 ## Background

 #### Hospital Emergency Room Overpopulation

Crowding has been classified as a widespread medical issue nationally in the United States. Patients that enter hospitals with injuries have been incorrectly assigned with emergency status and are placed in the ER (Emergency Room) not only preventing patients from getting the correct medical aid, but also creating overpopulation in ER waiting rooms. [^1] Crowding, delays, and diversions have increased to epidemic proportions. In the United States healthcare system, ER visits account for 11% of outpatient encounters, 28% of acute care visits, and 50% of hospital admissions. (Robert, 2012) In addition, the Emergency Room is the only medical treatment that all Americans have legal rights to regardless of their ability to pay. Moreover, making hospitals a hotspot for overpopulation at all times. Vast majority of people affected by Emergency Room overpopulation regulate in the "lower-income" communitees. A study conducted by The Center for Healthcare Research and Transformation determined that the people affected the indivuals whom are unisured are 3 times more likely to be in more aid than those insured in an Emergency Room. [^2]

#### Relationship between data and Background relevance 

Overpopulation in hospital Emergency Rooms has been overlooked as an issue in hospitals across The United States for decades. Emergency Rooms are a crucial resource for all citizens alike, regardless of citizenship, age, race, sex or salary. Trauma hospitals such as Grady's are even more affected by the overpopulation of patients as most patients suffer from servere injuries and require immidieate aid. However, due to crowded Emergency Waiting rooms and improper data to fix the issue patients receive improper care, as well as staff at risk of stress and anxiety due to the on-going influx of patients hourly. With the increase of data and awareness, waiting room crowdiness can be properly monitored and reviewed to find promising and consistant improvements to create a better hospital expirience all around. The jetson nano crowded verification requires not manual aid and can run from collecting images on hospital waiting rooms to determine how often their waiting room is crowded, but to also relay the status of crowdiness to incoming patients so they can estimate a wait or can find a more comporable location that would be more time benifical. In times like COVID-19 overpopulation is very dangerous. The spread of a virus can be easily contracted from simply standing too close to an indivual with the virus whether they present symptoms or not. 

 ## Global Context  
 
 #### Clinical aid
 The verifier is suited to in hospitals, doctors office, urgent cares and clinics as an aid to communicate to staff the influx of patients waiting     and can be used to collect data on patient care focused improvement. In pandemics such as COVID-19, populated areas were more likely to expose people and allow     them to easily contract the virus. In many circumstances a crowd verifier would be able to communcaite the capacity of certain areas before people entering areas,  giving individuals an idea of waits and delays mobilely without the need of a doctor or regular maintance and manual updates. 
  
 #### Vision Impaired aid
 
For this project 
![add image descrition here](direct image link here)

## The Algorithm

There are two datasets used for the succses of this project. The datasets are seperated by images that conotate as crowded and the other containing images that present as not_crowded or empty--

1) Firstly, the datasets go through the process of training, testing and val. The majority of the images go through training where the jetson nano is training to recognize and distiguise crowded and not_crowded images. The ratio between each folder is 8:1:1. During training, the data is ran for a set number of epochs. Epochs are how many times the data is being trained. As the epochs increase, the accuracy will most likely increase as well, however an increase of time is imminent. During this process the train and val accuracy can shift and go up or down. 
2) Once the process of training is complete the datasets then go through the process of testing. To test the images the docker is entered using the line provided below:

`./docker/run.sh`


## Running this project 1. Add steps for running this project.



3. Make sure to include any required libraries that need to be installed for your project to run.
   -crowded dataset:
   -Empty/not_crowded dataset: 

[View a video explanation here](video link)


[^1]: https://www.ncbi.nlm.nih.gov/pmc/articles/PMC3540619/
[^2]: https://chrt.org/publication/cover-michigan-survey-2011/
