Student Mentor Assignment APIs

* STUDENTS
* To Create a new student (Task: API to create a new student)
    - POST method: http://localhost:3010/student/create
    - Payload : { "id": 1, "name": "Studentname", "DOB": "dd-mm-yyyy", "email": email@gmail.com", "phone: ": "90000XXXXX", "location": "cityname","batch": "BXXWD", "course": "Full Stack Development" }

* Update a existing student details
    - PUT method: POST method: http://localhost:3010/student/update/1
    - Payload: { "name": "studentname edited"}

* To Get all students details listed
    - GET method: GET method: http://localhost:3010/student/all

* To Delete a particular student from the list
    - DELETE method: http://localhost:3010/student/delete/1

* MENTORS
* To Create a new mentor (Task: API to create a new mentor)
    - POST method: http://localhost:3010/mentor/create
    - Payload : { "id": 1, "name": "mentorname", "age": "00", email: "mentorname@email.com", "phone": "78788XXXXX", "location": "city", "batch": "BXXWD", "specialization": [], "student":[]}

* Update a particular mentor existing details
    - PUT method: http://localhost:3010/mentor/update/1
    - Payload : { "location": "citynewname" }

* To Get all mentor details listed
    - GET method: http://localhost:3010/mentor/all

* To Delete a particular mentor from the list
    - DELETE method: http://localhost:3010/mentor/delete/1

* API to Assign a Student to a Mentor
    - Select one mentor and add multiple students
    - A student who has a mentor should not be shown in the list
    - PUT method: http://localhost:3010/mentor/updateMentor/1
    - Payload : { "student": [2,5,6]} //2,5,6 are id's of students

* API to assign or change a mentor for a particular student
    - Select one student and assign one mentor
    - PUT method: http://localhost:3010/mentor/assign/1 (this will assign student 1 to mentor 1)
    - Payload : { "mentorId": 1}

* API to show all students for a particular Mentor
    - GET method: http://localhost:3010/mentor/get/1