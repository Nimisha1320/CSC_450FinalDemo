# Shopping System

## Author Information
- **Name**: Nimisha Bhoir
- **DePaul Student ID**: 2159009
- **Email ID**: nbhoir@depaul.edu

## Introduction
This project demonstrates a simple shopping system implemented in Java. It includes classes for user authentication, product management, shopping cart functionality, order processing, and a graphical user interface (GUI) using Swing.

## Requirements
- Java Development Kit (JDK) installed
- Eclipse IDE
- MySQL database server

## Setting Up the Database
1. **Create Database**:
   - Open MySQL Workbench or any MySQL client tool.
   - Execute the following SQL commands to create the database:
     ```sql
     CREATE DATABASE shopping_system;
     USE shopping_system;
     ```

2. **Create Users Table**:
   - Execute the following SQL command to create the `users` table:
     ```sql
     CREATE TABLE users (
         id INT AUTO_INCREMENT PRIMARY KEY,
         username VARCHAR(255) NOT NULL,
         password VARCHAR(255) NOT NULL
     );
     ```

3. **Insert Sample Data**:
   - Execute the following SQL commands to insert sample user data:
     ```sql
     INSERT INTO users (username, password) VALUES ('user', 'pass');
     INSERT INTO users (username, password) VALUES ('nimi', '1234');
     ```

## Running the Code in Eclipse (Mac)
1. **Clone the Repository**: 
   - Open Terminal.
   - Change the current working directory to the location where you want the cloned directory.
   - Run `git clone [repository URL]` to clone the repository.
   
2. **Open Eclipse**:
   - Open Eclipse IDE.

3. **Import the Project**:
   - In Eclipse, go to `File` > `Import`.
   - Select `Existing Projects into Workspace` under the `General` folder, and click `Next`.
   - Click `Browse` and navigate to the directory where you cloned the repository.
   - Select the project and click `Finish`.

4. **Run the Application**:
   - In Eclipse, navigate to the project structure.
   - Locate the `ShoppingSystemGUI.java` file under `src/depaul/edu` package.
   - Right-click on the file and select `Run As` > `Java Application`.
   
5. **Login**:
   - After running the application, you'll see the login interface.
   - Enter a valid username and password (e.g., username: user, password: pass).
   - Click the `Login` button.

6. **Explore and Place Order**:
   - Upon successful login, you'll see the product catalog.
   - Click the `Add to Cart` button for the desired products.
   - The selected items will be added to the cart displayed on the right.
   - Click the `Buy` button to place the order. If the payment is successful, the order will be placed, and the cart will be cleared.

7. **Logout and Exit**:
   - To exit the application, simply close the window.

## Running Unit Tests in Eclipse (Mac)
1. **Open Eclipse**:
   - Launch the Eclipse IDE on your Mac.

2. **Import the Project**:
   - If you haven't already imported the project, follow the instructions provided earlier to import the project into Eclipse.

3. **Navigate to Test Files**:
   - Locate the test files in the project structure. The test files are typically located under the `src` directory, in the same package structure as the source files.

4. **Run Unit Tests**:
   - Right-click on the test file you want to run.
   - Select `Run As` > `JUnit Test`.
   - Eclipse will execute the test cases defined in the selected file.

5. **View Test Results**:
   - After running the tests, Eclipse will display the results in the JUnit view.
   - Green bars indicate successful test cases, while red bars indicate failures.

6. **Repeat Steps for Other Test Files**:
   - Repeat steps 4-5 for each test file you want to run.

7. **Interpreting Results**:
   - If all tests pass without any failures, it indicates that the code behaves as expected.
   - If any tests fail, review the failed test cases and the corresponding code to identify and fix the issues.

## Notes
- The project includes mock implementations for user authentication, payment processing, and product management for demonstration purposes.
- Feel free to modify and extend the code according to your requirements.
