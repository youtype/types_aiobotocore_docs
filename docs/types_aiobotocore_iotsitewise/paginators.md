<a id="paginators-for-aiobotocore-iotsitewise-module"></a>

# Paginators for aiobotocore IoTSiteWise module

> [Index](../README.md) > [IoTSiteWise](./README.md) > Paginators

Auto-generated documentation for
[IoTSiteWise](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotsitewise.html#IoTSiteWise)
type annotations stubs module
[types-aiobotocore-iotsitewise](https://pypi.org/project/types-aiobotocore-iotsitewise/).

- [Paginators for aiobotocore IoTSiteWise module](#paginators-for-aiobotocore-iotsitewise-module)
  - [GetAssetPropertyAggregatesPaginator](#getassetpropertyaggregatespaginator)
  - [GetAssetPropertyValueHistoryPaginator](#getassetpropertyvaluehistorypaginator)
  - [GetInterpolatedAssetPropertyValuesPaginator](#getinterpolatedassetpropertyvaluespaginator)
  - [ListAccessPoliciesPaginator](#listaccesspoliciespaginator)
  - [ListAssetModelsPaginator](#listassetmodelspaginator)
  - [ListAssetRelationshipsPaginator](#listassetrelationshipspaginator)
  - [ListAssetsPaginator](#listassetspaginator)
  - [ListAssociatedAssetsPaginator](#listassociatedassetspaginator)
  - [ListDashboardsPaginator](#listdashboardspaginator)
  - [ListGatewaysPaginator](#listgatewayspaginator)
  - [ListPortalsPaginator](#listportalspaginator)
  - [ListProjectAssetsPaginator](#listprojectassetspaginator)
  - [ListProjectsPaginator](#listprojectspaginator)
  - [ListTimeSeriesPaginator](#listtimeseriespaginator)

<a id="getassetpropertyaggregatespaginator"></a>

## GetAssetPropertyAggregatesPaginator

Type annotations for
`session.create_client("iotsitewise").get_paginator("get_asset_property_aggregates")`.

Can be used directly:

```python
from aiobotocore.session import get_session

from types_aiobotocore_iotsitewise.paginator import GetAssetPropertyAggregatesPaginator

session = get_session()
async with session.create_client("iotsitewise") as client:
    client: IoTSiteWiseClient
    paginator: GetAssetPropertyAggregatesPaginator = client.get_paginator("get_asset_property_aggregates")
```

Boto3 documentation:
[IoTSiteWise.Paginator.GetAssetPropertyAggregates](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotsitewise.html#IoTSiteWise.Paginator.GetAssetPropertyAggregates)

Arguments for `GetAssetPropertyAggregatesPaginator.paginate` method:

- `aggregateTypes`:
  `Sequence`\[[AggregateTypeType](./literals.md#aggregatetypetype)\]
  *(required)*
- `resolution`: `str` *(required)*
- `startDate`: `Union`\[`datetime`, `str`\] *(required)*
- `endDate`: `Union`\[`datetime`, `str`\] *(required)*
- `assetId`: `str`
- `propertyId`: `str`
- `propertyAlias`: `str`
- `qualities`: `Sequence`\[[QualityType](./literals.md#qualitytype)\]
- `timeOrdering`: [TimeOrderingType](./literals.md#timeorderingtype)
- `PaginationConfig`:
  [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)

`GetAssetPropertyAggregatesPaginator.paginate` returns
`AsyncIterator`\[[GetAssetPropertyAggregatesResponseTypeDef](./type_defs.md#getassetpropertyaggregatesresponsetypedef)\].

<a id="getassetpropertyvaluehistorypaginator"></a>

## GetAssetPropertyValueHistoryPaginator

Type annotations for
`session.create_client("iotsitewise").get_paginator("get_asset_property_value_history")`.

Can be used directly:

```python
from aiobotocore.session import get_session

from types_aiobotocore_iotsitewise.paginator import GetAssetPropertyValueHistoryPaginator

session = get_session()
async with session.create_client("iotsitewise") as client:
    client: IoTSiteWiseClient
    paginator: GetAssetPropertyValueHistoryPaginator = client.get_paginator("get_asset_property_value_history")
```

Boto3 documentation:
[IoTSiteWise.Paginator.GetAssetPropertyValueHistory](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotsitewise.html#IoTSiteWise.Paginator.GetAssetPropertyValueHistory)

Arguments for `GetAssetPropertyValueHistoryPaginator.paginate` method:

- `assetId`: `str`
- `propertyId`: `str`
- `propertyAlias`: `str`
- `startDate`: `Union`\[`datetime`, `str`\]
- `endDate`: `Union`\[`datetime`, `str`\]
- `qualities`: `Sequence`\[[QualityType](./literals.md#qualitytype)\]
- `timeOrdering`: [TimeOrderingType](./literals.md#timeorderingtype)
- `PaginationConfig`:
  [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)

`GetAssetPropertyValueHistoryPaginator.paginate` returns
`AsyncIterator`\[[GetAssetPropertyValueHistoryResponseTypeDef](./type_defs.md#getassetpropertyvaluehistoryresponsetypedef)\].

<a id="getinterpolatedassetpropertyvaluespaginator"></a>

## GetInterpolatedAssetPropertyValuesPaginator

Type annotations for
`session.create_client("iotsitewise").get_paginator("get_interpolated_asset_property_values")`.

Can be used directly:

```python
from aiobotocore.session import get_session

from types_aiobotocore_iotsitewise.paginator import GetInterpolatedAssetPropertyValuesPaginator

session = get_session()
async with session.create_client("iotsitewise") as client:
    client: IoTSiteWiseClient
    paginator: GetInterpolatedAssetPropertyValuesPaginator = client.get_paginator("get_interpolated_asset_property_values")
```

Boto3 documentation:
[IoTSiteWise.Paginator.GetInterpolatedAssetPropertyValues](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotsitewise.html#IoTSiteWise.Paginator.GetInterpolatedAssetPropertyValues)

Arguments for `GetInterpolatedAssetPropertyValuesPaginator.paginate` method:

- `startTimeInSeconds`: `int` *(required)*
- `endTimeInSeconds`: `int` *(required)*
- `quality`: [QualityType](./literals.md#qualitytype) *(required)*
- `intervalInSeconds`: `int` *(required)*
- `type`: `str` *(required)*
- `assetId`: `str`
- `propertyId`: `str`
- `propertyAlias`: `str`
- `startTimeOffsetInNanos`: `int`
- `endTimeOffsetInNanos`: `int`
- `intervalWindowInSeconds`: `int`
- `PaginationConfig`:
  [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)

`GetInterpolatedAssetPropertyValuesPaginator.paginate` returns
`AsyncIterator`\[[GetInterpolatedAssetPropertyValuesResponseTypeDef](./type_defs.md#getinterpolatedassetpropertyvaluesresponsetypedef)\].

<a id="listaccesspoliciespaginator"></a>

## ListAccessPoliciesPaginator

Type annotations for
`session.create_client("iotsitewise").get_paginator("list_access_policies")`.

Can be used directly:

```python
from aiobotocore.session import get_session

from types_aiobotocore_iotsitewise.paginator import ListAccessPoliciesPaginator

session = get_session()
async with session.create_client("iotsitewise") as client:
    client: IoTSiteWiseClient
    paginator: ListAccessPoliciesPaginator = client.get_paginator("list_access_policies")
```

Boto3 documentation:
[IoTSiteWise.Paginator.ListAccessPolicies](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotsitewise.html#IoTSiteWise.Paginator.ListAccessPolicies)

Arguments for `ListAccessPoliciesPaginator.paginate` method:

- `identityType`: [IdentityTypeType](./literals.md#identitytypetype)
- `identityId`: `str`
- `resourceType`: [ResourceTypeType](./literals.md#resourcetypetype)
- `resourceId`: `str`
- `iamArn`: `str`
- `PaginationConfig`:
  [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)

`ListAccessPoliciesPaginator.paginate` returns
`AsyncIterator`\[[ListAccessPoliciesResponseTypeDef](./type_defs.md#listaccesspoliciesresponsetypedef)\].

<a id="listassetmodelspaginator"></a>

## ListAssetModelsPaginator

Type annotations for
`session.create_client("iotsitewise").get_paginator("list_asset_models")`.

Can be used directly:

```python
from aiobotocore.session import get_session

from types_aiobotocore_iotsitewise.paginator import ListAssetModelsPaginator

session = get_session()
async with session.create_client("iotsitewise") as client:
    client: IoTSiteWiseClient
    paginator: ListAssetModelsPaginator = client.get_paginator("list_asset_models")
```

Boto3 documentation:
[IoTSiteWise.Paginator.ListAssetModels](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotsitewise.html#IoTSiteWise.Paginator.ListAssetModels)

Arguments for `ListAssetModelsPaginator.paginate` method:

- `PaginationConfig`:
  [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)

`ListAssetModelsPaginator.paginate` returns
`AsyncIterator`\[[ListAssetModelsResponseTypeDef](./type_defs.md#listassetmodelsresponsetypedef)\].

<a id="listassetrelationshipspaginator"></a>

## ListAssetRelationshipsPaginator

Type annotations for
`session.create_client("iotsitewise").get_paginator("list_asset_relationships")`.

Can be used directly:

```python
from aiobotocore.session import get_session

from types_aiobotocore_iotsitewise.paginator import ListAssetRelationshipsPaginator

session = get_session()
async with session.create_client("iotsitewise") as client:
    client: IoTSiteWiseClient
    paginator: ListAssetRelationshipsPaginator = client.get_paginator("list_asset_relationships")
```

Boto3 documentation:
[IoTSiteWise.Paginator.ListAssetRelationships](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotsitewise.html#IoTSiteWise.Paginator.ListAssetRelationships)

Arguments for `ListAssetRelationshipsPaginator.paginate` method:

- `assetId`: `str` *(required)*
- `traversalType`: `Literal['PATH_TO_ROOT']` (see
  [TraversalTypeType](./literals.md#traversaltypetype)) *(required)*
- `PaginationConfig`:
  [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)

`ListAssetRelationshipsPaginator.paginate` returns
`AsyncIterator`\[[ListAssetRelationshipsResponseTypeDef](./type_defs.md#listassetrelationshipsresponsetypedef)\].

<a id="listassetspaginator"></a>

## ListAssetsPaginator

Type annotations for
`session.create_client("iotsitewise").get_paginator("list_assets")`.

Can be used directly:

```python
from aiobotocore.session import get_session

from types_aiobotocore_iotsitewise.paginator import ListAssetsPaginator

session = get_session()
async with session.create_client("iotsitewise") as client:
    client: IoTSiteWiseClient
    paginator: ListAssetsPaginator = client.get_paginator("list_assets")
```

Boto3 documentation:
[IoTSiteWise.Paginator.ListAssets](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotsitewise.html#IoTSiteWise.Paginator.ListAssets)

Arguments for `ListAssetsPaginator.paginate` method:

- `assetModelId`: `str`
- `filter`: [ListAssetsFilterType](./literals.md#listassetsfiltertype)
- `PaginationConfig`:
  [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)

`ListAssetsPaginator.paginate` returns
`AsyncIterator`\[[ListAssetsResponseTypeDef](./type_defs.md#listassetsresponsetypedef)\].

<a id="listassociatedassetspaginator"></a>

## ListAssociatedAssetsPaginator

Type annotations for
`session.create_client("iotsitewise").get_paginator("list_associated_assets")`.

Can be used directly:

```python
from aiobotocore.session import get_session

from types_aiobotocore_iotsitewise.paginator import ListAssociatedAssetsPaginator

session = get_session()
async with session.create_client("iotsitewise") as client:
    client: IoTSiteWiseClient
    paginator: ListAssociatedAssetsPaginator = client.get_paginator("list_associated_assets")
```

Boto3 documentation:
[IoTSiteWise.Paginator.ListAssociatedAssets](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotsitewise.html#IoTSiteWise.Paginator.ListAssociatedAssets)

Arguments for `ListAssociatedAssetsPaginator.paginate` method:

- `assetId`: `str` *(required)*
- `hierarchyId`: `str`
- `traversalDirection`:
  [TraversalDirectionType](./literals.md#traversaldirectiontype)
- `PaginationConfig`:
  [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)

`ListAssociatedAssetsPaginator.paginate` returns
`AsyncIterator`\[[ListAssociatedAssetsResponseTypeDef](./type_defs.md#listassociatedassetsresponsetypedef)\].

<a id="listdashboardspaginator"></a>

## ListDashboardsPaginator

Type annotations for
`session.create_client("iotsitewise").get_paginator("list_dashboards")`.

Can be used directly:

```python
from aiobotocore.session import get_session

from types_aiobotocore_iotsitewise.paginator import ListDashboardsPaginator

session = get_session()
async with session.create_client("iotsitewise") as client:
    client: IoTSiteWiseClient
    paginator: ListDashboardsPaginator = client.get_paginator("list_dashboards")
```

Boto3 documentation:
[IoTSiteWise.Paginator.ListDashboards](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotsitewise.html#IoTSiteWise.Paginator.ListDashboards)

Arguments for `ListDashboardsPaginator.paginate` method:

- `projectId`: `str` *(required)*
- `PaginationConfig`:
  [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)

`ListDashboardsPaginator.paginate` returns
`AsyncIterator`\[[ListDashboardsResponseTypeDef](./type_defs.md#listdashboardsresponsetypedef)\].

<a id="listgatewayspaginator"></a>

## ListGatewaysPaginator

Type annotations for
`session.create_client("iotsitewise").get_paginator("list_gateways")`.

Can be used directly:

```python
from aiobotocore.session import get_session

from types_aiobotocore_iotsitewise.paginator import ListGatewaysPaginator

session = get_session()
async with session.create_client("iotsitewise") as client:
    client: IoTSiteWiseClient
    paginator: ListGatewaysPaginator = client.get_paginator("list_gateways")
```

Boto3 documentation:
[IoTSiteWise.Paginator.ListGateways](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotsitewise.html#IoTSiteWise.Paginator.ListGateways)

Arguments for `ListGatewaysPaginator.paginate` method:

- `PaginationConfig`:
  [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)

`ListGatewaysPaginator.paginate` returns
`AsyncIterator`\[[ListGatewaysResponseTypeDef](./type_defs.md#listgatewaysresponsetypedef)\].

<a id="listportalspaginator"></a>

## ListPortalsPaginator

Type annotations for
`session.create_client("iotsitewise").get_paginator("list_portals")`.

Can be used directly:

```python
from aiobotocore.session import get_session

from types_aiobotocore_iotsitewise.paginator import ListPortalsPaginator

session = get_session()
async with session.create_client("iotsitewise") as client:
    client: IoTSiteWiseClient
    paginator: ListPortalsPaginator = client.get_paginator("list_portals")
```

Boto3 documentation:
[IoTSiteWise.Paginator.ListPortals](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotsitewise.html#IoTSiteWise.Paginator.ListPortals)

Arguments for `ListPortalsPaginator.paginate` method:

- `PaginationConfig`:
  [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)

`ListPortalsPaginator.paginate` returns
`AsyncIterator`\[[ListPortalsResponseTypeDef](./type_defs.md#listportalsresponsetypedef)\].

<a id="listprojectassetspaginator"></a>

## ListProjectAssetsPaginator

Type annotations for
`session.create_client("iotsitewise").get_paginator("list_project_assets")`.

Can be used directly:

```python
from aiobotocore.session import get_session

from types_aiobotocore_iotsitewise.paginator import ListProjectAssetsPaginator

session = get_session()
async with session.create_client("iotsitewise") as client:
    client: IoTSiteWiseClient
    paginator: ListProjectAssetsPaginator = client.get_paginator("list_project_assets")
```

Boto3 documentation:
[IoTSiteWise.Paginator.ListProjectAssets](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotsitewise.html#IoTSiteWise.Paginator.ListProjectAssets)

Arguments for `ListProjectAssetsPaginator.paginate` method:

- `projectId`: `str` *(required)*
- `PaginationConfig`:
  [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)

`ListProjectAssetsPaginator.paginate` returns
`AsyncIterator`\[[ListProjectAssetsResponseTypeDef](./type_defs.md#listprojectassetsresponsetypedef)\].

<a id="listprojectspaginator"></a>

## ListProjectsPaginator

Type annotations for
`session.create_client("iotsitewise").get_paginator("list_projects")`.

Can be used directly:

```python
from aiobotocore.session import get_session

from types_aiobotocore_iotsitewise.paginator import ListProjectsPaginator

session = get_session()
async with session.create_client("iotsitewise") as client:
    client: IoTSiteWiseClient
    paginator: ListProjectsPaginator = client.get_paginator("list_projects")
```

Boto3 documentation:
[IoTSiteWise.Paginator.ListProjects](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotsitewise.html#IoTSiteWise.Paginator.ListProjects)

Arguments for `ListProjectsPaginator.paginate` method:

- `portalId`: `str` *(required)*
- `PaginationConfig`:
  [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)

`ListProjectsPaginator.paginate` returns
`AsyncIterator`\[[ListProjectsResponseTypeDef](./type_defs.md#listprojectsresponsetypedef)\].

<a id="listtimeseriespaginator"></a>

## ListTimeSeriesPaginator

Type annotations for
`session.create_client("iotsitewise").get_paginator("list_time_series")`.

Can be used directly:

```python
from aiobotocore.session import get_session

from types_aiobotocore_iotsitewise.paginator import ListTimeSeriesPaginator

session = get_session()
async with session.create_client("iotsitewise") as client:
    client: IoTSiteWiseClient
    paginator: ListTimeSeriesPaginator = client.get_paginator("list_time_series")
```

Boto3 documentation:
[IoTSiteWise.Paginator.ListTimeSeries](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotsitewise.html#IoTSiteWise.Paginator.ListTimeSeries)

Arguments for `ListTimeSeriesPaginator.paginate` method:

- `assetId`: `str`
- `aliasPrefix`: `str`
- `timeSeriesType`:
  [ListTimeSeriesTypeType](./literals.md#listtimeseriestypetype)
- `PaginationConfig`:
  [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)

`ListTimeSeriesPaginator.paginate` returns
`AsyncIterator`\[[ListTimeSeriesResponseTypeDef](./type_defs.md#listtimeseriesresponsetypedef)\].
