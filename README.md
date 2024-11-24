FITPEO-REVENUE-CALCULATOR
Create a new Java project (no Maven).
Manually Download Dependencies:
Download the Selenium Java jar files from "Selenium Downloads".
Download WebDriverManager jar files from "WebDriverManager" on "Maven Repository".
-->Add JARs to Project:
Add the downloaded JARs to your project's build path.
Set Up the WebDriver
Install ChromeDriver (for Chrome users):
You can download ChromeDriver from here.
If you're using WebDriverManager (as recommended), it will automatically handle the driver setup.
Set the WebDriver Path:
If you are using WebDriverManager, no manual setup is required.
If you're setting the path manually, ensure the following line is included in your code:
"System.setProperty("webdriver.chrome.driver", "/path/to/chromedriver");"
Implement the Selenium WebDriver Script
-->Create a new Java class (e.g., FitPeoAutomation).
Run the Selenium Script
-->Option 1: Run in an IDE
Open your project in the IDE.
Right-click the Java file (e.g., FitPeoAutomation.java).
Select "Run" to execute the script.
The script should open a Chrome browser, perform the specified steps, and close the browser once done.
Option 2: Run via Command Line (Non-Maven Project)
If you're not using Maven, follow these steps:
Compile the Java file:
Open the command prompt or terminal.
Navigate to the directory containing your FitPeoAutomation.java file.
Compile the Java file using the following command:
"javac -cp .:selenium-java-4.x.x.jar:webdrivermanager-5.x.x.jar FitPeoAutomation.java"
Run the Java file:
Run the compiled Java class:
"java -cp .:selenium-java-4.x.x.jar:webdrivermanager-5.x.x.jar FitPeoAutomation"
--> Verifying the Script's Success
Step 1: The script should open the FitPeo Homepage and navigate to the Revenue Calculator page.
Step 2: It will scroll to the slider section and adjust the slider to 820.
Step 3: The script will update the text field to 560 and ensure the slider moves accordingly.
Step 4: It will select the required CPT codes and check if they are selected.
Step 5: Finally, it will verify if the Total Recurring Reimbursement value is displayed as $110700.


