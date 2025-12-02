# Ex02 Django ORM Web Application
# Date:28.08.2025
# AIM
To develop a Django application to store and retrieve data from a bank loan database using Object Relational Mapping(ORM).

# ENTITY RELATIONSHIP DIAGRAM
![WhatsApp Image 2024-12-13 at 09 31 03_361b8c4e](https://github.com/user-attachments/assets/47579f68-a135-49b9-9971-e150e3e13d8e)

## DESIGN STEPS
## STEP 1:
Create a New Django Project
## STEP 2:
Create a New Django App
## STEP 3:
Define Models for the Bank Loan Database
## STEP 4:
Register Models in Django Admin
## STEP 5:
Apply Migrations and Enter Data
## STEP 6:
Develop Views and Templates to Display Data

# PROGRAM:

```
model.py
from django.db import models
from django.contrib import admin

class Movie(models.Model):
    title = models.CharField(max_length=50)
    director = models.CharField(max_length=50)
    release_date = models.DateField()
    genre = models.CharField(max_length=30)
    rating = models.FloatField(default=0.0)

class MovieAdmin(admin.ModelAdmin):
    list_display = ('title', 'director', 'release_date', 'genre', 'rating')

admin.py
from django.contrib import admin
from .models import Movie, MovieAdmin

admin.site.register(Movie, MovieAdmin)


```
# OUTPUT:


<img width="1071" height="587" alt="image" src="https://github.com/user-attachments/assets/069f3343-6eb1-4e7d-9552-47ef21bf6246" />


![Screenshot_2024-11-20_162048 1](https://github.com/user-attachments/assets/29b647d1-f301-4297-8c10-d94e5d258f8a)



# RESULT
Thus the program for creating a database using ORM hass been executed successfully
