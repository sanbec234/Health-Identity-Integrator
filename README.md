# Health Identity Integrator (HID)
This Java Swing executable .jar file can retrieve useful information from database and display if the user is eligible for proceeding an application for a job.

This project is a simple Java Swing application that helps assess a candidate's health information for either a Driving License or Army eligibility. It interacts with other classes (`porg` and `army`) to perform checks based on the user's input (Aadhaar number).

## Features

- **Graphical User Interface (GUI)**: Built using Java Swing for an interactive experience.
- **User Input**: Allows users to enter the first 6 digits of their Aadhaar number for eligibility checking.
- **Driving License and Army**: Offers two separate categories for assessing the candidate's eligibility.
- **Exit Confirmation**: Prompts the user before exiting the application.
  

## Requirements

- Java Development Kit (JDK) 8 or higher
- Java Swing (included in the JDK)
- Any Java IDE (Eclipse, IntelliJ IDEA, etc.) or command-line tools for running the program

## How to Run

1. **Clone or Download the Repository**:
    ```bash
    git clone https://github.com/your-username/health-identity-integrator.git
    cd health-identity-integrator
    ```

2. **Compile the Java Files**:
    You can compile the Java files using the following command or through your IDE:
    ```bash
    javac -d bin src/HID/GUI.java src/HID/porg.java src/HID/army.java
    ```

3. **Run the Application**:
    After compiling, you can run the program using the following command:
    ```bash
    java HID.GUI
    ```

4. **Application Flow**:
    - On launching, the user is greeted with a welcome message and a "continue" button.
    - The user selects either "Driving License" or "Army" for the category.
    - The user enters the first six digits of their Aadhaar number.
    - Based on the category and Aadhaar number, the program calls either `porg.main()` for Driving License or `army.main()` for Army eligibility checks.

## Usage

1. Launch the application.
2. Select either **Driving License** or **Army** from the menu.
3. Enter the first six digits of your Aadhaar number.
4. The app will call the respective classes (`porg` or `army`) to determine eligibility based on the provided Aadhaar number.

## GUI Flow

1. **Main Menu**:
    - Displays a welcome message with a "continue" button.
2. **Category Selection**:
    - The user chooses between **Driving License** and **Army**.
3. **Driving License/Army Section**:
    - The user inputs the first six digits of their Aadhaar number.
    - The program performs eligibility checks by calling external classes (`porg` for Driving License, `army` for Army).

## Dependencies

- **Java Swing**: For the GUI components such as JFrame, JPanel, JButton, etc.
- **javax.swing.JOptionPane**: For user confirmation dialogs.
- **External Classes**: 
  - `porg`: Handles driving license eligibility.
  - `army`: Handles army eligibility.

## Contribution

If you'd like to contribute to this project, feel free to fork the repository, make your changes, and submit a pull request. All contributions are welcome!

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.
