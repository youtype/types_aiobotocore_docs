<a id="typed-dictionaries-for-aiobotocore-account-module"></a>

# Typed dictionaries for aiobotocore Account module

> [Index](../README.md) > [Account](./README.md) > Typed dictionaries

Auto-generated documentation for
[Account](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/account.html#Account)
type annotations stubs module
[types-aiobotocore-account](https://pypi.org/project/types-aiobotocore-account/).

- [Typed dictionaries for aiobotocore Account module](#typed-dictionaries-for-aiobotocore-account-module)
  - [AlternateContactTypeDef](#alternatecontacttypedef)
  - [DeleteAlternateContactRequestRequestTypeDef](#deletealternatecontactrequestrequesttypedef)
  - [GetAlternateContactRequestRequestTypeDef](#getalternatecontactrequestrequesttypedef)
  - [GetAlternateContactResponseTypeDef](#getalternatecontactresponsetypedef)
  - [PutAlternateContactRequestRequestTypeDef](#putalternatecontactrequestrequesttypedef)
  - [ResponseMetadataTypeDef](#responsemetadatatypedef)

<a id="alternatecontacttypedef"></a>

## AlternateContactTypeDef

```python
from types_aiobotocore_account.type_defs import AlternateContactTypeDef
```

Optional fields:

- `AlternateContactType`:
  [AlternateContactTypeType](./literals.md#alternatecontacttypetype)
- `EmailAddress`: `str`
- `Name`: `str`
- `PhoneNumber`: `str`
- `Title`: `str`

<a id="deletealternatecontactrequestrequesttypedef"></a>

## DeleteAlternateContactRequestRequestTypeDef

```python
from types_aiobotocore_account.type_defs import DeleteAlternateContactRequestRequestTypeDef
```

Required fields:

- `AlternateContactType`:
  [AlternateContactTypeType](./literals.md#alternatecontacttypetype)

Optional fields:

- `AccountId`: `str`

<a id="getalternatecontactrequestrequesttypedef"></a>

## GetAlternateContactRequestRequestTypeDef

```python
from types_aiobotocore_account.type_defs import GetAlternateContactRequestRequestTypeDef
```

Required fields:

- `AlternateContactType`:
  [AlternateContactTypeType](./literals.md#alternatecontacttypetype)

Optional fields:

- `AccountId`: `str`

<a id="getalternatecontactresponsetypedef"></a>

## GetAlternateContactResponseTypeDef

```python
from types_aiobotocore_account.type_defs import GetAlternateContactResponseTypeDef
```

Required fields:

- `AlternateContact`:
  [AlternateContactTypeDef](./type_defs.md#alternatecontacttypedef)
- `ResponseMetadata`:
  [ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef)

<a id="putalternatecontactrequestrequesttypedef"></a>

## PutAlternateContactRequestRequestTypeDef

```python
from types_aiobotocore_account.type_defs import PutAlternateContactRequestRequestTypeDef
```

Required fields:

- `AlternateContactType`:
  [AlternateContactTypeType](./literals.md#alternatecontacttypetype)
- `EmailAddress`: `str`
- `Name`: `str`
- `PhoneNumber`: `str`
- `Title`: `str`

Optional fields:

- `AccountId`: `str`

<a id="responsemetadatatypedef"></a>

## ResponseMetadataTypeDef

```python
from types_aiobotocore_account.type_defs import ResponseMetadataTypeDef
```

Required fields:

- `RequestId`: `str`
- `HostId`: `str`
- `HTTPStatusCode`: `int`
- `HTTPHeaders`: `Dict`\[`str`, `str`\]
- `RetryAttempts`: `int`
