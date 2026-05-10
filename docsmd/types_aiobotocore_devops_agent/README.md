# DevOpsAgentService module

> [Index](../README.md) > DevOpsAgentService


!!! note ""

    Auto-generated documentation for [DevOpsAgentService](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/devops-agent.html#devopsagentservice)
    type annotations stubs module [types-aiobotocore-devops-agent](https://pypi.org/project/types-aiobotocore-devops-agent/).

## How to install

### Generate locally (recommended)

You can generate type annotations for `aiobotocore` package locally with `mypy-boto3-builder`.
Use [uv](https://docs.astral.sh/uv/getting-started/installation/) for build isolation.

1. Run mypy-boto3-builder in your package root directory: `uvx --with 'aiobotocore==3.7.0' mypy-boto3-builder`
1. Select `aiobotocore` AWS SDK.
1. Add `DevOpsAgentService` service.
1. Use provided commands to install generated packages.



### From PyPI with pip

Install `types-aiobotocore` for `DevOpsAgentService` service.

```bash
# install with aiobotocore type annotations
python -m pip install 'types-aiobotocore[devops-agent]'

# Lite version does not provide session.client/resource overloads
# it is more RAM-friendly, but requires explicit type annotations
python -m pip install 'types-aiobotocore-lite[devops-agent]'

# standalone installation
python -m pip install types-aiobotocore-devops-agent
```



## How to uninstall

```bash
python -m pip uninstall -y types-aiobotocore-devops-agent
```

## Usage

Code samples can be found in [Examples](./usage.md).

## DevOpsAgentServiceClient

Type annotations and code completion for  `#!python session.create_client("devops-agent")` as [DevOpsAgentServiceClient](./client.md)
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/devops-agent.html#DevOpsAgentService.Client)

```python
# DevOpsAgentServiceClient usage example

from aiobotocore.session import get_session

from types_aiobotocore_devops_agent.client import DevOpsAgentServiceClient


session = get_session()
async with session.create_client("devops-agent") as client:
    client: DevOpsAgentServiceClient
```


## Paginators

Type annotations and code completion for
[paginators](./paginators.md)
from `#!python session.create_client("devops-agent").get_paginator("...")`.

```python
# ListAgentSpacesPaginator usage example

from types_aiobotocore_devops_agent.paginator import ListAgentSpacesPaginator

def get_list_agent_spaces_paginator() -> ListAgentSpacesPaginator:
    return client.get_paginator("list_agent_spaces"))
```

- [ListAgentSpacesPaginator](./paginators.md#listagentspacespaginator)
- [ListAssociationsPaginator](./paginators.md#listassociationspaginator)
- [ListBacklogTasksPaginator](./paginators.md#listbacklogtaskspaginator)
- [ListExecutionsPaginator](./paginators.md#listexecutionspaginator)
- [ListGoalsPaginator](./paginators.md#listgoalspaginator)
- [ListJournalRecordsPaginator](./paginators.md#listjournalrecordspaginator)
- [ListServicesPaginator](./paginators.md#listservicespaginator)








## Literals

Type annotations for [literals](./literals.md) used in methods and schema.

```python
# AuthFlowType usage example

from types_aiobotocore_devops_agent.literals import AuthFlowType

def get_value() -> AuthFlowType:
    return "iam"
```

- [AuthFlowType](./literals.md#authflowtype)
- [EventChannelTypeType](./literals.md#eventchanneltypetype)
- [ExecutionStatusType](./literals.md#executionstatustype)
- [GitLabTokenTypeType](./literals.md#gitlabtokentypetype)
- [GithubRepoOwnerTypeType](./literals.md#githubrepoownertypetype)
- [GoalStatusType](./literals.md#goalstatustype)
- [GoalTypeType](./literals.md#goaltypetype)
- [IpAddressTypeType](./literals.md#ipaddresstypetype)
- [ListAgentSpacesPaginatorName](./literals.md#listagentspacespaginatorname)
- [ListAssociationsPaginatorName](./literals.md#listassociationspaginatorname)
- [ListBacklogTasksPaginatorName](./literals.md#listbacklogtaskspaginatorname)
- [ListExecutionsPaginatorName](./literals.md#listexecutionspaginatorname)
- [ListGoalsPaginatorName](./literals.md#listgoalspaginatorname)
- [ListJournalRecordsPaginatorName](./literals.md#listjournalrecordspaginatorname)
- [ListServicesPaginatorName](./literals.md#listservicespaginatorname)
- [MCPServerAuthorizationMethodType](./literals.md#mcpserverauthorizationmethodtype)
- [MonitorAccountTypeType](./literals.md#monitoraccounttypetype)
- [NewRelicRegionType](./literals.md#newrelicregiontype)
- [OrderTypeType](./literals.md#ordertypetype)
- [PostRegisterServiceSupportedServiceType](./literals.md#postregisterservicesupportedservicetype)
- [PriorityType](./literals.md#prioritytype)
- [PrivateConnectionStatusType](./literals.md#privateconnectionstatustype)
- [PrivateConnectionTypeType](./literals.md#privateconnectiontypetype)
- [RecommendationPriorityType](./literals.md#recommendationprioritytype)
- [RecommendationStatusType](./literals.md#recommendationstatustype)
- [SchedulerStateType](./literals.md#schedulerstatetype)
- [ServiceType](./literals.md#servicetype)
- [SourceAccountTypeType](./literals.md#sourceaccounttypetype)
- [TaskSortFieldType](./literals.md#tasksortfieldtype)
- [TaskSortOrderType](./literals.md#tasksortordertype)
- [TaskStatusType](./literals.md#taskstatustype)
- [TaskTypeType](./literals.md#tasktypetype)
- [UserTypeType](./literals.md#usertypetype)
- [ValidationStatusType](./literals.md#validationstatustype)
- [WebhookTypeType](./literals.md#webhooktypetype)
- [DevOpsAgentServiceServiceName](./literals.md#devopsagentserviceservicename)
- [ServiceName](./literals.md#servicename)
- [ResourceServiceName](./literals.md#resourceservicename)
- [PaginatorName](./literals.md#paginatorname)




## Type definitions

Type annotations for [type definitions](./type_defs.md) used in methods and schema.

- [AWSConfigurationTypeDef](./type_defs.md#awsconfigurationtypedef)
- [RegisteredAzureDevOpsServiceDetailsTypeDef](./type_defs.md#registeredazuredevopsservicedetailstypedef)
- [RegisteredAzureIdentityDetailsOutputTypeDef](./type_defs.md#registeredazureidentitydetailsoutputtypedef)
- [RegisteredGitLabServiceDetailsTypeDef](./type_defs.md#registeredgitlabservicedetailstypedef)
- [RegisteredGithubServiceDetailsTypeDef](./type_defs.md#registeredgithubservicedetailstypedef)
- [RegisteredGrafanaServerDetailsTypeDef](./type_defs.md#registeredgrafanaserverdetailstypedef)
- [RegisteredMCPServerDetailsTypeDef](./type_defs.md#registeredmcpserverdetailstypedef)
- [RegisteredNewRelicDetailsTypeDef](./type_defs.md#registerednewrelicdetailstypedef)
- [RegisteredPagerDutyDetailsTypeDef](./type_defs.md#registeredpagerdutydetailstypedef)
- [RegisteredServiceNowDetailsTypeDef](./type_defs.md#registeredservicenowdetailstypedef)
- [RegisteredSlackServiceDetailsTypeDef](./type_defs.md#registeredslackservicedetailstypedef)
- [OAuthAdditionalStepDetailsTypeDef](./type_defs.md#oauthadditionalstepdetailstypedef)
- [AgentSpaceTypeDef](./type_defs.md#agentspacetypedef)
- [AssistantMessageBlockTypeDef](./type_defs.md#assistantmessageblocktypedef)
- [GenericWebhookTypeDef](./type_defs.md#genericwebhooktypedef)
- [ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef)
- [AzureConfigurationTypeDef](./type_defs.md#azureconfigurationtypedef)
- [AzureDevOpsConfigurationTypeDef](./type_defs.md#azuredevopsconfigurationtypedef)
- [ChatExecutionTypeDef](./type_defs.md#chatexecutiontypedef)
- [CreateAgentSpaceInputTypeDef](./type_defs.md#createagentspaceinputtypedef)
- [ReferenceInputTypeDef](./type_defs.md#referenceinputtypedef)
- [CreateChatRequestTypeDef](./type_defs.md#createchatrequesttypedef)
- [MCPServerAuthorizationDiscoveryConfigTypeDef](./type_defs.md#mcpserverauthorizationdiscoveryconfigtypedef)
- [DeleteAgentSpaceInputTypeDef](./type_defs.md#deleteagentspaceinputtypedef)
- [DeletePrivateConnectionInputTypeDef](./type_defs.md#deleteprivateconnectioninputtypedef)
- [DeregisterServiceInputTypeDef](./type_defs.md#deregisterserviceinputtypedef)
- [DescribePrivateConnectionInputTypeDef](./type_defs.md#describeprivateconnectioninputtypedef)
- [DisableOperatorAppInputTypeDef](./type_defs.md#disableoperatorappinputtypedef)
- [DisassociateServiceInputTypeDef](./type_defs.md#disassociateserviceinputtypedef)
- [DynatraceConfigurationOutputTypeDef](./type_defs.md#dynatraceconfigurationoutputtypedef)
- [DynatraceConfigurationTypeDef](./type_defs.md#dynatraceconfigurationtypedef)
- [DynatraceOAuthClientCredentialsConfigTypeDef](./type_defs.md#dynatraceoauthclientcredentialsconfigtypedef)
- [EnableOperatorAppInputTypeDef](./type_defs.md#enableoperatorappinputtypedef)
- [IamAuthConfigurationTypeDef](./type_defs.md#iamauthconfigurationtypedef)
- [IdcAuthConfigurationTypeDef](./type_defs.md#idcauthconfigurationtypedef)
- [IdpAuthConfigurationTypeDef](./type_defs.md#idpauthconfigurationtypedef)
- [EventChannelDetailsTypeDef](./type_defs.md#eventchanneldetailstypedef)
- [ExecutionTypeDef](./type_defs.md#executiontypedef)
- [UsageMetricTypeDef](./type_defs.md#usagemetrictypedef)
- [GetAgentSpaceInputTypeDef](./type_defs.md#getagentspaceinputtypedef)
- [GetAssociationInputTypeDef](./type_defs.md#getassociationinputtypedef)
- [GetBacklogTaskRequestTypeDef](./type_defs.md#getbacklogtaskrequesttypedef)
- [GetOperatorAppInputTypeDef](./type_defs.md#getoperatorappinputtypedef)
- [GetRecommendationRequestTypeDef](./type_defs.md#getrecommendationrequesttypedef)
- [GetServiceInputTypeDef](./type_defs.md#getserviceinputtypedef)
- [GitHubConfigurationTypeDef](./type_defs.md#githubconfigurationtypedef)
- [GitLabConfigurationTypeDef](./type_defs.md#gitlabconfigurationtypedef)
- [GitLabDetailsTypeDef](./type_defs.md#gitlabdetailstypedef)
- [GoalContentTypeDef](./type_defs.md#goalcontenttypedef)
- [GoalScheduleInputTypeDef](./type_defs.md#goalscheduleinputtypedef)
- [GoalScheduleTypeDef](./type_defs.md#goalscheduletypedef)
- [UserReferenceTypeDef](./type_defs.md#userreferencetypedef)
- [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
- [ListAgentSpacesInputTypeDef](./type_defs.md#listagentspacesinputtypedef)
- [ListAssociationsInputTypeDef](./type_defs.md#listassociationsinputtypedef)
- [ListChatsRequestTypeDef](./type_defs.md#listchatsrequesttypedef)
- [ListExecutionsRequestTypeDef](./type_defs.md#listexecutionsrequesttypedef)
- [ListGoalsRequestTypeDef](./type_defs.md#listgoalsrequesttypedef)
- [ListJournalRecordsRequestTypeDef](./type_defs.md#listjournalrecordsrequesttypedef)
- [ListPendingMessagesRequestTypeDef](./type_defs.md#listpendingmessagesrequesttypedef)
- [PrivateConnectionSummaryTypeDef](./type_defs.md#privateconnectionsummarytypedef)
- [ListRecommendationsRequestTypeDef](./type_defs.md#listrecommendationsrequesttypedef)
- [ListServicesInputTypeDef](./type_defs.md#listservicesinputtypedef)
- [ListTagsForResourceRequestTypeDef](./type_defs.md#listtagsforresourcerequesttypedef)
- [ListWebhooksInputTypeDef](./type_defs.md#listwebhooksinputtypedef)
- [WebhookTypeDef](./type_defs.md#webhooktypedef)
- [MCPServerAPIKeyConfigTypeDef](./type_defs.md#mcpserverapikeyconfigtypedef)
- [MCPServerBearerTokenConfigTypeDef](./type_defs.md#mcpserverbearertokenconfigtypedef)
- [MCPServerOAuth3LOConfigTypeDef](./type_defs.md#mcpserveroauth3loconfigtypedef)
- [MCPServerOAuthClientCredentialsConfigTypeDef](./type_defs.md#mcpserveroauthclientcredentialsconfigtypedef)
- [MCPServerConfigurationOutputTypeDef](./type_defs.md#mcpserverconfigurationoutputtypedef)
- [MCPServerConfigurationTypeDef](./type_defs.md#mcpserverconfigurationtypedef)
- [MCPServerGrafanaConfigurationOutputTypeDef](./type_defs.md#mcpservergrafanaconfigurationoutputtypedef)
- [MCPServerGrafanaConfigurationTypeDef](./type_defs.md#mcpservergrafanaconfigurationtypedef)
- [MCPServerNewRelicConfigurationTypeDef](./type_defs.md#mcpservernewrelicconfigurationtypedef)
- [UserMessageBlockTypeDef](./type_defs.md#usermessageblocktypedef)
- [NewRelicApiKeyConfigTypeDef](./type_defs.md#newrelicapikeyconfigtypedef)
- [PagerDutyOAuthClientCredentialsConfigTypeDef](./type_defs.md#pagerdutyoauthclientcredentialsconfigtypedef)
- [PagerDutyConfigurationOutputTypeDef](./type_defs.md#pagerdutyconfigurationoutputtypedef)
- [PagerDutyConfigurationTypeDef](./type_defs.md#pagerdutyconfigurationtypedef)
- [SelfManagedInputTypeDef](./type_defs.md#selfmanagedinputtypedef)
- [ServiceManagedInputTypeDef](./type_defs.md#servicemanagedinputtypedef)
- [RecommendationContentTypeDef](./type_defs.md#recommendationcontenttypedef)
- [ReferenceOutputTypeDef](./type_defs.md#referenceoutputtypedef)
- [RegisteredAzureIdentityDetailsTypeDef](./type_defs.md#registeredazureidentitydetailstypedef)
- [SendMessageJsonDeltaTypeDef](./type_defs.md#sendmessagejsondeltatypedef)
- [SendMessageTextDeltaTypeDef](./type_defs.md#sendmessagetextdeltatypedef)
- [SendMessageContentBlockStartEventTypeDef](./type_defs.md#sendmessagecontentblockstarteventtypedef)
- [SendMessageContentBlockStopEventTypeDef](./type_defs.md#sendmessagecontentblockstopeventtypedef)
- [SendMessageContextTypeDef](./type_defs.md#sendmessagecontexttypedef)
- [SendMessageResponseCreatedEventTypeDef](./type_defs.md#sendmessageresponsecreatedeventtypedef)
- [SendMessageResponseFailedEventTypeDef](./type_defs.md#sendmessageresponsefailedeventtypedef)
- [SendMessageResponseInProgressEventTypeDef](./type_defs.md#sendmessageresponseinprogresseventtypedef)
- [SendMessageSummaryEventTypeDef](./type_defs.md#sendmessagesummaryeventtypedef)
- [SendMessageUsageInfoTypeDef](./type_defs.md#sendmessageusageinfotypedef)
- [ServiceNowConfigurationOutputTypeDef](./type_defs.md#servicenowconfigurationoutputtypedef)
- [SourceAwsConfigurationTypeDef](./type_defs.md#sourceawsconfigurationtypedef)
- [ServiceNowConfigurationTypeDef](./type_defs.md#servicenowconfigurationtypedef)
- [ServiceNowOAuthClientCredentialsConfigTypeDef](./type_defs.md#servicenowoauthclientcredentialsconfigtypedef)
- [SlackChannelTypeDef](./type_defs.md#slackchanneltypedef)
- [TagResourceRequestTypeDef](./type_defs.md#tagresourcerequesttypedef)
- [TimestampTypeDef](./type_defs.md#timestamptypedef)
- [UntagResourceRequestTypeDef](./type_defs.md#untagresourcerequesttypedef)
- [UpdateAgentSpaceInputTypeDef](./type_defs.md#updateagentspaceinputtypedef)
- [UpdateBacklogTaskRequestTypeDef](./type_defs.md#updatebacklogtaskrequesttypedef)
- [UpdateOperatorAppIdpConfigInputTypeDef](./type_defs.md#updateoperatorappidpconfiginputtypedef)
- [UpdatePrivateConnectionCertificateInputTypeDef](./type_defs.md#updateprivateconnectioncertificateinputtypedef)
- [UpdateRecommendationRequestTypeDef](./type_defs.md#updaterecommendationrequesttypedef)
- [ValidateAwsAssociationsInputTypeDef](./type_defs.md#validateawsassociationsinputtypedef)
- [AdditionalServiceDetailsTypeDef](./type_defs.md#additionalservicedetailstypedef)
- [AdditionalServiceRegistrationStepTypeDef](./type_defs.md#additionalserviceregistrationsteptypedef)
- [CreateAgentSpaceOutputTypeDef](./type_defs.md#createagentspaceoutputtypedef)
- [CreateChatResponseTypeDef](./type_defs.md#createchatresponsetypedef)
- [CreatePrivateConnectionOutputTypeDef](./type_defs.md#createprivateconnectionoutputtypedef)
- [DeletePrivateConnectionOutputTypeDef](./type_defs.md#deleteprivateconnectionoutputtypedef)
- [DescribePrivateConnectionOutputTypeDef](./type_defs.md#describeprivateconnectionoutputtypedef)
- [EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef)
- [GetAgentSpaceOutputTypeDef](./type_defs.md#getagentspaceoutputtypedef)
- [ListAgentSpacesOutputTypeDef](./type_defs.md#listagentspacesoutputtypedef)
- [ListTagsForResourceResponseTypeDef](./type_defs.md#listtagsforresourceresponsetypedef)
- [UpdateAgentSpaceOutputTypeDef](./type_defs.md#updateagentspaceoutputtypedef)
- [UpdatePrivateConnectionCertificateOutputTypeDef](./type_defs.md#updateprivateconnectioncertificateoutputtypedef)
- [ListChatsResponseTypeDef](./type_defs.md#listchatsresponsetypedef)
- [CreateBacklogTaskRequestTypeDef](./type_defs.md#createbacklogtaskrequesttypedef)
- [DatadogAuthorizationConfigTypeDef](./type_defs.md#datadogauthorizationconfigtypedef)
- [DynatraceServiceAuthorizationConfigTypeDef](./type_defs.md#dynatraceserviceauthorizationconfigtypedef)
- [EnableOperatorAppOutputTypeDef](./type_defs.md#enableoperatorappoutputtypedef)
- [GetOperatorAppOutputTypeDef](./type_defs.md#getoperatorappoutputtypedef)
- [UpdateOperatorAppIdpConfigOutputTypeDef](./type_defs.md#updateoperatorappidpconfigoutputtypedef)
- [ListExecutionsResponseTypeDef](./type_defs.md#listexecutionsresponsetypedef)
- [GetAccountUsageOutputTypeDef](./type_defs.md#getaccountusageoutputtypedef)
- [UpdateGoalRequestTypeDef](./type_defs.md#updategoalrequesttypedef)
- [GoalTypeDef](./type_defs.md#goaltypedef)
- [JournalRecordTypeDef](./type_defs.md#journalrecordtypedef)
- [ListAgentSpacesInputPaginateTypeDef](./type_defs.md#listagentspacesinputpaginatetypedef)
- [ListAssociationsInputPaginateTypeDef](./type_defs.md#listassociationsinputpaginatetypedef)
- [ListExecutionsRequestPaginateTypeDef](./type_defs.md#listexecutionsrequestpaginatetypedef)
- [ListGoalsRequestPaginateTypeDef](./type_defs.md#listgoalsrequestpaginatetypedef)
- [ListJournalRecordsRequestPaginateTypeDef](./type_defs.md#listjournalrecordsrequestpaginatetypedef)
- [ListServicesInputPaginateTypeDef](./type_defs.md#listservicesinputpaginatetypedef)
- [ListPrivateConnectionsOutputTypeDef](./type_defs.md#listprivateconnectionsoutputtypedef)
- [ListWebhooksOutputTypeDef](./type_defs.md#listwebhooksoutputtypedef)
- [MCPServerAuthorizationConfigTypeDef](./type_defs.md#mcpserverauthorizationconfigtypedef)
- [MessageTypeDef](./type_defs.md#messagetypedef)
- [NewRelicServiceAuthorizationConfigTypeDef](./type_defs.md#newrelicserviceauthorizationconfigtypedef)
- [PagerDutyAuthorizationConfigTypeDef](./type_defs.md#pagerdutyauthorizationconfigtypedef)
- [PrivateConnectionModeTypeDef](./type_defs.md#privateconnectionmodetypedef)
- [RecommendationTypeDef](./type_defs.md#recommendationtypedef)
- [TaskTypeDef](./type_defs.md#tasktypedef)
- [RegisteredAzureIdentityDetailsUnionTypeDef](./type_defs.md#registeredazureidentitydetailsuniontypedef)
- [SendMessageContentBlockDeltaTypeDef](./type_defs.md#sendmessagecontentblockdeltatypedef)
- [SendMessageRequestTypeDef](./type_defs.md#sendmessagerequesttypedef)
- [SendMessageResponseCompletedEventTypeDef](./type_defs.md#sendmessageresponsecompletedeventtypedef)
- [ServiceNowServiceAuthorizationConfigTypeDef](./type_defs.md#servicenowserviceauthorizationconfigtypedef)
- [SlackTransmissionTargetTypeDef](./type_defs.md#slacktransmissiontargettypedef)
- [TaskFilterTypeDef](./type_defs.md#taskfiltertypedef)
- [RegisteredServiceTypeDef](./type_defs.md#registeredservicetypedef)
- [RegisterServiceOutputTypeDef](./type_defs.md#registerserviceoutputtypedef)
- [DatadogServiceDetailsTypeDef](./type_defs.md#datadogservicedetailstypedef)
- [DynatraceServiceDetailsTypeDef](./type_defs.md#dynatraceservicedetailstypedef)
- [ListGoalsResponseTypeDef](./type_defs.md#listgoalsresponsetypedef)
- [UpdateGoalResponseTypeDef](./type_defs.md#updategoalresponsetypedef)
- [ListJournalRecordsResponseTypeDef](./type_defs.md#listjournalrecordsresponsetypedef)
- [GrafanaServiceDetailsTypeDef](./type_defs.md#grafanaservicedetailstypedef)
- [MCPServerDetailsTypeDef](./type_defs.md#mcpserverdetailstypedef)
- [PendingMessageTypeDef](./type_defs.md#pendingmessagetypedef)
- [NewRelicServiceDetailsTypeDef](./type_defs.md#newrelicservicedetailstypedef)
- [PagerDutyDetailsTypeDef](./type_defs.md#pagerdutydetailstypedef)
- [CreatePrivateConnectionInputTypeDef](./type_defs.md#createprivateconnectioninputtypedef)
- [GetRecommendationResponseTypeDef](./type_defs.md#getrecommendationresponsetypedef)
- [ListRecommendationsResponseTypeDef](./type_defs.md#listrecommendationsresponsetypedef)
- [UpdateRecommendationResponseTypeDef](./type_defs.md#updaterecommendationresponsetypedef)
- [CreateBacklogTaskResponseTypeDef](./type_defs.md#createbacklogtaskresponsetypedef)
- [GetBacklogTaskResponseTypeDef](./type_defs.md#getbacklogtaskresponsetypedef)
- [ListBacklogTasksResponseTypeDef](./type_defs.md#listbacklogtasksresponsetypedef)
- [UpdateBacklogTaskResponseTypeDef](./type_defs.md#updatebacklogtaskresponsetypedef)
- [SendMessageContentBlockDeltaEventTypeDef](./type_defs.md#sendmessagecontentblockdeltaeventtypedef)
- [ServiceNowServiceDetailsTypeDef](./type_defs.md#servicenowservicedetailstypedef)
- [SlackConfigurationTypeDef](./type_defs.md#slackconfigurationtypedef)
- [ListBacklogTasksRequestPaginateTypeDef](./type_defs.md#listbacklogtasksrequestpaginatetypedef)
- [ListBacklogTasksRequestTypeDef](./type_defs.md#listbacklogtasksrequesttypedef)
- [GetServiceOutputTypeDef](./type_defs.md#getserviceoutputtypedef)
- [ListServicesOutputTypeDef](./type_defs.md#listservicesoutputtypedef)
- [ListPendingMessagesResponseTypeDef](./type_defs.md#listpendingmessagesresponsetypedef)
- [SendMessageEventsTypeDef](./type_defs.md#sendmessageeventstypedef)
- [ServiceDetailsTypeDef](./type_defs.md#servicedetailstypedef)
- [ServiceConfigurationOutputTypeDef](./type_defs.md#serviceconfigurationoutputtypedef)
- [ServiceConfigurationTypeDef](./type_defs.md#serviceconfigurationtypedef)
- [SendMessageResponseTypeDef](./type_defs.md#sendmessageresponsetypedef)
- [RegisterServiceInputTypeDef](./type_defs.md#registerserviceinputtypedef)
- [AssociationTypeDef](./type_defs.md#associationtypedef)
- [ServiceConfigurationUnionTypeDef](./type_defs.md#serviceconfigurationuniontypedef)
- [AssociateServiceOutputTypeDef](./type_defs.md#associateserviceoutputtypedef)
- [GetAssociationOutputTypeDef](./type_defs.md#getassociationoutputtypedef)
- [ListAssociationsOutputTypeDef](./type_defs.md#listassociationsoutputtypedef)
- [UpdateAssociationOutputTypeDef](./type_defs.md#updateassociationoutputtypedef)
- [AssociateServiceInputTypeDef](./type_defs.md#associateserviceinputtypedef)
- [UpdateAssociationInputTypeDef](./type_defs.md#updateassociationinputtypedef)

