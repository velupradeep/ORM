# Ex02 Django ORM Web Application
## Date: 15.03.2024

## AIM
To develop a Django application to store and retrieve data from a Book database using Object Relational Mapping(ORM).

## ER Diagram:
![er diagram](https://github.com/velupradeep/ORM/assets/150329341/b5922871-4ebb-439b-85f8-9e93f32ef266)


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

```
admin.py

from django.contrib import admin
from .models import Book,BookAdmin
admin.site.register(Book,BookAdmin)

models.py

from django.db import models
from django.contrib import admin
class Book(models.Model):
   bookid=models.IntegerField(primary_key=True);
   bookname=models.CharField(max_length=30);
   bookprice=models.IntegerField();
   author=models.CharField(max_length=30);
   qty=models.IntegerField();
class BookAdmin(admin.ModelAdmin):
   list_display=("bookid","bookname","bookprice","author","qty");

```

## OUTPUT

![alt text](<san/Screenshot (13).png>)


## RESULT
Thus the program for creating a database using ORM hass been executed successfully
