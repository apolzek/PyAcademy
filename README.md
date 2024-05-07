# PyAcademy - Mastering ELK with Python

[Mastering ELK with Python -PyAcademy](https://medium.com/@ashishmj/mastering-elk-with-python-18ab455e8e05) A simple project for searching courses/blogs and integrating the application with ELK stack
[Medium blog](https://medium.com/@ashishmj/mastering-elk-with-python-18ab455e8e05)

## About this repository

This repository contains the code for PyAcademy - Mastering ELK with Python

```bash
bin/elasticsearch-reset-password -u elastic
bin/logstash -f /home/apolzek/Workdir/github.com/apolzek/PyAcademy/logstash/logstash-simple.conf
bin/kibana
```

Update password on logstash-simple.conf file
Use elasticsearch token to configure kibana

```bash
python3 -m venv venv
source venv/bin/activate
pip3 install -r requirements.txt
```

http://127.0.0.1:5000/pyacademy/home

```bash
curl -H 'Content-Type: application/json' -d '{ "courseName":"Implementing gRPC In Python","courseId":"CR0013", "url" : "https://ashishmj.medium.com/implementing-grpc-in-python-51dd6be87ec3" , "duration": 70 ,"author": "Ashish MJ" ,"description" : "Course aims to outline the basics of gRPC and create a simple project by building endpoints using gRPC"}' -X POST http://localhost:5000/pyacademy/courses

curl -H 'Content-Type: application/json' -d '{ "courseName":"REST APIs in Go using Gorilla Mux","courseId":"CR0012", "url" : "https://blog.devgenius.io/rest-apis-in-go-using-gorilla-mux-01fab932c5a0" , "duration": 30 ,"author": "Ashish MJ" ,"description" : "Course aims to outline the basics of REST architecture and create a simple project by building REST APIs using Gorilla mux"}' -X POST http://localhost:5000/pyacademy/courses

curl -H 'Content-Type: application/json' -d '{ "courseName":"Build Microservices with Python","courseId":"CR0011", "url" : "https://blog.devgenius.io/build-microservices-with-python-63fd35fa3baa" , "duration": 90 ,"author": "Ashish MJ" ,"description" : "Course aims to outline the basics of Microservices based architecture and learn how to build microservices with Python"}' -X POST http://localhost:5000/pyacademy/courses

curl -H 'Content-Type: application/json' -d '{ "courseName":"Implement CI / CD using Jenkins for Python Application","courseId":"CR0010", "url" : "https://blog.devgenius.io/implement-ci-cd-using-jenkins-for-python-application-91a3bcf7d91" , "duration": 45 ,"author": "Ashish MJ" ,"description" : "Course aims to outline the basics of Jenkins and learn how to implement Continuous Integration / Continuous Delivery using Jenkins for a Python application"}' -X POST http://localhost:5000/pyacademy/courses
```