# Xilinx Adaptive Computing Contest 2020
<img src="https://www.xilinx.com/content/dam/xilinx/imgs/press/media-kits/corporate/xilinx-logo.png" width="140">

Team Members: Seongdae Kim, Yearam Kim, Hoo Kim
Applied Contest Area: Catergory 2: Intelligent Video Anlytics

### Project Overview
#
 우리 프로젝트는 이미지 인식과 자율주행 기술을 사용하고 있음. 
이미지 인식하는데에 있어서 Vitis AI 를 활용할 수 있음. Vitis 어떤 AI 인지. (장점 서술)
거위를 추적하는 자율주행 로봇은 골프장을 돌면서 자동으로 모니터링하는 기능을 갖추고 있음.
거위를 인식하고, 추적하여 상업지역에 피해를 끼치는 거위를 내쫓는 것이 우리 프로젝트의 컨셉 
거위을 인식할 떄 거위 사진 데이터를 축적하여 연구소에 제공함으로서 animal behavior Modification과 Pest Control 분야에 효율적 사용이 가능함. 

#### Purpose and Expectations
#
We have designed a big durable amphibious goose remover badger
For the PGA golf course that spends $250k a year on goose removal and maintenance. 
Our amphibious badger is able to photograph and detect geese and chase them away. 
In addition to that the badger has GPS patrol path with collision avoidance and neural network image recognition.
Our badger helps drive out the geese that interfere with the business in a low maintenance and cost-effective manner instead of the old fashion way of shooting them.


    
#### Our Robot
#
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
#### 성장 가능성
#
#### Our Action Plan
<img width="1157" alt="스크린샷 2020-12-08 오전 11 53 28" src="https://user-images.githubusercontent.com/68213891/101432328-ff179c80-394b-11eb-9274-44f355d08f6e.png">

#
#### Badger Robot
1. Badger Robot Design

2. 배져 로봇 블록 다이어그램 
    (a. 원래 다이어그램, b. ZU104로 electrical 파트가 대체된 다이어그램)
3. 장단점 비교
4. Geese detection by Vitis AI vs. 기존 detection / conversion이 가능하면 함께 비교 
#
#### Relevant Resource Files (Schematics, Code, CAD)
기존의 파일들을 정리하고 ZCU104 적용한 것을 시간이 허락되는데로 표현 
- Schematics
- Code
- CAD

#### Appendix

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
<img width="468" alt="image" src="https://user-images.githubusercontent.com/68213891/101432617-86651000-394c-11eb-82ae-f4fb8250ced8.png">
     
     
### Sd card    
Our project tried two approaches 1) Follow the user guide to generate the image 2) download and use the pre-imaged file    
     
To use Serial Communication, this driver should be installed, and you can get the file from the    
https://pynq.readthedocs.io/en/latest/getting_started/zcu104_setup.html 

<img width="468" alt="image" src="https://user-images.githubusercontent.com/68213891/101432623-88c76a00-394c-11eb-90f5-e4087b271a74.png">
<img width="468" alt="image" src="https://user-images.githubusercontent.com/68213891/101432629-8c5af100-394c-11eb-877d-8c30236577dd.png">
<img width="468" alt="image" src="https://user-images.githubusercontent.com/68213891/101433164-97fae780-394d-11eb-8fe7-0a92528b7d83.png">
<img width="369" alt="image" src="https://user-images.githubusercontent.com/68213891/101432636-8ebd4b00-394c-11eb-9daa-93f7ff149d6d.png">

     
### Vethernet    
<img width="372" alt="image" src="https://user-images.githubusercontent.com/68213891/101432642-91b83b80-394c-11eb-822f-e0f0f83fa3ad.png">
<img width="202" alt="image" src="https://user-images.githubusercontent.com/68213891/101432647-9381ff00-394c-11eb-8925-b88c91683505.png">
### ZCU104 webinar   
https://event.on24.com/eventRegistration/console/EventConsoleApollo.jsp?&eventid=2552508&sessionid=1&username=&partnerref=&format=fhvideo1&mobile=&flashsupportedmobiledevice=&helpcenter=&key=12AF8FECC081E16A1AD0DA74931F1585&newConsole=true&nxChe=true&text_language_id=en&playerwidth=748&playerheight=526&eventuserid=343773765&contenttype=A&mediametricsessionid=332153072&mediametricid=3593851&usercd=343773765&mode=launch
    
### ZCU104 Smart Camera Demo Design
https://github.com/Xilinx/Embedded-Reference-Platforms-User-Guide/blob/master/Docs/overview.md#213-zcu104-smart-camera-platform   
    
http://www.pynq.io/ pynq   
https://www.youtube.com/watch?v=emXEmVONk0Q  
    
Setup: Boot from SD Card

<img width="468" alt="image" src="https://user-images.githubusercontent.com/68213891/101432651-967cef80-394c-11eb-9164-e83aeb355a99.png">

<img width="468" alt="image" src="https://user-images.githubusercontent.com/68213891/101432659-9977e000-394c-11eb-9ee6-2de851b2f24e.png">

<img width="468" alt="image" src="https://user-images.githubusercontent.com/68213891/101432672-9d0b6700-394c-11eb-8ce2-f82c4b2e6db8.png">
