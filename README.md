# Stock Viewer

## Overview 

The Stock Viewer application is a versatile tool designed to provide users with
comprehensive insights into stock market data. Developed with JavaFX, this application
offers a user-friendly interface for accessing real-time and historical stock information,
facilitating informed investment decisions and market analysis.


**Technologies & IDE Used:**
- JavaFx
- Java
- MySQL
- Eclipse

**Requirements**

- **Operating System:** Compatible with Windows 10, macOS, or Linux distributions.
- **Java Development Kit (JDK):** Version 17 or higher installed on the system.
- **JavaFX:** JavaFX libraries and runtime environment integrated with the IDE for building and running JavaFX applications.
- **Database:** MySQL database server for storing and retrieving stock market data.

## Installation

1. **Download and Extract Data:**
   - **Download and Extract Libraries from the Release: Libraries for Demo and Lib** 
    
2. **JavaFX Installation and Configuration:**
   - To add the JavaFX module path to your project, follow these steps depending on the IDE you are using:
 
### **For Eclipse:**
 
- **Install JavaFX SDK:**
   - Download the JavaFX SDK from the official website: https://gluonhq.com/products/javafx/.
 
- **Add JavaFX to the Build Path:**
   - Right-click on your project in the Project Explorer.
   - Go to **preferences > java > Build Path > User Libraries>**
   - Create New Library javafx_17 and add jar files from Navigate to the `lib` directory of the unzipped JavaFX SDK (e.g., `C:\javafx-sdk-17\lib`) and select all the JAR files.
 
3. **Import Project to IDE**
    - File -> Import projects from File System -> Browse and Select the extracted Demo and Stock folder -> Finish.
    - Right click on Stock -> Build path -> Configure Build Path -> Remove the jar files from the Class path and Add the jar from StockLib folder to Class path.
    - Right click on Demo -> Build path -> Configure Build Path -> Remove the jar files from the Class path and Module path and Add the libraries from DemoLib folder.

## Run the Project

1. **Configure Project Dependencies:**

    - Right-click on the Demo project.
    - Go to Build Path > Configure Build Path > Projects.
    - Click on Add and select the Stock project to add it as a dependency to the Demo project.

2. **Run the StockRunner.java:**

    - First, run the StockRunner.java file from the Stock project.
    - For a smoother experience, set the date parameter in DDMMYYYY format:
      - Right-click on the Stock project.
      - Go to Run As > Run Configurations.
      - In the Params tab, set the date parameter and click Run.
      - After the first run, remove the date parameter from the Parms tab(If you need data of any particular date specify date and run it).

3. **Run the Main.java:**

    - Finally, run the Main.java file from the Demo project(Make sure you removed the date parameter from Stock project).
