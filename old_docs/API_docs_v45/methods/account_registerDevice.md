---
title: account.registerDevice
description: account.registerDevice parameters, return type and example
---
## Method: account.registerDevice  
[Back to methods index](index.md)


### Parameters:

| Name     |    Type       | Required |
|----------|:-------------:|---------:|
|token\_type|[int](../types/int.md) | Yes|
|token|[string](../types/string.md) | Yes|
|device\_model|[string](../types/string.md) | Yes|
|system\_version|[string](../types/string.md) | Yes|
|app\_version|[string](../types/string.md) | Yes|
|app\_sandbox|[Bool](../types/Bool.md) | Yes|
|lang\_code|[string](../types/string.md) | Yes|


### Return type: [Bool](../types/Bool.md)

### Example:


```
$MadelineProto = new \danog\MadelineProto\API();
if (isset($token)) { // Login as a bot
    $this->bot_login($token);
}
if (isset($number)) { // Login as a user
    $sentCode = $MadelineProto->phone_login($number);
    echo 'Enter the code you received: ';
    $code = '';
    for ($x = 0; $x < $sentCode['type']['length']; $x++) {
        $code .= fgetc(STDIN);
    }
    $MadelineProto->complete_phone_login($code);
}

$Bool = $MadelineProto->account->registerDevice(['token_type' => int, 'token' => string, 'device_model' => string, 'system_version' => string, 'app_version' => string, 'app_sandbox' => Bool, 'lang_code' => string, ]);
```

Or, if you're into Lua:

```
Bool = account.registerDevice({token_type=int, token=string, device_model=string, system_version=string, app_version=string, app_sandbox=Bool, lang_code=string, })
```

