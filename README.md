# Test Data Payload 

Stripe API Integration for .NET 6 using stripe.net package
# Steps for Installtion
- Clone the repo.
- Update the SecretKey in `appsettings.json` (use your private stripe secret key here).

# Test Payload
### Test Payload for customer/add 
    {
    "email": "yoourmail@gmail.com",
    "name": "Sarmad Kamal",
    "creditCard": {
        "name": "Sarmad Kamal",
        "cardNumber": "4242424242424242",
        "expirationYear": "2024",
        "expirationMonth": "12",
        "cvc": "999"
        }
    }
### Test Payload for payment/add
    {
    "customerId": "${customer_id}",
    "receiptEmail": "yoourmail@test.com",
    "description": "Demo product for Stripe .NET API",
    "currency": "USD",
    "amount": 1000
    }
#### customer_id value come from customer/add API