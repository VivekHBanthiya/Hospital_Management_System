# Hospital Management System

Welcome to the Hospital Management System repository! This system is designed to help hospitals manage patient records, doctor information, and appointment bookings efficiently. The application is built using Java and MySQL for database management.

## Features

1. **Add New Patients:**
   - Users can add new patient records to the system, including details such as name, age, and gender.

2. **View Patients List:**
   - The system provides a comprehensive list of all patients, allowing easy access to their information.

3. **View Doctors:**
   - Users can view a list of doctors along with their specializations. Note that only the database administrator can add new doctors.

4. **Book Appointment:**
   - Patients can book appointments with available doctors, and the system records the appointment details, including patient and doctor IDs and appointment date.

## Getting Started

### Prerequisites

Before using the application, make sure you have the following installed:

- Java Runtime Environment (JRE)
- MySQL Server

### Setup

1. Clone the repository to your local machine:

   ```bash
   https://github.com/VivekHBanthiya/Hospital_Management_System.git
   ```

2. Download the MySQL JDBC Driver JAR file and add it to your project's classpath. You can find the JAR file [here](https://dev.mysql.com/downloads/connector/j/).

3. Set up the MySQL database:
   - Create a database named `hospital`.
   - Create the following tables:

     - **Patients:**
       - Attributes: `id` (Primary Key), `name`, `age`, `gender`

     - **Doctors:**
       - Attributes: `id` (Primary Key), `name`, `specialization`

     - **Appointments:**
       - Attributes: `id` (Primary Key), `patient_id` (Foreign Key to `patients.id`), `doctor_id` (Foreign Key to `doctors.id`), `appointment_date`


**Note:**
- Ensure that you have added at least one doctor to the database before using the system. Only the database administrator can add new doctors.

## Contributors

- [Vivek Banthiya]([https://github.com/VivekHBanthiya])

Feel free to contribute to the project by opening issues or creating pull requests.

Thank you for using the Hospital Management System! If you encounter any issues or have suggestions, please let us know.
