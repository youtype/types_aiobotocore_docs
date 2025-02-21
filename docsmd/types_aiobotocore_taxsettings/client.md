# TaxSettingsClient

> [Index](../README.md) > [TaxSettings](./README.md) > TaxSettingsClient

!!! note ""

    Auto-generated documentation for [TaxSettings](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/taxsettings.html#taxsettings)
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
            client.AccessDeniedException,
        client.AttachmentUploadException,
        client.CaseCreationLimitExceededException,
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

def handle_error(exc: Exceptions.AccessDeniedException) -> None:
    ...
```


## Methods


### can\_paginate



Type annotations and code completion for `#!python session.create_client("taxsettings").can_paginate` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/taxsettings/client/can_paginate.html)

```python
# can_paginate method definition

def can_paginate(
    self,
    operation_name: str,
) -> bool:
    ...
```


### generate\_presigned\_url



Type annotations and code completion for `#!python session.create_client("taxsettings").generate_presigned_url` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/taxsettings/client/generate_presigned_url.html)

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


### batch\_delete\_tax\_registration

Deletes tax registration for multiple accounts in batch.

Type annotations and code completion for `#!python session.create_client("taxsettings").batch_delete_tax_registration` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/taxsettings/client/batch_delete_tax_registration.html)

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

kwargs: BatchDeleteTaxRegistrationRequestTypeDef = {  # (1)
    "accountIds": ...,
}

parent.batch_delete_tax_registration(**kwargs)
```

1. See [:material-code-braces: BatchDeleteTaxRegistrationRequestTypeDef](./type_defs.md#batchdeletetaxregistrationrequesttypedef) 

### batch\_get\_tax\_exemptions

Get the active tax exemptions for a given list of accounts.

Type annotations and code completion for `#!python session.create_client("taxsettings").batch_get_tax_exemptions` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/taxsettings/client/batch_get_tax_exemptions.html)

```python
# batch_get_tax_exemptions method definition

await def batch_get_tax_exemptions(
    self,
    *,
    accountIds: Sequence[str],
) -> BatchGetTaxExemptionsResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: BatchGetTaxExemptionsResponseTypeDef](./type_defs.md#batchgettaxexemptionsresponsetypedef) 


```python
# batch_get_tax_exemptions method usage example with argument unpacking

kwargs: BatchGetTaxExemptionsRequestTypeDef = {  # (1)
    "accountIds": ...,
}

parent.batch_get_tax_exemptions(**kwargs)
```

1. See [:material-code-braces: BatchGetTaxExemptionsRequestTypeDef](./type_defs.md#batchgettaxexemptionsrequesttypedef) 

### batch\_put\_tax\_registration

Adds or updates tax registration for multiple accounts in batch.

Type annotations and code completion for `#!python session.create_client("taxsettings").batch_put_tax_registration` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/taxsettings/client/batch_put_tax_registration.html)

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

kwargs: BatchPutTaxRegistrationRequestTypeDef = {  # (1)
    "accountIds": ...,
    "taxRegistrationEntry": ...,
}

parent.batch_put_tax_registration(**kwargs)
```

1. See [:material-code-braces: BatchPutTaxRegistrationRequestTypeDef](./type_defs.md#batchputtaxregistrationrequesttypedef) 

### delete\_supplemental\_tax\_registration

Deletes a supplemental tax registration for a single account.

Type annotations and code completion for `#!python session.create_client("taxsettings").delete_supplemental_tax_registration` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/taxsettings/client/delete_supplemental_tax_registration.html)

```python
# delete_supplemental_tax_registration method definition

await def delete_supplemental_tax_registration(
    self,
    *,
    authorityId: str,
) -> Dict[str, Any]:
    ...
```



```python
# delete_supplemental_tax_registration method usage example with argument unpacking

kwargs: DeleteSupplementalTaxRegistrationRequestTypeDef = {  # (1)
    "authorityId": ...,
}

parent.delete_supplemental_tax_registration(**kwargs)
```

1. See [:material-code-braces: DeleteSupplementalTaxRegistrationRequestTypeDef](./type_defs.md#deletesupplementaltaxregistrationrequesttypedef) 

### delete\_tax\_registration

Deletes tax registration for a single account.

Type annotations and code completion for `#!python session.create_client("taxsettings").delete_tax_registration` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/taxsettings/client/delete_tax_registration.html)

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

kwargs: DeleteTaxRegistrationRequestTypeDef = {  # (1)
    "accountId": ...,
}

parent.delete_tax_registration(**kwargs)
```

1. See [:material-code-braces: DeleteTaxRegistrationRequestTypeDef](./type_defs.md#deletetaxregistrationrequesttypedef) 

### get\_tax\_exemption\_types

Get supported tax exemption types.

Type annotations and code completion for `#!python session.create_client("taxsettings").get_tax_exemption_types` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/taxsettings/client/get_tax_exemption_types.html)

```python
# get_tax_exemption_types method definition

await def get_tax_exemption_types(
    self,
) -> GetTaxExemptionTypesResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetTaxExemptionTypesResponseTypeDef](./type_defs.md#gettaxexemptiontypesresponsetypedef) 

### get\_tax\_inheritance

The get account tax inheritance status.

Type annotations and code completion for `#!python session.create_client("taxsettings").get_tax_inheritance` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/taxsettings/client/get_tax_inheritance.html)

```python
# get_tax_inheritance method definition

await def get_tax_inheritance(
    self,
) -> GetTaxInheritanceResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetTaxInheritanceResponseTypeDef](./type_defs.md#gettaxinheritanceresponsetypedef) 

### get\_tax\_registration

Retrieves tax registration for a single account.

Type annotations and code completion for `#!python session.create_client("taxsettings").get_tax_registration` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/taxsettings/client/get_tax_registration.html)

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

kwargs: GetTaxRegistrationRequestTypeDef = {  # (1)
    "accountId": ...,
}

parent.get_tax_registration(**kwargs)
```

1. See [:material-code-braces: GetTaxRegistrationRequestTypeDef](./type_defs.md#gettaxregistrationrequesttypedef) 

### get\_tax\_registration\_document

Downloads your tax documents to the Amazon S3 bucket that you specify in your
request.

Type annotations and code completion for `#!python session.create_client("taxsettings").get_tax_registration_document` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/taxsettings/client/get_tax_registration_document.html)

```python
# get_tax_registration_document method definition

await def get_tax_registration_document(
    self,
    *,
    taxDocumentMetadata: TaxDocumentMetadataTypeDef,  # (1)
    destinationS3Location: DestinationS3LocationTypeDef = ...,  # (2)
) -> GetTaxRegistrationDocumentResponseTypeDef:  # (3)
    ...
```

1. See [:material-code-braces: TaxDocumentMetadataTypeDef](./type_defs.md#taxdocumentmetadatatypedef) 
2. See [:material-code-braces: DestinationS3LocationTypeDef](./type_defs.md#destinations3locationtypedef) 
3. See [:material-code-braces: GetTaxRegistrationDocumentResponseTypeDef](./type_defs.md#gettaxregistrationdocumentresponsetypedef) 


```python
# get_tax_registration_document method usage example with argument unpacking

kwargs: GetTaxRegistrationDocumentRequestTypeDef = {  # (1)
    "taxDocumentMetadata": ...,
}

parent.get_tax_registration_document(**kwargs)
```

1. See [:material-code-braces: GetTaxRegistrationDocumentRequestTypeDef](./type_defs.md#gettaxregistrationdocumentrequesttypedef) 

### list\_supplemental\_tax\_registrations

Retrieves supplemental tax registrations for a single account.

Type annotations and code completion for `#!python session.create_client("taxsettings").list_supplemental_tax_registrations` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/taxsettings/client/list_supplemental_tax_registrations.html)

```python
# list_supplemental_tax_registrations method definition

await def list_supplemental_tax_registrations(
    self,
    *,
    maxResults: int = ...,
    nextToken: str = ...,
) -> ListSupplementalTaxRegistrationsResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListSupplementalTaxRegistrationsResponseTypeDef](./type_defs.md#listsupplementaltaxregistrationsresponsetypedef) 


```python
# list_supplemental_tax_registrations method usage example with argument unpacking

kwargs: ListSupplementalTaxRegistrationsRequestTypeDef = {  # (1)
    "maxResults": ...,
}

parent.list_supplemental_tax_registrations(**kwargs)
```

1. See [:material-code-braces: ListSupplementalTaxRegistrationsRequestTypeDef](./type_defs.md#listsupplementaltaxregistrationsrequesttypedef) 

### list\_tax\_exemptions

Retrieves the tax exemption of accounts listed in a consolidated billing family.

Type annotations and code completion for `#!python session.create_client("taxsettings").list_tax_exemptions` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/taxsettings/client/list_tax_exemptions.html)

```python
# list_tax_exemptions method definition

await def list_tax_exemptions(
    self,
    *,
    maxResults: int = ...,
    nextToken: str = ...,
) -> ListTaxExemptionsResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListTaxExemptionsResponseTypeDef](./type_defs.md#listtaxexemptionsresponsetypedef) 


```python
# list_tax_exemptions method usage example with argument unpacking

kwargs: ListTaxExemptionsRequestTypeDef = {  # (1)
    "maxResults": ...,
}

parent.list_tax_exemptions(**kwargs)
```

1. See [:material-code-braces: ListTaxExemptionsRequestTypeDef](./type_defs.md#listtaxexemptionsrequesttypedef) 

### list\_tax\_registrations

Retrieves the tax registration of accounts listed in a consolidated billing
family.

Type annotations and code completion for `#!python session.create_client("taxsettings").list_tax_registrations` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/taxsettings/client/list_tax_registrations.html)

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

kwargs: ListTaxRegistrationsRequestTypeDef = {  # (1)
    "maxResults": ...,
}

parent.list_tax_registrations(**kwargs)
```

1. See [:material-code-braces: ListTaxRegistrationsRequestTypeDef](./type_defs.md#listtaxregistrationsrequesttypedef) 

### put\_supplemental\_tax\_registration

Stores supplemental tax registration for a single account.

Type annotations and code completion for `#!python session.create_client("taxsettings").put_supplemental_tax_registration` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/taxsettings/client/put_supplemental_tax_registration.html)

```python
# put_supplemental_tax_registration method definition

await def put_supplemental_tax_registration(
    self,
    *,
    taxRegistrationEntry: SupplementalTaxRegistrationEntryTypeDef,  # (1)
) -> PutSupplementalTaxRegistrationResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: SupplementalTaxRegistrationEntryTypeDef](./type_defs.md#supplementaltaxregistrationentrytypedef) 
2. See [:material-code-braces: PutSupplementalTaxRegistrationResponseTypeDef](./type_defs.md#putsupplementaltaxregistrationresponsetypedef) 


```python
# put_supplemental_tax_registration method usage example with argument unpacking

kwargs: PutSupplementalTaxRegistrationRequestTypeDef = {  # (1)
    "taxRegistrationEntry": ...,
}

parent.put_supplemental_tax_registration(**kwargs)
```

1. See [:material-code-braces: PutSupplementalTaxRegistrationRequestTypeDef](./type_defs.md#putsupplementaltaxregistrationrequesttypedef) 

### put\_tax\_exemption

Adds the tax exemption for a single account or all accounts listed in a
consolidated billing family.

Type annotations and code completion for `#!python session.create_client("taxsettings").put_tax_exemption` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/taxsettings/client/put_tax_exemption.html)

```python
# put_tax_exemption method definition

await def put_tax_exemption(
    self,
    *,
    accountIds: Sequence[str],
    authority: AuthorityTypeDef,  # (1)
    exemptionCertificate: ExemptionCertificateTypeDef,  # (2)
    exemptionType: str,
) -> PutTaxExemptionResponseTypeDef:  # (3)
    ...
```

1. See [:material-code-braces: AuthorityTypeDef](./type_defs.md#authoritytypedef) 
2. See [:material-code-braces: ExemptionCertificateTypeDef](./type_defs.md#exemptioncertificatetypedef) 
3. See [:material-code-braces: PutTaxExemptionResponseTypeDef](./type_defs.md#puttaxexemptionresponsetypedef) 


```python
# put_tax_exemption method usage example with argument unpacking

kwargs: PutTaxExemptionRequestTypeDef = {  # (1)
    "accountIds": ...,
    "authority": ...,
    "exemptionCertificate": ...,
    "exemptionType": ...,
}

parent.put_tax_exemption(**kwargs)
```

1. See [:material-code-braces: PutTaxExemptionRequestTypeDef](./type_defs.md#puttaxexemptionrequesttypedef) 

### put\_tax\_inheritance

The updated tax inheritance status.

Type annotations and code completion for `#!python session.create_client("taxsettings").put_tax_inheritance` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/taxsettings/client/put_tax_inheritance.html)

```python
# put_tax_inheritance method definition

await def put_tax_inheritance(
    self,
    *,
    heritageStatus: HeritageStatusType = ...,  # (1)
) -> Dict[str, Any]:
    ...
```

1. See [:material-code-brackets: HeritageStatusType](./literals.md#heritagestatustype) 


```python
# put_tax_inheritance method usage example with argument unpacking

kwargs: PutTaxInheritanceRequestTypeDef = {  # (1)
    "heritageStatus": ...,
}

parent.put_tax_inheritance(**kwargs)
```

1. See [:material-code-braces: PutTaxInheritanceRequestTypeDef](./type_defs.md#puttaxinheritancerequesttypedef) 

### put\_tax\_registration

Adds or updates tax registration for a single account.

Type annotations and code completion for `#!python session.create_client("taxsettings").put_tax_registration` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/taxsettings/client/put_tax_registration.html)

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

kwargs: PutTaxRegistrationRequestTypeDef = {  # (1)
    "taxRegistrationEntry": ...,
}

parent.put_tax_registration(**kwargs)
```

1. See [:material-code-braces: PutTaxRegistrationRequestTypeDef](./type_defs.md#puttaxregistrationrequesttypedef) 

### \_\_aenter\_\_



Type annotations and code completion for `#!python session.create_client("taxsettings").__aenter__` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/taxsettings.html#TaxSettings.Client)

```python
# __aenter__ method definition

await def __aenter__(
    self,
) -> Self:
    ...
```


### \_\_aexit\_\_



Type annotations and code completion for `#!python session.create_client("taxsettings").__aexit__` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/taxsettings.html#TaxSettings.Client)

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

Type annotations and code completion for `#!python session.create_client("taxsettings").get_paginator` method with overloads.

- `client.get_paginator("list_supplemental_tax_registrations")` -> [ListSupplementalTaxRegistrationsPaginator](./paginators.md#listsupplementaltaxregistrationspaginator)
- `client.get_paginator("list_tax_exemptions")` -> [ListTaxExemptionsPaginator](./paginators.md#listtaxexemptionspaginator)
- `client.get_paginator("list_tax_registrations")` -> [ListTaxRegistrationsPaginator](./paginators.md#listtaxregistrationspaginator)



