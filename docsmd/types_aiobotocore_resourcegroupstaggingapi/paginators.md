# Paginators

> [Index](../README.md) > [ResourceGroupsTaggingAPI](./README.md) > Paginators

!!! note ""

    Auto-generated documentation for [ResourceGroupsTaggingAPI](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/resourcegroupstaggingapi.html#resourcegroupstaggingapi)
    type annotations stubs module [types-aiobotocore-resourcegroupstaggingapi](https://pypi.org/project/types-aiobotocore-resourcegroupstaggingapi/).

## GetComplianceSummaryPaginator

Type annotations and code completion for `#!python session.create_client("resourcegroupstaggingapi").get_paginator("get_compliance_summary")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/resourcegroupstaggingapi/paginator/GetComplianceSummary.html#ResourceGroupsTaggingAPI.Paginator.GetComplianceSummary)

```python
# GetComplianceSummaryPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_resourcegroupstaggingapi.paginator import GetComplianceSummaryPaginator

session = get_session()
async with session.create_client("resourcegroupstaggingapi") as client:  # (1)
    paginator: GetComplianceSummaryPaginator = client.get_paginator("get_compliance_summary")  # (2)
    async for item in paginator.paginate(...):
        item: GetComplianceSummaryOutputTypeDef
        print(item)  # (3)
```

1. client: [ResourceGroupsTaggingAPIClient](./client.md)
2. paginator: [GetComplianceSummaryPaginator](./paginators.md#getcompliancesummarypaginator)
3. item: `AioPageIterator[GetComplianceSummaryOutputTypeDef]`


### paginate

Type annotations and code completion for `#!python GetComplianceSummaryPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    TargetIdFilters: Sequence[str] = ...,
    RegionFilters: Sequence[str] = ...,
    ResourceTypeFilters: Sequence[str] = ...,
    TagKeyFilters: Sequence[str] = ...,
    GroupBy: Sequence[GroupByAttributeType] = ...,  # (1)
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (2)
) -> aiobotocore.paginate.AioPageIterator[GetComplianceSummaryOutputTypeDef]:  # (3)
    ...
```

1. See `Sequence[GroupByAttributeType]`
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
3. See `AioPageIterator[GetComplianceSummaryOutputTypeDef]`


```python
# paginate method usage example with argument unpacking

kwargs: GetComplianceSummaryInputPaginateTypeDef = {  # (1)
    "TargetIdFilters": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: GetComplianceSummaryInputPaginateTypeDef](./type_defs.md#getcompliancesummaryinputpaginatetypedef)
## GetResourcesPaginator

Type annotations and code completion for `#!python session.create_client("resourcegroupstaggingapi").get_paginator("get_resources")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/resourcegroupstaggingapi/paginator/GetResources.html#ResourceGroupsTaggingAPI.Paginator.GetResources)

```python
# GetResourcesPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_resourcegroupstaggingapi.paginator import GetResourcesPaginator

session = get_session()
async with session.create_client("resourcegroupstaggingapi") as client:  # (1)
    paginator: GetResourcesPaginator = client.get_paginator("get_resources")  # (2)
    async for item in paginator.paginate(...):
        item: GetResourcesOutputTypeDef
        print(item)  # (3)
```

1. client: [ResourceGroupsTaggingAPIClient](./client.md)
2. paginator: [GetResourcesPaginator](./paginators.md#getresourcespaginator)
3. item: `AioPageIterator[GetResourcesOutputTypeDef]`


### paginate

Type annotations and code completion for `#!python GetResourcesPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    TagFilters: Sequence[TagFilterTypeDef] = ...,  # (1)
    TagsPerPage: int = ...,
    ResourceTypeFilters: Sequence[str] = ...,
    IncludeComplianceDetails: bool = ...,
    ExcludeCompliantResources: bool = ...,
    ResourceARNList: Sequence[str] = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (2)
) -> aiobotocore.paginate.AioPageIterator[GetResourcesOutputTypeDef]:  # (3)
    ...
```

1. See `Sequence[TagFilterTypeDef]`
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
3. See `AioPageIterator[GetResourcesOutputTypeDef]`


```python
# paginate method usage example with argument unpacking

kwargs: GetResourcesInputPaginateTypeDef = {  # (1)
    "TagFilters": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: GetResourcesInputPaginateTypeDef](./type_defs.md#getresourcesinputpaginatetypedef)
## GetTagKeysPaginator

Type annotations and code completion for `#!python session.create_client("resourcegroupstaggingapi").get_paginator("get_tag_keys")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/resourcegroupstaggingapi/paginator/GetTagKeys.html#ResourceGroupsTaggingAPI.Paginator.GetTagKeys)

```python
# GetTagKeysPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_resourcegroupstaggingapi.paginator import GetTagKeysPaginator

session = get_session()
async with session.create_client("resourcegroupstaggingapi") as client:  # (1)
    paginator: GetTagKeysPaginator = client.get_paginator("get_tag_keys")  # (2)
    async for item in paginator.paginate(...):
        item: GetTagKeysOutputTypeDef
        print(item)  # (3)
```

1. client: [ResourceGroupsTaggingAPIClient](./client.md)
2. paginator: [GetTagKeysPaginator](./paginators.md#gettagkeyspaginator)
3. item: `AioPageIterator[GetTagKeysOutputTypeDef]`


### paginate

Type annotations and code completion for `#!python GetTagKeysPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> aiobotocore.paginate.AioPageIterator[GetTagKeysOutputTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
2. See `AioPageIterator[GetTagKeysOutputTypeDef]`


```python
# paginate method usage example with argument unpacking

kwargs: GetTagKeysInputPaginateTypeDef = {  # (1)
    "PaginationConfig": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: GetTagKeysInputPaginateTypeDef](./type_defs.md#gettagkeysinputpaginatetypedef)
## GetTagValuesPaginator

Type annotations and code completion for `#!python session.create_client("resourcegroupstaggingapi").get_paginator("get_tag_values")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/resourcegroupstaggingapi/paginator/GetTagValues.html#ResourceGroupsTaggingAPI.Paginator.GetTagValues)

```python
# GetTagValuesPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_resourcegroupstaggingapi.paginator import GetTagValuesPaginator

session = get_session()
async with session.create_client("resourcegroupstaggingapi") as client:  # (1)
    paginator: GetTagValuesPaginator = client.get_paginator("get_tag_values")  # (2)
    async for item in paginator.paginate(...):
        item: GetTagValuesOutputTypeDef
        print(item)  # (3)
```

1. client: [ResourceGroupsTaggingAPIClient](./client.md)
2. paginator: [GetTagValuesPaginator](./paginators.md#gettagvaluespaginator)
3. item: `AioPageIterator[GetTagValuesOutputTypeDef]`


### paginate

Type annotations and code completion for `#!python GetTagValuesPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    Key: str,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> aiobotocore.paginate.AioPageIterator[GetTagValuesOutputTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
2. See `AioPageIterator[GetTagValuesOutputTypeDef]`


```python
# paginate method usage example with argument unpacking

kwargs: GetTagValuesInputPaginateTypeDef = {  # (1)
    "Key": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: GetTagValuesInputPaginateTypeDef](./type_defs.md#gettagvaluesinputpaginatetypedef)
## ListRequiredTagsPaginator

Type annotations and code completion for `#!python session.create_client("resourcegroupstaggingapi").get_paginator("list_required_tags")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/resourcegroupstaggingapi/paginator/ListRequiredTags.html#ResourceGroupsTaggingAPI.Paginator.ListRequiredTags)

```python
# ListRequiredTagsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_resourcegroupstaggingapi.paginator import ListRequiredTagsPaginator

session = get_session()
async with session.create_client("resourcegroupstaggingapi") as client:  # (1)
    paginator: ListRequiredTagsPaginator = client.get_paginator("list_required_tags")  # (2)
    async for item in paginator.paginate(...):
        item: ListRequiredTagsOutputTypeDef
        print(item)  # (3)
```

1. client: [ResourceGroupsTaggingAPIClient](./client.md)
2. paginator: [ListRequiredTagsPaginator](./paginators.md#listrequiredtagspaginator)
3. item: `AioPageIterator[ListRequiredTagsOutputTypeDef]`


### paginate

Type annotations and code completion for `#!python ListRequiredTagsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> aiobotocore.paginate.AioPageIterator[ListRequiredTagsOutputTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
2. See `AioPageIterator[ListRequiredTagsOutputTypeDef]`


```python
# paginate method usage example with argument unpacking

kwargs: ListRequiredTagsInputPaginateTypeDef = {  # (1)
    "PaginationConfig": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListRequiredTagsInputPaginateTypeDef](./type_defs.md#listrequiredtagsinputpaginatetypedef)
