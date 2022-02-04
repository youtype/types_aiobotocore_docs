<a id="paginators-for-aiobotocore-cloudtrail-module"></a>

# Paginators for aiobotocore CloudTrail module

> [Index](..) > [CloudTrail](.) > Paginators

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
`aiobotocore.create_client("cloudtrail").get_paginator("list_public_keys")`.

Can be used directly:

```python
from aiobotocore.session import Session

from types_aiobotocore_cloudtrail.paginator import ListPublicKeysPaginator

def get_list_public_keys_paginator() -> ListPublicKeysPaginator:
    return Session().create_client("cloudtrail").get_paginator("list_public_keys")
```

Boto3 documentation:
[CloudTrail.Paginator.ListPublicKeys](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudtrail.html#CloudTrail.Paginator.ListPublicKeys)

Arguments for `ListPublicKeysPaginator.paginate` method:

- `StartTime`: `Union`\[`datetime`, `str`\]
- `EndTime`: `Union`\[`datetime`, `str`\]
- `PaginationConfig`:
  [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)

`ListPublicKeysPaginator.paginate` returns
`_PageIterator`\[[ListPublicKeysResponseTypeDef](./type_defs.md#listpublickeysresponsetypedef)\].

<a id="listtagspaginator"></a>

## ListTagsPaginator

Type annotations for
`aiobotocore.create_client("cloudtrail").get_paginator("list_tags")`.

Can be used directly:

```python
from aiobotocore.session import Session

from types_aiobotocore_cloudtrail.paginator import ListTagsPaginator

def get_list_tags_paginator() -> ListTagsPaginator:
    return Session().create_client("cloudtrail").get_paginator("list_tags")
```

Boto3 documentation:
[CloudTrail.Paginator.ListTags](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudtrail.html#CloudTrail.Paginator.ListTags)

Arguments for `ListTagsPaginator.paginate` method:

- `ResourceIdList`: `Sequence`\[`str`\] *(required)*
- `PaginationConfig`:
  [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)

`ListTagsPaginator.paginate` returns
`_PageIterator`\[[ListTagsResponseTypeDef](./type_defs.md#listtagsresponsetypedef)\].

<a id="listtrailspaginator"></a>

## ListTrailsPaginator

Type annotations for
`aiobotocore.create_client("cloudtrail").get_paginator("list_trails")`.

Can be used directly:

```python
from aiobotocore.session import Session

from types_aiobotocore_cloudtrail.paginator import ListTrailsPaginator

def get_list_trails_paginator() -> ListTrailsPaginator:
    return Session().create_client("cloudtrail").get_paginator("list_trails")
```

Boto3 documentation:
[CloudTrail.Paginator.ListTrails](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudtrail.html#CloudTrail.Paginator.ListTrails)

Arguments for `ListTrailsPaginator.paginate` method:

- `PaginationConfig`:
  [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)

`ListTrailsPaginator.paginate` returns
`_PageIterator`\[[ListTrailsResponseTypeDef](./type_defs.md#listtrailsresponsetypedef)\].

<a id="lookupeventspaginator"></a>

## LookupEventsPaginator

Type annotations for
`aiobotocore.create_client("cloudtrail").get_paginator("lookup_events")`.

Can be used directly:

```python
from aiobotocore.session import Session

from types_aiobotocore_cloudtrail.paginator import LookupEventsPaginator

def get_lookup_events_paginator() -> LookupEventsPaginator:
    return Session().create_client("cloudtrail").get_paginator("lookup_events")
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
`_PageIterator`\[[LookupEventsResponseTypeDef](./type_defs.md#lookupeventsresponsetypedef)\].
