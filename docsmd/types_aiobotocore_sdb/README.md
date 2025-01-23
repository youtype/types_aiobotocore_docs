# SimpleDB module

> [Index](../README.md) > SimpleDB


!!! note ""

    Auto-generated documentation for [SimpleDB](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sdb.html#simpledb)
    type annotations stubs module [types-aiobotocore-sdb](https://pypi.org/project/types-aiobotocore-sdb/).

## How to install

### Generate locally (recommended)

You can generate type annotations for `aiobotocore` package locally with `mypy_boto3_builder`.
Use [uv](https://docs.astral.sh/uv/getting-started/installation/) for build isolation.

1. Run mypy-boto3-builder in your package root directory: `uvx --with 'aiobotocore==2.19.0' mypy_boto3_builder`
1. Select `aiobotocore` AWS SDK.
1. Add `SimpleDB` service.
1. Use provided commands to install generated packages.



### From PyPI with pip

Install `types-aiobotocore` for `SimpleDB` service.

```bash
# install with aiobotocore type annotations
python -m pip install 'types-aiobotocore[sdb]'

# Lite version does not provide session.client/resource overloads
# it is more RAM-friendly, but requires explicit type annotations
python -m pip install 'types-aiobotocore-lite[sdb]'

# standalone installation
python -m pip install types-aiobotocore-sdb
```



## How to uninstall

```bash
python -m pip uninstall -y types-aiobotocore-sdb
```

## Usage

Code samples can be found in [Examples](./usage.md).

## SimpleDBClient

Type annotations and code completion for  `#!python session.create_client("sdb")` as [SimpleDBClient](./client.md)
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sdb.html#SimpleDB.Client)

```python
# SimpleDBClient usage example

from aiobotocore.session import get_session

from types_aiobotocore_sdb.client import SimpleDBClient


session = get_session()
async with session.create_client("sdb") as client:
    client: SimpleDBClient
```


## Paginators

Type annotations and code completion for
[paginators](./paginators.md)
from `#!python session.create_client("sdb").get_paginator("...")`.

```python
# ListDomainsPaginator usage example

from types_aiobotocore_sdb.paginator import ListDomainsPaginator

def get_list_domains_paginator() -> ListDomainsPaginator:
    return client.get_paginator("list_domains"))
```

- [ListDomainsPaginator](./paginators.md#listdomainspaginator)
- [SelectPaginator](./paginators.md#selectpaginator)








## Literals

Type annotations for [literals](./literals.md) used in methods and schema.

```python
# ListDomainsPaginatorName usage example

from types_aiobotocore_sdb.literals import ListDomainsPaginatorName

def get_value() -> ListDomainsPaginatorName:
    return "list_domains"
```

- [ListDomainsPaginatorName](./literals.md#listdomainspaginatorname)
- [SelectPaginatorName](./literals.md#selectpaginatorname)
- [SimpleDBServiceName](./literals.md#simpledbservicename)
- [ServiceName](./literals.md#servicename)
- [ResourceServiceName](./literals.md#resourceservicename)
- [PaginatorName](./literals.md#paginatorname)
- [RegionName](./literals.md#regionname)




## Type definitions

Type annotations for [type definitions](./type_defs.md) used in methods and schema.

- [AttributeTypeDef](./type_defs.md#attributetypedef)
- [CreateDomainRequestRequestTypeDef](./type_defs.md#createdomainrequestrequesttypedef)
- [UpdateConditionTypeDef](./type_defs.md#updateconditiontypedef)
- [DeleteDomainRequestRequestTypeDef](./type_defs.md#deletedomainrequestrequesttypedef)
- [DomainMetadataRequestRequestTypeDef](./type_defs.md#domainmetadatarequestrequesttypedef)
- [ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef)
- [GetAttributesRequestRequestTypeDef](./type_defs.md#getattributesrequestrequesttypedef)
- [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
- [ListDomainsRequestRequestTypeDef](./type_defs.md#listdomainsrequestrequesttypedef)
- [ReplaceableAttributeTypeDef](./type_defs.md#replaceableattributetypedef)
- [SelectRequestRequestTypeDef](./type_defs.md#selectrequestrequesttypedef)
- [DeletableItemTypeDef](./type_defs.md#deletableitemtypedef)
- [ItemTypeDef](./type_defs.md#itemtypedef)
- [DeleteAttributesRequestRequestTypeDef](./type_defs.md#deleteattributesrequestrequesttypedef)
- [DomainMetadataResultTypeDef](./type_defs.md#domainmetadataresulttypedef)
- [EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef)
- [GetAttributesResultTypeDef](./type_defs.md#getattributesresulttypedef)
- [ListDomainsResultTypeDef](./type_defs.md#listdomainsresulttypedef)
- [ListDomainsRequestPaginateTypeDef](./type_defs.md#listdomainsrequestpaginatetypedef)
- [SelectRequestPaginateTypeDef](./type_defs.md#selectrequestpaginatetypedef)
- [PutAttributesRequestRequestTypeDef](./type_defs.md#putattributesrequestrequesttypedef)
- [ReplaceableItemTypeDef](./type_defs.md#replaceableitemtypedef)
- [BatchDeleteAttributesRequestRequestTypeDef](./type_defs.md#batchdeleteattributesrequestrequesttypedef)
- [SelectResultTypeDef](./type_defs.md#selectresulttypedef)
- [BatchPutAttributesRequestRequestTypeDef](./type_defs.md#batchputattributesrequestrequesttypedef)

