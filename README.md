# Virufy COVID-19 Open Cough Dataset

Virufy is a volunteer-run organization uniting the world to build a global artificial intelligence (AI) database of crowdsourced cough sounds to identify patterns that signify respiratory diseases, such as COVID-19.

Our research paper can be found on [arXiv](https://virufy.org/paper). Please cite us if you reference our materials!

## Why Open Data?
The COVID-19 pandemic is extremely detrimental to society and we need to all work together to overcome it. AI needs big data to work and we are unaware of any open source COVID-19 cough datasets anywhere in the world. We want to benefit humanity and have decided to be pioneers in open sourcing the first free COVID-19 cough dataset. This will spur innovation and collaboration from academia and industry all over the world.

## Data

All data is labeled with COVID-19 PCR test status, along with patient demographics as can be found in
[labels.csv](clinical/labels.csv).

### Clinical Data
Our clinical data is very accurate because it was collected at a hospital under supervision by physicians following Standard Operating Procedures (SOP) and informed patient consent. Our data is preprocessed and labeled with COVID-19 status (acquired from PCR testing), along with patient demographics (age, gender, medical history). Here, we have provided 121 segmented cough samples from 16 patients.

The data directory contains two different folders, one with the original cough audio recordings, and the other with the segmented versions of the coughs. The segmented coughs were created by identifying periods of relative silence in the recordings and separating coughs based on those silences. The segments which were not coughs or had too much background noise are removed.

### Crowdsourced Data
Our crowdsourced data is diverse, coming from multiple countries, and is expected to increase in volume significantly over time as more people donate their coughs. Here, we are open sourcing a subset of the data, so the community can begin to develop models and write research papers.

## Collaboration
We hope to create a community of researchers driven to use this data to create solutions for the pandemic.

If you'd like to join our community, please fill out [our form](https://forms.gle/XLxALoabybztCDUN6).

You may also contact us at open-data@virufy.org.

## Segmentations
This repo contains other two segmented files from two individual cough segmentatin methods (hysteresis comparator and RMS threshold). See clinical folder for detail.  

## Citation
For citing virufy-data and manual segmentation (`clinical/segmented`):  
```
G. Chaudhari et al., “Virufy: Global Applicability of Crowdsourced and Clinical Datasets 
for AI Detection of COVID-19 from Cough Audio Samples,” 2020, [Online]. 
Available: http://arxiv.org/abs/2011.13320.
```
For automatic segmentations (`segment` and `simple` directories under `clinical`):
```
B.T. Atmaja, Zanjabila, Suyanto, Dhany Arifianto, Akira Sasou.
Evaluation of Single Cough Segmentations, 2022.
```

