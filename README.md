# POM_Implemenation<br>
**This project include POM implementation**<br>
[**Prerequisite]([url](https://the-internet.herokuapp.com/login)) of this Project Automation:**<br>
[**Prerequisite]([url](https://the-internet.herokuapp.com/tables)) of this Project Automation:**<br>
[**Prerequisite]([url](https://the-internet.herokuapp.com/javascript_alerts)) of this Project Automation:**<br>
[**Prerequisite]([url](https://the-internet.herokuapp.com/upload)) of this Project Automation:**<br>
Install Visual studio<br>
Install Specflow<br>
Install Selenium Nunit ,SpecFlow , TestHostPlatform ,SDK , <br>
Install Nunit , Nunit3TestAdapter Package<br>
Install AutoIT(For Dialog Box handling)<br>
Install GIT Bash/GIT GUI<br>

****GIT COMMANDS FOR PUSH YOUR SOLUTION ****<br>
**git add ExtentReport.html POM_Implementation.rar POM_IMPLEMENTATION_COMPLETE.mp4<br>
git remote add origin https://github.com/Manniawan/POM_IMPLEMENTATION_COMPLETE.git<br>
git commit -m "First Commit"<br>
git push -f origin main<br>
git branch<br>
git checkout -b main<br>
git push -f origin main**<br>


**Working flow of this project ......**<br>

Implemented POM design Pattern <br>
Implemented BDD framework<br>
Used Gerkhin language for step Definitions (testCases)<br>
Each Test Case has its own implementation ...<br>
Each test Case manage in POM for readablity and Reuseability <br>

**Feature**: <br>
	login test cases of all herokuapp...<br>

**@LoginTests**<br>
**Scenario: A_Login Automation**<br>
Given I am on "Live" environment<br>
And I have opened herokuapp page<br>
And  I am logged in to "herokuapp" with "tomsmith" account<br>
Then I verify that i am on Logout Page<br>
Then I Logout from current page<br>
Then I Close Current Page<br>


**@TableTests**<br>
**######################### TASK 2 IMPLEMENTATION #############################**<br>
Scenario: Extract and verify data from the table (Dynamic Table Handling<br>
Given I am on "Tables" environment<br>
And I have opened herokuapp page<br>
When I extract all company names from the table<br>
Then I verify if "Jason Doe" exists in the table<br>
Then I Close Current Page<br>

**@U_AlertTests<br>
########################## TASK 3 IMPLEMENTATION #############################**<br>
Scenario Outline: Handling different JavaScript alerts<br>
Given I am on "Alerts" environment<br>
And I have opened herokuapp page<br>
When I click on '<alertType>' alert<br>
    Then I handle the '<alertType>' alert with '<action>'<br>
    Then I should see the message '<expectedMessage>'<br>
    
    Examples:<br>
      | alertType  | action  | expectedMessage                      |<br>
      | JS Alert  | accept  | You successfully clicked an alert   |<br>
      | JS Confirm | accept  | You clicked: Ok                    |<br>
      | JS Confirm | dismiss | You clicked: Cancel                |<br>
      | JS Prompt  | Hello   | You entered: Hello                 |<br>

#Scenario Outline: Z_Close Page <br>
#Then  I Close Current Page<br>
@WU_AlertTests<br>

**########################## TASK 4 Upload File And File Verification #############################**<br>
Scenario: Upload file and verify success<br>

  Given I am on "Upload" environment<br>
  And I have opened herokuapp page<br>
  When I upload a file "testfile"<br>
  Then I should see the uploaded file name "testfile.txt"<br>

  



Generated Custom Extent report at My own choice ....Provided custom code in solution can be checked !!!!!!
