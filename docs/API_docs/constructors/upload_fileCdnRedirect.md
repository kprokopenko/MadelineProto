---
title: upload.fileCdnRedirect
description: upload_fileCdnRedirect attributes, type and example
---
## Constructor: upload.fileCdnRedirect  
[Back to constructors index](index.md)



### Attributes:

| Name     |    Type       | Required |
|----------|:-------------:|---------:|
|dc\_id|[int](../types/int.md) | Yes|
|file\_token|[bytes](../types/bytes.md) | Yes|
|encryption\_key|[bytes](../types/bytes.md) | Yes|
|encryption\_iv|[bytes](../types/bytes.md) | Yes|



### Type: [upload\_File](../types/upload_File.md)


### Example:

```
$upload_fileCdnRedirect = ['_' => 'upload.fileCdnRedirect', 'dc_id' => int, 'file_token' => bytes, 'encryption_key' => bytes, 'encryption_iv' => bytes, ];
```  

Or, if you're into Lua:  


```
upload_fileCdnRedirect={_='upload.fileCdnRedirect', dc_id=int, file_token=bytes, encryption_key=bytes, encryption_iv=bytes, }

```


