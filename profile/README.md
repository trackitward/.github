<h1 align="center"> TrackIt </h1>

<div style="text-align: center">
  <img src="https://github.com/trackitward/.github/blob/main/profile/images/TrackIt%20text%20copy.png" alt="Trackit logo">
</div>

---

A web application that allows students to submit their units to teachers for them to accept or reject them

---

## Table of Contents

<summary>Click to drop down</summary>

- [Table of Contents](#table-of-contents)
- [Teacher Side](#teacher-side)
  - [Unit Submissions](#unit-submissions)
  - [Unit Acceptance/Rejection](#unit-acceptancerejection)
- [Student Side](#student-side)
  - [Student Login](#student-login)
  - [The Unit Tracker](#the-unit-tracker)
  - [How to Generate a Unit Submission Code](#how-to-generate-a-unit-submission-code)
- [Landing Page](#landing-page)
- [Code](#code)
  - [Front End](#front-end)
  - [Back End](#back-end)


---

## Teacher Side

### Unit Submissions

The following prompt allows teachers to input the unique code they receive from students.
![Unit Submission Empty](https://github.com/trackitward/.github/blob/main/profile/images/submission_code_empty.png)

Here is an example of a code:
![Unit Submission Full](https://github.com/trackitward/.github/blob/main/profile/images/submission_code_filled.png)


### Unit Acceptance/Rejection

After inputting the unique code received from the student, the teacher can view all the information of the submission including student name, course code, section number, unit number, and the last date the student submitted a unit. The teacher can then accept or reject the unit submission using the checkmark or cross button respectively. 
![Teacher Side Submission](https://github.com/trackitward/.github/blob/main/profile/images/teacher_side_before_submit.png)

---

## Student Side

### Student Login

When clicking "login" from the landing page, students are prompted to this page:

![Login Page](https://github.com/trackitward/.github/blob/main/profile/images/login.png)

Students can input their student number (Mary Ward student number) and password (students can choose their password) to login to Trackit.

![Student Login](https://github.com/trackitward/.github/blob/main/profile/images/login%20page%20with%20creds.png)

### The Unit Tracker

The main feature of the application, the unit tracker, is similar to the unit tracker found in the agenda. On the first column on the left, students can see the courses they are enrolled in. Each column afterwards are the units. Students can see the number of units they have completed in each course.

![Unit Tracker](https://github.com/trackitward/.github/blob/main/profile/images/unit%20tracker%20example.png)

### How to Generate a Unit Submission Code

By clicking on the course and unit of choice, students will be prompted to the following:

![Unit Submission](https://github.com/trackitward/.github/blob/main/profile/images/unit%20submission%20example.png)

This page includes all the information of the unit submission including student name, course code, section number, unit number, and last date of submission (note: last submission date is not shown for this example as no other units were submitted).

The number on the right is the submission number which should be given to the subject teacher.

The submission number expires in 2 minutes and every code is unique and random for security reasons.

---

## Landing Page

Picture of the landing page:
![Landing Page](https://github.com/trackitward/.github/blob/main/profile/images/trackit_website.png)

The "Student Login" and "Teacher Login" button on the top allows for students and teachers to log in to the application.

Founders:

- [Christian Fernandes](https://github.com/5late)
- [Nolawi Teklehaimanot](https://github.com/nolawiyonas1)
- [Ryan Alumkal](https://github.com/ryanalumkal)
- [Anthony Toyco](https://github.com/anthxnyy)
- [Josh Adolfo](https://github.com/atlysj)

---

## Code

### Front End

Written in pure HTML/CSS/Javascript. Using Javascript allowed us to create HTTP requests to our API that would be able to show the data to the users in a easy to access way.

- Click on the links below to go to important front-end files
  - [Unit Tracker](https://github.com/trackitward/trackit-web/blob/main/index.html)

    Unit tracker HTML
  - [Teacher Side](https://github.com/trackitward/trackit-web/blob/main/box.html)

    Teacher side view

  - [Student Login](https://github.com/trackitward/trackit-web/blob/main/student-login.html)

    Student login page

  - [Student Sign up](https://github.com/trackitward/trackit-web/blob/main/student-signup.html)

    Student sign up page

  - [Landing Page](https://github.com/trackitward/trackit-web/blob/main/landing-page.html)

    Trackit landing page

### Back End

The backend of the project is written in pure Golang. It provides a feature-rich HTTP API to the front-end and handles all information going through the TrackIt app. There are many safety features built-in, including rate limits to prevent the API from being attacked by large amounts of requests at a time.

- Click on the links below to go to important front-end files
  - [main.go](https://github.com/trackitward/trackit-core/blob/main/main.go)

    Control the main function of the API and route all the traffic through the correct endpoints
  - [unit-submission.go](https://github.com/trackitward/trackit-core/blob/main/unit-submission.go)

    Control the unit submission process by managing the user files

  - [auth.go](https://github.com/trackitward/trackit-core/blob/main/auth.go)

    Control authentication and logins

  - [student.go](https://github.com/trackitward/trackit-core/blob/main/student.go)

    Control student files and manage their profile and units files

  The backend stores information in JSON files saved with unique file names. The benefit to this way of doing storage is that it allows for the data to easily be written and read from the API. As well, it makes it easy to parse and pass over through the internet.

  Passwords for each user are HASHED and SALTED using a well known encryption algorithm known as bcrypt. This means that the users password is never logged in plain text, which highly increseas security as the files containing passwords have extra protection.

---
