# Stripe-Gateway-Integration-CodeIgniter 3.1.10

Import stripe.sql file in local database
download the project and place in wrok directory.


Create a developer account in stripe and from developer dashboard https://dashboard.stripe.com/
pick the publishkey and secretkey(test credentials) and paste in 

(1)\application\controllers\Welcome.php 
 "secret_key"      => "sk_test_********************",
"publishable_key" => "pk_test_********************"

(2)application\views\product_form.php
Stripe.setPublishableKey('pk_test_*********************');


project Path : localhost/stripe

Welcome page contain Card entering Form and section for admin login.

In Card Entering Form enter the Test card Details
Card Number 4242 4242 4242 4242	
Expiry :12 2024
CCvV : 123


select package ,fill details and submit payment
if charge payment success, payment successs page is shown else payment failure page is shown.

Admin Login
---------------
username : admin
password :1234567

On successfulLogin, will see a dashboard page with all subscriptions details of users in seen as table view.
Logut option is provided below.




