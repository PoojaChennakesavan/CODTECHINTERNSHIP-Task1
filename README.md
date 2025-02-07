Name: POOJA KC      
Company: CODTECH IT SOLUTIONS    
Id: CT12DS3006           
Domain: Python Programming                    
Duration: December,2024 to February,2025            
Mentor:NEELA SANTOSH KUMAR           

OVERVIEW OF THE PROJECT

PROJECT: STUDENT GRADE TRACKER SYSTEM

1. PROJECT DESCRIPTION:                 
The Student Grade Tracker is a Python-based application designed to help teachers or educators manage student grades efficiently. It allows users to:            
- Add and manage student information.            
- Input and track grades for various assessments (quizzes, midterms, finals, participation).                 
- Calculate final grades based on weighted scores.                       
- Display class averages and individual student grades.                 
- Visualize grade distributions using graphs.                      

The application is built using Tkinter for the graphical user interface (GUI) and **matplotlib** for data visualization. It also uses **pickle** for saving and loading class data.                

2. KEY FEATURES:            
The project includes the following features:           

2.1.Student management:          
- Add new students to a class.           
- Remove students from a class.           
- View a list of all students in a class.           

2.2.Grade Management:            
- Add grades for individual students or the entire class.           
- Input grades for quizzes, midterms, finals, and participation.            
- Automatically calculate final grades based on predefined weights:              
  - Quizzes: 25%               
  - Midterm: 30%                
  - Final Exam: 30%                 
  - Participation: 15%                  

2.3.Grade Visualization:             
- Display class averages for each assessment.              
- Visualize grade distributions using bar charts (via **matplotlib**).            

2.4.Data Persistence:               
- Save class data (student information and grades) to files using **pickle**.            
- Load saved class data when reopening the application.                 

Error Handling:    
- Validate user inputs (e.g., ensure grades are numeric and within the valid range).      
- Display error messages for invalid inputs or missing data.    

3. TECHNOLOGIES USED:        
The project leverages the following technologies and libraries:    

  Core Python: The application is written in **Python**, making it easy to understand and extend.    
  Tkinter:   
    - Used foR building the **graphical user interface (GUI)**.      
    - Provides widgets like buttons, labels, entry fields, and listboxes for user interaction.      
  Matplotlib:         
    - Used for **data visualization**.          
    - Generates bar charts to display grade distributions.        
  Pickle:      
    - Used for **data persistence**.        
    - Saves and loads class data (student information and grades) to/from files.         
  File Handling:    
    - Reads and writes to text files (e.g., `Classes` file) to manage class names.      

4. PROJECT STRUCTURE:        
The project is organized into several classes, each handling a specific functionality:        

4.1.Main Classes:     
 App:     
   - The main application window.     
   - Allows users to select a class or add a new class.        

Load:        
   - Handles loading and managing a specific class.     
   - Provides options to view students, add/remove students, and open student/class views.        

StudentPane:       
   - Manages individual student grades.                 
   - Allows users to add grades, calculate final grades, and view grade details.             

ClassPane:        
   - Manages class-wide operations.                
   - Displays class averages and allows adding grades for all students.              

Student:            
   - Represents a student object.              
   - Stores student information (name) and grades for quizzes, midterms, finals, and participation.                 

Helper Classes:        
- **`AddAClass`**: Handles adding a new class and its students.             
- **`AddStudents`**: Allows users to input student names for a new class.                
- **`DisplayGrade`**: Displays grades for a specific student.               
- **`CalculateGrade`**: Calculates and displays the final grade for a student.                  
- **`AddOneGrade`**: Allows users to add a single grade for a student.                      
- **`AddAllGrades`**: Allows users to add grades for all assessments for a student.                       
- **`FinishGrade`**: Ensures all missing grades for a student are filled.                   
- **`DisplayClassGrades`**: Displays class averages and allows visualization of grade distributions.                  
- **`ClassGraphAverage`**: Generates bar charts for grade distributions.                          

5.WORKFLOW:       
1. **Start the Application**:     
   - The user launches the application and sees a list of available classes.            

2. **Add a New Class**:                
   - The user can add a new class by specifying the class name and the number of students.                      
   - The user then inputs the names of the students.                  

3. **Manage Grades**:                    
   - The user selects a class and can:                 
     - Add grades for individual students or the entire class.                      
     - View and calculate final grades.                         
     - Display class averages and visualize grade distributions.                          

4. **Save and Load Data**:                
   - Class data is saved automatically using **pickle**.                     
   - The user can reload saved data when reopening the application.                     

6. CHALLENGES AND SOLUTIONS:       
#### **Challenges**            
1. **Data Persistence**:                   
   - Storing and retrieving student and grade data efficiently.              
2. **Input Validation**:                   
   - Ensuring users enter valid grades (numeric values between 0 and 100).                
3. **User Interface**:                
   - Designing an intuitive and user-friendly GUI.              

#### **Solutions**              
1. **Data Persistence**:                         
   - Used **pickle** to serialize and save class data to files.                 
2. **Input Validation**:                 
   - Added checks to ensure grades are numeric and within the valid range.                      
3. **User Interface**:                  
   - Used **Tkinter** to create a simple and functional GUI.                     
