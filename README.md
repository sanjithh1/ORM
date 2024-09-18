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
 ```
Name:Sanjith.R
Reg  no:212223230191
from django.db 
 import models 
 from django.contrib import admin
 Models.py
```
# Create your models here.

class Bank(models.Model): customer_id = models.IntegerField(primary_key=True) customer_name = models.CharField(max_length=50) account_type = models.CharField(max_length=50) loan_amount = models.DecimalField(max_digits=10, decimal_places=2)
monthly_interest = models.DecimalField(max_digits=5, decimal_places=2)
due_date = models.DateField()

class Loandetails(admin.ModelAdmin): list_display= ('customer_id','customer_name','account_type','loan_amount','monthly_interest','due_date')

admin.py from django.contrib import admin from .models import Bank,Loandetails


## OUTPUT

Include the screenshot of your admin page.
![image](https://github.com/user-attachments/assets/d51883a5-7a09-4906-9320-fea7f5ed281e)
![image](https://github.com/user-attachments/assets/8bd93f38-0755-4004-8e9e-c6d0f1063dec)


## RESULT
Thus the program for creating a database using ORM hass been executed successfully
