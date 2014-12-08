Commerce Payment Settings Switcher
==================================

Drupal Commerce module which allows you to easily switch payment settings based on environment variables.

## Payment settings

### Paypal

```
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

```
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

```
$conf['paymill_settings']['mode'] = 'test';
```
