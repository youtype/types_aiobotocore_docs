# RePostPrivate module

> [Index](../README.md) > RePostPrivate


!!! note ""

    Auto-generated documentation for [RePostPrivate](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/repostspace.html#RePostPrivate)
    type annotations stubs module [types-aiobotocore-repostspace](https://pypi.org/project/types-aiobotocore-repostspace/).

## How to install



### From PyPI with pip

Install `types-aiobotocore` for `RePostPrivate` service.

```bash
# install with aiobotocore type annotations
python -m pip install 'types-aiobotocore[repostspace]'


# Lite version does not provide session.client/resource overloads
# it is more RAM-friendly, but requires explicit type annotations
python -m pip install 'types-aiobotocore-lite[repostspace]'


# standalone installation
python -m pip install types-aiobotocore-repostspace
```



## How to uninstall

```bash
python -m pip uninstall -y types-aiobotocore-repostspace
```

## Usage

Code samples can be found in [Examples](./usage.md).

## RePostPrivateClient

Type annotations and code completion for  `#!python session.create_client("repostspace")` as [RePostPrivateClient](./client.md)
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/repostspace.html#RePostPrivate.Client)

```python
# RePostPrivateClient usage example

from aiobotocore.session import get_session

from types_aiobotocore_repostspace.client import RePostPrivateClient


session = get_session()
async with session.create_client("repostspace") as client:
    client: RePostPrivateClient
```


## Paginators

Type annotations and code completion for
[paginators](./paginators.md)
from `#!python session.create_client("repostspace").get_paginator("...")`.

```python
# ListSpacesPaginator usage example

from types_aiobotocore_repostspace.paginator import ListSpacesPaginator

def get_list_spaces_paginator() -> ListSpacesPaginator:
    return client.get_paginator("list_spaces"))
```

- [ListSpacesPaginator](./paginators.md#listspacespaginator)








## Literals

Type annotations for [literals](./literals.md) used in methods and schema.

```python
# ConfigurationStatusType usage example

from types_aiobotocore_repostspace.literals import ConfigurationStatusType

def get_value() -> ConfigurationStatusType:
    return "CONFIGURED"
```

- [ConfigurationStatusType](./literals.md#configurationstatustype)
- [ListSpacesPaginatorName](./literals.md#listspacespaginatorname)
- [RoleType](./literals.md#roletype)
- [TierLevelType](./literals.md#tierleveltype)
- [VanityDomainStatusType](./literals.md#vanitydomainstatustype)
- [RePostPrivateServiceName](./literals.md#repostprivateservicename)
- [ServiceName](./literals.md#servicename)
- [ResourceServiceName](./literals.md#resourceservicename)
- [PaginatorName](./literals.md#paginatorname)




## Type definitions

Type annotations for [type definitions](./type_defs.md) used in methods and schema.

- [BatchAddRoleInputRequestTypeDef](./type_defs.md#batchaddroleinputrequesttypedef)
- [BatchErrorTypeDef](./type_defs.md#batcherrortypedef)
- [ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef)
- [BatchRemoveRoleInputRequestTypeDef](./type_defs.md#batchremoveroleinputrequesttypedef)
- [CreateSpaceInputRequestTypeDef](./type_defs.md#createspaceinputrequesttypedef)
- [DeleteSpaceInputRequestTypeDef](./type_defs.md#deletespaceinputrequesttypedef)
- [DeregisterAdminInputRequestTypeDef](./type_defs.md#deregisteradmininputrequesttypedef)
- [GetSpaceInputRequestTypeDef](./type_defs.md#getspaceinputrequesttypedef)
- [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
- [ListSpacesInputRequestTypeDef](./type_defs.md#listspacesinputrequesttypedef)
- [SpaceDataTypeDef](./type_defs.md#spacedatatypedef)
- [ListTagsForResourceRequestRequestTypeDef](./type_defs.md#listtagsforresourcerequestrequesttypedef)
- [RegisterAdminInputRequestTypeDef](./type_defs.md#registeradmininputrequesttypedef)
- [SendInvitesInputRequestTypeDef](./type_defs.md#sendinvitesinputrequesttypedef)
- [TagResourceRequestRequestTypeDef](./type_defs.md#tagresourcerequestrequesttypedef)
- [UntagResourceRequestRequestTypeDef](./type_defs.md#untagresourcerequestrequesttypedef)
- [UpdateSpaceInputRequestTypeDef](./type_defs.md#updatespaceinputrequesttypedef)
- [BatchAddRoleOutputTypeDef](./type_defs.md#batchaddroleoutputtypedef)
- [BatchRemoveRoleOutputTypeDef](./type_defs.md#batchremoveroleoutputtypedef)
- [CreateSpaceOutputTypeDef](./type_defs.md#createspaceoutputtypedef)
- [EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef)
- [GetSpaceOutputTypeDef](./type_defs.md#getspaceoutputtypedef)
- [ListTagsForResourceResponseTypeDef](./type_defs.md#listtagsforresourceresponsetypedef)
- [ListSpacesInputListSpacesPaginateTypeDef](./type_defs.md#listspacesinputlistspacespaginatetypedef)
- [ListSpacesOutputTypeDef](./type_defs.md#listspacesoutputtypedef)

