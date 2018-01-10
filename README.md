# Performance Testing with JMeter
This repo contains some JMeter files that were used to run some practice performance tests using JMeter on some open API's and a locally hosted web app.

In order to run the tests the JMeter app is needed which can be found at the following link:

http://jmeter.apache.org/download_jmeter.cgi

Documentation can also be found at this link to explain how to write a test plan and run the tests.

###### Brief Guide to writing a test plan in the format in the .jmx files when opened in JMeter:

1. Create a thread group by right clicking on a test plan clicking add and then thread groups.

2. In the thread group set the amount of users you wish to simulate using the number of threads and ramp up period.

3. Right click on the thread group and add a HTTP request default found in the Config Element section.

4. Enter the Web Server Protocol (HTTP) and the server name or base url in the Server Name or IP option.

5. Right click the thread group and add a HTTP Request in the Sampler section.

6. Enter the action you wish to make, e.g GET and the remaining part of the url after what was placed in the Request Default. (The default must end on a /).

7. Right click on the thread group and add a View Results Tree in the Listener section.

8. Save the test plan and then press the green play button to run the test and view the result in the Results Tree where a green response is a success and a red a failure. More information on the response can be viewed by clickin on it.

This is a basic guide to creating a basic test plan. More in depth versions with more complicated requests and plans can be found in the files in this repo as well as a summary printed to xml for one of the test plans. For more guidance see the link above. 
