LINK TO DEPLOYED APP:
https://jpfp-pc.herokuapp.com/#/

# Students and Campuses

## Getting started

1. Fork and clone this repo.
2. `npm install`.
3. `npm run start:dev`
4. name your database acme_schools_db


## Project Features:

#### Seed

- [X] sync function which sync's and seeds your database when your application starts 

### Tier 1: All Campuses and Students

- [X] Display the campuses component when the url matches `/campuses`
- [X] Display the students component when the url matches `/students`
- [X] Add a links to the navbar that can be used to navigate to the campuses view and the students view

#### Backend Requirements

- Write a `campuses` model with the following information:
  - [X] name - not empty or null
  - [X] imageUrl - string can be null 
  - [X] address - not empty or null
  - [X] description - extremely large text
- Write a `students` model with the following information:
  - [X] firstName - not empty or null
  - [X] lastName - not empty or null
  - [X] email - not empty or null; must be a valid email
  - [X] imageUrl - string can be null 
  - [X] gpa - decimal between 0.0 and 4.0
- [X] Students may be associated with at most one campus. Likewise, campuses may be associated with many students


### Tier 2: Single Student and Single Campus


- Write a component to display a single campus with the following information:
  - [X] The campus's name, image, address and description
  - [X] A list of the names of all students in that campus (or a helpful message if it doesn't have any students)
- [X] Display the appropriate campus's info when the url matches `/campuses/:campusId`
- [X] Clicking on a campus from the campuses view should navigate to show that campus

- Write a component to display a single student with the following information:
  - [X] The student's full name, email, image, and gpa
  - [X] The name of their campus (or a helpful message if they don't have one)
- [X] Display the appropriate student when the url matches `/students/:studentId`
- [X] Clicking on a student from the students view should navigate to show that student

- [X] Clicking on the name of a student in the campus view should navigate to show that student in the student view
- [X] Clicking on the name of a campus in the student view should navigate to show that campus in the campus view


### Tier 3: Adding a Campus and Adding a Student


#### Frontend

- [X] Write a component to display a form for adding a new campus that contains inputs for _at least_ the name and address.
- [X] Display this component as part of the campuses view, alongside the list of campuses
- Submitting the form with a valid name/address should:

  - [X] Make an AJAX request that causes the new campus to be persisted in the database
  - [X] Add the new campus to the list of campuses without needing to refresh the page

- [X] Write a component to display a form for adding a new student that contains inputs for _at least_ first name, last name and email
- [X] Display this component as part of the students view, alongside the list of students
- Submitting the form with a valid first name/last name/email should:
  - [X] Make an AJAX request that causes the new student to be persisted in the database
  - [X] Add the new student to the list of students without needing to refresh the page



### Tier 4: Removing a Campus and Removing a Student


#### Frontend

- [X] In the campuses view, include an `X` button next to each campus
- Clicking the `X` button should:

  - [X] Make an AJAX request that causes that campus to be removed from database
  - [X] Remove the campus from the list of campuses without needing to refresh the page

- [X] In the students view, include an `X` button next to each student
- Clicking the `X` button should:
  - [X] Make an AJAX request that causes that student to be removed from database
  - [X] Remove the student from the list of students without needing to refresh the page


### Tier 5: Updating a Campus and Updating a Student


#### Frontend

- [X] Write a component to display a form updating _at least_ a campus's name and address
- [X] Display this component as part of the campus view
- Submitting the form with valid data should:
  - [X] Make an AJAX request that causes that campus to be updated in the database
  - [X] Update the campus in the current view without needing to refresh the page
- [X] In the campus view, display an `Unregister` button next to each of its students, which removes the student from the campus (in the database as well as this view); hint: the student is still in the database but is no longer associated with the campus

- [X] Write a component to display a form updating a student
- [X] Display this component as part of the student view
- Submitting the form with valid data should:
  - [X] Make an AJAX request that causes that student to be updated in the database
  - [X] Update the student in the current view without needing to refresh the page










