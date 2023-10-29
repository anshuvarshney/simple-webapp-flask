# Simple Web Application

This is a simple web application using [Python Flask](http://flask.pocoo.org/) and [MySQL](https://www.mysql.com/) database. 
This is used in the demonstration of development of Ansible Playbooks.
  
  Below are the steps required to get this working on a base linux system.
  
  - Install all required dependencies
  - Install and Configure Web Server
  - Start Web Server
   
## 1. Install all required dependencies
  
  Python and its dependencies

    apt-get install -y python-is-python3 && apt-get install -y python3-pip

   
## 2. Install and Configure Web Server

Install Python Flask dependency

    pip install flask
    pip install flask-mysql

- Copy app.py or download it from source repository
- Configure database credentials and parameters 

## 3. Start Web Server

Start web server

    FLASK_APP=app.py flask run --host=0.0.0.0
    
## 4. Test

Open a browser and go to URL

    http://<IP>:5000                            => Welcome
    http://<IP>:5000/how%20are%20you            => I am good, how about you?
![Screenshot from 2023-10-28 22-10-49](https://github.com/anshuvarshney/simple-webapp-flask/assets/115215127/d8ecdfe3-3b74-45dd-a35b-f95481390f47)



and 
![Screenshot from 2023-10-28 22-12-36](https://github.com/anshuvarshney/simple-webapp-flask/assets/115215127/91d220d9-d2f7-46cf-81ae-9f871bcfcc7d)
 


    
