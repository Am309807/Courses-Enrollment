# Courses-Enrollment
A API using Django + JWT that allows users to:
- Enroll and log in using JWT
- View available courses
- Enroll in courses
- View the courses the user is enrolled in

Setup Instructions:
1-Clone the Projectgit clone https://github.com/YourUsername/course-enrollment-api.git
2-Create and Activate a Virtual Environment:
python -m venv venv
source venv/bin/activate
3-Run Migrations:
python manage.py makemigrations
python manage.py migrate
4-Create Superuser:
python manage.py createsuperuser
5-Run the Development Server
python manage.py runserver

6-For registration and login, it is done through the application interface supported by Django, where registration is done through:
http://127.0.0.1:8000/api/register/
and login can be done through a request:
http://127.0.0.1:8000/api/login/
refresh user token:
http://127.0.0.1:8000/token/refresh/


7-Application interface testing:
-View all available courses:
Request type:GET  http://127.0.0.1:8000/api/courses/
-Register for a course:
Request type:POST  http://127.0.0.1:8000/api/enroll/
example:
Headers:
  Authorization: Bearer JWT_ACCESS_TOKEN
Body:
{
  "course_id": 1
}

-View the courses the logged-in user has enrolled in:
Request type:GET http://127.0.0.1:8000/api/my-courses/
Headers:
  Authorization: Bearer JWT_ACCESS_TOKEN










’ةةةة
