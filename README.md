# CrowdnessVerifier

 In this project the jetson nano is using imagenet to asses and verify the crowdness of an area, benificial forcollecting data in medical and scientific enviroments as well as an aid for indivuals whom are visually impaired. 

 ## Background

Crowding has been classified as a widespread medical issue nationally in the United States. Patients that enter hospitals with injuries have been incorrectly assigned with emergency status and are placed in the ER (Emergency Room) not only preventing patients from getting the correct medical aid, but also creating overpopulation in ER waiting rooms. [^1] Crowding, delays, and diversions have increased to epidemic proportions. In the United States healthcare system, ER visits account for 11% of outpatient encounters, 28% of acute care visits, and 50% of hospital admissions. (Robert, 2012) In addition, the Emergency Room is the only medical treatment that all Americans have legal rights to regardless of their ability to pay. Moreover, making hospitals a hotspot for overpopulation at all times. 

 ## Global Context  
 
 #### Clinical aid
 The verifier is suited to in hospitals, doctors office, urgent cares and clinics as an aid to communicate to staff the influx of patients waiting     and can be used to collect data on patient care focused improvement. In pandemics such as COVID-19, populated areas were more likely to expose people and allow     them to easily contract the virus. In many circumstances a crowd verifier would be able to communcaite the capacity of certain areas before people entering areas,  giving individuals an idea of waits and delays mobilely without the need of a doctor or regular maintance and manual updates. 
  
 #### Vision Impaired
 
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
