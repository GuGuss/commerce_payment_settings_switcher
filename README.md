Commerce Payment Settings Switcher
==================================

[Project is now maintained on Drupal.org](https://www.drupal.org/project/commerce_payment_settings_switcher).

Drupal Commerce module which allows you to easily switch payment settings based on environment variables.

## Payment settings

### Paypal
https://www.drupal.org/project/commerce_paypal
```php
// sites/default/settings.local.php
$conf['paypal_settings'] = array(
  'business' => '[PAYPAL_EMAIL]',
  'currency_code' => 'EUR',
  'allow_supported_currencies' => 'FALSE',
  'language' => 'FR',
  'server' => 'live', // 'sandbox'
  'payment_action' => 'sale',
  'ipn_logging' => 'notification',
  'receiver_emails' => '',
  'ipn_create_billing_profile' => 'FALSE',
  'show_payment_instructions' => 'FALSE',
);
```

### Stripe
https://www.drupal.org/project/commerce_stripe
```php
// sites/default/settings.local.php
$conf['stripe_settings'] = array(
  'mode' => 'test',
  'test' => array(
    'public_key' => '[TEST_PUBLIC_KEY]',
    'secret_key' => '[TEST_SECRET_KEY]',
  ),
);
```

### Paymill
https://www.drupal.org/project/commerce_paymill
```php
$conf['paymill_settings']['mode'] = 'test';
```

### Eway
https://www.drupal.org/project/commerce_eway
```php
$conf['eway_settings']['eway_testing'] = array(
  'test_mode' => 1,
  'live_database' => '',
  'test_mode_display_msg' => 1,
  'test_approve_anyway' => 1,
);
```
