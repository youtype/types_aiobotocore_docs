# CodeCatalyst module

> [Index](../README.md) > CodeCatalyst


!!! note ""

    Auto-generated documentation for [CodeCatalyst](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codecatalyst.html#codecatalyst)
    type annotations stubs module [types-aiobotocore-codecatalyst](https://pypi.org/project/types-aiobotocore-codecatalyst/).

## How to install

### Generate locally (recommended)

You can generate type annotations for `aiobotocore` package locally with `mypy_boto3_builder`.
Use [uv](https://docs.astral.sh/uv/getting-started/installation/) for build isolation.

1. Run mypy-boto3-builder in your package root directory: `uvx --with 'aiobotocore==2.19.0' mypy_boto3_builder`
1. Select `aiobotocore` AWS SDK.
1. Add `CodeCatalyst` service.
1. Use provided commands to install generated packages.



### From PyPI with pip

Install `types-aiobotocore` for `CodeCatalyst` service.

```bash
# install with aiobotocore type annotations
python -m pip install 'types-aiobotocore[codecatalyst]'

# Lite version does not provide session.client/resource overloads
# it is more RAM-friendly, but requires explicit type annotations
python -m pip install 'types-aiobotocore-lite[codecatalyst]'

# standalone installation
python -m pip install types-aiobotocore-codecatalyst
```



## How to uninstall

```bash
python -m pip uninstall -y types-aiobotocore-codecatalyst
```

## Usage

Code samples can be found in [Examples](./usage.md).

## CodeCatalystClient

Type annotations and code completion for  `#!python session.create_client("codecatalyst")` as [CodeCatalystClient](./client.md)
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codecatalyst.html#CodeCatalyst.Client)

```python
# CodeCatalystClient usage example

from aiobotocore.session import get_session

from types_aiobotocore_codecatalyst.client import CodeCatalystClient


session = get_session()
async with session.create_client("codecatalyst") as client:
    client: CodeCatalystClient
```


## Paginators

Type annotations and code completion for
[paginators](./paginators.md)
from `#!python session.create_client("codecatalyst").get_paginator("...")`.

```python
# ListAccessTokensPaginator usage example

from types_aiobotocore_codecatalyst.paginator import ListAccessTokensPaginator

def get_list_access_tokens_paginator() -> ListAccessTokensPaginator:
    return client.get_paginator("list_access_tokens"))
```

- [ListAccessTokensPaginator](./paginators.md#listaccesstokenspaginator)
- [ListDevEnvironmentSessionsPaginator](./paginators.md#listdevenvironmentsessionspaginator)
- [ListDevEnvironmentsPaginator](./paginators.md#listdevenvironmentspaginator)
- [ListEventLogsPaginator](./paginators.md#listeventlogspaginator)
- [ListProjectsPaginator](./paginators.md#listprojectspaginator)
- [ListSourceRepositoriesPaginator](./paginators.md#listsourcerepositoriespaginator)
- [ListSourceRepositoryBranchesPaginator](./paginators.md#listsourcerepositorybranchespaginator)
- [ListSpacesPaginator](./paginators.md#listspacespaginator)
- [ListWorkflowRunsPaginator](./paginators.md#listworkflowrunspaginator)
- [ListWorkflowsPaginator](./paginators.md#listworkflowspaginator)








## Literals

Type annotations for [literals](./literals.md) used in methods and schema.

```python
# ComparisonOperatorType usage example

from types_aiobotocore_codecatalyst.literals import ComparisonOperatorType

def get_value() -> ComparisonOperatorType:
    return "BEGINS_WITH"
```

- [ComparisonOperatorType](./literals.md#comparisonoperatortype)
- [DevEnvironmentSessionTypeType](./literals.md#devenvironmentsessiontypetype)
- [DevEnvironmentStatusType](./literals.md#devenvironmentstatustype)
- [FilterKeyType](./literals.md#filterkeytype)
- [InstanceTypeType](./literals.md#instancetypetype)
- [ListAccessTokensPaginatorName](./literals.md#listaccesstokenspaginatorname)
- [ListDevEnvironmentSessionsPaginatorName](./literals.md#listdevenvironmentsessionspaginatorname)
- [ListDevEnvironmentsPaginatorName](./literals.md#listdevenvironmentspaginatorname)
- [ListEventLogsPaginatorName](./literals.md#listeventlogspaginatorname)
- [ListProjectsPaginatorName](./literals.md#listprojectspaginatorname)
- [ListSourceRepositoriesPaginatorName](./literals.md#listsourcerepositoriespaginatorname)
- [ListSourceRepositoryBranchesPaginatorName](./literals.md#listsourcerepositorybranchespaginatorname)
- [ListSpacesPaginatorName](./literals.md#listspacespaginatorname)
- [ListWorkflowRunsPaginatorName](./literals.md#listworkflowrunspaginatorname)
- [ListWorkflowsPaginatorName](./literals.md#listworkflowspaginatorname)
- [OperationTypeType](./literals.md#operationtypetype)
- [UserTypeType](./literals.md#usertypetype)
- [WorkflowRunModeType](./literals.md#workflowrunmodetype)
- [WorkflowRunStatusType](./literals.md#workflowrunstatustype)
- [WorkflowStatusType](./literals.md#workflowstatustype)
- [CodeCatalystServiceName](./literals.md#codecatalystservicename)
- [ServiceName](./literals.md#servicename)
- [ResourceServiceName](./literals.md#resourceservicename)
- [PaginatorName](./literals.md#paginatorname)




## Type definitions

Type annotations for [type definitions](./type_defs.md) used in methods and schema.

- [AccessTokenSummaryTypeDef](./type_defs.md#accesstokensummarytypedef)
- [TimestampTypeDef](./type_defs.md#timestamptypedef)
- [ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef)
- [IdeConfigurationTypeDef](./type_defs.md#ideconfigurationtypedef)
- [PersistentStorageConfigurationTypeDef](./type_defs.md#persistentstorageconfigurationtypedef)
- [RepositoryInputTypeDef](./type_defs.md#repositoryinputtypedef)
- [CreateProjectRequestRequestTypeDef](./type_defs.md#createprojectrequestrequesttypedef)
- [CreateSourceRepositoryBranchRequestRequestTypeDef](./type_defs.md#createsourcerepositorybranchrequestrequesttypedef)
- [CreateSourceRepositoryRequestRequestTypeDef](./type_defs.md#createsourcerepositoryrequestrequesttypedef)
- [DeleteAccessTokenRequestRequestTypeDef](./type_defs.md#deleteaccesstokenrequestrequesttypedef)
- [DeleteDevEnvironmentRequestRequestTypeDef](./type_defs.md#deletedevenvironmentrequestrequesttypedef)
- [DeleteProjectRequestRequestTypeDef](./type_defs.md#deleteprojectrequestrequesttypedef)
- [DeleteSourceRepositoryRequestRequestTypeDef](./type_defs.md#deletesourcerepositoryrequestrequesttypedef)
- [DeleteSpaceRequestRequestTypeDef](./type_defs.md#deletespacerequestrequesttypedef)
- [DevEnvironmentAccessDetailsTypeDef](./type_defs.md#devenvironmentaccessdetailstypedef)
- [DevEnvironmentRepositorySummaryTypeDef](./type_defs.md#devenvironmentrepositorysummarytypedef)
- [ExecuteCommandSessionConfigurationTypeDef](./type_defs.md#executecommandsessionconfigurationtypedef)
- [DevEnvironmentSessionSummaryTypeDef](./type_defs.md#devenvironmentsessionsummarytypedef)
- [IdeTypeDef](./type_defs.md#idetypedef)
- [PersistentStorageTypeDef](./type_defs.md#persistentstoragetypedef)
- [EmailAddressTypeDef](./type_defs.md#emailaddresstypedef)
- [EventPayloadTypeDef](./type_defs.md#eventpayloadtypedef)
- [ProjectInformationTypeDef](./type_defs.md#projectinformationtypedef)
- [UserIdentityTypeDef](./type_defs.md#useridentitytypedef)
- [FilterTypeDef](./type_defs.md#filtertypedef)
- [GetDevEnvironmentRequestRequestTypeDef](./type_defs.md#getdevenvironmentrequestrequesttypedef)
- [GetProjectRequestRequestTypeDef](./type_defs.md#getprojectrequestrequesttypedef)
- [GetSourceRepositoryCloneUrlsRequestRequestTypeDef](./type_defs.md#getsourcerepositorycloneurlsrequestrequesttypedef)
- [GetSourceRepositoryRequestRequestTypeDef](./type_defs.md#getsourcerepositoryrequestrequesttypedef)
- [GetSpaceRequestRequestTypeDef](./type_defs.md#getspacerequestrequesttypedef)
- [GetSubscriptionRequestRequestTypeDef](./type_defs.md#getsubscriptionrequestrequesttypedef)
- [GetUserDetailsRequestRequestTypeDef](./type_defs.md#getuserdetailsrequestrequesttypedef)
- [GetWorkflowRequestRequestTypeDef](./type_defs.md#getworkflowrequestrequesttypedef)
- [WorkflowDefinitionTypeDef](./type_defs.md#workflowdefinitiontypedef)
- [GetWorkflowRunRequestRequestTypeDef](./type_defs.md#getworkflowrunrequestrequesttypedef)
- [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
- [ListAccessTokensRequestRequestTypeDef](./type_defs.md#listaccesstokensrequestrequesttypedef)
- [ListDevEnvironmentSessionsRequestRequestTypeDef](./type_defs.md#listdevenvironmentsessionsrequestrequesttypedef)
- [ProjectListFilterTypeDef](./type_defs.md#projectlistfiltertypedef)
- [ProjectSummaryTypeDef](./type_defs.md#projectsummarytypedef)
- [ListSourceRepositoriesItemTypeDef](./type_defs.md#listsourcerepositoriesitemtypedef)
- [ListSourceRepositoriesRequestRequestTypeDef](./type_defs.md#listsourcerepositoriesrequestrequesttypedef)
- [ListSourceRepositoryBranchesItemTypeDef](./type_defs.md#listsourcerepositorybranchesitemtypedef)
- [ListSourceRepositoryBranchesRequestRequestTypeDef](./type_defs.md#listsourcerepositorybranchesrequestrequesttypedef)
- [ListSpacesRequestRequestTypeDef](./type_defs.md#listspacesrequestrequesttypedef)
- [SpaceSummaryTypeDef](./type_defs.md#spacesummarytypedef)
- [ListWorkflowRunsRequestRequestTypeDef](./type_defs.md#listworkflowrunsrequestrequesttypedef)
- [WorkflowRunSummaryTypeDef](./type_defs.md#workflowrunsummarytypedef)
- [ListWorkflowsRequestRequestTypeDef](./type_defs.md#listworkflowsrequestrequesttypedef)
- [StartWorkflowRunRequestRequestTypeDef](./type_defs.md#startworkflowrunrequestrequesttypedef)
- [StopDevEnvironmentRequestRequestTypeDef](./type_defs.md#stopdevenvironmentrequestrequesttypedef)
- [StopDevEnvironmentSessionRequestRequestTypeDef](./type_defs.md#stopdevenvironmentsessionrequestrequesttypedef)
- [UpdateProjectRequestRequestTypeDef](./type_defs.md#updateprojectrequestrequesttypedef)
- [UpdateSpaceRequestRequestTypeDef](./type_defs.md#updatespacerequestrequesttypedef)
- [WorkflowDefinitionSummaryTypeDef](./type_defs.md#workflowdefinitionsummarytypedef)
- [CreateAccessTokenRequestRequestTypeDef](./type_defs.md#createaccesstokenrequestrequesttypedef)
- [ListEventLogsRequestRequestTypeDef](./type_defs.md#listeventlogsrequestrequesttypedef)
- [CreateAccessTokenResponseTypeDef](./type_defs.md#createaccesstokenresponsetypedef)
- [CreateDevEnvironmentResponseTypeDef](./type_defs.md#createdevenvironmentresponsetypedef)
- [CreateProjectResponseTypeDef](./type_defs.md#createprojectresponsetypedef)
- [CreateSourceRepositoryBranchResponseTypeDef](./type_defs.md#createsourcerepositorybranchresponsetypedef)
- [CreateSourceRepositoryResponseTypeDef](./type_defs.md#createsourcerepositoryresponsetypedef)
- [DeleteDevEnvironmentResponseTypeDef](./type_defs.md#deletedevenvironmentresponsetypedef)
- [DeleteProjectResponseTypeDef](./type_defs.md#deleteprojectresponsetypedef)
- [DeleteSourceRepositoryResponseTypeDef](./type_defs.md#deletesourcerepositoryresponsetypedef)
- [DeleteSpaceResponseTypeDef](./type_defs.md#deletespaceresponsetypedef)
- [GetProjectResponseTypeDef](./type_defs.md#getprojectresponsetypedef)
- [GetSourceRepositoryCloneUrlsResponseTypeDef](./type_defs.md#getsourcerepositorycloneurlsresponsetypedef)
- [GetSourceRepositoryResponseTypeDef](./type_defs.md#getsourcerepositoryresponsetypedef)
- [GetSpaceResponseTypeDef](./type_defs.md#getspaceresponsetypedef)
- [GetSubscriptionResponseTypeDef](./type_defs.md#getsubscriptionresponsetypedef)
- [GetWorkflowRunResponseTypeDef](./type_defs.md#getworkflowrunresponsetypedef)
- [ListAccessTokensResponseTypeDef](./type_defs.md#listaccesstokensresponsetypedef)
- [StartDevEnvironmentResponseTypeDef](./type_defs.md#startdevenvironmentresponsetypedef)
- [StartWorkflowRunResponseTypeDef](./type_defs.md#startworkflowrunresponsetypedef)
- [StopDevEnvironmentResponseTypeDef](./type_defs.md#stopdevenvironmentresponsetypedef)
- [StopDevEnvironmentSessionResponseTypeDef](./type_defs.md#stopdevenvironmentsessionresponsetypedef)
- [UpdateProjectResponseTypeDef](./type_defs.md#updateprojectresponsetypedef)
- [UpdateSpaceResponseTypeDef](./type_defs.md#updatespaceresponsetypedef)
- [VerifySessionResponseTypeDef](./type_defs.md#verifysessionresponsetypedef)
- [StartDevEnvironmentRequestRequestTypeDef](./type_defs.md#startdevenvironmentrequestrequesttypedef)
- [UpdateDevEnvironmentRequestRequestTypeDef](./type_defs.md#updatedevenvironmentrequestrequesttypedef)
- [UpdateDevEnvironmentResponseTypeDef](./type_defs.md#updatedevenvironmentresponsetypedef)
- [CreateDevEnvironmentRequestRequestTypeDef](./type_defs.md#createdevenvironmentrequestrequesttypedef)
- [StartDevEnvironmentSessionResponseTypeDef](./type_defs.md#startdevenvironmentsessionresponsetypedef)
- [DevEnvironmentSessionConfigurationTypeDef](./type_defs.md#devenvironmentsessionconfigurationtypedef)
- [ListDevEnvironmentSessionsResponseTypeDef](./type_defs.md#listdevenvironmentsessionsresponsetypedef)
- [DevEnvironmentSummaryTypeDef](./type_defs.md#devenvironmentsummarytypedef)
- [GetDevEnvironmentResponseTypeDef](./type_defs.md#getdevenvironmentresponsetypedef)
- [GetUserDetailsResponseTypeDef](./type_defs.md#getuserdetailsresponsetypedef)
- [EventLogEntryTypeDef](./type_defs.md#eventlogentrytypedef)
- [ListDevEnvironmentsRequestRequestTypeDef](./type_defs.md#listdevenvironmentsrequestrequesttypedef)
- [GetWorkflowResponseTypeDef](./type_defs.md#getworkflowresponsetypedef)
- [ListAccessTokensRequestPaginateTypeDef](./type_defs.md#listaccesstokensrequestpaginatetypedef)
- [ListDevEnvironmentSessionsRequestPaginateTypeDef](./type_defs.md#listdevenvironmentsessionsrequestpaginatetypedef)
- [ListDevEnvironmentsRequestPaginateTypeDef](./type_defs.md#listdevenvironmentsrequestpaginatetypedef)
- [ListEventLogsRequestPaginateTypeDef](./type_defs.md#listeventlogsrequestpaginatetypedef)
- [ListSourceRepositoriesRequestPaginateTypeDef](./type_defs.md#listsourcerepositoriesrequestpaginatetypedef)
- [ListSourceRepositoryBranchesRequestPaginateTypeDef](./type_defs.md#listsourcerepositorybranchesrequestpaginatetypedef)
- [ListSpacesRequestPaginateTypeDef](./type_defs.md#listspacesrequestpaginatetypedef)
- [ListWorkflowRunsRequestPaginateTypeDef](./type_defs.md#listworkflowrunsrequestpaginatetypedef)
- [ListWorkflowsRequestPaginateTypeDef](./type_defs.md#listworkflowsrequestpaginatetypedef)
- [ListProjectsRequestPaginateTypeDef](./type_defs.md#listprojectsrequestpaginatetypedef)
- [ListProjectsRequestRequestTypeDef](./type_defs.md#listprojectsrequestrequesttypedef)
- [ListProjectsResponseTypeDef](./type_defs.md#listprojectsresponsetypedef)
- [ListSourceRepositoriesResponseTypeDef](./type_defs.md#listsourcerepositoriesresponsetypedef)
- [ListSourceRepositoryBranchesResponseTypeDef](./type_defs.md#listsourcerepositorybranchesresponsetypedef)
- [ListSpacesResponseTypeDef](./type_defs.md#listspacesresponsetypedef)
- [ListWorkflowRunsResponseTypeDef](./type_defs.md#listworkflowrunsresponsetypedef)
- [WorkflowSummaryTypeDef](./type_defs.md#workflowsummarytypedef)
- [StartDevEnvironmentSessionRequestRequestTypeDef](./type_defs.md#startdevenvironmentsessionrequestrequesttypedef)
- [ListDevEnvironmentsResponseTypeDef](./type_defs.md#listdevenvironmentsresponsetypedef)
- [ListEventLogsResponseTypeDef](./type_defs.md#listeventlogsresponsetypedef)
- [ListWorkflowsResponseTypeDef](./type_defs.md#listworkflowsresponsetypedef)

