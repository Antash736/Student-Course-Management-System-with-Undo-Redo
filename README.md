# Student-Course-Management-System-with-Undo-Redo
A Java-based Student-Course Management System with full support for add/remove operations, enrollments, sorting, and undo/redo functionality. Built using custom linked lists and stacks, the project handles edge cases like full courses, duplicate entries, and abnormal student loads. Includes 15 comprehensive test scenarios covering all operations.
🎓 Student-Course Management System with Undo/Redo

This project is a Java-based Student-Course Management System that allows adding, removing, and managing students and courses. It supports enrollment operations, sorting, validation checks, and undo/redo functionality, making it a robust tool for managing academic data structures.

🚀 Features

Student Management

Add or remove students.

Check if a student is “normal” (enrolled in 2–7 courses).

View last added student.

Course Management

Add or remove courses.

Check if a course is full (max 30 students).

View last added course.

Enrollment

Enroll students in courses.

Remove students from courses.

Prevent duplicate enrollments or exceeding course capacity.

Sorting

Sort courses for a student by course ID.

Sort students in a course by student ID.

Undo/Redo Functionality

Supports undo and redo for:

Adding/removing students.

Adding/removing courses.

Enrolling/unenrolling students.

Maintains history of actions.

Edge Case Handling

Prevents duplicate entries.

Handles empty lists gracefully.

Detects abnormal student load (>7 courses).

Ensures system consistency after undo/redo sequences.

🛠️ Technologies Used

Java (Core language)

Linked Lists (Custom implementation for students and courses)

Stacks (Custom undo/redo stack)

📂 Project Structure

Student → Manages student-related operations.

Courses → Manages course-related operations.

StackUR → Handles undo/redo functionality.

demo → Main class with sample test cases.

▶️ How to Run

Clone the repository:

git clone https://github.com/yourusername/student-course-management.git
cd student-course-management


Compile the Java program:

javac demo.java


Run the program:

java demo

📖 Example Output

The demo class includes comprehensive test cases that cover:

Adding/removing students and courses.

Enrolling/unenrolling students.

Sorting lists.

Undo/redo sequences.

Edge cases such as full courses and abnormal students.

Example section of the output:

=== 1. إضافة طلاب ومواد ===
the student with ID : 1001 was Added Successfully
The Student With ID: 1001 Was Added Before!
the Course with ID : 2001 was Added Successfully
The Course With ID : 2001 Was Added Before!

=== 2. تسجيل طالب في مادة ===
The Student With ID: 1001 Is Enrolled in The Course With ID: 2001
The Student With ID: 1001 Was Enrolled Before!
Student 999 not found
Course 999 not found

🧪 Testing

The project contains 15 test scenarios in demo.java, including:

Normal workflows.

Edge cases.

Stress tests with multiple undo/redo operations.
