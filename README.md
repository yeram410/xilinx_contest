# Xilinx Adaptive Computing Contest 2020
<div>
<img width="140" alt="BADGER LOGO" src="https://user-images.githubusercontent.com/68213891/101435800-4d2e9f00-3950-11eb-93ef-5e960c513933.png">
    
<img src="https://www.xilinx.com/content/dam/xilinx/imgs/press/media-kits/corporate/xilinx-logo.png" width="140">
</div>


#### Team Members: Seongdae Kim, Yearam Kim, Hoo Kim    
#### Applied Contest Area: Catergory 2: Intelligent Video Anlytics
#
### Project Purpose and Expectations
We propose a driving robot optimized for golf courses that use image recognition and self-driving technology.
What's noteworthy in this paper is that we used Vitis AI, which Xilinx developed for all developers, to recognize images.
Self-driving robots that track geese are equipped with automatic monitoring functions as they go around golf courses.
The concept of our project is that several robots send and receive data from each other, recognize and track geese, and chase them away that cause damage to commercial areas. When robots recognize geese, they accumulate geese photo data and provide it to the lab, enabling efficient use in the area of animal behabior modification and Pest control Industry.

#
    
### Our Robot

#### Originality and Differentiation
We have designed a big durable amphibious goose remover badger
For the PGA golf course that spends $250k a year on goose removal and maintenance. 
Our amphibious badger is able to photograph and detect geese and chase them away. 
In addition to that the badger has GPS patrol path with collision avoidance and neural network image recognition.
Our badger helps drive out the geese that interfere with the business in a low maintenance and cost-effective manner instead of the old fashion way of shooting them.


#### Technical Development
1. Easy to Drive  
2. Neural Network Image Recognition    
3. Amphibious    
4. Autonomous    
<img width="700" alt="스크린샷 2020-12-08 오후 2 52 47" src="https://user-images.githubusercontent.com/68213891/101445552-0c8d5080-3965-11eb-834e-df167fb6b7ad.png">

<img width="700" alt="스크린샷 2020-12-08 오후 2 37 29" src="https://user-images.githubusercontent.com/68213891/101444487-eff01900-3962-11eb-81a3-70185d4f37eb.png">

<img width="700" alt="스크린샷 2020-12-08 오후 12 50 09" src="https://user-images.githubusercontent.com/68213891/101437604-e9a67080-3953-11eb-9905-a6513deb060e.png">

<img width="700" alt="스크린샷 2020-12-08 오후 1 09 35" src="https://user-images.githubusercontent.com/68213891/101438864-a5689f80-3956-11eb-83cb-d5a0c623cebc.png">
Autonomous Driving Video : https://youtu.be/4dddvqC3Yrw

#
### Applied Xilinx Product
According to the guidance of the contest condition, we use the following items for entering the contest category 2: Intelligent Video Analytics.
1. Zynq UltraScale - video codec unit (VCU) and the deep learning processing unit (DPU)
2. MPSoC ZCU104 Evaluation Kit 
3. Vitis AI - used 3 major machine models - classification, ssd, Yolov3

##### - Features of Xilinx products applied to items

##### - Topics for utilizing technology applied to items
#
#### Bill Of Materials
#
#### Full Instructions
Connecting to Badger Robot over WiFi
1.	Open up the lid of the waterproof housing and flip the red power switch on the battery (located front right side)
    a.	You should see a number of LEDs come on inside the housing
    b.	You may now close the lid and go to your computer
2.	On a laptop, connect to Kevin’s internal WiFi:
    a.	SSID: TP-LINK_4F36 (Badger?)
    b.	PASSWORD: 79393126 (need not to type for operation mode) 
3.	Once connected, open up an SSH client such as PUTTy and SSH into the main Pi
    a.	Enter the IP Address of the robot into putty: 192.168.0.101
        i.	Note: try 192.168.0.100 if .101 doesn’t work
    b.	Click connect
    c.	Once connected, you will be prompted for a username and password
        i.	USERNAME: xxx (intentionally hidden)
        ii.	PASSWORD: xxxxxx (intentionally hidden)
	      Note: Now that you are connected to the main Pi
4.	Start the program for the robot
    a.	In the PUTTy terminal, type: cd badger
    b.	Once in the badger folder, type: python BADGER.py
    c.	This will start the program for STEVE
	      Note: Now that the program is running
5.	Connect to the robot in the GUI
    a.	Run badger_robot_connect.py on your laptop
    b.	In the GUI, click connect
      Note: You are now connected to STEVE and have the ability to control it

GUI usage
1.	Code Download for GUI operation from GitBucket

#
### Badger Robot (BADGR)
The robot is designed for manufacturable, advanced prototype of the autonomous and amphibious goose chasing system, called the BADGR, which was prototyped in 2018. This system must meet the constraints outlined below and also be designed to be easily reproducible to meet the manufacturable specification. 
Requirement / Constraint and Description
1) Goose Detection: BADGR must be able to identify Canadian Geese with a camera
2) Amphibious Design: BADGR must be able to float and maneuver well in water
3) GPS Navigation: BADGR must be able to accurately navigate a path with GPS
4) Cloud Connectivity: BADGR must be able to upload all goose images to be shared with A&K	
5) Autonomous Design: BADGR must be able to be set up once and operate without further human interaction

The system will also have a base station, called the BADGR Den, which will be the housing station for the BADGR when it is not in use. This will have GPS and Radio communication with the BADGR and also allow for uploading geese images to the cloud. This is the extent of the scope of our project. It has been set based on a careful review of last year’s project in unison with communication with our sponsor about what they want in an upgraded version of the BADGR.

#### Badger Robot Design

#### Badger Robot System Diagram
#### Key features
##### Comparing goose detection(original model vs sample model)      
<img width="178" alt="image" src="https://user-images.githubusercontent.com/68213891/101438747-65a1b800-3956-11eb-8692-d8af0b869d97.png">
    
The original detection FPS are less than 4.5 but accuracy is more than 96.3%.
When we used ZCU104 board with yolov3 model to test, the models show good FPS near the performance FPS measured before. But when test 50 images with yolov3 vcc model, it showed bad result. Almost images are recognized as bird, but the accuracy are very low(average: 54.6%, standard variation: 44.71%). It is expected that the advantages of both cases can be used at the same time if the model is made and used by focusing more on Goose.


#
#### Relevant Resource Files (Schematics, Code, CAD)
- Schematics
- Code
- CAD

#

### Appendix

Contest Information: Adaptive Computing Developer Contest with Xilinx    
https://www.hackster.io/contests/xilinxadaptivecomputing   
   
Forum Resource link:   
https://forums.xilinx.com/t5/Adaptive-Computing-Challenge/bd-p/ACC_2020   
   
ZCU 104 Evaluation Kit Info.    
https://www.youtube.com/watch?v=DXiYMplqm2Q   
    
Hardware Configuration   
https://www.xilinx.com/products/boards-and-kits/zcu104.html#hardware    

<img width="468" alt="image" src="https://user-images.githubusercontent.com/68213891/101432463-42720b00-394c-11eb-8620-02acdc8c29d4.png">
    
Starting Manual   
https://github.com/Xilinx/ZCU104-reVISION-Getting-Started    
License Generation    
Note: For Vitis AI, there is no need to generate any Licnese   
    
<img width="468" alt="image" src="https://user-images.githubusercontent.com/68213891/101432609-82d18900-394c-11eb-8b53-59857fe9bbb6.png">
    
Vivado Design Suite User Guide:     
http://www.xilinx.com/cgi-bin/docs/rdoc?v=latest;d=iil.pdf;a=ObtainManageLicense     
    
##### USB-UART driver: CP210x USB to UART bridge    
To use Serial Communication, this driver should be installed, and you can get the file from the following site.     
https://xilinx-wiki.atlassian.net/wiki/spaces/A/pages/18842446/Setup+a+Serial+Console    
    
#### Booting option from the user-guide     
Note: SD1 Boot Mode is mainly used in this project with UART serial communication for debugging purpose.     
     
<img width="600" alt="image" src="https://user-images.githubusercontent.com/68213891/101432617-86651000-394c-11eb-82ae-f4fb8250ced8.png">
     
     
### SD card    
Our project tried two approaches 1) Follow the user guide to generate the image 2) download and use the pre-imaged file     
     
          
Note: after following the instructions, you may build the image; however, you may add and install a few files to make the image fully working with the provided examples in the user guide.     
     
To use Serial Communication, this driver should be installed, and you can get the file from the     
     
Note: Considered the pynq versions, however, in the project, this is not used as we decide to keep using petalinux + Vitis AI.      
     
Note: you may use the following link for checking information about pynq.     
https://pynq.readthedocs.io/en/latest/getting_started/zcu104_setup.html     
     
Example: Tried with the team’s laptop to run pynq + jupyter     

<img width="600" alt="image" src="https://user-images.githubusercontent.com/68213891/101432623-88c76a00-394c-11eb-90f5-e4087b271a74.png">
<img width="600" alt="image" src="https://user-images.githubusercontent.com/68213891/101432629-8c5af100-394c-11eb-877d-8c30236577dd.png">
<img width="600" alt="image" src="https://user-images.githubusercontent.com/68213891/101433164-97fae780-394d-11eb-8fe7-0a92528b7d83.png">
     
          
          
IP configuration     
     
<img width="500" alt="image" src="https://user-images.githubusercontent.com/68213891/101432636-8ebd4b00-394c-11eb-9daa-93f7ff149d6d.png">
    
Note: we only use the ethernet    
      
### Vethernet    
<img width="500" alt="image" src="https://user-images.githubusercontent.com/68213891/101432642-91b83b80-394c-11eb-822f-e0f0f83fa3ad.png">
<img width="400" alt="image" src="https://user-images.githubusercontent.com/68213891/101432647-9381ff00-394c-11eb-8925-b88c91683505.png">

### ZCU104 webinar     
     
https://event.on24.com/eventRegistration/console/EventConsoleApollo.jsp?&eventid=2552508&sessionid=1&username=&partnerref=&format=fhvideo1&mobile=&flashsupportedmobiledevice=&helpcenter=&key=12AF8FECC081E16A1AD0DA74931F1585&newConsole=true&nxChe=true&text_language_id=en&playerwidth=748&playerheight=526&eventuserid=343773765&contenttype=A&mediametricsessionid=332153072&mediametricid=3593851&usercd=343773765&mode=launch    
    
### ZCU104 Smart Camera Demo Design
https://github.com/Xilinx/Embedded-Reference-Platforms-User-Guide/blob/master/Docs/overview.md#213-zcu104-smart-camera-platform   
    
http://www.pynq.io/ pynq   
https://www.youtube.com/watch?v=emXEmVONk0Q  
    
Setup: Boot from SD Card

<img width="600" alt="image" src="https://user-images.githubusercontent.com/68213891/101432651-967cef80-394c-11eb-9164-e83aeb355a99.png">

<img width="600" alt="image" src="https://user-images.githubusercontent.com/68213891/101432659-9977e000-394c-11eb-9ee6-2de851b2f24e.png">


AI library      
https://www.xilinx.com/support/documentation/sw_manuals/vitis_ai/1_1/ug1354-xilinx-ai-sdk.pdf 

<img width="600" alt="image" src="https://user-images.githubusercontent.com/68213891/101432672-9d0b6700-394c-11eb-8ce2-f82c4b2e6db8.png">
https://github.com/Xilinx/Vitis-AI

### Our Action Plan
<img width="1157" alt="스크린샷 2020-12-08 오전 11 53 28" src="https://user-images.githubusercontent.com/68213891/101432328-ff179c80-394b-11eb-9274-44f355d08f6e.png">
