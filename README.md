# POM_Implemenation
**This project include POM implementation**
[**Prerequisite]([url](https://the-internet.herokuapp.com/login)) of this Project Automation:**
[**Prerequisite]([url](https://the-internet.herokuapp.com/tables)) of this Project Automation:**
[**Prerequisite]([url](https://the-internet.herokuapp.com/javascript_alerts)) of this Project Automation:**
[**Prerequisite]([url](https://the-internet.herokuapp.com/upload)) of this Project Automation:**
Install Visual studio
Install Specflow
Install Selenium Nunit ,SpecFlow , TestHostPlatform ,SDK , 
Install Nunit , Nunit3TestAdapter Package
Install AutoIT(For Dialog Box handling)
Install GIT Bash/GIT GUI

****GIT COMMANDS FOR PUSH YOUR SOLUTION ****
git add ExtentReport.html POM_Implementation.rar POM_IMPLEMENTATION_COMPLETE.mp4
git remote add origin https://github.com/Manniawan/POM_IMPLEMENTATION_COMPLETE.git
git commit -m "First Commit"
git push -f origin main
git branch
git checkout -b main
git push -f origin main


**Working flow of this project ......**

Implemented POM design Pattern 
Implemented BDD framework
Used Gerkhin language for step Definitions (testCases)
Each Test Case has its own implementation ...
Each test Case manage in POM for readablity and Reuseability 

**Feature**: 
	login test cases of all herokuapp...

**@LoginTests**
**Scenario: A_Login Automation**
Given I am on "Live" environment
And I have opened herokuapp page
And  I am logged in to "herokuapp" with "tomsmith" account
Then I verify that i am on Logout Page
Then I Logout from current page
Then I Close Current Page


**@TableTests**
**######################### TASK 2 IMPLEMENTATION #############################**
Scenario: Extract and verify data from the table (Dynamic Table Handling
Given I am on "Tables" environment
And I have opened herokuapp page
When I extract all company names from the table
Then I verify if "Jason Doe" exists in the table
Then I Close Current Page

**@U_AlertTests
########################## TASK 3 IMPLEMENTATION #############################**
Scenario Outline: Handling different JavaScript alerts
Given I am on "Alerts" environment
And I have opened herokuapp page
When I click on '<alertType>' alert
    Then I handle the '<alertType>' alert with '<action>'
    Then I should see the message '<expectedMessage>'
    
    Examples:
      | alertType  | action  | expectedMessage                      |
      | JS Alert  | accept  | You successfully clicked an alert   |
      | JS Confirm | accept  | You clicked: Ok                    |
      | JS Confirm | dismiss | You clicked: Cancel                |
      | JS Prompt  | Hello   | You entered: Hello                 |

#Scenario Outline: Z_Close Page 
#Then  I Close Current Page
@WU_AlertTests

**########################## TASK 4 Upload File And File Verification #############################**
Scenario: Upload file and verify success

  Given I am on "Upload" environment
  And I have opened herokuapp page
  When I upload a file "testfile"
  Then I should see the uploaded file name "testfile.txt"

  



Generated Custom Extent report at My own choice ....Provided custom code in solution can be checked !!!!!!
