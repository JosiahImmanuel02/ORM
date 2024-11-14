# Ex02 Django ORM Web Application
## Date: 

## AIM
To develop a Django application to store and retrieve data from a bank loan database using Object Relational Mapping(ORM).

## ENTITY RELATIONSHIP DIAGRAM



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
from .models import Football_player,Football_playerAdmin
admin.site.register(Football_player,Football_playerAdmin)

models.py
from django.db import models
from django.contrib import admin
class Football_player(models.Model):
    Name=models.CharField(max_length=15)
    Age=models.IntegerField()
    DOB=models.CharField(max_length=10)
    Jerseynumber=models.IntegerField()
    Email=models.EmailField()
class Football_playerAdmin(admin.ModelAdmin):
    list_display=('Name','Age','DOB','Jerseynumber','Email')

## OUTPUT

Include the screenshot of your admin page.


## RESULT
Thus the program for creating a database using ORM hass been executed successfully
