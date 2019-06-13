# Installation

- Step #1: Copy the Paydunya folder into to app/code directory
- Step #2: Run: composer config repositories.paydunyaexpress git https://github.com/paydunya/module-paydunyaexpress
- Step #3: composer require paydunya/module-paydunyaexpress:dev-master
- Step #4: Run: php bin/magento module:enable Paydunya_Paydunyaexpress --clear-static-content
- Step #5: Run the magento setup upgrade function: bin/magento setup:upgrade 

Once you have done this, you need to follow these steps to get it working:

1.  Create a merchant account (Business account) at https://www.paydunya.com. 
    After registration, you will be able to create an application and get your private keys and token.
2.  Log into your Magento admin and Clear your cache
    Go to Stores -> Configuration -> Sales -> Payment Methods and you will see. "PayDunya"
3.  Setting configurations. 
    Set Enabled - YES. 
    Test API - NO (if you set this to yes, this means you are using our test PayDunya API)
    Enter the Private Key & Token.
    New order status - This is the default order status set when a user selects PayDunya to "processing".
    All orders with this status mean the user created an order but pending the payment.
4.  Save configurations
  
Paydunya - Beyond limits!
