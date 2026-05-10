# ElementalInference module

> [Index](../README.md) > ElementalInference


!!! note ""

    Auto-generated documentation for [ElementalInference](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elementalinference.html#elementalinference)
    type annotations stubs module [types-aiobotocore-elementalinference](https://pypi.org/project/types-aiobotocore-elementalinference/).

## How to install

### Generate locally (recommended)

You can generate type annotations for `aiobotocore` package locally with `mypy-boto3-builder`.
Use [uv](https://docs.astral.sh/uv/getting-started/installation/) for build isolation.

1. Run mypy-boto3-builder in your package root directory: `uvx --with 'aiobotocore==3.7.0' mypy-boto3-builder`
1. Select `aiobotocore` AWS SDK.
1. Add `ElementalInference` service.
1. Use provided commands to install generated packages.



### From PyPI with pip

Install `types-aiobotocore` for `ElementalInference` service.

```bash
# install with aiobotocore type annotations
python -m pip install 'types-aiobotocore[elementalinference]'

# Lite version does not provide session.client/resource overloads
# it is more RAM-friendly, but requires explicit type annotations
python -m pip install 'types-aiobotocore-lite[elementalinference]'

# standalone installation
python -m pip install types-aiobotocore-elementalinference
```



## How to uninstall

```bash
python -m pip uninstall -y types-aiobotocore-elementalinference
```

## Usage

Code samples can be found in [Examples](./usage.md).

## ElementalInferenceClient

Type annotations and code completion for  `#!python session.create_client("elementalinference")` as [ElementalInferenceClient](./client.md)
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elementalinference.html#ElementalInference.Client)

```python
# ElementalInferenceClient usage example

from aiobotocore.session import get_session

from types_aiobotocore_elementalinference.client import ElementalInferenceClient


session = get_session()
async with session.create_client("elementalinference") as client:
    client: ElementalInferenceClient
```


## Paginators

Type annotations and code completion for
[paginators](./paginators.md)
from `#!python session.create_client("elementalinference").get_paginator("...")`.

```python
# ListFeedsPaginator usage example

from types_aiobotocore_elementalinference.paginator import ListFeedsPaginator

def get_list_feeds_paginator() -> ListFeedsPaginator:
    return client.get_paginator("list_feeds"))
```

- [ListFeedsPaginator](./paginators.md#listfeedspaginator)




## Waiters

Type annotations and code completion for
[waiters](./waiters.md)
from `#!python session.create_client("elementalinference").get_waiter("...")`.

```python
# FeedDeletedWaiter usage example

from types_aiobotocore_elementalinference.waiter import FeedDeletedWaiter

def get_feed_deleted_waiter() -> FeedDeletedWaiter:
    return Session().client("elementalinference").get_waiter("feed_deleted")
```

- [FeedDeletedWaiter](./waiters.md#feeddeletedwaiter)






## Literals

Type annotations for [literals](./literals.md) used in methods and schema.

```python
# FeedDeletedWaiterName usage example

from types_aiobotocore_elementalinference.literals import FeedDeletedWaiterName

def get_value() -> FeedDeletedWaiterName:
    return "feed_deleted"
```

- [FeedDeletedWaiterName](./literals.md#feeddeletedwaitername)
- [FeedStatusType](./literals.md#feedstatustype)
- [ListFeedsPaginatorName](./literals.md#listfeedspaginatorname)
- [OutputStatusType](./literals.md#outputstatustype)
- [ElementalInferenceServiceName](./literals.md#elementalinferenceservicename)
- [ServiceName](./literals.md#servicename)
- [ResourceServiceName](./literals.md#resourceservicename)
- [PaginatorName](./literals.md#paginatorname)
- [WaiterName](./literals.md#waitername)




## Type definitions

Type annotations for [type definitions](./type_defs.md) used in methods and schema.

- [ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef)
- [ClippingConfigTypeDef](./type_defs.md#clippingconfigtypedef)
- [FeedAssociationTypeDef](./type_defs.md#feedassociationtypedef)
- [DeleteFeedRequestTypeDef](./type_defs.md#deletefeedrequesttypedef)
- [DisassociateFeedRequestTypeDef](./type_defs.md#disassociatefeedrequesttypedef)
- [GetFeedRequestTypeDef](./type_defs.md#getfeedrequesttypedef)
- [WaiterConfigTypeDef](./type_defs.md#waiterconfigtypedef)
- [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
- [ListFeedsRequestTypeDef](./type_defs.md#listfeedsrequesttypedef)
- [ListTagsForResourceRequestTypeDef](./type_defs.md#listtagsforresourcerequesttypedef)
- [TagResourceRequestTypeDef](./type_defs.md#tagresourcerequesttypedef)
- [UntagResourceRequestTypeDef](./type_defs.md#untagresourcerequesttypedef)
- [AssociateFeedResponseTypeDef](./type_defs.md#associatefeedresponsetypedef)
- [DeleteFeedResponseTypeDef](./type_defs.md#deletefeedresponsetypedef)
- [DisassociateFeedResponseTypeDef](./type_defs.md#disassociatefeedresponsetypedef)
- [EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef)
- [ListTagsForResourceResponseTypeDef](./type_defs.md#listtagsforresourceresponsetypedef)
- [OutputConfigOutputTypeDef](./type_defs.md#outputconfigoutputtypedef)
- [OutputConfigTypeDef](./type_defs.md#outputconfigtypedef)
- [FeedSummaryTypeDef](./type_defs.md#feedsummarytypedef)
- [GetFeedRequestWaitTypeDef](./type_defs.md#getfeedrequestwaittypedef)
- [ListFeedsRequestPaginateTypeDef](./type_defs.md#listfeedsrequestpaginatetypedef)
- [GetOutputTypeDef](./type_defs.md#getoutputtypedef)
- [OutputConfigUnionTypeDef](./type_defs.md#outputconfiguniontypedef)
- [ListFeedsResponseTypeDef](./type_defs.md#listfeedsresponsetypedef)
- [CreateFeedResponseTypeDef](./type_defs.md#createfeedresponsetypedef)
- [GetFeedResponseTypeDef](./type_defs.md#getfeedresponsetypedef)
- [UpdateFeedResponseTypeDef](./type_defs.md#updatefeedresponsetypedef)
- [CreateOutputTypeDef](./type_defs.md#createoutputtypedef)
- [UpdateOutputTypeDef](./type_defs.md#updateoutputtypedef)
- [AssociateFeedRequestTypeDef](./type_defs.md#associatefeedrequesttypedef)
- [CreateFeedRequestTypeDef](./type_defs.md#createfeedrequesttypedef)
- [UpdateFeedRequestTypeDef](./type_defs.md#updatefeedrequesttypedef)

