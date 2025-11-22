# Ex02 Django ORM Web Application
## Date: 19-11-2025

## AIM
To develop a Django application to store and retrieve data from a Car Inventory Database using Object Relational Mapping(ORM).

## DESIGN STEPS

### STEP 1:
Clone the problem from GitHub

### STEP 2:
Create a new app in Django project

### STEP 3:
Enter the code for admin.py and models.py

### STEP 4:
Execute Django admin and create details for 5 Car 

## PROGRAM

```
model.py
from django.db import models
from django.contrib import admin
class Car(models.Model):
    brand = models.CharField(max_length=10)
    car_name = models.CharField(max_length=10)
    enginenum = models.IntegerField()
    release = models.DateField()

class CarAdmin(admin.ModelAdmin):
    list_display=('brand', 'car_name', 'enginenum', 'release')

admin.py
from django.contrib import admin
from.models import Car,CarAdmin
admin.site.register(Car,CarAdmin)

```


## OUTPUT
<img width="1919" height="1020" alt="Screenshot 2025-11-18 144134" src="https://github.com/user-attachments/assets/98491980-9618-4274-8ee1-f30d8066b6dc" />
<img width="1919" height="1011" alt="Screenshot 2025-11-18 144204" src="https://github.com/user-attachments/assets/6d635933-1723-47ce-9f71-c4db7fa793bb" />


## RESULT
Thus the program for creating car inventory database database using ORM hass been executed successfully
