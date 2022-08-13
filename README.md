# assign-mentor
Assigning mentor and students RESTAPI  build with NodeJs, Express and MongoDB. 

Live URL-(https://assign-mentor-rp.herokuapp.com/)

## Create mentor.
POST - /create-mentor <br />
Request body - <br />{
    "name": "Joe",
    "Students": []
}

## Create student.
POST - /create-student <br />
Request body - <br />{
    "name": "Rajesh"
}

## Adds mentor name to students who don't have mentors assigned.
PUT - /update-mentor/:mentorName  eg. /update-mentor/Joe <br />
Request body - <br /> {
    "Students": ["Rajesh","Roman"]
}

##  Update mentor for a particular student.
PUT - /update-student-mentor/:studentName eg. /update-student-mentor/Rajesh <br />
Request body - <br /> {
    "mentor": "Brad"
}

## Get students assign to particular mentor.
GET - /studentlist/:mentor  eg ./studentlist/Brad <br />

## Get Students.
GET - /student

## Get Mentors.
GET - /mentor
