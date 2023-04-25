# Performance Testing on a REST API using JMeter

## How to run this project
- Clone this project
- Open with JMeter / Command Shell
- Run Command:
```bash
jmeter -n -t Hotel-Booking-Project_T500.jmx -l report\Hotel-Booking-Project_T500.jtl
jmeter -g report\Hotel-Booking-Project_T500.jtl -o report\Hotel-Booking-Project_T500.html

jmeter -n -t Hotel-Booking-Project_T1000.jmx -l report\Hotel-Booking-Project_T1000.jtl
jmeter -g report\Hotel-Booking-Project_T1000.jtl -o report\Hotel-Booking-Project_T1000.html

jmeter -n -t Hotel-Booking-Project_T1300.jmx -l report\Hotel-Booking-Project_T1300.jtl
jmeter -g report\Hotel-Booking-Project_T1300.jtl -o report\Hotel-Booking-Project_T1300.html

jmeter -n -t Hotel-Booking-Project_T1500.jmx -l report\Hotel-Booking-Project_T1500.jtl
jmeter -g report\Hotel-Booking-Project_T1500.jtl -o report\Hotel-Booking-Project_T1500.html
```
## Technology used:
- JMeter

## Pre-requisite:
- Jdk
- JMeter

## 🔗 API Documentation:
https://restful-booker.herokuapp.com/apidoc/index.html#api-Booking
