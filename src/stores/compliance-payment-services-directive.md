---
title: Payment Services Directive
group: getting-started
---

Starting September 14, 2019, the European Union requires that all merchants in the EU and UK comply with the [Strong Customer Authentication](https://payments.cardinalcommerce.com/what-is-psd2-sca) (SCA) requirements of the [Payment Services Directive](https://info.cardinalcommerce.com/psd2-compliance) (PSD2). Merchants in all other countries are encouraged to comply with PSD2 as a best practice.

Strong Customer Authentication is a key component of PSD2, and requires two of the following:

- Something only the customer has (password or PIN)
- Something only the customer knows (unique security token generated by phone or key fob)
- Something only the customer is (biometric authentication such as a fingerprint or facial recognition)

European banks may decline payments that do not meet the requirements. However, low risk and low value transactions might still be accepted, as well as subsequent payments in a recurring subscription.

Due to this significant change and to ensure that customer payments are not declined, we are introducing the following changes and recommendations for native Commerce payment integrations.

### PSD2 Compliance Guide

|Payment Method |Compliance Requirements |
|--- |--- |
|[PayPal]({% link payment/paypal.md %}) |For most PayPal solutions, no action is needed to comply with PSD2, because the requirements are handled by PayPal. For information about specific solutions, see the note at the top of each PayPal topic.|
|[Braintree]({% link payment/braintree.md %}) |Starting with the changeover to the installed extension in 2.4.0, the requirements are handled within the included Braintree Payments module and no action is needed to comply with PSD2. <br /><br />**_Note:_** To comply with PSD2 using the core integration in previous releases, do one of the following:<br/>- (Recommended) Install the official Braintree payment integration extension from [Commerce Marketplace](https://marketplace.magento.com/catalogsearch/result/?q=braintree#q=braintree&idx=m2_cloud_prod_default_products&p=0&nR%5Bvisibility_search%5D%5B%3D%5D%5B0%5D=1){:target="_blank"}.<br/>- Enable and configure the Braintree payment method in the Commerce configuration.<br/><br/>These earlier core integrations support 3D Secure 2.0 verification. However, Braintree implementations that run on JavaScript SDK v2 do not support 3D Secure 2.0.|
|Other |For all other payment integrations, check the available extensions on [Commerce Marketplace](https://marketplace.magento.com/extensions/payments-security/payment-integration.html?_ga=2.108129217.2105547619.1564067043-238341041.1564067043){:target="_blank"}. Ask your payment provider what solution they recommend to support PSD2 requirements.|