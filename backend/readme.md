## Backend APIs:

### Signup:
```
curl --location --request POST 'http://127.0.0.1:8000/customers/signup' \
--header 'Content-Type: application/json' \
--data-raw '{
    "cust_email": "demo@gmail.com",
    "password": "111",
    "name": "abc",
    "address": "abc",
    "age": "30",
    "pincode": 44444,
    "phone_number" : "1234567890",
    "emergency_contact1" : "1234567899",
    "emergency_contact2" : "1234567898"
}'
```

### Login:
```
curl --location --request POST 'http://127.0.0.1:8000/customers/login' \
--header 'Content-Type: application/json' \
--data-raw '{
    "cust_email": "demo@gmail.com",
    "password": "111"
}'
```

### Send SMS:
```
curl --location --request POST 'http://127.0.0.1:8000/customers/send-sms' \
--header 'Content-Type: application/json' \
--data-raw '{
    "cust_email": "demo@gmail.com"
}'
```