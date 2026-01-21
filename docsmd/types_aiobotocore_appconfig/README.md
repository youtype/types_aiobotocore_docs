# AppConfig module

> [Index](../README.md) > AppConfig


!!! note ""

    Auto-generated documentation for [AppConfig](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appconfig.html#appconfig)
    type annotations stubs module [types-aiobotocore-appconfig](https://pypi.org/project/types-aiobotocore-appconfig/).

## How to install

### Generate locally (recommended)

You can generate type annotations for `aiobotocore` package locally with `mypy-boto3-builder`.
Use [uv](https://docs.astral.sh/uv/getting-started/installation/) for build isolation.

1. Run mypy-boto3-builder in your package root directory: `uvx --with 'aiobotocore==3.1.1' mypy-boto3-builder`
1. Select `aiobotocore` AWS SDK.
1. Add `AppConfig` service.
1. Use provided commands to install generated packages.



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




## Waiters

Type annotations and code completion for
[waiters](./waiters.md)
from `#!python session.create_client("appconfig").get_waiter("...")`.

```python
# DeploymentCompleteWaiter usage example

from types_aiobotocore_appconfig.waiter import DeploymentCompleteWaiter

def get_deployment_complete_waiter() -> DeploymentCompleteWaiter:
    return Session().client("appconfig").get_waiter("deployment_complete")
```

- [DeploymentCompleteWaiter](./waiters.md#deploymentcompletewaiter)
- [EnvironmentReadyForDeploymentWaiter](./waiters.md#environmentreadyfordeploymentwaiter)






## Literals

Type annotations for [literals](./literals.md) used in methods and schema.

```python
# ActionPointType usage example

from types_aiobotocore_appconfig.literals import ActionPointType

def get_value() -> ActionPointType:
    return "AT_DEPLOYMENT_TICK"
```

- [ActionPointType](./literals.md#actionpointtype)
- [DeletionProtectionCheckType](./literals.md#deletionprotectionchecktype)
- [DeploymentCompleteWaiterName](./literals.md#deploymentcompletewaitername)
- [DeploymentEventTypeType](./literals.md#deploymenteventtypetype)
- [DeploymentStateType](./literals.md#deploymentstatetype)
- [EnvironmentReadyForDeploymentWaiterName](./literals.md#environmentreadyfordeploymentwaitername)
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
- [WaiterName](./literals.md#waitername)
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
- [CreateApplicationRequestTypeDef](./type_defs.md#createapplicationrequesttypedef)
- [CreateDeploymentStrategyRequestTypeDef](./type_defs.md#createdeploymentstrategyrequesttypedef)
- [MonitorTypeDef](./type_defs.md#monitortypedef)
- [CreateExtensionAssociationRequestTypeDef](./type_defs.md#createextensionassociationrequesttypedef)
- [ParameterTypeDef](./type_defs.md#parametertypedef)
- [DeleteApplicationRequestTypeDef](./type_defs.md#deleteapplicationrequesttypedef)
- [DeleteConfigurationProfileRequestTypeDef](./type_defs.md#deleteconfigurationprofilerequesttypedef)
- [DeleteDeploymentStrategyRequestTypeDef](./type_defs.md#deletedeploymentstrategyrequesttypedef)
- [DeleteEnvironmentRequestTypeDef](./type_defs.md#deleteenvironmentrequesttypedef)
- [DeleteExtensionAssociationRequestTypeDef](./type_defs.md#deleteextensionassociationrequesttypedef)
- [DeleteExtensionRequestTypeDef](./type_defs.md#deleteextensionrequesttypedef)
- [DeleteHostedConfigurationVersionRequestTypeDef](./type_defs.md#deletehostedconfigurationversionrequesttypedef)
- [DeploymentStrategyTypeDef](./type_defs.md#deploymentstrategytypedef)
- [DeploymentSummaryTypeDef](./type_defs.md#deploymentsummarytypedef)
- [ExtensionAssociationSummaryTypeDef](./type_defs.md#extensionassociationsummarytypedef)
- [ExtensionSummaryTypeDef](./type_defs.md#extensionsummarytypedef)
- [GetApplicationRequestTypeDef](./type_defs.md#getapplicationrequesttypedef)
- [GetConfigurationProfileRequestTypeDef](./type_defs.md#getconfigurationprofilerequesttypedef)
- [GetConfigurationRequestTypeDef](./type_defs.md#getconfigurationrequesttypedef)
- [GetDeploymentRequestTypeDef](./type_defs.md#getdeploymentrequesttypedef)
- [WaiterConfigTypeDef](./type_defs.md#waiterconfigtypedef)
- [GetDeploymentStrategyRequestTypeDef](./type_defs.md#getdeploymentstrategyrequesttypedef)
- [GetEnvironmentRequestTypeDef](./type_defs.md#getenvironmentrequesttypedef)
- [GetExtensionAssociationRequestTypeDef](./type_defs.md#getextensionassociationrequesttypedef)
- [GetExtensionRequestTypeDef](./type_defs.md#getextensionrequesttypedef)
- [GetHostedConfigurationVersionRequestTypeDef](./type_defs.md#gethostedconfigurationversionrequesttypedef)
- [HostedConfigurationVersionSummaryTypeDef](./type_defs.md#hostedconfigurationversionsummarytypedef)
- [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
- [ListApplicationsRequestTypeDef](./type_defs.md#listapplicationsrequesttypedef)
- [ListConfigurationProfilesRequestTypeDef](./type_defs.md#listconfigurationprofilesrequesttypedef)
- [ListDeploymentStrategiesRequestTypeDef](./type_defs.md#listdeploymentstrategiesrequesttypedef)
- [ListDeploymentsRequestTypeDef](./type_defs.md#listdeploymentsrequesttypedef)
- [ListEnvironmentsRequestTypeDef](./type_defs.md#listenvironmentsrequesttypedef)
- [ListExtensionAssociationsRequestTypeDef](./type_defs.md#listextensionassociationsrequesttypedef)
- [ListExtensionsRequestTypeDef](./type_defs.md#listextensionsrequesttypedef)
- [ListHostedConfigurationVersionsRequestTypeDef](./type_defs.md#listhostedconfigurationversionsrequesttypedef)
- [ListTagsForResourceRequestTypeDef](./type_defs.md#listtagsforresourcerequesttypedef)
- [StartDeploymentRequestTypeDef](./type_defs.md#startdeploymentrequesttypedef)
- [StopDeploymentRequestTypeDef](./type_defs.md#stopdeploymentrequesttypedef)
- [TagResourceRequestTypeDef](./type_defs.md#tagresourcerequesttypedef)
- [UntagResourceRequestTypeDef](./type_defs.md#untagresourcerequesttypedef)
- [UpdateApplicationRequestTypeDef](./type_defs.md#updateapplicationrequesttypedef)
- [UpdateDeploymentStrategyRequestTypeDef](./type_defs.md#updatedeploymentstrategyrequesttypedef)
- [UpdateExtensionAssociationRequestTypeDef](./type_defs.md#updateextensionassociationrequesttypedef)
- [ValidateConfigurationRequestTypeDef](./type_defs.md#validateconfigurationrequesttypedef)
- [UpdateAccountSettingsRequestTypeDef](./type_defs.md#updateaccountsettingsrequesttypedef)
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
- [CreateHostedConfigurationVersionRequestTypeDef](./type_defs.md#createhostedconfigurationversionrequesttypedef)
- [ConfigurationProfilesTypeDef](./type_defs.md#configurationprofilestypedef)
- [ConfigurationProfileTypeDef](./type_defs.md#configurationprofiletypedef)
- [CreateConfigurationProfileRequestTypeDef](./type_defs.md#createconfigurationprofilerequesttypedef)
- [UpdateConfigurationProfileRequestTypeDef](./type_defs.md#updateconfigurationprofilerequesttypedef)
- [CreateEnvironmentRequestTypeDef](./type_defs.md#createenvironmentrequesttypedef)
- [EnvironmentResponseTypeDef](./type_defs.md#environmentresponsetypedef)
- [EnvironmentTypeDef](./type_defs.md#environmenttypedef)
- [UpdateEnvironmentRequestTypeDef](./type_defs.md#updateenvironmentrequesttypedef)
- [CreateExtensionRequestTypeDef](./type_defs.md#createextensionrequesttypedef)
- [ExtensionTypeDef](./type_defs.md#extensiontypedef)
- [UpdateExtensionRequestTypeDef](./type_defs.md#updateextensionrequesttypedef)
- [DeploymentStrategiesTypeDef](./type_defs.md#deploymentstrategiestypedef)
- [DeploymentsTypeDef](./type_defs.md#deploymentstypedef)
- [ExtensionAssociationsTypeDef](./type_defs.md#extensionassociationstypedef)
- [ExtensionsTypeDef](./type_defs.md#extensionstypedef)
- [GetDeploymentRequestWaitTypeDef](./type_defs.md#getdeploymentrequestwaittypedef)
- [GetEnvironmentRequestWaitTypeDef](./type_defs.md#getenvironmentrequestwaittypedef)
- [HostedConfigurationVersionsTypeDef](./type_defs.md#hostedconfigurationversionstypedef)
- [ListApplicationsRequestPaginateTypeDef](./type_defs.md#listapplicationsrequestpaginatetypedef)
- [ListConfigurationProfilesRequestPaginateTypeDef](./type_defs.md#listconfigurationprofilesrequestpaginatetypedef)
- [ListDeploymentStrategiesRequestPaginateTypeDef](./type_defs.md#listdeploymentstrategiesrequestpaginatetypedef)
- [ListDeploymentsRequestPaginateTypeDef](./type_defs.md#listdeploymentsrequestpaginatetypedef)
- [ListEnvironmentsRequestPaginateTypeDef](./type_defs.md#listenvironmentsrequestpaginatetypedef)
- [ListExtensionAssociationsRequestPaginateTypeDef](./type_defs.md#listextensionassociationsrequestpaginatetypedef)
- [ListExtensionsRequestPaginateTypeDef](./type_defs.md#listextensionsrequestpaginatetypedef)
- [ListHostedConfigurationVersionsRequestPaginateTypeDef](./type_defs.md#listhostedconfigurationversionsrequestpaginatetypedef)
- [DeploymentTypeDef](./type_defs.md#deploymenttypedef)
- [EnvironmentsTypeDef](./type_defs.md#environmentstypedef)

