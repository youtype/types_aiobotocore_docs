# Paginators

> [Index](../README.md) > [CloudTrail](./README.md) > Paginators

!!! note ""

    Auto-generated documentation for [CloudTrail](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudtrail.html#CloudTrail)
    type annotations stubs module [types-aiobotocore-cloudtrail](https://pypi.org/project/types-aiobotocore-cloudtrail/).

## ListPublicKeysPaginator

Type annotations and code completion for `#!python session.create_client("cloudtrail").get_paginator("list_public_keys")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudtrail.html#CloudTrail.Paginator.ListPublicKeys)

```python title="Usage example"
from aiobotocore.session import get_session

from types_aiobotocore_cloudtrail.paginator import ListPublicKeysPaginator

session = get_session()
async with session.create_client("cloudtrail") as client:  # (1)
    paginator: ListPublicKeysPaginator = client.get_paginator("list_public_keys")  # (2)
    async for item in paginator.paginate(...):
        item: ListPublicKeysResponseTypeDef
        print(item)  # (3)
```

1. client: [CloudTrailClient](./client.md)
2. paginator: [ListPublicKeysPaginator](./paginators.md#listpublickeyspaginator)
3. item: [:material-code-braces: ListPublicKeysResponseTypeDef](./type_defs.md#listpublickeysresponsetypedef) 


### paginate

Type annotations and code completion for `#!python ListPublicKeysPaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    StartTime: Union[datetime, str] = ...,
    EndTime: Union[datetime, str] = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AsyncIterator[ListPublicKeysResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListPublicKeysResponseTypeDef](./type_defs.md#listpublickeysresponsetypedef) 


```python title="Usage example with kwargs"
kwargs: ListPublicKeysRequestListPublicKeysPaginateTypeDef = {  # (1)
    "StartTime": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListPublicKeysRequestListPublicKeysPaginateTypeDef](./type_defs.md#listpublickeysrequestlistpublickeyspaginatetypedef) 
## ListTagsPaginator

Type annotations and code completion for `#!python session.create_client("cloudtrail").get_paginator("list_tags")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudtrail.html#CloudTrail.Paginator.ListTags)

```python title="Usage example"
from aiobotocore.session import get_session

from types_aiobotocore_cloudtrail.paginator import ListTagsPaginator

session = get_session()
async with session.create_client("cloudtrail") as client:  # (1)
    paginator: ListTagsPaginator = client.get_paginator("list_tags")  # (2)
    async for item in paginator.paginate(...):
        item: ListTagsResponseTypeDef
        print(item)  # (3)
```

1. client: [CloudTrailClient](./client.md)
2. paginator: [ListTagsPaginator](./paginators.md#listtagspaginator)
3. item: [:material-code-braces: ListTagsResponseTypeDef](./type_defs.md#listtagsresponsetypedef) 


### paginate

Type annotations and code completion for `#!python ListTagsPaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    ResourceIdList: Sequence[str],
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AsyncIterator[ListTagsResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListTagsResponseTypeDef](./type_defs.md#listtagsresponsetypedef) 


```python title="Usage example with kwargs"
kwargs: ListTagsRequestListTagsPaginateTypeDef = {  # (1)
    "ResourceIdList": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListTagsRequestListTagsPaginateTypeDef](./type_defs.md#listtagsrequestlisttagspaginatetypedef) 
## ListTrailsPaginator

Type annotations and code completion for `#!python session.create_client("cloudtrail").get_paginator("list_trails")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudtrail.html#CloudTrail.Paginator.ListTrails)

```python title="Usage example"
from aiobotocore.session import get_session

from types_aiobotocore_cloudtrail.paginator import ListTrailsPaginator

session = get_session()
async with session.create_client("cloudtrail") as client:  # (1)
    paginator: ListTrailsPaginator = client.get_paginator("list_trails")  # (2)
    async for item in paginator.paginate(...):
        item: ListTrailsResponseTypeDef
        print(item)  # (3)
```

1. client: [CloudTrailClient](./client.md)
2. paginator: [ListTrailsPaginator](./paginators.md#listtrailspaginator)
3. item: [:material-code-braces: ListTrailsResponseTypeDef](./type_defs.md#listtrailsresponsetypedef) 


### paginate

Type annotations and code completion for `#!python ListTrailsPaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AsyncIterator[ListTrailsResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListTrailsResponseTypeDef](./type_defs.md#listtrailsresponsetypedef) 


```python title="Usage example with kwargs"
kwargs: ListTrailsRequestListTrailsPaginateTypeDef = {  # (1)
    "PaginationConfig": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListTrailsRequestListTrailsPaginateTypeDef](./type_defs.md#listtrailsrequestlisttrailspaginatetypedef) 
## LookupEventsPaginator

Type annotations and code completion for `#!python session.create_client("cloudtrail").get_paginator("lookup_events")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudtrail.html#CloudTrail.Paginator.LookupEvents)

```python title="Usage example"
from aiobotocore.session import get_session

from types_aiobotocore_cloudtrail.paginator import LookupEventsPaginator

session = get_session()
async with session.create_client("cloudtrail") as client:  # (1)
    paginator: LookupEventsPaginator = client.get_paginator("lookup_events")  # (2)
    async for item in paginator.paginate(...):
        item: LookupEventsResponseTypeDef
        print(item)  # (3)
```

1. client: [CloudTrailClient](./client.md)
2. paginator: [LookupEventsPaginator](./paginators.md#lookupeventspaginator)
3. item: [:material-code-braces: LookupEventsResponseTypeDef](./type_defs.md#lookupeventsresponsetypedef) 


### paginate

Type annotations and code completion for `#!python LookupEventsPaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    LookupAttributes: Sequence[LookupAttributeTypeDef] = ...,  # (1)
    StartTime: Union[datetime, str] = ...,
    EndTime: Union[datetime, str] = ...,
    EventCategory: EventCategoryType = ...,  # (2)
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (3)
) -> AsyncIterator[LookupEventsResponseTypeDef]:  # (4)
    ...
```

1. See [:material-code-braces: LookupAttributeTypeDef](./type_defs.md#lookupattributetypedef) 
2. See [:material-code-brackets: EventCategoryType](./literals.md#eventcategorytype) 
3. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
4. See [:material-code-braces: LookupEventsResponseTypeDef](./type_defs.md#lookupeventsresponsetypedef) 


```python title="Usage example with kwargs"
kwargs: LookupEventsRequestLookupEventsPaginateTypeDef = {  # (1)
    "LookupAttributes": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: LookupEventsRequestLookupEventsPaginateTypeDef](./type_defs.md#lookupeventsrequestlookupeventspaginatetypedef) 
