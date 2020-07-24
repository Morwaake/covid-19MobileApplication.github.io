## Covid-19 Contact Tracing Application

You can use the [editor on GitHub](https://github.com/Morwaake/covid-19MobileApplication.github.io/edit/master/index.md) to maintain and preview the content for your website in Markdown files.

## INTRODCTION
After calls for a way of using technology to facilitate the lifting of restrictions on freedom of movement for people not self-isolating, whilst ensuring regulatory obligations such as the Human Rights Act and equivalent GDPR provisions, this paper proposes a reference architecture for a contact tracing mobile application database that maintains privacy, yet is built to scale to support large-scale lifting of restrictions of movement.
This proposes an Application that could be installed on mobile phones in order to identify people who were in close proximity to an infected person. This application should also alert people who have come into contact with someone who were pre-symptomatic in order to allow them to self-isolate.

### PROBLEM STATEMENT
The coronavirus COVID-19 pandemic is the defining global health crisis of our time and the greatest challenge we have faced since World War Two. Since its emergence in Asia late last year, the virus has spread to every continent. Cases are rising daily in Africa the Americas, and Europe.
Countries are racing to slow the spread of the virus by testing and treating patients, carrying out contact tracing, limiting travel, quarantining citizens, and cancelling large gatherings such as sporting events, concerts, and schools.
There is no doubt that extraordinary times call for extraordinary measures, and getting rid of the virus, saving lives and resuming normalcy is of paramount interest. All over the world governments have availed themselves of emergency measures to collect data from CCTV cameras, cell phones and credit-card transactions in order to track infected patients, their movements and encounters.

### OBJECTIVES
### GENERAL OBJECTIVE
	To provide details of people in contact with infected person
### SPECIFIC OBJECTIVES
	To exchange necessary details between people in close proximity
	To classify the contacts to the infected people
	To alert people who are contacts in case of  an infected person so they self-isolate
### LITERATURE RVIEW
### BACKGROUND
The project is aimed to develop a Covid-19 mobile application that will aid the Covid-19 response team with information need for contact tracing in the country and provide a way that the contacts of the infected person be alerted well in time to self-isolate from the rest of the community. The application is a mobile application that can be accessed by the community and the response task force. This system will provide better prospective for the enhancement of contact tracing in terms of Covid-19 in Botswana.
We should bear in mind that one of the main goal of the entire world at large is so that even with the current Covid-19 pandemic, the world should go back to normal or close to normal. We show that, when adopted sufficiently broadly, such a contact-tracing strategy can bring COVID-19 under complete control, end the need of social distancing, and return the society to full normalcy.
### SOME RELATED WORK
According to (Ye Xia,Gwendolyn Lee)We outline a contact-tracing strategy based on proximity sensing using mobile devices. We discuss what an ideal system should look like and what it can do. We show that, when adopted sufficiently broadly, such a contact-tracing strategy can bring COVID-19 under complete control, end the need of social distancing, and return the society to full normalcy. The most important piece of this contact-tracing strategy is the mobile device, the contact recorder, that everyone carries in the public. Think about a smart watch or a mobile phone. Each such device has a unique ID. On a central server, the device ID is tied to the individual’s identity and how the individual can be reached, such as a cell phone number or an email address. When two individuals are within a distance where virus transmission is possible, say 2 meters, the devices are able to detect each other and they each record the other device ID, the distance, and the duration of contact at the distance. The data is communicated to the central server, preferably in real time.
Suppose an individual, say person A, is sick, tested and confirmed to be infected. The central server checks the contact information recorded on A’s device and conducts risk evaluations of A’s recent contacts, say going back 14 days, and informs all those who are at risk of being infected by A through contact. Depending on the risk level, some of the at-risk individuals may be tested and/or quarantined; others may only receive a notification of caution. The risk evaluation may be based on the distance of contact, the duration of contact, and how infectious person A is estimated to be at the time of contact.
Also according to (Christoph, Michael , Daniel Günther, 2020)’ At my institute (160 people), we traced a number of contacts and noticed that the complexity of a manual process becomes quickly unmanageable. Due to the exponential character of the network of relations, there are simply too many contacts to betraced. We ended up isolating everyone first at the Institute level, shortly after that and independently of us at DLR level and finally at national level. This observed complexity led us to the conclusion that automatic means of tracing are essential. Raskar et al. [3] have analyzed an approach based on locating people with a focus on privacy-protection and self-protection against the disease. We follow a somewhat different approach. It is primarily based on contacts, rather than on locations, although locations may be used in addition.
The precondition for traceability is to use of a smartphone running a COVID-19 tracing app (the app) or alternatively the use of a low-cost device. For simplicity, the focus of the exposition will be on an app running on a smartphone. Every person leaving their home shall be requested to carry such a device, with the app installed and active. This might be an expectation; which people are free to follow or not. Whatever solution is preferred is a political decision. The main elements of its implementation are 
• The automated creation of a list of contact instances my_ctc, maintained in the personal device of the user. The number of such entries could be up to a few thousand entries per day as soon as big events take place again.
 • The maintenance of a list of infectious carriers of the disease ga_icd on the server of the Gesundheitsamt, currently around 70’000 entries in total with a growth rate of less than 4000 per day.
 • The search for entries from the personal list my_ctc in the list ga_icd retrieved from the Gesundheitsamt.
 • In the case of a hit, the app informs the server of the Gesundheitsamt about the identifier found.
 • The server and the app cooperate in classifying the category of the contact (Category 1 or 2, see below). The associated contact persons might be involved in this classification process. 
• Based on the result, the Gesundheitsamt decides about the quarantining and testing of the device’s owner

 
## CHALLENGE DEFINITION
### CATEGORY:
eHealth
### TITLE:
Mabapi application
### BACKGROUND:
The coronavirus COVID-19 pandemic is the defining global health crisis of our time and the greatest challenge we have faced since World War Two. Since its emergence in Asia late last year, the virus has spread to every continent. Cases are rising daily in Africa the Americas, and Europe.

In dealing with all this virus spread one of the major’s ways to combat this virus spread is through the contact tracing. This contact tracing is a method adopted worldwide. Currently in Botswana the method at which this is done is through manually citizens providing their details on paper at places of entry, working hand in hand with the newly released contact tracing application “Be Safe”.

The manual system includes having to write your details in plain text, hence there is little privacy for the citizen’s details. This manual system also is not standard as in what details it requires from citizen. Some may only have time in and not have time out, this comes faulty as time interval at which a person has been in a place is important. This manual system is even costly and takes time to run through when trying to get contacts.

The current Be Safe mobile application uses a qr scanner to register citizens as they enter a building or place, hence the citizen details are privately capturing. The set back about this mobile application is the fact that it is only used to capture entrance of citizens into a place, it does not capture the time they exit.

One of the commonalities in both the manual paper system and be safe mobile application is that they are more location-based contact tracing. The trace potential carriers based on places they have been to creating loopholes to other people who one might have been in contact with just passing. The second commonality includes the fact that they are far from normalcy where people where not required to provide details. For both, people must make a stop in their everyday lives to complete the providing of details.
### DESCRIPTION
To address some loopholes stated about the two current systems (manual system and Be Safe), I have come up with another mobile application named Mapadi. This Mabapi mobile application primarily is to be able to provide the covid 19 task team with details of possible carriers after a confirmed case. This mobile application will require the citizens to have smartphone to exchange information when ever there are in close range. The application works without users having to stop their routines to exchange details but instead it will be an automated process. This process will not only happen at some places hence not location based.
### LIST OF SKILLS REQUIRED/ACQUIRED
1.	PROGRAMMING FLATTER
2.	KNWOLEDGE ON DATABSE3.	
### LIST OF HARDWARE/SOFTWARE NEEDS
1.	Android Studio
2.	High performance computer (i5 +)
3.	8GB RAM
### USERS
•	Citizens
•	Covid-19 Task Force team


 
### IMPLEMENTATION DIRECTIONS

For mobile applications to be able to detect beacons in other mobile devices there are two main technologies associated with this. These are;
	Low – Level Bluetooth library
	Third party Library.
I have decided to use the Third party library being the Android Beacon Library.
It is advantageous as it is fairly easy to use, unlike low level Bluetooth library which is considered hard and it will require more work to be done.
The Android Beacon Library 
Distance estimates
The API provides estimates of the distance to a beacon in meters. The values are rough estimates based on the signal strength of the Bluetooth signal received at the mobile device. Applications should not expect a high precision in the numbers. They are most useful for determining which beacon is closest when multiple are visible.

How accurate are the estimates?
At close proximity of about 1 meter, you can expect to see distance estimates between 0.5-2 meters. At further distances you will see more variation. At 20 meters or actual distance, the estimate provided by the library may vary from 10-40 meters. The variation is caused by noise on the signal measurement, along with signal reflections and obstructions. CAUTION: Before building an app using distance estimates, be sure you read up on the limitations of this technology.

Variations in time
In order to reduce noise on the estimate, the library averages signal measurements over 20 seconds, throws out the top 10% and bottom 10% of measurements, and averages the rest. It is important to understand that the distance estimates are based on the previous 20 seconds in time, so when a mobile device moves, the distance estimate will lag until the device has been stationary for 20 seconds, at which time the distance estimate will stabilize. The variation in time is adjustable.

Device variations
A big challenge in providing accurate distance estimates with Android devices is that every device model receives signals differently. Each model may have a different Bluetooth chipset and antenna, and therefore may receive a different signal level when in the same position relative to a beacon. In order to address this, the library uses a different formula for calculating distance for different Android device models. Because not all devices have custom formulas built into the library, the library will fall back to the default device calculation for the Nexus 5 if no matching formula is found.

Formula
Despite formulas suggested by signal theory, the most accurate predictor of distance based on signal strength (RSSI) can be obtained by doing a power regression against a known table of distance/RSSI values for a specific device. This uses the formula d=A*(r/t)^B+C, where d is the distance in meters, r is the RSSI measured by the device and t is the reference RSSI at 1 meter. A, B, and C are constants.

Data for specific models
The list of models with specific calculations is available in the config file here. If you don’t see your model listed, see the section below on how you can get it added

Getting new Android device models added to the list
If you would like to get a new Android device model added to the list, you can help by taking measurements. In order to do this, you will need a beacon, an Android device, an iPhone 5, a copy of the Radius Networks’ Android Locate app, and an accurate way of measuring distance between your mobile device and the beacon. You’ll also need an outdoor space where you can do distance measurements that is free of obstructions in all directions for about 50 meters.

Once you have these tools, you can use the Calibration feature of the Android Locate app to get a 30 second running average of the RSSI for your device at specific distances. In order to do a new regression for your device, RSSI measurements must be collected at 20 different distances measured in meters: 0.25, 0.5, 1, 2, 3, 4, 5, 6, 7, 8, 9, 10, 12, 14, 16, 18, 20, 25, 30.

You also need to collect the information about your Android device under test, which can be found under Settings -> About Phone. The fields needed are: Model number, Android version, Build number, Manufacturer.

STEPS ON HOW TO WORK WITH BEACONS
1.	Add  android beacon library
2.	Need permission or request  permission to use Bluetooth and location in application
3.	Create  beacon manager and beacon consumer
4.	To manage the beacon activities in our application
5.	Create Beacon Region
With: UID major and minor identities we wish to listen for
6.	Start Monitoring For Beacon
This will raise big an event that our beacon consumer will act upon
This application will work along “concept of sharing ” ,sending the data to the covid-19 task force.

Bibliography
Christoph, Michael , Daniel Günther. (2020). Tracing Contacts to Control the COVID-19 Pandemic. arXiv, 1.
World Health Organization (WHO). (2020, April 27). Archived: WHO Timeline - COVID-19. Retrieved June 30, 2020, from World Health Organization (WHO): https://www.who.int/news-room/detail/27-04-2020-who-timeline---covid-19
Ye Xia,Gwendolyn Lee. (2020). Fast and Comprehensive Contact Tracing of COVID-19. How to Return to Normalcy, 1.


https://www.undp.org/content/undp/en/home/coronavirus.html
https://altbeacon.github.io/android-beacon-library/distance-calculations.html


### Markdown

Markdown is a lightweight and easy-to-use syntax for styling your writing. It includes conventions for

```markdown
Syntax highlighted code block

# Header 1
## Header 2
### Header 3

- Bulleted
- List

1. Numbered
2. List

**Bold** and _Italic_ and `Code` text

[Link](url) and ![Image](src)
```

For more details see [GitHub Flavored Markdown](https://guides.github.com/features/mastering-markdown/).

### DONE BY MORWAAKE 2020

Your Pages site will use the layout and styles from the Jekyll theme you have selected in your [repository settings](https://github.com/Morwaake/covid-19MobileApplication.github.io/settings). The name of this theme is saved in the Jekyll `_config.yml` configuration file.

### Support or Contact

Having trouble with Pages? Check out our [documentation](https://help.github.com/categories/github-pages-basics/) or [contact support](https://github.com/contact) and we’ll help you sort it out.
