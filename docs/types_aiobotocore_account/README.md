<a id="type-annotations-for-aiobotocore-account-module"></a>

# Type annotations for aiobotocore Account module

> [Index](../README.md) > Account

Auto-generated documentation for
[Account](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/account.html#Account)
type annotations stubs module
[types-aiobotocore-account](https://pypi.org/project/types-aiobotocore-account/).

- [Type annotations for aiobotocore Account module](#type-annotations-for-aiobotocore-account-module)
  - [How to install](#how-to-install)
    - [VSCode extension](#vscode-extension)
    - [From PyPI with pip](#from-pypi-with-pip)
  - [How to uninstall](#how-to-uninstall)
  - [Usage](#usage)
  - [AccountClient](#accountclient)
    - [Methods](#methods)
    - [Exceptions](#exceptions)
  - [Literals](#literals)
  - [Typed dictionaries](#typed-dictionaries)

<a id="how-to-install"></a>

## How to install

<a id="vscode-extension"></a>

### VSCode extension

Add
[AWS Boto3](https://marketplace.visualstudio.com/items?itemName=Boto3typed.boto3-ide)
extension to your VSCode and run `AWS boto3: Quick Start` command.

Click `Modify` and select `boto3 common` and `Account`.

<a id="from-pypi-with-pip"></a>

### From PyPI with pip

Install `types-aiobotocore` for `Account` service.

```bash
# install with aiobotocore type annotations
python -m pip install 'types-aiobotocore[account]'


# Lite version does not provide session.client/resource overloads
# it is more RAM-friendly, but requires explicit type annotations
python -m pip install 'types-aiobotocore-lite[account]'


# standalone installation
python -m pip install types-aiobotocore-account
```

<a id="how-to-uninstall"></a>

## How to uninstall

```bash
python -m pip uninstall -y types-aiobotocore-account
```

<a id="usage"></a>

## Usage

Code samples can be found [here](./usage.md).

<a id="accountclient"></a>

## AccountClient

Type annotations for `session.create_client("account")` as
[AccountClient](./client.md)

Can be used directly:

```python
from types_aiobotocore_account.client import AccountClient
```

<a id="methods"></a>

### Methods

- [__aenter__](./client.md#__aenter__)
- [__aexit__](./client.md#__aexit__)
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
- [AccountServiceName](./literals.md#accountservicename)
- [ServiceName](./literals.md#servicename)
- [ResourceServiceName](./literals.md#resourceservicename)

<a id="typed-dictionaries"></a>

## Typed dictionaries

Type annotations for [typed dictionaries](./type_defs.md) used in methods and
schema.

Can be used directly:

```python
from types_aiobotocore_account.type_defs import AlternateContactTypeDef, ...
```

- [AlternateContactTypeDef](./type_defs.md#alternatecontacttypedef)
- [DeleteAlternateContactRequestRequestTypeDef](./type_defs.md#deletealternatecontactrequestrequesttypedef)
- [GetAlternateContactRequestRequestTypeDef](./type_defs.md#getalternatecontactrequestrequesttypedef)
- [GetAlternateContactResponseTypeDef](./type_defs.md#getalternatecontactresponsetypedef)
- [PutAlternateContactRequestRequestTypeDef](./type_defs.md#putalternatecontactrequestrequesttypedef)
- [ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef)