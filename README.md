# Doctor Appointment System
A doctor's appointment system is a method for patients to schedule specific times to see a doctor for medical care or advice.

## Thought Process
In a standard doctor appointment system, appointment slots are established in accordance with the availability of the medical practitioners.

A doctor's availability is determined by specifying both the days of the week and the specific hours within those days.

Slots with different time durations can be systematically generated for extended periods, such as weeks, months, or even years ahead, aligning with the doctor's availability and patient needs.

A patient can book an appointment with a specific doctor by reserving an available time slot.

## Data Models
The doctor appointment system consists of four fundamental data models:

1. **Doctors:** This data model stores information about the doctors, including their details.

2. **Availabilities:** In this data model, the doctor's availability is recorded, specifying the days of the week and the specific hours within those days when they can accept appointments.

3. **Slots:** This data model is responsible for maintaining systematically generated slots based on the doctor's availabilities. Each slot can have a status of either 'available' or 'booked'.

4. **Appointments:** Here, records of all appointments made by patients are kept, including details about the appointment date and time, the patient, and the doctor involved.


## Technologies
| Name                    | Version |
| ----------------------- | --------|
| Ruby                    | 3.1.2   |
| Bundler                 | 2.4.6   |
| Rails API               | 7.0.8   |
| Active Model Serializer | 0.10.13 |
| Mysql                   | 8.0     |
| Swagger                 | 2.10.1  |
| Rspec                   | 6.0.3   |


## Development
### 1. Initial Setup
--------------------

Clone the project repo

    git clone https://github.com/maatif-us/doctor-appointment-system.git

Get into the project directory

    cd doctor-appointment-system

Install gems

    bundle install

Copy the environment variables example file

    cp config/application.example.yml config/application.yml

Database Setup

    bundle exec rails db:create db:migrate db:seed

Run Server

    bundle exec rails s
    
The application server is running on http://localhost:3000


### 3. Unit Testing
-------------------
Run the Unit tests

    bundle exec rspec

### 4. API Testing and Documentation
------------------------------------
Swagger is used to maintain the API documentation and endpoint testing.

Open Swagger UI

    http://localhost:3000/api-docs

Play with the API endpoints and have fun.

<img width="965" alt="swagger" src="https://github.com/maatif-us/doctor-appointment-system/assets/125513388/d33aa9b8-f6f2-4cab-a9e4-36446d91eb49">
