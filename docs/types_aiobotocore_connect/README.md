<a id="type-annotations-for-aiobotocore-connect-module"></a>

# Type annotations for aiobotocore Connect module

> [Index](../README.md) > Connect

Auto-generated documentation for
[Connect](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect)
type annotations stubs module
[types-aiobotocore-connect](https://pypi.org/project/types-aiobotocore-connect/).

- [Type annotations for aiobotocore Connect module](#type-annotations-for-aiobotocore-connect-module)
  - [How to install](#how-to-install)
    - [VSCode extension](#vscode-extension)
    - [From PyPI with pip](#from-pypi-with-pip)
  - [How to uninstall](#how-to-uninstall)
  - [Usage](#usage)
  - [ConnectClient](#connectclient)
    - [Methods](#methods)
    - [Exceptions](#exceptions)
  - [Paginators](#paginators)
  - [Literals](#literals)
  - [Typed dictionaries](#typed-dictionaries)

<a id="how-to-install"></a>

## How to install

<a id="vscode-extension"></a>

### VSCode extension

Add
[AWS Boto3](https://marketplace.visualstudio.com/items?itemName=Boto3typed.boto3-ide)
extension to your VSCode and run `AWS boto3: Quick Start` command.

Click `Modify` and select `boto3 common` and `Connect`.

<a id="from-pypi-with-pip"></a>

### From PyPI with pip

Install `types-aiobotocore` for `Connect` service.

```bash
# install with aiobotocore type annotations
python -m pip install 'types-aiobotocore[connect]'


# Lite version does not provide session.client/resource overloads
# it is more RAM-friendly, but requires explicit type annotations
python -m pip install 'types-aiobotocore-lite[connect]'


# standalone installation
python -m pip install types-aiobotocore-connect
```

<a id="how-to-uninstall"></a>

## How to uninstall

```bash
python -m pip uninstall -y types-aiobotocore-connect
```

<a id="usage"></a>

## Usage

Code samples can be found [here](./usage.md).

<a id="connectclient"></a>

## ConnectClient

Type annotations for `session.create_client("connect")` as
[ConnectClient](./client.md)

Can be used directly:

```python
from types_aiobotocore_connect.client import ConnectClient
```

<a id="methods"></a>

### Methods

- [__aenter__](./client.md#__aenter__)
- [__aexit__](./client.md#__aexit__)
- [associate_approved_origin](./client.md#associate_approved_origin)
- [associate_bot](./client.md#associate_bot)
- [associate_default_vocabulary](./client.md#associate_default_vocabulary)
- [associate_instance_storage_config](./client.md#associate_instance_storage_config)
- [associate_lambda_function](./client.md#associate_lambda_function)
- [associate_lex_bot](./client.md#associate_lex_bot)
- [associate_queue_quick_connects](./client.md#associate_queue_quick_connects)
- [associate_routing_profile_queues](./client.md#associate_routing_profile_queues)
- [associate_security_key](./client.md#associate_security_key)
- [can_paginate](./client.md#can_paginate)
- [create_agent_status](./client.md#create_agent_status)
- [create_contact_flow](./client.md#create_contact_flow)
- [create_contact_flow_module](./client.md#create_contact_flow_module)
- [create_hours_of_operation](./client.md#create_hours_of_operation)
- [create_instance](./client.md#create_instance)
- [create_integration_association](./client.md#create_integration_association)
- [create_queue](./client.md#create_queue)
- [create_quick_connect](./client.md#create_quick_connect)
- [create_routing_profile](./client.md#create_routing_profile)
- [create_security_profile](./client.md#create_security_profile)
- [create_use_case](./client.md#create_use_case)
- [create_user](./client.md#create_user)
- [create_user_hierarchy_group](./client.md#create_user_hierarchy_group)
- [create_vocabulary](./client.md#create_vocabulary)
- [delete_contact_flow](./client.md#delete_contact_flow)
- [delete_contact_flow_module](./client.md#delete_contact_flow_module)
- [delete_hours_of_operation](./client.md#delete_hours_of_operation)
- [delete_instance](./client.md#delete_instance)
- [delete_integration_association](./client.md#delete_integration_association)
- [delete_quick_connect](./client.md#delete_quick_connect)
- [delete_security_profile](./client.md#delete_security_profile)
- [delete_use_case](./client.md#delete_use_case)
- [delete_user](./client.md#delete_user)
- [delete_user_hierarchy_group](./client.md#delete_user_hierarchy_group)
- [delete_vocabulary](./client.md#delete_vocabulary)
- [describe_agent_status](./client.md#describe_agent_status)
- [describe_contact](./client.md#describe_contact)
- [describe_contact_flow](./client.md#describe_contact_flow)
- [describe_contact_flow_module](./client.md#describe_contact_flow_module)
- [describe_hours_of_operation](./client.md#describe_hours_of_operation)
- [describe_instance](./client.md#describe_instance)
- [describe_instance_attribute](./client.md#describe_instance_attribute)
- [describe_instance_storage_config](./client.md#describe_instance_storage_config)
- [describe_queue](./client.md#describe_queue)
- [describe_quick_connect](./client.md#describe_quick_connect)
- [describe_routing_profile](./client.md#describe_routing_profile)
- [describe_security_profile](./client.md#describe_security_profile)
- [describe_user](./client.md#describe_user)
- [describe_user_hierarchy_group](./client.md#describe_user_hierarchy_group)
- [describe_user_hierarchy_structure](./client.md#describe_user_hierarchy_structure)
- [describe_vocabulary](./client.md#describe_vocabulary)
- [disassociate_approved_origin](./client.md#disassociate_approved_origin)
- [disassociate_bot](./client.md#disassociate_bot)
- [disassociate_instance_storage_config](./client.md#disassociate_instance_storage_config)
- [disassociate_lambda_function](./client.md#disassociate_lambda_function)
- [disassociate_lex_bot](./client.md#disassociate_lex_bot)
- [disassociate_queue_quick_connects](./client.md#disassociate_queue_quick_connects)
- [disassociate_routing_profile_queues](./client.md#disassociate_routing_profile_queues)
- [disassociate_security_key](./client.md#disassociate_security_key)
- [exceptions](./client.md#exceptions)
- [generate_presigned_url](./client.md#generate_presigned_url)
- [get_contact_attributes](./client.md#get_contact_attributes)
- [get_current_metric_data](./client.md#get_current_metric_data)
- [get_federation_token](./client.md#get_federation_token)
- [get_metric_data](./client.md#get_metric_data)
- [get_paginator](./client.md#get_paginator)
- [list_agent_statuses](./client.md#list_agent_statuses)
- [list_approved_origins](./client.md#list_approved_origins)
- [list_bots](./client.md#list_bots)
- [list_contact_flow_modules](./client.md#list_contact_flow_modules)
- [list_contact_flows](./client.md#list_contact_flows)
- [list_contact_references](./client.md#list_contact_references)
- [list_default_vocabularies](./client.md#list_default_vocabularies)
- [list_hours_of_operations](./client.md#list_hours_of_operations)
- [list_instance_attributes](./client.md#list_instance_attributes)
- [list_instance_storage_configs](./client.md#list_instance_storage_configs)
- [list_instances](./client.md#list_instances)
- [list_integration_associations](./client.md#list_integration_associations)
- [list_lambda_functions](./client.md#list_lambda_functions)
- [list_lex_bots](./client.md#list_lex_bots)
- [list_phone_numbers](./client.md#list_phone_numbers)
- [list_prompts](./client.md#list_prompts)
- [list_queue_quick_connects](./client.md#list_queue_quick_connects)
- [list_queues](./client.md#list_queues)
- [list_quick_connects](./client.md#list_quick_connects)
- [list_routing_profile_queues](./client.md#list_routing_profile_queues)
- [list_routing_profiles](./client.md#list_routing_profiles)
- [list_security_keys](./client.md#list_security_keys)
- [list_security_profile_permissions](./client.md#list_security_profile_permissions)
- [list_security_profiles](./client.md#list_security_profiles)
- [list_tags_for_resource](./client.md#list_tags_for_resource)
- [list_use_cases](./client.md#list_use_cases)
- [list_user_hierarchy_groups](./client.md#list_user_hierarchy_groups)
- [list_users](./client.md#list_users)
- [resume_contact_recording](./client.md#resume_contact_recording)
- [search_vocabularies](./client.md#search_vocabularies)
- [start_chat_contact](./client.md#start_chat_contact)
- [start_contact_recording](./client.md#start_contact_recording)
- [start_contact_streaming](./client.md#start_contact_streaming)
- [start_outbound_voice_contact](./client.md#start_outbound_voice_contact)
- [start_task_contact](./client.md#start_task_contact)
- [stop_contact](./client.md#stop_contact)
- [stop_contact_recording](./client.md#stop_contact_recording)
- [stop_contact_streaming](./client.md#stop_contact_streaming)
- [suspend_contact_recording](./client.md#suspend_contact_recording)
- [tag_resource](./client.md#tag_resource)
- [untag_resource](./client.md#untag_resource)
- [update_agent_status](./client.md#update_agent_status)
- [update_contact](./client.md#update_contact)
- [update_contact_attributes](./client.md#update_contact_attributes)
- [update_contact_flow_content](./client.md#update_contact_flow_content)
- [update_contact_flow_metadata](./client.md#update_contact_flow_metadata)
- [update_contact_flow_module_content](./client.md#update_contact_flow_module_content)
- [update_contact_flow_module_metadata](./client.md#update_contact_flow_module_metadata)
- [update_contact_flow_name](./client.md#update_contact_flow_name)
- [update_contact_schedule](./client.md#update_contact_schedule)
- [update_hours_of_operation](./client.md#update_hours_of_operation)
- [update_instance_attribute](./client.md#update_instance_attribute)
- [update_instance_storage_config](./client.md#update_instance_storage_config)
- [update_queue_hours_of_operation](./client.md#update_queue_hours_of_operation)
- [update_queue_max_contacts](./client.md#update_queue_max_contacts)
- [update_queue_name](./client.md#update_queue_name)
- [update_queue_outbound_caller_config](./client.md#update_queue_outbound_caller_config)
- [update_queue_status](./client.md#update_queue_status)
- [update_quick_connect_config](./client.md#update_quick_connect_config)
- [update_quick_connect_name](./client.md#update_quick_connect_name)
- [update_routing_profile_concurrency](./client.md#update_routing_profile_concurrency)
- [update_routing_profile_default_outbound_queue](./client.md#update_routing_profile_default_outbound_queue)
- [update_routing_profile_name](./client.md#update_routing_profile_name)
- [update_routing_profile_queues](./client.md#update_routing_profile_queues)
- [update_security_profile](./client.md#update_security_profile)
- [update_user_hierarchy](./client.md#update_user_hierarchy)
- [update_user_hierarchy_group_name](./client.md#update_user_hierarchy_group_name)
- [update_user_hierarchy_structure](./client.md#update_user_hierarchy_structure)
- [update_user_identity_info](./client.md#update_user_identity_info)
- [update_user_phone_config](./client.md#update_user_phone_config)
- [update_user_routing_profile](./client.md#update_user_routing_profile)
- [update_user_security_profiles](./client.md#update_user_security_profiles)

<a id="exceptions"></a>

### Exceptions

ConnectClient [exceptions](./client.md#exceptions)

- AccessDeniedException
- ClientError
- ContactFlowNotPublishedException
- ContactNotFoundException
- DestinationNotAllowedException
- DuplicateResourceException
- IdempotencyException
- InternalServiceException
- InvalidContactFlowException
- InvalidContactFlowModuleException
- InvalidParameterException
- InvalidRequestException
- LimitExceededException
- OutboundContactNotPermittedException
- ResourceConflictException
- ResourceInUseException
- ResourceNotFoundException
- ServiceQuotaExceededException
- ThrottlingException
- UserNotFoundException

<a id="paginators"></a>

## Paginators

Type annotations for [paginators](./paginators.md) from
`boto3.client("connect").get_paginator("...")`.

Can be used directly:

```python
from types_aiobotocore_connect.paginator import GetMetricDataPaginator, ...
```

- [GetMetricDataPaginator](./paginators.md#getmetricdatapaginator)
- [ListAgentStatusesPaginator](./paginators.md#listagentstatusespaginator)
- [ListApprovedOriginsPaginator](./paginators.md#listapprovedoriginspaginator)
- [ListBotsPaginator](./paginators.md#listbotspaginator)
- [ListContactFlowModulesPaginator](./paginators.md#listcontactflowmodulespaginator)
- [ListContactFlowsPaginator](./paginators.md#listcontactflowspaginator)
- [ListContactReferencesPaginator](./paginators.md#listcontactreferencespaginator)
- [ListDefaultVocabulariesPaginator](./paginators.md#listdefaultvocabulariespaginator)
- [ListHoursOfOperationsPaginator](./paginators.md#listhoursofoperationspaginator)
- [ListInstanceAttributesPaginator](./paginators.md#listinstanceattributespaginator)
- [ListInstanceStorageConfigsPaginator](./paginators.md#listinstancestorageconfigspaginator)
- [ListInstancesPaginator](./paginators.md#listinstancespaginator)
- [ListIntegrationAssociationsPaginator](./paginators.md#listintegrationassociationspaginator)
- [ListLambdaFunctionsPaginator](./paginators.md#listlambdafunctionspaginator)
- [ListLexBotsPaginator](./paginators.md#listlexbotspaginator)
- [ListPhoneNumbersPaginator](./paginators.md#listphonenumberspaginator)
- [ListPromptsPaginator](./paginators.md#listpromptspaginator)
- [ListQueueQuickConnectsPaginator](./paginators.md#listqueuequickconnectspaginator)
- [ListQueuesPaginator](./paginators.md#listqueuespaginator)
- [ListQuickConnectsPaginator](./paginators.md#listquickconnectspaginator)
- [ListRoutingProfileQueuesPaginator](./paginators.md#listroutingprofilequeuespaginator)
- [ListRoutingProfilesPaginator](./paginators.md#listroutingprofilespaginator)
- [ListSecurityKeysPaginator](./paginators.md#listsecuritykeyspaginator)
- [ListSecurityProfilePermissionsPaginator](./paginators.md#listsecurityprofilepermissionspaginator)
- [ListSecurityProfilesPaginator](./paginators.md#listsecurityprofilespaginator)
- [ListUseCasesPaginator](./paginators.md#listusecasespaginator)
- [ListUserHierarchyGroupsPaginator](./paginators.md#listuserhierarchygroupspaginator)
- [ListUsersPaginator](./paginators.md#listuserspaginator)
- [SearchVocabulariesPaginator](./paginators.md#searchvocabulariespaginator)

<a id="literals"></a>

## Literals

Type annotations for [literals](./literals.md) used in methods and schema.

Can be used directly:

```python
from types_aiobotocore_connect.literals import AgentStatusStateType, ...
```

- [AgentStatusStateType](./literals.md#agentstatusstatetype)
- [AgentStatusTypeType](./literals.md#agentstatustypetype)
- [ChannelType](./literals.md#channeltype)
- [ComparisonType](./literals.md#comparisontype)
- [ContactFlowModuleStateType](./literals.md#contactflowmodulestatetype)
- [ContactFlowModuleStatusType](./literals.md#contactflowmodulestatustype)
- [ContactFlowStateType](./literals.md#contactflowstatetype)
- [ContactFlowTypeType](./literals.md#contactflowtypetype)
- [ContactInitiationMethodType](./literals.md#contactinitiationmethodtype)
- [CurrentMetricNameType](./literals.md#currentmetricnametype)
- [DirectoryTypeType](./literals.md#directorytypetype)
- [EncryptionTypeType](./literals.md#encryptiontypetype)
- [GetMetricDataPaginatorName](./literals.md#getmetricdatapaginatorname)
- [GroupingType](./literals.md#groupingtype)
- [HistoricalMetricNameType](./literals.md#historicalmetricnametype)
- [HoursOfOperationDaysType](./literals.md#hoursofoperationdaystype)
- [InstanceAttributeTypeType](./literals.md#instanceattributetypetype)
- [InstanceStatusType](./literals.md#instancestatustype)
- [InstanceStorageResourceTypeType](./literals.md#instancestorageresourcetypetype)
- [IntegrationTypeType](./literals.md#integrationtypetype)
- [LexVersionType](./literals.md#lexversiontype)
- [ListAgentStatusesPaginatorName](./literals.md#listagentstatusespaginatorname)
- [ListApprovedOriginsPaginatorName](./literals.md#listapprovedoriginspaginatorname)
- [ListBotsPaginatorName](./literals.md#listbotspaginatorname)
- [ListContactFlowModulesPaginatorName](./literals.md#listcontactflowmodulespaginatorname)
- [ListContactFlowsPaginatorName](./literals.md#listcontactflowspaginatorname)
- [ListContactReferencesPaginatorName](./literals.md#listcontactreferencespaginatorname)
- [ListDefaultVocabulariesPaginatorName](./literals.md#listdefaultvocabulariespaginatorname)
- [ListHoursOfOperationsPaginatorName](./literals.md#listhoursofoperationspaginatorname)
- [ListInstanceAttributesPaginatorName](./literals.md#listinstanceattributespaginatorname)
- [ListInstanceStorageConfigsPaginatorName](./literals.md#listinstancestorageconfigspaginatorname)
- [ListInstancesPaginatorName](./literals.md#listinstancespaginatorname)
- [ListIntegrationAssociationsPaginatorName](./literals.md#listintegrationassociationspaginatorname)
- [ListLambdaFunctionsPaginatorName](./literals.md#listlambdafunctionspaginatorname)
- [ListLexBotsPaginatorName](./literals.md#listlexbotspaginatorname)
- [ListPhoneNumbersPaginatorName](./literals.md#listphonenumberspaginatorname)
- [ListPromptsPaginatorName](./literals.md#listpromptspaginatorname)
- [ListQueueQuickConnectsPaginatorName](./literals.md#listqueuequickconnectspaginatorname)
- [ListQueuesPaginatorName](./literals.md#listqueuespaginatorname)
- [ListQuickConnectsPaginatorName](./literals.md#listquickconnectspaginatorname)
- [ListRoutingProfileQueuesPaginatorName](./literals.md#listroutingprofilequeuespaginatorname)
- [ListRoutingProfilesPaginatorName](./literals.md#listroutingprofilespaginatorname)
- [ListSecurityKeysPaginatorName](./literals.md#listsecuritykeyspaginatorname)
- [ListSecurityProfilePermissionsPaginatorName](./literals.md#listsecurityprofilepermissionspaginatorname)
- [ListSecurityProfilesPaginatorName](./literals.md#listsecurityprofilespaginatorname)
- [ListUseCasesPaginatorName](./literals.md#listusecasespaginatorname)
- [ListUserHierarchyGroupsPaginatorName](./literals.md#listuserhierarchygroupspaginatorname)
- [ListUsersPaginatorName](./literals.md#listuserspaginatorname)
- [PhoneNumberCountryCodeType](./literals.md#phonenumbercountrycodetype)
- [PhoneNumberTypeType](./literals.md#phonenumbertypetype)
- [PhoneTypeType](./literals.md#phonetypetype)
- [QueueStatusType](./literals.md#queuestatustype)
- [QueueTypeType](./literals.md#queuetypetype)
- [QuickConnectTypeType](./literals.md#quickconnecttypetype)
- [ReferenceStatusType](./literals.md#referencestatustype)
- [ReferenceTypeType](./literals.md#referencetypetype)
- [SearchVocabulariesPaginatorName](./literals.md#searchvocabulariespaginatorname)
- [SourceTypeType](./literals.md#sourcetypetype)
- [StatisticType](./literals.md#statistictype)
- [StorageTypeType](./literals.md#storagetypetype)
- [TrafficTypeType](./literals.md#traffictypetype)
- [UnitType](./literals.md#unittype)
- [UseCaseTypeType](./literals.md#usecasetypetype)
- [VocabularyLanguageCodeType](./literals.md#vocabularylanguagecodetype)
- [VocabularyStateType](./literals.md#vocabularystatetype)
- [VoiceRecordingTrackType](./literals.md#voicerecordingtracktype)
- [ConnectServiceName](./literals.md#connectservicename)
- [ServiceName](./literals.md#servicename)
- [ResourceServiceName](./literals.md#resourceservicename)
- [PaginatorName](./literals.md#paginatorname)

<a id="typed-dictionaries"></a>

## Typed dictionaries

Type annotations for [typed dictionaries](./type_defs.md) used in methods and
schema.

Can be used directly:

```python
from types_aiobotocore_connect.type_defs import AgentInfoTypeDef, ...
```

- [AgentInfoTypeDef](./type_defs.md#agentinfotypedef)
- [AgentStatusSummaryTypeDef](./type_defs.md#agentstatussummarytypedef)
- [AgentStatusTypeDef](./type_defs.md#agentstatustypedef)
- [AnswerMachineDetectionConfigTypeDef](./type_defs.md#answermachinedetectionconfigtypedef)
- [AssociateApprovedOriginRequestRequestTypeDef](./type_defs.md#associateapprovedoriginrequestrequesttypedef)
- [AssociateBotRequestRequestTypeDef](./type_defs.md#associatebotrequestrequesttypedef)
- [AssociateDefaultVocabularyRequestRequestTypeDef](./type_defs.md#associatedefaultvocabularyrequestrequesttypedef)
- [AssociateInstanceStorageConfigRequestRequestTypeDef](./type_defs.md#associateinstancestorageconfigrequestrequesttypedef)
- [AssociateInstanceStorageConfigResponseTypeDef](./type_defs.md#associateinstancestorageconfigresponsetypedef)
- [AssociateLambdaFunctionRequestRequestTypeDef](./type_defs.md#associatelambdafunctionrequestrequesttypedef)
- [AssociateLexBotRequestRequestTypeDef](./type_defs.md#associatelexbotrequestrequesttypedef)
- [AssociateQueueQuickConnectsRequestRequestTypeDef](./type_defs.md#associatequeuequickconnectsrequestrequesttypedef)
- [AssociateRoutingProfileQueuesRequestRequestTypeDef](./type_defs.md#associateroutingprofilequeuesrequestrequesttypedef)
- [AssociateSecurityKeyRequestRequestTypeDef](./type_defs.md#associatesecuritykeyrequestrequesttypedef)
- [AssociateSecurityKeyResponseTypeDef](./type_defs.md#associatesecuritykeyresponsetypedef)
- [AttachmentReferenceTypeDef](./type_defs.md#attachmentreferencetypedef)
- [AttributeTypeDef](./type_defs.md#attributetypedef)
- [ChatMessageTypeDef](./type_defs.md#chatmessagetypedef)
- [ChatStreamingConfigurationTypeDef](./type_defs.md#chatstreamingconfigurationtypedef)
- [ContactFlowModuleSummaryTypeDef](./type_defs.md#contactflowmodulesummarytypedef)
- [ContactFlowModuleTypeDef](./type_defs.md#contactflowmoduletypedef)
- [ContactFlowSummaryTypeDef](./type_defs.md#contactflowsummarytypedef)
- [ContactFlowTypeDef](./type_defs.md#contactflowtypedef)
- [ContactTypeDef](./type_defs.md#contacttypedef)
- [CreateAgentStatusRequestRequestTypeDef](./type_defs.md#createagentstatusrequestrequesttypedef)
- [CreateAgentStatusResponseTypeDef](./type_defs.md#createagentstatusresponsetypedef)
- [CreateContactFlowModuleRequestRequestTypeDef](./type_defs.md#createcontactflowmodulerequestrequesttypedef)
- [CreateContactFlowModuleResponseTypeDef](./type_defs.md#createcontactflowmoduleresponsetypedef)
- [CreateContactFlowRequestRequestTypeDef](./type_defs.md#createcontactflowrequestrequesttypedef)
- [CreateContactFlowResponseTypeDef](./type_defs.md#createcontactflowresponsetypedef)
- [CreateHoursOfOperationRequestRequestTypeDef](./type_defs.md#createhoursofoperationrequestrequesttypedef)
- [CreateHoursOfOperationResponseTypeDef](./type_defs.md#createhoursofoperationresponsetypedef)
- [CreateInstanceRequestRequestTypeDef](./type_defs.md#createinstancerequestrequesttypedef)
- [CreateInstanceResponseTypeDef](./type_defs.md#createinstanceresponsetypedef)
- [CreateIntegrationAssociationRequestRequestTypeDef](./type_defs.md#createintegrationassociationrequestrequesttypedef)
- [CreateIntegrationAssociationResponseTypeDef](./type_defs.md#createintegrationassociationresponsetypedef)
- [CreateQueueRequestRequestTypeDef](./type_defs.md#createqueuerequestrequesttypedef)
- [CreateQueueResponseTypeDef](./type_defs.md#createqueueresponsetypedef)
- [CreateQuickConnectRequestRequestTypeDef](./type_defs.md#createquickconnectrequestrequesttypedef)
- [CreateQuickConnectResponseTypeDef](./type_defs.md#createquickconnectresponsetypedef)
- [CreateRoutingProfileRequestRequestTypeDef](./type_defs.md#createroutingprofilerequestrequesttypedef)
- [CreateRoutingProfileResponseTypeDef](./type_defs.md#createroutingprofileresponsetypedef)
- [CreateSecurityProfileRequestRequestTypeDef](./type_defs.md#createsecurityprofilerequestrequesttypedef)
- [CreateSecurityProfileResponseTypeDef](./type_defs.md#createsecurityprofileresponsetypedef)
- [CreateUseCaseRequestRequestTypeDef](./type_defs.md#createusecaserequestrequesttypedef)
- [CreateUseCaseResponseTypeDef](./type_defs.md#createusecaseresponsetypedef)
- [CreateUserHierarchyGroupRequestRequestTypeDef](./type_defs.md#createuserhierarchygrouprequestrequesttypedef)
- [CreateUserHierarchyGroupResponseTypeDef](./type_defs.md#createuserhierarchygroupresponsetypedef)
- [CreateUserRequestRequestTypeDef](./type_defs.md#createuserrequestrequesttypedef)
- [CreateUserResponseTypeDef](./type_defs.md#createuserresponsetypedef)
- [CreateVocabularyRequestRequestTypeDef](./type_defs.md#createvocabularyrequestrequesttypedef)
- [CreateVocabularyResponseTypeDef](./type_defs.md#createvocabularyresponsetypedef)
- [CredentialsTypeDef](./type_defs.md#credentialstypedef)
- [CurrentMetricDataTypeDef](./type_defs.md#currentmetricdatatypedef)
- [CurrentMetricResultTypeDef](./type_defs.md#currentmetricresulttypedef)
- [CurrentMetricTypeDef](./type_defs.md#currentmetrictypedef)
- [DefaultVocabularyTypeDef](./type_defs.md#defaultvocabularytypedef)
- [DeleteContactFlowModuleRequestRequestTypeDef](./type_defs.md#deletecontactflowmodulerequestrequesttypedef)
- [DeleteContactFlowRequestRequestTypeDef](./type_defs.md#deletecontactflowrequestrequesttypedef)
- [DeleteHoursOfOperationRequestRequestTypeDef](./type_defs.md#deletehoursofoperationrequestrequesttypedef)
- [DeleteInstanceRequestRequestTypeDef](./type_defs.md#deleteinstancerequestrequesttypedef)
- [DeleteIntegrationAssociationRequestRequestTypeDef](./type_defs.md#deleteintegrationassociationrequestrequesttypedef)
- [DeleteQuickConnectRequestRequestTypeDef](./type_defs.md#deletequickconnectrequestrequesttypedef)
- [DeleteSecurityProfileRequestRequestTypeDef](./type_defs.md#deletesecurityprofilerequestrequesttypedef)
- [DeleteUseCaseRequestRequestTypeDef](./type_defs.md#deleteusecaserequestrequesttypedef)
- [DeleteUserHierarchyGroupRequestRequestTypeDef](./type_defs.md#deleteuserhierarchygrouprequestrequesttypedef)
- [DeleteUserRequestRequestTypeDef](./type_defs.md#deleteuserrequestrequesttypedef)
- [DeleteVocabularyRequestRequestTypeDef](./type_defs.md#deletevocabularyrequestrequesttypedef)
- [DeleteVocabularyResponseTypeDef](./type_defs.md#deletevocabularyresponsetypedef)
- [DescribeAgentStatusRequestRequestTypeDef](./type_defs.md#describeagentstatusrequestrequesttypedef)
- [DescribeAgentStatusResponseTypeDef](./type_defs.md#describeagentstatusresponsetypedef)
- [DescribeContactFlowModuleRequestRequestTypeDef](./type_defs.md#describecontactflowmodulerequestrequesttypedef)
- [DescribeContactFlowModuleResponseTypeDef](./type_defs.md#describecontactflowmoduleresponsetypedef)
- [DescribeContactFlowRequestRequestTypeDef](./type_defs.md#describecontactflowrequestrequesttypedef)
- [DescribeContactFlowResponseTypeDef](./type_defs.md#describecontactflowresponsetypedef)
- [DescribeContactRequestRequestTypeDef](./type_defs.md#describecontactrequestrequesttypedef)
- [DescribeContactResponseTypeDef](./type_defs.md#describecontactresponsetypedef)
- [DescribeHoursOfOperationRequestRequestTypeDef](./type_defs.md#describehoursofoperationrequestrequesttypedef)
- [DescribeHoursOfOperationResponseTypeDef](./type_defs.md#describehoursofoperationresponsetypedef)
- [DescribeInstanceAttributeRequestRequestTypeDef](./type_defs.md#describeinstanceattributerequestrequesttypedef)
- [DescribeInstanceAttributeResponseTypeDef](./type_defs.md#describeinstanceattributeresponsetypedef)
- [DescribeInstanceRequestRequestTypeDef](./type_defs.md#describeinstancerequestrequesttypedef)
- [DescribeInstanceResponseTypeDef](./type_defs.md#describeinstanceresponsetypedef)
- [DescribeInstanceStorageConfigRequestRequestTypeDef](./type_defs.md#describeinstancestorageconfigrequestrequesttypedef)
- [DescribeInstanceStorageConfigResponseTypeDef](./type_defs.md#describeinstancestorageconfigresponsetypedef)
- [DescribeQueueRequestRequestTypeDef](./type_defs.md#describequeuerequestrequesttypedef)
- [DescribeQueueResponseTypeDef](./type_defs.md#describequeueresponsetypedef)
- [DescribeQuickConnectRequestRequestTypeDef](./type_defs.md#describequickconnectrequestrequesttypedef)
- [DescribeQuickConnectResponseTypeDef](./type_defs.md#describequickconnectresponsetypedef)
- [DescribeRoutingProfileRequestRequestTypeDef](./type_defs.md#describeroutingprofilerequestrequesttypedef)
- [DescribeRoutingProfileResponseTypeDef](./type_defs.md#describeroutingprofileresponsetypedef)
- [DescribeSecurityProfileRequestRequestTypeDef](./type_defs.md#describesecurityprofilerequestrequesttypedef)
- [DescribeSecurityProfileResponseTypeDef](./type_defs.md#describesecurityprofileresponsetypedef)
- [DescribeUserHierarchyGroupRequestRequestTypeDef](./type_defs.md#describeuserhierarchygrouprequestrequesttypedef)
- [DescribeUserHierarchyGroupResponseTypeDef](./type_defs.md#describeuserhierarchygroupresponsetypedef)
- [DescribeUserHierarchyStructureRequestRequestTypeDef](./type_defs.md#describeuserhierarchystructurerequestrequesttypedef)
- [DescribeUserHierarchyStructureResponseTypeDef](./type_defs.md#describeuserhierarchystructureresponsetypedef)
- [DescribeUserRequestRequestTypeDef](./type_defs.md#describeuserrequestrequesttypedef)
- [DescribeUserResponseTypeDef](./type_defs.md#describeuserresponsetypedef)
- [DescribeVocabularyRequestRequestTypeDef](./type_defs.md#describevocabularyrequestrequesttypedef)
- [DescribeVocabularyResponseTypeDef](./type_defs.md#describevocabularyresponsetypedef)
- [DimensionsTypeDef](./type_defs.md#dimensionstypedef)
- [DisassociateApprovedOriginRequestRequestTypeDef](./type_defs.md#disassociateapprovedoriginrequestrequesttypedef)
- [DisassociateBotRequestRequestTypeDef](./type_defs.md#disassociatebotrequestrequesttypedef)
- [DisassociateInstanceStorageConfigRequestRequestTypeDef](./type_defs.md#disassociateinstancestorageconfigrequestrequesttypedef)
- [DisassociateLambdaFunctionRequestRequestTypeDef](./type_defs.md#disassociatelambdafunctionrequestrequesttypedef)
- [DisassociateLexBotRequestRequestTypeDef](./type_defs.md#disassociatelexbotrequestrequesttypedef)
- [DisassociateQueueQuickConnectsRequestRequestTypeDef](./type_defs.md#disassociatequeuequickconnectsrequestrequesttypedef)
- [DisassociateRoutingProfileQueuesRequestRequestTypeDef](./type_defs.md#disassociateroutingprofilequeuesrequestrequesttypedef)
- [DisassociateSecurityKeyRequestRequestTypeDef](./type_defs.md#disassociatesecuritykeyrequestrequesttypedef)
- [EncryptionConfigTypeDef](./type_defs.md#encryptionconfigtypedef)
- [FiltersTypeDef](./type_defs.md#filterstypedef)
- [GetContactAttributesRequestRequestTypeDef](./type_defs.md#getcontactattributesrequestrequesttypedef)
- [GetContactAttributesResponseTypeDef](./type_defs.md#getcontactattributesresponsetypedef)
- [GetCurrentMetricDataRequestRequestTypeDef](./type_defs.md#getcurrentmetricdatarequestrequesttypedef)
- [GetCurrentMetricDataResponseTypeDef](./type_defs.md#getcurrentmetricdataresponsetypedef)
- [GetFederationTokenRequestRequestTypeDef](./type_defs.md#getfederationtokenrequestrequesttypedef)
- [GetFederationTokenResponseTypeDef](./type_defs.md#getfederationtokenresponsetypedef)
- [GetMetricDataRequestRequestTypeDef](./type_defs.md#getmetricdatarequestrequesttypedef)
- [GetMetricDataResponseTypeDef](./type_defs.md#getmetricdataresponsetypedef)
- [HierarchyGroupSummaryTypeDef](./type_defs.md#hierarchygroupsummarytypedef)
- [HierarchyGroupTypeDef](./type_defs.md#hierarchygrouptypedef)
- [HierarchyLevelTypeDef](./type_defs.md#hierarchyleveltypedef)
- [HierarchyLevelUpdateTypeDef](./type_defs.md#hierarchylevelupdatetypedef)
- [HierarchyPathTypeDef](./type_defs.md#hierarchypathtypedef)
- [HierarchyStructureTypeDef](./type_defs.md#hierarchystructuretypedef)
- [HierarchyStructureUpdateTypeDef](./type_defs.md#hierarchystructureupdatetypedef)
- [HistoricalMetricDataTypeDef](./type_defs.md#historicalmetricdatatypedef)
- [HistoricalMetricResultTypeDef](./type_defs.md#historicalmetricresulttypedef)
- [HistoricalMetricTypeDef](./type_defs.md#historicalmetrictypedef)
- [HoursOfOperationConfigTypeDef](./type_defs.md#hoursofoperationconfigtypedef)
- [HoursOfOperationSummaryTypeDef](./type_defs.md#hoursofoperationsummarytypedef)
- [HoursOfOperationTimeSliceTypeDef](./type_defs.md#hoursofoperationtimeslicetypedef)
- [HoursOfOperationTypeDef](./type_defs.md#hoursofoperationtypedef)
- [InstanceStatusReasonTypeDef](./type_defs.md#instancestatusreasontypedef)
- [InstanceStorageConfigTypeDef](./type_defs.md#instancestorageconfigtypedef)
- [InstanceSummaryTypeDef](./type_defs.md#instancesummarytypedef)
- [InstanceTypeDef](./type_defs.md#instancetypedef)
- [IntegrationAssociationSummaryTypeDef](./type_defs.md#integrationassociationsummarytypedef)
- [KinesisFirehoseConfigTypeDef](./type_defs.md#kinesisfirehoseconfigtypedef)
- [KinesisStreamConfigTypeDef](./type_defs.md#kinesisstreamconfigtypedef)
- [KinesisVideoStreamConfigTypeDef](./type_defs.md#kinesisvideostreamconfigtypedef)
- [LexBotConfigTypeDef](./type_defs.md#lexbotconfigtypedef)
- [LexBotTypeDef](./type_defs.md#lexbottypedef)
- [LexV2BotTypeDef](./type_defs.md#lexv2bottypedef)
- [ListAgentStatusRequestRequestTypeDef](./type_defs.md#listagentstatusrequestrequesttypedef)
- [ListAgentStatusResponseTypeDef](./type_defs.md#listagentstatusresponsetypedef)
- [ListApprovedOriginsRequestRequestTypeDef](./type_defs.md#listapprovedoriginsrequestrequesttypedef)
- [ListApprovedOriginsResponseTypeDef](./type_defs.md#listapprovedoriginsresponsetypedef)
- [ListBotsRequestRequestTypeDef](./type_defs.md#listbotsrequestrequesttypedef)
- [ListBotsResponseTypeDef](./type_defs.md#listbotsresponsetypedef)
- [ListContactFlowModulesRequestRequestTypeDef](./type_defs.md#listcontactflowmodulesrequestrequesttypedef)
- [ListContactFlowModulesResponseTypeDef](./type_defs.md#listcontactflowmodulesresponsetypedef)
- [ListContactFlowsRequestRequestTypeDef](./type_defs.md#listcontactflowsrequestrequesttypedef)
- [ListContactFlowsResponseTypeDef](./type_defs.md#listcontactflowsresponsetypedef)
- [ListContactReferencesRequestRequestTypeDef](./type_defs.md#listcontactreferencesrequestrequesttypedef)
- [ListContactReferencesResponseTypeDef](./type_defs.md#listcontactreferencesresponsetypedef)
- [ListDefaultVocabulariesRequestRequestTypeDef](./type_defs.md#listdefaultvocabulariesrequestrequesttypedef)
- [ListDefaultVocabulariesResponseTypeDef](./type_defs.md#listdefaultvocabulariesresponsetypedef)
- [ListHoursOfOperationsRequestRequestTypeDef](./type_defs.md#listhoursofoperationsrequestrequesttypedef)
- [ListHoursOfOperationsResponseTypeDef](./type_defs.md#listhoursofoperationsresponsetypedef)
- [ListInstanceAttributesRequestRequestTypeDef](./type_defs.md#listinstanceattributesrequestrequesttypedef)
- [ListInstanceAttributesResponseTypeDef](./type_defs.md#listinstanceattributesresponsetypedef)
- [ListInstanceStorageConfigsRequestRequestTypeDef](./type_defs.md#listinstancestorageconfigsrequestrequesttypedef)
- [ListInstanceStorageConfigsResponseTypeDef](./type_defs.md#listinstancestorageconfigsresponsetypedef)
- [ListInstancesRequestRequestTypeDef](./type_defs.md#listinstancesrequestrequesttypedef)
- [ListInstancesResponseTypeDef](./type_defs.md#listinstancesresponsetypedef)
- [ListIntegrationAssociationsRequestRequestTypeDef](./type_defs.md#listintegrationassociationsrequestrequesttypedef)
- [ListIntegrationAssociationsResponseTypeDef](./type_defs.md#listintegrationassociationsresponsetypedef)
- [ListLambdaFunctionsRequestRequestTypeDef](./type_defs.md#listlambdafunctionsrequestrequesttypedef)
- [ListLambdaFunctionsResponseTypeDef](./type_defs.md#listlambdafunctionsresponsetypedef)
- [ListLexBotsRequestRequestTypeDef](./type_defs.md#listlexbotsrequestrequesttypedef)
- [ListLexBotsResponseTypeDef](./type_defs.md#listlexbotsresponsetypedef)
- [ListPhoneNumbersRequestRequestTypeDef](./type_defs.md#listphonenumbersrequestrequesttypedef)
- [ListPhoneNumbersResponseTypeDef](./type_defs.md#listphonenumbersresponsetypedef)
- [ListPromptsRequestRequestTypeDef](./type_defs.md#listpromptsrequestrequesttypedef)
- [ListPromptsResponseTypeDef](./type_defs.md#listpromptsresponsetypedef)
- [ListQueueQuickConnectsRequestRequestTypeDef](./type_defs.md#listqueuequickconnectsrequestrequesttypedef)
- [ListQueueQuickConnectsResponseTypeDef](./type_defs.md#listqueuequickconnectsresponsetypedef)
- [ListQueuesRequestRequestTypeDef](./type_defs.md#listqueuesrequestrequesttypedef)
- [ListQueuesResponseTypeDef](./type_defs.md#listqueuesresponsetypedef)
- [ListQuickConnectsRequestRequestTypeDef](./type_defs.md#listquickconnectsrequestrequesttypedef)
- [ListQuickConnectsResponseTypeDef](./type_defs.md#listquickconnectsresponsetypedef)
- [ListRoutingProfileQueuesRequestRequestTypeDef](./type_defs.md#listroutingprofilequeuesrequestrequesttypedef)
- [ListRoutingProfileQueuesResponseTypeDef](./type_defs.md#listroutingprofilequeuesresponsetypedef)
- [ListRoutingProfilesRequestRequestTypeDef](./type_defs.md#listroutingprofilesrequestrequesttypedef)
- [ListRoutingProfilesResponseTypeDef](./type_defs.md#listroutingprofilesresponsetypedef)
- [ListSecurityKeysRequestRequestTypeDef](./type_defs.md#listsecuritykeysrequestrequesttypedef)
- [ListSecurityKeysResponseTypeDef](./type_defs.md#listsecuritykeysresponsetypedef)
- [ListSecurityProfilePermissionsRequestRequestTypeDef](./type_defs.md#listsecurityprofilepermissionsrequestrequesttypedef)
- [ListSecurityProfilePermissionsResponseTypeDef](./type_defs.md#listsecurityprofilepermissionsresponsetypedef)
- [ListSecurityProfilesRequestRequestTypeDef](./type_defs.md#listsecurityprofilesrequestrequesttypedef)
- [ListSecurityProfilesResponseTypeDef](./type_defs.md#listsecurityprofilesresponsetypedef)
- [ListTagsForResourceRequestRequestTypeDef](./type_defs.md#listtagsforresourcerequestrequesttypedef)
- [ListTagsForResourceResponseTypeDef](./type_defs.md#listtagsforresourceresponsetypedef)
- [ListUseCasesRequestRequestTypeDef](./type_defs.md#listusecasesrequestrequesttypedef)
- [ListUseCasesResponseTypeDef](./type_defs.md#listusecasesresponsetypedef)
- [ListUserHierarchyGroupsRequestRequestTypeDef](./type_defs.md#listuserhierarchygroupsrequestrequesttypedef)
- [ListUserHierarchyGroupsResponseTypeDef](./type_defs.md#listuserhierarchygroupsresponsetypedef)
- [ListUsersRequestRequestTypeDef](./type_defs.md#listusersrequestrequesttypedef)
- [ListUsersResponseTypeDef](./type_defs.md#listusersresponsetypedef)
- [MediaConcurrencyTypeDef](./type_defs.md#mediaconcurrencytypedef)
- [OutboundCallerConfigTypeDef](./type_defs.md#outboundcallerconfigtypedef)
- [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
- [ParticipantDetailsTypeDef](./type_defs.md#participantdetailstypedef)
- [PhoneNumberQuickConnectConfigTypeDef](./type_defs.md#phonenumberquickconnectconfigtypedef)
- [PhoneNumberSummaryTypeDef](./type_defs.md#phonenumbersummarytypedef)
- [PromptSummaryTypeDef](./type_defs.md#promptsummarytypedef)
- [QueueInfoTypeDef](./type_defs.md#queueinfotypedef)
- [QueueQuickConnectConfigTypeDef](./type_defs.md#queuequickconnectconfigtypedef)
- [QueueReferenceTypeDef](./type_defs.md#queuereferencetypedef)
- [QueueSummaryTypeDef](./type_defs.md#queuesummarytypedef)
- [QueueTypeDef](./type_defs.md#queuetypedef)
- [QuickConnectConfigTypeDef](./type_defs.md#quickconnectconfigtypedef)
- [QuickConnectSummaryTypeDef](./type_defs.md#quickconnectsummarytypedef)
- [QuickConnectTypeDef](./type_defs.md#quickconnecttypedef)
- [ReferenceSummaryTypeDef](./type_defs.md#referencesummarytypedef)
- [ReferenceTypeDef](./type_defs.md#referencetypedef)
- [ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef)
- [ResumeContactRecordingRequestRequestTypeDef](./type_defs.md#resumecontactrecordingrequestrequesttypedef)
- [RoutingProfileQueueConfigSummaryTypeDef](./type_defs.md#routingprofilequeueconfigsummarytypedef)
- [RoutingProfileQueueConfigTypeDef](./type_defs.md#routingprofilequeueconfigtypedef)
- [RoutingProfileQueueReferenceTypeDef](./type_defs.md#routingprofilequeuereferencetypedef)
- [RoutingProfileSummaryTypeDef](./type_defs.md#routingprofilesummarytypedef)
- [RoutingProfileTypeDef](./type_defs.md#routingprofiletypedef)
- [S3ConfigTypeDef](./type_defs.md#s3configtypedef)
- [SearchVocabulariesRequestRequestTypeDef](./type_defs.md#searchvocabulariesrequestrequesttypedef)
- [SearchVocabulariesResponseTypeDef](./type_defs.md#searchvocabulariesresponsetypedef)
- [SecurityKeyTypeDef](./type_defs.md#securitykeytypedef)
- [SecurityProfileSummaryTypeDef](./type_defs.md#securityprofilesummarytypedef)
- [SecurityProfileTypeDef](./type_defs.md#securityprofiletypedef)
- [StartChatContactRequestRequestTypeDef](./type_defs.md#startchatcontactrequestrequesttypedef)
- [StartChatContactResponseTypeDef](./type_defs.md#startchatcontactresponsetypedef)
- [StartContactRecordingRequestRequestTypeDef](./type_defs.md#startcontactrecordingrequestrequesttypedef)
- [StartContactStreamingRequestRequestTypeDef](./type_defs.md#startcontactstreamingrequestrequesttypedef)
- [StartContactStreamingResponseTypeDef](./type_defs.md#startcontactstreamingresponsetypedef)
- [StartOutboundVoiceContactRequestRequestTypeDef](./type_defs.md#startoutboundvoicecontactrequestrequesttypedef)
- [StartOutboundVoiceContactResponseTypeDef](./type_defs.md#startoutboundvoicecontactresponsetypedef)
- [StartTaskContactRequestRequestTypeDef](./type_defs.md#starttaskcontactrequestrequesttypedef)
- [StartTaskContactResponseTypeDef](./type_defs.md#starttaskcontactresponsetypedef)
- [StopContactRecordingRequestRequestTypeDef](./type_defs.md#stopcontactrecordingrequestrequesttypedef)
- [StopContactRequestRequestTypeDef](./type_defs.md#stopcontactrequestrequesttypedef)
- [StopContactStreamingRequestRequestTypeDef](./type_defs.md#stopcontactstreamingrequestrequesttypedef)
- [SuspendContactRecordingRequestRequestTypeDef](./type_defs.md#suspendcontactrecordingrequestrequesttypedef)
- [TagResourceRequestRequestTypeDef](./type_defs.md#tagresourcerequestrequesttypedef)
- [ThresholdTypeDef](./type_defs.md#thresholdtypedef)
- [UntagResourceRequestRequestTypeDef](./type_defs.md#untagresourcerequestrequesttypedef)
- [UpdateAgentStatusRequestRequestTypeDef](./type_defs.md#updateagentstatusrequestrequesttypedef)
- [UpdateContactAttributesRequestRequestTypeDef](./type_defs.md#updatecontactattributesrequestrequesttypedef)
- [UpdateContactFlowContentRequestRequestTypeDef](./type_defs.md#updatecontactflowcontentrequestrequesttypedef)
- [UpdateContactFlowMetadataRequestRequestTypeDef](./type_defs.md#updatecontactflowmetadatarequestrequesttypedef)
- [UpdateContactFlowModuleContentRequestRequestTypeDef](./type_defs.md#updatecontactflowmodulecontentrequestrequesttypedef)
- [UpdateContactFlowModuleMetadataRequestRequestTypeDef](./type_defs.md#updatecontactflowmodulemetadatarequestrequesttypedef)
- [UpdateContactFlowNameRequestRequestTypeDef](./type_defs.md#updatecontactflownamerequestrequesttypedef)
- [UpdateContactRequestRequestTypeDef](./type_defs.md#updatecontactrequestrequesttypedef)
- [UpdateContactScheduleRequestRequestTypeDef](./type_defs.md#updatecontactschedulerequestrequesttypedef)
- [UpdateHoursOfOperationRequestRequestTypeDef](./type_defs.md#updatehoursofoperationrequestrequesttypedef)
- [UpdateInstanceAttributeRequestRequestTypeDef](./type_defs.md#updateinstanceattributerequestrequesttypedef)
- [UpdateInstanceStorageConfigRequestRequestTypeDef](./type_defs.md#updateinstancestorageconfigrequestrequesttypedef)
- [UpdateQueueHoursOfOperationRequestRequestTypeDef](./type_defs.md#updatequeuehoursofoperationrequestrequesttypedef)
- [UpdateQueueMaxContactsRequestRequestTypeDef](./type_defs.md#updatequeuemaxcontactsrequestrequesttypedef)
- [UpdateQueueNameRequestRequestTypeDef](./type_defs.md#updatequeuenamerequestrequesttypedef)
- [UpdateQueueOutboundCallerConfigRequestRequestTypeDef](./type_defs.md#updatequeueoutboundcallerconfigrequestrequesttypedef)
- [UpdateQueueStatusRequestRequestTypeDef](./type_defs.md#updatequeuestatusrequestrequesttypedef)
- [UpdateQuickConnectConfigRequestRequestTypeDef](./type_defs.md#updatequickconnectconfigrequestrequesttypedef)
- [UpdateQuickConnectNameRequestRequestTypeDef](./type_defs.md#updatequickconnectnamerequestrequesttypedef)
- [UpdateRoutingProfileConcurrencyRequestRequestTypeDef](./type_defs.md#updateroutingprofileconcurrencyrequestrequesttypedef)
- [UpdateRoutingProfileDefaultOutboundQueueRequestRequestTypeDef](./type_defs.md#updateroutingprofiledefaultoutboundqueuerequestrequesttypedef)
- [UpdateRoutingProfileNameRequestRequestTypeDef](./type_defs.md#updateroutingprofilenamerequestrequesttypedef)
- [UpdateRoutingProfileQueuesRequestRequestTypeDef](./type_defs.md#updateroutingprofilequeuesrequestrequesttypedef)
- [UpdateSecurityProfileRequestRequestTypeDef](./type_defs.md#updatesecurityprofilerequestrequesttypedef)
- [UpdateUserHierarchyGroupNameRequestRequestTypeDef](./type_defs.md#updateuserhierarchygroupnamerequestrequesttypedef)
- [UpdateUserHierarchyRequestRequestTypeDef](./type_defs.md#updateuserhierarchyrequestrequesttypedef)
- [UpdateUserHierarchyStructureRequestRequestTypeDef](./type_defs.md#updateuserhierarchystructurerequestrequesttypedef)
- [UpdateUserIdentityInfoRequestRequestTypeDef](./type_defs.md#updateuseridentityinforequestrequesttypedef)
- [UpdateUserPhoneConfigRequestRequestTypeDef](./type_defs.md#updateuserphoneconfigrequestrequesttypedef)
- [UpdateUserRoutingProfileRequestRequestTypeDef](./type_defs.md#updateuserroutingprofilerequestrequesttypedef)
- [UpdateUserSecurityProfilesRequestRequestTypeDef](./type_defs.md#updateusersecurityprofilesrequestrequesttypedef)
- [UrlReferenceTypeDef](./type_defs.md#urlreferencetypedef)
- [UseCaseTypeDef](./type_defs.md#usecasetypedef)
- [UserIdentityInfoTypeDef](./type_defs.md#useridentityinfotypedef)
- [UserPhoneConfigTypeDef](./type_defs.md#userphoneconfigtypedef)
- [UserQuickConnectConfigTypeDef](./type_defs.md#userquickconnectconfigtypedef)
- [UserSummaryTypeDef](./type_defs.md#usersummarytypedef)
- [UserTypeDef](./type_defs.md#usertypedef)
- [VocabularySummaryTypeDef](./type_defs.md#vocabularysummarytypedef)
- [VocabularyTypeDef](./type_defs.md#vocabularytypedef)
- [VoiceRecordingConfigurationTypeDef](./type_defs.md#voicerecordingconfigurationtypedef)