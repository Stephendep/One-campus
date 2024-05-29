# One Campus Project by Nwankpa Stephen

## Project Scenario

Jerome is a teacher at Grand Rapids High School. Due to a shortage of teachers willing to accept in-person teaching positions during the Covid era, Jerome has had to teach Math, Chemistry, Biology, and Physics to the 8th grade students. This project aims to automate the process of recording student scores, computing performance metrics, and querying student performance data.

## Student Information

The following are the students and their identity codes:

| Student Name       | ID      |
|--------------------|---------|
| Bett James         | GR-0483 |
| Namukolo Abrams    | GR-0484 |
| Vera Abutu         | GR-0485 |
| Kwame Doga         | GR-0486 |
| Lukeman Ahmad      | GR-0487 |
| Akin Torey         | GR-0488 |
| Luke Brant         | GR-0489 |
| James Kenyata      | GR-0490 |
| Ngugi Tionga       | GR-0491 |
| Okoro Eze          | GR-0492 |
| Agatha Chiluba     | GR-0493 |
| Mangu Joseph       | GR-0494 |
| Longe Jethro       | GR-0495 |
| Florence Giwa      | GR-0496 |
| Vetiva Lucent      | GR-0497 |
| Melody Braimoh     | GR-0498 |
| Victor Ihab        | GR-0499 |
| Mimi Trucker       | GR-0500 |
| Maguel Peter       | GR-0501 |
| Wellington Zuba    | GR-0502 |

## Project Capabilities

### Script Features

1. **Manual Input of Scores**
   - Enables manual loading of each student's scores by subject for quizzes, homework, attendance, and exams using the Python `input()` function.

2. **Automatic Computation**
   - Computes the Average Score, GPA (0 to 5.0), Grade, and Status (Pass, Fail, Retake) and stores them in a container for each student.

3. **Performance Records**
   - Holds each student's performance records in a container.
   - Holds each subject's performance records in a container for all students.
   - Holds all student performance records for all subjects in a container. This container includes scores for quizzes, homework, exams, Average Score, GPA, Grade, and Status.

### Script Utility

The script provides functionalities to query the performance data:

1. **Full Performance Records**
   - Fetches the full performance records of any student by providing the student's name or ID.

2. **Subject Performance Records**
   - Fetches a student's performance for any given subject by providing the student's name/ID and the subject name.

3. **Grade Categories**
   - Fetches the list of students in any of the grade categories (A, B, C, D, E, F).

4. **Student Status**
   - Fetches the list of students' statuses (Pass, Fail, Retake).

5. **Pass/Fail/Retake Determination**
   - Determines if a student passed, failed, or needs to retake a subject.

## Usage

1. Clone the repository.
2. Run the script and follow the prompts to input the scores.
3. Use the provided functions to query the performance data.

## Example

```python
# Example usage:
students["GR-0483"].input_scores()  # Input scores for a specific student
students["GR-0483"].compute_performance()  # Compute performance for the student

print(query_student_performance("GR-0483"))  # Query the performance of a student
print(query_student_subject_performance("GR-0483", "Math"))  # Query the performance of a student in a specific subject
print(query_students_by_grade('A'))  # Get list of students with grade A
print(query_students_by_status('Pass'))  # Get list of students with status Pass
