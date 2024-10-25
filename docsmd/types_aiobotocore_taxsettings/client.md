# TaxSettingsClient

> [Index](../README.md) > [TaxSettings](./README.md) > TaxSettingsClient

!!! note ""

    Auto-generated documentation for [TaxSettings](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/taxsettings.html#TaxSettings)
    type annotations stubs module [types-aiobotocore-taxsettings](https://pypi.org/project/types-aiobotocore-taxsettings/).

## TaxSettingsClient

Type annotations and code completion for `#!python session.create_client("taxsettings")`
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/taxsettings.html#TaxSettings.Client)

```python
# TaxSettingsClient usage example

from aiobotocore.session import get_session
from types_aiobotocore_taxsettings.client import TaxSettingsClient

session = get_session()
async with session.create_client("taxsettings") as client:
    client: TaxSettingsClient
```

## Exceptions


`aiobotocore` client exceptions are generated in runtime.
This class provides code completion for `#!python session.create_client("taxsettings").exceptions` structure.

```python
# TaxSettingsClient.exceptions usage example

async with session.create_client("taxsettings") as client:
    try:
        do_something(client)
    except (
            client.ClientError,
        client.ConflictException,
        client.InternalServerException,
        client.ResourceNotFoundException,
        client.ValidationException,
    ) as e:
        print(e)
```

```python
# TaxSettingsClient usage type checking example

from types_aiobotocore_taxsettings.client import Exceptions

def handle_error(exc: Exceptions.ClientError) -> None:
    ...
```


## Methods


### batch\_delete\_tax\_registration

Deletes tax registration for multiple accounts in batch.

Type annotations and code completion for `#!python session.create_client("taxsettings").batch_delete_tax_registration` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/taxsettings.html#TaxSettings.Client.batch_delete_tax_registration)

```python
# batch_delete_tax_registration method definition

await def batch_delete_tax_registration(
    self,
    *,
    accountIds: Sequence[str],
) -> BatchDeleteTaxRegistrationResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: BatchDeleteTaxRegistrationResponseTypeDef](./type_defs.md#batchdeletetaxregistrationresponsetypedef) 


```python
# batch_delete_tax_registration method usage example with argument unpacking

kwargs: BatchDeleteTaxRegistrationRequestRequestTypeDef = {  # (1)
    "accountIds": ...,
}

parent.batch_delete_tax_registration(**kwargs)
```

1. See [:material-code-braces: BatchDeleteTaxRegistrationRequestRequestTypeDef](./type_defs.md#batchdeletetaxregistrationrequestrequesttypedef) 

### batch\_put\_tax\_registration

Adds or updates tax registration for multiple accounts in batch.

Type annotations and code completion for `#!python session.create_client("taxsettings").batch_put_tax_registration` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/taxsettings.html#TaxSettings.Client.batch_put_tax_registration)

```python
# batch_put_tax_registration method definition

await def batch_put_tax_registration(
    self,
    *,
    accountIds: Sequence[str],
    taxRegistrationEntry: TaxRegistrationEntryTypeDef,  # (1)
) -> BatchPutTaxRegistrationResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: TaxRegistrationEntryTypeDef](./type_defs.md#taxregistrationentrytypedef) 
2. See [:material-code-braces: BatchPutTaxRegistrationResponseTypeDef](./type_defs.md#batchputtaxregistrationresponsetypedef) 


```python
# batch_put_tax_registration method usage example with argument unpacking

kwargs: BatchPutTaxRegistrationRequestRequestTypeDef = {  # (1)
    "accountIds": ...,
    "taxRegistrationEntry": ...,
}

parent.batch_put_tax_registration(**kwargs)
```

1. See [:material-code-braces: BatchPutTaxRegistrationRequestRequestTypeDef](./type_defs.md#batchputtaxregistrationrequestrequesttypedef) 

### can\_paginate

Check if an operation can be paginated.

Type annotations and code completion for `#!python session.create_client("taxsettings").can_paginate` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/taxsettings.html#TaxSettings.Client.can_paginate)

```python
# can_paginate method definition

def can_paginate(
    self,
    operation_name: str,
) -> bool:
    ...
```


### close

Closes underlying endpoint connections.

Type annotations and code completion for `#!python session.create_client("taxsettings").close` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/taxsettings.html#TaxSettings.Client.close)

```python
# close method definition

await def close(
    self,
) -> None:
    ...
```


### delete\_tax\_registration

Deletes tax registration for a single account.

Type annotations and code completion for `#!python session.create_client("taxsettings").delete_tax_registration` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/taxsettings.html#TaxSettings.Client.delete_tax_registration)

```python
# delete_tax_registration method definition

await def delete_tax_registration(
    self,
    *,
    accountId: str = ...,
) -> Dict[str, Any]:
    ...
```



```python
# delete_tax_registration method usage example with argument unpacking

kwargs: DeleteTaxRegistrationRequestRequestTypeDef = {  # (1)
    "accountId": ...,
}

parent.delete_tax_registration(**kwargs)
```

1. See [:material-code-braces: DeleteTaxRegistrationRequestRequestTypeDef](./type_defs.md#deletetaxregistrationrequestrequesttypedef) 

### generate\_presigned\_url

Generate a presigned url given a client, its method, and arguments.

Type annotations and code completion for `#!python session.create_client("taxsettings").generate_presigned_url` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/taxsettings.html#TaxSettings.Client.generate_presigned_url)

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


### get\_tax\_registration

Retrieves tax registration for a single account.

Type annotations and code completion for `#!python session.create_client("taxsettings").get_tax_registration` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/taxsettings.html#TaxSettings.Client.get_tax_registration)

```python
# get_tax_registration method definition

await def get_tax_registration(
    self,
    *,
    accountId: str = ...,
) -> GetTaxRegistrationResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetTaxRegistrationResponseTypeDef](./type_defs.md#gettaxregistrationresponsetypedef) 


```python
# get_tax_registration method usage example with argument unpacking

kwargs: GetTaxRegistrationRequestRequestTypeDef = {  # (1)
    "accountId": ...,
}

parent.get_tax_registration(**kwargs)
```

1. See [:material-code-braces: GetTaxRegistrationRequestRequestTypeDef](./type_defs.md#gettaxregistrationrequestrequesttypedef) 

### get\_tax\_registration\_document

Downloads your tax documents to the Amazon S3 bucket that you specify in your
request.

Type annotations and code completion for `#!python session.create_client("taxsettings").get_tax_registration_document` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/taxsettings.html#TaxSettings.Client.get_tax_registration_document)

```python
# get_tax_registration_document method definition

await def get_tax_registration_document(
    self,
    *,
    destinationS3Location: DestinationS3LocationTypeDef,  # (1)
    taxDocumentMetadata: TaxDocumentMetadataTypeDef,  # (2)
) -> GetTaxRegistrationDocumentResponseTypeDef:  # (3)
    ...
```

1. See [:material-code-braces: DestinationS3LocationTypeDef](./type_defs.md#destinations3locationtypedef) 
2. See [:material-code-braces: TaxDocumentMetadataTypeDef](./type_defs.md#taxdocumentmetadatatypedef) 
3. See [:material-code-braces: GetTaxRegistrationDocumentResponseTypeDef](./type_defs.md#gettaxregistrationdocumentresponsetypedef) 


```python
# get_tax_registration_document method usage example with argument unpacking

kwargs: GetTaxRegistrationDocumentRequestRequestTypeDef = {  # (1)
    "destinationS3Location": ...,
    "taxDocumentMetadata": ...,
}

parent.get_tax_registration_document(**kwargs)
```

1. See [:material-code-braces: GetTaxRegistrationDocumentRequestRequestTypeDef](./type_defs.md#gettaxregistrationdocumentrequestrequesttypedef) 

### list\_tax\_registrations

Retrieves the tax registration of accounts listed in a consolidated billing
family.

Type annotations and code completion for `#!python session.create_client("taxsettings").list_tax_registrations` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/taxsettings.html#TaxSettings.Client.list_tax_registrations)

```python
# list_tax_registrations method definition

await def list_tax_registrations(
    self,
    *,
    maxResults: int = ...,
    nextToken: str = ...,
) -> ListTaxRegistrationsResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListTaxRegistrationsResponseTypeDef](./type_defs.md#listtaxregistrationsresponsetypedef) 


```python
# list_tax_registrations method usage example with argument unpacking

kwargs: ListTaxRegistrationsRequestRequestTypeDef = {  # (1)
    "maxResults": ...,
}

parent.list_tax_registrations(**kwargs)
```

1. See [:material-code-braces: ListTaxRegistrationsRequestRequestTypeDef](./type_defs.md#listtaxregistrationsrequestrequesttypedef) 

### put\_tax\_registration

Adds or updates tax registration for a single account.

Type annotations and code completion for `#!python session.create_client("taxsettings").put_tax_registration` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/taxsettings.html#TaxSettings.Client.put_tax_registration)

```python
# put_tax_registration method definition

await def put_tax_registration(
    self,
    *,
    taxRegistrationEntry: TaxRegistrationEntryTypeDef,  # (1)
    accountId: str = ...,
) -> PutTaxRegistrationResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: TaxRegistrationEntryTypeDef](./type_defs.md#taxregistrationentrytypedef) 
2. See [:material-code-braces: PutTaxRegistrationResponseTypeDef](./type_defs.md#puttaxregistrationresponsetypedef) 


```python
# put_tax_registration method usage example with argument unpacking

kwargs: PutTaxRegistrationRequestRequestTypeDef = {  # (1)
    "taxRegistrationEntry": ...,
}

parent.put_tax_registration(**kwargs)
```

1. See [:material-code-braces: PutTaxRegistrationRequestRequestTypeDef](./type_defs.md#puttaxregistrationrequestrequesttypedef) 

### \_\_aenter\_\_



Type annotations and code completion for `#!python session.create_client("taxsettings").__aenter__` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/taxsettings.html#TaxSettings.Client.__aenter__)

```python
# __aenter__ method definition

await def __aenter__(
    self,
) -> "TaxSettingsClient":
    ...
```


### \_\_aexit\_\_



Type annotations and code completion for `#!python session.create_client("taxsettings").__aexit__` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/taxsettings.html#TaxSettings.Client.__aexit__)

```python
# __aexit__ method definition

await def __aexit__(
    self,
    exc_type: Any,
    exc_val: Any,
    exc_tb: Any,
) -> Any:
    ...
```




### get_paginator

Type annotations and code completion for `#!python session.create_client("taxsettings").get_paginator` method with overloads.

- `client.get_paginator("list_tax_registrations")` -> [ListTaxRegistrationsPaginator](./paginators.md#listtaxregistrationspaginator)



