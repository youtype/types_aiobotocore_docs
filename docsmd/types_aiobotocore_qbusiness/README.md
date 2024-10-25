# QBusiness module

> [Index](../README.md) > QBusiness


!!! note ""

    Auto-generated documentation for [QBusiness](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/qbusiness.html#QBusiness)
    type annotations stubs module [types-aiobotocore-qbusiness](https://pypi.org/project/types-aiobotocore-qbusiness/).

## How to install



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
- [ListConversationsPaginator](./paginators.md#listconversationspaginator)
- [ListDataSourceSyncJobsPaginator](./paginators.md#listdatasourcesyncjobspaginator)
- [ListDataSourcesPaginator](./paginators.md#listdatasourcespaginator)
- [ListDocumentsPaginator](./paginators.md#listdocumentspaginator)
- [ListGroupsPaginator](./paginators.md#listgroupspaginator)
- [ListIndicesPaginator](./paginators.md#listindicespaginator)
- [ListMessagesPaginator](./paginators.md#listmessagespaginator)
- [ListPluginsPaginator](./paginators.md#listpluginspaginator)
- [ListRetrieversPaginator](./paginators.md#listretrieverspaginator)
- [ListWebExperiencesPaginator](./paginators.md#listwebexperiencespaginator)








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
- [IndexStatusType](./literals.md#indexstatustype)
- [IndexTypeType](./literals.md#indextypetype)
- [ListApplicationsPaginatorName](./literals.md#listapplicationspaginatorname)
- [ListConversationsPaginatorName](./literals.md#listconversationspaginatorname)
- [ListDataSourceSyncJobsPaginatorName](./literals.md#listdatasourcesyncjobspaginatorname)
- [ListDataSourcesPaginatorName](./literals.md#listdatasourcespaginatorname)
- [ListDocumentsPaginatorName](./literals.md#listdocumentspaginatorname)
- [ListGroupsPaginatorName](./literals.md#listgroupspaginatorname)
- [ListIndicesPaginatorName](./literals.md#listindicespaginatorname)
- [ListMessagesPaginatorName](./literals.md#listmessagespaginatorname)
- [ListPluginsPaginatorName](./literals.md#listpluginspaginatorname)
- [ListRetrieversPaginatorName](./literals.md#listretrieverspaginatorname)
- [ListWebExperiencesPaginatorName](./literals.md#listwebexperiencespaginatorname)
- [MemberRelationType](./literals.md#memberrelationtype)
- [MembershipTypeType](./literals.md#membershiptypetype)
- [MessageTypeType](./literals.md#messagetypetype)
- [MessageUsefulnessReasonType](./literals.md#messageusefulnessreasontype)
- [MessageUsefulnessType](./literals.md#messageusefulnesstype)
- [NumberAttributeBoostingTypeType](./literals.md#numberattributeboostingtypetype)
- [PersonalizationControlModeType](./literals.md#personalizationcontrolmodetype)
- [PluginBuildStatusType](./literals.md#pluginbuildstatustype)
- [PluginStateType](./literals.md#pluginstatetype)
- [PluginTypeType](./literals.md#plugintypetype)
- [QAppsControlModeType](./literals.md#qappscontrolmodetype)
- [ReadAccessTypeType](./literals.md#readaccesstypetype)
- [ResponseScopeType](./literals.md#responsescopetype)
- [RetrieverStatusType](./literals.md#retrieverstatustype)
- [RetrieverTypeType](./literals.md#retrievertypetype)
- [RuleTypeType](./literals.md#ruletypetype)
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
- [ApplicationTypeDef](./type_defs.md#applicationtypedef)
- [AppliedAttachmentsConfigurationTypeDef](./type_defs.md#appliedattachmentsconfigurationtypedef)
- [AppliedCreatorModeConfigurationTypeDef](./type_defs.md#appliedcreatormodeconfigurationtypedef)
- [BlobTypeDef](./type_defs.md#blobtypedef)
- [ErrorDetailTypeDef](./type_defs.md#errordetailtypedef)
- [AttachmentsConfigurationTypeDef](./type_defs.md#attachmentsconfigurationtypedef)
- [AuthChallengeRequestTypeDef](./type_defs.md#authchallengerequesttypedef)
- [AuthChallengeResponseTypeDef](./type_defs.md#authchallengeresponsetypedef)
- [AutoSubscriptionConfigurationTypeDef](./type_defs.md#autosubscriptionconfigurationtypedef)
- [BasicAuthConfigurationTypeDef](./type_defs.md#basicauthconfigurationtypedef)
- [DeleteDocumentTypeDef](./type_defs.md#deletedocumenttypedef)
- [ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef)
- [BlockedPhrasesConfigurationTypeDef](./type_defs.md#blockedphrasesconfigurationtypedef)
- [BlockedPhrasesConfigurationUpdateTypeDef](./type_defs.md#blockedphrasesconfigurationupdatetypedef)
- [PluginConfigurationTypeDef](./type_defs.md#pluginconfigurationtypedef)
- [ContentBlockerRuleTypeDef](./type_defs.md#contentblockerruletypedef)
- [EligibleDataSourceTypeDef](./type_defs.md#eligibledatasourcetypedef)
- [ConversationTypeDef](./type_defs.md#conversationtypedef)
- [EncryptionConfigurationTypeDef](./type_defs.md#encryptionconfigurationtypedef)
- [PersonalizationConfigurationTypeDef](./type_defs.md#personalizationconfigurationtypedef)
- [QAppsConfigurationTypeDef](./type_defs.md#qappsconfigurationtypedef)
- [TagTypeDef](./type_defs.md#tagtypedef)
- [DataSourceVpcConfigurationTypeDef](./type_defs.md#datasourcevpcconfigurationtypedef)
- [IndexCapacityConfigurationTypeDef](./type_defs.md#indexcapacityconfigurationtypedef)
- [UserAliasTypeDef](./type_defs.md#useraliastypedef)
- [CreatorModeConfigurationTypeDef](./type_defs.md#creatormodeconfigurationtypedef)
- [DataSourceSyncJobMetricsTypeDef](./type_defs.md#datasourcesyncjobmetricstypedef)
- [DataSourceTypeDef](./type_defs.md#datasourcetypedef)
- [DataSourceVpcConfigurationOutputTypeDef](./type_defs.md#datasourcevpcconfigurationoutputtypedef)
- [DateAttributeBoostingConfigurationTypeDef](./type_defs.md#dateattributeboostingconfigurationtypedef)
- [DeleteApplicationRequestRequestTypeDef](./type_defs.md#deleteapplicationrequestrequesttypedef)
- [DeleteChatControlsConfigurationRequestRequestTypeDef](./type_defs.md#deletechatcontrolsconfigurationrequestrequesttypedef)
- [DeleteConversationRequestRequestTypeDef](./type_defs.md#deleteconversationrequestrequesttypedef)
- [DeleteDataSourceRequestRequestTypeDef](./type_defs.md#deletedatasourcerequestrequesttypedef)
- [DeleteGroupRequestRequestTypeDef](./type_defs.md#deletegrouprequestrequesttypedef)
- [DeleteIndexRequestRequestTypeDef](./type_defs.md#deleteindexrequestrequesttypedef)
- [DeletePluginRequestRequestTypeDef](./type_defs.md#deletepluginrequestrequesttypedef)
- [DeleteRetrieverRequestRequestTypeDef](./type_defs.md#deleteretrieverrequestrequesttypedef)
- [DeleteUserRequestRequestTypeDef](./type_defs.md#deleteuserrequestrequesttypedef)
- [DeleteWebExperienceRequestRequestTypeDef](./type_defs.md#deletewebexperiencerequestrequesttypedef)
- [NumberAttributeBoostingConfigurationTypeDef](./type_defs.md#numberattributeboostingconfigurationtypedef)
- [StringAttributeBoostingConfigurationOutputTypeDef](./type_defs.md#stringattributeboostingconfigurationoutputtypedef)
- [StringListAttributeBoostingConfigurationTypeDef](./type_defs.md#stringlistattributeboostingconfigurationtypedef)
- [DocumentAttributeValueOutputTypeDef](./type_defs.md#documentattributevalueoutputtypedef)
- [DocumentAttributeConfigurationTypeDef](./type_defs.md#documentattributeconfigurationtypedef)
- [TimestampTypeDef](./type_defs.md#timestamptypedef)
- [GetApplicationRequestRequestTypeDef](./type_defs.md#getapplicationrequestrequesttypedef)
- [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
- [GetChatControlsConfigurationRequestRequestTypeDef](./type_defs.md#getchatcontrolsconfigurationrequestrequesttypedef)
- [GetDataSourceRequestRequestTypeDef](./type_defs.md#getdatasourcerequestrequesttypedef)
- [GetGroupRequestRequestTypeDef](./type_defs.md#getgrouprequestrequesttypedef)
- [GetIndexRequestRequestTypeDef](./type_defs.md#getindexrequestrequesttypedef)
- [GetPluginRequestRequestTypeDef](./type_defs.md#getpluginrequestrequesttypedef)
- [GetRetrieverRequestRequestTypeDef](./type_defs.md#getretrieverrequestrequesttypedef)
- [GetUserRequestRequestTypeDef](./type_defs.md#getuserrequestrequesttypedef)
- [GetWebExperienceRequestRequestTypeDef](./type_defs.md#getwebexperiencerequestrequesttypedef)
- [MemberGroupTypeDef](./type_defs.md#membergrouptypedef)
- [MemberUserTypeDef](./type_defs.md#memberusertypedef)
- [GroupSummaryTypeDef](./type_defs.md#groupsummarytypedef)
- [OpenIDConnectProviderConfigurationTypeDef](./type_defs.md#openidconnectproviderconfigurationtypedef)
- [SamlProviderConfigurationTypeDef](./type_defs.md#samlproviderconfigurationtypedef)
- [TextDocumentStatisticsTypeDef](./type_defs.md#textdocumentstatisticstypedef)
- [IndexTypeDef](./type_defs.md#indextypedef)
- [KendraIndexConfigurationTypeDef](./type_defs.md#kendraindexconfigurationtypedef)
- [ListApplicationsRequestRequestTypeDef](./type_defs.md#listapplicationsrequestrequesttypedef)
- [ListConversationsRequestRequestTypeDef](./type_defs.md#listconversationsrequestrequesttypedef)
- [ListDataSourcesRequestRequestTypeDef](./type_defs.md#listdatasourcesrequestrequesttypedef)
- [ListDocumentsRequestRequestTypeDef](./type_defs.md#listdocumentsrequestrequesttypedef)
- [ListIndicesRequestRequestTypeDef](./type_defs.md#listindicesrequestrequesttypedef)
- [ListMessagesRequestRequestTypeDef](./type_defs.md#listmessagesrequestrequesttypedef)
- [ListPluginsRequestRequestTypeDef](./type_defs.md#listpluginsrequestrequesttypedef)
- [PluginTypeDef](./type_defs.md#plugintypedef)
- [ListRetrieversRequestRequestTypeDef](./type_defs.md#listretrieversrequestrequesttypedef)
- [RetrieverTypeDef](./type_defs.md#retrievertypedef)
- [ListTagsForResourceRequestRequestTypeDef](./type_defs.md#listtagsforresourcerequestrequesttypedef)
- [ListWebExperiencesRequestRequestTypeDef](./type_defs.md#listwebexperiencesrequestrequesttypedef)
- [WebExperienceTypeDef](./type_defs.md#webexperiencetypedef)
- [OAuth2ClientCredentialConfigurationTypeDef](./type_defs.md#oauth2clientcredentialconfigurationtypedef)
- [PrincipalGroupTypeDef](./type_defs.md#principalgrouptypedef)
- [PrincipalUserTypeDef](./type_defs.md#principalusertypedef)
- [UsersAndGroupsOutputTypeDef](./type_defs.md#usersandgroupsoutputtypedef)
- [SamlConfigurationTypeDef](./type_defs.md#samlconfigurationtypedef)
- [SnippetExcerptTypeDef](./type_defs.md#snippetexcerpttypedef)
- [StartDataSourceSyncJobRequestRequestTypeDef](./type_defs.md#startdatasourcesyncjobrequestrequesttypedef)
- [StopDataSourceSyncJobRequestRequestTypeDef](./type_defs.md#stopdatasourcesyncjobrequestrequesttypedef)
- [StringAttributeBoostingConfigurationTypeDef](./type_defs.md#stringattributeboostingconfigurationtypedef)
- [UntagResourceRequestRequestTypeDef](./type_defs.md#untagresourcerequestrequesttypedef)
- [UsersAndGroupsTypeDef](./type_defs.md#usersandgroupstypedef)
- [APISchemaTypeDef](./type_defs.md#apischematypedef)
- [ActionExecutionOutputTypeDef](./type_defs.md#actionexecutionoutputtypedef)
- [ActionExecutionPayloadFieldUnionTypeDef](./type_defs.md#actionexecutionpayloadfielduniontypedef)
- [ActionReviewPayloadFieldTypeDef](./type_defs.md#actionreviewpayloadfieldtypedef)
- [AttachmentInputTypeDef](./type_defs.md#attachmentinputtypedef)
- [DocumentContentTypeDef](./type_defs.md#documentcontenttypedef)
- [AttachmentOutputTypeDef](./type_defs.md#attachmentoutputtypedef)
- [DocumentDetailsTypeDef](./type_defs.md#documentdetailstypedef)
- [FailedDocumentTypeDef](./type_defs.md#faileddocumenttypedef)
- [GroupStatusDetailTypeDef](./type_defs.md#groupstatusdetailtypedef)
- [BatchDeleteDocumentRequestRequestTypeDef](./type_defs.md#batchdeletedocumentrequestrequesttypedef)
- [CreateApplicationResponseTypeDef](./type_defs.md#createapplicationresponsetypedef)
- [CreateDataSourceResponseTypeDef](./type_defs.md#createdatasourceresponsetypedef)
- [CreateIndexResponseTypeDef](./type_defs.md#createindexresponsetypedef)
- [CreatePluginResponseTypeDef](./type_defs.md#createpluginresponsetypedef)
- [CreateRetrieverResponseTypeDef](./type_defs.md#createretrieverresponsetypedef)
- [CreateWebExperienceResponseTypeDef](./type_defs.md#createwebexperienceresponsetypedef)
- [EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef)
- [ListApplicationsResponseTypeDef](./type_defs.md#listapplicationsresponsetypedef)
- [StartDataSourceSyncJobResponseTypeDef](./type_defs.md#startdatasourcesyncjobresponsetypedef)
- [ChatModeConfigurationTypeDef](./type_defs.md#chatmodeconfigurationtypedef)
- [ContentRetrievalRuleOutputTypeDef](./type_defs.md#contentretrievalruleoutputtypedef)
- [ContentRetrievalRuleTypeDef](./type_defs.md#contentretrievalruletypedef)
- [ListConversationsResponseTypeDef](./type_defs.md#listconversationsresponsetypedef)
- [GetApplicationResponseTypeDef](./type_defs.md#getapplicationresponsetypedef)
- [UpdateApplicationRequestRequestTypeDef](./type_defs.md#updateapplicationrequestrequesttypedef)
- [CreateApplicationRequestRequestTypeDef](./type_defs.md#createapplicationrequestrequesttypedef)
- [ListTagsForResourceResponseTypeDef](./type_defs.md#listtagsforresourceresponsetypedef)
- [TagResourceRequestRequestTypeDef](./type_defs.md#tagresourcerequestrequesttypedef)
- [CreateIndexRequestRequestTypeDef](./type_defs.md#createindexrequestrequesttypedef)
- [CreateUserRequestRequestTypeDef](./type_defs.md#createuserrequestrequesttypedef)
- [GetUserResponseTypeDef](./type_defs.md#getuserresponsetypedef)
- [UpdateUserRequestRequestTypeDef](./type_defs.md#updateuserrequestrequesttypedef)
- [UpdateUserResponseTypeDef](./type_defs.md#updateuserresponsetypedef)
- [DataSourceSyncJobTypeDef](./type_defs.md#datasourcesyncjobtypedef)
- [ListDataSourcesResponseTypeDef](./type_defs.md#listdatasourcesresponsetypedef)
- [DocumentAttributeBoostingConfigurationOutputTypeDef](./type_defs.md#documentattributeboostingconfigurationoutputtypedef)
- [DocumentAttributeConditionOutputTypeDef](./type_defs.md#documentattributeconditionoutputtypedef)
- [DocumentAttributeTargetOutputTypeDef](./type_defs.md#documentattributetargetoutputtypedef)
- [UpdateIndexRequestRequestTypeDef](./type_defs.md#updateindexrequestrequesttypedef)
- [DocumentAttributeValueTypeDef](./type_defs.md#documentattributevaluetypedef)
- [ListDataSourceSyncJobsRequestRequestTypeDef](./type_defs.md#listdatasourcesyncjobsrequestrequesttypedef)
- [ListGroupsRequestRequestTypeDef](./type_defs.md#listgroupsrequestrequesttypedef)
- [MessageUsefulnessFeedbackTypeDef](./type_defs.md#messageusefulnessfeedbacktypedef)
- [GetChatControlsConfigurationRequestGetChatControlsConfigurationPaginateTypeDef](./type_defs.md#getchatcontrolsconfigurationrequestgetchatcontrolsconfigurationpaginatetypedef)
- [ListApplicationsRequestListApplicationsPaginateTypeDef](./type_defs.md#listapplicationsrequestlistapplicationspaginatetypedef)
- [ListConversationsRequestListConversationsPaginateTypeDef](./type_defs.md#listconversationsrequestlistconversationspaginatetypedef)
- [ListDataSourceSyncJobsRequestListDataSourceSyncJobsPaginateTypeDef](./type_defs.md#listdatasourcesyncjobsrequestlistdatasourcesyncjobspaginatetypedef)
- [ListDataSourcesRequestListDataSourcesPaginateTypeDef](./type_defs.md#listdatasourcesrequestlistdatasourcespaginatetypedef)
- [ListDocumentsRequestListDocumentsPaginateTypeDef](./type_defs.md#listdocumentsrequestlistdocumentspaginatetypedef)
- [ListGroupsRequestListGroupsPaginateTypeDef](./type_defs.md#listgroupsrequestlistgroupspaginatetypedef)
- [ListIndicesRequestListIndicesPaginateTypeDef](./type_defs.md#listindicesrequestlistindicespaginatetypedef)
- [ListMessagesRequestListMessagesPaginateTypeDef](./type_defs.md#listmessagesrequestlistmessagespaginatetypedef)
- [ListPluginsRequestListPluginsPaginateTypeDef](./type_defs.md#listpluginsrequestlistpluginspaginatetypedef)
- [ListRetrieversRequestListRetrieversPaginateTypeDef](./type_defs.md#listretrieversrequestlistretrieverspaginatetypedef)
- [ListWebExperiencesRequestListWebExperiencesPaginateTypeDef](./type_defs.md#listwebexperiencesrequestlistwebexperiencespaginatetypedef)
- [GroupMembersTypeDef](./type_defs.md#groupmemberstypedef)
- [ListGroupsResponseTypeDef](./type_defs.md#listgroupsresponsetypedef)
- [IdentityProviderConfigurationTypeDef](./type_defs.md#identityproviderconfigurationtypedef)
- [IndexStatisticsTypeDef](./type_defs.md#indexstatisticstypedef)
- [ListIndicesResponseTypeDef](./type_defs.md#listindicesresponsetypedef)
- [ListPluginsResponseTypeDef](./type_defs.md#listpluginsresponsetypedef)
- [ListRetrieversResponseTypeDef](./type_defs.md#listretrieversresponsetypedef)
- [ListWebExperiencesResponseTypeDef](./type_defs.md#listwebexperiencesresponsetypedef)
- [PluginAuthConfigurationOutputTypeDef](./type_defs.md#pluginauthconfigurationoutputtypedef)
- [PluginAuthConfigurationTypeDef](./type_defs.md#pluginauthconfigurationtypedef)
- [PrincipalTypeDef](./type_defs.md#principaltypedef)
- [WebExperienceAuthConfigurationTypeDef](./type_defs.md#webexperienceauthconfigurationtypedef)
- [TextSegmentTypeDef](./type_defs.md#textsegmenttypedef)
- [StringAttributeBoostingConfigurationUnionTypeDef](./type_defs.md#stringattributeboostingconfigurationuniontypedef)
- [UsersAndGroupsUnionTypeDef](./type_defs.md#usersandgroupsuniontypedef)
- [CustomPluginConfigurationTypeDef](./type_defs.md#custompluginconfigurationtypedef)
- [ActionExecutionTypeDef](./type_defs.md#actionexecutiontypedef)
- [ActionReviewTypeDef](./type_defs.md#actionreviewtypedef)
- [ListDocumentsResponseTypeDef](./type_defs.md#listdocumentsresponsetypedef)
- [BatchDeleteDocumentResponseTypeDef](./type_defs.md#batchdeletedocumentresponsetypedef)
- [BatchPutDocumentResponseTypeDef](./type_defs.md#batchputdocumentresponsetypedef)
- [GetGroupResponseTypeDef](./type_defs.md#getgroupresponsetypedef)
- [RuleConfigurationOutputTypeDef](./type_defs.md#ruleconfigurationoutputtypedef)
- [ContentRetrievalRuleUnionTypeDef](./type_defs.md#contentretrievalruleuniontypedef)
- [ListDataSourceSyncJobsResponseTypeDef](./type_defs.md#listdatasourcesyncjobsresponsetypedef)
- [NativeIndexConfigurationOutputTypeDef](./type_defs.md#nativeindexconfigurationoutputtypedef)
- [HookConfigurationOutputTypeDef](./type_defs.md#hookconfigurationoutputtypedef)
- [InlineDocumentEnrichmentConfigurationOutputTypeDef](./type_defs.md#inlinedocumentenrichmentconfigurationoutputtypedef)
- [DocumentAttributeValueUnionTypeDef](./type_defs.md#documentattributevalueuniontypedef)
- [PutFeedbackRequestRequestTypeDef](./type_defs.md#putfeedbackrequestrequesttypedef)
- [PutGroupRequestRequestTypeDef](./type_defs.md#putgrouprequestrequesttypedef)
- [CreateWebExperienceRequestRequestTypeDef](./type_defs.md#createwebexperiencerequestrequesttypedef)
- [GetIndexResponseTypeDef](./type_defs.md#getindexresponsetypedef)
- [AccessControlTypeDef](./type_defs.md#accesscontroltypedef)
- [GetWebExperienceResponseTypeDef](./type_defs.md#getwebexperienceresponsetypedef)
- [UpdateWebExperienceRequestRequestTypeDef](./type_defs.md#updatewebexperiencerequestrequesttypedef)
- [SourceAttributionTypeDef](./type_defs.md#sourceattributiontypedef)
- [DocumentAttributeBoostingConfigurationTypeDef](./type_defs.md#documentattributeboostingconfigurationtypedef)
- [CreatePluginRequestRequestTypeDef](./type_defs.md#createpluginrequestrequesttypedef)
- [GetPluginResponseTypeDef](./type_defs.md#getpluginresponsetypedef)
- [UpdatePluginRequestRequestTypeDef](./type_defs.md#updatepluginrequestrequesttypedef)
- [RuleOutputTypeDef](./type_defs.md#ruleoutputtypedef)
- [RuleConfigurationTypeDef](./type_defs.md#ruleconfigurationtypedef)
- [RetrieverConfigurationOutputTypeDef](./type_defs.md#retrieverconfigurationoutputtypedef)
- [DocumentEnrichmentConfigurationOutputTypeDef](./type_defs.md#documentenrichmentconfigurationoutputtypedef)
- [DocumentAttributeConditionTypeDef](./type_defs.md#documentattributeconditiontypedef)
- [DocumentAttributeTargetTypeDef](./type_defs.md#documentattributetargettypedef)
- [DocumentAttributeTypeDef](./type_defs.md#documentattributetypedef)
- [AccessConfigurationTypeDef](./type_defs.md#accessconfigurationtypedef)
- [ChatSyncOutputTypeDef](./type_defs.md#chatsyncoutputtypedef)
- [MessageTypeDef](./type_defs.md#messagetypedef)
- [DocumentAttributeBoostingConfigurationUnionTypeDef](./type_defs.md#documentattributeboostingconfigurationuniontypedef)
- [TopicConfigurationOutputTypeDef](./type_defs.md#topicconfigurationoutputtypedef)
- [RuleConfigurationUnionTypeDef](./type_defs.md#ruleconfigurationuniontypedef)
- [GetRetrieverResponseTypeDef](./type_defs.md#getretrieverresponsetypedef)
- [GetDataSourceResponseTypeDef](./type_defs.md#getdatasourceresponsetypedef)
- [DocumentAttributeConditionUnionTypeDef](./type_defs.md#documentattributeconditionuniontypedef)
- [DocumentAttributeTargetUnionTypeDef](./type_defs.md#documentattributetargetuniontypedef)
- [AttributeFilterTypeDef](./type_defs.md#attributefiltertypedef)
- [ListMessagesResponseTypeDef](./type_defs.md#listmessagesresponsetypedef)
- [NativeIndexConfigurationTypeDef](./type_defs.md#nativeindexconfigurationtypedef)
- [GetChatControlsConfigurationResponseTypeDef](./type_defs.md#getchatcontrolsconfigurationresponsetypedef)
- [RuleTypeDef](./type_defs.md#ruletypedef)
- [HookConfigurationTypeDef](./type_defs.md#hookconfigurationtypedef)
- [InlineDocumentEnrichmentConfigurationTypeDef](./type_defs.md#inlinedocumentenrichmentconfigurationtypedef)
- [ChatSyncInputRequestTypeDef](./type_defs.md#chatsyncinputrequesttypedef)
- [NativeIndexConfigurationUnionTypeDef](./type_defs.md#nativeindexconfigurationuniontypedef)
- [RuleUnionTypeDef](./type_defs.md#ruleuniontypedef)
- [HookConfigurationUnionTypeDef](./type_defs.md#hookconfigurationuniontypedef)
- [InlineDocumentEnrichmentConfigurationUnionTypeDef](./type_defs.md#inlinedocumentenrichmentconfigurationuniontypedef)
- [RetrieverConfigurationTypeDef](./type_defs.md#retrieverconfigurationtypedef)
- [TopicConfigurationTypeDef](./type_defs.md#topicconfigurationtypedef)
- [DocumentEnrichmentConfigurationTypeDef](./type_defs.md#documentenrichmentconfigurationtypedef)
- [CreateRetrieverRequestRequestTypeDef](./type_defs.md#createretrieverrequestrequesttypedef)
- [UpdateRetrieverRequestRequestTypeDef](./type_defs.md#updateretrieverrequestrequesttypedef)
- [TopicConfigurationUnionTypeDef](./type_defs.md#topicconfigurationuniontypedef)
- [CreateDataSourceRequestRequestTypeDef](./type_defs.md#createdatasourcerequestrequesttypedef)
- [DocumentEnrichmentConfigurationUnionTypeDef](./type_defs.md#documentenrichmentconfigurationuniontypedef)
- [UpdateDataSourceRequestRequestTypeDef](./type_defs.md#updatedatasourcerequestrequesttypedef)
- [UpdateChatControlsConfigurationRequestRequestTypeDef](./type_defs.md#updatechatcontrolsconfigurationrequestrequesttypedef)
- [DocumentTypeDef](./type_defs.md#documenttypedef)
- [BatchPutDocumentRequestRequestTypeDef](./type_defs.md#batchputdocumentrequestrequesttypedef)

