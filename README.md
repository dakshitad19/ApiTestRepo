# ApiTestRepo
**# ApiTestRepo
IMP NOTE**
1.	Sometimes API are giving 429 instead of 200 status code, please have a look at script (
    test cases) and code it is correctly represented
2.	Sometimes API’s are giving unexpected response pattern also like content-type, please have a look at script, code & framework.


**TITLE**
API automation using Rest Assured Library has been used 
Deliverables: 
•	Framework – Rest Assured
•	Config Reader File – Has all the common method to fetch the config.properties file.
•	Test cases are separated with different scenarios, there can be single class file but public methods of each test is different
•	Test case Report generation are in ALLURE HTML format will be open in browser.


**LANGUAGE**
 JAVA

**BUILD AUTOMATION TOOL**
Maven 

** POM File**
Pom.xml consist of all dependencies 

**IDE **
Intellj

PROJECT STRUCTURE DETAILS 
1.	Config.properties file has the Hostname(hosturl) and Endpoints
2.	Location of Config Reader =  RestAssured<  src < main <utils (inside this package , ConfigReader File is present 
3.	Location of Test files = RestAssured < src <main <test  <java (has all the test classes)


**REQUIREMENT #1**
1.	Location -  RestAssured < src <main <test < java
2.	AllEmployeeTest.java - contains the Assertion of status code & profile_image_empty for all emps through looping
3.	Reusable methods have been used 
4.	BaseUrl static method has been created once, using BaseUrl in entire program wherever it is needed

**REQUIREMENT #2**
1.	Location - RestAssured < src <main <test < java
2.	EmpRecordTest.java -  emp id has been fetched through an excel sheet (location – SingleEmpRecord(folder) < xlsx file is present  
3.	BaseUrl has been set  in config file 
4.	empID has been taken from xlsx sheet and adding empID in URL through code
5.	Assertion of 200 is present 
6.	Assertion of response body(in separate java file) -  In EmpecordResponseTest.java (< src <main <test < java) , along with the single emp record data has been picked from excel 
7.	Assertion of Verifying msg body (in separate java file) -  In EmpecordResponseMsgTest.java , along with the single emp record data has been picked from excel.




**REPORT GENERATION (ALLURE)**
1.	If using Inellj import the framework from Github run following commands
•	mvn clean package  - For BUILD SUCCESS
•	mvn compile package 
•	Go to < src <main <test < java -> Run All Tests, once all test has been executed in terminal of Intellij



**2.	Run command =  allure serve allure-results** 
3.	 As this allure-results folder is present in root directory.
4.	Allure Reports will be open in browser automatically after running this command , it will be in index.html format.



**IMP NOTE**
1.	Sometimes API are giving 429 instead of 200 status code, please have a look at script and code it is correctly represented
2.	Sometimes API’s are giving unexpected response pattern also like content-type,  please have a look at script , code & framework 




CREATED_BY
Dakshita Dhaundiyal
dakshitad19@gmail.com



