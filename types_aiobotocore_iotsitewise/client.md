<a id="iotsitewiseclient-for-aiobotocore-iotsitewise-module"></a>

# IoTSiteWiseClient for aiobotocore IoTSiteWise module

> [Index](..) > [IoTSiteWise](.) > IoTSiteWiseClient

Auto-generated documentation for
[IoTSiteWise](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotsitewise.html#IoTSiteWise)
type annotations stubs module
[types-aiobotocore-iotsitewise](https://pypi.org/project/types-aiobotocore-iotsitewise/).

- [IoTSiteWiseClient for aiobotocore IoTSiteWise module](#iotsitewiseclient-for-aiobotocore-iotsitewise-module)
  - [IoTSiteWiseClient](#iotsitewiseclient)
  - [Exceptions](#exceptions)
  - [Methods](#methods)
    - [exceptions](#exceptions)
    - [associate_assets](#associate_assets)
    - [associate_time_series_to_asset_property](#associate_time_series_to_asset_property)
    - [batch_associate_project_assets](#batch_associate_project_assets)
    - [batch_disassociate_project_assets](#batch_disassociate_project_assets)
    - [batch_put_asset_property_value](#batch_put_asset_property_value)
    - [can_paginate](#can_paginate)
    - [create_access_policy](#create_access_policy)
    - [create_asset](#create_asset)
    - [create_asset_model](#create_asset_model)
    - [create_dashboard](#create_dashboard)
    - [create_gateway](#create_gateway)
    - [create_portal](#create_portal)
    - [create_project](#create_project)
    - [delete_access_policy](#delete_access_policy)
    - [delete_asset](#delete_asset)
    - [delete_asset_model](#delete_asset_model)
    - [delete_dashboard](#delete_dashboard)
    - [delete_gateway](#delete_gateway)
    - [delete_portal](#delete_portal)
    - [delete_project](#delete_project)
    - [delete_time_series](#delete_time_series)
    - [describe_access_policy](#describe_access_policy)
    - [describe_asset](#describe_asset)
    - [describe_asset_model](#describe_asset_model)
    - [describe_asset_property](#describe_asset_property)
    - [describe_dashboard](#describe_dashboard)
    - [describe_default_encryption_configuration](#describe_default_encryption_configuration)
    - [describe_gateway](#describe_gateway)
    - [describe_gateway_capability_configuration](#describe_gateway_capability_configuration)
    - [describe_logging_options](#describe_logging_options)
    - [describe_portal](#describe_portal)
    - [describe_project](#describe_project)
    - [describe_storage_configuration](#describe_storage_configuration)
    - [describe_time_series](#describe_time_series)
    - [disassociate_assets](#disassociate_assets)
    - [disassociate_time_series_from_asset_property](#disassociate_time_series_from_asset_property)
    - [generate_presigned_url](#generate_presigned_url)
    - [get_asset_property_aggregates](#get_asset_property_aggregates)
    - [get_asset_property_value](#get_asset_property_value)
    - [get_asset_property_value_history](#get_asset_property_value_history)
    - [get_interpolated_asset_property_values](#get_interpolated_asset_property_values)
    - [list_access_policies](#list_access_policies)
    - [list_asset_models](#list_asset_models)
    - [list_asset_relationships](#list_asset_relationships)
    - [list_assets](#list_assets)
    - [list_associated_assets](#list_associated_assets)
    - [list_dashboards](#list_dashboards)
    - [list_gateways](#list_gateways)
    - [list_portals](#list_portals)
    - [list_project_assets](#list_project_assets)
    - [list_projects](#list_projects)
    - [list_tags_for_resource](#list_tags_for_resource)
    - [list_time_series](#list_time_series)
    - [put_default_encryption_configuration](#put_default_encryption_configuration)
    - [put_logging_options](#put_logging_options)
    - [put_storage_configuration](#put_storage_configuration)
    - [tag_resource](#tag_resource)
    - [untag_resource](#untag_resource)
    - [update_access_policy](#update_access_policy)
    - [update_asset](#update_asset)
    - [update_asset_model](#update_asset_model)
    - [update_asset_property](#update_asset_property)
    - [update_dashboard](#update_dashboard)
    - [update_gateway](#update_gateway)
    - [update_gateway_capability_configuration](#update_gateway_capability_configuration)
    - [update_portal](#update_portal)
    - [update_project](#update_project)
    - [__aenter__](#__aenter__)
    - [__aexit__](#__aexit__)
    - [get_paginator](#get_paginator)
    - [get_waiter](#get_waiter)

<a id="iotsitewiseclient"></a>

## IoTSiteWiseClient

Type annotations for `session.create_client("iotsitewise")`

Can be used directly:

```python
from aiobotocore.session import get_session
from types_aiobotocore_iotsitewise.client import IoTSiteWiseClient

session = get_session()
async with session.create_client("iotsitewise") as client:
    client: IoTSiteWiseClient
```

Boto3 documentation:
[IoTSiteWise.Client](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotsitewise.html#IoTSiteWise.Client)

<a id="exceptions"></a>

## Exceptions

`boto3` client exceptions are generated in runtime. This class can be used for
static analysis directly:

```python
from types_aiobotocore_iotsitewise.client import Exceptions

def handle_error(exc: Exceptions.ClientError) -> None:
    ...
```

Exceptions:

- `Exceptions.ClientError`
- `Exceptions.ConflictingOperationException`
- `Exceptions.InternalFailureException`
- `Exceptions.InvalidRequestException`
- `Exceptions.LimitExceededException`
- `Exceptions.ResourceAlreadyExistsException`
- `Exceptions.ResourceNotFoundException`
- `Exceptions.ServiceUnavailableException`
- `Exceptions.ThrottlingException`
- `Exceptions.TooManyTagsException`
- `Exceptions.UnauthorizedException`

<a id="methods"></a>

## Methods

<a id="exceptions"></a>

### exceptions

IoTSiteWiseClient exceptions.

Type annotations for `session.create_client("iotsitewise").exceptions` method.

Boto3 documentation:
[IoTSiteWise.Client.exceptions](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotsitewise.html#IoTSiteWise.Client.exceptions)

Returns [Exceptions](#exceptions).

<a id="associate_assets"></a>

### associate_assets

Associates a child asset with the given parent asset through a hierarchy
defined in the parent asset's model.

Type annotations for `session.create_client("iotsitewise").associate_assets`
method.

Boto3 documentation:
[IoTSiteWise.Client.associate_assets](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotsitewise.html#IoTSiteWise.Client.associate_assets)

Asynchronous method. Use `await associate_assets(...)` for a synchronous call.

Arguments mapping described in
[AssociateAssetsRequestRequestTypeDef](./type_defs.md#associateassetsrequestrequesttypedef).

Keyword-only arguments:

- `assetId`: `str` *(required)*
- `hierarchyId`: `str` *(required)*
- `childAssetId`: `str` *(required)*
- `clientToken`: `str`

<a id="associate_time_series_to_asset_property"></a>

### associate_time_series_to_asset_property

Associates a time series (data stream) with an asset property.

Type annotations for
`session.create_client("iotsitewise").associate_time_series_to_asset_property`
method.

Boto3 documentation:
[IoTSiteWise.Client.associate_time_series_to_asset_property](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotsitewise.html#IoTSiteWise.Client.associate_time_series_to_asset_property)

Asynchronous method. Use `await associate_time_series_to_asset_property(...)`
for a synchronous call.

Arguments mapping described in
[AssociateTimeSeriesToAssetPropertyRequestRequestTypeDef](./type_defs.md#associatetimeseriestoassetpropertyrequestrequesttypedef).

Keyword-only arguments:

- `alias`: `str` *(required)*
- `assetId`: `str` *(required)*
- `propertyId`: `str` *(required)*
- `clientToken`: `str`

<a id="batch_associate_project_assets"></a>

### batch_associate_project_assets

Associates a group (batch) of assets with an IoT SiteWise Monitor project.

Type annotations for
`session.create_client("iotsitewise").batch_associate_project_assets` method.

Boto3 documentation:
[IoTSiteWise.Client.batch_associate_project_assets](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotsitewise.html#IoTSiteWise.Client.batch_associate_project_assets)

Asynchronous method. Use `await batch_associate_project_assets(...)` for a
synchronous call.

Arguments mapping described in
[BatchAssociateProjectAssetsRequestRequestTypeDef](./type_defs.md#batchassociateprojectassetsrequestrequesttypedef).

Keyword-only arguments:

- `projectId`: `str` *(required)*
- `assetIds`: `Sequence`\[`str`\] *(required)*
- `clientToken`: `str`

Returns a `Coroutine` for
[BatchAssociateProjectAssetsResponseTypeDef](./type_defs.md#batchassociateprojectassetsresponsetypedef).

<a id="batch_disassociate_project_assets"></a>

### batch_disassociate_project_assets

Disassociates a group (batch) of assets from an IoT SiteWise Monitor project.

Type annotations for
`session.create_client("iotsitewise").batch_disassociate_project_assets`
method.

Boto3 documentation:
[IoTSiteWise.Client.batch_disassociate_project_assets](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotsitewise.html#IoTSiteWise.Client.batch_disassociate_project_assets)

Asynchronous method. Use `await batch_disassociate_project_assets(...)` for a
synchronous call.

Arguments mapping described in
[BatchDisassociateProjectAssetsRequestRequestTypeDef](./type_defs.md#batchdisassociateprojectassetsrequestrequesttypedef).

Keyword-only arguments:

- `projectId`: `str` *(required)*
- `assetIds`: `Sequence`\[`str`\] *(required)*
- `clientToken`: `str`

Returns a `Coroutine` for
[BatchDisassociateProjectAssetsResponseTypeDef](./type_defs.md#batchdisassociateprojectassetsresponsetypedef).

<a id="batch_put_asset_property_value"></a>

### batch_put_asset_property_value

Sends a list of asset property values to IoT SiteWise.

Type annotations for
`session.create_client("iotsitewise").batch_put_asset_property_value` method.

Boto3 documentation:
[IoTSiteWise.Client.batch_put_asset_property_value](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotsitewise.html#IoTSiteWise.Client.batch_put_asset_property_value)

Asynchronous method. Use `await batch_put_asset_property_value(...)` for a
synchronous call.

Arguments mapping described in
[BatchPutAssetPropertyValueRequestRequestTypeDef](./type_defs.md#batchputassetpropertyvaluerequestrequesttypedef).

Keyword-only arguments:

- `entries`:
  `Sequence`\[[PutAssetPropertyValueEntryTypeDef](./type_defs.md#putassetpropertyvalueentrytypedef)\]
  *(required)*

Returns a `Coroutine` for
[BatchPutAssetPropertyValueResponseTypeDef](./type_defs.md#batchputassetpropertyvalueresponsetypedef).

<a id="can_paginate"></a>

### can_paginate

Check if an operation can be paginated.

Type annotations for `session.create_client("iotsitewise").can_paginate`
method.

Boto3 documentation:
[IoTSiteWise.Client.can_paginate](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotsitewise.html#IoTSiteWise.Client.can_paginate)

Arguments:

- `operation_name`: `str` *(required)*

Returns `bool`.

<a id="create_access_policy"></a>

### create_access_policy

Creates an access policy that grants the specified identity (Amazon Web
Services SSO user, Amazon Web Services SSO group, or IAM user) access to the
specified IoT SiteWise Monitor portal or project resource.

Type annotations for
`session.create_client("iotsitewise").create_access_policy` method.

Boto3 documentation:
[IoTSiteWise.Client.create_access_policy](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotsitewise.html#IoTSiteWise.Client.create_access_policy)

Asynchronous method. Use `await create_access_policy(...)` for a synchronous
call.

Arguments mapping described in
[CreateAccessPolicyRequestRequestTypeDef](./type_defs.md#createaccesspolicyrequestrequesttypedef).

Keyword-only arguments:

- `accessPolicyIdentity`: [IdentityTypeDef](./type_defs.md#identitytypedef)
  *(required)*
- `accessPolicyResource`: [ResourceTypeDef](./type_defs.md#resourcetypedef)
  *(required)*
- `accessPolicyPermission`: [PermissionType](./literals.md#permissiontype)
  *(required)*
- `clientToken`: `str`
- `tags`: `Mapping`\[`str`, `str`\]

Returns a `Coroutine` for
[CreateAccessPolicyResponseTypeDef](./type_defs.md#createaccesspolicyresponsetypedef).

<a id="create_asset"></a>

### create_asset

Creates an asset from an existing asset model.

Type annotations for `session.create_client("iotsitewise").create_asset`
method.

Boto3 documentation:
[IoTSiteWise.Client.create_asset](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotsitewise.html#IoTSiteWise.Client.create_asset)

Asynchronous method. Use `await create_asset(...)` for a synchronous call.

Arguments mapping described in
[CreateAssetRequestRequestTypeDef](./type_defs.md#createassetrequestrequesttypedef).

Keyword-only arguments:

- `assetName`: `str` *(required)*
- `assetModelId`: `str` *(required)*
- `clientToken`: `str`
- `tags`: `Mapping`\[`str`, `str`\]

Returns a `Coroutine` for
[CreateAssetResponseTypeDef](./type_defs.md#createassetresponsetypedef).

<a id="create_asset_model"></a>

### create_asset_model

Creates an asset model from specified property and hierarchy definitions.

Type annotations for `session.create_client("iotsitewise").create_asset_model`
method.

Boto3 documentation:
[IoTSiteWise.Client.create_asset_model](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotsitewise.html#IoTSiteWise.Client.create_asset_model)

Asynchronous method. Use `await create_asset_model(...)` for a synchronous
call.

Arguments mapping described in
[CreateAssetModelRequestRequestTypeDef](./type_defs.md#createassetmodelrequestrequesttypedef).

Keyword-only arguments:

- `assetModelName`: `str` *(required)*
- `assetModelDescription`: `str`
- `assetModelProperties`:
  `Sequence`\[[AssetModelPropertyDefinitionTypeDef](./type_defs.md#assetmodelpropertydefinitiontypedef)\]
- `assetModelHierarchies`:
  `Sequence`\[[AssetModelHierarchyDefinitionTypeDef](./type_defs.md#assetmodelhierarchydefinitiontypedef)\]
- `assetModelCompositeModels`:
  `Sequence`\[[AssetModelCompositeModelDefinitionTypeDef](./type_defs.md#assetmodelcompositemodeldefinitiontypedef)\]
- `clientToken`: `str`
- `tags`: `Mapping`\[`str`, `str`\]

Returns a `Coroutine` for
[CreateAssetModelResponseTypeDef](./type_defs.md#createassetmodelresponsetypedef).

<a id="create_dashboard"></a>

### create_dashboard

Creates a dashboard in an IoT SiteWise Monitor project.

Type annotations for `session.create_client("iotsitewise").create_dashboard`
method.

Boto3 documentation:
[IoTSiteWise.Client.create_dashboard](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotsitewise.html#IoTSiteWise.Client.create_dashboard)

Asynchronous method. Use `await create_dashboard(...)` for a synchronous call.

Arguments mapping described in
[CreateDashboardRequestRequestTypeDef](./type_defs.md#createdashboardrequestrequesttypedef).

Keyword-only arguments:

- `projectId`: `str` *(required)*
- `dashboardName`: `str` *(required)*
- `dashboardDefinition`: `str` *(required)*
- `dashboardDescription`: `str`
- `clientToken`: `str`
- `tags`: `Mapping`\[`str`, `str`\]

Returns a `Coroutine` for
[CreateDashboardResponseTypeDef](./type_defs.md#createdashboardresponsetypedef).

<a id="create_gateway"></a>

### create_gateway

Creates a gateway, which is a virtual or edge device that delivers industrial
data streams from local servers to IoT SiteWise.

Type annotations for `session.create_client("iotsitewise").create_gateway`
method.

Boto3 documentation:
[IoTSiteWise.Client.create_gateway](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotsitewise.html#IoTSiteWise.Client.create_gateway)

Asynchronous method. Use `await create_gateway(...)` for a synchronous call.

Arguments mapping described in
[CreateGatewayRequestRequestTypeDef](./type_defs.md#creategatewayrequestrequesttypedef).

Keyword-only arguments:

- `gatewayName`: `str` *(required)*
- `gatewayPlatform`:
  [GatewayPlatformTypeDef](./type_defs.md#gatewayplatformtypedef) *(required)*
- `tags`: `Mapping`\[`str`, `str`\]

Returns a `Coroutine` for
[CreateGatewayResponseTypeDef](./type_defs.md#creategatewayresponsetypedef).

<a id="create_portal"></a>

### create_portal

Creates a portal, which can contain projects and dashboards.

Type annotations for `session.create_client("iotsitewise").create_portal`
method.

Boto3 documentation:
[IoTSiteWise.Client.create_portal](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotsitewise.html#IoTSiteWise.Client.create_portal)

Asynchronous method. Use `await create_portal(...)` for a synchronous call.

Arguments mapping described in
[CreatePortalRequestRequestTypeDef](./type_defs.md#createportalrequestrequesttypedef).

Keyword-only arguments:

- `portalName`: `str` *(required)*
- `portalContactEmail`: `str` *(required)*
- `roleArn`: `str` *(required)*
- `portalDescription`: `str`
- `clientToken`: `str`
- `portalLogoImageFile`: [ImageFileTypeDef](./type_defs.md#imagefiletypedef)
- `tags`: `Mapping`\[`str`, `str`\]
- `portalAuthMode`: [AuthModeType](./literals.md#authmodetype)
- `notificationSenderEmail`: `str`
- `alarms`: [AlarmsTypeDef](./type_defs.md#alarmstypedef)

Returns a `Coroutine` for
[CreatePortalResponseTypeDef](./type_defs.md#createportalresponsetypedef).

<a id="create_project"></a>

### create_project

Creates a project in the specified portal.

Type annotations for `session.create_client("iotsitewise").create_project`
method.

Boto3 documentation:
[IoTSiteWise.Client.create_project](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotsitewise.html#IoTSiteWise.Client.create_project)

Asynchronous method. Use `await create_project(...)` for a synchronous call.

Arguments mapping described in
[CreateProjectRequestRequestTypeDef](./type_defs.md#createprojectrequestrequesttypedef).

Keyword-only arguments:

- `portalId`: `str` *(required)*
- `projectName`: `str` *(required)*
- `projectDescription`: `str`
- `clientToken`: `str`
- `tags`: `Mapping`\[`str`, `str`\]

Returns a `Coroutine` for
[CreateProjectResponseTypeDef](./type_defs.md#createprojectresponsetypedef).

<a id="delete_access_policy"></a>

### delete_access_policy

Deletes an access policy that grants the specified identity access to the
specified IoT SiteWise Monitor resource.

Type annotations for
`session.create_client("iotsitewise").delete_access_policy` method.

Boto3 documentation:
[IoTSiteWise.Client.delete_access_policy](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotsitewise.html#IoTSiteWise.Client.delete_access_policy)

Asynchronous method. Use `await delete_access_policy(...)` for a synchronous
call.

Arguments mapping described in
[DeleteAccessPolicyRequestRequestTypeDef](./type_defs.md#deleteaccesspolicyrequestrequesttypedef).

Keyword-only arguments:

- `accessPolicyId`: `str` *(required)*
- `clientToken`: `str`

Returns a `Coroutine` for `Dict`\[`str`, `Any`\].

<a id="delete_asset"></a>

### delete_asset

Deletes an asset.

Type annotations for `session.create_client("iotsitewise").delete_asset`
method.

Boto3 documentation:
[IoTSiteWise.Client.delete_asset](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotsitewise.html#IoTSiteWise.Client.delete_asset)

Asynchronous method. Use `await delete_asset(...)` for a synchronous call.

Arguments mapping described in
[DeleteAssetRequestRequestTypeDef](./type_defs.md#deleteassetrequestrequesttypedef).

Keyword-only arguments:

- `assetId`: `str` *(required)*
- `clientToken`: `str`

Returns a `Coroutine` for
[DeleteAssetResponseTypeDef](./type_defs.md#deleteassetresponsetypedef).

<a id="delete_asset_model"></a>

### delete_asset_model

Deletes an asset model.

Type annotations for `session.create_client("iotsitewise").delete_asset_model`
method.

Boto3 documentation:
[IoTSiteWise.Client.delete_asset_model](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotsitewise.html#IoTSiteWise.Client.delete_asset_model)

Asynchronous method. Use `await delete_asset_model(...)` for a synchronous
call.

Arguments mapping described in
[DeleteAssetModelRequestRequestTypeDef](./type_defs.md#deleteassetmodelrequestrequesttypedef).

Keyword-only arguments:

- `assetModelId`: `str` *(required)*
- `clientToken`: `str`

Returns a `Coroutine` for
[DeleteAssetModelResponseTypeDef](./type_defs.md#deleteassetmodelresponsetypedef).

<a id="delete_dashboard"></a>

### delete_dashboard

Deletes a dashboard from IoT SiteWise Monitor.

Type annotations for `session.create_client("iotsitewise").delete_dashboard`
method.

Boto3 documentation:
[IoTSiteWise.Client.delete_dashboard](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotsitewise.html#IoTSiteWise.Client.delete_dashboard)

Asynchronous method. Use `await delete_dashboard(...)` for a synchronous call.

Arguments mapping described in
[DeleteDashboardRequestRequestTypeDef](./type_defs.md#deletedashboardrequestrequesttypedef).

Keyword-only arguments:

- `dashboardId`: `str` *(required)*
- `clientToken`: `str`

Returns a `Coroutine` for `Dict`\[`str`, `Any`\].

<a id="delete_gateway"></a>

### delete_gateway

Deletes a gateway from IoT SiteWise.

Type annotations for `session.create_client("iotsitewise").delete_gateway`
method.

Boto3 documentation:
[IoTSiteWise.Client.delete_gateway](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotsitewise.html#IoTSiteWise.Client.delete_gateway)

Asynchronous method. Use `await delete_gateway(...)` for a synchronous call.

Arguments mapping described in
[DeleteGatewayRequestRequestTypeDef](./type_defs.md#deletegatewayrequestrequesttypedef).

Keyword-only arguments:

- `gatewayId`: `str` *(required)*

<a id="delete_portal"></a>

### delete_portal

Deletes a portal from IoT SiteWise Monitor.

Type annotations for `session.create_client("iotsitewise").delete_portal`
method.

Boto3 documentation:
[IoTSiteWise.Client.delete_portal](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotsitewise.html#IoTSiteWise.Client.delete_portal)

Asynchronous method. Use `await delete_portal(...)` for a synchronous call.

Arguments mapping described in
[DeletePortalRequestRequestTypeDef](./type_defs.md#deleteportalrequestrequesttypedef).

Keyword-only arguments:

- `portalId`: `str` *(required)*
- `clientToken`: `str`

Returns a `Coroutine` for
[DeletePortalResponseTypeDef](./type_defs.md#deleteportalresponsetypedef).

<a id="delete_project"></a>

### delete_project

Deletes a project from IoT SiteWise Monitor.

Type annotations for `session.create_client("iotsitewise").delete_project`
method.

Boto3 documentation:
[IoTSiteWise.Client.delete_project](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotsitewise.html#IoTSiteWise.Client.delete_project)

Asynchronous method. Use `await delete_project(...)` for a synchronous call.

Arguments mapping described in
[DeleteProjectRequestRequestTypeDef](./type_defs.md#deleteprojectrequestrequesttypedef).

Keyword-only arguments:

- `projectId`: `str` *(required)*
- `clientToken`: `str`

Returns a `Coroutine` for `Dict`\[`str`, `Any`\].

<a id="delete_time_series"></a>

### delete_time_series

Deletes a time series (data stream).

Type annotations for `session.create_client("iotsitewise").delete_time_series`
method.

Boto3 documentation:
[IoTSiteWise.Client.delete_time_series](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotsitewise.html#IoTSiteWise.Client.delete_time_series)

Asynchronous method. Use `await delete_time_series(...)` for a synchronous
call.

Arguments mapping described in
[DeleteTimeSeriesRequestRequestTypeDef](./type_defs.md#deletetimeseriesrequestrequesttypedef).

Keyword-only arguments:

- `alias`: `str`
- `assetId`: `str`
- `propertyId`: `str`
- `clientToken`: `str`

<a id="describe_access_policy"></a>

### describe_access_policy

Describes an access policy, which specifies an identity's access to an IoT
SiteWise Monitor portal or project.

Type annotations for
`session.create_client("iotsitewise").describe_access_policy` method.

Boto3 documentation:
[IoTSiteWise.Client.describe_access_policy](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotsitewise.html#IoTSiteWise.Client.describe_access_policy)

Asynchronous method. Use `await describe_access_policy(...)` for a synchronous
call.

Arguments mapping described in
[DescribeAccessPolicyRequestRequestTypeDef](./type_defs.md#describeaccesspolicyrequestrequesttypedef).

Keyword-only arguments:

- `accessPolicyId`: `str` *(required)*

Returns a `Coroutine` for
[DescribeAccessPolicyResponseTypeDef](./type_defs.md#describeaccesspolicyresponsetypedef).

<a id="describe_asset"></a>

### describe_asset

Retrieves information about an asset.

Type annotations for `session.create_client("iotsitewise").describe_asset`
method.

Boto3 documentation:
[IoTSiteWise.Client.describe_asset](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotsitewise.html#IoTSiteWise.Client.describe_asset)

Asynchronous method. Use `await describe_asset(...)` for a synchronous call.

Arguments mapping described in
[DescribeAssetRequestRequestTypeDef](./type_defs.md#describeassetrequestrequesttypedef).

Keyword-only arguments:

- `assetId`: `str` *(required)*

Returns a `Coroutine` for
[DescribeAssetResponseTypeDef](./type_defs.md#describeassetresponsetypedef).

<a id="describe_asset_model"></a>

### describe_asset_model

Retrieves information about an asset model.

Type annotations for
`session.create_client("iotsitewise").describe_asset_model` method.

Boto3 documentation:
[IoTSiteWise.Client.describe_asset_model](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotsitewise.html#IoTSiteWise.Client.describe_asset_model)

Asynchronous method. Use `await describe_asset_model(...)` for a synchronous
call.

Arguments mapping described in
[DescribeAssetModelRequestRequestTypeDef](./type_defs.md#describeassetmodelrequestrequesttypedef).

Keyword-only arguments:

- `assetModelId`: `str` *(required)*

Returns a `Coroutine` for
[DescribeAssetModelResponseTypeDef](./type_defs.md#describeassetmodelresponsetypedef).

<a id="describe_asset_property"></a>

### describe_asset_property

Retrieves information about an asset property.

Type annotations for
`session.create_client("iotsitewise").describe_asset_property` method.

Boto3 documentation:
[IoTSiteWise.Client.describe_asset_property](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotsitewise.html#IoTSiteWise.Client.describe_asset_property)

Asynchronous method. Use `await describe_asset_property(...)` for a synchronous
call.

Arguments mapping described in
[DescribeAssetPropertyRequestRequestTypeDef](./type_defs.md#describeassetpropertyrequestrequesttypedef).

Keyword-only arguments:

- `assetId`: `str` *(required)*
- `propertyId`: `str` *(required)*

Returns a `Coroutine` for
[DescribeAssetPropertyResponseTypeDef](./type_defs.md#describeassetpropertyresponsetypedef).

<a id="describe_dashboard"></a>

### describe_dashboard

Retrieves information about a dashboard.

Type annotations for `session.create_client("iotsitewise").describe_dashboard`
method.

Boto3 documentation:
[IoTSiteWise.Client.describe_dashboard](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotsitewise.html#IoTSiteWise.Client.describe_dashboard)

Asynchronous method. Use `await describe_dashboard(...)` for a synchronous
call.

Arguments mapping described in
[DescribeDashboardRequestRequestTypeDef](./type_defs.md#describedashboardrequestrequesttypedef).

Keyword-only arguments:

- `dashboardId`: `str` *(required)*

Returns a `Coroutine` for
[DescribeDashboardResponseTypeDef](./type_defs.md#describedashboardresponsetypedef).

<a id="describe_default_encryption_configuration"></a>

### describe_default_encryption_configuration

Retrieves information about the default encryption configuration for the Amazon
Web Services account in the default or specified Region.

Type annotations for
`session.create_client("iotsitewise").describe_default_encryption_configuration`
method.

Boto3 documentation:
[IoTSiteWise.Client.describe_default_encryption_configuration](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotsitewise.html#IoTSiteWise.Client.describe_default_encryption_configuration)

Asynchronous method. Use `await describe_default_encryption_configuration(...)`
for a synchronous call.

Returns a `Coroutine` for
[DescribeDefaultEncryptionConfigurationResponseTypeDef](./type_defs.md#describedefaultencryptionconfigurationresponsetypedef).

<a id="describe_gateway"></a>

### describe_gateway

Retrieves information about a gateway.

Type annotations for `session.create_client("iotsitewise").describe_gateway`
method.

Boto3 documentation:
[IoTSiteWise.Client.describe_gateway](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotsitewise.html#IoTSiteWise.Client.describe_gateway)

Asynchronous method. Use `await describe_gateway(...)` for a synchronous call.

Arguments mapping described in
[DescribeGatewayRequestRequestTypeDef](./type_defs.md#describegatewayrequestrequesttypedef).

Keyword-only arguments:

- `gatewayId`: `str` *(required)*

Returns a `Coroutine` for
[DescribeGatewayResponseTypeDef](./type_defs.md#describegatewayresponsetypedef).

<a id="describe_gateway_capability_configuration"></a>

### describe_gateway_capability_configuration

Retrieves information about a gateway capability configuration.

Type annotations for
`session.create_client("iotsitewise").describe_gateway_capability_configuration`
method.

Boto3 documentation:
[IoTSiteWise.Client.describe_gateway_capability_configuration](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotsitewise.html#IoTSiteWise.Client.describe_gateway_capability_configuration)

Asynchronous method. Use `await describe_gateway_capability_configuration(...)`
for a synchronous call.

Arguments mapping described in
[DescribeGatewayCapabilityConfigurationRequestRequestTypeDef](./type_defs.md#describegatewaycapabilityconfigurationrequestrequesttypedef).

Keyword-only arguments:

- `gatewayId`: `str` *(required)*
- `capabilityNamespace`: `str` *(required)*

Returns a `Coroutine` for
[DescribeGatewayCapabilityConfigurationResponseTypeDef](./type_defs.md#describegatewaycapabilityconfigurationresponsetypedef).

<a id="describe_logging_options"></a>

### describe_logging_options

Retrieves the current IoT SiteWise logging options.

Type annotations for
`session.create_client("iotsitewise").describe_logging_options` method.

Boto3 documentation:
[IoTSiteWise.Client.describe_logging_options](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotsitewise.html#IoTSiteWise.Client.describe_logging_options)

Asynchronous method. Use `await describe_logging_options(...)` for a
synchronous call.

Returns a `Coroutine` for
[DescribeLoggingOptionsResponseTypeDef](./type_defs.md#describeloggingoptionsresponsetypedef).

<a id="describe_portal"></a>

### describe_portal

Retrieves information about a portal.

Type annotations for `session.create_client("iotsitewise").describe_portal`
method.

Boto3 documentation:
[IoTSiteWise.Client.describe_portal](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotsitewise.html#IoTSiteWise.Client.describe_portal)

Asynchronous method. Use `await describe_portal(...)` for a synchronous call.

Arguments mapping described in
[DescribePortalRequestRequestTypeDef](./type_defs.md#describeportalrequestrequesttypedef).

Keyword-only arguments:

- `portalId`: `str` *(required)*

Returns a `Coroutine` for
[DescribePortalResponseTypeDef](./type_defs.md#describeportalresponsetypedef).

<a id="describe_project"></a>

### describe_project

Retrieves information about a project.

Type annotations for `session.create_client("iotsitewise").describe_project`
method.

Boto3 documentation:
[IoTSiteWise.Client.describe_project](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotsitewise.html#IoTSiteWise.Client.describe_project)

Asynchronous method. Use `await describe_project(...)` for a synchronous call.

Arguments mapping described in
[DescribeProjectRequestRequestTypeDef](./type_defs.md#describeprojectrequestrequesttypedef).

Keyword-only arguments:

- `projectId`: `str` *(required)*

Returns a `Coroutine` for
[DescribeProjectResponseTypeDef](./type_defs.md#describeprojectresponsetypedef).

<a id="describe_storage_configuration"></a>

### describe_storage_configuration

Retrieves information about the storage configuration for IoT SiteWise.

Type annotations for
`session.create_client("iotsitewise").describe_storage_configuration` method.

Boto3 documentation:
[IoTSiteWise.Client.describe_storage_configuration](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotsitewise.html#IoTSiteWise.Client.describe_storage_configuration)

Asynchronous method. Use `await describe_storage_configuration(...)` for a
synchronous call.

Returns a `Coroutine` for
[DescribeStorageConfigurationResponseTypeDef](./type_defs.md#describestorageconfigurationresponsetypedef).

<a id="describe_time_series"></a>

### describe_time_series

Retrieves information about a time series (data stream).

Type annotations for
`session.create_client("iotsitewise").describe_time_series` method.

Boto3 documentation:
[IoTSiteWise.Client.describe_time_series](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotsitewise.html#IoTSiteWise.Client.describe_time_series)

Asynchronous method. Use `await describe_time_series(...)` for a synchronous
call.

Arguments mapping described in
[DescribeTimeSeriesRequestRequestTypeDef](./type_defs.md#describetimeseriesrequestrequesttypedef).

Keyword-only arguments:

- `alias`: `str`
- `assetId`: `str`
- `propertyId`: `str`

Returns a `Coroutine` for
[DescribeTimeSeriesResponseTypeDef](./type_defs.md#describetimeseriesresponsetypedef).

<a id="disassociate_assets"></a>

### disassociate_assets

Disassociates a child asset from the given parent asset through a hierarchy
defined in the parent asset's model.

Type annotations for `session.create_client("iotsitewise").disassociate_assets`
method.

Boto3 documentation:
[IoTSiteWise.Client.disassociate_assets](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotsitewise.html#IoTSiteWise.Client.disassociate_assets)

Asynchronous method. Use `await disassociate_assets(...)` for a synchronous
call.

Arguments mapping described in
[DisassociateAssetsRequestRequestTypeDef](./type_defs.md#disassociateassetsrequestrequesttypedef).

Keyword-only arguments:

- `assetId`: `str` *(required)*
- `hierarchyId`: `str` *(required)*
- `childAssetId`: `str` *(required)*
- `clientToken`: `str`

<a id="disassociate_time_series_from_asset_property"></a>

### disassociate_time_series_from_asset_property

Disassociates a time series (data stream) from an asset property.

Type annotations for
`session.create_client("iotsitewise").disassociate_time_series_from_asset_property`
method.

Boto3 documentation:
[IoTSiteWise.Client.disassociate_time_series_from_asset_property](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotsitewise.html#IoTSiteWise.Client.disassociate_time_series_from_asset_property)

Asynchronous method. Use
`await disassociate_time_series_from_asset_property(...)` for a synchronous
call.

Arguments mapping described in
[DisassociateTimeSeriesFromAssetPropertyRequestRequestTypeDef](./type_defs.md#disassociatetimeseriesfromassetpropertyrequestrequesttypedef).

Keyword-only arguments:

- `alias`: `str` *(required)*
- `assetId`: `str` *(required)*
- `propertyId`: `str` *(required)*
- `clientToken`: `str`

<a id="generate_presigned_url"></a>

### generate_presigned_url

Generate a presigned url given a client, its method, and arguments.

Type annotations for
`session.create_client("iotsitewise").generate_presigned_url` method.

Boto3 documentation:
[IoTSiteWise.Client.generate_presigned_url](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotsitewise.html#IoTSiteWise.Client.generate_presigned_url)

Asynchronous method. Use `await generate_presigned_url(...)` for a synchronous
call.

Arguments:

- `ClientMethod`: `str` *(required)*
- `Params`: `Mapping`\[`str`, `Any`\]
- `ExpiresIn`: `int`
- `HttpMethod`: `str`

Returns a `Coroutine` for `str`.

<a id="get_asset_property_aggregates"></a>

### get_asset_property_aggregates

Gets aggregated values for an asset property.

Type annotations for
`session.create_client("iotsitewise").get_asset_property_aggregates` method.

Boto3 documentation:
[IoTSiteWise.Client.get_asset_property_aggregates](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotsitewise.html#IoTSiteWise.Client.get_asset_property_aggregates)

Asynchronous method. Use `await get_asset_property_aggregates(...)` for a
synchronous call.

Arguments mapping described in
[GetAssetPropertyAggregatesRequestRequestTypeDef](./type_defs.md#getassetpropertyaggregatesrequestrequesttypedef).

Keyword-only arguments:

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
- `nextToken`: `str`
- `maxResults`: `int`

Returns a `Coroutine` for
[GetAssetPropertyAggregatesResponseTypeDef](./type_defs.md#getassetpropertyaggregatesresponsetypedef).

<a id="get_asset_property_value"></a>

### get_asset_property_value

Gets an asset property's current value.

Type annotations for
`session.create_client("iotsitewise").get_asset_property_value` method.

Boto3 documentation:
[IoTSiteWise.Client.get_asset_property_value](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotsitewise.html#IoTSiteWise.Client.get_asset_property_value)

Asynchronous method. Use `await get_asset_property_value(...)` for a
synchronous call.

Arguments mapping described in
[GetAssetPropertyValueRequestRequestTypeDef](./type_defs.md#getassetpropertyvaluerequestrequesttypedef).

Keyword-only arguments:

- `assetId`: `str`
- `propertyId`: `str`
- `propertyAlias`: `str`

Returns a `Coroutine` for
[GetAssetPropertyValueResponseTypeDef](./type_defs.md#getassetpropertyvalueresponsetypedef).

<a id="get_asset_property_value_history"></a>

### get_asset_property_value_history

Gets the history of an asset property's values.

Type annotations for
`session.create_client("iotsitewise").get_asset_property_value_history` method.

Boto3 documentation:
[IoTSiteWise.Client.get_asset_property_value_history](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotsitewise.html#IoTSiteWise.Client.get_asset_property_value_history)

Asynchronous method. Use `await get_asset_property_value_history(...)` for a
synchronous call.

Arguments mapping described in
[GetAssetPropertyValueHistoryRequestRequestTypeDef](./type_defs.md#getassetpropertyvaluehistoryrequestrequesttypedef).

Keyword-only arguments:

- `assetId`: `str`
- `propertyId`: `str`
- `propertyAlias`: `str`
- `startDate`: `Union`\[`datetime`, `str`\]
- `endDate`: `Union`\[`datetime`, `str`\]
- `qualities`: `Sequence`\[[QualityType](./literals.md#qualitytype)\]
- `timeOrdering`: [TimeOrderingType](./literals.md#timeorderingtype)
- `nextToken`: `str`
- `maxResults`: `int`

Returns a `Coroutine` for
[GetAssetPropertyValueHistoryResponseTypeDef](./type_defs.md#getassetpropertyvaluehistoryresponsetypedef).

<a id="get_interpolated_asset_property_values"></a>

### get_interpolated_asset_property_values

Get interpolated values for an asset property for a specified time interval,
during a period of time.

Type annotations for
`session.create_client("iotsitewise").get_interpolated_asset_property_values`
method.

Boto3 documentation:
[IoTSiteWise.Client.get_interpolated_asset_property_values](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotsitewise.html#IoTSiteWise.Client.get_interpolated_asset_property_values)

Asynchronous method. Use `await get_interpolated_asset_property_values(...)`
for a synchronous call.

Arguments mapping described in
[GetInterpolatedAssetPropertyValuesRequestRequestTypeDef](./type_defs.md#getinterpolatedassetpropertyvaluesrequestrequesttypedef).

Keyword-only arguments:

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
- `nextToken`: `str`
- `maxResults`: `int`
- `intervalWindowInSeconds`: `int`

Returns a `Coroutine` for
[GetInterpolatedAssetPropertyValuesResponseTypeDef](./type_defs.md#getinterpolatedassetpropertyvaluesresponsetypedef).

<a id="list_access_policies"></a>

### list_access_policies

Retrieves a paginated list of access policies for an identity (an Amazon Web
Services SSO user, an Amazon Web Services SSO group, or an IAM user) or an IoT
SiteWise Monitor resource (a portal or project).

Type annotations for
`session.create_client("iotsitewise").list_access_policies` method.

Boto3 documentation:
[IoTSiteWise.Client.list_access_policies](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotsitewise.html#IoTSiteWise.Client.list_access_policies)

Asynchronous method. Use `await list_access_policies(...)` for a synchronous
call.

Arguments mapping described in
[ListAccessPoliciesRequestRequestTypeDef](./type_defs.md#listaccesspoliciesrequestrequesttypedef).

Keyword-only arguments:

- `identityType`: [IdentityTypeType](./literals.md#identitytypetype)
- `identityId`: `str`
- `resourceType`: [ResourceTypeType](./literals.md#resourcetypetype)
- `resourceId`: `str`
- `iamArn`: `str`
- `nextToken`: `str`
- `maxResults`: `int`

Returns a `Coroutine` for
[ListAccessPoliciesResponseTypeDef](./type_defs.md#listaccesspoliciesresponsetypedef).

<a id="list_asset_models"></a>

### list_asset_models

Retrieves a paginated list of summaries of all asset models.

Type annotations for `session.create_client("iotsitewise").list_asset_models`
method.

Boto3 documentation:
[IoTSiteWise.Client.list_asset_models](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotsitewise.html#IoTSiteWise.Client.list_asset_models)

Asynchronous method. Use `await list_asset_models(...)` for a synchronous call.

Arguments mapping described in
[ListAssetModelsRequestRequestTypeDef](./type_defs.md#listassetmodelsrequestrequesttypedef).

Keyword-only arguments:

- `nextToken`: `str`
- `maxResults`: `int`

Returns a `Coroutine` for
[ListAssetModelsResponseTypeDef](./type_defs.md#listassetmodelsresponsetypedef).

<a id="list_asset_relationships"></a>

### list_asset_relationships

Retrieves a paginated list of asset relationships for an asset.

Type annotations for
`session.create_client("iotsitewise").list_asset_relationships` method.

Boto3 documentation:
[IoTSiteWise.Client.list_asset_relationships](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotsitewise.html#IoTSiteWise.Client.list_asset_relationships)

Asynchronous method. Use `await list_asset_relationships(...)` for a
synchronous call.

Arguments mapping described in
[ListAssetRelationshipsRequestRequestTypeDef](./type_defs.md#listassetrelationshipsrequestrequesttypedef).

Keyword-only arguments:

- `assetId`: `str` *(required)*
- `traversalType`: `Literal['PATH_TO_ROOT']` (see
  [TraversalTypeType](./literals.md#traversaltypetype)) *(required)*
- `nextToken`: `str`
- `maxResults`: `int`

Returns a `Coroutine` for
[ListAssetRelationshipsResponseTypeDef](./type_defs.md#listassetrelationshipsresponsetypedef).

<a id="list_assets"></a>

### list_assets

Retrieves a paginated list of asset summaries.

Type annotations for `session.create_client("iotsitewise").list_assets` method.

Boto3 documentation:
[IoTSiteWise.Client.list_assets](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotsitewise.html#IoTSiteWise.Client.list_assets)

Asynchronous method. Use `await list_assets(...)` for a synchronous call.

Arguments mapping described in
[ListAssetsRequestRequestTypeDef](./type_defs.md#listassetsrequestrequesttypedef).

Keyword-only arguments:

- `nextToken`: `str`
- `maxResults`: `int`
- `assetModelId`: `str`
- `filter`: [ListAssetsFilterType](./literals.md#listassetsfiltertype)

Returns a `Coroutine` for
[ListAssetsResponseTypeDef](./type_defs.md#listassetsresponsetypedef).

<a id="list_associated_assets"></a>

### list_associated_assets

Retrieves a paginated list of associated assets.

Type annotations for
`session.create_client("iotsitewise").list_associated_assets` method.

Boto3 documentation:
[IoTSiteWise.Client.list_associated_assets](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotsitewise.html#IoTSiteWise.Client.list_associated_assets)

Asynchronous method. Use `await list_associated_assets(...)` for a synchronous
call.

Arguments mapping described in
[ListAssociatedAssetsRequestRequestTypeDef](./type_defs.md#listassociatedassetsrequestrequesttypedef).

Keyword-only arguments:

- `assetId`: `str` *(required)*
- `hierarchyId`: `str`
- `traversalDirection`:
  [TraversalDirectionType](./literals.md#traversaldirectiontype)
- `nextToken`: `str`
- `maxResults`: `int`

Returns a `Coroutine` for
[ListAssociatedAssetsResponseTypeDef](./type_defs.md#listassociatedassetsresponsetypedef).

<a id="list_dashboards"></a>

### list_dashboards

Retrieves a paginated list of dashboards for an IoT SiteWise Monitor project.

Type annotations for `session.create_client("iotsitewise").list_dashboards`
method.

Boto3 documentation:
[IoTSiteWise.Client.list_dashboards](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotsitewise.html#IoTSiteWise.Client.list_dashboards)

Asynchronous method. Use `await list_dashboards(...)` for a synchronous call.

Arguments mapping described in
[ListDashboardsRequestRequestTypeDef](./type_defs.md#listdashboardsrequestrequesttypedef).

Keyword-only arguments:

- `projectId`: `str` *(required)*
- `nextToken`: `str`
- `maxResults`: `int`

Returns a `Coroutine` for
[ListDashboardsResponseTypeDef](./type_defs.md#listdashboardsresponsetypedef).

<a id="list_gateways"></a>

### list_gateways

Retrieves a paginated list of gateways.

Type annotations for `session.create_client("iotsitewise").list_gateways`
method.

Boto3 documentation:
[IoTSiteWise.Client.list_gateways](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotsitewise.html#IoTSiteWise.Client.list_gateways)

Asynchronous method. Use `await list_gateways(...)` for a synchronous call.

Arguments mapping described in
[ListGatewaysRequestRequestTypeDef](./type_defs.md#listgatewaysrequestrequesttypedef).

Keyword-only arguments:

- `nextToken`: `str`
- `maxResults`: `int`

Returns a `Coroutine` for
[ListGatewaysResponseTypeDef](./type_defs.md#listgatewaysresponsetypedef).

<a id="list_portals"></a>

### list_portals

Retrieves a paginated list of IoT SiteWise Monitor portals.

Type annotations for `session.create_client("iotsitewise").list_portals`
method.

Boto3 documentation:
[IoTSiteWise.Client.list_portals](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotsitewise.html#IoTSiteWise.Client.list_portals)

Asynchronous method. Use `await list_portals(...)` for a synchronous call.

Arguments mapping described in
[ListPortalsRequestRequestTypeDef](./type_defs.md#listportalsrequestrequesttypedef).

Keyword-only arguments:

- `nextToken`: `str`
- `maxResults`: `int`

Returns a `Coroutine` for
[ListPortalsResponseTypeDef](./type_defs.md#listportalsresponsetypedef).

<a id="list_project_assets"></a>

### list_project_assets

Retrieves a paginated list of assets associated with an IoT SiteWise Monitor
project.

Type annotations for `session.create_client("iotsitewise").list_project_assets`
method.

Boto3 documentation:
[IoTSiteWise.Client.list_project_assets](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotsitewise.html#IoTSiteWise.Client.list_project_assets)

Asynchronous method. Use `await list_project_assets(...)` for a synchronous
call.

Arguments mapping described in
[ListProjectAssetsRequestRequestTypeDef](./type_defs.md#listprojectassetsrequestrequesttypedef).

Keyword-only arguments:

- `projectId`: `str` *(required)*
- `nextToken`: `str`
- `maxResults`: `int`

Returns a `Coroutine` for
[ListProjectAssetsResponseTypeDef](./type_defs.md#listprojectassetsresponsetypedef).

<a id="list_projects"></a>

### list_projects

Retrieves a paginated list of projects for an IoT SiteWise Monitor portal.

Type annotations for `session.create_client("iotsitewise").list_projects`
method.

Boto3 documentation:
[IoTSiteWise.Client.list_projects](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotsitewise.html#IoTSiteWise.Client.list_projects)

Asynchronous method. Use `await list_projects(...)` for a synchronous call.

Arguments mapping described in
[ListProjectsRequestRequestTypeDef](./type_defs.md#listprojectsrequestrequesttypedef).

Keyword-only arguments:

- `portalId`: `str` *(required)*
- `nextToken`: `str`
- `maxResults`: `int`

Returns a `Coroutine` for
[ListProjectsResponseTypeDef](./type_defs.md#listprojectsresponsetypedef).

<a id="list_tags_for_resource"></a>

### list_tags_for_resource

Retrieves the list of tags for an IoT SiteWise resource.

Type annotations for
`session.create_client("iotsitewise").list_tags_for_resource` method.

Boto3 documentation:
[IoTSiteWise.Client.list_tags_for_resource](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotsitewise.html#IoTSiteWise.Client.list_tags_for_resource)

Asynchronous method. Use `await list_tags_for_resource(...)` for a synchronous
call.

Arguments mapping described in
[ListTagsForResourceRequestRequestTypeDef](./type_defs.md#listtagsforresourcerequestrequesttypedef).

Keyword-only arguments:

- `resourceArn`: `str` *(required)*

Returns a `Coroutine` for
[ListTagsForResourceResponseTypeDef](./type_defs.md#listtagsforresourceresponsetypedef).

<a id="list_time_series"></a>

### list_time_series

Retrieves a paginated list of time series (data streams).

Type annotations for `session.create_client("iotsitewise").list_time_series`
method.

Boto3 documentation:
[IoTSiteWise.Client.list_time_series](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotsitewise.html#IoTSiteWise.Client.list_time_series)

Asynchronous method. Use `await list_time_series(...)` for a synchronous call.

Arguments mapping described in
[ListTimeSeriesRequestRequestTypeDef](./type_defs.md#listtimeseriesrequestrequesttypedef).

Keyword-only arguments:

- `nextToken`: `str`
- `maxResults`: `int`
- `assetId`: `str`
- `aliasPrefix`: `str`
- `timeSeriesType`:
  [ListTimeSeriesTypeType](./literals.md#listtimeseriestypetype)

Returns a `Coroutine` for
[ListTimeSeriesResponseTypeDef](./type_defs.md#listtimeseriesresponsetypedef).

<a id="put_default_encryption_configuration"></a>

### put_default_encryption_configuration

Sets the default encryption configuration for the Amazon Web Services account.

Type annotations for
`session.create_client("iotsitewise").put_default_encryption_configuration`
method.

Boto3 documentation:
[IoTSiteWise.Client.put_default_encryption_configuration](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotsitewise.html#IoTSiteWise.Client.put_default_encryption_configuration)

Asynchronous method. Use `await put_default_encryption_configuration(...)` for
a synchronous call.

Arguments mapping described in
[PutDefaultEncryptionConfigurationRequestRequestTypeDef](./type_defs.md#putdefaultencryptionconfigurationrequestrequesttypedef).

Keyword-only arguments:

- `encryptionType`: [EncryptionTypeType](./literals.md#encryptiontypetype)
  *(required)*
- `kmsKeyId`: `str`

Returns a `Coroutine` for
[PutDefaultEncryptionConfigurationResponseTypeDef](./type_defs.md#putdefaultencryptionconfigurationresponsetypedef).

<a id="put_logging_options"></a>

### put_logging_options

Sets logging options for IoT SiteWise.

Type annotations for `session.create_client("iotsitewise").put_logging_options`
method.

Boto3 documentation:
[IoTSiteWise.Client.put_logging_options](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotsitewise.html#IoTSiteWise.Client.put_logging_options)

Asynchronous method. Use `await put_logging_options(...)` for a synchronous
call.

Arguments mapping described in
[PutLoggingOptionsRequestRequestTypeDef](./type_defs.md#putloggingoptionsrequestrequesttypedef).

Keyword-only arguments:

- `loggingOptions`:
  [LoggingOptionsTypeDef](./type_defs.md#loggingoptionstypedef) *(required)*

Returns a `Coroutine` for `Dict`\[`str`, `Any`\].

<a id="put_storage_configuration"></a>

### put_storage_configuration

Configures storage settings for IoT SiteWise.

Type annotations for
`session.create_client("iotsitewise").put_storage_configuration` method.

Boto3 documentation:
[IoTSiteWise.Client.put_storage_configuration](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotsitewise.html#IoTSiteWise.Client.put_storage_configuration)

Asynchronous method. Use `await put_storage_configuration(...)` for a
synchronous call.

Arguments mapping described in
[PutStorageConfigurationRequestRequestTypeDef](./type_defs.md#putstorageconfigurationrequestrequesttypedef).

Keyword-only arguments:

- `storageType`: [StorageTypeType](./literals.md#storagetypetype) *(required)*
- `multiLayerStorage`:
  [MultiLayerStorageTypeDef](./type_defs.md#multilayerstoragetypedef)
- `disassociatedDataStorage`:
  [DisassociatedDataStorageStateType](./literals.md#disassociateddatastoragestatetype)
- `retentionPeriod`:
  [RetentionPeriodTypeDef](./type_defs.md#retentionperiodtypedef)

Returns a `Coroutine` for
[PutStorageConfigurationResponseTypeDef](./type_defs.md#putstorageconfigurationresponsetypedef).

<a id="tag_resource"></a>

### tag_resource

Adds tags to an IoT SiteWise resource.

Type annotations for `session.create_client("iotsitewise").tag_resource`
method.

Boto3 documentation:
[IoTSiteWise.Client.tag_resource](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotsitewise.html#IoTSiteWise.Client.tag_resource)

Asynchronous method. Use `await tag_resource(...)` for a synchronous call.

Arguments mapping described in
[TagResourceRequestRequestTypeDef](./type_defs.md#tagresourcerequestrequesttypedef).

Keyword-only arguments:

- `resourceArn`: `str` *(required)*
- `tags`: `Mapping`\[`str`, `str`\] *(required)*

Returns a `Coroutine` for `Dict`\[`str`, `Any`\].

<a id="untag_resource"></a>

### untag_resource

Removes a tag from an IoT SiteWise resource.

Type annotations for `session.create_client("iotsitewise").untag_resource`
method.

Boto3 documentation:
[IoTSiteWise.Client.untag_resource](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotsitewise.html#IoTSiteWise.Client.untag_resource)

Asynchronous method. Use `await untag_resource(...)` for a synchronous call.

Arguments mapping described in
[UntagResourceRequestRequestTypeDef](./type_defs.md#untagresourcerequestrequesttypedef).

Keyword-only arguments:

- `resourceArn`: `str` *(required)*
- `tagKeys`: `Sequence`\[`str`\] *(required)*

Returns a `Coroutine` for `Dict`\[`str`, `Any`\].

<a id="update_access_policy"></a>

### update_access_policy

Updates an existing access policy that specifies an identity's access to an IoT
SiteWise Monitor portal or project resource.

Type annotations for
`session.create_client("iotsitewise").update_access_policy` method.

Boto3 documentation:
[IoTSiteWise.Client.update_access_policy](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotsitewise.html#IoTSiteWise.Client.update_access_policy)

Asynchronous method. Use `await update_access_policy(...)` for a synchronous
call.

Arguments mapping described in
[UpdateAccessPolicyRequestRequestTypeDef](./type_defs.md#updateaccesspolicyrequestrequesttypedef).

Keyword-only arguments:

- `accessPolicyId`: `str` *(required)*
- `accessPolicyIdentity`: [IdentityTypeDef](./type_defs.md#identitytypedef)
  *(required)*
- `accessPolicyResource`: [ResourceTypeDef](./type_defs.md#resourcetypedef)
  *(required)*
- `accessPolicyPermission`: [PermissionType](./literals.md#permissiontype)
  *(required)*
- `clientToken`: `str`

Returns a `Coroutine` for `Dict`\[`str`, `Any`\].

<a id="update_asset"></a>

### update_asset

Updates an asset's name.

Type annotations for `session.create_client("iotsitewise").update_asset`
method.

Boto3 documentation:
[IoTSiteWise.Client.update_asset](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotsitewise.html#IoTSiteWise.Client.update_asset)

Asynchronous method. Use `await update_asset(...)` for a synchronous call.

Arguments mapping described in
[UpdateAssetRequestRequestTypeDef](./type_defs.md#updateassetrequestrequesttypedef).

Keyword-only arguments:

- `assetId`: `str` *(required)*
- `assetName`: `str` *(required)*
- `clientToken`: `str`

Returns a `Coroutine` for
[UpdateAssetResponseTypeDef](./type_defs.md#updateassetresponsetypedef).

<a id="update_asset_model"></a>

### update_asset_model

Updates an asset model and all of the assets that were created from the model.

Type annotations for `session.create_client("iotsitewise").update_asset_model`
method.

Boto3 documentation:
[IoTSiteWise.Client.update_asset_model](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotsitewise.html#IoTSiteWise.Client.update_asset_model)

Asynchronous method. Use `await update_asset_model(...)` for a synchronous
call.

Arguments mapping described in
[UpdateAssetModelRequestRequestTypeDef](./type_defs.md#updateassetmodelrequestrequesttypedef).

Keyword-only arguments:

- `assetModelId`: `str` *(required)*
- `assetModelName`: `str` *(required)*
- `assetModelDescription`: `str`
- `assetModelProperties`:
  `Sequence`\[[AssetModelPropertyTypeDef](./type_defs.md#assetmodelpropertytypedef)\]
- `assetModelHierarchies`:
  `Sequence`\[[AssetModelHierarchyTypeDef](./type_defs.md#assetmodelhierarchytypedef)\]
- `assetModelCompositeModels`:
  `Sequence`\[[AssetModelCompositeModelTypeDef](./type_defs.md#assetmodelcompositemodeltypedef)\]
- `clientToken`: `str`

Returns a `Coroutine` for
[UpdateAssetModelResponseTypeDef](./type_defs.md#updateassetmodelresponsetypedef).

<a id="update_asset_property"></a>

### update_asset_property

Updates an asset property's alias and notification state.

Type annotations for
`session.create_client("iotsitewise").update_asset_property` method.

Boto3 documentation:
[IoTSiteWise.Client.update_asset_property](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotsitewise.html#IoTSiteWise.Client.update_asset_property)

Asynchronous method. Use `await update_asset_property(...)` for a synchronous
call.

Arguments mapping described in
[UpdateAssetPropertyRequestRequestTypeDef](./type_defs.md#updateassetpropertyrequestrequesttypedef).

Keyword-only arguments:

- `assetId`: `str` *(required)*
- `propertyId`: `str` *(required)*
- `propertyAlias`: `str`
- `propertyNotificationState`:
  [PropertyNotificationStateType](./literals.md#propertynotificationstatetype)
- `clientToken`: `str`

<a id="update_dashboard"></a>

### update_dashboard

Updates an IoT SiteWise Monitor dashboard.

Type annotations for `session.create_client("iotsitewise").update_dashboard`
method.

Boto3 documentation:
[IoTSiteWise.Client.update_dashboard](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotsitewise.html#IoTSiteWise.Client.update_dashboard)

Asynchronous method. Use `await update_dashboard(...)` for a synchronous call.

Arguments mapping described in
[UpdateDashboardRequestRequestTypeDef](./type_defs.md#updatedashboardrequestrequesttypedef).

Keyword-only arguments:

- `dashboardId`: `str` *(required)*
- `dashboardName`: `str` *(required)*
- `dashboardDefinition`: `str` *(required)*
- `dashboardDescription`: `str`
- `clientToken`: `str`

Returns a `Coroutine` for `Dict`\[`str`, `Any`\].

<a id="update_gateway"></a>

### update_gateway

Updates a gateway's name.

Type annotations for `session.create_client("iotsitewise").update_gateway`
method.

Boto3 documentation:
[IoTSiteWise.Client.update_gateway](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotsitewise.html#IoTSiteWise.Client.update_gateway)

Asynchronous method. Use `await update_gateway(...)` for a synchronous call.

Arguments mapping described in
[UpdateGatewayRequestRequestTypeDef](./type_defs.md#updategatewayrequestrequesttypedef).

Keyword-only arguments:

- `gatewayId`: `str` *(required)*
- `gatewayName`: `str` *(required)*

<a id="update_gateway_capability_configuration"></a>

### update_gateway_capability_configuration

Updates a gateway capability configuration or defines a new capability
configuration.

Type annotations for
`session.create_client("iotsitewise").update_gateway_capability_configuration`
method.

Boto3 documentation:
[IoTSiteWise.Client.update_gateway_capability_configuration](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotsitewise.html#IoTSiteWise.Client.update_gateway_capability_configuration)

Asynchronous method. Use `await update_gateway_capability_configuration(...)`
for a synchronous call.

Arguments mapping described in
[UpdateGatewayCapabilityConfigurationRequestRequestTypeDef](./type_defs.md#updategatewaycapabilityconfigurationrequestrequesttypedef).

Keyword-only arguments:

- `gatewayId`: `str` *(required)*
- `capabilityNamespace`: `str` *(required)*
- `capabilityConfiguration`: `str` *(required)*

Returns a `Coroutine` for
[UpdateGatewayCapabilityConfigurationResponseTypeDef](./type_defs.md#updategatewaycapabilityconfigurationresponsetypedef).

<a id="update_portal"></a>

### update_portal

Updates an IoT SiteWise Monitor portal.

Type annotations for `session.create_client("iotsitewise").update_portal`
method.

Boto3 documentation:
[IoTSiteWise.Client.update_portal](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotsitewise.html#IoTSiteWise.Client.update_portal)

Asynchronous method. Use `await update_portal(...)` for a synchronous call.

Arguments mapping described in
[UpdatePortalRequestRequestTypeDef](./type_defs.md#updateportalrequestrequesttypedef).

Keyword-only arguments:

- `portalId`: `str` *(required)*
- `portalName`: `str` *(required)*
- `portalContactEmail`: `str` *(required)*
- `roleArn`: `str` *(required)*
- `portalDescription`: `str`
- `portalLogoImage`: [ImageTypeDef](./type_defs.md#imagetypedef)
- `clientToken`: `str`
- `notificationSenderEmail`: `str`
- `alarms`: [AlarmsTypeDef](./type_defs.md#alarmstypedef)

Returns a `Coroutine` for
[UpdatePortalResponseTypeDef](./type_defs.md#updateportalresponsetypedef).

<a id="update_project"></a>

### update_project

Updates an IoT SiteWise Monitor project.

Type annotations for `session.create_client("iotsitewise").update_project`
method.

Boto3 documentation:
[IoTSiteWise.Client.update_project](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotsitewise.html#IoTSiteWise.Client.update_project)

Asynchronous method. Use `await update_project(...)` for a synchronous call.

Arguments mapping described in
[UpdateProjectRequestRequestTypeDef](./type_defs.md#updateprojectrequestrequesttypedef).

Keyword-only arguments:

- `projectId`: `str` *(required)*
- `projectName`: `str` *(required)*
- `projectDescription`: `str`
- `clientToken`: `str`

Returns a `Coroutine` for `Dict`\[`str`, `Any`\].

<a id="__aenter__"></a>

### __aenter__

Type annotations for `session.create_client("iotsitewise").__aenter__` method.

Boto3 documentation:
[IoTSiteWise.Client.__aenter__](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotsitewise.html#IoTSiteWise.Client.__aenter__)

Asynchronous method. Use `await __aenter__(...)` for a synchronous call.

Returns a `Coroutine` for [IoTSiteWiseClient](#iotsitewiseclient).

<a id="__aexit__"></a>

### __aexit__

Type annotations for `session.create_client("iotsitewise").__aexit__` method.

Boto3 documentation:
[IoTSiteWise.Client.__aexit__](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotsitewise.html#IoTSiteWise.Client.__aexit__)

Asynchronous method. Use `await __aexit__(...)` for a synchronous call.

Arguments:

- `exc_type`: `Any` *(required)*
- `exc_val`: `Any` *(required)*
- `exc_tb`: `Any` *(required)*

Returns a `Coroutine` for `Any`.

<a id="get_paginator"></a>

### get_paginator

Type annotations for `session.create_client("iotsitewise").get_paginator`
method with overloads.

- `client.get_paginator("get_asset_property_aggregates")` ->
  [GetAssetPropertyAggregatesPaginator](./paginators.md#getassetpropertyaggregatespaginator)
- `client.get_paginator("get_asset_property_value_history")` ->
  [GetAssetPropertyValueHistoryPaginator](./paginators.md#getassetpropertyvaluehistorypaginator)
- `client.get_paginator("get_interpolated_asset_property_values")` ->
  [GetInterpolatedAssetPropertyValuesPaginator](./paginators.md#getinterpolatedassetpropertyvaluespaginator)
- `client.get_paginator("list_access_policies")` ->
  [ListAccessPoliciesPaginator](./paginators.md#listaccesspoliciespaginator)
- `client.get_paginator("list_asset_models")` ->
  [ListAssetModelsPaginator](./paginators.md#listassetmodelspaginator)
- `client.get_paginator("list_asset_relationships")` ->
  [ListAssetRelationshipsPaginator](./paginators.md#listassetrelationshipspaginator)
- `client.get_paginator("list_assets")` ->
  [ListAssetsPaginator](./paginators.md#listassetspaginator)
- `client.get_paginator("list_associated_assets")` ->
  [ListAssociatedAssetsPaginator](./paginators.md#listassociatedassetspaginator)
- `client.get_paginator("list_dashboards")` ->
  [ListDashboardsPaginator](./paginators.md#listdashboardspaginator)
- `client.get_paginator("list_gateways")` ->
  [ListGatewaysPaginator](./paginators.md#listgatewayspaginator)
- `client.get_paginator("list_portals")` ->
  [ListPortalsPaginator](./paginators.md#listportalspaginator)
- `client.get_paginator("list_project_assets")` ->
  [ListProjectAssetsPaginator](./paginators.md#listprojectassetspaginator)
- `client.get_paginator("list_projects")` ->
  [ListProjectsPaginator](./paginators.md#listprojectspaginator)
- `client.get_paginator("list_time_series")` ->
  [ListTimeSeriesPaginator](./paginators.md#listtimeseriespaginator)

<a id="get_waiter"></a>

### get_waiter

Type annotations for `session.create_client("iotsitewise").get_waiter` method
with overloads.

- `client.get_waiter("asset_active")` ->
  [AssetActiveWaiter](./waiters.md#assetactivewaiter)
- `client.get_waiter("asset_model_active")` ->
  [AssetModelActiveWaiter](./waiters.md#assetmodelactivewaiter)
- `client.get_waiter("asset_model_not_exists")` ->
  [AssetModelNotExistsWaiter](./waiters.md#assetmodelnotexistswaiter)
- `client.get_waiter("asset_not_exists")` ->
  [AssetNotExistsWaiter](./waiters.md#assetnotexistswaiter)
- `client.get_waiter("portal_active")` ->
  [PortalActiveWaiter](./waiters.md#portalactivewaiter)
- `client.get_waiter("portal_not_exists")` ->
  [PortalNotExistsWaiter](./waiters.md#portalnotexistswaiter)
