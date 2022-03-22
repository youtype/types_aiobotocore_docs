<a id="paginators-for-aiobotocore-servicequotas-module"></a>

# Paginators for aiobotocore ServiceQuotas module

> [Index](../README.md) > [ServiceQuotas](./README.md) > Paginators

Auto-generated documentation for
[ServiceQuotas](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/service-quotas.html#ServiceQuotas)
type annotations stubs module
[types-aiobotocore-service-quotas](https://pypi.org/project/types-aiobotocore-service-quotas/).

- [Paginators for aiobotocore ServiceQuotas module](#paginators-for-aiobotocore-servicequotas-module)
  - [ListAWSDefaultServiceQuotasPaginator](#listawsdefaultservicequotaspaginator)
  - [ListRequestedServiceQuotaChangeHistoryPaginator](#listrequestedservicequotachangehistorypaginator)
  - [ListRequestedServiceQuotaChangeHistoryByQuotaPaginator](#listrequestedservicequotachangehistorybyquotapaginator)
  - [ListServiceQuotaIncreaseRequestsInTemplatePaginator](#listservicequotaincreaserequestsintemplatepaginator)
  - [ListServiceQuotasPaginator](#listservicequotaspaginator)
  - [ListServicesPaginator](#listservicespaginator)

<a id="listawsdefaultservicequotaspaginator"></a>

## ListAWSDefaultServiceQuotasPaginator

Type annotations for
`session.create_client("service-quotas").get_paginator("list_aws_default_service_quotas")`.

Can be used directly:

```python
from aiobotocore.session import get_session

from types_aiobotocore_service_quotas.paginator import ListAWSDefaultServiceQuotasPaginator

session = get_session()
async with session.create_client("service-quotas") as client:
    client: ServiceQuotasClient
    paginator: ListAWSDefaultServiceQuotasPaginator = client.get_paginator("list_aws_default_service_quotas")
```

Boto3 documentation:
[ServiceQuotas.Paginator.ListAWSDefaultServiceQuotas](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/service-quotas.html#ServiceQuotas.Paginator.ListAWSDefaultServiceQuotas)

Arguments for `ListAWSDefaultServiceQuotasPaginator.paginate` method:

- `ServiceCode`: `str` *(required)*
- `PaginationConfig`:
  [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)

`ListAWSDefaultServiceQuotasPaginator.paginate` returns
`AsyncIterator`\[[ListAWSDefaultServiceQuotasResponseTypeDef](./type_defs.md#listawsdefaultservicequotasresponsetypedef)\].

<a id="listrequestedservicequotachangehistorypaginator"></a>

## ListRequestedServiceQuotaChangeHistoryPaginator

Type annotations for
`session.create_client("service-quotas").get_paginator("list_requested_service_quota_change_history")`.

Can be used directly:

```python
from aiobotocore.session import get_session

from types_aiobotocore_service_quotas.paginator import ListRequestedServiceQuotaChangeHistoryPaginator

session = get_session()
async with session.create_client("service-quotas") as client:
    client: ServiceQuotasClient
    paginator: ListRequestedServiceQuotaChangeHistoryPaginator = client.get_paginator("list_requested_service_quota_change_history")
```

Boto3 documentation:
[ServiceQuotas.Paginator.ListRequestedServiceQuotaChangeHistory](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/service-quotas.html#ServiceQuotas.Paginator.ListRequestedServiceQuotaChangeHistory)

Arguments for `ListRequestedServiceQuotaChangeHistoryPaginator.paginate`
method:

- `ServiceCode`: `str`
- `Status`: [RequestStatusType](./literals.md#requeststatustype)
- `PaginationConfig`:
  [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)

`ListRequestedServiceQuotaChangeHistoryPaginator.paginate` returns
`AsyncIterator`\[[ListRequestedServiceQuotaChangeHistoryResponseTypeDef](./type_defs.md#listrequestedservicequotachangehistoryresponsetypedef)\].

<a id="listrequestedservicequotachangehistorybyquotapaginator"></a>

## ListRequestedServiceQuotaChangeHistoryByQuotaPaginator

Type annotations for
`session.create_client("service-quotas").get_paginator("list_requested_service_quota_change_history_by_quota")`.

Can be used directly:

```python
from aiobotocore.session import get_session

from types_aiobotocore_service_quotas.paginator import ListRequestedServiceQuotaChangeHistoryByQuotaPaginator

session = get_session()
async with session.create_client("service-quotas") as client:
    client: ServiceQuotasClient
    paginator: ListRequestedServiceQuotaChangeHistoryByQuotaPaginator = client.get_paginator("list_requested_service_quota_change_history_by_quota")
```

Boto3 documentation:
[ServiceQuotas.Paginator.ListRequestedServiceQuotaChangeHistoryByQuota](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/service-quotas.html#ServiceQuotas.Paginator.ListRequestedServiceQuotaChangeHistoryByQuota)

Arguments for `ListRequestedServiceQuotaChangeHistoryByQuotaPaginator.paginate`
method:

- `ServiceCode`: `str` *(required)*
- `QuotaCode`: `str` *(required)*
- `Status`: [RequestStatusType](./literals.md#requeststatustype)
- `PaginationConfig`:
  [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)

`ListRequestedServiceQuotaChangeHistoryByQuotaPaginator.paginate` returns
`AsyncIterator`\[[ListRequestedServiceQuotaChangeHistoryByQuotaResponseTypeDef](./type_defs.md#listrequestedservicequotachangehistorybyquotaresponsetypedef)\].

<a id="listservicequotaincreaserequestsintemplatepaginator"></a>

## ListServiceQuotaIncreaseRequestsInTemplatePaginator

Type annotations for
`session.create_client("service-quotas").get_paginator("list_service_quota_increase_requests_in_template")`.

Can be used directly:

```python
from aiobotocore.session import get_session

from types_aiobotocore_service_quotas.paginator import ListServiceQuotaIncreaseRequestsInTemplatePaginator

session = get_session()
async with session.create_client("service-quotas") as client:
    client: ServiceQuotasClient
    paginator: ListServiceQuotaIncreaseRequestsInTemplatePaginator = client.get_paginator("list_service_quota_increase_requests_in_template")
```

Boto3 documentation:
[ServiceQuotas.Paginator.ListServiceQuotaIncreaseRequestsInTemplate](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/service-quotas.html#ServiceQuotas.Paginator.ListServiceQuotaIncreaseRequestsInTemplate)

Arguments for `ListServiceQuotaIncreaseRequestsInTemplatePaginator.paginate`
method:

- `ServiceCode`: `str`
- `AwsRegion`: `str`
- `PaginationConfig`:
  [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)

`ListServiceQuotaIncreaseRequestsInTemplatePaginator.paginate` returns
`AsyncIterator`\[[ListServiceQuotaIncreaseRequestsInTemplateResponseTypeDef](./type_defs.md#listservicequotaincreaserequestsintemplateresponsetypedef)\].

<a id="listservicequotaspaginator"></a>

## ListServiceQuotasPaginator

Type annotations for
`session.create_client("service-quotas").get_paginator("list_service_quotas")`.

Can be used directly:

```python
from aiobotocore.session import get_session

from types_aiobotocore_service_quotas.paginator import ListServiceQuotasPaginator

session = get_session()
async with session.create_client("service-quotas") as client:
    client: ServiceQuotasClient
    paginator: ListServiceQuotasPaginator = client.get_paginator("list_service_quotas")
```

Boto3 documentation:
[ServiceQuotas.Paginator.ListServiceQuotas](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/service-quotas.html#ServiceQuotas.Paginator.ListServiceQuotas)

Arguments for `ListServiceQuotasPaginator.paginate` method:

- `ServiceCode`: `str` *(required)*
- `PaginationConfig`:
  [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)

`ListServiceQuotasPaginator.paginate` returns
`AsyncIterator`\[[ListServiceQuotasResponseTypeDef](./type_defs.md#listservicequotasresponsetypedef)\].

<a id="listservicespaginator"></a>

## ListServicesPaginator

Type annotations for
`session.create_client("service-quotas").get_paginator("list_services")`.

Can be used directly:

```python
from aiobotocore.session import get_session

from types_aiobotocore_service_quotas.paginator import ListServicesPaginator

session = get_session()
async with session.create_client("service-quotas") as client:
    client: ServiceQuotasClient
    paginator: ListServicesPaginator = client.get_paginator("list_services")
```

Boto3 documentation:
[ServiceQuotas.Paginator.ListServices](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/service-quotas.html#ServiceQuotas.Paginator.ListServices)

Arguments for `ListServicesPaginator.paginate` method:

- `PaginationConfig`:
  [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)

`ListServicesPaginator.paginate` returns
`AsyncIterator`\[[ListServicesResponseTypeDef](./type_defs.md#listservicesresponsetypedef)\].
