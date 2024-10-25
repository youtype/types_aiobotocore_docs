# AppConfig module

> [Index](../README.md) > AppConfig


!!! note ""

    Auto-generated documentation for [AppConfig](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appconfig.html#AppConfig)
    type annotations stubs module [types-aiobotocore-appconfig](https://pypi.org/project/types-aiobotocore-appconfig/).

## How to install



### From PyPI with pip

Install `types-aiobotocore` for `AppConfig` service.

```bash
# install with aiobotocore type annotations
python -m pip install 'types-aiobotocore[appconfig]'


# Lite version does not provide session.client/resource overloads
# it is more RAM-friendly, but requires explicit type annotations
python -m pip install 'types-aiobotocore-lite[appconfig]'


# standalone installation
python -m pip install types-aiobotocore-appconfig
```



## How to uninstall

```bash
python -m pip uninstall -y types-aiobotocore-appconfig
```

## Usage

Code samples can be found in [Examples](./usage.md).

## AppConfigClient

Type annotations and code completion for  `#!python session.create_client("appconfig")` as [AppConfigClient](./client.md)
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appconfig.html#AppConfig.Client)

```python
# AppConfigClient usage example

from aiobotocore.session import get_session

from types_aiobotocore_appconfig.client import AppConfigClient


session = get_session()
async with session.create_client("appconfig") as client:
    client: AppConfigClient
```


## Paginators

Type annotations and code completion for
[paginators](./paginators.md)
from `#!python session.create_client("appconfig").get_paginator("...")`.

```python
# ListApplicationsPaginator usage example

from types_aiobotocore_appconfig.paginator import ListApplicationsPaginator

def get_list_applications_paginator() -> ListApplicationsPaginator:
    return client.get_paginator("list_applications"))
```

- [ListApplicationsPaginator](./paginators.md#listapplicationspaginator)
- [ListConfigurationProfilesPaginator](./paginators.md#listconfigurationprofilespaginator)
- [ListDeploymentStrategiesPaginator](./paginators.md#listdeploymentstrategiespaginator)
- [ListDeploymentsPaginator](./paginators.md#listdeploymentspaginator)
- [ListEnvironmentsPaginator](./paginators.md#listenvironmentspaginator)
- [ListExtensionAssociationsPaginator](./paginators.md#listextensionassociationspaginator)
- [ListExtensionsPaginator](./paginators.md#listextensionspaginator)
- [ListHostedConfigurationVersionsPaginator](./paginators.md#listhostedconfigurationversionspaginator)








## Literals

Type annotations for [literals](./literals.md) used in methods and schema.

```python
# ActionPointType usage example

from types_aiobotocore_appconfig.literals import ActionPointType

def get_value() -> ActionPointType:
    return "ON_DEPLOYMENT_BAKING"
```

- [ActionPointType](./literals.md#actionpointtype)
- [DeletionProtectionCheckType](./literals.md#deletionprotectionchecktype)
- [DeploymentEventTypeType](./literals.md#deploymenteventtypetype)
- [DeploymentStateType](./literals.md#deploymentstatetype)
- [EnvironmentStateType](./literals.md#environmentstatetype)
- [GrowthTypeType](./literals.md#growthtypetype)
- [ListApplicationsPaginatorName](./literals.md#listapplicationspaginatorname)
- [ListConfigurationProfilesPaginatorName](./literals.md#listconfigurationprofilespaginatorname)
- [ListDeploymentStrategiesPaginatorName](./literals.md#listdeploymentstrategiespaginatorname)
- [ListDeploymentsPaginatorName](./literals.md#listdeploymentspaginatorname)
- [ListEnvironmentsPaginatorName](./literals.md#listenvironmentspaginatorname)
- [ListExtensionAssociationsPaginatorName](./literals.md#listextensionassociationspaginatorname)
- [ListExtensionsPaginatorName](./literals.md#listextensionspaginatorname)
- [ListHostedConfigurationVersionsPaginatorName](./literals.md#listhostedconfigurationversionspaginatorname)
- [ReplicateToType](./literals.md#replicatetotype)
- [TriggeredByType](./literals.md#triggeredbytype)
- [ValidatorTypeType](./literals.md#validatortypetype)
- [AppConfigServiceName](./literals.md#appconfigservicename)
- [ServiceName](./literals.md#servicename)
- [ResourceServiceName](./literals.md#resourceservicename)
- [PaginatorName](./literals.md#paginatorname)
- [RegionName](./literals.md#regionname)




## Type definitions

Type annotations for [type definitions](./type_defs.md) used in methods and schema.

- [DeletionProtectionSettingsTypeDef](./type_defs.md#deletionprotectionsettingstypedef)
- [ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef)
- [ActionInvocationTypeDef](./type_defs.md#actioninvocationtypedef)
- [ActionTypeDef](./type_defs.md#actiontypedef)
- [ApplicationTypeDef](./type_defs.md#applicationtypedef)
- [AppliedExtensionTypeDef](./type_defs.md#appliedextensiontypedef)
- [BlobTypeDef](./type_defs.md#blobtypedef)
- [ConfigurationProfileSummaryTypeDef](./type_defs.md#configurationprofilesummarytypedef)
- [ValidatorTypeDef](./type_defs.md#validatortypedef)
- [CreateApplicationRequestRequestTypeDef](./type_defs.md#createapplicationrequestrequesttypedef)
- [CreateDeploymentStrategyRequestRequestTypeDef](./type_defs.md#createdeploymentstrategyrequestrequesttypedef)
- [MonitorTypeDef](./type_defs.md#monitortypedef)
- [CreateExtensionAssociationRequestRequestTypeDef](./type_defs.md#createextensionassociationrequestrequesttypedef)
- [ParameterTypeDef](./type_defs.md#parametertypedef)
- [DeleteApplicationRequestRequestTypeDef](./type_defs.md#deleteapplicationrequestrequesttypedef)
- [DeleteConfigurationProfileRequestRequestTypeDef](./type_defs.md#deleteconfigurationprofilerequestrequesttypedef)
- [DeleteDeploymentStrategyRequestRequestTypeDef](./type_defs.md#deletedeploymentstrategyrequestrequesttypedef)
- [DeleteEnvironmentRequestRequestTypeDef](./type_defs.md#deleteenvironmentrequestrequesttypedef)
- [DeleteExtensionAssociationRequestRequestTypeDef](./type_defs.md#deleteextensionassociationrequestrequesttypedef)
- [DeleteExtensionRequestRequestTypeDef](./type_defs.md#deleteextensionrequestrequesttypedef)
- [DeleteHostedConfigurationVersionRequestRequestTypeDef](./type_defs.md#deletehostedconfigurationversionrequestrequesttypedef)
- [DeploymentStrategyTypeDef](./type_defs.md#deploymentstrategytypedef)
- [DeploymentSummaryTypeDef](./type_defs.md#deploymentsummarytypedef)
- [ExtensionAssociationSummaryTypeDef](./type_defs.md#extensionassociationsummarytypedef)
- [ExtensionSummaryTypeDef](./type_defs.md#extensionsummarytypedef)
- [GetApplicationRequestRequestTypeDef](./type_defs.md#getapplicationrequestrequesttypedef)
- [GetConfigurationProfileRequestRequestTypeDef](./type_defs.md#getconfigurationprofilerequestrequesttypedef)
- [GetConfigurationRequestRequestTypeDef](./type_defs.md#getconfigurationrequestrequesttypedef)
- [GetDeploymentRequestRequestTypeDef](./type_defs.md#getdeploymentrequestrequesttypedef)
- [GetDeploymentStrategyRequestRequestTypeDef](./type_defs.md#getdeploymentstrategyrequestrequesttypedef)
- [GetEnvironmentRequestRequestTypeDef](./type_defs.md#getenvironmentrequestrequesttypedef)
- [GetExtensionAssociationRequestRequestTypeDef](./type_defs.md#getextensionassociationrequestrequesttypedef)
- [GetExtensionRequestRequestTypeDef](./type_defs.md#getextensionrequestrequesttypedef)
- [GetHostedConfigurationVersionRequestRequestTypeDef](./type_defs.md#gethostedconfigurationversionrequestrequesttypedef)
- [HostedConfigurationVersionSummaryTypeDef](./type_defs.md#hostedconfigurationversionsummarytypedef)
- [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
- [ListApplicationsRequestRequestTypeDef](./type_defs.md#listapplicationsrequestrequesttypedef)
- [ListConfigurationProfilesRequestRequestTypeDef](./type_defs.md#listconfigurationprofilesrequestrequesttypedef)
- [ListDeploymentStrategiesRequestRequestTypeDef](./type_defs.md#listdeploymentstrategiesrequestrequesttypedef)
- [ListDeploymentsRequestRequestTypeDef](./type_defs.md#listdeploymentsrequestrequesttypedef)
- [ListEnvironmentsRequestRequestTypeDef](./type_defs.md#listenvironmentsrequestrequesttypedef)
- [ListExtensionAssociationsRequestRequestTypeDef](./type_defs.md#listextensionassociationsrequestrequesttypedef)
- [ListExtensionsRequestRequestTypeDef](./type_defs.md#listextensionsrequestrequesttypedef)
- [ListHostedConfigurationVersionsRequestRequestTypeDef](./type_defs.md#listhostedconfigurationversionsrequestrequesttypedef)
- [ListTagsForResourceRequestRequestTypeDef](./type_defs.md#listtagsforresourcerequestrequesttypedef)
- [StartDeploymentRequestRequestTypeDef](./type_defs.md#startdeploymentrequestrequesttypedef)
- [StopDeploymentRequestRequestTypeDef](./type_defs.md#stopdeploymentrequestrequesttypedef)
- [TagResourceRequestRequestTypeDef](./type_defs.md#tagresourcerequestrequesttypedef)
- [UntagResourceRequestRequestTypeDef](./type_defs.md#untagresourcerequestrequesttypedef)
- [UpdateApplicationRequestRequestTypeDef](./type_defs.md#updateapplicationrequestrequesttypedef)
- [UpdateDeploymentStrategyRequestRequestTypeDef](./type_defs.md#updatedeploymentstrategyrequestrequesttypedef)
- [UpdateExtensionAssociationRequestRequestTypeDef](./type_defs.md#updateextensionassociationrequestrequesttypedef)
- [ValidateConfigurationRequestRequestTypeDef](./type_defs.md#validateconfigurationrequestrequesttypedef)
- [UpdateAccountSettingsRequestRequestTypeDef](./type_defs.md#updateaccountsettingsrequestrequesttypedef)
- [AccountSettingsTypeDef](./type_defs.md#accountsettingstypedef)
- [ApplicationResponseTypeDef](./type_defs.md#applicationresponsetypedef)
- [ConfigurationTypeDef](./type_defs.md#configurationtypedef)
- [DeploymentStrategyResponseTypeDef](./type_defs.md#deploymentstrategyresponsetypedef)
- [EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef)
- [ExtensionAssociationTypeDef](./type_defs.md#extensionassociationtypedef)
- [HostedConfigurationVersionTypeDef](./type_defs.md#hostedconfigurationversiontypedef)
- [ResourceTagsTypeDef](./type_defs.md#resourcetagstypedef)
- [DeploymentEventTypeDef](./type_defs.md#deploymenteventtypedef)
- [ApplicationsTypeDef](./type_defs.md#applicationstypedef)
- [CreateHostedConfigurationVersionRequestRequestTypeDef](./type_defs.md#createhostedconfigurationversionrequestrequesttypedef)
- [ConfigurationProfilesTypeDef](./type_defs.md#configurationprofilestypedef)
- [ConfigurationProfileTypeDef](./type_defs.md#configurationprofiletypedef)
- [CreateConfigurationProfileRequestRequestTypeDef](./type_defs.md#createconfigurationprofilerequestrequesttypedef)
- [UpdateConfigurationProfileRequestRequestTypeDef](./type_defs.md#updateconfigurationprofilerequestrequesttypedef)
- [CreateEnvironmentRequestRequestTypeDef](./type_defs.md#createenvironmentrequestrequesttypedef)
- [EnvironmentResponseTypeDef](./type_defs.md#environmentresponsetypedef)
- [EnvironmentTypeDef](./type_defs.md#environmenttypedef)
- [UpdateEnvironmentRequestRequestTypeDef](./type_defs.md#updateenvironmentrequestrequesttypedef)
- [CreateExtensionRequestRequestTypeDef](./type_defs.md#createextensionrequestrequesttypedef)
- [ExtensionTypeDef](./type_defs.md#extensiontypedef)
- [UpdateExtensionRequestRequestTypeDef](./type_defs.md#updateextensionrequestrequesttypedef)
- [DeploymentStrategiesTypeDef](./type_defs.md#deploymentstrategiestypedef)
- [DeploymentsTypeDef](./type_defs.md#deploymentstypedef)
- [ExtensionAssociationsTypeDef](./type_defs.md#extensionassociationstypedef)
- [ExtensionsTypeDef](./type_defs.md#extensionstypedef)
- [HostedConfigurationVersionsTypeDef](./type_defs.md#hostedconfigurationversionstypedef)
- [ListApplicationsRequestListApplicationsPaginateTypeDef](./type_defs.md#listapplicationsrequestlistapplicationspaginatetypedef)
- [ListConfigurationProfilesRequestListConfigurationProfilesPaginateTypeDef](./type_defs.md#listconfigurationprofilesrequestlistconfigurationprofilespaginatetypedef)
- [ListDeploymentStrategiesRequestListDeploymentStrategiesPaginateTypeDef](./type_defs.md#listdeploymentstrategiesrequestlistdeploymentstrategiespaginatetypedef)
- [ListDeploymentsRequestListDeploymentsPaginateTypeDef](./type_defs.md#listdeploymentsrequestlistdeploymentspaginatetypedef)
- [ListEnvironmentsRequestListEnvironmentsPaginateTypeDef](./type_defs.md#listenvironmentsrequestlistenvironmentspaginatetypedef)
- [ListExtensionAssociationsRequestListExtensionAssociationsPaginateTypeDef](./type_defs.md#listextensionassociationsrequestlistextensionassociationspaginatetypedef)
- [ListExtensionsRequestListExtensionsPaginateTypeDef](./type_defs.md#listextensionsrequestlistextensionspaginatetypedef)
- [ListHostedConfigurationVersionsRequestListHostedConfigurationVersionsPaginateTypeDef](./type_defs.md#listhostedconfigurationversionsrequestlisthostedconfigurationversionspaginatetypedef)
- [DeploymentTypeDef](./type_defs.md#deploymenttypedef)
- [EnvironmentsTypeDef](./type_defs.md#environmentstypedef)

