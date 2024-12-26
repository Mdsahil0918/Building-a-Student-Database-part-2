# My Computer Science Students - Bash and SQL Script

This project contains a Bash script designed to query a PostgreSQL database named `students` and retrieve various insights about computer science students and their courses. The script showcases how Bash and SQL can be combined to extract and format data dynamically.

---

## Features

The script performs the following tasks:

1. **List of Top Students:**

   - Retrieves the first name, last name, and GPA of students with a perfect 4.0 GPA.

2. **Courses Alphabetically Before 'D':**

   - Lists all course names where the first letter is alphabetically before 'D'.

3. **Filtered Students by Last Name and GPA:**

   - Fetches students whose last name begins with 'R' or later in the alphabet and have a GPA either greater than 3.8 or less than 2.0.

4. **Search by Last Name Criteria:**

   - Finds students whose last names contain a case-insensitive "sa" or have 'r' as the second-to-last letter.

5. **Unassigned Majors with Specific Criteria:**

   - Retrieves students without a major whose first name starts with 'D' or have a GPA greater than 3.0.

6. **Courses Meeting Specific Patterns:**

   - Lists the first five courses in reverse alphabetical order with an 'e' as the second letter or ending in 's'.

7. **Average GPA:**

   - Calculates the average GPA of all students, rounded to two decimal places.

8. **Major Statistics:**

   - Provides the major ID, number of students in that major, and their average GPA for majors with more than one student.

9. **Unused Majors and Specific Names:**

   - Lists majors (in alphabetical order) that either have no students or include a student whose first name contains a case-insensitive "ma".

10. **Unique Courses Unenrolled by a Specific Student:**

    - Displays unique courses (in reverse alphabetical order) that no student or a specific student (`Obie Hilpert`) is taking.

11. **Courses with Single Enrollment:**

    - Lists courses (in alphabetical order) with only one student enrolled.

---

## Prerequisites

### Database Setup:

- PostgreSQL should be installed and running.
- The database `students` must be populated with the following tables:
  1. `students`: Contains details about students, including their first name, last name, GPA, and major ID.
  2. `courses`: Contains details about courses.
  3. `majors`: Contains details about majors.
  4. `majors_courses`: A join table linking majors and courses.

### User Permissions:

- The script uses the PostgreSQL user `freecodecamp` to connect to the database. Ensure this user has appropriate permissions.

---

## How to Run the Script

1. Clone the repository containing the script:
   ```bash
   git clone https://github.com/your-username/your-repo-name.git
   ```
2. Navigate to the script's directory:
   ```bash
   cd your-repo-name
   ```
3. Make the script executable:
   ```bash
   chmod +x script.sh
   ```
4. Execute the script:
   ```bash
   ./script.sh
   ```

---

## Output

The script generates the requested data directly in the terminal. Each query result is labeled for clarity.

---

## Contribution

Contributions are welcome! If you'd like to improve this script, feel free to:

1. Fork the repository.
2. Create a new branch for your feature.
3. Submit a pull request with a detailed explanation.

---

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

