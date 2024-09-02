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

- *Operating System:* Compatible with Windows 10, macOS, or Linux distributions.
- *Java Development Kit (JDK):* Version 17 or higher installed on the system.
- *JavaFX:* JavaFX libraries and runtime environment integrated with the IDE for building and running JavaFX applications.
- *Database:* MySQL database server for storing and retrieving stock market data.

## Installation

1. **Download and Extract Data:**
    
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

1. First run the StocksRunner.java from the Stock project.
   - For smoother experience before running it set the date parameter in DDMMYYYY format once.
     ->Right click on Stock -> Run As -> Run Configurations -> In Params tab, Set parameter and click on Run.
   - Now remove the date parameter and run it once again.

2. In MySQL
   - Create a Database and tables, Copy the below queries.
    ```sql
    Create database userdetails
    ```
   - In userdetails database, create credentials and feedback tables.
     ```sql
     Create table credentials( uid int auto_increment not null, name varchar(10), password varchar(20), phone varchar(20), PRIMARY KEY(uid));
     ```
     ```sql
     Create table feedback(name varchar(10),email varchar(50), phone varchar(20), comments varchar(255));
     ```

3. Now run the Main.java from Demo. Register user before login.
