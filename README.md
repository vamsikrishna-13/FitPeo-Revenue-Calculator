To begin with, create a new Java project without using Maven. 

For this, you will need to manually download the necessary dependencies. First, download the Selenium Java jar files from the Selenium Downloads page. Additionally, download the WebDriverManager jar files from the Maven Repository. Once these jar files are downloaded, you will need to add them to your project's build path to ensure the necessary libraries are included.
Next, set up the WebDriver.

If you are using Chrome, you will need to install ChromeDriver, which can be downloaded from the official site. However, if you are using WebDriverManager (which is the recommended approach), it will automatically handle the setup of the driver for you, meaning no manual intervention is needed. 

If you choose to set the path manually, make sure to include the following line in your code: System.setProperty("webdriver.chrome.driver", "/path/to/chromedriver");.
After setting up the WebDriver, create a new Java class (e.g., FitPeoAutomation) to implement the Selenium WebDriver script. This script will automate tasks such as opening the FitPeo homepage, navigating to the Revenue Calculator page, interacting with UI elements like sliders, text fields, and checkboxes, and verifying that the correct Total Recurring Reimbursement value is displayed.

To run the Selenium script, there are two options available. Option 1 is to run the script within an Integrated Development Environment (IDE) such as Eclipse or IntelliJ. After opening your project, simply right-click the Java file (e.g., FitPeoAutomation.java) and select the "Run" option. The script should then open a Chrome browser, perform the tasks as described, and close the browser when completed.
Option 2 involves running the script via the command line if you're not using Maven. 

To do this, first compile the Java file by opening the terminal or command prompt and navigating to the directory containing the FitPeoAutomation.java file. Use the following command to compile the file:
"javac -cp .:selenium-java-4.x.x.jar:webdrivermanager-5.x.x.jar FitPeoAutomation.java"


After compilation, run the Java file with this command:
"java -cp .:selenium-java-4.x.x.jar:webdrivermanager-5.x.x.jar FitPeoAutomation"


Finally, verify that the script has executed successfully by checking the following steps:

 ->The script should open the FitPeo homepage and navigate to the Revenue Calculator page.

->It will scroll to the slider section and adjust the slider to the value of 820.

->The script will then update the text field to 560 and confirm that the slider moves accordingly.

->Next, it will select the required CPT codes and check if they are correctly selected.

->Lastly, it will ensure that the Total Recurring Reimbursement value is displayed as $110,700, confirming the correctness of the operation.
