# PaymentCryptographyControlPlaneClient

> [Index](../README.md) > [PaymentCryptographyControlPlane](./README.md) > PaymentCryptographyControlPlaneClient

!!! note ""

    Auto-generated documentation for [PaymentCryptographyControlPlane](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/payment-cryptography.html#paymentcryptographycontrolplane)
    type annotations stubs module [types-aiobotocore-payment-cryptography](https://pypi.org/project/types-aiobotocore-payment-cryptography/).

## PaymentCryptographyControlPlaneClient

Type annotations and code completion for `#!python session.create_client("payment-cryptography")`
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/payment-cryptography.html#PaymentCryptographyControlPlane.Client)

```python
# PaymentCryptographyControlPlaneClient usage example

from aiobotocore.session import get_session
from types_aiobotocore_payment_cryptography.client import PaymentCryptographyControlPlaneClient

session = get_session()
async with session.create_client("payment-cryptography") as client:
    client: PaymentCryptographyControlPlaneClient
```

## Exceptions


`aiobotocore` client exceptions are generated in runtime.
This class provides code completion for `#!python session.create_client("payment-cryptography").exceptions` structure.

```python
# PaymentCryptographyControlPlaneClient.exceptions usage example

async with session.create_client("payment-cryptography") as client:
    try:
        do_something(client)
    except (
            client.AccessDeniedException,
        client.ClientError,
        client.ConflictException,
        client.InternalServerException,
        client.ResourceNotFoundException,
        client.ServiceQuotaExceededException,
        client.ServiceUnavailableException,
        client.ThrottlingException,
        client.ValidationException,
    ) as e:
        print(e)
```

```python
# PaymentCryptographyControlPlaneClient usage type checking example

from types_aiobotocore_payment_cryptography.client import Exceptions

def handle_error(exc: Exceptions.AccessDeniedException) -> None:
    ...
```


## Methods


### can\_paginate



Type annotations and code completion for `#!python session.create_client("payment-cryptography").can_paginate` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/payment-cryptography/client/can_paginate.html)

```python
# can_paginate method definition

def can_paginate(
    self,
    operation_name: str,
) -> bool:
    ...
```


### generate\_presigned\_url



Type annotations and code completion for `#!python session.create_client("payment-cryptography").generate_presigned_url` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/payment-cryptography/client/generate_presigned_url.html)

```python
# generate_presigned_url method definition

await def generate_presigned_url(
    self,
    ClientMethod: str,
    Params: Mapping[str, Any] = ...,
    ExpiresIn: int = 3600,
    HttpMethod: str = ...,
) -> str:
    ...
```


### create\_alias

Creates an <i>alias</i>, or a friendly name, for an Amazon Web Services Payment
Cryptography key.

Type annotations and code completion for `#!python session.create_client("payment-cryptography").create_alias` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/payment-cryptography/client/create_alias.html)

```python
# create_alias method definition

await def create_alias(
    self,
    *,
    AliasName: str,
    KeyArn: str = ...,
) -> CreateAliasOutputTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: CreateAliasOutputTypeDef](./type_defs.md#createaliasoutputtypedef) 


```python
# create_alias method usage example with argument unpacking

kwargs: CreateAliasInputTypeDef = {  # (1)
    "AliasName": ...,
}

parent.create_alias(**kwargs)
```

1. See [:material-code-braces: CreateAliasInputTypeDef](./type_defs.md#createaliasinputtypedef) 

### create\_key

Creates an Amazon Web Services Payment Cryptography key, a logical
representation of a cryptographic key, that is unique in your account and
Amazon Web Services Region.

Type annotations and code completion for `#!python session.create_client("payment-cryptography").create_key` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/payment-cryptography/client/create_key.html)

```python
# create_key method definition

await def create_key(
    self,
    *,
    KeyAttributes: KeyAttributesTypeDef,  # (1)
    Exportable: bool,
    KeyCheckValueAlgorithm: KeyCheckValueAlgorithmType = ...,  # (2)
    Enabled: bool = ...,
    Tags: Sequence[TagTypeDef] = ...,  # (3)
) -> CreateKeyOutputTypeDef:  # (4)
    ...
```

1. See [:material-code-braces: KeyAttributesTypeDef](./type_defs.md#keyattributestypedef) 
2. See [:material-code-brackets: KeyCheckValueAlgorithmType](./literals.md#keycheckvaluealgorithmtype) 
3. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
4. See [:material-code-braces: CreateKeyOutputTypeDef](./type_defs.md#createkeyoutputtypedef) 


```python
# create_key method usage example with argument unpacking

kwargs: CreateKeyInputTypeDef = {  # (1)
    "KeyAttributes": ...,
    "Exportable": ...,
}

parent.create_key(**kwargs)
```

1. See [:material-code-braces: CreateKeyInputTypeDef](./type_defs.md#createkeyinputtypedef) 

### delete\_alias

Deletes the alias, but doesn't affect the underlying key.

Type annotations and code completion for `#!python session.create_client("payment-cryptography").delete_alias` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/payment-cryptography/client/delete_alias.html)

```python
# delete_alias method definition

await def delete_alias(
    self,
    *,
    AliasName: str,
) -> Dict[str, Any]:
    ...
```



```python
# delete_alias method usage example with argument unpacking

kwargs: DeleteAliasInputTypeDef = {  # (1)
    "AliasName": ...,
}

parent.delete_alias(**kwargs)
```

1. See [:material-code-braces: DeleteAliasInputTypeDef](./type_defs.md#deletealiasinputtypedef) 

### delete\_key

Deletes the key material and metadata associated with Amazon Web Services
Payment Cryptography key.

Type annotations and code completion for `#!python session.create_client("payment-cryptography").delete_key` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/payment-cryptography/client/delete_key.html)

```python
# delete_key method definition

await def delete_key(
    self,
    *,
    KeyIdentifier: str,
    DeleteKeyInDays: int = ...,
) -> DeleteKeyOutputTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DeleteKeyOutputTypeDef](./type_defs.md#deletekeyoutputtypedef) 


```python
# delete_key method usage example with argument unpacking

kwargs: DeleteKeyInputTypeDef = {  # (1)
    "KeyIdentifier": ...,
}

parent.delete_key(**kwargs)
```

1. See [:material-code-braces: DeleteKeyInputTypeDef](./type_defs.md#deletekeyinputtypedef) 

### export\_key

Exports a key from Amazon Web Services Payment Cryptography.

Type annotations and code completion for `#!python session.create_client("payment-cryptography").export_key` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/payment-cryptography/client/export_key.html)

```python
# export_key method definition

await def export_key(
    self,
    *,
    KeyMaterial: ExportKeyMaterialTypeDef,  # (1)
    ExportKeyIdentifier: str,
    ExportAttributes: ExportAttributesTypeDef = ...,  # (2)
) -> ExportKeyOutputTypeDef:  # (3)
    ...
```

1. See [:material-code-braces: ExportKeyMaterialTypeDef](./type_defs.md#exportkeymaterialtypedef) 
2. See [:material-code-braces: ExportAttributesTypeDef](./type_defs.md#exportattributestypedef) 
3. See [:material-code-braces: ExportKeyOutputTypeDef](./type_defs.md#exportkeyoutputtypedef) 


```python
# export_key method usage example with argument unpacking

kwargs: ExportKeyInputTypeDef = {  # (1)
    "KeyMaterial": ...,
    "ExportKeyIdentifier": ...,
}

parent.export_key(**kwargs)
```

1. See [:material-code-braces: ExportKeyInputTypeDef](./type_defs.md#exportkeyinputtypedef) 

### get\_alias

Gets the Amazon Web Services Payment Cryptography key associated with the alias.

Type annotations and code completion for `#!python session.create_client("payment-cryptography").get_alias` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/payment-cryptography/client/get_alias.html)

```python
# get_alias method definition

await def get_alias(
    self,
    *,
    AliasName: str,
) -> GetAliasOutputTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetAliasOutputTypeDef](./type_defs.md#getaliasoutputtypedef) 


```python
# get_alias method usage example with argument unpacking

kwargs: GetAliasInputTypeDef = {  # (1)
    "AliasName": ...,
}

parent.get_alias(**kwargs)
```

1. See [:material-code-braces: GetAliasInputTypeDef](./type_defs.md#getaliasinputtypedef) 

### get\_key

Gets the key material for an Amazon Web Services Payment Cryptography key,
including the immutable and mutable data specified when the key was created.

Type annotations and code completion for `#!python session.create_client("payment-cryptography").get_key` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/payment-cryptography/client/get_key.html)

```python
# get_key method definition

await def get_key(
    self,
    *,
    KeyIdentifier: str,
) -> GetKeyOutputTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetKeyOutputTypeDef](./type_defs.md#getkeyoutputtypedef) 


```python
# get_key method usage example with argument unpacking

kwargs: GetKeyInputTypeDef = {  # (1)
    "KeyIdentifier": ...,
}

parent.get_key(**kwargs)
```

1. See [:material-code-braces: GetKeyInputTypeDef](./type_defs.md#getkeyinputtypedef) 

### get\_parameters\_for\_export

Gets the export token and the signing key certificate to initiate a TR-34 key
export from Amazon Web Services Payment Cryptography.

Type annotations and code completion for `#!python session.create_client("payment-cryptography").get_parameters_for_export` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/payment-cryptography/client/get_parameters_for_export.html)

```python
# get_parameters_for_export method definition

await def get_parameters_for_export(
    self,
    *,
    KeyMaterialType: KeyMaterialTypeType,  # (1)
    SigningKeyAlgorithm: KeyAlgorithmType,  # (2)
) -> GetParametersForExportOutputTypeDef:  # (3)
    ...
```

1. See [:material-code-brackets: KeyMaterialTypeType](./literals.md#keymaterialtypetype) 
2. See [:material-code-brackets: KeyAlgorithmType](./literals.md#keyalgorithmtype) 
3. See [:material-code-braces: GetParametersForExportOutputTypeDef](./type_defs.md#getparametersforexportoutputtypedef) 


```python
# get_parameters_for_export method usage example with argument unpacking

kwargs: GetParametersForExportInputTypeDef = {  # (1)
    "KeyMaterialType": ...,
    "SigningKeyAlgorithm": ...,
}

parent.get_parameters_for_export(**kwargs)
```

1. See [:material-code-braces: GetParametersForExportInputTypeDef](./type_defs.md#getparametersforexportinputtypedef) 

### get\_parameters\_for\_import

Gets the import token and the wrapping key certificate in PEM format (base64
encoded) to initiate a TR-34 WrappedKeyBlock or a RSA WrappedKeyCryptogram
import into Amazon Web Services Payment Cryptography.

Type annotations and code completion for `#!python session.create_client("payment-cryptography").get_parameters_for_import` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/payment-cryptography/client/get_parameters_for_import.html)

```python
# get_parameters_for_import method definition

await def get_parameters_for_import(
    self,
    *,
    KeyMaterialType: KeyMaterialTypeType,  # (1)
    WrappingKeyAlgorithm: KeyAlgorithmType,  # (2)
) -> GetParametersForImportOutputTypeDef:  # (3)
    ...
```

1. See [:material-code-brackets: KeyMaterialTypeType](./literals.md#keymaterialtypetype) 
2. See [:material-code-brackets: KeyAlgorithmType](./literals.md#keyalgorithmtype) 
3. See [:material-code-braces: GetParametersForImportOutputTypeDef](./type_defs.md#getparametersforimportoutputtypedef) 


```python
# get_parameters_for_import method usage example with argument unpacking

kwargs: GetParametersForImportInputTypeDef = {  # (1)
    "KeyMaterialType": ...,
    "WrappingKeyAlgorithm": ...,
}

parent.get_parameters_for_import(**kwargs)
```

1. See [:material-code-braces: GetParametersForImportInputTypeDef](./type_defs.md#getparametersforimportinputtypedef) 

### get\_public\_key\_certificate

Gets the public key certificate of the asymmetric key pair that exists within
Amazon Web Services Payment Cryptography.

Type annotations and code completion for `#!python session.create_client("payment-cryptography").get_public_key_certificate` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/payment-cryptography/client/get_public_key_certificate.html)

```python
# get_public_key_certificate method definition

await def get_public_key_certificate(
    self,
    *,
    KeyIdentifier: str,
) -> GetPublicKeyCertificateOutputTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetPublicKeyCertificateOutputTypeDef](./type_defs.md#getpublickeycertificateoutputtypedef) 


```python
# get_public_key_certificate method usage example with argument unpacking

kwargs: GetPublicKeyCertificateInputTypeDef = {  # (1)
    "KeyIdentifier": ...,
}

parent.get_public_key_certificate(**kwargs)
```

1. See [:material-code-braces: GetPublicKeyCertificateInputTypeDef](./type_defs.md#getpublickeycertificateinputtypedef) 

### import\_key

Imports symmetric keys and public key certificates in PEM format (base64
encoded) into Amazon Web Services Payment Cryptography.

Type annotations and code completion for `#!python session.create_client("payment-cryptography").import_key` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/payment-cryptography/client/import_key.html)

```python
# import_key method definition

await def import_key(
    self,
    *,
    KeyMaterial: ImportKeyMaterialTypeDef,  # (1)
    KeyCheckValueAlgorithm: KeyCheckValueAlgorithmType = ...,  # (2)
    Enabled: bool = ...,
    Tags: Sequence[TagTypeDef] = ...,  # (3)
) -> ImportKeyOutputTypeDef:  # (4)
    ...
```

1. See [:material-code-braces: ImportKeyMaterialTypeDef](./type_defs.md#importkeymaterialtypedef) 
2. See [:material-code-brackets: KeyCheckValueAlgorithmType](./literals.md#keycheckvaluealgorithmtype) 
3. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
4. See [:material-code-braces: ImportKeyOutputTypeDef](./type_defs.md#importkeyoutputtypedef) 


```python
# import_key method usage example with argument unpacking

kwargs: ImportKeyInputTypeDef = {  # (1)
    "KeyMaterial": ...,
}

parent.import_key(**kwargs)
```

1. See [:material-code-braces: ImportKeyInputTypeDef](./type_defs.md#importkeyinputtypedef) 

### list\_aliases

Lists the aliases for all keys in the caller's Amazon Web Services account and
Amazon Web Services Region.

Type annotations and code completion for `#!python session.create_client("payment-cryptography").list_aliases` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/payment-cryptography/client/list_aliases.html)

```python
# list_aliases method definition

await def list_aliases(
    self,
    *,
    KeyArn: str = ...,
    NextToken: str = ...,
    MaxResults: int = ...,
) -> ListAliasesOutputTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListAliasesOutputTypeDef](./type_defs.md#listaliasesoutputtypedef) 


```python
# list_aliases method usage example with argument unpacking

kwargs: ListAliasesInputTypeDef = {  # (1)
    "KeyArn": ...,
}

parent.list_aliases(**kwargs)
```

1. See [:material-code-braces: ListAliasesInputTypeDef](./type_defs.md#listaliasesinputtypedef) 

### list\_keys

Lists the keys in the caller's Amazon Web Services account and Amazon Web
Services Region.

Type annotations and code completion for `#!python session.create_client("payment-cryptography").list_keys` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/payment-cryptography/client/list_keys.html)

```python
# list_keys method definition

await def list_keys(
    self,
    *,
    KeyState: KeyStateType = ...,  # (1)
    NextToken: str = ...,
    MaxResults: int = ...,
) -> ListKeysOutputTypeDef:  # (2)
    ...
```

1. See [:material-code-brackets: KeyStateType](./literals.md#keystatetype) 
2. See [:material-code-braces: ListKeysOutputTypeDef](./type_defs.md#listkeysoutputtypedef) 


```python
# list_keys method usage example with argument unpacking

kwargs: ListKeysInputTypeDef = {  # (1)
    "KeyState": ...,
}

parent.list_keys(**kwargs)
```

1. See [:material-code-braces: ListKeysInputTypeDef](./type_defs.md#listkeysinputtypedef) 

### list\_tags\_for\_resource

Lists the tags for an Amazon Web Services resource.

Type annotations and code completion for `#!python session.create_client("payment-cryptography").list_tags_for_resource` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/payment-cryptography/client/list_tags_for_resource.html)

```python
# list_tags_for_resource method definition

await def list_tags_for_resource(
    self,
    *,
    ResourceArn: str,
    NextToken: str = ...,
    MaxResults: int = ...,
) -> ListTagsForResourceOutputTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListTagsForResourceOutputTypeDef](./type_defs.md#listtagsforresourceoutputtypedef) 


```python
# list_tags_for_resource method usage example with argument unpacking

kwargs: ListTagsForResourceInputTypeDef = {  # (1)
    "ResourceArn": ...,
}

parent.list_tags_for_resource(**kwargs)
```

1. See [:material-code-braces: ListTagsForResourceInputTypeDef](./type_defs.md#listtagsforresourceinputtypedef) 

### restore\_key

Cancels a scheduled key deletion during the waiting period.

Type annotations and code completion for `#!python session.create_client("payment-cryptography").restore_key` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/payment-cryptography/client/restore_key.html)

```python
# restore_key method definition

await def restore_key(
    self,
    *,
    KeyIdentifier: str,
) -> RestoreKeyOutputTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: RestoreKeyOutputTypeDef](./type_defs.md#restorekeyoutputtypedef) 


```python
# restore_key method usage example with argument unpacking

kwargs: RestoreKeyInputTypeDef = {  # (1)
    "KeyIdentifier": ...,
}

parent.restore_key(**kwargs)
```

1. See [:material-code-braces: RestoreKeyInputTypeDef](./type_defs.md#restorekeyinputtypedef) 

### start\_key\_usage

Enables an Amazon Web Services Payment Cryptography key, which makes it active
for cryptographic operations within Amazon Web Services Payment Cryptography.

Type annotations and code completion for `#!python session.create_client("payment-cryptography").start_key_usage` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/payment-cryptography/client/start_key_usage.html)

```python
# start_key_usage method definition

await def start_key_usage(
    self,
    *,
    KeyIdentifier: str,
) -> StartKeyUsageOutputTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: StartKeyUsageOutputTypeDef](./type_defs.md#startkeyusageoutputtypedef) 


```python
# start_key_usage method usage example with argument unpacking

kwargs: StartKeyUsageInputTypeDef = {  # (1)
    "KeyIdentifier": ...,
}

parent.start_key_usage(**kwargs)
```

1. See [:material-code-braces: StartKeyUsageInputTypeDef](./type_defs.md#startkeyusageinputtypedef) 

### stop\_key\_usage

Disables an Amazon Web Services Payment Cryptography key, which makes it
inactive within Amazon Web Services Payment Cryptography.

Type annotations and code completion for `#!python session.create_client("payment-cryptography").stop_key_usage` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/payment-cryptography/client/stop_key_usage.html)

```python
# stop_key_usage method definition

await def stop_key_usage(
    self,
    *,
    KeyIdentifier: str,
) -> StopKeyUsageOutputTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: StopKeyUsageOutputTypeDef](./type_defs.md#stopkeyusageoutputtypedef) 


```python
# stop_key_usage method usage example with argument unpacking

kwargs: StopKeyUsageInputTypeDef = {  # (1)
    "KeyIdentifier": ...,
}

parent.stop_key_usage(**kwargs)
```

1. See [:material-code-braces: StopKeyUsageInputTypeDef](./type_defs.md#stopkeyusageinputtypedef) 

### tag\_resource

Adds or edits tags on an Amazon Web Services Payment Cryptography key.

Type annotations and code completion for `#!python session.create_client("payment-cryptography").tag_resource` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/payment-cryptography/client/tag_resource.html)

```python
# tag_resource method definition

await def tag_resource(
    self,
    *,
    ResourceArn: str,
    Tags: Sequence[TagTypeDef],  # (1)
) -> Dict[str, Any]:
    ...
```

1. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 


```python
# tag_resource method usage example with argument unpacking

kwargs: TagResourceInputTypeDef = {  # (1)
    "ResourceArn": ...,
    "Tags": ...,
}

parent.tag_resource(**kwargs)
```

1. See [:material-code-braces: TagResourceInputTypeDef](./type_defs.md#tagresourceinputtypedef) 

### untag\_resource

Deletes a tag from an Amazon Web Services Payment Cryptography key.

Type annotations and code completion for `#!python session.create_client("payment-cryptography").untag_resource` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/payment-cryptography/client/untag_resource.html)

```python
# untag_resource method definition

await def untag_resource(
    self,
    *,
    ResourceArn: str,
    TagKeys: Sequence[str],
) -> Dict[str, Any]:
    ...
```



```python
# untag_resource method usage example with argument unpacking

kwargs: UntagResourceInputTypeDef = {  # (1)
    "ResourceArn": ...,
    "TagKeys": ...,
}

parent.untag_resource(**kwargs)
```

1. See [:material-code-braces: UntagResourceInputTypeDef](./type_defs.md#untagresourceinputtypedef) 

### update\_alias

Associates an existing Amazon Web Services Payment Cryptography alias with a
different key.

Type annotations and code completion for `#!python session.create_client("payment-cryptography").update_alias` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/payment-cryptography/client/update_alias.html)

```python
# update_alias method definition

await def update_alias(
    self,
    *,
    AliasName: str,
    KeyArn: str = ...,
) -> UpdateAliasOutputTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: UpdateAliasOutputTypeDef](./type_defs.md#updatealiasoutputtypedef) 


```python
# update_alias method usage example with argument unpacking

kwargs: UpdateAliasInputTypeDef = {  # (1)
    "AliasName": ...,
}

parent.update_alias(**kwargs)
```

1. See [:material-code-braces: UpdateAliasInputTypeDef](./type_defs.md#updatealiasinputtypedef) 

### \_\_aenter\_\_



Type annotations and code completion for `#!python session.create_client("payment-cryptography").__aenter__` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/payment-cryptography.html#PaymentCryptographyControlPlane.Client)

```python
# __aenter__ method definition

await def __aenter__(
    self,
) -> Self:
    ...
```


### \_\_aexit\_\_



Type annotations and code completion for `#!python session.create_client("payment-cryptography").__aexit__` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/payment-cryptography.html#PaymentCryptographyControlPlane.Client)

```python
# __aexit__ method definition

await def __aexit__(
    self,
    exc_type: Union[Type[BaseException], None],
    exc_val: Union[BaseException, None],
    exc_tb: Union[TracebackType, None],
) -> None:
    ...
```




### get_paginator

Type annotations and code completion for `#!python session.create_client("payment-cryptography").get_paginator` method with overloads.

- `client.get_paginator("list_aliases")` -> [ListAliasesPaginator](./paginators.md#listaliasespaginator)
- `client.get_paginator("list_keys")` -> [ListKeysPaginator](./paginators.md#listkeyspaginator)
- `client.get_paginator("list_tags_for_resource")` -> [ListTagsForResourcePaginator](./paginators.md#listtagsforresourcepaginator)



