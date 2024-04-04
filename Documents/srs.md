# JOB HOSTING PLATFORM APP

## Overview
The GIUP is a web application designed to connect employers with individuals seeking temporary/contract work. It offers a seamless experience for job posting, applicant tracking, and hiring processes.

The Name 'GIUP': in Vietnamese, giúp means help, and that is the spirit of the app, is to assist business to find staff and worker to find work.

Similar to: Seek (job hosting) and Uber (operating system)


## Business Use Case
Why focus on temporary work? the seasonal demand in hospitality and event industry


## Benefit
-For employer: managing cost and time (no need for long hiring process and managing employees), improve staff quality and retention (staff are screened by the app)
-For employee:  extra  income (easily find work in free time)



## Features

### Employer Features

1. **User Registration and Authentication:**
   - Employers can securely register and authenticate their accounts.

2. **Job Posting:**
   - Employers can post temporary/contract job listings with details such as title, description, location, duration, required skills, and compensation. Through this process, the app will save the username to the database so later when check if they can edit the page, the app will compare with the username in local storage, if matches then the user will have admin/ employer access

3. **Applicant Tracking:**
   - Tools for employers to track and manage job applicants efficiently- accept/reject applicants

4. **Job Management:**
   - Employers can edit (open/close job status), or delete job postings

### Job Seeker Features
can GET list of users, job listings and applicants,
POST new users, jobs, and apply for the job,
use PUT to update user, job status and reject/accept applicants

1. **User Registration and Authentication:**
   - Job seekers can securely register and authenticate their accounts.

2. **Job Search:**
   - Job seekers can search for temporary/contract job listings based on various criteria.

3. **Application Submission:**
   - Job seekers can submit applications for desired positions.

4. **Application Tracking:**
   - Job seekers can track the status of their applications.


### Flow
Admin:
Sign Up -> Log In -> Post Job -> Accept/Reject Applicants -> Close The Job -> Rate Employee -> Pay the app 

User:
Sign Up -> Log In -> Apply Job -> Work if got accepted -> Rate Employer -> Get payment from the app

## Non-Functional Requirements

1. **Security:**
   - Generate token after logged in to check if the user is logged in on certain pages
   - Username is saved in local storage when logged in to authorize user for certain tasks

2. **Performance:**
   - Optimize platform performance for fast loading times
   - Optimize for small/ large screen size
   - Intuitive and user-friendly interface

## Technical Requirements

1. **Technology Stack:**
   - Frontend: React.js
   - Backend: Node.js

2. **Hosting and Infrastructure:**
   - Not yet implemented

3. **API Integration:**
   - mock-up user data: https://jsonplaceholder.typicode.com/users
   - internal API

4. **Libraries:**
   - Back End: Axios (fetch data), Mongoose (MongoDB object modeling tool), cors (cross origin request), jsonwebtoken (generate token for authentication)

   - Front End: material UI, framer-motion (animations), react-fast-marquee (review marquee), react-router-dom (routes), react-type-animation (animated sentence), 


## Data
   - Database: MongoDB
User, Job, Application (for admin and user)




## Future Implementation
 - Notification system 
 - Profile management
 - oauth (fb, google)
 - messaging feature (communication between employer and applicants)
 - Rating system (after the job finished)
 - payment plans 
 - update security 
 - filtering system for job (by date, by rate,...)


## Conclusion

The Job Hosting Platform App GIUP aims to provide a comprehensive solution for temporary/contract work, meeting the needs of both employers and job seekers. By implementing the specified features and adhering to the outlined requirements, the platform offers a seamless and efficient experience for job posting, applicant tracking, and hiring processes.
