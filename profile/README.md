<h1 align="center"> TrackIt </h1>

<div style="text-align: center">
  <img src="https://github.com/trackitward/.github/blob/main/profile/images/TrackIt%20text%20copy.png" alt="Trackit logo">
</div>

---

A web application that allows students to submit their units to teachers for them to accept or reject them

---

## Table of Contents

<details>
  <summary>Click to drop down</summary>

- [Table of Contents](#table-of-contents)
- [Teacher Side](#teacher-side)
  - [Teacher Login](#teacher-login)
  - [How to Accept Units](#how-to-accept-units)
  - [How to Reject Units](#how-to-reject-units)
- [Student Side](#student-side)
  - [Student Login](#student-login)
  - [The Unit Tracker](#the-unit-tracker)
  - [How to Generate a Unit Submission Code](#how-to-generate-a-unit-submission-code)
- [Landing Page](#landing-page)
- [Code](#code)
  - [Front End](#front-end)
  - [Back End](#back-end)

</details>

---

## Teacher Side

### Teacher Login

This page allows teachers to login:
![Teacher Login](https://github.com/trackitward/.github/blob/main/profile/images/teacher_login.png)

### How to Accept Units

### How to Reject Units

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

- Christian Fernandes
- Nolawi Teklehaimanot
- Ryan Alumkal
- Anthony Toyco
- Josh Adolfo

---

## Code

### Front End

Written in pure HTML/CSS/Javascript

- Click on the links below to go to important front-end files
  - [Unit Tracker](https://github.com/trackitward/trackit-web/blob/main/index.html)
  - [Teacher Side](https://github.com/trackitward/trackit-web/blob/main/box.html)
  - [Student Login](https://github.com/trackitward/trackit-web/blob/main/student-login.html)
  - [Student Sign up](https://github.com/trackitward/trackit-web/blob/main/student-signup.html)
  - [Landing Page](https://github.com/trackitward/trackit-web/blob/main/landing-page.html)

### Back End

The backend of the project is written in pure Golang. It provides a feature-rich HTTP API to the front-end and handles all information going through the TrackIt app. There are many safety features built-in, including rate limits to prevent the API from being attacked by large amounts of requests at a time.

- Click on the links below to go to important front-end files
  - []

---
