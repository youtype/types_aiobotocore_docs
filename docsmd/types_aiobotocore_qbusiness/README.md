# QBusiness module

> [Index](../README.md) > QBusiness


!!! note ""

    Auto-generated documentation for [QBusiness](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/qbusiness.html#qbusiness)
    type annotations stubs module [types-aiobotocore-qbusiness](https://pypi.org/project/types-aiobotocore-qbusiness/).

## How to install

### Generate locally (recommended)

You can generate type annotations for `aiobotocore` package locally with `mypy-boto3-builder`.
Use [uv](https://docs.astral.sh/uv/getting-started/installation/) for build isolation.

1. Run mypy-boto3-builder in your package root directory: `uvx --with 'aiobotocore==2.20.0' mypy-boto3-builder`
1. Select `aiobotocore` AWS SDK.
1. Add `QBusiness` service.
1. Use provided commands to install generated packages.



### From PyPI with pip

Install `types-aiobotocore` for `QBusiness` service.

```bash
# install with aiobotocore type annotations
python -m pip install 'types-aiobotocore[qbusiness]'

# Lite version does not provide session.client/resource overloads
# it is more RAM-friendly, but requires explicit type annotations
python -m pip install 'types-aiobotocore-lite[qbusiness]'

# standalone installation
python -m pip install types-aiobotocore-qbusiness
```



## How to uninstall

```bash
python -m pip uninstall -y types-aiobotocore-qbusiness
```

## Usage

Code samples can be found in [Examples](./usage.md).

## QBusinessClient

Type annotations and code completion for  `#!python session.create_client("qbusiness")` as [QBusinessClient](./client.md)
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/qbusiness.html#QBusiness.Client)

```python
# QBusinessClient usage example

from aiobotocore.session import get_session

from types_aiobotocore_qbusiness.client import QBusinessClient


session = get_session()
async with session.create_client("qbusiness") as client:
    client: QBusinessClient
```


## Paginators

Type annotations and code completion for
[paginators](./paginators.md)
from `#!python session.create_client("qbusiness").get_paginator("...")`.

```python
# GetChatControlsConfigurationPaginator usage example

from types_aiobotocore_qbusiness.paginator import GetChatControlsConfigurationPaginator

def get_get_chat_controls_configuration_paginator() -> GetChatControlsConfigurationPaginator:
    return client.get_paginator("get_chat_controls_configuration"))
```

- [GetChatControlsConfigurationPaginator](./paginators.md#getchatcontrolsconfigurationpaginator)
- [ListApplicationsPaginator](./paginators.md#listapplicationspaginator)
- [ListAttachmentsPaginator](./paginators.md#listattachmentspaginator)
- [ListConversationsPaginator](./paginators.md#listconversationspaginator)
- [ListDataAccessorsPaginator](./paginators.md#listdataaccessorspaginator)
- [ListDataSourceSyncJobsPaginator](./paginators.md#listdatasourcesyncjobspaginator)
- [ListDataSourcesPaginator](./paginators.md#listdatasourcespaginator)
- [ListDocumentsPaginator](./paginators.md#listdocumentspaginator)
- [ListGroupsPaginator](./paginators.md#listgroupspaginator)
- [ListIndicesPaginator](./paginators.md#listindicespaginator)
- [ListMessagesPaginator](./paginators.md#listmessagespaginator)
- [ListPluginActionsPaginator](./paginators.md#listpluginactionspaginator)
- [ListPluginTypeActionsPaginator](./paginators.md#listplugintypeactionspaginator)
- [ListPluginTypeMetadataPaginator](./paginators.md#listplugintypemetadatapaginator)
- [ListPluginsPaginator](./paginators.md#listpluginspaginator)
- [ListRetrieversPaginator](./paginators.md#listretrieverspaginator)
- [ListSubscriptionsPaginator](./paginators.md#listsubscriptionspaginator)
- [ListWebExperiencesPaginator](./paginators.md#listwebexperiencespaginator)
- [SearchRelevantContentPaginator](./paginators.md#searchrelevantcontentpaginator)








## Literals

Type annotations for [literals](./literals.md) used in methods and schema.

```python
# APISchemaTypeType usage example

from types_aiobotocore_qbusiness.literals import APISchemaTypeType

def get_value() -> APISchemaTypeType:
    return "OPEN_API_V3"
```

- [APISchemaTypeType](./literals.md#apischematypetype)
- [ActionPayloadFieldTypeType](./literals.md#actionpayloadfieldtypetype)
- [ApplicationStatusType](./literals.md#applicationstatustype)
- [AttachmentStatusType](./literals.md#attachmentstatustype)
- [AttachmentsControlModeType](./literals.md#attachmentscontrolmodetype)
- [AttributeTypeType](./literals.md#attributetypetype)
- [AttributeValueOperatorType](./literals.md#attributevalueoperatortype)
- [AutoSubscriptionStatusType](./literals.md#autosubscriptionstatustype)
- [BrowserExtensionType](./literals.md#browserextensiontype)
- [ChatModeType](./literals.md#chatmodetype)
- [ContentTypeType](./literals.md#contenttypetype)
- [CreatorModeControlType](./literals.md#creatormodecontroltype)
- [DataSourceStatusType](./literals.md#datasourcestatustype)
- [DataSourceSyncJobStatusType](./literals.md#datasourcesyncjobstatustype)
- [DocumentAttributeBoostingLevelType](./literals.md#documentattributeboostingleveltype)
- [DocumentContentOperatorType](./literals.md#documentcontentoperatortype)
- [DocumentEnrichmentConditionOperatorType](./literals.md#documentenrichmentconditionoperatortype)
- [DocumentStatusType](./literals.md#documentstatustype)
- [ErrorCodeType](./literals.md#errorcodetype)
- [GetChatControlsConfigurationPaginatorName](./literals.md#getchatcontrolsconfigurationpaginatorname)
- [GroupStatusType](./literals.md#groupstatustype)
- [IdentityTypeType](./literals.md#identitytypetype)
- [ImageExtractionStatusType](./literals.md#imageextractionstatustype)
- [IndexStatusType](./literals.md#indexstatustype)
- [IndexTypeType](./literals.md#indextypetype)
- [ListApplicationsPaginatorName](./literals.md#listapplicationspaginatorname)
- [ListAttachmentsPaginatorName](./literals.md#listattachmentspaginatorname)
- [ListConversationsPaginatorName](./literals.md#listconversationspaginatorname)
- [ListDataAccessorsPaginatorName](./literals.md#listdataaccessorspaginatorname)
- [ListDataSourceSyncJobsPaginatorName](./literals.md#listdatasourcesyncjobspaginatorname)
- [ListDataSourcesPaginatorName](./literals.md#listdatasourcespaginatorname)
- [ListDocumentsPaginatorName](./literals.md#listdocumentspaginatorname)
- [ListGroupsPaginatorName](./literals.md#listgroupspaginatorname)
- [ListIndicesPaginatorName](./literals.md#listindicespaginatorname)
- [ListMessagesPaginatorName](./literals.md#listmessagespaginatorname)
- [ListPluginActionsPaginatorName](./literals.md#listpluginactionspaginatorname)
- [ListPluginTypeActionsPaginatorName](./literals.md#listplugintypeactionspaginatorname)
- [ListPluginTypeMetadataPaginatorName](./literals.md#listplugintypemetadatapaginatorname)
- [ListPluginsPaginatorName](./literals.md#listpluginspaginatorname)
- [ListRetrieversPaginatorName](./literals.md#listretrieverspaginatorname)
- [ListSubscriptionsPaginatorName](./literals.md#listsubscriptionspaginatorname)
- [ListWebExperiencesPaginatorName](./literals.md#listwebexperiencespaginatorname)
- [MemberRelationType](./literals.md#memberrelationtype)
- [MembershipTypeType](./literals.md#membershiptypetype)
- [MessageTypeType](./literals.md#messagetypetype)
- [MessageUsefulnessReasonType](./literals.md#messageusefulnessreasontype)
- [MessageUsefulnessType](./literals.md#messageusefulnesstype)
- [NumberAttributeBoostingTypeType](./literals.md#numberattributeboostingtypetype)
- [OrchestrationControlType](./literals.md#orchestrationcontroltype)
- [PersonalizationControlModeType](./literals.md#personalizationcontrolmodetype)
- [PluginBuildStatusType](./literals.md#pluginbuildstatustype)
- [PluginStateType](./literals.md#pluginstatetype)
- [PluginTypeCategoryType](./literals.md#plugintypecategorytype)
- [PluginTypeType](./literals.md#plugintypetype)
- [QAppsControlModeType](./literals.md#qappscontrolmodetype)
- [ReadAccessTypeType](./literals.md#readaccesstypetype)
- [ResponseScopeType](./literals.md#responsescopetype)
- [RetrieverStatusType](./literals.md#retrieverstatustype)
- [RetrieverTypeType](./literals.md#retrievertypetype)
- [RuleTypeType](./literals.md#ruletypetype)
- [ScoreConfidenceType](./literals.md#scoreconfidencetype)
- [SearchRelevantContentPaginatorName](./literals.md#searchrelevantcontentpaginatorname)
- [StatusType](./literals.md#statustype)
- [StringAttributeValueBoostingLevelType](./literals.md#stringattributevalueboostingleveltype)
- [SubscriptionTypeType](./literals.md#subscriptiontypetype)
- [WebExperienceSamplePromptsControlModeType](./literals.md#webexperiencesamplepromptscontrolmodetype)
- [WebExperienceStatusType](./literals.md#webexperiencestatustype)
- [QBusinessServiceName](./literals.md#qbusinessservicename)
- [ServiceName](./literals.md#servicename)
- [ResourceServiceName](./literals.md#resourceservicename)
- [PaginatorName](./literals.md#paginatorname)
- [RegionName](./literals.md#regionname)




## Type definitions

Type annotations for [type definitions](./type_defs.md) used in methods and schema.

- [S3TypeDef](./type_defs.md#s3typedef)
- [ActionExecutionPayloadFieldOutputTypeDef](./type_defs.md#actionexecutionpayloadfieldoutputtypedef)
- [ActionExecutionPayloadFieldTypeDef](./type_defs.md#actionexecutionpayloadfieldtypedef)
- [ActionReviewPayloadFieldAllowedValueTypeDef](./type_defs.md#actionreviewpayloadfieldallowedvaluetypedef)
- [ActionSummaryTypeDef](./type_defs.md#actionsummarytypedef)
- [QuickSightConfigurationTypeDef](./type_defs.md#quicksightconfigurationtypedef)
- [AppliedAttachmentsConfigurationTypeDef](./type_defs.md#appliedattachmentsconfigurationtypedef)
- [AppliedCreatorModeConfigurationTypeDef](./type_defs.md#appliedcreatormodeconfigurationtypedef)
- [AppliedOrchestrationConfigurationTypeDef](./type_defs.md#appliedorchestrationconfigurationtypedef)
- [AssociatePermissionRequestTypeDef](./type_defs.md#associatepermissionrequesttypedef)
- [ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef)
- [BlobTypeDef](./type_defs.md#blobtypedef)
- [ErrorDetailTypeDef](./type_defs.md#errordetailtypedef)
- [AttachmentsConfigurationTypeDef](./type_defs.md#attachmentsconfigurationtypedef)
- [AuthChallengeRequestEventTypeDef](./type_defs.md#authchallengerequesteventtypedef)
- [AuthChallengeRequestTypeDef](./type_defs.md#authchallengerequesttypedef)
- [AuthChallengeResponseEventTypeDef](./type_defs.md#authchallengeresponseeventtypedef)
- [AuthChallengeResponseTypeDef](./type_defs.md#authchallengeresponsetypedef)
- [AutoSubscriptionConfigurationTypeDef](./type_defs.md#autosubscriptionconfigurationtypedef)
- [BasicAuthConfigurationTypeDef](./type_defs.md#basicauthconfigurationtypedef)
- [DeleteDocumentTypeDef](./type_defs.md#deletedocumenttypedef)
- [BlockedPhrasesConfigurationTypeDef](./type_defs.md#blockedphrasesconfigurationtypedef)
- [BlockedPhrasesConfigurationUpdateTypeDef](./type_defs.md#blockedphrasesconfigurationupdatetypedef)
- [BrowserExtensionConfigurationOutputTypeDef](./type_defs.md#browserextensionconfigurationoutputtypedef)
- [BrowserExtensionConfigurationTypeDef](./type_defs.md#browserextensionconfigurationtypedef)
- [CancelSubscriptionRequestTypeDef](./type_defs.md#cancelsubscriptionrequesttypedef)
- [SubscriptionDetailsTypeDef](./type_defs.md#subscriptiondetailstypedef)
- [TextInputEventTypeDef](./type_defs.md#textinputeventtypedef)
- [PluginConfigurationTypeDef](./type_defs.md#pluginconfigurationtypedef)
- [TextOutputEventTypeDef](./type_defs.md#textoutputeventtypedef)
- [ContentBlockerRuleTypeDef](./type_defs.md#contentblockerruletypedef)
- [EligibleDataSourceTypeDef](./type_defs.md#eligibledatasourcetypedef)
- [RetrieverContentSourceTypeDef](./type_defs.md#retrievercontentsourcetypedef)
- [ConversationSourceTypeDef](./type_defs.md#conversationsourcetypedef)
- [ConversationTypeDef](./type_defs.md#conversationtypedef)
- [EncryptionConfigurationTypeDef](./type_defs.md#encryptionconfigurationtypedef)
- [PersonalizationConfigurationTypeDef](./type_defs.md#personalizationconfigurationtypedef)
- [QAppsConfigurationTypeDef](./type_defs.md#qappsconfigurationtypedef)
- [TagTypeDef](./type_defs.md#tagtypedef)
- [IndexCapacityConfigurationTypeDef](./type_defs.md#indexcapacityconfigurationtypedef)
- [SubscriptionPrincipalTypeDef](./type_defs.md#subscriptionprincipaltypedef)
- [UserAliasTypeDef](./type_defs.md#useraliastypedef)
- [CustomizationConfigurationTypeDef](./type_defs.md#customizationconfigurationtypedef)
- [CreatorModeConfigurationTypeDef](./type_defs.md#creatormodeconfigurationtypedef)
- [DataAccessorTypeDef](./type_defs.md#dataaccessortypedef)
- [DataSourceSyncJobMetricsTypeDef](./type_defs.md#datasourcesyncjobmetricstypedef)
- [DataSourceTypeDef](./type_defs.md#datasourcetypedef)
- [DataSourceVpcConfigurationOutputTypeDef](./type_defs.md#datasourcevpcconfigurationoutputtypedef)
- [DataSourceVpcConfigurationTypeDef](./type_defs.md#datasourcevpcconfigurationtypedef)
- [DateAttributeBoostingConfigurationTypeDef](./type_defs.md#dateattributeboostingconfigurationtypedef)
- [DeleteApplicationRequestTypeDef](./type_defs.md#deleteapplicationrequesttypedef)
- [DeleteChatControlsConfigurationRequestTypeDef](./type_defs.md#deletechatcontrolsconfigurationrequesttypedef)
- [DeleteConversationRequestTypeDef](./type_defs.md#deleteconversationrequesttypedef)
- [DeleteDataAccessorRequestTypeDef](./type_defs.md#deletedataaccessorrequesttypedef)
- [DeleteDataSourceRequestTypeDef](./type_defs.md#deletedatasourcerequesttypedef)
- [DeleteGroupRequestTypeDef](./type_defs.md#deletegrouprequesttypedef)
- [DeleteIndexRequestTypeDef](./type_defs.md#deleteindexrequesttypedef)
- [DeletePluginRequestTypeDef](./type_defs.md#deletepluginrequesttypedef)
- [DeleteRetrieverRequestTypeDef](./type_defs.md#deleteretrieverrequesttypedef)
- [DeleteUserRequestTypeDef](./type_defs.md#deleteuserrequesttypedef)
- [DeleteWebExperienceRequestTypeDef](./type_defs.md#deletewebexperiencerequesttypedef)
- [DisassociatePermissionRequestTypeDef](./type_defs.md#disassociatepermissionrequesttypedef)
- [NumberAttributeBoostingConfigurationTypeDef](./type_defs.md#numberattributeboostingconfigurationtypedef)
- [StringAttributeBoostingConfigurationOutputTypeDef](./type_defs.md#stringattributeboostingconfigurationoutputtypedef)
- [StringListAttributeBoostingConfigurationTypeDef](./type_defs.md#stringlistattributeboostingconfigurationtypedef)
- [StringAttributeBoostingConfigurationTypeDef](./type_defs.md#stringattributeboostingconfigurationtypedef)
- [DocumentAttributeValueOutputTypeDef](./type_defs.md#documentattributevalueoutputtypedef)
- [DocumentAttributeConfigurationTypeDef](./type_defs.md#documentattributeconfigurationtypedef)
- [TimestampTypeDef](./type_defs.md#timestamptypedef)
- [GetApplicationRequestTypeDef](./type_defs.md#getapplicationrequesttypedef)
- [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
- [GetChatControlsConfigurationRequestTypeDef](./type_defs.md#getchatcontrolsconfigurationrequesttypedef)
- [GetDataAccessorRequestTypeDef](./type_defs.md#getdataaccessorrequesttypedef)
- [GetDataSourceRequestTypeDef](./type_defs.md#getdatasourcerequesttypedef)
- [GetGroupRequestTypeDef](./type_defs.md#getgrouprequesttypedef)
- [GetIndexRequestTypeDef](./type_defs.md#getindexrequesttypedef)
- [GetMediaRequestTypeDef](./type_defs.md#getmediarequesttypedef)
- [GetPluginRequestTypeDef](./type_defs.md#getpluginrequesttypedef)
- [GetPolicyRequestTypeDef](./type_defs.md#getpolicyrequesttypedef)
- [GetRetrieverRequestTypeDef](./type_defs.md#getretrieverrequesttypedef)
- [GetUserRequestTypeDef](./type_defs.md#getuserrequesttypedef)
- [GetWebExperienceRequestTypeDef](./type_defs.md#getwebexperiencerequesttypedef)
- [MemberGroupTypeDef](./type_defs.md#membergrouptypedef)
- [MemberUserTypeDef](./type_defs.md#memberusertypedef)
- [GroupSummaryTypeDef](./type_defs.md#groupsummarytypedef)
- [IdcAuthConfigurationTypeDef](./type_defs.md#idcauthconfigurationtypedef)
- [OpenIDConnectProviderConfigurationTypeDef](./type_defs.md#openidconnectproviderconfigurationtypedef)
- [SamlProviderConfigurationTypeDef](./type_defs.md#samlproviderconfigurationtypedef)
- [ImageExtractionConfigurationTypeDef](./type_defs.md#imageextractionconfigurationtypedef)
- [TextDocumentStatisticsTypeDef](./type_defs.md#textdocumentstatisticstypedef)
- [IndexTypeDef](./type_defs.md#indextypedef)
- [KendraIndexConfigurationTypeDef](./type_defs.md#kendraindexconfigurationtypedef)
- [ListApplicationsRequestTypeDef](./type_defs.md#listapplicationsrequesttypedef)
- [ListAttachmentsRequestTypeDef](./type_defs.md#listattachmentsrequesttypedef)
- [ListConversationsRequestTypeDef](./type_defs.md#listconversationsrequesttypedef)
- [ListDataAccessorsRequestTypeDef](./type_defs.md#listdataaccessorsrequesttypedef)
- [ListDataSourcesRequestTypeDef](./type_defs.md#listdatasourcesrequesttypedef)
- [ListDocumentsRequestTypeDef](./type_defs.md#listdocumentsrequesttypedef)
- [ListIndicesRequestTypeDef](./type_defs.md#listindicesrequesttypedef)
- [ListMessagesRequestTypeDef](./type_defs.md#listmessagesrequesttypedef)
- [ListPluginActionsRequestTypeDef](./type_defs.md#listpluginactionsrequesttypedef)
- [ListPluginTypeActionsRequestTypeDef](./type_defs.md#listplugintypeactionsrequesttypedef)
- [ListPluginTypeMetadataRequestTypeDef](./type_defs.md#listplugintypemetadatarequesttypedef)
- [PluginTypeMetadataSummaryTypeDef](./type_defs.md#plugintypemetadatasummarytypedef)
- [ListPluginsRequestTypeDef](./type_defs.md#listpluginsrequesttypedef)
- [PluginTypeDef](./type_defs.md#plugintypedef)
- [ListRetrieversRequestTypeDef](./type_defs.md#listretrieversrequesttypedef)
- [RetrieverTypeDef](./type_defs.md#retrievertypedef)
- [ListSubscriptionsRequestTypeDef](./type_defs.md#listsubscriptionsrequesttypedef)
- [ListTagsForResourceRequestTypeDef](./type_defs.md#listtagsforresourcerequesttypedef)
- [ListWebExperiencesRequestTypeDef](./type_defs.md#listwebexperiencesrequesttypedef)
- [WebExperienceTypeDef](./type_defs.md#webexperiencetypedef)
- [OAuth2ClientCredentialConfigurationTypeDef](./type_defs.md#oauth2clientcredentialconfigurationtypedef)
- [OrchestrationConfigurationTypeDef](./type_defs.md#orchestrationconfigurationtypedef)
- [PrincipalGroupTypeDef](./type_defs.md#principalgrouptypedef)
- [PrincipalUserTypeDef](./type_defs.md#principalusertypedef)
- [ScoreAttributesTypeDef](./type_defs.md#scoreattributestypedef)
- [UsersAndGroupsOutputTypeDef](./type_defs.md#usersandgroupsoutputtypedef)
- [SamlConfigurationTypeDef](./type_defs.md#samlconfigurationtypedef)
- [SnippetExcerptTypeDef](./type_defs.md#snippetexcerpttypedef)
- [StartDataSourceSyncJobRequestTypeDef](./type_defs.md#startdatasourcesyncjobrequesttypedef)
- [StopDataSourceSyncJobRequestTypeDef](./type_defs.md#stopdatasourcesyncjobrequesttypedef)
- [UntagResourceRequestTypeDef](./type_defs.md#untagresourcerequesttypedef)
- [UpdateSubscriptionRequestTypeDef](./type_defs.md#updatesubscriptionrequesttypedef)
- [UsersAndGroupsTypeDef](./type_defs.md#usersandgroupstypedef)
- [APISchemaTypeDef](./type_defs.md#apischematypedef)
- [ActionExecutionOutputTypeDef](./type_defs.md#actionexecutionoutputtypedef)
- [ActionExecutionPayloadFieldUnionTypeDef](./type_defs.md#actionexecutionpayloadfielduniontypedef)
- [ActionExecutionTypeDef](./type_defs.md#actionexecutiontypedef)
- [ActionReviewPayloadFieldTypeDef](./type_defs.md#actionreviewpayloadfieldtypedef)
- [ApplicationTypeDef](./type_defs.md#applicationtypedef)
- [AssociatePermissionResponseTypeDef](./type_defs.md#associatepermissionresponsetypedef)
- [CreateApplicationResponseTypeDef](./type_defs.md#createapplicationresponsetypedef)
- [CreateDataAccessorResponseTypeDef](./type_defs.md#createdataaccessorresponsetypedef)
- [CreateDataSourceResponseTypeDef](./type_defs.md#createdatasourceresponsetypedef)
- [CreateIndexResponseTypeDef](./type_defs.md#createindexresponsetypedef)
- [CreatePluginResponseTypeDef](./type_defs.md#createpluginresponsetypedef)
- [CreateRetrieverResponseTypeDef](./type_defs.md#createretrieverresponsetypedef)
- [CreateWebExperienceResponseTypeDef](./type_defs.md#createwebexperienceresponsetypedef)
- [EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef)
- [GetMediaResponseTypeDef](./type_defs.md#getmediaresponsetypedef)
- [GetPolicyResponseTypeDef](./type_defs.md#getpolicyresponsetypedef)
- [ListPluginActionsResponseTypeDef](./type_defs.md#listpluginactionsresponsetypedef)
- [ListPluginTypeActionsResponseTypeDef](./type_defs.md#listplugintypeactionsresponsetypedef)
- [StartDataSourceSyncJobResponseTypeDef](./type_defs.md#startdatasourcesyncjobresponsetypedef)
- [DocumentContentTypeDef](./type_defs.md#documentcontenttypedef)
- [AttachmentOutputTypeDef](./type_defs.md#attachmentoutputtypedef)
- [DocumentDetailsTypeDef](./type_defs.md#documentdetailstypedef)
- [FailedDocumentTypeDef](./type_defs.md#faileddocumenttypedef)
- [GroupStatusDetailTypeDef](./type_defs.md#groupstatusdetailtypedef)
- [BatchDeleteDocumentRequestTypeDef](./type_defs.md#batchdeletedocumentrequesttypedef)
- [BrowserExtensionConfigurationUnionTypeDef](./type_defs.md#browserextensionconfigurationuniontypedef)
- [CancelSubscriptionResponseTypeDef](./type_defs.md#cancelsubscriptionresponsetypedef)
- [CreateSubscriptionResponseTypeDef](./type_defs.md#createsubscriptionresponsetypedef)
- [UpdateSubscriptionResponseTypeDef](./type_defs.md#updatesubscriptionresponsetypedef)
- [ChatModeConfigurationTypeDef](./type_defs.md#chatmodeconfigurationtypedef)
- [ContentRetrievalRuleOutputTypeDef](./type_defs.md#contentretrievalruleoutputtypedef)
- [ContentRetrievalRuleTypeDef](./type_defs.md#contentretrievalruletypedef)
- [ContentSourceTypeDef](./type_defs.md#contentsourcetypedef)
- [CopyFromSourceTypeDef](./type_defs.md#copyfromsourcetypedef)
- [ListConversationsResponseTypeDef](./type_defs.md#listconversationsresponsetypedef)
- [GetApplicationResponseTypeDef](./type_defs.md#getapplicationresponsetypedef)
- [UpdateApplicationRequestTypeDef](./type_defs.md#updateapplicationrequesttypedef)
- [CreateApplicationRequestTypeDef](./type_defs.md#createapplicationrequesttypedef)
- [ListTagsForResourceResponseTypeDef](./type_defs.md#listtagsforresourceresponsetypedef)
- [TagResourceRequestTypeDef](./type_defs.md#tagresourcerequesttypedef)
- [CreateIndexRequestTypeDef](./type_defs.md#createindexrequesttypedef)
- [CreateSubscriptionRequestTypeDef](./type_defs.md#createsubscriptionrequesttypedef)
- [SubscriptionTypeDef](./type_defs.md#subscriptiontypedef)
- [CreateUserRequestTypeDef](./type_defs.md#createuserrequesttypedef)
- [GetUserResponseTypeDef](./type_defs.md#getuserresponsetypedef)
- [UpdateUserRequestTypeDef](./type_defs.md#updateuserrequesttypedef)
- [UpdateUserResponseTypeDef](./type_defs.md#updateuserresponsetypedef)
- [ListDataAccessorsResponseTypeDef](./type_defs.md#listdataaccessorsresponsetypedef)
- [DataSourceSyncJobTypeDef](./type_defs.md#datasourcesyncjobtypedef)
- [ListDataSourcesResponseTypeDef](./type_defs.md#listdatasourcesresponsetypedef)
- [DataSourceVpcConfigurationUnionTypeDef](./type_defs.md#datasourcevpcconfigurationuniontypedef)
- [DocumentAttributeBoostingConfigurationOutputTypeDef](./type_defs.md#documentattributeboostingconfigurationoutputtypedef)
- [DocumentAttributeBoostingConfigurationTypeDef](./type_defs.md#documentattributeboostingconfigurationtypedef)
- [DocumentAttributeConditionOutputTypeDef](./type_defs.md#documentattributeconditionoutputtypedef)
- [DocumentAttributeOutputTypeDef](./type_defs.md#documentattributeoutputtypedef)
- [DocumentAttributeTargetOutputTypeDef](./type_defs.md#documentattributetargetoutputtypedef)
- [UpdateIndexRequestTypeDef](./type_defs.md#updateindexrequesttypedef)
- [DocumentAttributeValueTypeDef](./type_defs.md#documentattributevaluetypedef)
- [ListDataSourceSyncJobsRequestTypeDef](./type_defs.md#listdatasourcesyncjobsrequesttypedef)
- [ListGroupsRequestTypeDef](./type_defs.md#listgroupsrequesttypedef)
- [MessageUsefulnessFeedbackTypeDef](./type_defs.md#messageusefulnessfeedbacktypedef)
- [GetChatControlsConfigurationRequestPaginateTypeDef](./type_defs.md#getchatcontrolsconfigurationrequestpaginatetypedef)
- [ListApplicationsRequestPaginateTypeDef](./type_defs.md#listapplicationsrequestpaginatetypedef)
- [ListAttachmentsRequestPaginateTypeDef](./type_defs.md#listattachmentsrequestpaginatetypedef)
- [ListConversationsRequestPaginateTypeDef](./type_defs.md#listconversationsrequestpaginatetypedef)
- [ListDataAccessorsRequestPaginateTypeDef](./type_defs.md#listdataaccessorsrequestpaginatetypedef)
- [ListDataSourceSyncJobsRequestPaginateTypeDef](./type_defs.md#listdatasourcesyncjobsrequestpaginatetypedef)
- [ListDataSourcesRequestPaginateTypeDef](./type_defs.md#listdatasourcesrequestpaginatetypedef)
- [ListDocumentsRequestPaginateTypeDef](./type_defs.md#listdocumentsrequestpaginatetypedef)
- [ListGroupsRequestPaginateTypeDef](./type_defs.md#listgroupsrequestpaginatetypedef)
- [ListIndicesRequestPaginateTypeDef](./type_defs.md#listindicesrequestpaginatetypedef)
- [ListMessagesRequestPaginateTypeDef](./type_defs.md#listmessagesrequestpaginatetypedef)
- [ListPluginActionsRequestPaginateTypeDef](./type_defs.md#listpluginactionsrequestpaginatetypedef)
- [ListPluginTypeActionsRequestPaginateTypeDef](./type_defs.md#listplugintypeactionsrequestpaginatetypedef)
- [ListPluginTypeMetadataRequestPaginateTypeDef](./type_defs.md#listplugintypemetadatarequestpaginatetypedef)
- [ListPluginsRequestPaginateTypeDef](./type_defs.md#listpluginsrequestpaginatetypedef)
- [ListRetrieversRequestPaginateTypeDef](./type_defs.md#listretrieversrequestpaginatetypedef)
- [ListSubscriptionsRequestPaginateTypeDef](./type_defs.md#listsubscriptionsrequestpaginatetypedef)
- [ListWebExperiencesRequestPaginateTypeDef](./type_defs.md#listwebexperiencesrequestpaginatetypedef)
- [GroupMembersTypeDef](./type_defs.md#groupmemberstypedef)
- [ListGroupsResponseTypeDef](./type_defs.md#listgroupsresponsetypedef)
- [IdentityProviderConfigurationTypeDef](./type_defs.md#identityproviderconfigurationtypedef)
- [MediaExtractionConfigurationTypeDef](./type_defs.md#mediaextractionconfigurationtypedef)
- [IndexStatisticsTypeDef](./type_defs.md#indexstatisticstypedef)
- [ListIndicesResponseTypeDef](./type_defs.md#listindicesresponsetypedef)
- [ListPluginTypeMetadataResponseTypeDef](./type_defs.md#listplugintypemetadataresponsetypedef)
- [ListPluginsResponseTypeDef](./type_defs.md#listpluginsresponsetypedef)
- [ListRetrieversResponseTypeDef](./type_defs.md#listretrieversresponsetypedef)
- [ListWebExperiencesResponseTypeDef](./type_defs.md#listwebexperiencesresponsetypedef)
- [PluginAuthConfigurationOutputTypeDef](./type_defs.md#pluginauthconfigurationoutputtypedef)
- [PluginAuthConfigurationTypeDef](./type_defs.md#pluginauthconfigurationtypedef)
- [PrincipalTypeDef](./type_defs.md#principaltypedef)
- [WebExperienceAuthConfigurationTypeDef](./type_defs.md#webexperienceauthconfigurationtypedef)
- [TextSegmentTypeDef](./type_defs.md#textsegmenttypedef)
- [UsersAndGroupsUnionTypeDef](./type_defs.md#usersandgroupsuniontypedef)
- [CustomPluginConfigurationTypeDef](./type_defs.md#custompluginconfigurationtypedef)
- [ActionExecutionEventTypeDef](./type_defs.md#actionexecutioneventtypedef)
- [ActionExecutionUnionTypeDef](./type_defs.md#actionexecutionuniontypedef)
- [ActionReviewEventTypeDef](./type_defs.md#actionrevieweventtypedef)
- [ActionReviewTypeDef](./type_defs.md#actionreviewtypedef)
- [ListApplicationsResponseTypeDef](./type_defs.md#listapplicationsresponsetypedef)
- [FailedAttachmentEventTypeDef](./type_defs.md#failedattachmenteventtypedef)
- [ListDocumentsResponseTypeDef](./type_defs.md#listdocumentsresponsetypedef)
- [BatchDeleteDocumentResponseTypeDef](./type_defs.md#batchdeletedocumentresponsetypedef)
- [BatchPutDocumentResponseTypeDef](./type_defs.md#batchputdocumentresponsetypedef)
- [GetGroupResponseTypeDef](./type_defs.md#getgroupresponsetypedef)
- [RuleConfigurationOutputTypeDef](./type_defs.md#ruleconfigurationoutputtypedef)
- [ContentRetrievalRuleUnionTypeDef](./type_defs.md#contentretrievalruleuniontypedef)
- [AttachmentInputTypeDef](./type_defs.md#attachmentinputtypedef)
- [AttachmentTypeDef](./type_defs.md#attachmenttypedef)
- [ListSubscriptionsResponseTypeDef](./type_defs.md#listsubscriptionsresponsetypedef)
- [ListDataSourceSyncJobsResponseTypeDef](./type_defs.md#listdatasourcesyncjobsresponsetypedef)
- [NativeIndexConfigurationOutputTypeDef](./type_defs.md#nativeindexconfigurationoutputtypedef)
- [NativeIndexConfigurationTypeDef](./type_defs.md#nativeindexconfigurationtypedef)
- [HookConfigurationOutputTypeDef](./type_defs.md#hookconfigurationoutputtypedef)
- [AttributeFilterOutputTypeDef](./type_defs.md#attributefilteroutputtypedef)
- [RelevantContentTypeDef](./type_defs.md#relevantcontenttypedef)
- [InlineDocumentEnrichmentConfigurationOutputTypeDef](./type_defs.md#inlinedocumentenrichmentconfigurationoutputtypedef)
- [DocumentAttributeValueUnionTypeDef](./type_defs.md#documentattributevalueuniontypedef)
- [PutFeedbackRequestTypeDef](./type_defs.md#putfeedbackrequesttypedef)
- [PutGroupRequestTypeDef](./type_defs.md#putgrouprequesttypedef)
- [CreateWebExperienceRequestTypeDef](./type_defs.md#createwebexperiencerequesttypedef)
- [GetIndexResponseTypeDef](./type_defs.md#getindexresponsetypedef)
- [PluginAuthConfigurationUnionTypeDef](./type_defs.md#pluginauthconfigurationuniontypedef)
- [AccessControlTypeDef](./type_defs.md#accesscontroltypedef)
- [GetWebExperienceResponseTypeDef](./type_defs.md#getwebexperienceresponsetypedef)
- [UpdateWebExperienceRequestTypeDef](./type_defs.md#updatewebexperiencerequesttypedef)
- [SourceAttributionTypeDef](./type_defs.md#sourceattributiontypedef)
- [GetPluginResponseTypeDef](./type_defs.md#getpluginresponsetypedef)
- [RuleOutputTypeDef](./type_defs.md#ruleoutputtypedef)
- [RuleConfigurationTypeDef](./type_defs.md#ruleconfigurationtypedef)
- [AttachmentInputEventTypeDef](./type_defs.md#attachmentinputeventtypedef)
- [ListAttachmentsResponseTypeDef](./type_defs.md#listattachmentsresponsetypedef)
- [RetrieverConfigurationOutputTypeDef](./type_defs.md#retrieverconfigurationoutputtypedef)
- [RetrieverConfigurationTypeDef](./type_defs.md#retrieverconfigurationtypedef)
- [ActionFilterConfigurationOutputTypeDef](./type_defs.md#actionfilterconfigurationoutputtypedef)
- [SearchRelevantContentResponseTypeDef](./type_defs.md#searchrelevantcontentresponsetypedef)
- [DocumentEnrichmentConfigurationOutputTypeDef](./type_defs.md#documentenrichmentconfigurationoutputtypedef)
- [DocumentAttributeConditionTypeDef](./type_defs.md#documentattributeconditiontypedef)
- [DocumentAttributeTargetTypeDef](./type_defs.md#documentattributetargettypedef)
- [DocumentAttributeTypeDef](./type_defs.md#documentattributetypedef)
- [CreatePluginRequestTypeDef](./type_defs.md#createpluginrequesttypedef)
- [UpdatePluginRequestTypeDef](./type_defs.md#updatepluginrequesttypedef)
- [AccessConfigurationTypeDef](./type_defs.md#accessconfigurationtypedef)
- [ChatSyncOutputTypeDef](./type_defs.md#chatsyncoutputtypedef)
- [MessageTypeDef](./type_defs.md#messagetypedef)
- [MetadataEventTypeDef](./type_defs.md#metadataeventtypedef)
- [TopicConfigurationOutputTypeDef](./type_defs.md#topicconfigurationoutputtypedef)
- [RuleConfigurationUnionTypeDef](./type_defs.md#ruleconfigurationuniontypedef)
- [GetRetrieverResponseTypeDef](./type_defs.md#getretrieverresponsetypedef)
- [RetrieverConfigurationUnionTypeDef](./type_defs.md#retrieverconfigurationuniontypedef)
- [ActionConfigurationOutputTypeDef](./type_defs.md#actionconfigurationoutputtypedef)
- [GetDataSourceResponseTypeDef](./type_defs.md#getdatasourceresponsetypedef)
- [DocumentAttributeConditionUnionTypeDef](./type_defs.md#documentattributeconditionuniontypedef)
- [DocumentAttributeTargetUnionTypeDef](./type_defs.md#documentattributetargetuniontypedef)
- [DocumentAttributeUnionTypeDef](./type_defs.md#documentattributeuniontypedef)
- [ListMessagesResponseTypeDef](./type_defs.md#listmessagesresponsetypedef)
- [ChatOutputStreamTypeDef](./type_defs.md#chatoutputstreamtypedef)
- [GetChatControlsConfigurationResponseTypeDef](./type_defs.md#getchatcontrolsconfigurationresponsetypedef)
- [RuleTypeDef](./type_defs.md#ruletypedef)
- [CreateRetrieverRequestTypeDef](./type_defs.md#createretrieverrequesttypedef)
- [UpdateRetrieverRequestTypeDef](./type_defs.md#updateretrieverrequesttypedef)
- [GetDataAccessorResponseTypeDef](./type_defs.md#getdataaccessorresponsetypedef)
- [HookConfigurationTypeDef](./type_defs.md#hookconfigurationtypedef)
- [InlineDocumentEnrichmentConfigurationTypeDef](./type_defs.md#inlinedocumentenrichmentconfigurationtypedef)
- [AttributeFilterPaginatorTypeDef](./type_defs.md#attributefilterpaginatortypedef)
- [AttributeFilterTypeDef](./type_defs.md#attributefiltertypedef)
- [ChatOutputTypeDef](./type_defs.md#chatoutputtypedef)
- [RuleUnionTypeDef](./type_defs.md#ruleuniontypedef)
- [HookConfigurationUnionTypeDef](./type_defs.md#hookconfigurationuniontypedef)
- [InlineDocumentEnrichmentConfigurationUnionTypeDef](./type_defs.md#inlinedocumentenrichmentconfigurationuniontypedef)
- [SearchRelevantContentRequestPaginateTypeDef](./type_defs.md#searchrelevantcontentrequestpaginatetypedef)
- [AttributeFilterUnionTypeDef](./type_defs.md#attributefilteruniontypedef)
- [TopicConfigurationTypeDef](./type_defs.md#topicconfigurationtypedef)
- [DocumentEnrichmentConfigurationTypeDef](./type_defs.md#documentenrichmentconfigurationtypedef)
- [ActionFilterConfigurationTypeDef](./type_defs.md#actionfilterconfigurationtypedef)
- [ChatSyncInputTypeDef](./type_defs.md#chatsyncinputtypedef)
- [ConfigurationEventTypeDef](./type_defs.md#configurationeventtypedef)
- [SearchRelevantContentRequestTypeDef](./type_defs.md#searchrelevantcontentrequesttypedef)
- [TopicConfigurationUnionTypeDef](./type_defs.md#topicconfigurationuniontypedef)
- [DocumentEnrichmentConfigurationUnionTypeDef](./type_defs.md#documentenrichmentconfigurationuniontypedef)
- [ActionFilterConfigurationUnionTypeDef](./type_defs.md#actionfilterconfigurationuniontypedef)
- [ChatInputStreamTypeDef](./type_defs.md#chatinputstreamtypedef)
- [UpdateChatControlsConfigurationRequestTypeDef](./type_defs.md#updatechatcontrolsconfigurationrequesttypedef)
- [CreateDataSourceRequestTypeDef](./type_defs.md#createdatasourcerequesttypedef)
- [DocumentTypeDef](./type_defs.md#documenttypedef)
- [UpdateDataSourceRequestTypeDef](./type_defs.md#updatedatasourcerequesttypedef)
- [ActionConfigurationTypeDef](./type_defs.md#actionconfigurationtypedef)
- [ChatInputTypeDef](./type_defs.md#chatinputtypedef)
- [BatchPutDocumentRequestTypeDef](./type_defs.md#batchputdocumentrequesttypedef)
- [ActionConfigurationUnionTypeDef](./type_defs.md#actionconfigurationuniontypedef)
- [CreateDataAccessorRequestTypeDef](./type_defs.md#createdataaccessorrequesttypedef)
- [UpdateDataAccessorRequestTypeDef](./type_defs.md#updatedataaccessorrequesttypedef)

