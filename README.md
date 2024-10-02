# Ex02 Django ORM Web Application
## Date: 18/09/24

## AIM
To develop a Django application to store and retrieve data from a bank loan database using Object Relational Mapping(ORM).

## ENTITY RELATIONSHIP DIAGRAM

![image](https://github.com/user-attachments/assets/80559042-1cd0-4ff8-a6c1-3b9efe697f33)


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
admin.py
from django.contrib import admin
from .models import Bankloan,BankloanAdmin
admin.site.register(Bankloan,BankloanAdmin)

model.py
from django.db import models
from django.contrib import admin
class Bankloan(models.Model):
    Name=models.CharField(max_length=50);
    Gender=models.CharField(max_length=10);
    Token_no=models.IntegerField(primary_key=True);
    Amount=models.IntegerField();
    Phone=models.IntegerField();


class BankloanAdmin(admin.ModelAdmin):
    list_display=('Name','Gender','Token_no','Amount','Phone')

```

## OUTPUT

Include the screenshot of your admin page.
![image](https://github.com/user-attachments/assets/8e60d0c7-5634-48b8-bb2b-2022191a5bca)



## RESULT
Thus the program for creating a database using ORM hass been executed successfully
