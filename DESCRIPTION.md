# ITRY
## Introduction
With an increasingly ageing population and a growing segment of vulnerable populations specifically the increasing trend of elderly with no next of kin, Community First Responders (CFRs) must be alerted at the onset of incidents which require emergency response (e.g. cardiac arrests, falls, unattended cooking fires etc.) and mobilised for effective early intervention.

For the general population, alerting CFRs about the situation is seen as a rather simple step to accomplish,the same cannot be said for the elderly. This problem is further compounded by fact that we see more elderly living alone with no next of kin to look out for them. Often, cases involving elderly go unreported until it is too late. The lingering smell of decomposed bodies and an individuals prolonged absence or a full-on-fire are the only tell-tale signs of an emergency that has occured sometime back.

Advancements in statistics and technology has blessed us with data analytics, sensors and data storage solutions like the cloud. This has allowed us to collect , store and analyse information about the environment around us automatically. All these can be pivoted towards emergency response as ameans of detecting emergencies which could have been unseen when no one is available to report or witness them. The availability of such information allows CFRs to kick into gear for effective early intervention before it escalates to anything more.

## Idea of project

Our team has decided to make use of Internet of Things (IOT) devices to collect data, transmit data to the cloud and make use of IBM Watson Studio to analyse and visualise the data to SCDF in order to improve their sense-making to be alerted at the onset of incidents which require emergency response and mobilise the CFRs for effective early intervention for the elderly population.

### Retrieving data from IOT Device

We were able to make use of node red and an andriod device in this case to establish a link to generate a sensor that is capable of measuring acceleration. This acceleration sensor can help us keep track of the movement of elderly in real time. In cases where there are sharp increase in acceleration. This could prompt a warning of possible fall cases of the elderly. In the IOT platform, the data collected can also be visualised in a graph form where we can keep track in real time.

### Analysing data collected using R studio 

This data will be matched with prior data that are obtained and comparison will be made between the datas to see if there are any abnormalities in activvity of the elderly. This comparison will be done using an algorithm in R studio and data visualization tactics will be used to determine if there is any indication of abnormal activities. In the event that the system triggers the push notifications of abnormal activites, the Community First Responders will then be activated on site to check out the situation. 

## Conclusion
In conclusion,  we strongly believe that our proposed solution will greatly improve SCDF's sense-making to be alerted at the onset of incidents which require emergency responses and mobilise CFRs for effective early intervention especially to the elderly living without any next of kin.

## Disclaimer
Disclaimer : Due to time constraints, we were only able to demonstrate the following :
1.	The streaming of movement data from sensor to the IoT platform
2.	The analysis of temperature data on R in Juptyer Notebook
More is left to be desired. Such as :
1.	The integration of the various services and databases. 
2.	Analysis with more user data.
3.	Selection of model for analysis.

## Acknowledgements
We would like to take this opportunity to thank and acknowledge IBM and SCDF for organising the Call for Code 2020 and providing us with the opportunity and learning experience to participate in this Hackathon.
