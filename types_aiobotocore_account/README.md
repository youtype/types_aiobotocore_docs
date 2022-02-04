<a id="type-annotations-for-aiobotocore-account-module"></a>

# Type annotations for aiobotocore Account module

> [Index](..) > Account

Auto-generated documentation for
[Account](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/account.html#Account)
type annotations stubs module
[types-aiobotocore-account](https://pypi.org/project/types-aiobotocore-account/).

```bash
# install with types-aiobotocore
pip install 'types-aiobotocore[account]'

# install as a standalone
pip install types-aiobotocore-account
```

- [Type annotations for aiobotocore Account module](#type-annotations-for-aiobotocore-account-module)
  - [AccountClient](#accountclient)
    - [Methods](#methods)
    - [Exceptions](#exceptions)
  - [Literals](#literals)
  - [Typed dictionaries](#typed-dictionaries)

<a id="accountclient"></a>

## AccountClient

Type annotations for `aiobotocore.create_client("account")` as
[AccountClient](./client.md)

Can be used directly:

```python
from types_aiobotocore_account.client import AccountClient
```

<a id="methods"></a>

### Methods

- [can_paginate](./client.md#can_paginate)
- [delete_alternate_contact](./client.md#delete_alternate_contact)
- [exceptions](./client.md#exceptions)
- [generate_presigned_url](./client.md#generate_presigned_url)
- [get_alternate_contact](./client.md#get_alternate_contact)
- [put_alternate_contact](./client.md#put_alternate_contact)

<a id="exceptions"></a>

### Exceptions

AccountClient [exceptions](./client.md#exceptions)

- AccessDeniedException
- ClientError
- InternalServerException
- ResourceNotFoundException
- TooManyRequestsException
- ValidationException

<a id="literals"></a>

## Literals

Type annotations for [literals](./literals.md) used in methods and schema.

Can be used directly:

```python
from types_aiobotocore_account.literals import AlternateContactTypeType, ...
```

- [AlternateContactTypeType](./literals.md#alternatecontacttypetype)
- [ServiceName](./literals.md#servicename)

<a id="typed-dictionaries"></a>

## Typed dictionaries

Type annotations for [typed dictionaries](./type_defs.md) used in methods and
schema.

Can be used directly:

```python
from mypy_boto3_account.type_defs import AlternateContactTypeDef, ...
```

- [AlternateContactTypeDef](./type_defs.md#alternatecontacttypedef)
- [DeleteAlternateContactRequestRequestTypeDef](./type_defs.md#deletealternatecontactrequestrequesttypedef)
- [GetAlternateContactRequestRequestTypeDef](./type_defs.md#getalternatecontactrequestrequesttypedef)
- [GetAlternateContactResponseTypeDef](./type_defs.md#getalternatecontactresponsetypedef)
- [PutAlternateContactRequestRequestTypeDef](./type_defs.md#putalternatecontactrequestrequesttypedef)
- [ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef)
