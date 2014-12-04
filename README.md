Commerce Payment Settings Switcher
==================================

Drupal Commerce module which allows you to easily switch payment settings based on environment variables.

This module lets you define a ``paypal_settings`` variable or a ``stripe_settings`` variable in your ``settings.local.php``, to override the configuration of your payment gateway.

## Paypal settings

```
// sites/default/settings.local.php
$conf['paypal_settings'] = array(
  "business" => "admin@example.com",
  "currency_code" => "EUR",
  "allow_supported_currencies" => "FALSE",
  "language" => "FR",
  "server" => "live",
  "payment_action" => "sale",
  "ipn_logging" => "notification",
  "receiver_emails" => "", 
  "ipn_create_billing_profile" => "FALSE",
  "show_payment_instructions" => "FALSE",
);
```
