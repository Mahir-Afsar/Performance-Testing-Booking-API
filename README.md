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

## Reporting in jmeter

I’ve completed performance test on frequently used API for test App. 
Test executed for the below mentioned scenario in https://restful-booker.herokuapp.com/

- 500 Concurrent Request with 1 Loop Count; Avg TPS for Total Samples is ~ 35 And Total Concurrent API requested: 3000.
- 1000 Concurrent Request with 1 Loop Count; Avg TPS for Total Samples is ~ 100 And Total Concurrent API requested: 6000.
- 1300 Concurrent Request with 1 Loop Count; Avg TPS for Total Samples is ~ 106 And Total Concurrent API requested: 7800.
- 1500 Concurrent Request with 1 Loop Count; Avg TPS for Total Samples is ~ 81 And Total Concurrent API requested: 9000.

While executed 1500 concurrent request, found  24 request got connection timeout and error rate is 0.27%. 

Summary: Server can handle almost concurrent 7800 API call with almost zero (0) error rate.
