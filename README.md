# checkout-steps
This is a simple visual representation of all the steps you need to follow to implement checkout payment gateway.

Apple Pay or Google Pay:
Here are the steps for Apple/Google Pay checkout. First, you need to configure Apple/Google Pay configurations, which is required by  Flutter Pay package. This package opens a bottom sheet for you, where your cards are selectable for authentication using Face ID or fingerprint. Then, the bottom sheet returns a token to you, which you need to convert to Base64 and send to the checkout. Checkout returns a new token.  Along with your amount and channel you need to send this token to your backend.  What will the backend do? It will take all these things and request checkout again. If the response is successful, your payment will be successfully completed.

Credit card:


![image](https://github.com/rizzzvi/checkout-steps/assets/51655413/fc73e86a-caaa-4d03-9b0a-a05fe5404cad)
![image](https://github.com/rizzzvi/checkout-steps/assets/51655413/47d23f38-8a78-43e5-a46e-4d472480faea)


