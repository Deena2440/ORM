## Ex02 Django ORM Web Application
## Date:31/02/2030
## AIM
To develop a Django application to store and retrieve data from a bank loan database using Object Relational Mapping(ORM).

## ENTITY RELATIONSHIP DIAGRAM

![image](https://github.com/user-attachments/assets/73f88e27-5f5b-4171-8e31-1b0df7977603)

## DESIGN STEPS
## STEP 1:
Clone the problem from GitHub

## STEP 2:
Create a new app in Django project

## STEP 3:
Enter the code for admin.py and models.py

## STEP 4:
Execute Django admin and create details for 10 books

## PROGRAM
models.py

from django.db import models from django.contrib import admin class Bank_loan (models.Model): customer_id=models.IntegerField(primary_key=True) customer_name=models.CharField(max_length=100) loan_amount=models.IntegerField() customer_age=models.IntegerField() email=models.EmailField()

class Bank_loanAdmin(admin.ModelAdmin): list_display=('customer_id','customer_name','loan_amount','customer_age','email')

admin.py

from django.contrib import admin from .models import Bank_loan,Bank_loanAdmin admin.site.register(Bank_loan,Bank_loanAdmin)

## OUTPUT
![image](https://github.com/user-attachments/assets/81a60cad-aa4f-40f9-a8f6-dcd64d96ba11)
![image](https://github.com/user-attachments/assets/6d241abe-906b-4885-ac74-4f0cc4124b72)
## RESULT
Thus the program for creating a database using ORM hass been executed successfully
