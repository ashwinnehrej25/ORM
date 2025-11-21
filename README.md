# Ex02 Django ORM Web Application
## Date: 21.11.2025
##ref no:25015594

## AIM
To develop a Django Application to store and retrieve data from a E-Commerce Website Database for Amazon or Flipkart using Object Relational Mapping(ORM).



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
~~~
admin.py

from django.contrib import admin
from .models import amazon_DB,amazon_DBAdmin
admin.site.register(amazon_DB,amazon_DBAdmin)

models.py
from django.db import models 
from django.contrib import admin
class amazon_DB (models.Model):
     Product_name=models.CharField(max_length=20)
     S_no=models.IntegerField (primary_key=True)
     Product_type=models.CharField(max_length=20)
     Price=models.CharField(max_length=20)
     Year=models.IntegerField()
class amazon_DBAdmin(admin.ModelAdmin):
     list_display=["Product_name","S_no","Product_type","Price","Year"]

     
## OUTPUT
<img width="1890" height="1001" alt="Screenshot 2025-11-21 203337" src="https://github.com/user-attachments/assets/26547a76-9de0-4aa9-9172-bc1c0e43f3f8" />
<img width="1805" height="1022" alt="Screenshot 2025-11-21 203440" src="https://github.com/user-attachments/assets/44dc7495-424b-4c59-95f2-5c908b626257" />




## RESULT
Thus the program for creating E-commerce website database using ORM hass been executed successfully
