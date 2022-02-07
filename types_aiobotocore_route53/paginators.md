<a id="paginators-for-aiobotocore-route53-module"></a>

# Paginators for aiobotocore Route53 module

> [Index](..) > [Route53](.) > Paginators

Auto-generated documentation for
[Route53](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53.html#Route53)
type annotations stubs module
[types-aiobotocore-route53](https://pypi.org/project/types-aiobotocore-route53/).

- [Paginators for aiobotocore Route53 module](#paginators-for-aiobotocore-route53-module)
  - [ListHealthChecksPaginator](#listhealthcheckspaginator)
  - [ListHostedZonesPaginator](#listhostedzonespaginator)
  - [ListQueryLoggingConfigsPaginator](#listqueryloggingconfigspaginator)
  - [ListResourceRecordSetsPaginator](#listresourcerecordsetspaginator)
  - [ListVPCAssociationAuthorizationsPaginator](#listvpcassociationauthorizationspaginator)

<a id="listhealthcheckspaginator"></a>

## ListHealthChecksPaginator

Type annotations for
`session.create_client("route53").get_paginator("list_health_checks")`.

Can be used directly:

```python
from aiobotocore.session import get_session

from types_aiobotocore_route53.paginator import ListHealthChecksPaginator

session = get_session()
async with session.create_client("route53") as client:
    client: Route53Client
    paginator: ListHealthChecksPaginator = client.get_paginator("list_health_checks")
```

Boto3 documentation:
[Route53.Paginator.ListHealthChecks](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53.html#Route53.Paginator.ListHealthChecks)

Arguments for `ListHealthChecksPaginator.paginate` method:

- `PaginationConfig`:
  [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)

`ListHealthChecksPaginator.paginate` returns
`_PageIterator`\[[ListHealthChecksResponseTypeDef](./type_defs.md#listhealthchecksresponsetypedef)\].

<a id="listhostedzonespaginator"></a>

## ListHostedZonesPaginator

Type annotations for
`session.create_client("route53").get_paginator("list_hosted_zones")`.

Can be used directly:

```python
from aiobotocore.session import get_session

from types_aiobotocore_route53.paginator import ListHostedZonesPaginator

session = get_session()
async with session.create_client("route53") as client:
    client: Route53Client
    paginator: ListHostedZonesPaginator = client.get_paginator("list_hosted_zones")
```

Boto3 documentation:
[Route53.Paginator.ListHostedZones](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53.html#Route53.Paginator.ListHostedZones)

Arguments for `ListHostedZonesPaginator.paginate` method:

- `DelegationSetId`: `str`
- `PaginationConfig`:
  [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)

`ListHostedZonesPaginator.paginate` returns
`_PageIterator`\[[ListHostedZonesResponseTypeDef](./type_defs.md#listhostedzonesresponsetypedef)\].

<a id="listqueryloggingconfigspaginator"></a>

## ListQueryLoggingConfigsPaginator

Type annotations for
`session.create_client("route53").get_paginator("list_query_logging_configs")`.

Can be used directly:

```python
from aiobotocore.session import get_session

from types_aiobotocore_route53.paginator import ListQueryLoggingConfigsPaginator

session = get_session()
async with session.create_client("route53") as client:
    client: Route53Client
    paginator: ListQueryLoggingConfigsPaginator = client.get_paginator("list_query_logging_configs")
```

Boto3 documentation:
[Route53.Paginator.ListQueryLoggingConfigs](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53.html#Route53.Paginator.ListQueryLoggingConfigs)

Arguments for `ListQueryLoggingConfigsPaginator.paginate` method:

- `HostedZoneId`: `str`
- `PaginationConfig`:
  [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)

`ListQueryLoggingConfigsPaginator.paginate` returns
`_PageIterator`\[[ListQueryLoggingConfigsResponseTypeDef](./type_defs.md#listqueryloggingconfigsresponsetypedef)\].

<a id="listresourcerecordsetspaginator"></a>

## ListResourceRecordSetsPaginator

Type annotations for
`session.create_client("route53").get_paginator("list_resource_record_sets")`.

Can be used directly:

```python
from aiobotocore.session import get_session

from types_aiobotocore_route53.paginator import ListResourceRecordSetsPaginator

session = get_session()
async with session.create_client("route53") as client:
    client: Route53Client
    paginator: ListResourceRecordSetsPaginator = client.get_paginator("list_resource_record_sets")
```

Boto3 documentation:
[Route53.Paginator.ListResourceRecordSets](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53.html#Route53.Paginator.ListResourceRecordSets)

Arguments for `ListResourceRecordSetsPaginator.paginate` method:

- `HostedZoneId`: `str` *(required)*
- `PaginationConfig`:
  [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)

`ListResourceRecordSetsPaginator.paginate` returns
`_PageIterator`\[[ListResourceRecordSetsResponseTypeDef](./type_defs.md#listresourcerecordsetsresponsetypedef)\].

<a id="listvpcassociationauthorizationspaginator"></a>

## ListVPCAssociationAuthorizationsPaginator

Type annotations for
`session.create_client("route53").get_paginator("list_vpc_association_authorizations")`.

Can be used directly:

```python
from aiobotocore.session import get_session

from types_aiobotocore_route53.paginator import ListVPCAssociationAuthorizationsPaginator

session = get_session()
async with session.create_client("route53") as client:
    client: Route53Client
    paginator: ListVPCAssociationAuthorizationsPaginator = client.get_paginator("list_vpc_association_authorizations")
```

Boto3 documentation:
[Route53.Paginator.ListVPCAssociationAuthorizations](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53.html#Route53.Paginator.ListVPCAssociationAuthorizations)

Arguments for `ListVPCAssociationAuthorizationsPaginator.paginate` method:

- `HostedZoneId`: `str` *(required)*
- `MaxResults`: `str`
- `PaginationConfig`:
  [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)

`ListVPCAssociationAuthorizationsPaginator.paginate` returns
`_PageIterator`\[[ListVPCAssociationAuthorizationsResponseTypeDef](./type_defs.md#listvpcassociationauthorizationsresponsetypedef)\].
