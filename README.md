# Edusys
EduSys is a web based attendance and marks tracking system for school and colleges. Teachers can hand out information regarding
marks and attendance of student to the respective students and their parents.
This is simple to use and easy to set up. It can be extended by simply adding newer addons.

###Currently Supported Features:
  * Add Admin to manage Teachers and Class
  * Add Class
  * Add Teacher to a Class
  * Take Daily Attendance
  * Add Subjects for Class
  * Add Exam 
  * Add Marks
  * View reports - Student or Class
  * Add Principal: Who can view each Class report.


![2016-12-14 9](https://cloud.githubusercontent.com/assets/14165258/21170997/23722db2-c1ef-11e6-90cf-c46ad8c40b02.png)
----
![2016-12-14 10](https://cloud.githubusercontent.com/assets/14165258/21171006/26b8f14a-c1ef-11e6-994a-34d8b726d445.png)
----
![2016-12-14 11](https://cloud.githubusercontent.com/assets/14165258/21171009/288372de-c1ef-11e6-815c-d113582b41de.png)
----
![2016-12-14 12](https://cloud.githubusercontent.com/assets/14165258/21171011/2a8b3e36-c1ef-11e6-9d2a-f75489be25e3.png)
----


##Getting started

In order to set up edusys you will need to fulfil folowing dependencies :


  * python 2.7 or python 3.4 (Others havent been tested)
  * django 1.10 or above 


### Setting up Edusys

  1. clone the master branch
  2. go to source/EDUsys/settings.py and set up the database configurations
  Edit these as per your need or leave it as is to use sqlite.
  
  ```python
    DATABASES = {
      'default': {
          'ENGINE': 'django.db.backends.sqlite3',
          'NAME': os.path.join(BASE_DIR, 'db.sqlite3'),
      }
    }
  ```
  
  3. Create a superuser my running the command

    ```
      python manage.py createsuperuser
    ```
  
  4. Now run edusys using the server of your choice.
    
      If you want to use the development server itself :

      ```
        python manage.py runserver
      ```
  5. Login to django-admin by going to the url
  
  > www.domainorip/admin
  
  6. Create the folowing **user groups** :
  
  > * Teacher
  > * Student
  > * Principal
  > * Admin

  7. Now Add and Admin and a Pricipal.
  
  8. Then go to www.domainorip.com and Login as Admin. And use it as you need
  
  9. Enjoy :)
  
##Development

> Currently I am not working on this project anymore. Though feel free to email me if you need anything.

The project follows standard django structure.
`attendance` is the main app for the project.

Feel free to fork it and help develop it more.



