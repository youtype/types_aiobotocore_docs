# IoTSiteWiseClient

> [Index](../README.md) > [IoTSiteWise](./README.md) > IoTSiteWiseClient

!!! note ""

    Auto-generated documentation for [IoTSiteWise](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotsitewise.html#iotsitewise)
    type annotations stubs module [types-aiobotocore-iotsitewise](https://pypi.org/project/types-aiobotocore-iotsitewise/).

## IoTSiteWiseClient

Type annotations and code completion for `#!python session.create_client("iotsitewise")`
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotsitewise.html#IoTSiteWise.Client)

```python
# IoTSiteWiseClient usage example

from aiobotocore.session import get_session
from types_aiobotocore_iotsitewise.client import IoTSiteWiseClient

session = get_session()
async with session.create_client("iotsitewise") as client:
    client: IoTSiteWiseClient
```

## Exceptions


`aiobotocore` client exceptions are generated in runtime.
This class provides code completion for `#!python session.create_client("iotsitewise").exceptions` structure.

```python
# IoTSiteWiseClient.exceptions usage example

async with session.create_client("iotsitewise") as client:
    try:
        do_something(client)
    except (
            client.AccessDeniedException,
        client.ClientError,
        client.ConflictingOperationException,
        client.InternalFailureException,
        client.InvalidRequestException,
        client.LimitExceededException,
        client.PreconditionFailedException,
        client.QueryTimeoutException,
        client.ResourceAlreadyExistsException,
        client.ResourceNotFoundException,
        client.ServiceUnavailableException,
        client.ThrottlingException,
        client.TooManyTagsException,
        client.UnauthorizedException,
        client.ValidationException,
    ) as e:
        print(e)
```

```python
# IoTSiteWiseClient usage type checking example

from types_aiobotocore_iotsitewise.client import Exceptions

def handle_error(exc: Exceptions.AccessDeniedException) -> None:
    ...
```


## Methods


### can\_paginate



Type annotations and code completion for `#!python session.create_client("iotsitewise").can_paginate` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotsitewise/client/can_paginate.html)

```python
# can_paginate method definition

def can_paginate(
    self,
    operation_name: str,
) -> bool:
    ...
```


### generate\_presigned\_url



Type annotations and code completion for `#!python session.create_client("iotsitewise").generate_presigned_url` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotsitewise/client/generate_presigned_url.html)

```python
# generate_presigned_url method definition

await def generate_presigned_url(
    self,
    ClientMethod: str,
    Params: Mapping[str, Any] = ...,
    ExpiresIn: int = 3600,
    HttpMethod: str = ...,
) -> str:
    ...
```


### associate\_assets

Associates a child asset with the given parent asset through a hierarchy
defined in the parent asset's model.

Type annotations and code completion for `#!python session.create_client("iotsitewise").associate_assets` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotsitewise/client/associate_assets.html)

```python
# associate_assets method definition

await def associate_assets(
    self,
    *,
    assetId: str,
    hierarchyId: str,
    childAssetId: str,
    clientToken: str = ...,
) -> EmptyResponseMetadataTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef) 


```python
# associate_assets method usage example with argument unpacking

kwargs: AssociateAssetsRequestTypeDef = {  # (1)
    "assetId": ...,
    "hierarchyId": ...,
    "childAssetId": ...,
}

parent.associate_assets(**kwargs)
```

1. See [:material-code-braces: AssociateAssetsRequestTypeDef](./type_defs.md#associateassetsrequesttypedef) 

### associate\_time\_series\_to\_asset\_property

Associates a time series (data stream) with an asset property.

Type annotations and code completion for `#!python session.create_client("iotsitewise").associate_time_series_to_asset_property` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotsitewise/client/associate_time_series_to_asset_property.html)

```python
# associate_time_series_to_asset_property method definition

await def associate_time_series_to_asset_property(
    self,
    *,
    alias: str,
    assetId: str,
    propertyId: str,
    clientToken: str = ...,
) -> EmptyResponseMetadataTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef) 


```python
# associate_time_series_to_asset_property method usage example with argument unpacking

kwargs: AssociateTimeSeriesToAssetPropertyRequestTypeDef = {  # (1)
    "alias": ...,
    "assetId": ...,
    "propertyId": ...,
}

parent.associate_time_series_to_asset_property(**kwargs)
```

1. See [:material-code-braces: AssociateTimeSeriesToAssetPropertyRequestTypeDef](./type_defs.md#associatetimeseriestoassetpropertyrequesttypedef) 

### batch\_associate\_project\_assets

Associates a group (batch) of assets with an IoT SiteWise Monitor project.

Type annotations and code completion for `#!python session.create_client("iotsitewise").batch_associate_project_assets` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotsitewise/client/batch_associate_project_assets.html)

```python
# batch_associate_project_assets method definition

await def batch_associate_project_assets(
    self,
    *,
    projectId: str,
    assetIds: Sequence[str],
    clientToken: str = ...,
) -> BatchAssociateProjectAssetsResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: BatchAssociateProjectAssetsResponseTypeDef](./type_defs.md#batchassociateprojectassetsresponsetypedef) 


```python
# batch_associate_project_assets method usage example with argument unpacking

kwargs: BatchAssociateProjectAssetsRequestTypeDef = {  # (1)
    "projectId": ...,
    "assetIds": ...,
}

parent.batch_associate_project_assets(**kwargs)
```

1. See [:material-code-braces: BatchAssociateProjectAssetsRequestTypeDef](./type_defs.md#batchassociateprojectassetsrequesttypedef) 

### batch\_disassociate\_project\_assets

Disassociates a group (batch) of assets from an IoT SiteWise Monitor project.

Type annotations and code completion for `#!python session.create_client("iotsitewise").batch_disassociate_project_assets` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotsitewise/client/batch_disassociate_project_assets.html)

```python
# batch_disassociate_project_assets method definition

await def batch_disassociate_project_assets(
    self,
    *,
    projectId: str,
    assetIds: Sequence[str],
    clientToken: str = ...,
) -> BatchDisassociateProjectAssetsResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: BatchDisassociateProjectAssetsResponseTypeDef](./type_defs.md#batchdisassociateprojectassetsresponsetypedef) 


```python
# batch_disassociate_project_assets method usage example with argument unpacking

kwargs: BatchDisassociateProjectAssetsRequestTypeDef = {  # (1)
    "projectId": ...,
    "assetIds": ...,
}

parent.batch_disassociate_project_assets(**kwargs)
```

1. See [:material-code-braces: BatchDisassociateProjectAssetsRequestTypeDef](./type_defs.md#batchdisassociateprojectassetsrequesttypedef) 

### batch\_get\_asset\_property\_aggregates

Gets aggregated values (for example, average, minimum, and maximum) for one or
more asset properties.

Type annotations and code completion for `#!python session.create_client("iotsitewise").batch_get_asset_property_aggregates` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotsitewise/client/batch_get_asset_property_aggregates.html)

```python
# batch_get_asset_property_aggregates method definition

await def batch_get_asset_property_aggregates(
    self,
    *,
    entries: Sequence[BatchGetAssetPropertyAggregatesEntryTypeDef],  # (1)
    nextToken: str = ...,
    maxResults: int = ...,
) -> BatchGetAssetPropertyAggregatesResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: BatchGetAssetPropertyAggregatesEntryTypeDef](./type_defs.md#batchgetassetpropertyaggregatesentrytypedef) 
2. See [:material-code-braces: BatchGetAssetPropertyAggregatesResponseTypeDef](./type_defs.md#batchgetassetpropertyaggregatesresponsetypedef) 


```python
# batch_get_asset_property_aggregates method usage example with argument unpacking

kwargs: BatchGetAssetPropertyAggregatesRequestTypeDef = {  # (1)
    "entries": ...,
}

parent.batch_get_asset_property_aggregates(**kwargs)
```

1. See [:material-code-braces: BatchGetAssetPropertyAggregatesRequestTypeDef](./type_defs.md#batchgetassetpropertyaggregatesrequesttypedef) 

### batch\_get\_asset\_property\_value

Gets the current value for one or more asset properties.

Type annotations and code completion for `#!python session.create_client("iotsitewise").batch_get_asset_property_value` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotsitewise/client/batch_get_asset_property_value.html)

```python
# batch_get_asset_property_value method definition

await def batch_get_asset_property_value(
    self,
    *,
    entries: Sequence[BatchGetAssetPropertyValueEntryTypeDef],  # (1)
    nextToken: str = ...,
) -> BatchGetAssetPropertyValueResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: BatchGetAssetPropertyValueEntryTypeDef](./type_defs.md#batchgetassetpropertyvalueentrytypedef) 
2. See [:material-code-braces: BatchGetAssetPropertyValueResponseTypeDef](./type_defs.md#batchgetassetpropertyvalueresponsetypedef) 


```python
# batch_get_asset_property_value method usage example with argument unpacking

kwargs: BatchGetAssetPropertyValueRequestTypeDef = {  # (1)
    "entries": ...,
}

parent.batch_get_asset_property_value(**kwargs)
```

1. See [:material-code-braces: BatchGetAssetPropertyValueRequestTypeDef](./type_defs.md#batchgetassetpropertyvaluerequesttypedef) 

### batch\_get\_asset\_property\_value\_history

Gets the historical values for one or more asset properties.

Type annotations and code completion for `#!python session.create_client("iotsitewise").batch_get_asset_property_value_history` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotsitewise/client/batch_get_asset_property_value_history.html)

```python
# batch_get_asset_property_value_history method definition

await def batch_get_asset_property_value_history(
    self,
    *,
    entries: Sequence[BatchGetAssetPropertyValueHistoryEntryTypeDef],  # (1)
    nextToken: str = ...,
    maxResults: int = ...,
) -> BatchGetAssetPropertyValueHistoryResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: BatchGetAssetPropertyValueHistoryEntryTypeDef](./type_defs.md#batchgetassetpropertyvaluehistoryentrytypedef) 
2. See [:material-code-braces: BatchGetAssetPropertyValueHistoryResponseTypeDef](./type_defs.md#batchgetassetpropertyvaluehistoryresponsetypedef) 


```python
# batch_get_asset_property_value_history method usage example with argument unpacking

kwargs: BatchGetAssetPropertyValueHistoryRequestTypeDef = {  # (1)
    "entries": ...,
}

parent.batch_get_asset_property_value_history(**kwargs)
```

1. See [:material-code-braces: BatchGetAssetPropertyValueHistoryRequestTypeDef](./type_defs.md#batchgetassetpropertyvaluehistoryrequesttypedef) 

### batch\_put\_asset\_property\_value

Sends a list of asset property values to IoT SiteWise.

Type annotations and code completion for `#!python session.create_client("iotsitewise").batch_put_asset_property_value` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotsitewise/client/batch_put_asset_property_value.html)

```python
# batch_put_asset_property_value method definition

await def batch_put_asset_property_value(
    self,
    *,
    entries: Sequence[PutAssetPropertyValueEntryTypeDef],  # (1)
    enablePartialEntryProcessing: bool = ...,
) -> BatchPutAssetPropertyValueResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: PutAssetPropertyValueEntryTypeDef](./type_defs.md#putassetpropertyvalueentrytypedef) 
2. See [:material-code-braces: BatchPutAssetPropertyValueResponseTypeDef](./type_defs.md#batchputassetpropertyvalueresponsetypedef) 


```python
# batch_put_asset_property_value method usage example with argument unpacking

kwargs: BatchPutAssetPropertyValueRequestTypeDef = {  # (1)
    "entries": ...,
}

parent.batch_put_asset_property_value(**kwargs)
```

1. See [:material-code-braces: BatchPutAssetPropertyValueRequestTypeDef](./type_defs.md#batchputassetpropertyvaluerequesttypedef) 

### create\_access\_policy

Creates an access policy that grants the specified identity (IAM Identity
Center user, IAM Identity Center group, or IAM user) access to the specified
IoT SiteWise Monitor portal or project resource.

Type annotations and code completion for `#!python session.create_client("iotsitewise").create_access_policy` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotsitewise/client/create_access_policy.html)

```python
# create_access_policy method definition

await def create_access_policy(
    self,
    *,
    accessPolicyIdentity: IdentityTypeDef,  # (1)
    accessPolicyResource: ResourceTypeDef,  # (2)
    accessPolicyPermission: PermissionType,  # (3)
    clientToken: str = ...,
    tags: Mapping[str, str] = ...,
) -> CreateAccessPolicyResponseTypeDef:  # (4)
    ...
```

1. See [:material-code-braces: IdentityTypeDef](./type_defs.md#identitytypedef) 
2. See [:material-code-braces: ResourceTypeDef](./type_defs.md#resourcetypedef) 
3. See [:material-code-brackets: PermissionType](./literals.md#permissiontype) 
4. See [:material-code-braces: CreateAccessPolicyResponseTypeDef](./type_defs.md#createaccesspolicyresponsetypedef) 


```python
# create_access_policy method usage example with argument unpacking

kwargs: CreateAccessPolicyRequestTypeDef = {  # (1)
    "accessPolicyIdentity": ...,
    "accessPolicyResource": ...,
    "accessPolicyPermission": ...,
}

parent.create_access_policy(**kwargs)
```

1. See [:material-code-braces: CreateAccessPolicyRequestTypeDef](./type_defs.md#createaccesspolicyrequesttypedef) 

### create\_asset

Creates an asset from an existing asset model.

Type annotations and code completion for `#!python session.create_client("iotsitewise").create_asset` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotsitewise/client/create_asset.html)

```python
# create_asset method definition

await def create_asset(
    self,
    *,
    assetName: str,
    assetModelId: str,
    clientToken: str = ...,
    tags: Mapping[str, str] = ...,
    assetDescription: str = ...,
    assetId: str = ...,
    assetExternalId: str = ...,
) -> CreateAssetResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: CreateAssetResponseTypeDef](./type_defs.md#createassetresponsetypedef) 


```python
# create_asset method usage example with argument unpacking

kwargs: CreateAssetRequestTypeDef = {  # (1)
    "assetName": ...,
    "assetModelId": ...,
}

parent.create_asset(**kwargs)
```

1. See [:material-code-braces: CreateAssetRequestTypeDef](./type_defs.md#createassetrequesttypedef) 

### create\_asset\_model

Creates an asset model from specified property and hierarchy definitions.

Type annotations and code completion for `#!python session.create_client("iotsitewise").create_asset_model` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotsitewise/client/create_asset_model.html)

```python
# create_asset_model method definition

await def create_asset_model(
    self,
    *,
    assetModelName: str,
    assetModelType: AssetModelTypeType = ...,  # (1)
    assetModelId: str = ...,
    assetModelExternalId: str = ...,
    assetModelDescription: str = ...,
    assetModelProperties: Sequence[AssetModelPropertyDefinitionTypeDef] = ...,  # (2)
    assetModelHierarchies: Sequence[AssetModelHierarchyDefinitionTypeDef] = ...,  # (3)
    assetModelCompositeModels: Sequence[AssetModelCompositeModelDefinitionTypeDef] = ...,  # (4)
    clientToken: str = ...,
    tags: Mapping[str, str] = ...,
) -> CreateAssetModelResponseTypeDef:  # (5)
    ...
```

1. See [:material-code-brackets: AssetModelTypeType](./literals.md#assetmodeltypetype) 
2. See [:material-code-braces: AssetModelPropertyDefinitionTypeDef](./type_defs.md#assetmodelpropertydefinitiontypedef) 
3. See [:material-code-braces: AssetModelHierarchyDefinitionTypeDef](./type_defs.md#assetmodelhierarchydefinitiontypedef) 
4. See [:material-code-braces: AssetModelCompositeModelDefinitionTypeDef](./type_defs.md#assetmodelcompositemodeldefinitiontypedef) 
5. See [:material-code-braces: CreateAssetModelResponseTypeDef](./type_defs.md#createassetmodelresponsetypedef) 


```python
# create_asset_model method usage example with argument unpacking

kwargs: CreateAssetModelRequestTypeDef = {  # (1)
    "assetModelName": ...,
}

parent.create_asset_model(**kwargs)
```

1. See [:material-code-braces: CreateAssetModelRequestTypeDef](./type_defs.md#createassetmodelrequesttypedef) 

### create\_asset\_model\_composite\_model

Creates a custom composite model from specified property and hierarchy
definitions.

Type annotations and code completion for `#!python session.create_client("iotsitewise").create_asset_model_composite_model` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotsitewise/client/create_asset_model_composite_model.html)

```python
# create_asset_model_composite_model method definition

await def create_asset_model_composite_model(
    self,
    *,
    assetModelId: str,
    assetModelCompositeModelName: str,
    assetModelCompositeModelType: str,
    assetModelCompositeModelExternalId: str = ...,
    parentAssetModelCompositeModelId: str = ...,
    assetModelCompositeModelId: str = ...,
    assetModelCompositeModelDescription: str = ...,
    clientToken: str = ...,
    composedAssetModelId: str = ...,
    assetModelCompositeModelProperties: Sequence[AssetModelPropertyDefinitionTypeDef] = ...,  # (1)
    ifMatch: str = ...,
    ifNoneMatch: str = ...,
    matchForVersionType: AssetModelVersionTypeType = ...,  # (2)
) -> CreateAssetModelCompositeModelResponseTypeDef:  # (3)
    ...
```

1. See [:material-code-braces: AssetModelPropertyDefinitionTypeDef](./type_defs.md#assetmodelpropertydefinitiontypedef) 
2. See [:material-code-brackets: AssetModelVersionTypeType](./literals.md#assetmodelversiontypetype) 
3. See [:material-code-braces: CreateAssetModelCompositeModelResponseTypeDef](./type_defs.md#createassetmodelcompositemodelresponsetypedef) 


```python
# create_asset_model_composite_model method usage example with argument unpacking

kwargs: CreateAssetModelCompositeModelRequestTypeDef = {  # (1)
    "assetModelId": ...,
    "assetModelCompositeModelName": ...,
    "assetModelCompositeModelType": ...,
}

parent.create_asset_model_composite_model(**kwargs)
```

1. See [:material-code-braces: CreateAssetModelCompositeModelRequestTypeDef](./type_defs.md#createassetmodelcompositemodelrequesttypedef) 

### create\_bulk\_import\_job

Defines a job to ingest data to IoT SiteWise from Amazon S3.

Type annotations and code completion for `#!python session.create_client("iotsitewise").create_bulk_import_job` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotsitewise/client/create_bulk_import_job.html)

```python
# create_bulk_import_job method definition

await def create_bulk_import_job(
    self,
    *,
    jobName: str,
    jobRoleArn: str,
    files: Sequence[FileTypeDef],  # (1)
    errorReportLocation: ErrorReportLocationTypeDef,  # (2)
    jobConfiguration: JobConfigurationUnionTypeDef,  # (3)
    adaptiveIngestion: bool = ...,
    deleteFilesAfterImport: bool = ...,
) -> CreateBulkImportJobResponseTypeDef:  # (4)
    ...
```

1. See [:material-code-braces: FileTypeDef](./type_defs.md#filetypedef) 
2. See [:material-code-braces: ErrorReportLocationTypeDef](./type_defs.md#errorreportlocationtypedef) 
3. See [:material-code-braces: JobConfigurationTypeDef](./type_defs.md#jobconfigurationtypedef) [:material-code-braces: JobConfigurationOutputTypeDef](./type_defs.md#jobconfigurationoutputtypedef) 
4. See [:material-code-braces: CreateBulkImportJobResponseTypeDef](./type_defs.md#createbulkimportjobresponsetypedef) 


```python
# create_bulk_import_job method usage example with argument unpacking

kwargs: CreateBulkImportJobRequestTypeDef = {  # (1)
    "jobName": ...,
    "jobRoleArn": ...,
    "files": ...,
    "errorReportLocation": ...,
    "jobConfiguration": ...,
}

parent.create_bulk_import_job(**kwargs)
```

1. See [:material-code-braces: CreateBulkImportJobRequestTypeDef](./type_defs.md#createbulkimportjobrequesttypedef) 

### create\_dashboard

Creates a dashboard in an IoT SiteWise Monitor project.

Type annotations and code completion for `#!python session.create_client("iotsitewise").create_dashboard` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotsitewise/client/create_dashboard.html)

```python
# create_dashboard method definition

await def create_dashboard(
    self,
    *,
    projectId: str,
    dashboardName: str,
    dashboardDefinition: str,
    dashboardDescription: str = ...,
    clientToken: str = ...,
    tags: Mapping[str, str] = ...,
) -> CreateDashboardResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: CreateDashboardResponseTypeDef](./type_defs.md#createdashboardresponsetypedef) 


```python
# create_dashboard method usage example with argument unpacking

kwargs: CreateDashboardRequestTypeDef = {  # (1)
    "projectId": ...,
    "dashboardName": ...,
    "dashboardDefinition": ...,
}

parent.create_dashboard(**kwargs)
```

1. See [:material-code-braces: CreateDashboardRequestTypeDef](./type_defs.md#createdashboardrequesttypedef) 

### create\_dataset

Creates a dataset to connect an external datasource.

Type annotations and code completion for `#!python session.create_client("iotsitewise").create_dataset` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotsitewise/client/create_dataset.html)

```python
# create_dataset method definition

await def create_dataset(
    self,
    *,
    datasetName: str,
    datasetSource: DatasetSourceTypeDef,  # (1)
    datasetId: str = ...,
    datasetDescription: str = ...,
    clientToken: str = ...,
    tags: Mapping[str, str] = ...,
) -> CreateDatasetResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: DatasetSourceTypeDef](./type_defs.md#datasetsourcetypedef) 
2. See [:material-code-braces: CreateDatasetResponseTypeDef](./type_defs.md#createdatasetresponsetypedef) 


```python
# create_dataset method usage example with argument unpacking

kwargs: CreateDatasetRequestTypeDef = {  # (1)
    "datasetName": ...,
    "datasetSource": ...,
}

parent.create_dataset(**kwargs)
```

1. See [:material-code-braces: CreateDatasetRequestTypeDef](./type_defs.md#createdatasetrequesttypedef) 

### create\_gateway

Creates a gateway, which is a virtual or edge device that delivers industrial
data streams from local servers to IoT SiteWise.

Type annotations and code completion for `#!python session.create_client("iotsitewise").create_gateway` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotsitewise/client/create_gateway.html)

```python
# create_gateway method definition

await def create_gateway(
    self,
    *,
    gatewayName: str,
    gatewayPlatform: GatewayPlatformTypeDef,  # (1)
    tags: Mapping[str, str] = ...,
) -> CreateGatewayResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: GatewayPlatformTypeDef](./type_defs.md#gatewayplatformtypedef) 
2. See [:material-code-braces: CreateGatewayResponseTypeDef](./type_defs.md#creategatewayresponsetypedef) 


```python
# create_gateway method usage example with argument unpacking

kwargs: CreateGatewayRequestTypeDef = {  # (1)
    "gatewayName": ...,
    "gatewayPlatform": ...,
}

parent.create_gateway(**kwargs)
```

1. See [:material-code-braces: CreateGatewayRequestTypeDef](./type_defs.md#creategatewayrequesttypedef) 

### create\_portal

Creates a portal, which can contain projects and dashboards.

Type annotations and code completion for `#!python session.create_client("iotsitewise").create_portal` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotsitewise/client/create_portal.html)

```python
# create_portal method definition

await def create_portal(
    self,
    *,
    portalName: str,
    portalContactEmail: str,
    roleArn: str,
    portalDescription: str = ...,
    clientToken: str = ...,
    portalLogoImageFile: ImageFileTypeDef = ...,  # (1)
    tags: Mapping[str, str] = ...,
    portalAuthMode: AuthModeType = ...,  # (2)
    notificationSenderEmail: str = ...,
    alarms: AlarmsTypeDef = ...,  # (3)
    portalType: PortalTypeType = ...,  # (4)
    portalTypeConfiguration: Mapping[str, PortalTypeEntryUnionTypeDef] = ...,  # (5)
) -> CreatePortalResponseTypeDef:  # (6)
    ...
```

1. See [:material-code-braces: ImageFileTypeDef](./type_defs.md#imagefiletypedef) 
2. See [:material-code-brackets: AuthModeType](./literals.md#authmodetype) 
3. See [:material-code-braces: AlarmsTypeDef](./type_defs.md#alarmstypedef) 
4. See [:material-code-brackets: PortalTypeType](./literals.md#portaltypetype) 
5. See [:material-code-braces: PortalTypeEntryTypeDef](./type_defs.md#portaltypeentrytypedef) [:material-code-braces: PortalTypeEntryOutputTypeDef](./type_defs.md#portaltypeentryoutputtypedef) 
6. See [:material-code-braces: CreatePortalResponseTypeDef](./type_defs.md#createportalresponsetypedef) 


```python
# create_portal method usage example with argument unpacking

kwargs: CreatePortalRequestTypeDef = {  # (1)
    "portalName": ...,
    "portalContactEmail": ...,
    "roleArn": ...,
}

parent.create_portal(**kwargs)
```

1. See [:material-code-braces: CreatePortalRequestTypeDef](./type_defs.md#createportalrequesttypedef) 

### create\_project

Creates a project in the specified portal.

Type annotations and code completion for `#!python session.create_client("iotsitewise").create_project` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotsitewise/client/create_project.html)

```python
# create_project method definition

await def create_project(
    self,
    *,
    portalId: str,
    projectName: str,
    projectDescription: str = ...,
    clientToken: str = ...,
    tags: Mapping[str, str] = ...,
) -> CreateProjectResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: CreateProjectResponseTypeDef](./type_defs.md#createprojectresponsetypedef) 


```python
# create_project method usage example with argument unpacking

kwargs: CreateProjectRequestTypeDef = {  # (1)
    "portalId": ...,
    "projectName": ...,
}

parent.create_project(**kwargs)
```

1. See [:material-code-braces: CreateProjectRequestTypeDef](./type_defs.md#createprojectrequesttypedef) 

### delete\_access\_policy

Deletes an access policy that grants the specified identity access to the
specified IoT SiteWise Monitor resource.

Type annotations and code completion for `#!python session.create_client("iotsitewise").delete_access_policy` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotsitewise/client/delete_access_policy.html)

```python
# delete_access_policy method definition

await def delete_access_policy(
    self,
    *,
    accessPolicyId: str,
    clientToken: str = ...,
) -> Dict[str, Any]:
    ...
```



```python
# delete_access_policy method usage example with argument unpacking

kwargs: DeleteAccessPolicyRequestTypeDef = {  # (1)
    "accessPolicyId": ...,
}

parent.delete_access_policy(**kwargs)
```

1. See [:material-code-braces: DeleteAccessPolicyRequestTypeDef](./type_defs.md#deleteaccesspolicyrequesttypedef) 

### delete\_asset

Deletes an asset.

Type annotations and code completion for `#!python session.create_client("iotsitewise").delete_asset` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotsitewise/client/delete_asset.html)

```python
# delete_asset method definition

await def delete_asset(
    self,
    *,
    assetId: str,
    clientToken: str = ...,
) -> DeleteAssetResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DeleteAssetResponseTypeDef](./type_defs.md#deleteassetresponsetypedef) 


```python
# delete_asset method usage example with argument unpacking

kwargs: DeleteAssetRequestTypeDef = {  # (1)
    "assetId": ...,
}

parent.delete_asset(**kwargs)
```

1. See [:material-code-braces: DeleteAssetRequestTypeDef](./type_defs.md#deleteassetrequesttypedef) 

### delete\_asset\_model

Deletes an asset model.

Type annotations and code completion for `#!python session.create_client("iotsitewise").delete_asset_model` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotsitewise/client/delete_asset_model.html)

```python
# delete_asset_model method definition

await def delete_asset_model(
    self,
    *,
    assetModelId: str,
    clientToken: str = ...,
    ifMatch: str = ...,
    ifNoneMatch: str = ...,
    matchForVersionType: AssetModelVersionTypeType = ...,  # (1)
) -> DeleteAssetModelResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-brackets: AssetModelVersionTypeType](./literals.md#assetmodelversiontypetype) 
2. See [:material-code-braces: DeleteAssetModelResponseTypeDef](./type_defs.md#deleteassetmodelresponsetypedef) 


```python
# delete_asset_model method usage example with argument unpacking

kwargs: DeleteAssetModelRequestTypeDef = {  # (1)
    "assetModelId": ...,
}

parent.delete_asset_model(**kwargs)
```

1. See [:material-code-braces: DeleteAssetModelRequestTypeDef](./type_defs.md#deleteassetmodelrequesttypedef) 

### delete\_asset\_model\_composite\_model

Deletes a composite model.

Type annotations and code completion for `#!python session.create_client("iotsitewise").delete_asset_model_composite_model` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotsitewise/client/delete_asset_model_composite_model.html)

```python
# delete_asset_model_composite_model method definition

await def delete_asset_model_composite_model(
    self,
    *,
    assetModelId: str,
    assetModelCompositeModelId: str,
    clientToken: str = ...,
    ifMatch: str = ...,
    ifNoneMatch: str = ...,
    matchForVersionType: AssetModelVersionTypeType = ...,  # (1)
) -> DeleteAssetModelCompositeModelResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-brackets: AssetModelVersionTypeType](./literals.md#assetmodelversiontypetype) 
2. See [:material-code-braces: DeleteAssetModelCompositeModelResponseTypeDef](./type_defs.md#deleteassetmodelcompositemodelresponsetypedef) 


```python
# delete_asset_model_composite_model method usage example with argument unpacking

kwargs: DeleteAssetModelCompositeModelRequestTypeDef = {  # (1)
    "assetModelId": ...,
    "assetModelCompositeModelId": ...,
}

parent.delete_asset_model_composite_model(**kwargs)
```

1. See [:material-code-braces: DeleteAssetModelCompositeModelRequestTypeDef](./type_defs.md#deleteassetmodelcompositemodelrequesttypedef) 

### delete\_dashboard

Deletes a dashboard from IoT SiteWise Monitor.

Type annotations and code completion for `#!python session.create_client("iotsitewise").delete_dashboard` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotsitewise/client/delete_dashboard.html)

```python
# delete_dashboard method definition

await def delete_dashboard(
    self,
    *,
    dashboardId: str,
    clientToken: str = ...,
) -> Dict[str, Any]:
    ...
```



```python
# delete_dashboard method usage example with argument unpacking

kwargs: DeleteDashboardRequestTypeDef = {  # (1)
    "dashboardId": ...,
}

parent.delete_dashboard(**kwargs)
```

1. See [:material-code-braces: DeleteDashboardRequestTypeDef](./type_defs.md#deletedashboardrequesttypedef) 

### delete\_dataset

Deletes a dataset.

Type annotations and code completion for `#!python session.create_client("iotsitewise").delete_dataset` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotsitewise/client/delete_dataset.html)

```python
# delete_dataset method definition

await def delete_dataset(
    self,
    *,
    datasetId: str,
    clientToken: str = ...,
) -> DeleteDatasetResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DeleteDatasetResponseTypeDef](./type_defs.md#deletedatasetresponsetypedef) 


```python
# delete_dataset method usage example with argument unpacking

kwargs: DeleteDatasetRequestTypeDef = {  # (1)
    "datasetId": ...,
}

parent.delete_dataset(**kwargs)
```

1. See [:material-code-braces: DeleteDatasetRequestTypeDef](./type_defs.md#deletedatasetrequesttypedef) 

### delete\_gateway

Deletes a gateway from IoT SiteWise.

Type annotations and code completion for `#!python session.create_client("iotsitewise").delete_gateway` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotsitewise/client/delete_gateway.html)

```python
# delete_gateway method definition

await def delete_gateway(
    self,
    *,
    gatewayId: str,
) -> EmptyResponseMetadataTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef) 


```python
# delete_gateway method usage example with argument unpacking

kwargs: DeleteGatewayRequestTypeDef = {  # (1)
    "gatewayId": ...,
}

parent.delete_gateway(**kwargs)
```

1. See [:material-code-braces: DeleteGatewayRequestTypeDef](./type_defs.md#deletegatewayrequesttypedef) 

### delete\_portal

Deletes a portal from IoT SiteWise Monitor.

Type annotations and code completion for `#!python session.create_client("iotsitewise").delete_portal` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotsitewise/client/delete_portal.html)

```python
# delete_portal method definition

await def delete_portal(
    self,
    *,
    portalId: str,
    clientToken: str = ...,
) -> DeletePortalResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DeletePortalResponseTypeDef](./type_defs.md#deleteportalresponsetypedef) 


```python
# delete_portal method usage example with argument unpacking

kwargs: DeletePortalRequestTypeDef = {  # (1)
    "portalId": ...,
}

parent.delete_portal(**kwargs)
```

1. See [:material-code-braces: DeletePortalRequestTypeDef](./type_defs.md#deleteportalrequesttypedef) 

### delete\_project

Deletes a project from IoT SiteWise Monitor.

Type annotations and code completion for `#!python session.create_client("iotsitewise").delete_project` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotsitewise/client/delete_project.html)

```python
# delete_project method definition

await def delete_project(
    self,
    *,
    projectId: str,
    clientToken: str = ...,
) -> Dict[str, Any]:
    ...
```



```python
# delete_project method usage example with argument unpacking

kwargs: DeleteProjectRequestTypeDef = {  # (1)
    "projectId": ...,
}

parent.delete_project(**kwargs)
```

1. See [:material-code-braces: DeleteProjectRequestTypeDef](./type_defs.md#deleteprojectrequesttypedef) 

### delete\_time\_series

Deletes a time series (data stream).

Type annotations and code completion for `#!python session.create_client("iotsitewise").delete_time_series` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotsitewise/client/delete_time_series.html)

```python
# delete_time_series method definition

await def delete_time_series(
    self,
    *,
    alias: str = ...,
    assetId: str = ...,
    propertyId: str = ...,
    clientToken: str = ...,
) -> EmptyResponseMetadataTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef) 


```python
# delete_time_series method usage example with argument unpacking

kwargs: DeleteTimeSeriesRequestTypeDef = {  # (1)
    "alias": ...,
}

parent.delete_time_series(**kwargs)
```

1. See [:material-code-braces: DeleteTimeSeriesRequestTypeDef](./type_defs.md#deletetimeseriesrequesttypedef) 

### describe\_access\_policy

Describes an access policy, which specifies an identity's access to an IoT
SiteWise Monitor portal or project.

Type annotations and code completion for `#!python session.create_client("iotsitewise").describe_access_policy` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotsitewise/client/describe_access_policy.html)

```python
# describe_access_policy method definition

await def describe_access_policy(
    self,
    *,
    accessPolicyId: str,
) -> DescribeAccessPolicyResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DescribeAccessPolicyResponseTypeDef](./type_defs.md#describeaccesspolicyresponsetypedef) 


```python
# describe_access_policy method usage example with argument unpacking

kwargs: DescribeAccessPolicyRequestTypeDef = {  # (1)
    "accessPolicyId": ...,
}

parent.describe_access_policy(**kwargs)
```

1. See [:material-code-braces: DescribeAccessPolicyRequestTypeDef](./type_defs.md#describeaccesspolicyrequesttypedef) 

### describe\_action

Retrieves information about an action.

Type annotations and code completion for `#!python session.create_client("iotsitewise").describe_action` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotsitewise/client/describe_action.html)

```python
# describe_action method definition

await def describe_action(
    self,
    *,
    actionId: str,
) -> DescribeActionResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DescribeActionResponseTypeDef](./type_defs.md#describeactionresponsetypedef) 


```python
# describe_action method usage example with argument unpacking

kwargs: DescribeActionRequestTypeDef = {  # (1)
    "actionId": ...,
}

parent.describe_action(**kwargs)
```

1. See [:material-code-braces: DescribeActionRequestTypeDef](./type_defs.md#describeactionrequesttypedef) 

### describe\_asset

Retrieves information about an asset.

Type annotations and code completion for `#!python session.create_client("iotsitewise").describe_asset` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotsitewise/client/describe_asset.html)

```python
# describe_asset method definition

await def describe_asset(
    self,
    *,
    assetId: str,
    excludeProperties: bool = ...,
) -> DescribeAssetResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DescribeAssetResponseTypeDef](./type_defs.md#describeassetresponsetypedef) 


```python
# describe_asset method usage example with argument unpacking

kwargs: DescribeAssetRequestTypeDef = {  # (1)
    "assetId": ...,
}

parent.describe_asset(**kwargs)
```

1. See [:material-code-braces: DescribeAssetRequestTypeDef](./type_defs.md#describeassetrequesttypedef) 

### describe\_asset\_composite\_model

Retrieves information about an asset composite model (also known as an asset
component).

Type annotations and code completion for `#!python session.create_client("iotsitewise").describe_asset_composite_model` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotsitewise/client/describe_asset_composite_model.html)

```python
# describe_asset_composite_model method definition

await def describe_asset_composite_model(
    self,
    *,
    assetId: str,
    assetCompositeModelId: str,
) -> DescribeAssetCompositeModelResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DescribeAssetCompositeModelResponseTypeDef](./type_defs.md#describeassetcompositemodelresponsetypedef) 


```python
# describe_asset_composite_model method usage example with argument unpacking

kwargs: DescribeAssetCompositeModelRequestTypeDef = {  # (1)
    "assetId": ...,
    "assetCompositeModelId": ...,
}

parent.describe_asset_composite_model(**kwargs)
```

1. See [:material-code-braces: DescribeAssetCompositeModelRequestTypeDef](./type_defs.md#describeassetcompositemodelrequesttypedef) 

### describe\_asset\_model

Retrieves information about an asset model.

Type annotations and code completion for `#!python session.create_client("iotsitewise").describe_asset_model` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotsitewise/client/describe_asset_model.html)

```python
# describe_asset_model method definition

await def describe_asset_model(
    self,
    *,
    assetModelId: str,
    excludeProperties: bool = ...,
    assetModelVersion: str = ...,
) -> DescribeAssetModelResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DescribeAssetModelResponseTypeDef](./type_defs.md#describeassetmodelresponsetypedef) 


```python
# describe_asset_model method usage example with argument unpacking

kwargs: DescribeAssetModelRequestTypeDef = {  # (1)
    "assetModelId": ...,
}

parent.describe_asset_model(**kwargs)
```

1. See [:material-code-braces: DescribeAssetModelRequestTypeDef](./type_defs.md#describeassetmodelrequesttypedef) 

### describe\_asset\_model\_composite\_model

Retrieves information about an asset model composite model (also known as an
asset model component).

Type annotations and code completion for `#!python session.create_client("iotsitewise").describe_asset_model_composite_model` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotsitewise/client/describe_asset_model_composite_model.html)

```python
# describe_asset_model_composite_model method definition

await def describe_asset_model_composite_model(
    self,
    *,
    assetModelId: str,
    assetModelCompositeModelId: str,
    assetModelVersion: str = ...,
) -> DescribeAssetModelCompositeModelResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DescribeAssetModelCompositeModelResponseTypeDef](./type_defs.md#describeassetmodelcompositemodelresponsetypedef) 


```python
# describe_asset_model_composite_model method usage example with argument unpacking

kwargs: DescribeAssetModelCompositeModelRequestTypeDef = {  # (1)
    "assetModelId": ...,
    "assetModelCompositeModelId": ...,
}

parent.describe_asset_model_composite_model(**kwargs)
```

1. See [:material-code-braces: DescribeAssetModelCompositeModelRequestTypeDef](./type_defs.md#describeassetmodelcompositemodelrequesttypedef) 

### describe\_asset\_property

Retrieves information about an asset property.

Type annotations and code completion for `#!python session.create_client("iotsitewise").describe_asset_property` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotsitewise/client/describe_asset_property.html)

```python
# describe_asset_property method definition

await def describe_asset_property(
    self,
    *,
    assetId: str,
    propertyId: str,
) -> DescribeAssetPropertyResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DescribeAssetPropertyResponseTypeDef](./type_defs.md#describeassetpropertyresponsetypedef) 


```python
# describe_asset_property method usage example with argument unpacking

kwargs: DescribeAssetPropertyRequestTypeDef = {  # (1)
    "assetId": ...,
    "propertyId": ...,
}

parent.describe_asset_property(**kwargs)
```

1. See [:material-code-braces: DescribeAssetPropertyRequestTypeDef](./type_defs.md#describeassetpropertyrequesttypedef) 

### describe\_bulk\_import\_job

Retrieves information about a bulk import job request.

Type annotations and code completion for `#!python session.create_client("iotsitewise").describe_bulk_import_job` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotsitewise/client/describe_bulk_import_job.html)

```python
# describe_bulk_import_job method definition

await def describe_bulk_import_job(
    self,
    *,
    jobId: str,
) -> DescribeBulkImportJobResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DescribeBulkImportJobResponseTypeDef](./type_defs.md#describebulkimportjobresponsetypedef) 


```python
# describe_bulk_import_job method usage example with argument unpacking

kwargs: DescribeBulkImportJobRequestTypeDef = {  # (1)
    "jobId": ...,
}

parent.describe_bulk_import_job(**kwargs)
```

1. See [:material-code-braces: DescribeBulkImportJobRequestTypeDef](./type_defs.md#describebulkimportjobrequesttypedef) 

### describe\_dashboard

Retrieves information about a dashboard.

Type annotations and code completion for `#!python session.create_client("iotsitewise").describe_dashboard` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotsitewise/client/describe_dashboard.html)

```python
# describe_dashboard method definition

await def describe_dashboard(
    self,
    *,
    dashboardId: str,
) -> DescribeDashboardResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DescribeDashboardResponseTypeDef](./type_defs.md#describedashboardresponsetypedef) 


```python
# describe_dashboard method usage example with argument unpacking

kwargs: DescribeDashboardRequestTypeDef = {  # (1)
    "dashboardId": ...,
}

parent.describe_dashboard(**kwargs)
```

1. See [:material-code-braces: DescribeDashboardRequestTypeDef](./type_defs.md#describedashboardrequesttypedef) 

### describe\_dataset

Retrieves information about a dataset.

Type annotations and code completion for `#!python session.create_client("iotsitewise").describe_dataset` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotsitewise/client/describe_dataset.html)

```python
# describe_dataset method definition

await def describe_dataset(
    self,
    *,
    datasetId: str,
) -> DescribeDatasetResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DescribeDatasetResponseTypeDef](./type_defs.md#describedatasetresponsetypedef) 


```python
# describe_dataset method usage example with argument unpacking

kwargs: DescribeDatasetRequestTypeDef = {  # (1)
    "datasetId": ...,
}

parent.describe_dataset(**kwargs)
```

1. See [:material-code-braces: DescribeDatasetRequestTypeDef](./type_defs.md#describedatasetrequesttypedef) 

### describe\_default\_encryption\_configuration

Retrieves information about the default encryption configuration for the Amazon
Web Services account in the default or specified Region.

Type annotations and code completion for `#!python session.create_client("iotsitewise").describe_default_encryption_configuration` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotsitewise/client/describe_default_encryption_configuration.html)

```python
# describe_default_encryption_configuration method definition

await def describe_default_encryption_configuration(
    self,
) -> DescribeDefaultEncryptionConfigurationResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DescribeDefaultEncryptionConfigurationResponseTypeDef](./type_defs.md#describedefaultencryptionconfigurationresponsetypedef) 

### describe\_gateway

Retrieves information about a gateway.

Type annotations and code completion for `#!python session.create_client("iotsitewise").describe_gateway` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotsitewise/client/describe_gateway.html)

```python
# describe_gateway method definition

await def describe_gateway(
    self,
    *,
    gatewayId: str,
) -> DescribeGatewayResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DescribeGatewayResponseTypeDef](./type_defs.md#describegatewayresponsetypedef) 


```python
# describe_gateway method usage example with argument unpacking

kwargs: DescribeGatewayRequestTypeDef = {  # (1)
    "gatewayId": ...,
}

parent.describe_gateway(**kwargs)
```

1. See [:material-code-braces: DescribeGatewayRequestTypeDef](./type_defs.md#describegatewayrequesttypedef) 

### describe\_gateway\_capability\_configuration

Retrieves information about a gateway capability configuration.

Type annotations and code completion for `#!python session.create_client("iotsitewise").describe_gateway_capability_configuration` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotsitewise/client/describe_gateway_capability_configuration.html)

```python
# describe_gateway_capability_configuration method definition

await def describe_gateway_capability_configuration(
    self,
    *,
    gatewayId: str,
    capabilityNamespace: str,
) -> DescribeGatewayCapabilityConfigurationResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DescribeGatewayCapabilityConfigurationResponseTypeDef](./type_defs.md#describegatewaycapabilityconfigurationresponsetypedef) 


```python
# describe_gateway_capability_configuration method usage example with argument unpacking

kwargs: DescribeGatewayCapabilityConfigurationRequestTypeDef = {  # (1)
    "gatewayId": ...,
    "capabilityNamespace": ...,
}

parent.describe_gateway_capability_configuration(**kwargs)
```

1. See [:material-code-braces: DescribeGatewayCapabilityConfigurationRequestTypeDef](./type_defs.md#describegatewaycapabilityconfigurationrequesttypedef) 

### describe\_logging\_options

Retrieves the current IoT SiteWise logging options.

Type annotations and code completion for `#!python session.create_client("iotsitewise").describe_logging_options` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotsitewise/client/describe_logging_options.html)

```python
# describe_logging_options method definition

await def describe_logging_options(
    self,
) -> DescribeLoggingOptionsResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DescribeLoggingOptionsResponseTypeDef](./type_defs.md#describeloggingoptionsresponsetypedef) 

### describe\_portal

Retrieves information about a portal.

Type annotations and code completion for `#!python session.create_client("iotsitewise").describe_portal` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotsitewise/client/describe_portal.html)

```python
# describe_portal method definition

await def describe_portal(
    self,
    *,
    portalId: str,
) -> DescribePortalResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DescribePortalResponseTypeDef](./type_defs.md#describeportalresponsetypedef) 


```python
# describe_portal method usage example with argument unpacking

kwargs: DescribePortalRequestTypeDef = {  # (1)
    "portalId": ...,
}

parent.describe_portal(**kwargs)
```

1. See [:material-code-braces: DescribePortalRequestTypeDef](./type_defs.md#describeportalrequesttypedef) 

### describe\_project

Retrieves information about a project.

Type annotations and code completion for `#!python session.create_client("iotsitewise").describe_project` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotsitewise/client/describe_project.html)

```python
# describe_project method definition

await def describe_project(
    self,
    *,
    projectId: str,
) -> DescribeProjectResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DescribeProjectResponseTypeDef](./type_defs.md#describeprojectresponsetypedef) 


```python
# describe_project method usage example with argument unpacking

kwargs: DescribeProjectRequestTypeDef = {  # (1)
    "projectId": ...,
}

parent.describe_project(**kwargs)
```

1. See [:material-code-braces: DescribeProjectRequestTypeDef](./type_defs.md#describeprojectrequesttypedef) 

### describe\_storage\_configuration

Retrieves information about the storage configuration for IoT SiteWise.

Type annotations and code completion for `#!python session.create_client("iotsitewise").describe_storage_configuration` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotsitewise/client/describe_storage_configuration.html)

```python
# describe_storage_configuration method definition

await def describe_storage_configuration(
    self,
) -> DescribeStorageConfigurationResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DescribeStorageConfigurationResponseTypeDef](./type_defs.md#describestorageconfigurationresponsetypedef) 

### describe\_time\_series

Retrieves information about a time series (data stream).

Type annotations and code completion for `#!python session.create_client("iotsitewise").describe_time_series` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotsitewise/client/describe_time_series.html)

```python
# describe_time_series method definition

await def describe_time_series(
    self,
    *,
    alias: str = ...,
    assetId: str = ...,
    propertyId: str = ...,
) -> DescribeTimeSeriesResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DescribeTimeSeriesResponseTypeDef](./type_defs.md#describetimeseriesresponsetypedef) 


```python
# describe_time_series method usage example with argument unpacking

kwargs: DescribeTimeSeriesRequestTypeDef = {  # (1)
    "alias": ...,
}

parent.describe_time_series(**kwargs)
```

1. See [:material-code-braces: DescribeTimeSeriesRequestTypeDef](./type_defs.md#describetimeseriesrequesttypedef) 

### disassociate\_assets

Disassociates a child asset from the given parent asset through a hierarchy
defined in the parent asset's model.

Type annotations and code completion for `#!python session.create_client("iotsitewise").disassociate_assets` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotsitewise/client/disassociate_assets.html)

```python
# disassociate_assets method definition

await def disassociate_assets(
    self,
    *,
    assetId: str,
    hierarchyId: str,
    childAssetId: str,
    clientToken: str = ...,
) -> EmptyResponseMetadataTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef) 


```python
# disassociate_assets method usage example with argument unpacking

kwargs: DisassociateAssetsRequestTypeDef = {  # (1)
    "assetId": ...,
    "hierarchyId": ...,
    "childAssetId": ...,
}

parent.disassociate_assets(**kwargs)
```

1. See [:material-code-braces: DisassociateAssetsRequestTypeDef](./type_defs.md#disassociateassetsrequesttypedef) 

### disassociate\_time\_series\_from\_asset\_property

Disassociates a time series (data stream) from an asset property.

Type annotations and code completion for `#!python session.create_client("iotsitewise").disassociate_time_series_from_asset_property` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotsitewise/client/disassociate_time_series_from_asset_property.html)

```python
# disassociate_time_series_from_asset_property method definition

await def disassociate_time_series_from_asset_property(
    self,
    *,
    alias: str,
    assetId: str,
    propertyId: str,
    clientToken: str = ...,
) -> EmptyResponseMetadataTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef) 


```python
# disassociate_time_series_from_asset_property method usage example with argument unpacking

kwargs: DisassociateTimeSeriesFromAssetPropertyRequestTypeDef = {  # (1)
    "alias": ...,
    "assetId": ...,
    "propertyId": ...,
}

parent.disassociate_time_series_from_asset_property(**kwargs)
```

1. See [:material-code-braces: DisassociateTimeSeriesFromAssetPropertyRequestTypeDef](./type_defs.md#disassociatetimeseriesfromassetpropertyrequesttypedef) 

### execute\_action

Executes an action on a target resource.

Type annotations and code completion for `#!python session.create_client("iotsitewise").execute_action` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotsitewise/client/execute_action.html)

```python
# execute_action method definition

await def execute_action(
    self,
    *,
    targetResource: TargetResourceTypeDef,  # (1)
    actionDefinitionId: str,
    actionPayload: ActionPayloadTypeDef,  # (2)
    clientToken: str = ...,
) -> ExecuteActionResponseTypeDef:  # (3)
    ...
```

1. See [:material-code-braces: TargetResourceTypeDef](./type_defs.md#targetresourcetypedef) 
2. See [:material-code-braces: ActionPayloadTypeDef](./type_defs.md#actionpayloadtypedef) 
3. See [:material-code-braces: ExecuteActionResponseTypeDef](./type_defs.md#executeactionresponsetypedef) 


```python
# execute_action method usage example with argument unpacking

kwargs: ExecuteActionRequestTypeDef = {  # (1)
    "targetResource": ...,
    "actionDefinitionId": ...,
    "actionPayload": ...,
}

parent.execute_action(**kwargs)
```

1. See [:material-code-braces: ExecuteActionRequestTypeDef](./type_defs.md#executeactionrequesttypedef) 

### execute\_query

Run SQL queries to retrieve metadata and time-series data from asset models,
assets, measurements, metrics, transforms, and aggregates.

Type annotations and code completion for `#!python session.create_client("iotsitewise").execute_query` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotsitewise/client/execute_query.html)

```python
# execute_query method definition

await def execute_query(
    self,
    *,
    queryStatement: str,
    nextToken: str = ...,
    maxResults: int = ...,
    clientToken: str = ...,
) -> ExecuteQueryResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ExecuteQueryResponseTypeDef](./type_defs.md#executequeryresponsetypedef) 


```python
# execute_query method usage example with argument unpacking

kwargs: ExecuteQueryRequestTypeDef = {  # (1)
    "queryStatement": ...,
}

parent.execute_query(**kwargs)
```

1. See [:material-code-braces: ExecuteQueryRequestTypeDef](./type_defs.md#executequeryrequesttypedef) 

### get\_asset\_property\_aggregates

Gets aggregated values for an asset property.

Type annotations and code completion for `#!python session.create_client("iotsitewise").get_asset_property_aggregates` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotsitewise/client/get_asset_property_aggregates.html)

```python
# get_asset_property_aggregates method definition

await def get_asset_property_aggregates(
    self,
    *,
    aggregateTypes: Sequence[AggregateTypeType],  # (1)
    resolution: str,
    startDate: TimestampTypeDef,
    endDate: TimestampTypeDef,
    assetId: str = ...,
    propertyId: str = ...,
    propertyAlias: str = ...,
    qualities: Sequence[QualityType] = ...,  # (2)
    timeOrdering: TimeOrderingType = ...,  # (3)
    nextToken: str = ...,
    maxResults: int = ...,
) -> GetAssetPropertyAggregatesResponseTypeDef:  # (4)
    ...
```

1. See [:material-code-brackets: AggregateTypeType](./literals.md#aggregatetypetype) 
2. See [:material-code-brackets: QualityType](./literals.md#qualitytype) 
3. See [:material-code-brackets: TimeOrderingType](./literals.md#timeorderingtype) 
4. See [:material-code-braces: GetAssetPropertyAggregatesResponseTypeDef](./type_defs.md#getassetpropertyaggregatesresponsetypedef) 


```python
# get_asset_property_aggregates method usage example with argument unpacking

kwargs: GetAssetPropertyAggregatesRequestTypeDef = {  # (1)
    "aggregateTypes": ...,
    "resolution": ...,
    "startDate": ...,
    "endDate": ...,
}

parent.get_asset_property_aggregates(**kwargs)
```

1. See [:material-code-braces: GetAssetPropertyAggregatesRequestTypeDef](./type_defs.md#getassetpropertyaggregatesrequesttypedef) 

### get\_asset\_property\_value

Gets an asset property's current value.

Type annotations and code completion for `#!python session.create_client("iotsitewise").get_asset_property_value` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotsitewise/client/get_asset_property_value.html)

```python
# get_asset_property_value method definition

await def get_asset_property_value(
    self,
    *,
    assetId: str = ...,
    propertyId: str = ...,
    propertyAlias: str = ...,
) -> GetAssetPropertyValueResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetAssetPropertyValueResponseTypeDef](./type_defs.md#getassetpropertyvalueresponsetypedef) 


```python
# get_asset_property_value method usage example with argument unpacking

kwargs: GetAssetPropertyValueRequestTypeDef = {  # (1)
    "assetId": ...,
}

parent.get_asset_property_value(**kwargs)
```

1. See [:material-code-braces: GetAssetPropertyValueRequestTypeDef](./type_defs.md#getassetpropertyvaluerequesttypedef) 

### get\_asset\_property\_value\_history

Gets the history of an asset property's values.

Type annotations and code completion for `#!python session.create_client("iotsitewise").get_asset_property_value_history` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotsitewise/client/get_asset_property_value_history.html)

```python
# get_asset_property_value_history method definition

await def get_asset_property_value_history(
    self,
    *,
    assetId: str = ...,
    propertyId: str = ...,
    propertyAlias: str = ...,
    startDate: TimestampTypeDef = ...,
    endDate: TimestampTypeDef = ...,
    qualities: Sequence[QualityType] = ...,  # (1)
    timeOrdering: TimeOrderingType = ...,  # (2)
    nextToken: str = ...,
    maxResults: int = ...,
) -> GetAssetPropertyValueHistoryResponseTypeDef:  # (3)
    ...
```

1. See [:material-code-brackets: QualityType](./literals.md#qualitytype) 
2. See [:material-code-brackets: TimeOrderingType](./literals.md#timeorderingtype) 
3. See [:material-code-braces: GetAssetPropertyValueHistoryResponseTypeDef](./type_defs.md#getassetpropertyvaluehistoryresponsetypedef) 


```python
# get_asset_property_value_history method usage example with argument unpacking

kwargs: GetAssetPropertyValueHistoryRequestTypeDef = {  # (1)
    "assetId": ...,
}

parent.get_asset_property_value_history(**kwargs)
```

1. See [:material-code-braces: GetAssetPropertyValueHistoryRequestTypeDef](./type_defs.md#getassetpropertyvaluehistoryrequesttypedef) 

### get\_interpolated\_asset\_property\_values

Get interpolated values for an asset property for a specified time interval,
during a period of time.

Type annotations and code completion for `#!python session.create_client("iotsitewise").get_interpolated_asset_property_values` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotsitewise/client/get_interpolated_asset_property_values.html)

```python
# get_interpolated_asset_property_values method definition

await def get_interpolated_asset_property_values(
    self,
    *,
    startTimeInSeconds: int,
    endTimeInSeconds: int,
    quality: QualityType,  # (1)
    intervalInSeconds: int,
    type: str,
    assetId: str = ...,
    propertyId: str = ...,
    propertyAlias: str = ...,
    startTimeOffsetInNanos: int = ...,
    endTimeOffsetInNanos: int = ...,
    nextToken: str = ...,
    maxResults: int = ...,
    intervalWindowInSeconds: int = ...,
) -> GetInterpolatedAssetPropertyValuesResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-brackets: QualityType](./literals.md#qualitytype) 
2. See [:material-code-braces: GetInterpolatedAssetPropertyValuesResponseTypeDef](./type_defs.md#getinterpolatedassetpropertyvaluesresponsetypedef) 


```python
# get_interpolated_asset_property_values method usage example with argument unpacking

kwargs: GetInterpolatedAssetPropertyValuesRequestTypeDef = {  # (1)
    "startTimeInSeconds": ...,
    "endTimeInSeconds": ...,
    "quality": ...,
    "intervalInSeconds": ...,
    "type": ...,
}

parent.get_interpolated_asset_property_values(**kwargs)
```

1. See [:material-code-braces: GetInterpolatedAssetPropertyValuesRequestTypeDef](./type_defs.md#getinterpolatedassetpropertyvaluesrequesttypedef) 

### invoke\_assistant

Invokes SiteWise Assistant to start or continue a conversation.

Type annotations and code completion for `#!python session.create_client("iotsitewise").invoke_assistant` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotsitewise/client/invoke_assistant.html)

```python
# invoke_assistant method definition

await def invoke_assistant(
    self,
    *,
    message: str,
    conversationId: str = ...,
    enableTrace: bool = ...,
) -> InvokeAssistantResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: InvokeAssistantResponseTypeDef](./type_defs.md#invokeassistantresponsetypedef) 


```python
# invoke_assistant method usage example with argument unpacking

kwargs: InvokeAssistantRequestTypeDef = {  # (1)
    "message": ...,
}

parent.invoke_assistant(**kwargs)
```

1. See [:material-code-braces: InvokeAssistantRequestTypeDef](./type_defs.md#invokeassistantrequesttypedef) 

### list\_access\_policies

Retrieves a paginated list of access policies for an identity (an IAM Identity
Center user, an IAM Identity Center group, or an IAM user) or an IoT SiteWise
Monitor resource (a portal or project).

Type annotations and code completion for `#!python session.create_client("iotsitewise").list_access_policies` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotsitewise/client/list_access_policies.html)

```python
# list_access_policies method definition

await def list_access_policies(
    self,
    *,
    identityType: IdentityTypeType = ...,  # (1)
    identityId: str = ...,
    resourceType: ResourceTypeType = ...,  # (2)
    resourceId: str = ...,
    iamArn: str = ...,
    nextToken: str = ...,
    maxResults: int = ...,
) -> ListAccessPoliciesResponseTypeDef:  # (3)
    ...
```

1. See [:material-code-brackets: IdentityTypeType](./literals.md#identitytypetype) 
2. See [:material-code-brackets: ResourceTypeType](./literals.md#resourcetypetype) 
3. See [:material-code-braces: ListAccessPoliciesResponseTypeDef](./type_defs.md#listaccesspoliciesresponsetypedef) 


```python
# list_access_policies method usage example with argument unpacking

kwargs: ListAccessPoliciesRequestTypeDef = {  # (1)
    "identityType": ...,
}

parent.list_access_policies(**kwargs)
```

1. See [:material-code-braces: ListAccessPoliciesRequestTypeDef](./type_defs.md#listaccesspoliciesrequesttypedef) 

### list\_actions

Retrieves a paginated list of actions for a specific target resource.

Type annotations and code completion for `#!python session.create_client("iotsitewise").list_actions` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotsitewise/client/list_actions.html)

```python
# list_actions method definition

await def list_actions(
    self,
    *,
    targetResourceType: TargetResourceTypeType,  # (1)
    targetResourceId: str,
    nextToken: str = ...,
    maxResults: int = ...,
) -> ListActionsResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-brackets: TargetResourceTypeType](./literals.md#targetresourcetypetype) 
2. See [:material-code-braces: ListActionsResponseTypeDef](./type_defs.md#listactionsresponsetypedef) 


```python
# list_actions method usage example with argument unpacking

kwargs: ListActionsRequestTypeDef = {  # (1)
    "targetResourceType": ...,
    "targetResourceId": ...,
}

parent.list_actions(**kwargs)
```

1. See [:material-code-braces: ListActionsRequestTypeDef](./type_defs.md#listactionsrequesttypedef) 

### list\_asset\_model\_composite\_models

Retrieves a paginated list of composite models associated with the asset model.

Type annotations and code completion for `#!python session.create_client("iotsitewise").list_asset_model_composite_models` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotsitewise/client/list_asset_model_composite_models.html)

```python
# list_asset_model_composite_models method definition

await def list_asset_model_composite_models(
    self,
    *,
    assetModelId: str,
    nextToken: str = ...,
    maxResults: int = ...,
    assetModelVersion: str = ...,
) -> ListAssetModelCompositeModelsResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListAssetModelCompositeModelsResponseTypeDef](./type_defs.md#listassetmodelcompositemodelsresponsetypedef) 


```python
# list_asset_model_composite_models method usage example with argument unpacking

kwargs: ListAssetModelCompositeModelsRequestTypeDef = {  # (1)
    "assetModelId": ...,
}

parent.list_asset_model_composite_models(**kwargs)
```

1. See [:material-code-braces: ListAssetModelCompositeModelsRequestTypeDef](./type_defs.md#listassetmodelcompositemodelsrequesttypedef) 

### list\_asset\_model\_properties

Retrieves a paginated list of properties associated with an asset model.

Type annotations and code completion for `#!python session.create_client("iotsitewise").list_asset_model_properties` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotsitewise/client/list_asset_model_properties.html)

```python
# list_asset_model_properties method definition

await def list_asset_model_properties(
    self,
    *,
    assetModelId: str,
    nextToken: str = ...,
    maxResults: int = ...,
    filter: ListAssetModelPropertiesFilterType = ...,  # (1)
    assetModelVersion: str = ...,
) -> ListAssetModelPropertiesResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-brackets: ListAssetModelPropertiesFilterType](./literals.md#listassetmodelpropertiesfiltertype) 
2. See [:material-code-braces: ListAssetModelPropertiesResponseTypeDef](./type_defs.md#listassetmodelpropertiesresponsetypedef) 


```python
# list_asset_model_properties method usage example with argument unpacking

kwargs: ListAssetModelPropertiesRequestTypeDef = {  # (1)
    "assetModelId": ...,
}

parent.list_asset_model_properties(**kwargs)
```

1. See [:material-code-braces: ListAssetModelPropertiesRequestTypeDef](./type_defs.md#listassetmodelpropertiesrequesttypedef) 

### list\_asset\_models

Retrieves a paginated list of summaries of all asset models.

Type annotations and code completion for `#!python session.create_client("iotsitewise").list_asset_models` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotsitewise/client/list_asset_models.html)

```python
# list_asset_models method definition

await def list_asset_models(
    self,
    *,
    assetModelTypes: Sequence[AssetModelTypeType] = ...,  # (1)
    nextToken: str = ...,
    maxResults: int = ...,
    assetModelVersion: str = ...,
) -> ListAssetModelsResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-brackets: AssetModelTypeType](./literals.md#assetmodeltypetype) 
2. See [:material-code-braces: ListAssetModelsResponseTypeDef](./type_defs.md#listassetmodelsresponsetypedef) 


```python
# list_asset_models method usage example with argument unpacking

kwargs: ListAssetModelsRequestTypeDef = {  # (1)
    "assetModelTypes": ...,
}

parent.list_asset_models(**kwargs)
```

1. See [:material-code-braces: ListAssetModelsRequestTypeDef](./type_defs.md#listassetmodelsrequesttypedef) 

### list\_asset\_properties

Retrieves a paginated list of properties associated with an asset.

Type annotations and code completion for `#!python session.create_client("iotsitewise").list_asset_properties` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotsitewise/client/list_asset_properties.html)

```python
# list_asset_properties method definition

await def list_asset_properties(
    self,
    *,
    assetId: str,
    nextToken: str = ...,
    maxResults: int = ...,
    filter: ListAssetPropertiesFilterType = ...,  # (1)
) -> ListAssetPropertiesResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-brackets: ListAssetPropertiesFilterType](./literals.md#listassetpropertiesfiltertype) 
2. See [:material-code-braces: ListAssetPropertiesResponseTypeDef](./type_defs.md#listassetpropertiesresponsetypedef) 


```python
# list_asset_properties method usage example with argument unpacking

kwargs: ListAssetPropertiesRequestTypeDef = {  # (1)
    "assetId": ...,
}

parent.list_asset_properties(**kwargs)
```

1. See [:material-code-braces: ListAssetPropertiesRequestTypeDef](./type_defs.md#listassetpropertiesrequesttypedef) 

### list\_asset\_relationships

Retrieves a paginated list of asset relationships for an asset.

Type annotations and code completion for `#!python session.create_client("iotsitewise").list_asset_relationships` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotsitewise/client/list_asset_relationships.html)

```python
# list_asset_relationships method definition

await def list_asset_relationships(
    self,
    *,
    assetId: str,
    traversalType: TraversalTypeType,  # (1)
    nextToken: str = ...,
    maxResults: int = ...,
) -> ListAssetRelationshipsResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-brackets: TraversalTypeType](./literals.md#traversaltypetype) 
2. See [:material-code-braces: ListAssetRelationshipsResponseTypeDef](./type_defs.md#listassetrelationshipsresponsetypedef) 


```python
# list_asset_relationships method usage example with argument unpacking

kwargs: ListAssetRelationshipsRequestTypeDef = {  # (1)
    "assetId": ...,
    "traversalType": ...,
}

parent.list_asset_relationships(**kwargs)
```

1. See [:material-code-braces: ListAssetRelationshipsRequestTypeDef](./type_defs.md#listassetrelationshipsrequesttypedef) 

### list\_assets

Retrieves a paginated list of asset summaries.

Type annotations and code completion for `#!python session.create_client("iotsitewise").list_assets` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotsitewise/client/list_assets.html)

```python
# list_assets method definition

await def list_assets(
    self,
    *,
    nextToken: str = ...,
    maxResults: int = ...,
    assetModelId: str = ...,
    filter: ListAssetsFilterType = ...,  # (1)
) -> ListAssetsResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-brackets: ListAssetsFilterType](./literals.md#listassetsfiltertype) 
2. See [:material-code-braces: ListAssetsResponseTypeDef](./type_defs.md#listassetsresponsetypedef) 


```python
# list_assets method usage example with argument unpacking

kwargs: ListAssetsRequestTypeDef = {  # (1)
    "nextToken": ...,
}

parent.list_assets(**kwargs)
```

1. See [:material-code-braces: ListAssetsRequestTypeDef](./type_defs.md#listassetsrequesttypedef) 

### list\_associated\_assets

Retrieves a paginated list of associated assets.

Type annotations and code completion for `#!python session.create_client("iotsitewise").list_associated_assets` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotsitewise/client/list_associated_assets.html)

```python
# list_associated_assets method definition

await def list_associated_assets(
    self,
    *,
    assetId: str,
    hierarchyId: str = ...,
    traversalDirection: TraversalDirectionType = ...,  # (1)
    nextToken: str = ...,
    maxResults: int = ...,
) -> ListAssociatedAssetsResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-brackets: TraversalDirectionType](./literals.md#traversaldirectiontype) 
2. See [:material-code-braces: ListAssociatedAssetsResponseTypeDef](./type_defs.md#listassociatedassetsresponsetypedef) 


```python
# list_associated_assets method usage example with argument unpacking

kwargs: ListAssociatedAssetsRequestTypeDef = {  # (1)
    "assetId": ...,
}

parent.list_associated_assets(**kwargs)
```

1. See [:material-code-braces: ListAssociatedAssetsRequestTypeDef](./type_defs.md#listassociatedassetsrequesttypedef) 

### list\_bulk\_import\_jobs

Retrieves a paginated list of bulk import job requests.

Type annotations and code completion for `#!python session.create_client("iotsitewise").list_bulk_import_jobs` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotsitewise/client/list_bulk_import_jobs.html)

```python
# list_bulk_import_jobs method definition

await def list_bulk_import_jobs(
    self,
    *,
    nextToken: str = ...,
    maxResults: int = ...,
    filter: ListBulkImportJobsFilterType = ...,  # (1)
) -> ListBulkImportJobsResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-brackets: ListBulkImportJobsFilterType](./literals.md#listbulkimportjobsfiltertype) 
2. See [:material-code-braces: ListBulkImportJobsResponseTypeDef](./type_defs.md#listbulkimportjobsresponsetypedef) 


```python
# list_bulk_import_jobs method usage example with argument unpacking

kwargs: ListBulkImportJobsRequestTypeDef = {  # (1)
    "nextToken": ...,
}

parent.list_bulk_import_jobs(**kwargs)
```

1. See [:material-code-braces: ListBulkImportJobsRequestTypeDef](./type_defs.md#listbulkimportjobsrequesttypedef) 

### list\_composition\_relationships

Retrieves a paginated list of composition relationships for an asset model of
type <code>COMPONENT_MODEL</code>.

Type annotations and code completion for `#!python session.create_client("iotsitewise").list_composition_relationships` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotsitewise/client/list_composition_relationships.html)

```python
# list_composition_relationships method definition

await def list_composition_relationships(
    self,
    *,
    assetModelId: str,
    nextToken: str = ...,
    maxResults: int = ...,
) -> ListCompositionRelationshipsResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListCompositionRelationshipsResponseTypeDef](./type_defs.md#listcompositionrelationshipsresponsetypedef) 


```python
# list_composition_relationships method usage example with argument unpacking

kwargs: ListCompositionRelationshipsRequestTypeDef = {  # (1)
    "assetModelId": ...,
}

parent.list_composition_relationships(**kwargs)
```

1. See [:material-code-braces: ListCompositionRelationshipsRequestTypeDef](./type_defs.md#listcompositionrelationshipsrequesttypedef) 

### list\_dashboards

Retrieves a paginated list of dashboards for an IoT SiteWise Monitor project.

Type annotations and code completion for `#!python session.create_client("iotsitewise").list_dashboards` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotsitewise/client/list_dashboards.html)

```python
# list_dashboards method definition

await def list_dashboards(
    self,
    *,
    projectId: str,
    nextToken: str = ...,
    maxResults: int = ...,
) -> ListDashboardsResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListDashboardsResponseTypeDef](./type_defs.md#listdashboardsresponsetypedef) 


```python
# list_dashboards method usage example with argument unpacking

kwargs: ListDashboardsRequestTypeDef = {  # (1)
    "projectId": ...,
}

parent.list_dashboards(**kwargs)
```

1. See [:material-code-braces: ListDashboardsRequestTypeDef](./type_defs.md#listdashboardsrequesttypedef) 

### list\_datasets

Retrieves a paginated list of datasets for a specific target resource.

Type annotations and code completion for `#!python session.create_client("iotsitewise").list_datasets` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotsitewise/client/list_datasets.html)

```python
# list_datasets method definition

await def list_datasets(
    self,
    *,
    sourceType: DatasetSourceTypeType,  # (1)
    nextToken: str = ...,
    maxResults: int = ...,
) -> ListDatasetsResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-brackets: DatasetSourceTypeType](./literals.md#datasetsourcetypetype) 
2. See [:material-code-braces: ListDatasetsResponseTypeDef](./type_defs.md#listdatasetsresponsetypedef) 


```python
# list_datasets method usage example with argument unpacking

kwargs: ListDatasetsRequestTypeDef = {  # (1)
    "sourceType": ...,
}

parent.list_datasets(**kwargs)
```

1. See [:material-code-braces: ListDatasetsRequestTypeDef](./type_defs.md#listdatasetsrequesttypedef) 

### list\_gateways

Retrieves a paginated list of gateways.

Type annotations and code completion for `#!python session.create_client("iotsitewise").list_gateways` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotsitewise/client/list_gateways.html)

```python
# list_gateways method definition

await def list_gateways(
    self,
    *,
    nextToken: str = ...,
    maxResults: int = ...,
) -> ListGatewaysResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListGatewaysResponseTypeDef](./type_defs.md#listgatewaysresponsetypedef) 


```python
# list_gateways method usage example with argument unpacking

kwargs: ListGatewaysRequestTypeDef = {  # (1)
    "nextToken": ...,
}

parent.list_gateways(**kwargs)
```

1. See [:material-code-braces: ListGatewaysRequestTypeDef](./type_defs.md#listgatewaysrequesttypedef) 

### list\_portals

Retrieves a paginated list of IoT SiteWise Monitor portals.

Type annotations and code completion for `#!python session.create_client("iotsitewise").list_portals` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotsitewise/client/list_portals.html)

```python
# list_portals method definition

await def list_portals(
    self,
    *,
    nextToken: str = ...,
    maxResults: int = ...,
) -> ListPortalsResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListPortalsResponseTypeDef](./type_defs.md#listportalsresponsetypedef) 


```python
# list_portals method usage example with argument unpacking

kwargs: ListPortalsRequestTypeDef = {  # (1)
    "nextToken": ...,
}

parent.list_portals(**kwargs)
```

1. See [:material-code-braces: ListPortalsRequestTypeDef](./type_defs.md#listportalsrequesttypedef) 

### list\_project\_assets

Retrieves a paginated list of assets associated with an IoT SiteWise Monitor
project.

Type annotations and code completion for `#!python session.create_client("iotsitewise").list_project_assets` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotsitewise/client/list_project_assets.html)

```python
# list_project_assets method definition

await def list_project_assets(
    self,
    *,
    projectId: str,
    nextToken: str = ...,
    maxResults: int = ...,
) -> ListProjectAssetsResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListProjectAssetsResponseTypeDef](./type_defs.md#listprojectassetsresponsetypedef) 


```python
# list_project_assets method usage example with argument unpacking

kwargs: ListProjectAssetsRequestTypeDef = {  # (1)
    "projectId": ...,
}

parent.list_project_assets(**kwargs)
```

1. See [:material-code-braces: ListProjectAssetsRequestTypeDef](./type_defs.md#listprojectassetsrequesttypedef) 

### list\_projects

Retrieves a paginated list of projects for an IoT SiteWise Monitor portal.

Type annotations and code completion for `#!python session.create_client("iotsitewise").list_projects` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotsitewise/client/list_projects.html)

```python
# list_projects method definition

await def list_projects(
    self,
    *,
    portalId: str,
    nextToken: str = ...,
    maxResults: int = ...,
) -> ListProjectsResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListProjectsResponseTypeDef](./type_defs.md#listprojectsresponsetypedef) 


```python
# list_projects method usage example with argument unpacking

kwargs: ListProjectsRequestTypeDef = {  # (1)
    "portalId": ...,
}

parent.list_projects(**kwargs)
```

1. See [:material-code-braces: ListProjectsRequestTypeDef](./type_defs.md#listprojectsrequesttypedef) 

### list\_tags\_for\_resource

Retrieves the list of tags for an IoT SiteWise resource.

Type annotations and code completion for `#!python session.create_client("iotsitewise").list_tags_for_resource` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotsitewise/client/list_tags_for_resource.html)

```python
# list_tags_for_resource method definition

await def list_tags_for_resource(
    self,
    *,
    resourceArn: str,
) -> ListTagsForResourceResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListTagsForResourceResponseTypeDef](./type_defs.md#listtagsforresourceresponsetypedef) 


```python
# list_tags_for_resource method usage example with argument unpacking

kwargs: ListTagsForResourceRequestTypeDef = {  # (1)
    "resourceArn": ...,
}

parent.list_tags_for_resource(**kwargs)
```

1. See [:material-code-braces: ListTagsForResourceRequestTypeDef](./type_defs.md#listtagsforresourcerequesttypedef) 

### list\_time\_series

Retrieves a paginated list of time series (data streams).

Type annotations and code completion for `#!python session.create_client("iotsitewise").list_time_series` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotsitewise/client/list_time_series.html)

```python
# list_time_series method definition

await def list_time_series(
    self,
    *,
    nextToken: str = ...,
    maxResults: int = ...,
    assetId: str = ...,
    aliasPrefix: str = ...,
    timeSeriesType: ListTimeSeriesTypeType = ...,  # (1)
) -> ListTimeSeriesResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-brackets: ListTimeSeriesTypeType](./literals.md#listtimeseriestypetype) 
2. See [:material-code-braces: ListTimeSeriesResponseTypeDef](./type_defs.md#listtimeseriesresponsetypedef) 


```python
# list_time_series method usage example with argument unpacking

kwargs: ListTimeSeriesRequestTypeDef = {  # (1)
    "nextToken": ...,
}

parent.list_time_series(**kwargs)
```

1. See [:material-code-braces: ListTimeSeriesRequestTypeDef](./type_defs.md#listtimeseriesrequesttypedef) 

### put\_default\_encryption\_configuration

Sets the default encryption configuration for the Amazon Web Services account.

Type annotations and code completion for `#!python session.create_client("iotsitewise").put_default_encryption_configuration` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotsitewise/client/put_default_encryption_configuration.html)

```python
# put_default_encryption_configuration method definition

await def put_default_encryption_configuration(
    self,
    *,
    encryptionType: EncryptionTypeType,  # (1)
    kmsKeyId: str = ...,
) -> PutDefaultEncryptionConfigurationResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-brackets: EncryptionTypeType](./literals.md#encryptiontypetype) 
2. See [:material-code-braces: PutDefaultEncryptionConfigurationResponseTypeDef](./type_defs.md#putdefaultencryptionconfigurationresponsetypedef) 


```python
# put_default_encryption_configuration method usage example with argument unpacking

kwargs: PutDefaultEncryptionConfigurationRequestTypeDef = {  # (1)
    "encryptionType": ...,
}

parent.put_default_encryption_configuration(**kwargs)
```

1. See [:material-code-braces: PutDefaultEncryptionConfigurationRequestTypeDef](./type_defs.md#putdefaultencryptionconfigurationrequesttypedef) 

### put\_logging\_options

Sets logging options for IoT SiteWise.

Type annotations and code completion for `#!python session.create_client("iotsitewise").put_logging_options` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotsitewise/client/put_logging_options.html)

```python
# put_logging_options method definition

await def put_logging_options(
    self,
    *,
    loggingOptions: LoggingOptionsTypeDef,  # (1)
) -> Dict[str, Any]:
    ...
```

1. See [:material-code-braces: LoggingOptionsTypeDef](./type_defs.md#loggingoptionstypedef) 


```python
# put_logging_options method usage example with argument unpacking

kwargs: PutLoggingOptionsRequestTypeDef = {  # (1)
    "loggingOptions": ...,
}

parent.put_logging_options(**kwargs)
```

1. See [:material-code-braces: PutLoggingOptionsRequestTypeDef](./type_defs.md#putloggingoptionsrequesttypedef) 

### put\_storage\_configuration

Configures storage settings for IoT SiteWise.

Type annotations and code completion for `#!python session.create_client("iotsitewise").put_storage_configuration` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotsitewise/client/put_storage_configuration.html)

```python
# put_storage_configuration method definition

await def put_storage_configuration(
    self,
    *,
    storageType: StorageTypeType,  # (1)
    multiLayerStorage: MultiLayerStorageTypeDef = ...,  # (2)
    disassociatedDataStorage: DisassociatedDataStorageStateType = ...,  # (3)
    retentionPeriod: RetentionPeriodTypeDef = ...,  # (4)
    warmTier: WarmTierStateType = ...,  # (5)
    warmTierRetentionPeriod: WarmTierRetentionPeriodTypeDef = ...,  # (6)
    disallowIngestNullNaN: bool = ...,
) -> PutStorageConfigurationResponseTypeDef:  # (7)
    ...
```

1. See [:material-code-brackets: StorageTypeType](./literals.md#storagetypetype) 
2. See [:material-code-braces: MultiLayerStorageTypeDef](./type_defs.md#multilayerstoragetypedef) 
3. See [:material-code-brackets: DisassociatedDataStorageStateType](./literals.md#disassociateddatastoragestatetype) 
4. See [:material-code-braces: RetentionPeriodTypeDef](./type_defs.md#retentionperiodtypedef) 
5. See [:material-code-brackets: WarmTierStateType](./literals.md#warmtierstatetype) 
6. See [:material-code-braces: WarmTierRetentionPeriodTypeDef](./type_defs.md#warmtierretentionperiodtypedef) 
7. See [:material-code-braces: PutStorageConfigurationResponseTypeDef](./type_defs.md#putstorageconfigurationresponsetypedef) 


```python
# put_storage_configuration method usage example with argument unpacking

kwargs: PutStorageConfigurationRequestTypeDef = {  # (1)
    "storageType": ...,
}

parent.put_storage_configuration(**kwargs)
```

1. See [:material-code-braces: PutStorageConfigurationRequestTypeDef](./type_defs.md#putstorageconfigurationrequesttypedef) 

### tag\_resource

Adds tags to an IoT SiteWise resource.

Type annotations and code completion for `#!python session.create_client("iotsitewise").tag_resource` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotsitewise/client/tag_resource.html)

```python
# tag_resource method definition

await def tag_resource(
    self,
    *,
    resourceArn: str,
    tags: Mapping[str, str],
) -> Dict[str, Any]:
    ...
```



```python
# tag_resource method usage example with argument unpacking

kwargs: TagResourceRequestTypeDef = {  # (1)
    "resourceArn": ...,
    "tags": ...,
}

parent.tag_resource(**kwargs)
```

1. See [:material-code-braces: TagResourceRequestTypeDef](./type_defs.md#tagresourcerequesttypedef) 

### untag\_resource

Removes a tag from an IoT SiteWise resource.

Type annotations and code completion for `#!python session.create_client("iotsitewise").untag_resource` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotsitewise/client/untag_resource.html)

```python
# untag_resource method definition

await def untag_resource(
    self,
    *,
    resourceArn: str,
    tagKeys: Sequence[str],
) -> Dict[str, Any]:
    ...
```



```python
# untag_resource method usage example with argument unpacking

kwargs: UntagResourceRequestTypeDef = {  # (1)
    "resourceArn": ...,
    "tagKeys": ...,
}

parent.untag_resource(**kwargs)
```

1. See [:material-code-braces: UntagResourceRequestTypeDef](./type_defs.md#untagresourcerequesttypedef) 

### update\_access\_policy

Updates an existing access policy that specifies an identity's access to an IoT
SiteWise Monitor portal or project resource.

Type annotations and code completion for `#!python session.create_client("iotsitewise").update_access_policy` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotsitewise/client/update_access_policy.html)

```python
# update_access_policy method definition

await def update_access_policy(
    self,
    *,
    accessPolicyId: str,
    accessPolicyIdentity: IdentityTypeDef,  # (1)
    accessPolicyResource: ResourceTypeDef,  # (2)
    accessPolicyPermission: PermissionType,  # (3)
    clientToken: str = ...,
) -> Dict[str, Any]:
    ...
```

1. See [:material-code-braces: IdentityTypeDef](./type_defs.md#identitytypedef) 
2. See [:material-code-braces: ResourceTypeDef](./type_defs.md#resourcetypedef) 
3. See [:material-code-brackets: PermissionType](./literals.md#permissiontype) 


```python
# update_access_policy method usage example with argument unpacking

kwargs: UpdateAccessPolicyRequestTypeDef = {  # (1)
    "accessPolicyId": ...,
    "accessPolicyIdentity": ...,
    "accessPolicyResource": ...,
    "accessPolicyPermission": ...,
}

parent.update_access_policy(**kwargs)
```

1. See [:material-code-braces: UpdateAccessPolicyRequestTypeDef](./type_defs.md#updateaccesspolicyrequesttypedef) 

### update\_asset

Updates an asset's name.

Type annotations and code completion for `#!python session.create_client("iotsitewise").update_asset` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotsitewise/client/update_asset.html)

```python
# update_asset method definition

await def update_asset(
    self,
    *,
    assetId: str,
    assetName: str,
    clientToken: str = ...,
    assetDescription: str = ...,
    assetExternalId: str = ...,
) -> UpdateAssetResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: UpdateAssetResponseTypeDef](./type_defs.md#updateassetresponsetypedef) 


```python
# update_asset method usage example with argument unpacking

kwargs: UpdateAssetRequestTypeDef = {  # (1)
    "assetId": ...,
    "assetName": ...,
}

parent.update_asset(**kwargs)
```

1. See [:material-code-braces: UpdateAssetRequestTypeDef](./type_defs.md#updateassetrequesttypedef) 

### update\_asset\_model

Updates an asset model and all of the assets that were created from the model.

Type annotations and code completion for `#!python session.create_client("iotsitewise").update_asset_model` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotsitewise/client/update_asset_model.html)

```python
# update_asset_model method definition

await def update_asset_model(
    self,
    *,
    assetModelId: str,
    assetModelName: str,
    assetModelExternalId: str = ...,
    assetModelDescription: str = ...,
    assetModelProperties: Sequence[AssetModelPropertyUnionTypeDef] = ...,  # (1)
    assetModelHierarchies: Sequence[AssetModelHierarchyTypeDef] = ...,  # (2)
    assetModelCompositeModels: Sequence[AssetModelCompositeModelUnionTypeDef] = ...,  # (3)
    clientToken: str = ...,
    ifMatch: str = ...,
    ifNoneMatch: str = ...,
    matchForVersionType: AssetModelVersionTypeType = ...,  # (4)
) -> UpdateAssetModelResponseTypeDef:  # (5)
    ...
```

1. See [:material-code-braces: AssetModelPropertyTypeDef](./type_defs.md#assetmodelpropertytypedef) [:material-code-braces: AssetModelPropertyOutputTypeDef](./type_defs.md#assetmodelpropertyoutputtypedef) 
2. See [:material-code-braces: AssetModelHierarchyTypeDef](./type_defs.md#assetmodelhierarchytypedef) 
3. See [:material-code-braces: AssetModelCompositeModelTypeDef](./type_defs.md#assetmodelcompositemodeltypedef) [:material-code-braces: AssetModelCompositeModelOutputTypeDef](./type_defs.md#assetmodelcompositemodeloutputtypedef) 
4. See [:material-code-brackets: AssetModelVersionTypeType](./literals.md#assetmodelversiontypetype) 
5. See [:material-code-braces: UpdateAssetModelResponseTypeDef](./type_defs.md#updateassetmodelresponsetypedef) 


```python
# update_asset_model method usage example with argument unpacking

kwargs: UpdateAssetModelRequestTypeDef = {  # (1)
    "assetModelId": ...,
    "assetModelName": ...,
}

parent.update_asset_model(**kwargs)
```

1. See [:material-code-braces: UpdateAssetModelRequestTypeDef](./type_defs.md#updateassetmodelrequesttypedef) 

### update\_asset\_model\_composite\_model

Updates a composite model and all of the assets that were created from the
model.

Type annotations and code completion for `#!python session.create_client("iotsitewise").update_asset_model_composite_model` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotsitewise/client/update_asset_model_composite_model.html)

```python
# update_asset_model_composite_model method definition

await def update_asset_model_composite_model(
    self,
    *,
    assetModelId: str,
    assetModelCompositeModelId: str,
    assetModelCompositeModelName: str,
    assetModelCompositeModelExternalId: str = ...,
    assetModelCompositeModelDescription: str = ...,
    clientToken: str = ...,
    assetModelCompositeModelProperties: Sequence[AssetModelPropertyUnionTypeDef] = ...,  # (1)
    ifMatch: str = ...,
    ifNoneMatch: str = ...,
    matchForVersionType: AssetModelVersionTypeType = ...,  # (2)
) -> UpdateAssetModelCompositeModelResponseTypeDef:  # (3)
    ...
```

1. See [:material-code-braces: AssetModelPropertyTypeDef](./type_defs.md#assetmodelpropertytypedef) [:material-code-braces: AssetModelPropertyOutputTypeDef](./type_defs.md#assetmodelpropertyoutputtypedef) 
2. See [:material-code-brackets: AssetModelVersionTypeType](./literals.md#assetmodelversiontypetype) 
3. See [:material-code-braces: UpdateAssetModelCompositeModelResponseTypeDef](./type_defs.md#updateassetmodelcompositemodelresponsetypedef) 


```python
# update_asset_model_composite_model method usage example with argument unpacking

kwargs: UpdateAssetModelCompositeModelRequestTypeDef = {  # (1)
    "assetModelId": ...,
    "assetModelCompositeModelId": ...,
    "assetModelCompositeModelName": ...,
}

parent.update_asset_model_composite_model(**kwargs)
```

1. See [:material-code-braces: UpdateAssetModelCompositeModelRequestTypeDef](./type_defs.md#updateassetmodelcompositemodelrequesttypedef) 

### update\_asset\_property

Updates an asset property's alias and notification state.

Type annotations and code completion for `#!python session.create_client("iotsitewise").update_asset_property` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotsitewise/client/update_asset_property.html)

```python
# update_asset_property method definition

await def update_asset_property(
    self,
    *,
    assetId: str,
    propertyId: str,
    propertyAlias: str = ...,
    propertyNotificationState: PropertyNotificationStateType = ...,  # (1)
    clientToken: str = ...,
    propertyUnit: str = ...,
) -> EmptyResponseMetadataTypeDef:  # (2)
    ...
```

1. See [:material-code-brackets: PropertyNotificationStateType](./literals.md#propertynotificationstatetype) 
2. See [:material-code-braces: EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef) 


```python
# update_asset_property method usage example with argument unpacking

kwargs: UpdateAssetPropertyRequestTypeDef = {  # (1)
    "assetId": ...,
    "propertyId": ...,
}

parent.update_asset_property(**kwargs)
```

1. See [:material-code-braces: UpdateAssetPropertyRequestTypeDef](./type_defs.md#updateassetpropertyrequesttypedef) 

### update\_dashboard

Updates an IoT SiteWise Monitor dashboard.

Type annotations and code completion for `#!python session.create_client("iotsitewise").update_dashboard` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotsitewise/client/update_dashboard.html)

```python
# update_dashboard method definition

await def update_dashboard(
    self,
    *,
    dashboardId: str,
    dashboardName: str,
    dashboardDefinition: str,
    dashboardDescription: str = ...,
    clientToken: str = ...,
) -> Dict[str, Any]:
    ...
```



```python
# update_dashboard method usage example with argument unpacking

kwargs: UpdateDashboardRequestTypeDef = {  # (1)
    "dashboardId": ...,
    "dashboardName": ...,
    "dashboardDefinition": ...,
}

parent.update_dashboard(**kwargs)
```

1. See [:material-code-braces: UpdateDashboardRequestTypeDef](./type_defs.md#updatedashboardrequesttypedef) 

### update\_dataset

Updates a dataset.

Type annotations and code completion for `#!python session.create_client("iotsitewise").update_dataset` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotsitewise/client/update_dataset.html)

```python
# update_dataset method definition

await def update_dataset(
    self,
    *,
    datasetId: str,
    datasetName: str,
    datasetSource: DatasetSourceTypeDef,  # (1)
    datasetDescription: str = ...,
    clientToken: str = ...,
) -> UpdateDatasetResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: DatasetSourceTypeDef](./type_defs.md#datasetsourcetypedef) 
2. See [:material-code-braces: UpdateDatasetResponseTypeDef](./type_defs.md#updatedatasetresponsetypedef) 


```python
# update_dataset method usage example with argument unpacking

kwargs: UpdateDatasetRequestTypeDef = {  # (1)
    "datasetId": ...,
    "datasetName": ...,
    "datasetSource": ...,
}

parent.update_dataset(**kwargs)
```

1. See [:material-code-braces: UpdateDatasetRequestTypeDef](./type_defs.md#updatedatasetrequesttypedef) 

### update\_gateway

Updates a gateway's name.

Type annotations and code completion for `#!python session.create_client("iotsitewise").update_gateway` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotsitewise/client/update_gateway.html)

```python
# update_gateway method definition

await def update_gateway(
    self,
    *,
    gatewayId: str,
    gatewayName: str,
) -> EmptyResponseMetadataTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef) 


```python
# update_gateway method usage example with argument unpacking

kwargs: UpdateGatewayRequestTypeDef = {  # (1)
    "gatewayId": ...,
    "gatewayName": ...,
}

parent.update_gateway(**kwargs)
```

1. See [:material-code-braces: UpdateGatewayRequestTypeDef](./type_defs.md#updategatewayrequesttypedef) 

### update\_gateway\_capability\_configuration

Updates a gateway capability configuration or defines a new capability
configuration.

Type annotations and code completion for `#!python session.create_client("iotsitewise").update_gateway_capability_configuration` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotsitewise/client/update_gateway_capability_configuration.html)

```python
# update_gateway_capability_configuration method definition

await def update_gateway_capability_configuration(
    self,
    *,
    gatewayId: str,
    capabilityNamespace: str,
    capabilityConfiguration: str,
) -> UpdateGatewayCapabilityConfigurationResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: UpdateGatewayCapabilityConfigurationResponseTypeDef](./type_defs.md#updategatewaycapabilityconfigurationresponsetypedef) 


```python
# update_gateway_capability_configuration method usage example with argument unpacking

kwargs: UpdateGatewayCapabilityConfigurationRequestTypeDef = {  # (1)
    "gatewayId": ...,
    "capabilityNamespace": ...,
    "capabilityConfiguration": ...,
}

parent.update_gateway_capability_configuration(**kwargs)
```

1. See [:material-code-braces: UpdateGatewayCapabilityConfigurationRequestTypeDef](./type_defs.md#updategatewaycapabilityconfigurationrequesttypedef) 

### update\_portal

Updates an IoT SiteWise Monitor portal.

Type annotations and code completion for `#!python session.create_client("iotsitewise").update_portal` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotsitewise/client/update_portal.html)

```python
# update_portal method definition

await def update_portal(
    self,
    *,
    portalId: str,
    portalName: str,
    portalContactEmail: str,
    roleArn: str,
    portalDescription: str = ...,
    portalLogoImage: ImageTypeDef = ...,  # (1)
    clientToken: str = ...,
    notificationSenderEmail: str = ...,
    alarms: AlarmsTypeDef = ...,  # (2)
    portalType: PortalTypeType = ...,  # (3)
    portalTypeConfiguration: Mapping[str, PortalTypeEntryUnionTypeDef] = ...,  # (4)
) -> UpdatePortalResponseTypeDef:  # (5)
    ...
```

1. See [:material-code-braces: ImageTypeDef](./type_defs.md#imagetypedef) 
2. See [:material-code-braces: AlarmsTypeDef](./type_defs.md#alarmstypedef) 
3. See [:material-code-brackets: PortalTypeType](./literals.md#portaltypetype) 
4. See [:material-code-braces: PortalTypeEntryTypeDef](./type_defs.md#portaltypeentrytypedef) [:material-code-braces: PortalTypeEntryOutputTypeDef](./type_defs.md#portaltypeentryoutputtypedef) 
5. See [:material-code-braces: UpdatePortalResponseTypeDef](./type_defs.md#updateportalresponsetypedef) 


```python
# update_portal method usage example with argument unpacking

kwargs: UpdatePortalRequestTypeDef = {  # (1)
    "portalId": ...,
    "portalName": ...,
    "portalContactEmail": ...,
    "roleArn": ...,
}

parent.update_portal(**kwargs)
```

1. See [:material-code-braces: UpdatePortalRequestTypeDef](./type_defs.md#updateportalrequesttypedef) 

### update\_project

Updates an IoT SiteWise Monitor project.

Type annotations and code completion for `#!python session.create_client("iotsitewise").update_project` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotsitewise/client/update_project.html)

```python
# update_project method definition

await def update_project(
    self,
    *,
    projectId: str,
    projectName: str,
    projectDescription: str = ...,
    clientToken: str = ...,
) -> Dict[str, Any]:
    ...
```



```python
# update_project method usage example with argument unpacking

kwargs: UpdateProjectRequestTypeDef = {  # (1)
    "projectId": ...,
    "projectName": ...,
}

parent.update_project(**kwargs)
```

1. See [:material-code-braces: UpdateProjectRequestTypeDef](./type_defs.md#updateprojectrequesttypedef) 

### \_\_aenter\_\_



Type annotations and code completion for `#!python session.create_client("iotsitewise").__aenter__` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotsitewise.html#IoTSiteWise.Client)

```python
# __aenter__ method definition

await def __aenter__(
    self,
) -> Self:
    ...
```


### \_\_aexit\_\_



Type annotations and code completion for `#!python session.create_client("iotsitewise").__aexit__` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotsitewise.html#IoTSiteWise.Client)

```python
# __aexit__ method definition

await def __aexit__(
    self,
    exc_type: Union[Type[BaseException], None],
    exc_val: Union[BaseException, None],
    exc_tb: Union[TracebackType, None],
) -> None:
    ...
```




### get_paginator

Type annotations and code completion for `#!python session.create_client("iotsitewise").get_paginator` method with overloads.

- `client.get_paginator("execute_query")` -> [ExecuteQueryPaginator](./paginators.md#executequerypaginator)
- `client.get_paginator("get_asset_property_aggregates")` -> [GetAssetPropertyAggregatesPaginator](./paginators.md#getassetpropertyaggregatespaginator)
- `client.get_paginator("get_asset_property_value_history")` -> [GetAssetPropertyValueHistoryPaginator](./paginators.md#getassetpropertyvaluehistorypaginator)
- `client.get_paginator("get_interpolated_asset_property_values")` -> [GetInterpolatedAssetPropertyValuesPaginator](./paginators.md#getinterpolatedassetpropertyvaluespaginator)
- `client.get_paginator("list_access_policies")` -> [ListAccessPoliciesPaginator](./paginators.md#listaccesspoliciespaginator)
- `client.get_paginator("list_actions")` -> [ListActionsPaginator](./paginators.md#listactionspaginator)
- `client.get_paginator("list_asset_model_composite_models")` -> [ListAssetModelCompositeModelsPaginator](./paginators.md#listassetmodelcompositemodelspaginator)
- `client.get_paginator("list_asset_model_properties")` -> [ListAssetModelPropertiesPaginator](./paginators.md#listassetmodelpropertiespaginator)
- `client.get_paginator("list_asset_models")` -> [ListAssetModelsPaginator](./paginators.md#listassetmodelspaginator)
- `client.get_paginator("list_asset_properties")` -> [ListAssetPropertiesPaginator](./paginators.md#listassetpropertiespaginator)
- `client.get_paginator("list_asset_relationships")` -> [ListAssetRelationshipsPaginator](./paginators.md#listassetrelationshipspaginator)
- `client.get_paginator("list_assets")` -> [ListAssetsPaginator](./paginators.md#listassetspaginator)
- `client.get_paginator("list_associated_assets")` -> [ListAssociatedAssetsPaginator](./paginators.md#listassociatedassetspaginator)
- `client.get_paginator("list_bulk_import_jobs")` -> [ListBulkImportJobsPaginator](./paginators.md#listbulkimportjobspaginator)
- `client.get_paginator("list_composition_relationships")` -> [ListCompositionRelationshipsPaginator](./paginators.md#listcompositionrelationshipspaginator)
- `client.get_paginator("list_dashboards")` -> [ListDashboardsPaginator](./paginators.md#listdashboardspaginator)
- `client.get_paginator("list_datasets")` -> [ListDatasetsPaginator](./paginators.md#listdatasetspaginator)
- `client.get_paginator("list_gateways")` -> [ListGatewaysPaginator](./paginators.md#listgatewayspaginator)
- `client.get_paginator("list_portals")` -> [ListPortalsPaginator](./paginators.md#listportalspaginator)
- `client.get_paginator("list_project_assets")` -> [ListProjectAssetsPaginator](./paginators.md#listprojectassetspaginator)
- `client.get_paginator("list_projects")` -> [ListProjectsPaginator](./paginators.md#listprojectspaginator)
- `client.get_paginator("list_time_series")` -> [ListTimeSeriesPaginator](./paginators.md#listtimeseriespaginator)




### get_waiter

Type annotations and code completion for `#!python session.create_client("iotsitewise").get_waiter` method with overloads.

- `client.get_waiter("asset_active")` -> [AssetActiveWaiter](./waiters.md#assetactivewaiter)
- `client.get_waiter("asset_model_active")` -> [AssetModelActiveWaiter](./waiters.md#assetmodelactivewaiter)
- `client.get_waiter("asset_model_not_exists")` -> [AssetModelNotExistsWaiter](./waiters.md#assetmodelnotexistswaiter)
- `client.get_waiter("asset_not_exists")` -> [AssetNotExistsWaiter](./waiters.md#assetnotexistswaiter)
- `client.get_waiter("portal_active")` -> [PortalActiveWaiter](./waiters.md#portalactivewaiter)
- `client.get_waiter("portal_not_exists")` -> [PortalNotExistsWaiter](./waiters.md#portalnotexistswaiter)

