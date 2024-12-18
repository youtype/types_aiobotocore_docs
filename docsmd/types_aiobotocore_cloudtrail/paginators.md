# Paginators

> [Index](../README.md) > [CloudTrail](./README.md) > Paginators

!!! note ""

    Auto-generated documentation for [CloudTrail](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudtrail.html#cloudtrail)
    type annotations stubs module [types-aiobotocore-cloudtrail](https://pypi.org/project/types-aiobotocore-cloudtrail/).

## ListImportFailuresPaginator

Type annotations and code completion for `#!python session.create_client("cloudtrail").get_paginator("list_import_failures")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudtrail/paginator/ListImportFailures.html#CloudTrail.Paginator.ListImportFailures)

```python
# ListImportFailuresPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_cloudtrail.paginator import ListImportFailuresPaginator

session = get_session()
async with session.create_client("cloudtrail") as client:  # (1)
    paginator: ListImportFailuresPaginator = client.get_paginator("list_import_failures")  # (2)
    async for item in paginator.paginate(...):
        item: ListImportFailuresResponseTypeDef
        print(item)  # (3)
```

1. client: [CloudTrailClient](./client.md)
2. paginator: [ListImportFailuresPaginator](./paginators.md#listimportfailurespaginator)
3. item: [:material-code-braces: ListImportFailuresResponseTypeDef](./type_defs.md#listimportfailuresresponsetypedef) 


### paginate

Type annotations and code completion for `#!python ListImportFailuresPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    ImportId: str,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AsyncIterator[ListImportFailuresResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListImportFailuresResponseTypeDef](./type_defs.md#listimportfailuresresponsetypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: ListImportFailuresRequestListImportFailuresPaginateTypeDef = {  # (1)
    "ImportId": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListImportFailuresRequestListImportFailuresPaginateTypeDef](./type_defs.md#listimportfailuresrequestlistimportfailurespaginatetypedef) 
## ListImportsPaginator

Type annotations and code completion for `#!python session.create_client("cloudtrail").get_paginator("list_imports")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudtrail/paginator/ListImports.html#CloudTrail.Paginator.ListImports)

```python
# ListImportsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_cloudtrail.paginator import ListImportsPaginator

session = get_session()
async with session.create_client("cloudtrail") as client:  # (1)
    paginator: ListImportsPaginator = client.get_paginator("list_imports")  # (2)
    async for item in paginator.paginate(...):
        item: ListImportsResponseTypeDef
        print(item)  # (3)
```

1. client: [CloudTrailClient](./client.md)
2. paginator: [ListImportsPaginator](./paginators.md#listimportspaginator)
3. item: [:material-code-braces: ListImportsResponseTypeDef](./type_defs.md#listimportsresponsetypedef) 


### paginate

Type annotations and code completion for `#!python ListImportsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    Destination: str = ...,
    ImportStatus: ImportStatusType = ...,  # (1)
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (2)
) -> AsyncIterator[ListImportsResponseTypeDef]:  # (3)
    ...
```

1. See [:material-code-brackets: ImportStatusType](./literals.md#importstatustype) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
3. See [:material-code-braces: ListImportsResponseTypeDef](./type_defs.md#listimportsresponsetypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: ListImportsRequestListImportsPaginateTypeDef = {  # (1)
    "Destination": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListImportsRequestListImportsPaginateTypeDef](./type_defs.md#listimportsrequestlistimportspaginatetypedef) 
## ListPublicKeysPaginator

Type annotations and code completion for `#!python session.create_client("cloudtrail").get_paginator("list_public_keys")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudtrail/paginator/ListPublicKeys.html#CloudTrail.Paginator.ListPublicKeys)

```python
# ListPublicKeysPaginator usage example

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

```python
# paginate method definition

def paginate(
    self,
    *,
    StartTime: TimestampTypeDef = ...,
    EndTime: TimestampTypeDef = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AsyncIterator[ListPublicKeysResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListPublicKeysResponseTypeDef](./type_defs.md#listpublickeysresponsetypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: ListPublicKeysRequestListPublicKeysPaginateTypeDef = {  # (1)
    "StartTime": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListPublicKeysRequestListPublicKeysPaginateTypeDef](./type_defs.md#listpublickeysrequestlistpublickeyspaginatetypedef) 
## ListTagsPaginator

Type annotations and code completion for `#!python session.create_client("cloudtrail").get_paginator("list_tags")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudtrail/paginator/ListTags.html#CloudTrail.Paginator.ListTags)

```python
# ListTagsPaginator usage example

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

```python
# paginate method definition

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


```python
# paginate method usage example with argument unpacking

kwargs: ListTagsRequestListTagsPaginateTypeDef = {  # (1)
    "ResourceIdList": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListTagsRequestListTagsPaginateTypeDef](./type_defs.md#listtagsrequestlisttagspaginatetypedef) 
## ListTrailsPaginator

Type annotations and code completion for `#!python session.create_client("cloudtrail").get_paginator("list_trails")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudtrail/paginator/ListTrails.html#CloudTrail.Paginator.ListTrails)

```python
# ListTrailsPaginator usage example

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

```python
# paginate method definition

def paginate(
    self,
    *,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AsyncIterator[ListTrailsResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListTrailsResponseTypeDef](./type_defs.md#listtrailsresponsetypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: ListTrailsRequestListTrailsPaginateTypeDef = {  # (1)
    "PaginationConfig": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListTrailsRequestListTrailsPaginateTypeDef](./type_defs.md#listtrailsrequestlisttrailspaginatetypedef) 
## LookupEventsPaginator

Type annotations and code completion for `#!python session.create_client("cloudtrail").get_paginator("lookup_events")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudtrail/paginator/LookupEvents.html#CloudTrail.Paginator.LookupEvents)

```python
# LookupEventsPaginator usage example

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

```python
# paginate method definition

def paginate(
    self,
    *,
    LookupAttributes: Sequence[LookupAttributeTypeDef] = ...,  # (1)
    StartTime: TimestampTypeDef = ...,
    EndTime: TimestampTypeDef = ...,
    EventCategory: EventCategoryType = ...,  # (2)
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (3)
) -> AsyncIterator[LookupEventsResponseTypeDef]:  # (4)
    ...
```

1. See [:material-code-braces: LookupAttributeTypeDef](./type_defs.md#lookupattributetypedef) 
2. See [:material-code-brackets: EventCategoryType](./literals.md#eventcategorytype) 
3. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
4. See [:material-code-braces: LookupEventsResponseTypeDef](./type_defs.md#lookupeventsresponsetypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: LookupEventsRequestLookupEventsPaginateTypeDef = {  # (1)
    "LookupAttributes": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: LookupEventsRequestLookupEventsPaginateTypeDef](./type_defs.md#lookupeventsrequestlookupeventspaginatetypedef) 
