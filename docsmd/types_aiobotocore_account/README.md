# Account module

> [Index](../README.md) > Account


!!! note ""

    Auto-generated documentation for [Account](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/account.html#Account)
    type annotations stubs module [types-aiobotocore-account](https://pypi.org/project/types-aiobotocore-account/).

## How to install

### VSCode extension

Add [AWS Boto3](https://marketplace.visualstudio.com/items?itemName=Boto3typed.boto3-ide)
extension to your VSCode and run `AWS boto3: Quick Start` command.

Click `Modify` and select `boto3 common` and `Account`.

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



## How to uninstall

```bash
python -m pip uninstall -y types-aiobotocore-account
```

## Usage

Code samples can be found in [Examples](./usage.md).

## AccountClient

Type annotations and code completion for  `#!python session.create_client("account")` as [AccountClient](./client.md)
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/account.html#Account.Client)

```python title="Usage example"
from aiobotocore.session import get_session

from types_aiobotocore_account.client import AccountClient


session = get_session()
async with session.create_client("account") as client:
    client: AccountClient
```








## Literals

Type annotations for [literals](./literals.md) used in methods and schema.

```python title="Usage example"
from types_aiobotocore_account.literals import AlternateContactTypeType

def get_value() -> AlternateContactTypeType:
    return "BILLING"
```

- [AlternateContactTypeType](./literals.md#alternatecontacttypetype)
- [AccountServiceName](./literals.md#accountservicename)
- [ServiceName](./literals.md#servicename)
- [ResourceServiceName](./literals.md#resourceservicename)




## Typed dictionaries

Type annotations for [typed dictionaries](./type_defs.md) used in methods and schema.

```python title="Usage example"
from types_aiobotocore_account.type_defs import AlternateContactTypeDef

def get_value() -> AlternateContactTypeDef:
    return {
        "AlternateContactType": ...,
    }
```

- [AlternateContactTypeDef](./type_defs.md#alternatecontacttypedef)
- [DeleteAlternateContactRequestRequestTypeDef](./type_defs.md#deletealternatecontactrequestrequesttypedef)
- [GetAlternateContactRequestRequestTypeDef](./type_defs.md#getalternatecontactrequestrequesttypedef)
- [GetAlternateContactResponseTypeDef](./type_defs.md#getalternatecontactresponsetypedef)
- [PutAlternateContactRequestRequestTypeDef](./type_defs.md#putalternatecontactrequestrequesttypedef)
- [ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef)

