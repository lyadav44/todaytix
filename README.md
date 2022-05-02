Take-home assignment for Test Automation Engineer for Today tix
# TodayTixAssessment
This project is created to automate the Login Page of Todaytix.com. I have used the TestNG framework to create this project and used the pom.xml file to add the dependencies.
I have created End to End Test cases. There are four runnable test cases to verify the basic login functionality of https://www.todaytix.com/
1. **verifyTitleOfLandingPage**: This test case is created to verify the title of the landing page after navigating to the URL: https://www.todaytix.com/

2. **verifyLogin**: This test case is to verify the positive scenario of the login page. 
--User navigates to the home page and clicks the login button, 
--Enters the Email address and password and click on the login button and 
--Verify the landing page after login into the site and Log out.
**Please Note: I have used test account credentials as username and password.**    

3. **verifyLoginWithoutEnteringPassword**: This test case covers the negative scenario to test the login page. 
--User clicks on the login button 
--And enters Email and leaves the password blank and 
--Click on the login button.
-- Verify the error message shown by the system.

4. **verifyLoginEnteringInvalidEmail**: This test case cover when an invalid email address is entered.
--User clicks on the login button 
--And enters an invalid Email address
--Click on the login button.
-- Verify the error message shown by the system.
 
**1. Include instructions to install dependencies**
--All the dependencies are added to **pom.xml** file (I have used dependencies for JUnit, selenium-java, TestNG, WebdriverManager)

**2. Include instructions to run the test scripts**
--Download the Project from the Github using Git command in git bash 
--Import the project in eclipse or other IDE
--The eclipse should have a TestNG plug-in. If not it can be installed through the Eclipse marketplace
--The test file is included in **AppTest.java** file under **src/test/java**. 
  I have used testNG annotation **@BeforeSuite**, **@BeforeTest**,**@Test**, **@AfterSuite**.
  All the test cases are written under @Test
--Run the TestNg test using the testng.xml file

**3. State what else you would do when given more time**
-- I would have created the TestNg Framework based on the page object model and created an object repository for storing all web elements and common methods of the webpage to improve the reusability.
-- I would have created a Base class where all the Browser setup, loading configuration file, and other reusable methods like the screenshot, handling sync issues
   and common methods are added. All page object classes will extend the BasePage, thus inheriting all the base methods
-- I would have used JSON file or excel or properties file to pass the data.
-- Though TestNg creates its report, I would have tried to integrate the ExtentReports with TestNG to produce 
   HTML-based documents that offer several advantages like pie charts, graphs, screenshots, and test summaries and are visually attractive too
-- I have covered only three basic test cases on login functionality but there can me more created more functional like
 1. Verifying Sign up functionality
 2. Verifying the login through the Google account
 3. Verifying the login through the Facebook account
 4. Verifying  the login through the Apple account
 5. Verifying the functionality of the Forget password link
 
