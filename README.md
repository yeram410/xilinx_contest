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
### Project Overview
We have designed a big durable amphibious goose remover badger
For the PGA golf course that spends $250k a year on goose removal and maintenance. 
Our amphibious badger is able to photograph and detect geese and chase them away. 
In addition to that the badger has GPS patrol path with collision avoidance and neural network image recognition.
Our badger helps drive out the geese that interfere with the business in a low maintenance and cost-effective manner instead of the old fashion way of shooting them.

#
    
### Our Robot

<img width="700" alt="스크린샷 2020-12-08 오후 12 57 45" src="https://user-images.githubusercontent.com/68213891/101438123-faa3b180-3954-11eb-9c50-c3636df69425.png">

<img width="650" alt="스크린샷 2020-12-08 오후 12 49 35" src="https://user-images.githubusercontent.com/68213891/101437577-d693a080-3953-11eb-9df2-c81780997e65.png">

<img width="700" alt="스크린샷 2020-12-08 오후 12 50 09" src="https://user-images.githubusercontent.com/68213891/101437604-e9a67080-3953-11eb-9905-a6513deb060e.png">

<img width="700" alt="스크린샷 2020-12-08 오후 1 09 35" src="https://user-images.githubusercontent.com/68213891/101438864-a5689f80-3956-11eb-83cb-d5a0c623cebc.png">
Autonomous Driving Video : https://youtu.be/4dddvqC3Yrw



##### **- Originality and Differentiation**



##### **- Technical Development**

#
#### Applied Xilinx Product
##### - Features of Xilinx products applied to items
##### - Topics for utilizing technology applied to items
#
#### Bill Of Materials
#
#### Full Instructions
#
#### Badger Robot
1. Badger Robot Design

2. 배져 로봇 블록 다이어그램 
    (a. 원래 다이어그램, b. ZU104로 electrical 파트가 대체된 다이어그램)

3. 장단점 비교
4. Comparing goose detection(original model vs sample model)      
<img width="178" alt="image" src="https://user-images.githubusercontent.com/68213891/101438747-65a1b800-3956-11eb-8692-d8af0b869d97.png">
    
The original detection FPS are less than 4.5 but accuracy is more than 96.3%.
When we used ZCU104 board with yolov3 model to test, the models show good FPS near the performance FPS measured before. But when test 50 images with yolov3 vcc model, it showed bad result. Almost images are recognized as bird, but the accuracy are very low(average: 54.6%, standard variation: 44.71%). It is expected that the advantages of both cases can be used at the same time if the model is made and used by focusing more on Goose.


#
#### Relevant Resource Files (Schematics, Code, CAD)
기존의 파일들을 정리하고 ZCU104 적용한 것을 시간이 허락되는데로 표현 
- Schematics
- Code
- CAD
#
#### Our Action Plan
<img width="1157" alt="스크린샷 2020-12-08 오전 11 53 28" src="https://user-images.githubusercontent.com/68213891/101432328-ff179c80-394b-11eb-9274-44f355d08f6e.png">
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
     
     
### Sd card    
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

