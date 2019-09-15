# Dermaviz
<p align="center">
  <img src="https://github.com/SVAI/Dermaviz/raw/master/assets/logo.png" width="256" title="Dermaviz Logo"/>
</p>

# Dermaviz: Comprehensive Research Suite for integrated Phenotyping, Genotyping and 3D Modeling for NF patients

Dermaviz is a full research suite designed to advance and integrate the collection of data from NF patients.


## Abstract: 

 Neurofibromatosis type 1 (NF1) displays considerable variability in phenotypic expression and recent work identified phenotypic subtypes of disease. Large scale phenotypic-genotypic correlations will lead to better understanding of disease subtypes and more personalized screening and treatment of NF1. We have created an easy-to-use iOS mobile application that creates and exports a 3D model to HIPPA compliant cloud storage, integrates phenotypic and genomic data, and enables fast and comprehensive data collection for a large number of NF patients (>7,000). This solution will enable rapid collection of integrated patient data, leading to understanding of disease, identification of genetic modifiers, improved risk stratification, and measurement of response to therapeutics.

## Introduction: 

Neurofibromatosis (NF) type 1 is a highly heterogeneous disease. Currently, we do not have ways to predict which patients will develop certain characteristics or respond to therapies. In order to improve management of NF1, including both risk stratification and targeted therapeutics, a better understanding of disease heterogeneity is needed. A recent study by Tabata et. al. (under review) identified phenotypic subtypes. However, genotypic and phenotypic data is needed from a large sample size (>2000) in order to perform genome-wide association studies to identify novel modifiers of disease to further understand heterogeneity. Our work creates a novel method of data collection that will enable rapid data collection of phenotypic, genotypic, and 3D patient data in order to rapidly advance research for NF1. This solution will enable personalized risk stratification, development of therapeutics, and response to therapeutics. Integration of our solution with existing data will synergistically result in a powerful database for discovery. Furthermore, our solution is scalable, HIPPA compliant, and translatable to other rare diseases.

![Figure 4](https://raw.githubusercontent.com/SVAI/Dermaviz/master/assets/Figure4.jpg)
  

## Methods *: How did we go about solving it?*

  

## Results *: What did we observe? Figures are great!*

We created an iOS app that takes a high-resolution 3D scan of a patient’s face and exports it to a HIPAA-compliant Google Cloud server. We also developed a pipeline for connecting all collected 3D models to Google BigQuery as well to Machine-Learning ready stacks.

3D scan of team members’ faces successfully captured the makeshift “neurofibromas” that were placed on the skin. Furthermore, the 3D face image was successfully exported to the Google Cloud server and linked to clinical, genomic, and survey data.

Our suite integrates with a patient questionnaire and genomic data collection. Each patient is assigned a unique invite code that allows them to “log-in” to the app and take scans. All scans are securely uploaded to our HIPPA-compliant Google Cloud server over HTTPS. Each scan is sorted by date taken to provide clinicians with a comprehensive view on the development of NF over time. These scans are available in the standard `.obj` format. The dermatologist will also have access to patient data that includes submitted answers in the questionnaire as well the genomic data collected.

#### Patient Invite Code:

Once the form data and genomic data is available, the Dermaviz server generates an invite code and sends it to the patient. On the app, the patient enters the invite code. This code is cached client side and is used to send all data to the server.
<img src="https://raw.githubusercontent.com/SVAI/Dermaviz/master/assets/invite-code.png" height="512" title="Dermaviz Invite Code"/>

#### Patient Scanning
After entering the invite code, patients are instructed to scan their face. After a successful scan, these scans are uploaded to our server. 

##### Demo 1:
<img src="https://github.com/SVAI/Dermaviz/raw/master/assets/demo-1.gif" height="512" />

##### Demo 2:
<img src="https://github.com/SVAI/Dermaviz/raw/master/assets/demo-2.gif" height="512" />

## Conclusion/Discussion:

A phone application that captures high-resolution 3D images of NF1 patient skin allows for rapid collection of phenotypic NF1 data. We created here an iOS app that takes a high resolution 3D scan of the patient’s face, links it to patient clinical, genomic, and survey data, and exports it to a HIPAA-compliant Google Cloud folder for visualization by dermatologists and NF1 researchers. Rapid collection of phenotypic data and linking with clinical, genomic, and survey data enables robust characterizations of disease heterogeneity and will dramatically accelerate research in NF1 in the following areas:

-   Obtaining prognostic information on who might need treatment
    
-   Capturing the natural history of NF1
    
-   Measuring cutaneous tumor burden over time
    
-   Tracking response to future therapies
    
-   Identifying pathways that modulate number of neurofibromas, which will present new genetic and molecular targets for drug therapy
    
-   Extrapolate to any rare cutaneous disease (Gorlin’s, dysplastic nevus syndrome, phakomatosis pigmentokeratotica, tuberous sclerosis, RAS-opathies, etc.)

### Please make sure you address ALL of the following:

  

#### *1. What additional data would you like to have*

  

#### *2. What are the next rational steps?*

  

#### *3. What additional tools or pipelines will be needed for those steps?*

  

#### *4. What skills would additional collaborators ideally have?*

  

## Reproduction: *How to reproduce the findings!*

  

## Acknowledgments

Special thanks to [Bellus3D](https://bellus3d.com/) for licensing their 3D technology for us to research and build upon.

Logo credits to [RoundIcons](https://www.flaticon.com/authors/roundicons).
