# Ex02 Django ORM Web Application
## Date: 12/03/2024

## AIM
To develop a Django application to store and retrieve data from a Book database using Object Relational Mapping(ORM).

## Entity Relationship Diagram
![2](https://github.com/selvasachein/ORM/assets/151444759/c6fc4e2a-abf6-427a-9576-e285d2efbf08)

## DESIGN STEPS

### STEP 1:
Clone the problem from GitHub

### STEP 2:
Create a new app in Django project

### STEP 3:
Enter the code for admin.py and models.py

### STEP 4:
Execute Django admin and create details for 10 books

## PROGRAM
admin.py
from django.contrib import admin
from .models import student,studentAdmin
admin.site.register(student,studentAdmin)

models.py
from django.db import models
from django.contrib import admin
class student (models.Model):
    name=models.CharField(max_length=20,help_text="student")
    rollno=models.IntegerField()
    refno=models.IntegerField()
    age=models.IntegerField()
    email=models.EmailField()
class studentAdmin(admin.ModelAdmin):
    list_display=('name','rollno','refno','age','email')

## OUTPUT
![1](https://github.com/selvasachein/ORM/assets/151444759/dce88341-07cf-4bc6-92c3-fa7abbfb330d)


## RESULT
Thus the program for creating a database using ORM hass been executed successfully
