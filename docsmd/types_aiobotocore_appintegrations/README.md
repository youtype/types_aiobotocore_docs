# AppIntegrationsService module

> [Index](../README.md) > AppIntegrationsService


!!! note ""

    Auto-generated documentation for [AppIntegrationsService](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appintegrations.html#appintegrationsservice)
    type annotations stubs module [types-aiobotocore-appintegrations](https://pypi.org/project/types-aiobotocore-appintegrations/).

## How to install

### Generate locally (recommended)

You can generate type annotations for `aiobotocore` package locally with `mypy-boto3-builder`.
Use [uv](https://docs.astral.sh/uv/getting-started/installation/) for build isolation.

1. Run mypy-boto3-builder in your package root directory: `uvx --with 'aiobotocore==3.1.1' mypy-boto3-builder`
1. Select `aiobotocore` AWS SDK.
1. Add `AppIntegrationsService` service.
1. Use provided commands to install generated packages.



### From PyPI with pip

Install `types-aiobotocore` for `AppIntegrationsService` service.

```bash
# install with aiobotocore type annotations
python -m pip install 'types-aiobotocore[appintegrations]'

# Lite version does not provide session.client/resource overloads
# it is more RAM-friendly, but requires explicit type annotations
python -m pip install 'types-aiobotocore-lite[appintegrations]'

# standalone installation
python -m pip install types-aiobotocore-appintegrations
```



## How to uninstall

```bash
python -m pip uninstall -y types-aiobotocore-appintegrations
```

## Usage

Code samples can be found in [Examples](./usage.md).

## AppIntegrationsServiceClient

Type annotations and code completion for  `#!python session.create_client("appintegrations")` as [AppIntegrationsServiceClient](./client.md)
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appintegrations.html#AppIntegrationsService.Client)

```python
# AppIntegrationsServiceClient usage example

from aiobotocore.session import get_session

from types_aiobotocore_appintegrations.client import AppIntegrationsServiceClient


session = get_session()
async with session.create_client("appintegrations") as client:
    client: AppIntegrationsServiceClient
```


## Paginators

Type annotations and code completion for
[paginators](./paginators.md)
from `#!python session.create_client("appintegrations").get_paginator("...")`.

```python
# ListApplicationAssociationsPaginator usage example

from types_aiobotocore_appintegrations.paginator import ListApplicationAssociationsPaginator

def get_list_application_associations_paginator() -> ListApplicationAssociationsPaginator:
    return client.get_paginator("list_application_associations"))
```

- [ListApplicationAssociationsPaginator](./paginators.md#listapplicationassociationspaginator)
- [ListApplicationsPaginator](./paginators.md#listapplicationspaginator)
- [ListDataIntegrationAssociationsPaginator](./paginators.md#listdataintegrationassociationspaginator)
- [ListDataIntegrationsPaginator](./paginators.md#listdataintegrationspaginator)
- [ListEventIntegrationAssociationsPaginator](./paginators.md#listeventintegrationassociationspaginator)
- [ListEventIntegrationsPaginator](./paginators.md#listeventintegrationspaginator)








## Literals

Type annotations for [literals](./literals.md) used in methods and schema.

```python
# ApplicationTypeType usage example

from types_aiobotocore_appintegrations.literals import ApplicationTypeType

def get_value() -> ApplicationTypeType:
    return "MCP_SERVER"
```

- [ApplicationTypeType](./literals.md#applicationtypetype)
- [ContactHandlingScopeType](./literals.md#contacthandlingscopetype)
- [ExecutionModeType](./literals.md#executionmodetype)
- [ExecutionStatusType](./literals.md#executionstatustype)
- [ListApplicationAssociationsPaginatorName](./literals.md#listapplicationassociationspaginatorname)
- [ListApplicationsPaginatorName](./literals.md#listapplicationspaginatorname)
- [ListDataIntegrationAssociationsPaginatorName](./literals.md#listdataintegrationassociationspaginatorname)
- [ListDataIntegrationsPaginatorName](./literals.md#listdataintegrationspaginatorname)
- [ListEventIntegrationAssociationsPaginatorName](./literals.md#listeventintegrationassociationspaginatorname)
- [ListEventIntegrationsPaginatorName](./literals.md#listeventintegrationspaginatorname)
- [AppIntegrationsServiceServiceName](./literals.md#appintegrationsserviceservicename)
- [ServiceName](./literals.md#servicename)
- [ResourceServiceName](./literals.md#resourceservicename)
- [PaginatorName](./literals.md#paginatorname)
- [RegionName](./literals.md#regionname)




## Type definitions

Type annotations for [type definitions](./type_defs.md) used in methods and schema.

- [ApplicationAssociationSummaryTypeDef](./type_defs.md#applicationassociationsummarytypedef)
- [ContactHandlingTypeDef](./type_defs.md#contacthandlingtypedef)
- [ExternalUrlConfigOutputTypeDef](./type_defs.md#externalurlconfigoutputtypedef)
- [ExternalUrlConfigTypeDef](./type_defs.md#externalurlconfigtypedef)
- [ApplicationSummaryTypeDef](./type_defs.md#applicationsummarytypedef)
- [PublicationTypeDef](./type_defs.md#publicationtypedef)
- [SubscriptionTypeDef](./type_defs.md#subscriptiontypedef)
- [ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef)
- [ScheduleConfigurationTypeDef](./type_defs.md#scheduleconfigurationtypedef)
- [FileConfigurationOutputTypeDef](./type_defs.md#fileconfigurationoutputtypedef)
- [EventFilterTypeDef](./type_defs.md#eventfiltertypedef)
- [LastExecutionStatusTypeDef](./type_defs.md#lastexecutionstatustypedef)
- [DataIntegrationSummaryTypeDef](./type_defs.md#dataintegrationsummarytypedef)
- [DeleteApplicationRequestTypeDef](./type_defs.md#deleteapplicationrequesttypedef)
- [DeleteDataIntegrationRequestTypeDef](./type_defs.md#deletedataintegrationrequesttypedef)
- [DeleteEventIntegrationRequestTypeDef](./type_defs.md#deleteeventintegrationrequesttypedef)
- [EventIntegrationAssociationTypeDef](./type_defs.md#eventintegrationassociationtypedef)
- [OnDemandConfigurationTypeDef](./type_defs.md#ondemandconfigurationtypedef)
- [FileConfigurationTypeDef](./type_defs.md#fileconfigurationtypedef)
- [GetApplicationRequestTypeDef](./type_defs.md#getapplicationrequesttypedef)
- [IframeConfigOutputTypeDef](./type_defs.md#iframeconfigoutputtypedef)
- [GetDataIntegrationRequestTypeDef](./type_defs.md#getdataintegrationrequesttypedef)
- [GetEventIntegrationRequestTypeDef](./type_defs.md#geteventintegrationrequesttypedef)
- [IframeConfigTypeDef](./type_defs.md#iframeconfigtypedef)
- [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
- [ListApplicationAssociationsRequestTypeDef](./type_defs.md#listapplicationassociationsrequesttypedef)
- [ListApplicationsRequestTypeDef](./type_defs.md#listapplicationsrequesttypedef)
- [ListDataIntegrationAssociationsRequestTypeDef](./type_defs.md#listdataintegrationassociationsrequesttypedef)
- [ListDataIntegrationsRequestTypeDef](./type_defs.md#listdataintegrationsrequesttypedef)
- [ListEventIntegrationAssociationsRequestTypeDef](./type_defs.md#listeventintegrationassociationsrequesttypedef)
- [ListEventIntegrationsRequestTypeDef](./type_defs.md#listeventintegrationsrequesttypedef)
- [ListTagsForResourceRequestTypeDef](./type_defs.md#listtagsforresourcerequesttypedef)
- [TagResourceRequestTypeDef](./type_defs.md#tagresourcerequesttypedef)
- [UntagResourceRequestTypeDef](./type_defs.md#untagresourcerequesttypedef)
- [UpdateDataIntegrationRequestTypeDef](./type_defs.md#updatedataintegrationrequesttypedef)
- [UpdateEventIntegrationRequestTypeDef](./type_defs.md#updateeventintegrationrequesttypedef)
- [ApplicationConfigTypeDef](./type_defs.md#applicationconfigtypedef)
- [ApplicationSourceConfigOutputTypeDef](./type_defs.md#applicationsourceconfigoutputtypedef)
- [ApplicationSourceConfigTypeDef](./type_defs.md#applicationsourceconfigtypedef)
- [CreateApplicationResponseTypeDef](./type_defs.md#createapplicationresponsetypedef)
- [CreateDataIntegrationAssociationResponseTypeDef](./type_defs.md#createdataintegrationassociationresponsetypedef)
- [CreateEventIntegrationResponseTypeDef](./type_defs.md#createeventintegrationresponsetypedef)
- [ListApplicationAssociationsResponseTypeDef](./type_defs.md#listapplicationassociationsresponsetypedef)
- [ListApplicationsResponseTypeDef](./type_defs.md#listapplicationsresponsetypedef)
- [ListTagsForResourceResponseTypeDef](./type_defs.md#listtagsforresourceresponsetypedef)
- [CreateDataIntegrationResponseTypeDef](./type_defs.md#createdataintegrationresponsetypedef)
- [GetDataIntegrationResponseTypeDef](./type_defs.md#getdataintegrationresponsetypedef)
- [CreateEventIntegrationRequestTypeDef](./type_defs.md#createeventintegrationrequesttypedef)
- [EventIntegrationTypeDef](./type_defs.md#eventintegrationtypedef)
- [GetEventIntegrationResponseTypeDef](./type_defs.md#geteventintegrationresponsetypedef)
- [ListDataIntegrationsResponseTypeDef](./type_defs.md#listdataintegrationsresponsetypedef)
- [ListEventIntegrationAssociationsResponseTypeDef](./type_defs.md#listeventintegrationassociationsresponsetypedef)
- [ExecutionConfigurationTypeDef](./type_defs.md#executionconfigurationtypedef)
- [FileConfigurationUnionTypeDef](./type_defs.md#fileconfigurationuniontypedef)
- [IframeConfigUnionTypeDef](./type_defs.md#iframeconfiguniontypedef)
- [ListApplicationAssociationsRequestPaginateTypeDef](./type_defs.md#listapplicationassociationsrequestpaginatetypedef)
- [ListApplicationsRequestPaginateTypeDef](./type_defs.md#listapplicationsrequestpaginatetypedef)
- [ListDataIntegrationAssociationsRequestPaginateTypeDef](./type_defs.md#listdataintegrationassociationsrequestpaginatetypedef)
- [ListDataIntegrationsRequestPaginateTypeDef](./type_defs.md#listdataintegrationsrequestpaginatetypedef)
- [ListEventIntegrationAssociationsRequestPaginateTypeDef](./type_defs.md#listeventintegrationassociationsrequestpaginatetypedef)
- [ListEventIntegrationsRequestPaginateTypeDef](./type_defs.md#listeventintegrationsrequestpaginatetypedef)
- [GetApplicationResponseTypeDef](./type_defs.md#getapplicationresponsetypedef)
- [ApplicationSourceConfigUnionTypeDef](./type_defs.md#applicationsourceconfiguniontypedef)
- [ListEventIntegrationsResponseTypeDef](./type_defs.md#listeventintegrationsresponsetypedef)
- [CreateDataIntegrationAssociationRequestTypeDef](./type_defs.md#createdataintegrationassociationrequesttypedef)
- [DataIntegrationAssociationSummaryTypeDef](./type_defs.md#dataintegrationassociationsummarytypedef)
- [UpdateDataIntegrationAssociationRequestTypeDef](./type_defs.md#updatedataintegrationassociationrequesttypedef)
- [CreateDataIntegrationRequestTypeDef](./type_defs.md#createdataintegrationrequesttypedef)
- [CreateApplicationRequestTypeDef](./type_defs.md#createapplicationrequesttypedef)
- [UpdateApplicationRequestTypeDef](./type_defs.md#updateapplicationrequesttypedef)
- [ListDataIntegrationAssociationsResponseTypeDef](./type_defs.md#listdataintegrationassociationsresponsetypedef)

