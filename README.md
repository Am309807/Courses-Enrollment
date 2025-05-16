# Courses-Enrollment
A API using Django + JWT that allows users to:
- Enroll and log in using JWT
- View available courses
- Enroll in courses
- View the courses the user is enrolled in

Setup Instructions:
1-Clone the Projectgit clone https://github.com/Am309807/Courses-Enrollment
2-Create and Activate a Virtual Environment:
python -m venv venv
source venv/bin/activate
3-Install Dependencies:
pip install -r requirements.txt
4-Run Migrations:
python manage.py makemigrations
python manage.py migrate
5-Create Superuser:
python manage.py createsuperuser
6-Run the Development Server:
python manage.py runserver

Registration and Login:
1-For registration and login, it is done through the application interface supported by Django, where registration is done through:
http://127.0.0.1:8000/api/register/
2-and login can be done through a request:
http://127.0.0.1:8000/api/login/
3-refresh user token:
http://127.0.0.1:8000/token/refresh/

Application interface testing:
1-View all available courses:
Request type:GET  http://127.0.0.1:8000/api/courses/
2-Register for a course:
Request type:POST  http://127.0.0.1:8000/api/enroll
example:

Headers:
  Authorization: Bearer JWT_ACCESS_TOKEN
Body:
{
  "course_id": 1
}

3-View the courses the logged-in user has enrolled in:
Request type:GET http://127.0.0.1:8000/api/my-courses/

Headers:
  Authorization: Bearer JWT_ACCESS_TOKEN










’ةةةة
