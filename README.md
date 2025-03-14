# JMeter Performance Testing for Booking and DMoney APIs

#### This project contains JMeter test plans and resources for performance testing of the Booking API and functional testing of the DMoney API. The tests include load and stress testing for the Booking API and transaction-based testing for the DMoney API.

## Table of Contents
1. Overview
2.  Tools and Technologies I have used
3. prerequisites
4. How to Run the Tests
5. Results and Reports

## Overview
This project includes two main tasks:
1. Booking API Performance Testing:
   - Perform load and stress testing on the booking API.
   - Simulate 120,000 users over a 12-hour period performing login, create booking, and search booking operations.
   - Generate HTML reports and Excel summaries for both load and stress test
2. DMoney API Functional Testing:
   - Simulate transactions such as deposits, money transfers, and payments using CSV data.
   - Validate all transactions using assertions.
   - Generate an HTML report for the test results.
  
## Tools and Technologies I have used:
   - Postman
   - JMeter
   - Git and GitHub
   - Excel

## Prerequisites
   Before running the tests, ensure you have the following installed:
   1. JMeetr:
      - download and install Apache jMeter from https://jmeter.apache.org/ .
      - Ensure Jmeter is added to your system's PATH for easy execution.
   2. Java:
       - JMeter requires Java to run. Install Java JDK version 8 or higher.
       - Ensure Java is added to your system's PATH.
   3. Git:
       - Install Git to clone this repository.
   4. CSV Files:
       - The CSV files (deposit.csv, sendmoney.csv, payment.csv ) are prepopulated with sample data. Modify them as needed for your tests.
  
  ## How to Run the Tests<br>
   **Booking API Tests**
  1. Clone the Repository: 
   ``` git clone https://github.com/nadim45448/jmeter-assignment ```
  3. Run the Load Test and Generate HTML report
     - Execute the booking.jmx file using JMeter:
      ``` jmeter -n -t booking.jmx -l booking.jtl -e -o Reports ```       
     - Replace -l booking.jtl with the desired output file name.
  4. Open the index.html file in the Reports/ folder to view the results.
  5. Stress rest:
     - Follow the same steps as the load test but adjust the number of threads/users in the Thread Group.
    
  **DMoney API Test:**
  1. Run the Test Plan and Generate HTML Report
     - Execute the dmoney.jmx file using JMeter: 
      ``` jmeter -n -t dmoney.jmx -l dmoney.jtl -e -o Reports ```
  2.   Open the index.html file in the Reports/ folder to view the results.

## Results and Reports
 **Booking API**
  - **Load Test Requests Summary and Statistics**<br>
   ![image](https://github.com/user-attachments/assets/66dd1c40-6ff8-4cf2-b65a-f71218df753d)

  - **Load Test Report**<br>
   ![image](https://github.com/user-attachments/assets/f1be0506-d2d1-45e6-b248-26a19ba48b64)
   
  - **Stress Test Requests Summary and Statistics**<br>
    ![image](https://github.com/user-attachments/assets/dde3ed72-f577-435d-ac51-5c2cebd841cd)

  - **Stress Test Report**<br>
   ![image](https://github.com/user-attachments/assets/34ad24a2-983b-42e5-9247-8804a1df9571)

  - 📊 **<a href="https://docs.google.com/spreadsheets/d/13FlXgoEg1emIJRHJocIbhRUfDzg6O5d_/edit?usp=sharing" target="_blank" style="color: blue; text-decoration: none;">View Booking API Test Report</a>**


 **DMoney API**
  - **Requests Summary and Statistics**<br>
    ![image](https://github.com/user-attachments/assets/9e0faf5f-d827-41b3-b246-b36f61797fa9)




    


    
  


    

    

   

    





    
    
      
     
     
     
     
   





