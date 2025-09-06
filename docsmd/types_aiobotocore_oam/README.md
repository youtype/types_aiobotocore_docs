# CloudWatchObservabilityAccessManager module

> [Index](../README.md) > CloudWatchObservabilityAccessManager


!!! note ""

    Auto-generated documentation for [CloudWatchObservabilityAccessManager](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/oam.html#cloudwatchobservabilityaccessmanager)
    type annotations stubs module [types-aiobotocore-oam](https://pypi.org/project/types-aiobotocore-oam/).

## How to install

### Generate locally (recommended)

You can generate type annotations for `aiobotocore` package locally with `mypy-boto3-builder`.
Use [uv](https://docs.astral.sh/uv/getting-started/installation/) for build isolation.

1. Run mypy-boto3-builder in your package root directory: `uvx --with 'aiobotocore==2.24.2' mypy-boto3-builder`
1. Select `aiobotocore` AWS SDK.
1. Add `CloudWatchObservabilityAccessManager` service.
1. Use provided commands to install generated packages.



### From PyPI with pip

Install `types-aiobotocore` for `CloudWatchObservabilityAccessManager` service.

```bash
# install with aiobotocore type annotations
python -m pip install 'types-aiobotocore[oam]'

# Lite version does not provide session.client/resource overloads
# it is more RAM-friendly, but requires explicit type annotations
python -m pip install 'types-aiobotocore-lite[oam]'

# standalone installation
python -m pip install types-aiobotocore-oam
```



## How to uninstall

```bash
python -m pip uninstall -y types-aiobotocore-oam
```

## Usage

Code samples can be found in [Examples](./usage.md).

## CloudWatchObservabilityAccessManagerClient

Type annotations and code completion for  `#!python session.create_client("oam")` as [CloudWatchObservabilityAccessManagerClient](./client.md)
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/oam.html#CloudWatchObservabilityAccessManager.Client)

```python
# CloudWatchObservabilityAccessManagerClient usage example

from aiobotocore.session import get_session

from types_aiobotocore_oam.client import CloudWatchObservabilityAccessManagerClient


session = get_session()
async with session.create_client("oam") as client:
    client: CloudWatchObservabilityAccessManagerClient
```


## Paginators

Type annotations and code completion for
[paginators](./paginators.md)
from `#!python session.create_client("oam").get_paginator("...")`.

```python
# ListAttachedLinksPaginator usage example

from types_aiobotocore_oam.paginator import ListAttachedLinksPaginator

def get_list_attached_links_paginator() -> ListAttachedLinksPaginator:
    return client.get_paginator("list_attached_links"))
```

- [ListAttachedLinksPaginator](./paginators.md#listattachedlinkspaginator)
- [ListLinksPaginator](./paginators.md#listlinkspaginator)
- [ListSinksPaginator](./paginators.md#listsinkspaginator)








## Literals

Type annotations for [literals](./literals.md) used in methods and schema.

```python
# ListAttachedLinksPaginatorName usage example

from types_aiobotocore_oam.literals import ListAttachedLinksPaginatorName

def get_value() -> ListAttachedLinksPaginatorName:
    return "list_attached_links"
```

- [ListAttachedLinksPaginatorName](./literals.md#listattachedlinkspaginatorname)
- [ListLinksPaginatorName](./literals.md#listlinkspaginatorname)
- [ListSinksPaginatorName](./literals.md#listsinkspaginatorname)
- [ResourceTypeType](./literals.md#resourcetypetype)
- [CloudWatchObservabilityAccessManagerServiceName](./literals.md#cloudwatchobservabilityaccessmanagerservicename)
- [ServiceName](./literals.md#servicename)
- [ResourceServiceName](./literals.md#resourceservicename)
- [PaginatorName](./literals.md#paginatorname)
- [RegionName](./literals.md#regionname)




## Type definitions

Type annotations for [type definitions](./type_defs.md) used in methods and schema.

- [ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef)
- [CreateSinkInputTypeDef](./type_defs.md#createsinkinputtypedef)
- [DeleteLinkInputTypeDef](./type_defs.md#deletelinkinputtypedef)
- [DeleteSinkInputTypeDef](./type_defs.md#deletesinkinputtypedef)
- [GetLinkInputTypeDef](./type_defs.md#getlinkinputtypedef)
- [GetSinkInputTypeDef](./type_defs.md#getsinkinputtypedef)
- [GetSinkPolicyInputTypeDef](./type_defs.md#getsinkpolicyinputtypedef)
- [LogGroupConfigurationTypeDef](./type_defs.md#loggroupconfigurationtypedef)
- [MetricConfigurationTypeDef](./type_defs.md#metricconfigurationtypedef)
- [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
- [ListAttachedLinksInputTypeDef](./type_defs.md#listattachedlinksinputtypedef)
- [ListAttachedLinksItemTypeDef](./type_defs.md#listattachedlinksitemtypedef)
- [ListLinksInputTypeDef](./type_defs.md#listlinksinputtypedef)
- [ListLinksItemTypeDef](./type_defs.md#listlinksitemtypedef)
- [ListSinksInputTypeDef](./type_defs.md#listsinksinputtypedef)
- [ListSinksItemTypeDef](./type_defs.md#listsinksitemtypedef)
- [ListTagsForResourceInputTypeDef](./type_defs.md#listtagsforresourceinputtypedef)
- [PutSinkPolicyInputTypeDef](./type_defs.md#putsinkpolicyinputtypedef)
- [TagResourceInputTypeDef](./type_defs.md#tagresourceinputtypedef)
- [UntagResourceInputTypeDef](./type_defs.md#untagresourceinputtypedef)
- [CreateSinkOutputTypeDef](./type_defs.md#createsinkoutputtypedef)
- [GetSinkOutputTypeDef](./type_defs.md#getsinkoutputtypedef)
- [GetSinkPolicyOutputTypeDef](./type_defs.md#getsinkpolicyoutputtypedef)
- [ListTagsForResourceOutputTypeDef](./type_defs.md#listtagsforresourceoutputtypedef)
- [PutSinkPolicyOutputTypeDef](./type_defs.md#putsinkpolicyoutputtypedef)
- [LinkConfigurationTypeDef](./type_defs.md#linkconfigurationtypedef)
- [ListAttachedLinksInputPaginateTypeDef](./type_defs.md#listattachedlinksinputpaginatetypedef)
- [ListLinksInputPaginateTypeDef](./type_defs.md#listlinksinputpaginatetypedef)
- [ListSinksInputPaginateTypeDef](./type_defs.md#listsinksinputpaginatetypedef)
- [ListAttachedLinksOutputTypeDef](./type_defs.md#listattachedlinksoutputtypedef)
- [ListLinksOutputTypeDef](./type_defs.md#listlinksoutputtypedef)
- [ListSinksOutputTypeDef](./type_defs.md#listsinksoutputtypedef)
- [CreateLinkInputTypeDef](./type_defs.md#createlinkinputtypedef)
- [CreateLinkOutputTypeDef](./type_defs.md#createlinkoutputtypedef)
- [GetLinkOutputTypeDef](./type_defs.md#getlinkoutputtypedef)
- [UpdateLinkInputTypeDef](./type_defs.md#updatelinkinputtypedef)
- [UpdateLinkOutputTypeDef](./type_defs.md#updatelinkoutputtypedef)

