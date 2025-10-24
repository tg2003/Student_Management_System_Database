#### ATTENDANCE PROCEDURES

1\. AttendanceByCourseSummary

Input: course CHAR(6) (course code)

Purpose: Shows attendance summary for all students in a specific course

Output: Student list with present/medical counts, percentage, and eligibility



2\. SingleStudentSummary

Input: regno CHAR(6) (student ID)

Purpose: Shows attendance summary for one student across all subjects

Output: Course-wise attendance percentage and eligibility



3\. AttendanceByStudentCourse

Input: regno CHAR(6), course CHAR(6), type CHAR(1) (T/P/A)

Purpose: Detailed attendance for one student in one course

Output: Attendance percentage and eligibility for specific student-course combination



4\. BatchAttendanceCategory

Input: None

Purpose: Categorizes entire batch into attendance groups

Output: Count of students in different attendance categories



#### MARK/GRADE PROCEDURES

5\. Final\_Marks\_Only

Input: studentID CHAR(6), courseCode CHAR(6) (both optional)

Purpose: Shows final marks and grades for students/courses

Output: Final marks and letter grades



6\. Student\_Course\_Details

Input: studentID CHAR(6), courseCode CHAR(6) (both optional)

Purpose: Detailed admin view of marks breakdown

Output: Complete mark details with weighted calculations



#### GPA PROCEDURES

7\. Calculate\_SGPA

Input: studentID CHAR(6) (optional)

Purpose: Calculates Semester GPA for students

Output: Total grade points, credits, and SGPA



8\. Calculate\_CGPA

Input: studentID CHAR(6) (optional)

Purpose: Calculates Cumulative GPA and determines class

Output: CGPA and class classification (First Class, Second Class, etc.)



#### **VIEWS**

9\. v\_mark\_weight\_temp

Purpose: Calculates weighted marks for all components

Used by: Grade view and mark procedures



10\. grade

Purpose: Final grade calculation with letter grades



11\. Student\_Grade\_Point\_View

Purpose: Converts grades to grade points for GPA calculation

Includes: Special handling for repeat courses and different grading scales





