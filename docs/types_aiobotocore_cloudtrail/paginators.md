<a id="paginators-for-aiobotocore-cloudtrail-module"></a>

# Paginators for aiobotocore CloudTrail module

> [Index](../README.md) > [CloudTrail](./README.md) > Paginators

Auto-generated documentation for
[CloudTrail](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudtrail.html#CloudTrail)
type annotations stubs module
[types-aiobotocore-cloudtrail](https://pypi.org/project/types-aiobotocore-cloudtrail/).

- [Paginators for aiobotocore CloudTrail module](#paginators-for-aiobotocore-cloudtrail-module)
  - [ListPublicKeysPaginator](#listpublickeyspaginator)
  - [ListTagsPaginator](#listtagspaginator)
  - [ListTrailsPaginator](#listtrailspaginator)
  - [LookupEventsPaginator](#lookupeventspaginator)

<a id="listpublickeyspaginator"></a>

## ListPublicKeysPaginator

Type annotations for
`session.create_client("cloudtrail").get_paginator("list_public_keys")`.

Can be used directly:

```python
from aiobotocore.session import get_session

from types_aiobotocore_cloudtrail.paginator import ListPublicKeysPaginator

session = get_session()
async with session.create_client("cloudtrail") as client:
    client: CloudTrailClient
    paginator: ListPublicKeysPaginator = client.get_paginator("list_public_keys")
```

Boto3 documentation:
[CloudTrail.Paginator.ListPublicKeys](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudtrail.html#CloudTrail.Paginator.ListPublicKeys)

Arguments for `ListPublicKeysPaginator.paginate` method:

- `StartTime`: `Union`\[`datetime`, `str`\]
- `EndTime`: `Union`\[`datetime`, `str`\]
- `PaginationConfig`:
  [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)

`ListPublicKeysPaginator.paginate` returns
`AsyncIterator`\[[ListPublicKeysResponseTypeDef](./type_defs.md#listpublickeysresponsetypedef)\].

<a id="listtagspaginator"></a>

## ListTagsPaginator

Type annotations for
`session.create_client("cloudtrail").get_paginator("list_tags")`.

Can be used directly:

```python
from aiobotocore.session import get_session

from types_aiobotocore_cloudtrail.paginator import ListTagsPaginator

session = get_session()
async with session.create_client("cloudtrail") as client:
    client: CloudTrailClient
    paginator: ListTagsPaginator = client.get_paginator("list_tags")
```

Boto3 documentation:
[CloudTrail.Paginator.ListTags](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudtrail.html#CloudTrail.Paginator.ListTags)

Arguments for `ListTagsPaginator.paginate` method:

- `ResourceIdList`: `Sequence`\[`str`\] *(required)*
- `PaginationConfig`:
  [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)

`ListTagsPaginator.paginate` returns
`AsyncIterator`\[[ListTagsResponseTypeDef](./type_defs.md#listtagsresponsetypedef)\].

<a id="listtrailspaginator"></a>

## ListTrailsPaginator

Type annotations for
`session.create_client("cloudtrail").get_paginator("list_trails")`.

Can be used directly:

```python
from aiobotocore.session import get_session

from types_aiobotocore_cloudtrail.paginator import ListTrailsPaginator

session = get_session()
async with session.create_client("cloudtrail") as client:
    client: CloudTrailClient
    paginator: ListTrailsPaginator = client.get_paginator("list_trails")
```

Boto3 documentation:
[CloudTrail.Paginator.ListTrails](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudtrail.html#CloudTrail.Paginator.ListTrails)

Arguments for `ListTrailsPaginator.paginate` method:

- `PaginationConfig`:
  [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)

`ListTrailsPaginator.paginate` returns
`AsyncIterator`\[[ListTrailsResponseTypeDef](./type_defs.md#listtrailsresponsetypedef)\].

<a id="lookupeventspaginator"></a>

## LookupEventsPaginator

Type annotations for
`session.create_client("cloudtrail").get_paginator("lookup_events")`.

Can be used directly:

```python
from aiobotocore.session import get_session

from types_aiobotocore_cloudtrail.paginator import LookupEventsPaginator

session = get_session()
async with session.create_client("cloudtrail") as client:
    client: CloudTrailClient
    paginator: LookupEventsPaginator = client.get_paginator("lookup_events")
```

Boto3 documentation:
[CloudTrail.Paginator.LookupEvents](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudtrail.html#CloudTrail.Paginator.LookupEvents)

Arguments for `LookupEventsPaginator.paginate` method:

- `LookupAttributes`:
  `Sequence`\[[LookupAttributeTypeDef](./type_defs.md#lookupattributetypedef)\]
- `StartTime`: `Union`\[`datetime`, `str`\]
- `EndTime`: `Union`\[`datetime`, `str`\]
- `EventCategory`: `Literal['insight']` (see
  [EventCategoryType](./literals.md#eventcategorytype))
- `PaginationConfig`:
  [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)

`LookupEventsPaginator.paginate` returns
`AsyncIterator`\[[LookupEventsResponseTypeDef](./type_defs.md#lookupeventsresponsetypedef)\].
