# IdentityStore module

> [Index](../README.md) > IdentityStore


!!! note ""

    Auto-generated documentation for [IdentityStore](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/identitystore.html#IdentityStore)
    type annotations stubs module [types-aiobotocore-identitystore](https://pypi.org/project/types-aiobotocore-identitystore/).

## How to install

### VSCode extension

Add [AWS Boto3](https://marketplace.visualstudio.com/items?itemName=Boto3typed.boto3-ide)
extension to your VSCode and run `AWS boto3: Quick Start` command.

Click `Modify` and select `boto3 common` and `IdentityStore`.

### From PyPI with pip

Install `types-aiobotocore` for `IdentityStore` service.

```bash
# install with aiobotocore type annotations
python -m pip install 'types-aiobotocore[identitystore]'


# Lite version does not provide session.client/resource overloads
# it is more RAM-friendly, but requires explicit type annotations
python -m pip install 'types-aiobotocore-lite[identitystore]'


# standalone installation
python -m pip install types-aiobotocore-identitystore
```



## How to uninstall

```bash
python -m pip uninstall -y types-aiobotocore-identitystore
```

## Usage

Code samples can be found in [Examples](./usage.md).

## IdentityStoreClient

Type annotations and code completion for  `#!python session.create_client("identitystore")` as [IdentityStoreClient](./client.md)
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/identitystore.html#IdentityStore.Client)

```python title="Usage example"
from aiobotocore.session import get_session

from types_aiobotocore_identitystore.client import IdentityStoreClient


session = get_session()
async with session.create_client("identitystore") as client:
    client: IdentityStoreClient
```








## Literals

Type annotations for [literals](./literals.md) used in methods and schema.

```python title="Usage example"
from types_aiobotocore_identitystore.literals import IdentityStoreServiceName

def get_value() -> IdentityStoreServiceName:
    return "identitystore"
```

- [IdentityStoreServiceName](./literals.md#identitystoreservicename)
- [ServiceName](./literals.md#servicename)
- [ResourceServiceName](./literals.md#resourceservicename)
- [RegionName](./literals.md#regionname)




## Typed dictionaries

Type annotations for [typed dictionaries](./type_defs.md) used in methods and schema.

```python title="Usage example"
from types_aiobotocore_identitystore.type_defs import DescribeGroupRequestRequestTypeDef

def get_value() -> DescribeGroupRequestRequestTypeDef:
    return {
        "IdentityStoreId": ...,
        "GroupId": ...,
    }
```

- [DescribeGroupRequestRequestTypeDef](./type_defs.md#describegrouprequestrequesttypedef)
- [DescribeGroupResponseTypeDef](./type_defs.md#describegroupresponsetypedef)
- [DescribeUserRequestRequestTypeDef](./type_defs.md#describeuserrequestrequesttypedef)
- [DescribeUserResponseTypeDef](./type_defs.md#describeuserresponsetypedef)
- [FilterTypeDef](./type_defs.md#filtertypedef)
- [GroupTypeDef](./type_defs.md#grouptypedef)
- [ListGroupsRequestRequestTypeDef](./type_defs.md#listgroupsrequestrequesttypedef)
- [ListGroupsResponseTypeDef](./type_defs.md#listgroupsresponsetypedef)
- [ListUsersRequestRequestTypeDef](./type_defs.md#listusersrequestrequesttypedef)
- [ListUsersResponseTypeDef](./type_defs.md#listusersresponsetypedef)
- [ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef)
- [UserTypeDef](./type_defs.md#usertypedef)

