<a id="paginators-for-aiobotocore-connect-module"></a>

# Paginators for aiobotocore Connect module

> [Index](../README.md) > [Connect](./README.md) > Paginators

Auto-generated documentation for
[Connect](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect)
type annotations stubs module
[types-aiobotocore-connect](https://pypi.org/project/types-aiobotocore-connect/).

- [Paginators for aiobotocore Connect module](#paginators-for-aiobotocore-connect-module)
  - [GetMetricDataPaginator](#getmetricdatapaginator)
  - [ListAgentStatusesPaginator](#listagentstatusespaginator)
  - [ListApprovedOriginsPaginator](#listapprovedoriginspaginator)
  - [ListBotsPaginator](#listbotspaginator)
  - [ListContactFlowModulesPaginator](#listcontactflowmodulespaginator)
  - [ListContactFlowsPaginator](#listcontactflowspaginator)
  - [ListContactReferencesPaginator](#listcontactreferencespaginator)
  - [ListDefaultVocabulariesPaginator](#listdefaultvocabulariespaginator)
  - [ListHoursOfOperationsPaginator](#listhoursofoperationspaginator)
  - [ListInstanceAttributesPaginator](#listinstanceattributespaginator)
  - [ListInstanceStorageConfigsPaginator](#listinstancestorageconfigspaginator)
  - [ListInstancesPaginator](#listinstancespaginator)
  - [ListIntegrationAssociationsPaginator](#listintegrationassociationspaginator)
  - [ListLambdaFunctionsPaginator](#listlambdafunctionspaginator)
  - [ListLexBotsPaginator](#listlexbotspaginator)
  - [ListPhoneNumbersPaginator](#listphonenumberspaginator)
  - [ListPromptsPaginator](#listpromptspaginator)
  - [ListQueueQuickConnectsPaginator](#listqueuequickconnectspaginator)
  - [ListQueuesPaginator](#listqueuespaginator)
  - [ListQuickConnectsPaginator](#listquickconnectspaginator)
  - [ListRoutingProfileQueuesPaginator](#listroutingprofilequeuespaginator)
  - [ListRoutingProfilesPaginator](#listroutingprofilespaginator)
  - [ListSecurityKeysPaginator](#listsecuritykeyspaginator)
  - [ListSecurityProfilePermissionsPaginator](#listsecurityprofilepermissionspaginator)
  - [ListSecurityProfilesPaginator](#listsecurityprofilespaginator)
  - [ListUseCasesPaginator](#listusecasespaginator)
  - [ListUserHierarchyGroupsPaginator](#listuserhierarchygroupspaginator)
  - [ListUsersPaginator](#listuserspaginator)
  - [SearchVocabulariesPaginator](#searchvocabulariespaginator)

<a id="getmetricdatapaginator"></a>

## GetMetricDataPaginator

Type annotations for
`session.create_client("connect").get_paginator("get_metric_data")`.

Can be used directly:

```python
from aiobotocore.session import get_session

from types_aiobotocore_connect.paginator import GetMetricDataPaginator

session = get_session()
async with session.create_client("connect") as client:
    client: ConnectClient
    paginator: GetMetricDataPaginator = client.get_paginator("get_metric_data")
```

Boto3 documentation:
[Connect.Paginator.GetMetricData](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Paginator.GetMetricData)

Arguments for `GetMetricDataPaginator.paginate` method:

- `InstanceId`: `str` *(required)*
- `StartTime`: `Union`\[`datetime`, `str`\] *(required)*
- `EndTime`: `Union`\[`datetime`, `str`\] *(required)*
- `Filters`: [FiltersTypeDef](./type_defs.md#filterstypedef) *(required)*
- `HistoricalMetrics`:
  `Sequence`\[[HistoricalMetricTypeDef](./type_defs.md#historicalmetrictypedef)\]
  *(required)*
- `Groupings`: `Sequence`\[[GroupingType](./literals.md#groupingtype)\]
- `PaginationConfig`:
  [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)

`GetMetricDataPaginator.paginate` returns
`AsyncIterator`\[[GetMetricDataResponseTypeDef](./type_defs.md#getmetricdataresponsetypedef)\].

<a id="listagentstatusespaginator"></a>

## ListAgentStatusesPaginator

Type annotations for
`session.create_client("connect").get_paginator("list_agent_statuses")`.

Can be used directly:

```python
from aiobotocore.session import get_session

from types_aiobotocore_connect.paginator import ListAgentStatusesPaginator

session = get_session()
async with session.create_client("connect") as client:
    client: ConnectClient
    paginator: ListAgentStatusesPaginator = client.get_paginator("list_agent_statuses")
```

Boto3 documentation:
[Connect.Paginator.ListAgentStatuses](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Paginator.ListAgentStatuses)

Arguments for `ListAgentStatusesPaginator.paginate` method:

- `InstanceId`: `str` *(required)*
- `AgentStatusTypes`:
  `Sequence`\[[AgentStatusTypeType](./literals.md#agentstatustypetype)\]
- `PaginationConfig`:
  [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)

`ListAgentStatusesPaginator.paginate` returns
`AsyncIterator`\[[ListAgentStatusResponseTypeDef](./type_defs.md#listagentstatusresponsetypedef)\].

<a id="listapprovedoriginspaginator"></a>

## ListApprovedOriginsPaginator

Type annotations for
`session.create_client("connect").get_paginator("list_approved_origins")`.

Can be used directly:

```python
from aiobotocore.session import get_session

from types_aiobotocore_connect.paginator import ListApprovedOriginsPaginator

session = get_session()
async with session.create_client("connect") as client:
    client: ConnectClient
    paginator: ListApprovedOriginsPaginator = client.get_paginator("list_approved_origins")
```

Boto3 documentation:
[Connect.Paginator.ListApprovedOrigins](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Paginator.ListApprovedOrigins)

Arguments for `ListApprovedOriginsPaginator.paginate` method:

- `InstanceId`: `str` *(required)*
- `PaginationConfig`:
  [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)

`ListApprovedOriginsPaginator.paginate` returns
`AsyncIterator`\[[ListApprovedOriginsResponseTypeDef](./type_defs.md#listapprovedoriginsresponsetypedef)\].

<a id="listbotspaginator"></a>

## ListBotsPaginator

Type annotations for
`session.create_client("connect").get_paginator("list_bots")`.

Can be used directly:

```python
from aiobotocore.session import get_session

from types_aiobotocore_connect.paginator import ListBotsPaginator

session = get_session()
async with session.create_client("connect") as client:
    client: ConnectClient
    paginator: ListBotsPaginator = client.get_paginator("list_bots")
```

Boto3 documentation:
[Connect.Paginator.ListBots](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Paginator.ListBots)

Arguments for `ListBotsPaginator.paginate` method:

- `InstanceId`: `str` *(required)*
- `LexVersion`: [LexVersionType](./literals.md#lexversiontype) *(required)*
- `PaginationConfig`:
  [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)

`ListBotsPaginator.paginate` returns
`AsyncIterator`\[[ListBotsResponseTypeDef](./type_defs.md#listbotsresponsetypedef)\].

<a id="listcontactflowmodulespaginator"></a>

## ListContactFlowModulesPaginator

Type annotations for
`session.create_client("connect").get_paginator("list_contact_flow_modules")`.

Can be used directly:

```python
from aiobotocore.session import get_session

from types_aiobotocore_connect.paginator import ListContactFlowModulesPaginator

session = get_session()
async with session.create_client("connect") as client:
    client: ConnectClient
    paginator: ListContactFlowModulesPaginator = client.get_paginator("list_contact_flow_modules")
```

Boto3 documentation:
[Connect.Paginator.ListContactFlowModules](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Paginator.ListContactFlowModules)

Arguments for `ListContactFlowModulesPaginator.paginate` method:

- `InstanceId`: `str` *(required)*
- `ContactFlowModuleState`:
  [ContactFlowModuleStateType](./literals.md#contactflowmodulestatetype)
- `PaginationConfig`:
  [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)

`ListContactFlowModulesPaginator.paginate` returns
`AsyncIterator`\[[ListContactFlowModulesResponseTypeDef](./type_defs.md#listcontactflowmodulesresponsetypedef)\].

<a id="listcontactflowspaginator"></a>

## ListContactFlowsPaginator

Type annotations for
`session.create_client("connect").get_paginator("list_contact_flows")`.

Can be used directly:

```python
from aiobotocore.session import get_session

from types_aiobotocore_connect.paginator import ListContactFlowsPaginator

session = get_session()
async with session.create_client("connect") as client:
    client: ConnectClient
    paginator: ListContactFlowsPaginator = client.get_paginator("list_contact_flows")
```

Boto3 documentation:
[Connect.Paginator.ListContactFlows](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Paginator.ListContactFlows)

Arguments for `ListContactFlowsPaginator.paginate` method:

- `InstanceId`: `str` *(required)*
- `ContactFlowTypes`:
  `Sequence`\[[ContactFlowTypeType](./literals.md#contactflowtypetype)\]
- `PaginationConfig`:
  [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)

`ListContactFlowsPaginator.paginate` returns
`AsyncIterator`\[[ListContactFlowsResponseTypeDef](./type_defs.md#listcontactflowsresponsetypedef)\].

<a id="listcontactreferencespaginator"></a>

## ListContactReferencesPaginator

Type annotations for
`session.create_client("connect").get_paginator("list_contact_references")`.

Can be used directly:

```python
from aiobotocore.session import get_session

from types_aiobotocore_connect.paginator import ListContactReferencesPaginator

session = get_session()
async with session.create_client("connect") as client:
    client: ConnectClient
    paginator: ListContactReferencesPaginator = client.get_paginator("list_contact_references")
```

Boto3 documentation:
[Connect.Paginator.ListContactReferences](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Paginator.ListContactReferences)

Arguments for `ListContactReferencesPaginator.paginate` method:

- `InstanceId`: `str` *(required)*
- `ContactId`: `str` *(required)*
- `ReferenceTypes`:
  `Sequence`\[[ReferenceTypeType](./literals.md#referencetypetype)\]
  *(required)*
- `PaginationConfig`:
  [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)

`ListContactReferencesPaginator.paginate` returns
`AsyncIterator`\[[ListContactReferencesResponseTypeDef](./type_defs.md#listcontactreferencesresponsetypedef)\].

<a id="listdefaultvocabulariespaginator"></a>

## ListDefaultVocabulariesPaginator

Type annotations for
`session.create_client("connect").get_paginator("list_default_vocabularies")`.

Can be used directly:

```python
from aiobotocore.session import get_session

from types_aiobotocore_connect.paginator import ListDefaultVocabulariesPaginator

session = get_session()
async with session.create_client("connect") as client:
    client: ConnectClient
    paginator: ListDefaultVocabulariesPaginator = client.get_paginator("list_default_vocabularies")
```

Boto3 documentation:
[Connect.Paginator.ListDefaultVocabularies](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Paginator.ListDefaultVocabularies)

Arguments for `ListDefaultVocabulariesPaginator.paginate` method:

- `InstanceId`: `str` *(required)*
- `LanguageCode`:
  [VocabularyLanguageCodeType](./literals.md#vocabularylanguagecodetype)
- `PaginationConfig`:
  [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)

`ListDefaultVocabulariesPaginator.paginate` returns
`AsyncIterator`\[[ListDefaultVocabulariesResponseTypeDef](./type_defs.md#listdefaultvocabulariesresponsetypedef)\].

<a id="listhoursofoperationspaginator"></a>

## ListHoursOfOperationsPaginator

Type annotations for
`session.create_client("connect").get_paginator("list_hours_of_operations")`.

Can be used directly:

```python
from aiobotocore.session import get_session

from types_aiobotocore_connect.paginator import ListHoursOfOperationsPaginator

session = get_session()
async with session.create_client("connect") as client:
    client: ConnectClient
    paginator: ListHoursOfOperationsPaginator = client.get_paginator("list_hours_of_operations")
```

Boto3 documentation:
[Connect.Paginator.ListHoursOfOperations](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Paginator.ListHoursOfOperations)

Arguments for `ListHoursOfOperationsPaginator.paginate` method:

- `InstanceId`: `str` *(required)*
- `PaginationConfig`:
  [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)

`ListHoursOfOperationsPaginator.paginate` returns
`AsyncIterator`\[[ListHoursOfOperationsResponseTypeDef](./type_defs.md#listhoursofoperationsresponsetypedef)\].

<a id="listinstanceattributespaginator"></a>

## ListInstanceAttributesPaginator

Type annotations for
`session.create_client("connect").get_paginator("list_instance_attributes")`.

Can be used directly:

```python
from aiobotocore.session import get_session

from types_aiobotocore_connect.paginator import ListInstanceAttributesPaginator

session = get_session()
async with session.create_client("connect") as client:
    client: ConnectClient
    paginator: ListInstanceAttributesPaginator = client.get_paginator("list_instance_attributes")
```

Boto3 documentation:
[Connect.Paginator.ListInstanceAttributes](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Paginator.ListInstanceAttributes)

Arguments for `ListInstanceAttributesPaginator.paginate` method:

- `InstanceId`: `str` *(required)*
- `PaginationConfig`:
  [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)

`ListInstanceAttributesPaginator.paginate` returns
`AsyncIterator`\[[ListInstanceAttributesResponseTypeDef](./type_defs.md#listinstanceattributesresponsetypedef)\].

<a id="listinstancestorageconfigspaginator"></a>

## ListInstanceStorageConfigsPaginator

Type annotations for
`session.create_client("connect").get_paginator("list_instance_storage_configs")`.

Can be used directly:

```python
from aiobotocore.session import get_session

from types_aiobotocore_connect.paginator import ListInstanceStorageConfigsPaginator

session = get_session()
async with session.create_client("connect") as client:
    client: ConnectClient
    paginator: ListInstanceStorageConfigsPaginator = client.get_paginator("list_instance_storage_configs")
```

Boto3 documentation:
[Connect.Paginator.ListInstanceStorageConfigs](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Paginator.ListInstanceStorageConfigs)

Arguments for `ListInstanceStorageConfigsPaginator.paginate` method:

- `InstanceId`: `str` *(required)*
- `ResourceType`:
  [InstanceStorageResourceTypeType](./literals.md#instancestorageresourcetypetype)
  *(required)*
- `PaginationConfig`:
  [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)

`ListInstanceStorageConfigsPaginator.paginate` returns
`AsyncIterator`\[[ListInstanceStorageConfigsResponseTypeDef](./type_defs.md#listinstancestorageconfigsresponsetypedef)\].

<a id="listinstancespaginator"></a>

## ListInstancesPaginator

Type annotations for
`session.create_client("connect").get_paginator("list_instances")`.

Can be used directly:

```python
from aiobotocore.session import get_session

from types_aiobotocore_connect.paginator import ListInstancesPaginator

session = get_session()
async with session.create_client("connect") as client:
    client: ConnectClient
    paginator: ListInstancesPaginator = client.get_paginator("list_instances")
```

Boto3 documentation:
[Connect.Paginator.ListInstances](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Paginator.ListInstances)

Arguments for `ListInstancesPaginator.paginate` method:

- `PaginationConfig`:
  [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)

`ListInstancesPaginator.paginate` returns
`AsyncIterator`\[[ListInstancesResponseTypeDef](./type_defs.md#listinstancesresponsetypedef)\].

<a id="listintegrationassociationspaginator"></a>

## ListIntegrationAssociationsPaginator

Type annotations for
`session.create_client("connect").get_paginator("list_integration_associations")`.

Can be used directly:

```python
from aiobotocore.session import get_session

from types_aiobotocore_connect.paginator import ListIntegrationAssociationsPaginator

session = get_session()
async with session.create_client("connect") as client:
    client: ConnectClient
    paginator: ListIntegrationAssociationsPaginator = client.get_paginator("list_integration_associations")
```

Boto3 documentation:
[Connect.Paginator.ListIntegrationAssociations](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Paginator.ListIntegrationAssociations)

Arguments for `ListIntegrationAssociationsPaginator.paginate` method:

- `InstanceId`: `str` *(required)*
- `IntegrationType`: [IntegrationTypeType](./literals.md#integrationtypetype)
- `PaginationConfig`:
  [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)

`ListIntegrationAssociationsPaginator.paginate` returns
`AsyncIterator`\[[ListIntegrationAssociationsResponseTypeDef](./type_defs.md#listintegrationassociationsresponsetypedef)\].

<a id="listlambdafunctionspaginator"></a>

## ListLambdaFunctionsPaginator

Type annotations for
`session.create_client("connect").get_paginator("list_lambda_functions")`.

Can be used directly:

```python
from aiobotocore.session import get_session

from types_aiobotocore_connect.paginator import ListLambdaFunctionsPaginator

session = get_session()
async with session.create_client("connect") as client:
    client: ConnectClient
    paginator: ListLambdaFunctionsPaginator = client.get_paginator("list_lambda_functions")
```

Boto3 documentation:
[Connect.Paginator.ListLambdaFunctions](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Paginator.ListLambdaFunctions)

Arguments for `ListLambdaFunctionsPaginator.paginate` method:

- `InstanceId`: `str` *(required)*
- `PaginationConfig`:
  [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)

`ListLambdaFunctionsPaginator.paginate` returns
`AsyncIterator`\[[ListLambdaFunctionsResponseTypeDef](./type_defs.md#listlambdafunctionsresponsetypedef)\].

<a id="listlexbotspaginator"></a>

## ListLexBotsPaginator

Type annotations for
`session.create_client("connect").get_paginator("list_lex_bots")`.

Can be used directly:

```python
from aiobotocore.session import get_session

from types_aiobotocore_connect.paginator import ListLexBotsPaginator

session = get_session()
async with session.create_client("connect") as client:
    client: ConnectClient
    paginator: ListLexBotsPaginator = client.get_paginator("list_lex_bots")
```

Boto3 documentation:
[Connect.Paginator.ListLexBots](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Paginator.ListLexBots)

Arguments for `ListLexBotsPaginator.paginate` method:

- `InstanceId`: `str` *(required)*
- `PaginationConfig`:
  [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)

`ListLexBotsPaginator.paginate` returns
`AsyncIterator`\[[ListLexBotsResponseTypeDef](./type_defs.md#listlexbotsresponsetypedef)\].

<a id="listphonenumberspaginator"></a>

## ListPhoneNumbersPaginator

Type annotations for
`session.create_client("connect").get_paginator("list_phone_numbers")`.

Can be used directly:

```python
from aiobotocore.session import get_session

from types_aiobotocore_connect.paginator import ListPhoneNumbersPaginator

session = get_session()
async with session.create_client("connect") as client:
    client: ConnectClient
    paginator: ListPhoneNumbersPaginator = client.get_paginator("list_phone_numbers")
```

Boto3 documentation:
[Connect.Paginator.ListPhoneNumbers](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Paginator.ListPhoneNumbers)

Arguments for `ListPhoneNumbersPaginator.paginate` method:

- `InstanceId`: `str` *(required)*
- `PhoneNumberTypes`:
  `Sequence`\[[PhoneNumberTypeType](./literals.md#phonenumbertypetype)\]
- `PhoneNumberCountryCodes`:
  `Sequence`\[[PhoneNumberCountryCodeType](./literals.md#phonenumbercountrycodetype)\]
- `PaginationConfig`:
  [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)

`ListPhoneNumbersPaginator.paginate` returns
`AsyncIterator`\[[ListPhoneNumbersResponseTypeDef](./type_defs.md#listphonenumbersresponsetypedef)\].

<a id="listpromptspaginator"></a>

## ListPromptsPaginator

Type annotations for
`session.create_client("connect").get_paginator("list_prompts")`.

Can be used directly:

```python
from aiobotocore.session import get_session

from types_aiobotocore_connect.paginator import ListPromptsPaginator

session = get_session()
async with session.create_client("connect") as client:
    client: ConnectClient
    paginator: ListPromptsPaginator = client.get_paginator("list_prompts")
```

Boto3 documentation:
[Connect.Paginator.ListPrompts](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Paginator.ListPrompts)

Arguments for `ListPromptsPaginator.paginate` method:

- `InstanceId`: `str` *(required)*
- `PaginationConfig`:
  [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)

`ListPromptsPaginator.paginate` returns
`AsyncIterator`\[[ListPromptsResponseTypeDef](./type_defs.md#listpromptsresponsetypedef)\].

<a id="listqueuequickconnectspaginator"></a>

## ListQueueQuickConnectsPaginator

Type annotations for
`session.create_client("connect").get_paginator("list_queue_quick_connects")`.

Can be used directly:

```python
from aiobotocore.session import get_session

from types_aiobotocore_connect.paginator import ListQueueQuickConnectsPaginator

session = get_session()
async with session.create_client("connect") as client:
    client: ConnectClient
    paginator: ListQueueQuickConnectsPaginator = client.get_paginator("list_queue_quick_connects")
```

Boto3 documentation:
[Connect.Paginator.ListQueueQuickConnects](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Paginator.ListQueueQuickConnects)

Arguments for `ListQueueQuickConnectsPaginator.paginate` method:

- `InstanceId`: `str` *(required)*
- `QueueId`: `str` *(required)*
- `PaginationConfig`:
  [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)

`ListQueueQuickConnectsPaginator.paginate` returns
`AsyncIterator`\[[ListQueueQuickConnectsResponseTypeDef](./type_defs.md#listqueuequickconnectsresponsetypedef)\].

<a id="listqueuespaginator"></a>

## ListQueuesPaginator

Type annotations for
`session.create_client("connect").get_paginator("list_queues")`.

Can be used directly:

```python
from aiobotocore.session import get_session

from types_aiobotocore_connect.paginator import ListQueuesPaginator

session = get_session()
async with session.create_client("connect") as client:
    client: ConnectClient
    paginator: ListQueuesPaginator = client.get_paginator("list_queues")
```

Boto3 documentation:
[Connect.Paginator.ListQueues](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Paginator.ListQueues)

Arguments for `ListQueuesPaginator.paginate` method:

- `InstanceId`: `str` *(required)*
- `QueueTypes`: `Sequence`\[[QueueTypeType](./literals.md#queuetypetype)\]
- `PaginationConfig`:
  [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)

`ListQueuesPaginator.paginate` returns
`AsyncIterator`\[[ListQueuesResponseTypeDef](./type_defs.md#listqueuesresponsetypedef)\].

<a id="listquickconnectspaginator"></a>

## ListQuickConnectsPaginator

Type annotations for
`session.create_client("connect").get_paginator("list_quick_connects")`.

Can be used directly:

```python
from aiobotocore.session import get_session

from types_aiobotocore_connect.paginator import ListQuickConnectsPaginator

session = get_session()
async with session.create_client("connect") as client:
    client: ConnectClient
    paginator: ListQuickConnectsPaginator = client.get_paginator("list_quick_connects")
```

Boto3 documentation:
[Connect.Paginator.ListQuickConnects](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Paginator.ListQuickConnects)

Arguments for `ListQuickConnectsPaginator.paginate` method:

- `InstanceId`: `str` *(required)*
- `QuickConnectTypes`:
  `Sequence`\[[QuickConnectTypeType](./literals.md#quickconnecttypetype)\]
- `PaginationConfig`:
  [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)

`ListQuickConnectsPaginator.paginate` returns
`AsyncIterator`\[[ListQuickConnectsResponseTypeDef](./type_defs.md#listquickconnectsresponsetypedef)\].

<a id="listroutingprofilequeuespaginator"></a>

## ListRoutingProfileQueuesPaginator

Type annotations for
`session.create_client("connect").get_paginator("list_routing_profile_queues")`.

Can be used directly:

```python
from aiobotocore.session import get_session

from types_aiobotocore_connect.paginator import ListRoutingProfileQueuesPaginator

session = get_session()
async with session.create_client("connect") as client:
    client: ConnectClient
    paginator: ListRoutingProfileQueuesPaginator = client.get_paginator("list_routing_profile_queues")
```

Boto3 documentation:
[Connect.Paginator.ListRoutingProfileQueues](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Paginator.ListRoutingProfileQueues)

Arguments for `ListRoutingProfileQueuesPaginator.paginate` method:

- `InstanceId`: `str` *(required)*
- `RoutingProfileId`: `str` *(required)*
- `PaginationConfig`:
  [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)

`ListRoutingProfileQueuesPaginator.paginate` returns
`AsyncIterator`\[[ListRoutingProfileQueuesResponseTypeDef](./type_defs.md#listroutingprofilequeuesresponsetypedef)\].

<a id="listroutingprofilespaginator"></a>

## ListRoutingProfilesPaginator

Type annotations for
`session.create_client("connect").get_paginator("list_routing_profiles")`.

Can be used directly:

```python
from aiobotocore.session import get_session

from types_aiobotocore_connect.paginator import ListRoutingProfilesPaginator

session = get_session()
async with session.create_client("connect") as client:
    client: ConnectClient
    paginator: ListRoutingProfilesPaginator = client.get_paginator("list_routing_profiles")
```

Boto3 documentation:
[Connect.Paginator.ListRoutingProfiles](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Paginator.ListRoutingProfiles)

Arguments for `ListRoutingProfilesPaginator.paginate` method:

- `InstanceId`: `str` *(required)*
- `PaginationConfig`:
  [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)

`ListRoutingProfilesPaginator.paginate` returns
`AsyncIterator`\[[ListRoutingProfilesResponseTypeDef](./type_defs.md#listroutingprofilesresponsetypedef)\].

<a id="listsecuritykeyspaginator"></a>

## ListSecurityKeysPaginator

Type annotations for
`session.create_client("connect").get_paginator("list_security_keys")`.

Can be used directly:

```python
from aiobotocore.session import get_session

from types_aiobotocore_connect.paginator import ListSecurityKeysPaginator

session = get_session()
async with session.create_client("connect") as client:
    client: ConnectClient
    paginator: ListSecurityKeysPaginator = client.get_paginator("list_security_keys")
```

Boto3 documentation:
[Connect.Paginator.ListSecurityKeys](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Paginator.ListSecurityKeys)

Arguments for `ListSecurityKeysPaginator.paginate` method:

- `InstanceId`: `str` *(required)*
- `PaginationConfig`:
  [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)

`ListSecurityKeysPaginator.paginate` returns
`AsyncIterator`\[[ListSecurityKeysResponseTypeDef](./type_defs.md#listsecuritykeysresponsetypedef)\].

<a id="listsecurityprofilepermissionspaginator"></a>

## ListSecurityProfilePermissionsPaginator

Type annotations for
`session.create_client("connect").get_paginator("list_security_profile_permissions")`.

Can be used directly:

```python
from aiobotocore.session import get_session

from types_aiobotocore_connect.paginator import ListSecurityProfilePermissionsPaginator

session = get_session()
async with session.create_client("connect") as client:
    client: ConnectClient
    paginator: ListSecurityProfilePermissionsPaginator = client.get_paginator("list_security_profile_permissions")
```

Boto3 documentation:
[Connect.Paginator.ListSecurityProfilePermissions](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Paginator.ListSecurityProfilePermissions)

Arguments for `ListSecurityProfilePermissionsPaginator.paginate` method:

- `SecurityProfileId`: `str` *(required)*
- `InstanceId`: `str` *(required)*
- `PaginationConfig`:
  [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)

`ListSecurityProfilePermissionsPaginator.paginate` returns
`AsyncIterator`\[[ListSecurityProfilePermissionsResponseTypeDef](./type_defs.md#listsecurityprofilepermissionsresponsetypedef)\].

<a id="listsecurityprofilespaginator"></a>

## ListSecurityProfilesPaginator

Type annotations for
`session.create_client("connect").get_paginator("list_security_profiles")`.

Can be used directly:

```python
from aiobotocore.session import get_session

from types_aiobotocore_connect.paginator import ListSecurityProfilesPaginator

session = get_session()
async with session.create_client("connect") as client:
    client: ConnectClient
    paginator: ListSecurityProfilesPaginator = client.get_paginator("list_security_profiles")
```

Boto3 documentation:
[Connect.Paginator.ListSecurityProfiles](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Paginator.ListSecurityProfiles)

Arguments for `ListSecurityProfilesPaginator.paginate` method:

- `InstanceId`: `str` *(required)*
- `PaginationConfig`:
  [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)

`ListSecurityProfilesPaginator.paginate` returns
`AsyncIterator`\[[ListSecurityProfilesResponseTypeDef](./type_defs.md#listsecurityprofilesresponsetypedef)\].

<a id="listusecasespaginator"></a>

## ListUseCasesPaginator

Type annotations for
`session.create_client("connect").get_paginator("list_use_cases")`.

Can be used directly:

```python
from aiobotocore.session import get_session

from types_aiobotocore_connect.paginator import ListUseCasesPaginator

session = get_session()
async with session.create_client("connect") as client:
    client: ConnectClient
    paginator: ListUseCasesPaginator = client.get_paginator("list_use_cases")
```

Boto3 documentation:
[Connect.Paginator.ListUseCases](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Paginator.ListUseCases)

Arguments for `ListUseCasesPaginator.paginate` method:

- `InstanceId`: `str` *(required)*
- `IntegrationAssociationId`: `str` *(required)*
- `PaginationConfig`:
  [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)

`ListUseCasesPaginator.paginate` returns
`AsyncIterator`\[[ListUseCasesResponseTypeDef](./type_defs.md#listusecasesresponsetypedef)\].

<a id="listuserhierarchygroupspaginator"></a>

## ListUserHierarchyGroupsPaginator

Type annotations for
`session.create_client("connect").get_paginator("list_user_hierarchy_groups")`.

Can be used directly:

```python
from aiobotocore.session import get_session

from types_aiobotocore_connect.paginator import ListUserHierarchyGroupsPaginator

session = get_session()
async with session.create_client("connect") as client:
    client: ConnectClient
    paginator: ListUserHierarchyGroupsPaginator = client.get_paginator("list_user_hierarchy_groups")
```

Boto3 documentation:
[Connect.Paginator.ListUserHierarchyGroups](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Paginator.ListUserHierarchyGroups)

Arguments for `ListUserHierarchyGroupsPaginator.paginate` method:

- `InstanceId`: `str` *(required)*
- `PaginationConfig`:
  [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)

`ListUserHierarchyGroupsPaginator.paginate` returns
`AsyncIterator`\[[ListUserHierarchyGroupsResponseTypeDef](./type_defs.md#listuserhierarchygroupsresponsetypedef)\].

<a id="listuserspaginator"></a>

## ListUsersPaginator

Type annotations for
`session.create_client("connect").get_paginator("list_users")`.

Can be used directly:

```python
from aiobotocore.session import get_session

from types_aiobotocore_connect.paginator import ListUsersPaginator

session = get_session()
async with session.create_client("connect") as client:
    client: ConnectClient
    paginator: ListUsersPaginator = client.get_paginator("list_users")
```

Boto3 documentation:
[Connect.Paginator.ListUsers](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Paginator.ListUsers)

Arguments for `ListUsersPaginator.paginate` method:

- `InstanceId`: `str` *(required)*
- `PaginationConfig`:
  [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)

`ListUsersPaginator.paginate` returns
`AsyncIterator`\[[ListUsersResponseTypeDef](./type_defs.md#listusersresponsetypedef)\].

<a id="searchvocabulariespaginator"></a>

## SearchVocabulariesPaginator

Type annotations for
`session.create_client("connect").get_paginator("search_vocabularies")`.

Can be used directly:

```python
from aiobotocore.session import get_session

from types_aiobotocore_connect.paginator import SearchVocabulariesPaginator

session = get_session()
async with session.create_client("connect") as client:
    client: ConnectClient
    paginator: SearchVocabulariesPaginator = client.get_paginator("search_vocabularies")
```

Boto3 documentation:
[Connect.Paginator.SearchVocabularies](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Paginator.SearchVocabularies)

Arguments for `SearchVocabulariesPaginator.paginate` method:

- `InstanceId`: `str` *(required)*
- `State`: [VocabularyStateType](./literals.md#vocabularystatetype)
- `NameStartsWith`: `str`
- `LanguageCode`:
  [VocabularyLanguageCodeType](./literals.md#vocabularylanguagecodetype)
- `PaginationConfig`:
  [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)

`SearchVocabulariesPaginator.paginate` returns
`AsyncIterator`\[[SearchVocabulariesResponseTypeDef](./type_defs.md#searchvocabulariesresponsetypedef)\].
