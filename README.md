# OTP-in-django
Quick and simple technique to implement the OTP functionality in your Django Project.

### Python Packages required: ```pyotp, base64, django, django-rest-framework```

## API Calls
```
py manage.py createsuperuser first registermobile No. 
```

#### GET 
This is to register the mobile number into the database and generate OTP.

```http://127.0.0.1:8000/verify/1234567890/```

#### POST
This is to verify the mobile number using OTP.

```http://127.0.0.1:8000/verify/1234567890/```

Data: 
```
   {
    "otp":786512
   }
```