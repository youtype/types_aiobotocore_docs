# IoTTwinMaker module

> [Index](../README.md) > IoTTwinMaker


!!! note ""

    Auto-generated documentation for [IoTTwinMaker](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iottwinmaker.html#iottwinmaker)
    type annotations stubs module [types-aiobotocore-iottwinmaker](https://pypi.org/project/types-aiobotocore-iottwinmaker/).

## How to install

### Generate locally (recommended)

You can generate type annotations for `aiobotocore` package locally with `mypy_boto3_builder`.
Use [uv](https://docs.astral.sh/uv/getting-started/installation/) for build isolation.

1. Run mypy-boto3-builder in your package root directory: `uvx --with 'aiobotocore==2.16.0' mypy_boto3_builder`
1. Select `aiobotocore` AWS SDK.
1. Add `IoTTwinMaker` service.
1. Use provided commands to install generated packages.



### From PyPI with pip

Install `types-aiobotocore` for `IoTTwinMaker` service.

```bash
# install with aiobotocore type annotations
python -m pip install 'types-aiobotocore[iottwinmaker]'

# Lite version does not provide session.client/resource overloads
# it is more RAM-friendly, but requires explicit type annotations
python -m pip install 'types-aiobotocore-lite[iottwinmaker]'

# standalone installation
python -m pip install types-aiobotocore-iottwinmaker
```



## How to uninstall

```bash
python -m pip uninstall -y types-aiobotocore-iottwinmaker
```

## Usage

Code samples can be found in [Examples](./usage.md).

## IoTTwinMakerClient

Type annotations and code completion for  `#!python session.create_client("iottwinmaker")` as [IoTTwinMakerClient](./client.md)
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iottwinmaker.html#IoTTwinMaker.Client)

```python
# IoTTwinMakerClient usage example

from aiobotocore.session import get_session

from types_aiobotocore_iottwinmaker.client import IoTTwinMakerClient


session = get_session()
async with session.create_client("iottwinmaker") as client:
    client: IoTTwinMakerClient
```








## Literals

Type annotations for [literals](./literals.md) used in methods and schema.

```python
# ColumnTypeType usage example

from types_aiobotocore_iottwinmaker.literals import ColumnTypeType

def get_value() -> ColumnTypeType:
    return "EDGE"
```

- [ColumnTypeType](./literals.md#columntypetype)
- [ComponentUpdateTypeType](./literals.md#componentupdatetypetype)
- [DestinationTypeType](./literals.md#destinationtypetype)
- [ErrorCodeType](./literals.md#errorcodetype)
- [GroupTypeType](./literals.md#grouptypetype)
- [InterpolationTypeType](./literals.md#interpolationtypetype)
- [MetadataTransferJobStateType](./literals.md#metadatatransferjobstatetype)
- [OrderByTimeType](./literals.md#orderbytimetype)
- [OrderType](./literals.md#ordertype)
- [ParentEntityUpdateTypeType](./literals.md#parententityupdatetypetype)
- [PricingModeType](./literals.md#pricingmodetype)
- [PricingTierType](./literals.md#pricingtiertype)
- [PropertyGroupUpdateTypeType](./literals.md#propertygroupupdatetypetype)
- [PropertyUpdateTypeType](./literals.md#propertyupdatetypetype)
- [SceneErrorCodeType](./literals.md#sceneerrorcodetype)
- [ScopeType](./literals.md#scopetype)
- [SourceTypeType](./literals.md#sourcetypetype)
- [StateType](./literals.md#statetype)
- [SyncJobStateType](./literals.md#syncjobstatetype)
- [SyncResourceStateType](./literals.md#syncresourcestatetype)
- [SyncResourceTypeType](./literals.md#syncresourcetypetype)
- [TypeType](./literals.md#typetype)
- [UpdateReasonType](./literals.md#updatereasontype)
- [IoTTwinMakerServiceName](./literals.md#iottwinmakerservicename)
- [ServiceName](./literals.md#servicename)
- [ResourceServiceName](./literals.md#resourceservicename)
- [RegionName](./literals.md#regionname)




## Type definitions

Type annotations for [type definitions](./type_defs.md) used in methods and schema.

- [ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef)
- [BundleInformationTypeDef](./type_defs.md#bundleinformationtypedef)
- [CancelMetadataTransferJobRequestRequestTypeDef](./type_defs.md#cancelmetadatatransferjobrequestrequesttypedef)
- [MetadataTransferJobProgressTypeDef](./type_defs.md#metadatatransferjobprogresstypedef)
- [ColumnDescriptionTypeDef](./type_defs.md#columndescriptiontypedef)
- [ComponentPropertyGroupRequestTypeDef](./type_defs.md#componentpropertygrouprequesttypedef)
- [ComponentPropertyGroupResponseTypeDef](./type_defs.md#componentpropertygroupresponsetypedef)
- [CompositeComponentTypeRequestTypeDef](./type_defs.md#compositecomponenttyperequesttypedef)
- [CompositeComponentTypeResponseTypeDef](./type_defs.md#compositecomponenttyperesponsetypedef)
- [PropertyGroupRequestTypeDef](./type_defs.md#propertygrouprequesttypedef)
- [CreateSceneRequestRequestTypeDef](./type_defs.md#createscenerequestrequesttypedef)
- [CreateSyncJobRequestRequestTypeDef](./type_defs.md#createsyncjobrequestrequesttypedef)
- [CreateWorkspaceRequestRequestTypeDef](./type_defs.md#createworkspacerequestrequesttypedef)
- [LambdaFunctionTypeDef](./type_defs.md#lambdafunctiontypedef)
- [RelationshipTypeDef](./type_defs.md#relationshiptypedef)
- [RelationshipValueTypeDef](./type_defs.md#relationshipvaluetypedef)
- [DeleteComponentTypeRequestRequestTypeDef](./type_defs.md#deletecomponenttyperequestrequesttypedef)
- [DeleteEntityRequestRequestTypeDef](./type_defs.md#deleteentityrequestrequesttypedef)
- [DeleteSceneRequestRequestTypeDef](./type_defs.md#deletescenerequestrequesttypedef)
- [DeleteSyncJobRequestRequestTypeDef](./type_defs.md#deletesyncjobrequestrequesttypedef)
- [DeleteWorkspaceRequestRequestTypeDef](./type_defs.md#deleteworkspacerequestrequesttypedef)
- [IotTwinMakerDestinationConfigurationTypeDef](./type_defs.md#iottwinmakerdestinationconfigurationtypedef)
- [S3DestinationConfigurationTypeDef](./type_defs.md#s3destinationconfigurationtypedef)
- [EntityPropertyReferenceOutputTypeDef](./type_defs.md#entitypropertyreferenceoutputtypedef)
- [EntityPropertyReferenceTypeDef](./type_defs.md#entitypropertyreferencetypedef)
- [ErrorDetailsTypeDef](./type_defs.md#errordetailstypedef)
- [ExecuteQueryRequestRequestTypeDef](./type_defs.md#executequeryrequestrequesttypedef)
- [RowTypeDef](./type_defs.md#rowtypedef)
- [FilterByAssetModelTypeDef](./type_defs.md#filterbyassetmodeltypedef)
- [FilterByAssetTypeDef](./type_defs.md#filterbyassettypedef)
- [FilterByComponentTypeTypeDef](./type_defs.md#filterbycomponenttypetypedef)
- [FilterByEntityTypeDef](./type_defs.md#filterbyentitytypedef)
- [GetComponentTypeRequestRequestTypeDef](./type_defs.md#getcomponenttyperequestrequesttypedef)
- [PropertyGroupResponseTypeDef](./type_defs.md#propertygroupresponsetypedef)
- [GetEntityRequestRequestTypeDef](./type_defs.md#getentityrequestrequesttypedef)
- [GetMetadataTransferJobRequestRequestTypeDef](./type_defs.md#getmetadatatransferjobrequestrequesttypedef)
- [InterpolationParametersTypeDef](./type_defs.md#interpolationparameterstypedef)
- [TimestampTypeDef](./type_defs.md#timestamptypedef)
- [GetSceneRequestRequestTypeDef](./type_defs.md#getscenerequestrequesttypedef)
- [SceneErrorTypeDef](./type_defs.md#sceneerrortypedef)
- [GetSyncJobRequestRequestTypeDef](./type_defs.md#getsyncjobrequestrequesttypedef)
- [GetWorkspaceRequestRequestTypeDef](./type_defs.md#getworkspacerequestrequesttypedef)
- [ListComponentTypesFilterTypeDef](./type_defs.md#listcomponenttypesfiltertypedef)
- [ListComponentsRequestRequestTypeDef](./type_defs.md#listcomponentsrequestrequesttypedef)
- [ListEntitiesFilterTypeDef](./type_defs.md#listentitiesfiltertypedef)
- [ListMetadataTransferJobsFilterTypeDef](./type_defs.md#listmetadatatransferjobsfiltertypedef)
- [ListPropertiesRequestRequestTypeDef](./type_defs.md#listpropertiesrequestrequesttypedef)
- [ListScenesRequestRequestTypeDef](./type_defs.md#listscenesrequestrequesttypedef)
- [SceneSummaryTypeDef](./type_defs.md#scenesummarytypedef)
- [ListSyncJobsRequestRequestTypeDef](./type_defs.md#listsyncjobsrequestrequesttypedef)
- [SyncResourceFilterTypeDef](./type_defs.md#syncresourcefiltertypedef)
- [ListTagsForResourceRequestRequestTypeDef](./type_defs.md#listtagsforresourcerequestrequesttypedef)
- [ListWorkspacesRequestRequestTypeDef](./type_defs.md#listworkspacesrequestrequesttypedef)
- [WorkspaceSummaryTypeDef](./type_defs.md#workspacesummarytypedef)
- [OrderByTypeDef](./type_defs.md#orderbytypedef)
- [ParentEntityUpdateRequestTypeDef](./type_defs.md#parententityupdaterequesttypedef)
- [S3SourceConfigurationTypeDef](./type_defs.md#s3sourceconfigurationtypedef)
- [TagResourceRequestRequestTypeDef](./type_defs.md#tagresourcerequestrequesttypedef)
- [UntagResourceRequestRequestTypeDef](./type_defs.md#untagresourcerequestrequesttypedef)
- [UpdatePricingPlanRequestRequestTypeDef](./type_defs.md#updatepricingplanrequestrequesttypedef)
- [UpdateSceneRequestRequestTypeDef](./type_defs.md#updatescenerequestrequesttypedef)
- [UpdateWorkspaceRequestRequestTypeDef](./type_defs.md#updateworkspacerequestrequesttypedef)
- [CreateComponentTypeResponseTypeDef](./type_defs.md#createcomponenttyperesponsetypedef)
- [CreateEntityResponseTypeDef](./type_defs.md#createentityresponsetypedef)
- [CreateSceneResponseTypeDef](./type_defs.md#createsceneresponsetypedef)
- [CreateSyncJobResponseTypeDef](./type_defs.md#createsyncjobresponsetypedef)
- [CreateWorkspaceResponseTypeDef](./type_defs.md#createworkspaceresponsetypedef)
- [DeleteComponentTypeResponseTypeDef](./type_defs.md#deletecomponenttyperesponsetypedef)
- [DeleteEntityResponseTypeDef](./type_defs.md#deleteentityresponsetypedef)
- [DeleteSyncJobResponseTypeDef](./type_defs.md#deletesyncjobresponsetypedef)
- [DeleteWorkspaceResponseTypeDef](./type_defs.md#deleteworkspaceresponsetypedef)
- [GetWorkspaceResponseTypeDef](./type_defs.md#getworkspaceresponsetypedef)
- [ListTagsForResourceResponseTypeDef](./type_defs.md#listtagsforresourceresponsetypedef)
- [UpdateComponentTypeResponseTypeDef](./type_defs.md#updatecomponenttyperesponsetypedef)
- [UpdateEntityResponseTypeDef](./type_defs.md#updateentityresponsetypedef)
- [UpdateSceneResponseTypeDef](./type_defs.md#updatesceneresponsetypedef)
- [UpdateWorkspaceResponseTypeDef](./type_defs.md#updateworkspaceresponsetypedef)
- [PricingPlanTypeDef](./type_defs.md#pricingplantypedef)
- [DataConnectorTypeDef](./type_defs.md#dataconnectortypedef)
- [DataValueOutputTypeDef](./type_defs.md#datavalueoutputtypedef)
- [DataValueTypeDef](./type_defs.md#datavaluetypedef)
- [DestinationConfigurationTypeDef](./type_defs.md#destinationconfigurationtypedef)
- [EntityPropertyReferenceUnionTypeDef](./type_defs.md#entitypropertyreferenceuniontypedef)
- [MetadataTransferJobStatusTypeDef](./type_defs.md#metadatatransferjobstatustypedef)
- [StatusTypeDef](./type_defs.md#statustypedef)
- [SyncJobStatusTypeDef](./type_defs.md#syncjobstatustypedef)
- [SyncResourceStatusTypeDef](./type_defs.md#syncresourcestatustypedef)
- [ExecuteQueryResponseTypeDef](./type_defs.md#executequeryresponsetypedef)
- [IotSiteWiseSourceConfigurationFilterTypeDef](./type_defs.md#iotsitewisesourceconfigurationfiltertypedef)
- [IotTwinMakerSourceConfigurationFilterTypeDef](./type_defs.md#iottwinmakersourceconfigurationfiltertypedef)
- [GetSceneResponseTypeDef](./type_defs.md#getsceneresponsetypedef)
- [ListComponentTypesRequestRequestTypeDef](./type_defs.md#listcomponenttypesrequestrequesttypedef)
- [ListEntitiesRequestRequestTypeDef](./type_defs.md#listentitiesrequestrequesttypedef)
- [ListMetadataTransferJobsRequestRequestTypeDef](./type_defs.md#listmetadatatransferjobsrequestrequesttypedef)
- [ListScenesResponseTypeDef](./type_defs.md#listscenesresponsetypedef)
- [ListSyncResourcesRequestRequestTypeDef](./type_defs.md#listsyncresourcesrequestrequesttypedef)
- [ListWorkspacesResponseTypeDef](./type_defs.md#listworkspacesresponsetypedef)
- [GetPricingPlanResponseTypeDef](./type_defs.md#getpricingplanresponsetypedef)
- [UpdatePricingPlanResponseTypeDef](./type_defs.md#updatepricingplanresponsetypedef)
- [FunctionRequestTypeDef](./type_defs.md#functionrequesttypedef)
- [FunctionResponseTypeDef](./type_defs.md#functionresponsetypedef)
- [DataTypeOutputTypeDef](./type_defs.md#datatypeoutputtypedef)
- [PropertyLatestValueTypeDef](./type_defs.md#propertylatestvaluetypedef)
- [PropertyValueOutputTypeDef](./type_defs.md#propertyvalueoutputtypedef)
- [DataValueUnionTypeDef](./type_defs.md#datavalueuniontypedef)
- [CancelMetadataTransferJobResponseTypeDef](./type_defs.md#cancelmetadatatransferjobresponsetypedef)
- [CreateMetadataTransferJobResponseTypeDef](./type_defs.md#createmetadatatransferjobresponsetypedef)
- [MetadataTransferJobSummaryTypeDef](./type_defs.md#metadatatransferjobsummarytypedef)
- [ComponentSummaryTypeDef](./type_defs.md#componentsummarytypedef)
- [ComponentTypeSummaryTypeDef](./type_defs.md#componenttypesummarytypedef)
- [EntitySummaryTypeDef](./type_defs.md#entitysummarytypedef)
- [GetSyncJobResponseTypeDef](./type_defs.md#getsyncjobresponsetypedef)
- [SyncJobSummaryTypeDef](./type_defs.md#syncjobsummarytypedef)
- [SyncResourceSummaryTypeDef](./type_defs.md#syncresourcesummarytypedef)
- [IotSiteWiseSourceConfigurationOutputTypeDef](./type_defs.md#iotsitewisesourceconfigurationoutputtypedef)
- [IotSiteWiseSourceConfigurationTypeDef](./type_defs.md#iotsitewisesourceconfigurationtypedef)
- [IotTwinMakerSourceConfigurationOutputTypeDef](./type_defs.md#iottwinmakersourceconfigurationoutputtypedef)
- [IotTwinMakerSourceConfigurationTypeDef](./type_defs.md#iottwinmakersourceconfigurationtypedef)
- [PropertyDefinitionResponseTypeDef](./type_defs.md#propertydefinitionresponsetypedef)
- [GetPropertyValueResponseTypeDef](./type_defs.md#getpropertyvalueresponsetypedef)
- [PropertyValueEntryOutputTypeDef](./type_defs.md#propertyvalueentryoutputtypedef)
- [PropertyValueHistoryTypeDef](./type_defs.md#propertyvaluehistorytypedef)
- [DataTypeTypeDef](./type_defs.md#datatypetypedef)
- [PropertyFilterTypeDef](./type_defs.md#propertyfiltertypedef)
- [PropertyValueTypeDef](./type_defs.md#propertyvaluetypedef)
- [ListMetadataTransferJobsResponseTypeDef](./type_defs.md#listmetadatatransferjobsresponsetypedef)
- [ListComponentsResponseTypeDef](./type_defs.md#listcomponentsresponsetypedef)
- [ListComponentTypesResponseTypeDef](./type_defs.md#listcomponenttypesresponsetypedef)
- [ListEntitiesResponseTypeDef](./type_defs.md#listentitiesresponsetypedef)
- [ListSyncJobsResponseTypeDef](./type_defs.md#listsyncjobsresponsetypedef)
- [ListSyncResourcesResponseTypeDef](./type_defs.md#listsyncresourcesresponsetypedef)
- [IotSiteWiseSourceConfigurationUnionTypeDef](./type_defs.md#iotsitewisesourceconfigurationuniontypedef)
- [SourceConfigurationOutputTypeDef](./type_defs.md#sourceconfigurationoutputtypedef)
- [IotTwinMakerSourceConfigurationUnionTypeDef](./type_defs.md#iottwinmakersourceconfigurationuniontypedef)
- [GetComponentTypeResponseTypeDef](./type_defs.md#getcomponenttyperesponsetypedef)
- [PropertyResponseTypeDef](./type_defs.md#propertyresponsetypedef)
- [PropertySummaryTypeDef](./type_defs.md#propertysummarytypedef)
- [BatchPutPropertyErrorTypeDef](./type_defs.md#batchputpropertyerrortypedef)
- [GetPropertyValueHistoryResponseTypeDef](./type_defs.md#getpropertyvaluehistoryresponsetypedef)
- [DataTypeUnionTypeDef](./type_defs.md#datatypeuniontypedef)
- [GetPropertyValueHistoryRequestRequestTypeDef](./type_defs.md#getpropertyvaluehistoryrequestrequesttypedef)
- [TabularConditionsTypeDef](./type_defs.md#tabularconditionstypedef)
- [PropertyValueUnionTypeDef](./type_defs.md#propertyvalueuniontypedef)
- [GetMetadataTransferJobResponseTypeDef](./type_defs.md#getmetadatatransferjobresponsetypedef)
- [SourceConfigurationTypeDef](./type_defs.md#sourceconfigurationtypedef)
- [ComponentResponseTypeDef](./type_defs.md#componentresponsetypedef)
- [ListPropertiesResponseTypeDef](./type_defs.md#listpropertiesresponsetypedef)
- [BatchPutPropertyErrorEntryTypeDef](./type_defs.md#batchputpropertyerrorentrytypedef)
- [PropertyDefinitionRequestTypeDef](./type_defs.md#propertydefinitionrequesttypedef)
- [GetPropertyValueRequestRequestTypeDef](./type_defs.md#getpropertyvaluerequestrequesttypedef)
- [PropertyValueEntryTypeDef](./type_defs.md#propertyvalueentrytypedef)
- [SourceConfigurationUnionTypeDef](./type_defs.md#sourceconfigurationuniontypedef)
- [GetEntityResponseTypeDef](./type_defs.md#getentityresponsetypedef)
- [BatchPutPropertyValuesResponseTypeDef](./type_defs.md#batchputpropertyvaluesresponsetypedef)
- [CreateComponentTypeRequestRequestTypeDef](./type_defs.md#createcomponenttyperequestrequesttypedef)
- [PropertyRequestTypeDef](./type_defs.md#propertyrequesttypedef)
- [UpdateComponentTypeRequestRequestTypeDef](./type_defs.md#updatecomponenttyperequestrequesttypedef)
- [PropertyValueEntryUnionTypeDef](./type_defs.md#propertyvalueentryuniontypedef)
- [CreateMetadataTransferJobRequestRequestTypeDef](./type_defs.md#createmetadatatransferjobrequestrequesttypedef)
- [ComponentRequestTypeDef](./type_defs.md#componentrequesttypedef)
- [ComponentUpdateRequestTypeDef](./type_defs.md#componentupdaterequesttypedef)
- [CompositeComponentRequestTypeDef](./type_defs.md#compositecomponentrequesttypedef)
- [CompositeComponentUpdateRequestTypeDef](./type_defs.md#compositecomponentupdaterequesttypedef)
- [BatchPutPropertyValuesRequestRequestTypeDef](./type_defs.md#batchputpropertyvaluesrequestrequesttypedef)
- [CreateEntityRequestRequestTypeDef](./type_defs.md#createentityrequestrequesttypedef)
- [UpdateEntityRequestRequestTypeDef](./type_defs.md#updateentityrequestrequesttypedef)

