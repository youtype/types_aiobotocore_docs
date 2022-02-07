<a id="paginators-for-aiobotocore-pinpointemail-module"></a>

# Paginators for aiobotocore PinpointEmail module

> [Index](..) > [PinpointEmail](.) > Paginators

Auto-generated documentation for
[PinpointEmail](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pinpoint-email.html#PinpointEmail)
type annotations stubs module
[types-aiobotocore-pinpoint-email](https://pypi.org/project/types-aiobotocore-pinpoint-email/).

- [Paginators for aiobotocore PinpointEmail module](#paginators-for-aiobotocore-pinpointemail-module)
  - [GetDedicatedIpsPaginator](#getdedicatedipspaginator)
  - [ListConfigurationSetsPaginator](#listconfigurationsetspaginator)
  - [ListDedicatedIpPoolsPaginator](#listdedicatedippoolspaginator)
  - [ListDeliverabilityTestReportsPaginator](#listdeliverabilitytestreportspaginator)
  - [ListEmailIdentitiesPaginator](#listemailidentitiespaginator)

<a id="getdedicatedipspaginator"></a>

## GetDedicatedIpsPaginator

Type annotations for
`session.create_client("pinpoint-email").get_paginator("get_dedicated_ips")`.

Can be used directly:

```python
from aiobotocore.session import get_session

from types_aiobotocore_pinpoint_email.paginator import GetDedicatedIpsPaginator

session = get_session()
async with session.create_client("pinpoint-email") as client:
    client: PinpointEmailClient
    paginator: GetDedicatedIpsPaginator = client.get_paginator("get_dedicated_ips")
```

Boto3 documentation:
[PinpointEmail.Paginator.GetDedicatedIps](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pinpoint-email.html#PinpointEmail.Paginator.GetDedicatedIps)

Arguments for `GetDedicatedIpsPaginator.paginate` method:

- `PoolName`: `str`
- `PaginationConfig`:
  [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)

`GetDedicatedIpsPaginator.paginate` returns
`_PageIterator`\[[GetDedicatedIpsResponseTypeDef](./type_defs.md#getdedicatedipsresponsetypedef)\].

<a id="listconfigurationsetspaginator"></a>

## ListConfigurationSetsPaginator

Type annotations for
`session.create_client("pinpoint-email").get_paginator("list_configuration_sets")`.

Can be used directly:

```python
from aiobotocore.session import get_session

from types_aiobotocore_pinpoint_email.paginator import ListConfigurationSetsPaginator

session = get_session()
async with session.create_client("pinpoint-email") as client:
    client: PinpointEmailClient
    paginator: ListConfigurationSetsPaginator = client.get_paginator("list_configuration_sets")
```

Boto3 documentation:
[PinpointEmail.Paginator.ListConfigurationSets](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pinpoint-email.html#PinpointEmail.Paginator.ListConfigurationSets)

Arguments for `ListConfigurationSetsPaginator.paginate` method:

- `PaginationConfig`:
  [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)

`ListConfigurationSetsPaginator.paginate` returns
`_PageIterator`\[[ListConfigurationSetsResponseTypeDef](./type_defs.md#listconfigurationsetsresponsetypedef)\].

<a id="listdedicatedippoolspaginator"></a>

## ListDedicatedIpPoolsPaginator

Type annotations for
`session.create_client("pinpoint-email").get_paginator("list_dedicated_ip_pools")`.

Can be used directly:

```python
from aiobotocore.session import get_session

from types_aiobotocore_pinpoint_email.paginator import ListDedicatedIpPoolsPaginator

session = get_session()
async with session.create_client("pinpoint-email") as client:
    client: PinpointEmailClient
    paginator: ListDedicatedIpPoolsPaginator = client.get_paginator("list_dedicated_ip_pools")
```

Boto3 documentation:
[PinpointEmail.Paginator.ListDedicatedIpPools](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pinpoint-email.html#PinpointEmail.Paginator.ListDedicatedIpPools)

Arguments for `ListDedicatedIpPoolsPaginator.paginate` method:

- `PaginationConfig`:
  [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)

`ListDedicatedIpPoolsPaginator.paginate` returns
`_PageIterator`\[[ListDedicatedIpPoolsResponseTypeDef](./type_defs.md#listdedicatedippoolsresponsetypedef)\].

<a id="listdeliverabilitytestreportspaginator"></a>

## ListDeliverabilityTestReportsPaginator

Type annotations for
`session.create_client("pinpoint-email").get_paginator("list_deliverability_test_reports")`.

Can be used directly:

```python
from aiobotocore.session import get_session

from types_aiobotocore_pinpoint_email.paginator import ListDeliverabilityTestReportsPaginator

session = get_session()
async with session.create_client("pinpoint-email") as client:
    client: PinpointEmailClient
    paginator: ListDeliverabilityTestReportsPaginator = client.get_paginator("list_deliverability_test_reports")
```

Boto3 documentation:
[PinpointEmail.Paginator.ListDeliverabilityTestReports](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pinpoint-email.html#PinpointEmail.Paginator.ListDeliverabilityTestReports)

Arguments for `ListDeliverabilityTestReportsPaginator.paginate` method:

- `PaginationConfig`:
  [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)

`ListDeliverabilityTestReportsPaginator.paginate` returns
`_PageIterator`\[[ListDeliverabilityTestReportsResponseTypeDef](./type_defs.md#listdeliverabilitytestreportsresponsetypedef)\].

<a id="listemailidentitiespaginator"></a>

## ListEmailIdentitiesPaginator

Type annotations for
`session.create_client("pinpoint-email").get_paginator("list_email_identities")`.

Can be used directly:

```python
from aiobotocore.session import get_session

from types_aiobotocore_pinpoint_email.paginator import ListEmailIdentitiesPaginator

session = get_session()
async with session.create_client("pinpoint-email") as client:
    client: PinpointEmailClient
    paginator: ListEmailIdentitiesPaginator = client.get_paginator("list_email_identities")
```

Boto3 documentation:
[PinpointEmail.Paginator.ListEmailIdentities](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pinpoint-email.html#PinpointEmail.Paginator.ListEmailIdentities)

Arguments for `ListEmailIdentitiesPaginator.paginate` method:

- `PaginationConfig`:
  [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)

`ListEmailIdentitiesPaginator.paginate` returns
`_PageIterator`\[[ListEmailIdentitiesResponseTypeDef](./type_defs.md#listemailidentitiesresponsetypedef)\].
