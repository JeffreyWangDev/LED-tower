# LED-tower

## Goal
A easy to assemble, good looking, NON creaking acylic led light tower. 


https://cad.onshape.com/documents/002277c803df31649a501ead/w/61b45c9ab1050f526b4947af/e/f2e1a3ee0f85b37ee5d59af5
 https://oshwlab.com/jeffrey098765437/led-tower-pcb
 
## Why??
I always loved playing with lights. I love how it can show so much and look so cool in the process. While I have made many projects with LEDS in the past, I never made my own control board or a pcb for those leds. For this project, I want to develop an ESP32-based main board with a greater than 7 amp BEC for the LEDs, and 3-4 USB-C ports for charging with full USB 3.0 support. 

## Challenges
1. Figure out a way to attach the acrylic pieces to the aluminum frame
2. Figure out how to support usb 3.0, its all just magic for me right now
3. Dont burn down my house

## Software 
I will be ether using WLED or making a simple dashboard with python to control everything 


<img width="500" height="832" alt="image" src="https://github.com/user-attachments/assets/e1e43e13-0289-4524-953f-7f0fb8e83b50" />
<img width="153" height="984" alt="image" src="https://github.com/user-attachments/assets/15ad285b-f689-48c9-add3-0bb87fc6fdf8" />
<img width="590" height="520" alt="image" src="https://github.com/user-attachments/assets/0d61bee7-6afe-4506-86d1-d0bb6ae7bf0e" />


<img width="847" height="892" alt="image" src="https://github.com/user-attachments/assets/8ca6466d-665d-4cc2-a6e5-f9494f89068a" />


For wiring, its just 5v from the control board and a control sig line.


BOM:

| Item  | Price |
| ------------- | ------------- |
| PCB  | $58  |
| 6061 Aluminum  | $120  |
| [Acrylic ](https://www.homedepot.com/p/OPTIX-24-in-x-48-in-x-0-220-1-4-in-Clear-Acrylic-Sheet-MC-20/202038051) | $88 |
| [M3 by 16](https://www.amazon.com/BNUOK-180pcs-Socket-Threads-Spanner/dp/B0DJQGGGJS?th=1)  | $8 |
| [M3 by 10](https://www.amazon.com/M3-0-5-Socket-Stainless-Machine-Fasteners/dp/B0949K3233/)  | $6 |
| [M3 by 6](https://www.amazon.com/Socket-Screws-Bolts-Thread-100pcs/dp/B07CMRQ3TB?th=1)  | $7 |
| [M6 by 12](https://www.amazon.com/M6-Countersunk-Socket-Screws-Furniture/dp/B0CKW4MHGZ/)  | $8 |
| [M6 by 12](https://www.amazon.com/Stainless-Fasteners-Replacement-M6-1-0mm-Hexagonal/dp/B0CZQRH3L2)  | $6 |
| [15v psu](https://www.amazon.com/COOLM-100-240V-Supply-Adapter-Converter/dp/B07CBTWT1V)  | $25 |
| [Barrel jacks](https://www.amazon.com/FILSHU-Socket-Threaded-Connector-Adapter/dp/B08271YLXZ/)  | $8 |
| [Headers](https://www.amazon.com/dp/B0B42G18JH)  | $10 |
| [Antenna](https://www.amazon.com/dp/B0B42G18JH)  | $10 |
