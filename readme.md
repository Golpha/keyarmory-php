## Key Armory client library for PHP

This is the official PHP client library for the Key Armory Encryption Key Orchestration Service. You'll first need an account by going to https://keyarmory.com. Follow the instructions to set up a project and key pool and then place the API Key you receive in the initialization script below.

### Installation
```
composer install keyarmory/keyarmory
```

### Initialization
```js
$keyarmory = new KeyArmory([
    api_key: 'your_api_key_here'
]);
```

### Encryption
```js
$encrypted_string = $keyarmory->encrypt($your_data);
```

### Decryption
```js
$your_data = $keyarmory->decrypt($encrypted_string);
```