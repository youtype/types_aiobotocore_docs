<a id="paginators-for-aiobotocore-resourcegroupstaggingapi-module"></a>

# Paginators for aiobotocore ResourceGroupsTaggingAPI module

> [Index](..) > [ResourceGroupsTaggingAPI](.) > Paginators

Auto-generated documentation for
[ResourceGroupsTaggingAPI](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/resourcegroupstaggingapi.html#ResourceGroupsTaggingAPI)
type annotations stubs module
[types-aiobotocore-resourcegroupstaggingapi](https://pypi.org/project/types-aiobotocore-resourcegroupstaggingapi/).

- [Paginators for aiobotocore ResourceGroupsTaggingAPI module](#paginators-for-aiobotocore-resourcegroupstaggingapi-module)
  - [GetComplianceSummaryPaginator](#getcompliancesummarypaginator)
  - [GetResourcesPaginator](#getresourcespaginator)
  - [GetTagKeysPaginator](#gettagkeyspaginator)
  - [GetTagValuesPaginator](#gettagvaluespaginator)

<a id="getcompliancesummarypaginator"></a>

## GetComplianceSummaryPaginator

Type annotations for
`session.create_client("resourcegroupstaggingapi").get_paginator("get_compliance_summary")`.

Can be used directly:

```python
from aiobotocore.session import get_session

from types_aiobotocore_resourcegroupstaggingapi.paginator import GetComplianceSummaryPaginator

session = get_session()
async with session.create_client("resourcegroupstaggingapi") as client:
    client: ResourceGroupsTaggingAPIClient
    paginator: GetComplianceSummaryPaginator = client.get_paginator("get_compliance_summary")
```

Boto3 documentation:
[ResourceGroupsTaggingAPI.Paginator.GetComplianceSummary](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/resourcegroupstaggingapi.html#ResourceGroupsTaggingAPI.Paginator.GetComplianceSummary)

Arguments for `GetComplianceSummaryPaginator.paginate` method:

- `TargetIdFilters`: `Sequence`\[`str`\]
- `RegionFilters`: `Sequence`\[`str`\]
- `ResourceTypeFilters`: `Sequence`\[`str`\]
- `TagKeyFilters`: `Sequence`\[`str`\]
- `GroupBy`:
  `Sequence`\[[GroupByAttributeType](./literals.md#groupbyattributetype)\]
- `PaginationConfig`:
  [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)

`GetComplianceSummaryPaginator.paginate` returns
`AsyncIterable`\[[GetComplianceSummaryOutputTypeDef](./type_defs.md#getcompliancesummaryoutputtypedef)\].

<a id="getresourcespaginator"></a>

## GetResourcesPaginator

Type annotations for
`session.create_client("resourcegroupstaggingapi").get_paginator("get_resources")`.

Can be used directly:

```python
from aiobotocore.session import get_session

from types_aiobotocore_resourcegroupstaggingapi.paginator import GetResourcesPaginator

session = get_session()
async with session.create_client("resourcegroupstaggingapi") as client:
    client: ResourceGroupsTaggingAPIClient
    paginator: GetResourcesPaginator = client.get_paginator("get_resources")
```

Boto3 documentation:
[ResourceGroupsTaggingAPI.Paginator.GetResources](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/resourcegroupstaggingapi.html#ResourceGroupsTaggingAPI.Paginator.GetResources)

Arguments for `GetResourcesPaginator.paginate` method:

- `TagFilters`:
  `Sequence`\[[TagFilterTypeDef](./type_defs.md#tagfiltertypedef)\]
- `TagsPerPage`: `int`
- `ResourceTypeFilters`: `Sequence`\[`str`\]
- `IncludeComplianceDetails`: `bool`
- `ExcludeCompliantResources`: `bool`
- `ResourceARNList`: `Sequence`\[`str`\]
- `PaginationConfig`:
  [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)

`GetResourcesPaginator.paginate` returns
`AsyncIterable`\[[GetResourcesOutputTypeDef](./type_defs.md#getresourcesoutputtypedef)\].

<a id="gettagkeyspaginator"></a>

## GetTagKeysPaginator

Type annotations for
`session.create_client("resourcegroupstaggingapi").get_paginator("get_tag_keys")`.

Can be used directly:

```python
from aiobotocore.session import get_session

from types_aiobotocore_resourcegroupstaggingapi.paginator import GetTagKeysPaginator

session = get_session()
async with session.create_client("resourcegroupstaggingapi") as client:
    client: ResourceGroupsTaggingAPIClient
    paginator: GetTagKeysPaginator = client.get_paginator("get_tag_keys")
```

Boto3 documentation:
[ResourceGroupsTaggingAPI.Paginator.GetTagKeys](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/resourcegroupstaggingapi.html#ResourceGroupsTaggingAPI.Paginator.GetTagKeys)

Arguments for `GetTagKeysPaginator.paginate` method:

- `PaginationConfig`:
  [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)

`GetTagKeysPaginator.paginate` returns
`AsyncIterable`\[[GetTagKeysOutputTypeDef](./type_defs.md#gettagkeysoutputtypedef)\].

<a id="gettagvaluespaginator"></a>

## GetTagValuesPaginator

Type annotations for
`session.create_client("resourcegroupstaggingapi").get_paginator("get_tag_values")`.

Can be used directly:

```python
from aiobotocore.session import get_session

from types_aiobotocore_resourcegroupstaggingapi.paginator import GetTagValuesPaginator

session = get_session()
async with session.create_client("resourcegroupstaggingapi") as client:
    client: ResourceGroupsTaggingAPIClient
    paginator: GetTagValuesPaginator = client.get_paginator("get_tag_values")
```

Boto3 documentation:
[ResourceGroupsTaggingAPI.Paginator.GetTagValues](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/resourcegroupstaggingapi.html#ResourceGroupsTaggingAPI.Paginator.GetTagValues)

Arguments for `GetTagValuesPaginator.paginate` method:

- `Key`: `str` *(required)*
- `PaginationConfig`:
  [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)

`GetTagValuesPaginator.paginate` returns
`AsyncIterable`\[[GetTagValuesOutputTypeDef](./type_defs.md#gettagvaluesoutputtypedef)\].
