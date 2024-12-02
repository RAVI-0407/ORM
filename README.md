# Ex02 Django ORM Web Application
# Date:27/09/2024
# AIM
To develop a Django application to store and retrieve data from a bank loan database using Object Relational Mapping(ORM).

# ENTITY RELATIONSHIP DIAGRAM
## DESIGN STEPS
## STEP 1:
Clone the problem from GitHub

## STEP 2:
Create a new app in Django project

## STEP 3:
Enter the code for admin.py and models.py

## STEP 4:
Execute Django admin and create details for 10 books

# PROGRAM
 # models.py
 ```
from django.db import models
from django.contrib import admin

class Book(models.Model):
   Name= models.CharField(max_length=100)
   Email= models.EmailField()
   Book_No= models.CharField(max_length=100)
   Book_Name= models.CharField(max_length=100)
   Address= models.CharField(max_length=255)
   Phone_No= models.CharField(max_length=15)
class BookAdmin(admin.ModelAdmin):
 list_display = ('Name','Email','Book_No','Book_Name','Address','Phone_No') 
```
 # admin.py
 ```
from django.contrib import admin
from .models import Book, BookAdmin
admin.site.register(Book, BookAdmin)
```
# OUTPUT

![Screenshot 2024-12-02 144832](https://github.com/user-attachments/assets/4d3ec80d-d5a3-42da-bd7c-9a815ea97001)

![Screenshot 2024-12-02 144842](https://github.com/user-attachments/assets/5368c94c-67f3-4d01-a940-45c73fe025e6)

![Screenshot 2024-12-02 144850](https://github.com/user-attachments/assets/9fe27528-9a01-4d3f-8102-21db9e2b1418)

# RESULT
Thus the program for creating a database using ORM hass been executed successfully
