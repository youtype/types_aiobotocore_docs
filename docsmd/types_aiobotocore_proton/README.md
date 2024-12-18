# Proton module

> [Index](../README.md) > Proton


!!! note ""

    Auto-generated documentation for [Proton](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#proton)
    type annotations stubs module [types-aiobotocore-proton](https://pypi.org/project/types-aiobotocore-proton/).

## How to install

### Generate locally (recommended)

You can generate type annotations for `aiobotocore` package locally with `mypy_boto3_builder`.
Use [uv](https://docs.astral.sh/uv/getting-started/installation/) for build isolation.

1. Run mypy-boto3-builder in your package root directory: `uvx --with 'aiobotocore==2.16.0' mypy_boto3_builder`
1. Select `aiobotocore` AWS SDK.
1. Add `Proton` service.
1. Use provided commands to install generated packages.



### From PyPI with pip

Install `types-aiobotocore` for `Proton` service.

```bash
# install with aiobotocore type annotations
python -m pip install 'types-aiobotocore[proton]'

# Lite version does not provide session.client/resource overloads
# it is more RAM-friendly, but requires explicit type annotations
python -m pip install 'types-aiobotocore-lite[proton]'

# standalone installation
python -m pip install types-aiobotocore-proton
```



## How to uninstall

```bash
python -m pip uninstall -y types-aiobotocore-proton
```

## Usage

Code samples can be found in [Examples](./usage.md).

## ProtonClient

Type annotations and code completion for  `#!python session.create_client("proton")` as [ProtonClient](./client.md)
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Client)

```python
# ProtonClient usage example

from aiobotocore.session import get_session

from types_aiobotocore_proton.client import ProtonClient


session = get_session()
async with session.create_client("proton") as client:
    client: ProtonClient
```


## Paginators

Type annotations and code completion for
[paginators](./paginators.md)
from `#!python session.create_client("proton").get_paginator("...")`.

```python
# ListComponentOutputsPaginator usage example

from types_aiobotocore_proton.paginator import ListComponentOutputsPaginator

def get_list_component_outputs_paginator() -> ListComponentOutputsPaginator:
    return client.get_paginator("list_component_outputs"))
```

- [ListComponentOutputsPaginator](./paginators.md#listcomponentoutputspaginator)
- [ListComponentProvisionedResourcesPaginator](./paginators.md#listcomponentprovisionedresourcespaginator)
- [ListComponentsPaginator](./paginators.md#listcomponentspaginator)
- [ListDeploymentsPaginator](./paginators.md#listdeploymentspaginator)
- [ListEnvironmentAccountConnectionsPaginator](./paginators.md#listenvironmentaccountconnectionspaginator)
- [ListEnvironmentOutputsPaginator](./paginators.md#listenvironmentoutputspaginator)
- [ListEnvironmentProvisionedResourcesPaginator](./paginators.md#listenvironmentprovisionedresourcespaginator)
- [ListEnvironmentTemplateVersionsPaginator](./paginators.md#listenvironmenttemplateversionspaginator)
- [ListEnvironmentTemplatesPaginator](./paginators.md#listenvironmenttemplatespaginator)
- [ListEnvironmentsPaginator](./paginators.md#listenvironmentspaginator)
- [ListRepositoriesPaginator](./paginators.md#listrepositoriespaginator)
- [ListRepositorySyncDefinitionsPaginator](./paginators.md#listrepositorysyncdefinitionspaginator)
- [ListServiceInstanceOutputsPaginator](./paginators.md#listserviceinstanceoutputspaginator)
- [ListServiceInstanceProvisionedResourcesPaginator](./paginators.md#listserviceinstanceprovisionedresourcespaginator)
- [ListServiceInstancesPaginator](./paginators.md#listserviceinstancespaginator)
- [ListServicePipelineOutputsPaginator](./paginators.md#listservicepipelineoutputspaginator)
- [ListServicePipelineProvisionedResourcesPaginator](./paginators.md#listservicepipelineprovisionedresourcespaginator)
- [ListServiceTemplateVersionsPaginator](./paginators.md#listservicetemplateversionspaginator)
- [ListServiceTemplatesPaginator](./paginators.md#listservicetemplatespaginator)
- [ListServicesPaginator](./paginators.md#listservicespaginator)
- [ListTagsForResourcePaginator](./paginators.md#listtagsforresourcepaginator)




## Waiters

Type annotations and code completion for
[waiters](./waiters.md)
from `#!python session.create_client("proton").get_waiter("...")`.

```python
# ComponentDeletedWaiter usage example

from types_aiobotocore_proton.waiter import ComponentDeletedWaiter

def get_component_deleted_waiter() -> ComponentDeletedWaiter:
    return Session().client("proton").get_waiter("component_deleted")
```

- [ComponentDeletedWaiter](./waiters.md#componentdeletedwaiter)
- [ComponentDeployedWaiter](./waiters.md#componentdeployedwaiter)
- [EnvironmentDeployedWaiter](./waiters.md#environmentdeployedwaiter)
- [EnvironmentTemplateVersionRegisteredWaiter](./waiters.md#environmenttemplateversionregisteredwaiter)
- [ServiceCreatedWaiter](./waiters.md#servicecreatedwaiter)
- [ServiceDeletedWaiter](./waiters.md#servicedeletedwaiter)
- [ServiceInstanceDeployedWaiter](./waiters.md#serviceinstancedeployedwaiter)
- [ServicePipelineDeployedWaiter](./waiters.md#servicepipelinedeployedwaiter)
- [ServiceTemplateVersionRegisteredWaiter](./waiters.md#servicetemplateversionregisteredwaiter)
- [ServiceUpdatedWaiter](./waiters.md#serviceupdatedwaiter)






## Literals

Type annotations for [literals](./literals.md) used in methods and schema.

```python
# BlockerStatusType usage example

from types_aiobotocore_proton.literals import BlockerStatusType

def get_value() -> BlockerStatusType:
    return "ACTIVE"
```

- [BlockerStatusType](./literals.md#blockerstatustype)
- [BlockerTypeType](./literals.md#blockertypetype)
- [ComponentDeletedWaiterName](./literals.md#componentdeletedwaitername)
- [ComponentDeployedWaiterName](./literals.md#componentdeployedwaitername)
- [ComponentDeploymentUpdateTypeType](./literals.md#componentdeploymentupdatetypetype)
- [DeploymentStatusType](./literals.md#deploymentstatustype)
- [DeploymentTargetResourceTypeType](./literals.md#deploymenttargetresourcetypetype)
- [DeploymentUpdateTypeType](./literals.md#deploymentupdatetypetype)
- [EnvironmentAccountConnectionRequesterAccountTypeType](./literals.md#environmentaccountconnectionrequesteraccounttypetype)
- [EnvironmentAccountConnectionStatusType](./literals.md#environmentaccountconnectionstatustype)
- [EnvironmentDeployedWaiterName](./literals.md#environmentdeployedwaitername)
- [EnvironmentTemplateVersionRegisteredWaiterName](./literals.md#environmenttemplateversionregisteredwaitername)
- [ListComponentOutputsPaginatorName](./literals.md#listcomponentoutputspaginatorname)
- [ListComponentProvisionedResourcesPaginatorName](./literals.md#listcomponentprovisionedresourcespaginatorname)
- [ListComponentsPaginatorName](./literals.md#listcomponentspaginatorname)
- [ListDeploymentsPaginatorName](./literals.md#listdeploymentspaginatorname)
- [ListEnvironmentAccountConnectionsPaginatorName](./literals.md#listenvironmentaccountconnectionspaginatorname)
- [ListEnvironmentOutputsPaginatorName](./literals.md#listenvironmentoutputspaginatorname)
- [ListEnvironmentProvisionedResourcesPaginatorName](./literals.md#listenvironmentprovisionedresourcespaginatorname)
- [ListEnvironmentTemplateVersionsPaginatorName](./literals.md#listenvironmenttemplateversionspaginatorname)
- [ListEnvironmentTemplatesPaginatorName](./literals.md#listenvironmenttemplatespaginatorname)
- [ListEnvironmentsPaginatorName](./literals.md#listenvironmentspaginatorname)
- [ListRepositoriesPaginatorName](./literals.md#listrepositoriespaginatorname)
- [ListRepositorySyncDefinitionsPaginatorName](./literals.md#listrepositorysyncdefinitionspaginatorname)
- [ListServiceInstanceOutputsPaginatorName](./literals.md#listserviceinstanceoutputspaginatorname)
- [ListServiceInstanceProvisionedResourcesPaginatorName](./literals.md#listserviceinstanceprovisionedresourcespaginatorname)
- [ListServiceInstancesFilterByType](./literals.md#listserviceinstancesfilterbytype)
- [ListServiceInstancesPaginatorName](./literals.md#listserviceinstancespaginatorname)
- [ListServiceInstancesSortByType](./literals.md#listserviceinstancessortbytype)
- [ListServicePipelineOutputsPaginatorName](./literals.md#listservicepipelineoutputspaginatorname)
- [ListServicePipelineProvisionedResourcesPaginatorName](./literals.md#listservicepipelineprovisionedresourcespaginatorname)
- [ListServiceTemplateVersionsPaginatorName](./literals.md#listservicetemplateversionspaginatorname)
- [ListServiceTemplatesPaginatorName](./literals.md#listservicetemplatespaginatorname)
- [ListServicesPaginatorName](./literals.md#listservicespaginatorname)
- [ListTagsForResourcePaginatorName](./literals.md#listtagsforresourcepaginatorname)
- [ProvisionedResourceEngineType](./literals.md#provisionedresourceenginetype)
- [ProvisioningType](./literals.md#provisioningtype)
- [RepositoryProviderType](./literals.md#repositoryprovidertype)
- [RepositorySyncStatusType](./literals.md#repositorysyncstatustype)
- [ResourceDeploymentStatusType](./literals.md#resourcedeploymentstatustype)
- [ResourceSyncStatusType](./literals.md#resourcesyncstatustype)
- [ServiceCreatedWaiterName](./literals.md#servicecreatedwaitername)
- [ServiceDeletedWaiterName](./literals.md#servicedeletedwaitername)
- [ServiceInstanceDeployedWaiterName](./literals.md#serviceinstancedeployedwaitername)
- [ServicePipelineDeployedWaiterName](./literals.md#servicepipelinedeployedwaitername)
- [ServiceStatusType](./literals.md#servicestatustype)
- [ServiceTemplateSupportedComponentSourceTypeType](./literals.md#servicetemplatesupportedcomponentsourcetypetype)
- [ServiceTemplateVersionRegisteredWaiterName](./literals.md#servicetemplateversionregisteredwaitername)
- [ServiceUpdatedWaiterName](./literals.md#serviceupdatedwaitername)
- [SortOrderType](./literals.md#sortordertype)
- [SyncTypeType](./literals.md#synctypetype)
- [TemplateTypeType](./literals.md#templatetypetype)
- [TemplateVersionStatusType](./literals.md#templateversionstatustype)
- [ProtonServiceName](./literals.md#protonservicename)
- [ServiceName](./literals.md#servicename)
- [ResourceServiceName](./literals.md#resourceservicename)
- [PaginatorName](./literals.md#paginatorname)
- [WaiterName](./literals.md#waitername)
- [RegionName](./literals.md#regionname)




## Type definitions

Type annotations for [type definitions](./type_defs.md) used in methods and schema.

- [AcceptEnvironmentAccountConnectionInputRequestTypeDef](./type_defs.md#acceptenvironmentaccountconnectioninputrequesttypedef)
- [EnvironmentAccountConnectionTypeDef](./type_defs.md#environmentaccountconnectiontypedef)
- [ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef)
- [RepositoryBranchTypeDef](./type_defs.md#repositorybranchtypedef)
- [CancelComponentDeploymentInputRequestTypeDef](./type_defs.md#cancelcomponentdeploymentinputrequesttypedef)
- [ComponentTypeDef](./type_defs.md#componenttypedef)
- [CancelEnvironmentDeploymentInputRequestTypeDef](./type_defs.md#cancelenvironmentdeploymentinputrequesttypedef)
- [CancelServiceInstanceDeploymentInputRequestTypeDef](./type_defs.md#cancelserviceinstancedeploymentinputrequesttypedef)
- [ServiceInstanceTypeDef](./type_defs.md#serviceinstancetypedef)
- [CancelServicePipelineDeploymentInputRequestTypeDef](./type_defs.md#cancelservicepipelinedeploymentinputrequesttypedef)
- [ServicePipelineTypeDef](./type_defs.md#servicepipelinetypedef)
- [CompatibleEnvironmentTemplateInputTypeDef](./type_defs.md#compatibleenvironmenttemplateinputtypedef)
- [CompatibleEnvironmentTemplateTypeDef](./type_defs.md#compatibleenvironmenttemplatetypedef)
- [ComponentStateTypeDef](./type_defs.md#componentstatetypedef)
- [ComponentSummaryTypeDef](./type_defs.md#componentsummarytypedef)
- [ResourceCountsSummaryTypeDef](./type_defs.md#resourcecountssummarytypedef)
- [TagTypeDef](./type_defs.md#tagtypedef)
- [RepositoryBranchInputTypeDef](./type_defs.md#repositorybranchinputtypedef)
- [EnvironmentTemplateTypeDef](./type_defs.md#environmenttemplatetypedef)
- [EnvironmentTemplateVersionTypeDef](./type_defs.md#environmenttemplateversiontypedef)
- [RepositoryTypeDef](./type_defs.md#repositorytypedef)
- [CreateServiceSyncConfigInputRequestTypeDef](./type_defs.md#createservicesyncconfiginputrequesttypedef)
- [ServiceSyncConfigTypeDef](./type_defs.md#servicesyncconfigtypedef)
- [ServiceTemplateTypeDef](./type_defs.md#servicetemplatetypedef)
- [CreateTemplateSyncConfigInputRequestTypeDef](./type_defs.md#createtemplatesyncconfiginputrequesttypedef)
- [TemplateSyncConfigTypeDef](./type_defs.md#templatesyncconfigtypedef)
- [DeleteComponentInputRequestTypeDef](./type_defs.md#deletecomponentinputrequesttypedef)
- [DeleteDeploymentInputRequestTypeDef](./type_defs.md#deletedeploymentinputrequesttypedef)
- [DeleteEnvironmentAccountConnectionInputRequestTypeDef](./type_defs.md#deleteenvironmentaccountconnectioninputrequesttypedef)
- [DeleteEnvironmentInputRequestTypeDef](./type_defs.md#deleteenvironmentinputrequesttypedef)
- [DeleteEnvironmentTemplateInputRequestTypeDef](./type_defs.md#deleteenvironmenttemplateinputrequesttypedef)
- [DeleteEnvironmentTemplateVersionInputRequestTypeDef](./type_defs.md#deleteenvironmenttemplateversioninputrequesttypedef)
- [DeleteRepositoryInputRequestTypeDef](./type_defs.md#deleterepositoryinputrequesttypedef)
- [DeleteServiceInputRequestTypeDef](./type_defs.md#deleteserviceinputrequesttypedef)
- [DeleteServiceSyncConfigInputRequestTypeDef](./type_defs.md#deleteservicesyncconfiginputrequesttypedef)
- [DeleteServiceTemplateInputRequestTypeDef](./type_defs.md#deleteservicetemplateinputrequesttypedef)
- [DeleteServiceTemplateVersionInputRequestTypeDef](./type_defs.md#deleteservicetemplateversioninputrequesttypedef)
- [DeleteTemplateSyncConfigInputRequestTypeDef](./type_defs.md#deletetemplatesyncconfiginputrequesttypedef)
- [EnvironmentStateTypeDef](./type_defs.md#environmentstatetypedef)
- [ServiceInstanceStateTypeDef](./type_defs.md#serviceinstancestatetypedef)
- [ServicePipelineStateTypeDef](./type_defs.md#servicepipelinestatetypedef)
- [DeploymentSummaryTypeDef](./type_defs.md#deploymentsummarytypedef)
- [EnvironmentAccountConnectionSummaryTypeDef](./type_defs.md#environmentaccountconnectionsummarytypedef)
- [EnvironmentSummaryTypeDef](./type_defs.md#environmentsummarytypedef)
- [EnvironmentTemplateFilterTypeDef](./type_defs.md#environmenttemplatefiltertypedef)
- [EnvironmentTemplateSummaryTypeDef](./type_defs.md#environmenttemplatesummarytypedef)
- [EnvironmentTemplateVersionSummaryTypeDef](./type_defs.md#environmenttemplateversionsummarytypedef)
- [WaiterConfigTypeDef](./type_defs.md#waiterconfigtypedef)
- [GetComponentInputRequestTypeDef](./type_defs.md#getcomponentinputrequesttypedef)
- [GetDeploymentInputRequestTypeDef](./type_defs.md#getdeploymentinputrequesttypedef)
- [GetEnvironmentAccountConnectionInputRequestTypeDef](./type_defs.md#getenvironmentaccountconnectioninputrequesttypedef)
- [GetEnvironmentInputRequestTypeDef](./type_defs.md#getenvironmentinputrequesttypedef)
- [GetEnvironmentTemplateInputRequestTypeDef](./type_defs.md#getenvironmenttemplateinputrequesttypedef)
- [GetEnvironmentTemplateVersionInputRequestTypeDef](./type_defs.md#getenvironmenttemplateversioninputrequesttypedef)
- [GetRepositoryInputRequestTypeDef](./type_defs.md#getrepositoryinputrequesttypedef)
- [GetRepositorySyncStatusInputRequestTypeDef](./type_defs.md#getrepositorysyncstatusinputrequesttypedef)
- [GetServiceInputRequestTypeDef](./type_defs.md#getserviceinputrequesttypedef)
- [GetServiceInstanceInputRequestTypeDef](./type_defs.md#getserviceinstanceinputrequesttypedef)
- [GetServiceInstanceSyncStatusInputRequestTypeDef](./type_defs.md#getserviceinstancesyncstatusinputrequesttypedef)
- [RevisionTypeDef](./type_defs.md#revisiontypedef)
- [GetServiceSyncBlockerSummaryInputRequestTypeDef](./type_defs.md#getservicesyncblockersummaryinputrequesttypedef)
- [GetServiceSyncConfigInputRequestTypeDef](./type_defs.md#getservicesyncconfiginputrequesttypedef)
- [GetServiceTemplateInputRequestTypeDef](./type_defs.md#getservicetemplateinputrequesttypedef)
- [GetServiceTemplateVersionInputRequestTypeDef](./type_defs.md#getservicetemplateversioninputrequesttypedef)
- [GetTemplateSyncConfigInputRequestTypeDef](./type_defs.md#gettemplatesyncconfiginputrequesttypedef)
- [GetTemplateSyncStatusInputRequestTypeDef](./type_defs.md#gettemplatesyncstatusinputrequesttypedef)
- [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
- [ListComponentOutputsInputRequestTypeDef](./type_defs.md#listcomponentoutputsinputrequesttypedef)
- [OutputTypeDef](./type_defs.md#outputtypedef)
- [ListComponentProvisionedResourcesInputRequestTypeDef](./type_defs.md#listcomponentprovisionedresourcesinputrequesttypedef)
- [ProvisionedResourceTypeDef](./type_defs.md#provisionedresourcetypedef)
- [ListComponentsInputRequestTypeDef](./type_defs.md#listcomponentsinputrequesttypedef)
- [ListDeploymentsInputRequestTypeDef](./type_defs.md#listdeploymentsinputrequesttypedef)
- [ListEnvironmentAccountConnectionsInputRequestTypeDef](./type_defs.md#listenvironmentaccountconnectionsinputrequesttypedef)
- [ListEnvironmentOutputsInputRequestTypeDef](./type_defs.md#listenvironmentoutputsinputrequesttypedef)
- [ListEnvironmentProvisionedResourcesInputRequestTypeDef](./type_defs.md#listenvironmentprovisionedresourcesinputrequesttypedef)
- [ListEnvironmentTemplateVersionsInputRequestTypeDef](./type_defs.md#listenvironmenttemplateversionsinputrequesttypedef)
- [ListEnvironmentTemplatesInputRequestTypeDef](./type_defs.md#listenvironmenttemplatesinputrequesttypedef)
- [ListRepositoriesInputRequestTypeDef](./type_defs.md#listrepositoriesinputrequesttypedef)
- [RepositorySummaryTypeDef](./type_defs.md#repositorysummarytypedef)
- [ListRepositorySyncDefinitionsInputRequestTypeDef](./type_defs.md#listrepositorysyncdefinitionsinputrequesttypedef)
- [RepositorySyncDefinitionTypeDef](./type_defs.md#repositorysyncdefinitiontypedef)
- [ListServiceInstanceOutputsInputRequestTypeDef](./type_defs.md#listserviceinstanceoutputsinputrequesttypedef)
- [ListServiceInstanceProvisionedResourcesInputRequestTypeDef](./type_defs.md#listserviceinstanceprovisionedresourcesinputrequesttypedef)
- [ListServiceInstancesFilterTypeDef](./type_defs.md#listserviceinstancesfiltertypedef)
- [ServiceInstanceSummaryTypeDef](./type_defs.md#serviceinstancesummarytypedef)
- [ListServicePipelineOutputsInputRequestTypeDef](./type_defs.md#listservicepipelineoutputsinputrequesttypedef)
- [ListServicePipelineProvisionedResourcesInputRequestTypeDef](./type_defs.md#listservicepipelineprovisionedresourcesinputrequesttypedef)
- [ListServiceTemplateVersionsInputRequestTypeDef](./type_defs.md#listservicetemplateversionsinputrequesttypedef)
- [ServiceTemplateVersionSummaryTypeDef](./type_defs.md#servicetemplateversionsummarytypedef)
- [ListServiceTemplatesInputRequestTypeDef](./type_defs.md#listservicetemplatesinputrequesttypedef)
- [ServiceTemplateSummaryTypeDef](./type_defs.md#servicetemplatesummarytypedef)
- [ListServicesInputRequestTypeDef](./type_defs.md#listservicesinputrequesttypedef)
- [ServiceSummaryTypeDef](./type_defs.md#servicesummarytypedef)
- [ListTagsForResourceInputRequestTypeDef](./type_defs.md#listtagsforresourceinputrequesttypedef)
- [RejectEnvironmentAccountConnectionInputRequestTypeDef](./type_defs.md#rejectenvironmentaccountconnectioninputrequesttypedef)
- [RepositorySyncEventTypeDef](./type_defs.md#repositorysynceventtypedef)
- [ResourceSyncEventTypeDef](./type_defs.md#resourcesynceventtypedef)
- [S3ObjectSourceTypeDef](./type_defs.md#s3objectsourcetypedef)
- [SyncBlockerContextTypeDef](./type_defs.md#syncblockercontexttypedef)
- [UntagResourceInputRequestTypeDef](./type_defs.md#untagresourceinputrequesttypedef)
- [UpdateComponentInputRequestTypeDef](./type_defs.md#updatecomponentinputrequesttypedef)
- [UpdateEnvironmentAccountConnectionInputRequestTypeDef](./type_defs.md#updateenvironmentaccountconnectioninputrequesttypedef)
- [UpdateEnvironmentTemplateInputRequestTypeDef](./type_defs.md#updateenvironmenttemplateinputrequesttypedef)
- [UpdateEnvironmentTemplateVersionInputRequestTypeDef](./type_defs.md#updateenvironmenttemplateversioninputrequesttypedef)
- [UpdateServiceInputRequestTypeDef](./type_defs.md#updateserviceinputrequesttypedef)
- [UpdateServiceInstanceInputRequestTypeDef](./type_defs.md#updateserviceinstanceinputrequesttypedef)
- [UpdateServicePipelineInputRequestTypeDef](./type_defs.md#updateservicepipelineinputrequesttypedef)
- [UpdateServiceSyncBlockerInputRequestTypeDef](./type_defs.md#updateservicesyncblockerinputrequesttypedef)
- [UpdateServiceSyncConfigInputRequestTypeDef](./type_defs.md#updateservicesyncconfiginputrequesttypedef)
- [UpdateServiceTemplateInputRequestTypeDef](./type_defs.md#updateservicetemplateinputrequesttypedef)
- [UpdateTemplateSyncConfigInputRequestTypeDef](./type_defs.md#updatetemplatesyncconfiginputrequesttypedef)
- [AcceptEnvironmentAccountConnectionOutputTypeDef](./type_defs.md#acceptenvironmentaccountconnectionoutputtypedef)
- [CreateEnvironmentAccountConnectionOutputTypeDef](./type_defs.md#createenvironmentaccountconnectionoutputtypedef)
- [DeleteEnvironmentAccountConnectionOutputTypeDef](./type_defs.md#deleteenvironmentaccountconnectionoutputtypedef)
- [GetEnvironmentAccountConnectionOutputTypeDef](./type_defs.md#getenvironmentaccountconnectionoutputtypedef)
- [RejectEnvironmentAccountConnectionOutputTypeDef](./type_defs.md#rejectenvironmentaccountconnectionoutputtypedef)
- [UpdateEnvironmentAccountConnectionOutputTypeDef](./type_defs.md#updateenvironmentaccountconnectionoutputtypedef)
- [AccountSettingsTypeDef](./type_defs.md#accountsettingstypedef)
- [EnvironmentTypeDef](./type_defs.md#environmenttypedef)
- [CancelComponentDeploymentOutputTypeDef](./type_defs.md#cancelcomponentdeploymentoutputtypedef)
- [CreateComponentOutputTypeDef](./type_defs.md#createcomponentoutputtypedef)
- [DeleteComponentOutputTypeDef](./type_defs.md#deletecomponentoutputtypedef)
- [GetComponentOutputTypeDef](./type_defs.md#getcomponentoutputtypedef)
- [UpdateComponentOutputTypeDef](./type_defs.md#updatecomponentoutputtypedef)
- [CancelServiceInstanceDeploymentOutputTypeDef](./type_defs.md#cancelserviceinstancedeploymentoutputtypedef)
- [CreateServiceInstanceOutputTypeDef](./type_defs.md#createserviceinstanceoutputtypedef)
- [GetServiceInstanceOutputTypeDef](./type_defs.md#getserviceinstanceoutputtypedef)
- [UpdateServiceInstanceOutputTypeDef](./type_defs.md#updateserviceinstanceoutputtypedef)
- [CancelServicePipelineDeploymentOutputTypeDef](./type_defs.md#cancelservicepipelinedeploymentoutputtypedef)
- [ServiceTypeDef](./type_defs.md#servicetypedef)
- [UpdateServicePipelineOutputTypeDef](./type_defs.md#updateservicepipelineoutputtypedef)
- [UpdateServiceTemplateVersionInputRequestTypeDef](./type_defs.md#updateservicetemplateversioninputrequesttypedef)
- [ServiceTemplateVersionTypeDef](./type_defs.md#servicetemplateversiontypedef)
- [ListComponentsOutputTypeDef](./type_defs.md#listcomponentsoutputtypedef)
- [CountsSummaryTypeDef](./type_defs.md#countssummarytypedef)
- [CreateComponentInputRequestTypeDef](./type_defs.md#createcomponentinputrequesttypedef)
- [CreateEnvironmentAccountConnectionInputRequestTypeDef](./type_defs.md#createenvironmentaccountconnectioninputrequesttypedef)
- [CreateEnvironmentTemplateInputRequestTypeDef](./type_defs.md#createenvironmenttemplateinputrequesttypedef)
- [CreateRepositoryInputRequestTypeDef](./type_defs.md#createrepositoryinputrequesttypedef)
- [CreateServiceInputRequestTypeDef](./type_defs.md#createserviceinputrequesttypedef)
- [CreateServiceInstanceInputRequestTypeDef](./type_defs.md#createserviceinstanceinputrequesttypedef)
- [CreateServiceTemplateInputRequestTypeDef](./type_defs.md#createservicetemplateinputrequesttypedef)
- [ListTagsForResourceOutputTypeDef](./type_defs.md#listtagsforresourceoutputtypedef)
- [TagResourceInputRequestTypeDef](./type_defs.md#tagresourceinputrequesttypedef)
- [CreateEnvironmentInputRequestTypeDef](./type_defs.md#createenvironmentinputrequesttypedef)
- [UpdateAccountSettingsInputRequestTypeDef](./type_defs.md#updateaccountsettingsinputrequesttypedef)
- [UpdateEnvironmentInputRequestTypeDef](./type_defs.md#updateenvironmentinputrequesttypedef)
- [CreateEnvironmentTemplateOutputTypeDef](./type_defs.md#createenvironmenttemplateoutputtypedef)
- [DeleteEnvironmentTemplateOutputTypeDef](./type_defs.md#deleteenvironmenttemplateoutputtypedef)
- [GetEnvironmentTemplateOutputTypeDef](./type_defs.md#getenvironmenttemplateoutputtypedef)
- [UpdateEnvironmentTemplateOutputTypeDef](./type_defs.md#updateenvironmenttemplateoutputtypedef)
- [CreateEnvironmentTemplateVersionOutputTypeDef](./type_defs.md#createenvironmenttemplateversionoutputtypedef)
- [DeleteEnvironmentTemplateVersionOutputTypeDef](./type_defs.md#deleteenvironmenttemplateversionoutputtypedef)
- [GetEnvironmentTemplateVersionOutputTypeDef](./type_defs.md#getenvironmenttemplateversionoutputtypedef)
- [UpdateEnvironmentTemplateVersionOutputTypeDef](./type_defs.md#updateenvironmenttemplateversionoutputtypedef)
- [CreateRepositoryOutputTypeDef](./type_defs.md#createrepositoryoutputtypedef)
- [DeleteRepositoryOutputTypeDef](./type_defs.md#deleterepositoryoutputtypedef)
- [GetRepositoryOutputTypeDef](./type_defs.md#getrepositoryoutputtypedef)
- [CreateServiceSyncConfigOutputTypeDef](./type_defs.md#createservicesyncconfigoutputtypedef)
- [DeleteServiceSyncConfigOutputTypeDef](./type_defs.md#deleteservicesyncconfigoutputtypedef)
- [GetServiceSyncConfigOutputTypeDef](./type_defs.md#getservicesyncconfigoutputtypedef)
- [UpdateServiceSyncConfigOutputTypeDef](./type_defs.md#updateservicesyncconfigoutputtypedef)
- [CreateServiceTemplateOutputTypeDef](./type_defs.md#createservicetemplateoutputtypedef)
- [DeleteServiceTemplateOutputTypeDef](./type_defs.md#deleteservicetemplateoutputtypedef)
- [GetServiceTemplateOutputTypeDef](./type_defs.md#getservicetemplateoutputtypedef)
- [UpdateServiceTemplateOutputTypeDef](./type_defs.md#updateservicetemplateoutputtypedef)
- [CreateTemplateSyncConfigOutputTypeDef](./type_defs.md#createtemplatesyncconfigoutputtypedef)
- [DeleteTemplateSyncConfigOutputTypeDef](./type_defs.md#deletetemplatesyncconfigoutputtypedef)
- [GetTemplateSyncConfigOutputTypeDef](./type_defs.md#gettemplatesyncconfigoutputtypedef)
- [UpdateTemplateSyncConfigOutputTypeDef](./type_defs.md#updatetemplatesyncconfigoutputtypedef)
- [DeploymentStateTypeDef](./type_defs.md#deploymentstatetypedef)
- [ListDeploymentsOutputTypeDef](./type_defs.md#listdeploymentsoutputtypedef)
- [ListEnvironmentAccountConnectionsOutputTypeDef](./type_defs.md#listenvironmentaccountconnectionsoutputtypedef)
- [ListEnvironmentsOutputTypeDef](./type_defs.md#listenvironmentsoutputtypedef)
- [ListEnvironmentsInputRequestTypeDef](./type_defs.md#listenvironmentsinputrequesttypedef)
- [ListEnvironmentTemplatesOutputTypeDef](./type_defs.md#listenvironmenttemplatesoutputtypedef)
- [ListEnvironmentTemplateVersionsOutputTypeDef](./type_defs.md#listenvironmenttemplateversionsoutputtypedef)
- [GetComponentInputComponentDeletedWaitTypeDef](./type_defs.md#getcomponentinputcomponentdeletedwaittypedef)
- [GetComponentInputComponentDeployedWaitTypeDef](./type_defs.md#getcomponentinputcomponentdeployedwaittypedef)
- [GetEnvironmentInputEnvironmentDeployedWaitTypeDef](./type_defs.md#getenvironmentinputenvironmentdeployedwaittypedef)
- [GetEnvironmentTemplateVersionInputEnvironmentTemplateVersionRegisteredWaitTypeDef](./type_defs.md#getenvironmenttemplateversioninputenvironmenttemplateversionregisteredwaittypedef)
- [GetServiceInputServiceCreatedWaitTypeDef](./type_defs.md#getserviceinputservicecreatedwaittypedef)
- [GetServiceInputServiceDeletedWaitTypeDef](./type_defs.md#getserviceinputservicedeletedwaittypedef)
- [GetServiceInputServicePipelineDeployedWaitTypeDef](./type_defs.md#getserviceinputservicepipelinedeployedwaittypedef)
- [GetServiceInputServiceUpdatedWaitTypeDef](./type_defs.md#getserviceinputserviceupdatedwaittypedef)
- [GetServiceInstanceInputServiceInstanceDeployedWaitTypeDef](./type_defs.md#getserviceinstanceinputserviceinstancedeployedwaittypedef)
- [GetServiceTemplateVersionInputServiceTemplateVersionRegisteredWaitTypeDef](./type_defs.md#getservicetemplateversioninputservicetemplateversionregisteredwaittypedef)
- [ListComponentOutputsInputListComponentOutputsPaginateTypeDef](./type_defs.md#listcomponentoutputsinputlistcomponentoutputspaginatetypedef)
- [ListComponentProvisionedResourcesInputListComponentProvisionedResourcesPaginateTypeDef](./type_defs.md#listcomponentprovisionedresourcesinputlistcomponentprovisionedresourcespaginatetypedef)
- [ListComponentsInputListComponentsPaginateTypeDef](./type_defs.md#listcomponentsinputlistcomponentspaginatetypedef)
- [ListDeploymentsInputListDeploymentsPaginateTypeDef](./type_defs.md#listdeploymentsinputlistdeploymentspaginatetypedef)
- [ListEnvironmentAccountConnectionsInputListEnvironmentAccountConnectionsPaginateTypeDef](./type_defs.md#listenvironmentaccountconnectionsinputlistenvironmentaccountconnectionspaginatetypedef)
- [ListEnvironmentOutputsInputListEnvironmentOutputsPaginateTypeDef](./type_defs.md#listenvironmentoutputsinputlistenvironmentoutputspaginatetypedef)
- [ListEnvironmentProvisionedResourcesInputListEnvironmentProvisionedResourcesPaginateTypeDef](./type_defs.md#listenvironmentprovisionedresourcesinputlistenvironmentprovisionedresourcespaginatetypedef)
- [ListEnvironmentTemplateVersionsInputListEnvironmentTemplateVersionsPaginateTypeDef](./type_defs.md#listenvironmenttemplateversionsinputlistenvironmenttemplateversionspaginatetypedef)
- [ListEnvironmentTemplatesInputListEnvironmentTemplatesPaginateTypeDef](./type_defs.md#listenvironmenttemplatesinputlistenvironmenttemplatespaginatetypedef)
- [ListEnvironmentsInputListEnvironmentsPaginateTypeDef](./type_defs.md#listenvironmentsinputlistenvironmentspaginatetypedef)
- [ListRepositoriesInputListRepositoriesPaginateTypeDef](./type_defs.md#listrepositoriesinputlistrepositoriespaginatetypedef)
- [ListRepositorySyncDefinitionsInputListRepositorySyncDefinitionsPaginateTypeDef](./type_defs.md#listrepositorysyncdefinitionsinputlistrepositorysyncdefinitionspaginatetypedef)
- [ListServiceInstanceOutputsInputListServiceInstanceOutputsPaginateTypeDef](./type_defs.md#listserviceinstanceoutputsinputlistserviceinstanceoutputspaginatetypedef)
- [ListServiceInstanceProvisionedResourcesInputListServiceInstanceProvisionedResourcesPaginateTypeDef](./type_defs.md#listserviceinstanceprovisionedresourcesinputlistserviceinstanceprovisionedresourcespaginatetypedef)
- [ListServicePipelineOutputsInputListServicePipelineOutputsPaginateTypeDef](./type_defs.md#listservicepipelineoutputsinputlistservicepipelineoutputspaginatetypedef)
- [ListServicePipelineProvisionedResourcesInputListServicePipelineProvisionedResourcesPaginateTypeDef](./type_defs.md#listservicepipelineprovisionedresourcesinputlistservicepipelineprovisionedresourcespaginatetypedef)
- [ListServiceTemplateVersionsInputListServiceTemplateVersionsPaginateTypeDef](./type_defs.md#listservicetemplateversionsinputlistservicetemplateversionspaginatetypedef)
- [ListServiceTemplatesInputListServiceTemplatesPaginateTypeDef](./type_defs.md#listservicetemplatesinputlistservicetemplatespaginatetypedef)
- [ListServicesInputListServicesPaginateTypeDef](./type_defs.md#listservicesinputlistservicespaginatetypedef)
- [ListTagsForResourceInputListTagsForResourcePaginateTypeDef](./type_defs.md#listtagsforresourceinputlisttagsforresourcepaginatetypedef)
- [ListComponentOutputsOutputTypeDef](./type_defs.md#listcomponentoutputsoutputtypedef)
- [ListEnvironmentOutputsOutputTypeDef](./type_defs.md#listenvironmentoutputsoutputtypedef)
- [ListServiceInstanceOutputsOutputTypeDef](./type_defs.md#listserviceinstanceoutputsoutputtypedef)
- [ListServicePipelineOutputsOutputTypeDef](./type_defs.md#listservicepipelineoutputsoutputtypedef)
- [NotifyResourceDeploymentStatusChangeInputRequestTypeDef](./type_defs.md#notifyresourcedeploymentstatuschangeinputrequesttypedef)
- [ListComponentProvisionedResourcesOutputTypeDef](./type_defs.md#listcomponentprovisionedresourcesoutputtypedef)
- [ListEnvironmentProvisionedResourcesOutputTypeDef](./type_defs.md#listenvironmentprovisionedresourcesoutputtypedef)
- [ListServiceInstanceProvisionedResourcesOutputTypeDef](./type_defs.md#listserviceinstanceprovisionedresourcesoutputtypedef)
- [ListServicePipelineProvisionedResourcesOutputTypeDef](./type_defs.md#listservicepipelineprovisionedresourcesoutputtypedef)
- [ListRepositoriesOutputTypeDef](./type_defs.md#listrepositoriesoutputtypedef)
- [ListRepositorySyncDefinitionsOutputTypeDef](./type_defs.md#listrepositorysyncdefinitionsoutputtypedef)
- [ListServiceInstancesInputListServiceInstancesPaginateTypeDef](./type_defs.md#listserviceinstancesinputlistserviceinstancespaginatetypedef)
- [ListServiceInstancesInputRequestTypeDef](./type_defs.md#listserviceinstancesinputrequesttypedef)
- [ListServiceInstancesOutputTypeDef](./type_defs.md#listserviceinstancesoutputtypedef)
- [ListServiceTemplateVersionsOutputTypeDef](./type_defs.md#listservicetemplateversionsoutputtypedef)
- [ListServiceTemplatesOutputTypeDef](./type_defs.md#listservicetemplatesoutputtypedef)
- [ListServicesOutputTypeDef](./type_defs.md#listservicesoutputtypedef)
- [RepositorySyncAttemptTypeDef](./type_defs.md#repositorysyncattempttypedef)
- [ResourceSyncAttemptTypeDef](./type_defs.md#resourcesyncattempttypedef)
- [TemplateVersionSourceInputTypeDef](./type_defs.md#templateversionsourceinputtypedef)
- [SyncBlockerTypeDef](./type_defs.md#syncblockertypedef)
- [GetAccountSettingsOutputTypeDef](./type_defs.md#getaccountsettingsoutputtypedef)
- [UpdateAccountSettingsOutputTypeDef](./type_defs.md#updateaccountsettingsoutputtypedef)
- [CancelEnvironmentDeploymentOutputTypeDef](./type_defs.md#cancelenvironmentdeploymentoutputtypedef)
- [CreateEnvironmentOutputTypeDef](./type_defs.md#createenvironmentoutputtypedef)
- [DeleteEnvironmentOutputTypeDef](./type_defs.md#deleteenvironmentoutputtypedef)
- [GetEnvironmentOutputTypeDef](./type_defs.md#getenvironmentoutputtypedef)
- [UpdateEnvironmentOutputTypeDef](./type_defs.md#updateenvironmentoutputtypedef)
- [CreateServiceOutputTypeDef](./type_defs.md#createserviceoutputtypedef)
- [DeleteServiceOutputTypeDef](./type_defs.md#deleteserviceoutputtypedef)
- [GetServiceOutputTypeDef](./type_defs.md#getserviceoutputtypedef)
- [UpdateServiceOutputTypeDef](./type_defs.md#updateserviceoutputtypedef)
- [CreateServiceTemplateVersionOutputTypeDef](./type_defs.md#createservicetemplateversionoutputtypedef)
- [DeleteServiceTemplateVersionOutputTypeDef](./type_defs.md#deleteservicetemplateversionoutputtypedef)
- [GetServiceTemplateVersionOutputTypeDef](./type_defs.md#getservicetemplateversionoutputtypedef)
- [UpdateServiceTemplateVersionOutputTypeDef](./type_defs.md#updateservicetemplateversionoutputtypedef)
- [GetResourcesSummaryOutputTypeDef](./type_defs.md#getresourcessummaryoutputtypedef)
- [DeploymentTypeDef](./type_defs.md#deploymenttypedef)
- [GetRepositorySyncStatusOutputTypeDef](./type_defs.md#getrepositorysyncstatusoutputtypedef)
- [GetServiceInstanceSyncStatusOutputTypeDef](./type_defs.md#getserviceinstancesyncstatusoutputtypedef)
- [GetTemplateSyncStatusOutputTypeDef](./type_defs.md#gettemplatesyncstatusoutputtypedef)
- [CreateEnvironmentTemplateVersionInputRequestTypeDef](./type_defs.md#createenvironmenttemplateversioninputrequesttypedef)
- [CreateServiceTemplateVersionInputRequestTypeDef](./type_defs.md#createservicetemplateversioninputrequesttypedef)
- [ServiceSyncBlockerSummaryTypeDef](./type_defs.md#servicesyncblockersummarytypedef)
- [UpdateServiceSyncBlockerOutputTypeDef](./type_defs.md#updateservicesyncblockeroutputtypedef)
- [DeleteDeploymentOutputTypeDef](./type_defs.md#deletedeploymentoutputtypedef)
- [GetDeploymentOutputTypeDef](./type_defs.md#getdeploymentoutputtypedef)
- [GetServiceSyncBlockerSummaryOutputTypeDef](./type_defs.md#getservicesyncblockersummaryoutputtypedef)

