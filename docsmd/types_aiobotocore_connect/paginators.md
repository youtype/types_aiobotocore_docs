# Paginators

> [Index](../README.md) > [Connect](./README.md) > Paginators

!!! note ""

    Auto-generated documentation for [Connect](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#connect)
    type annotations stubs module [types-aiobotocore-connect](https://pypi.org/project/types-aiobotocore-connect/).

## GetMetricDataPaginator

Type annotations and code completion for `#!python session.create_client("connect").get_paginator("get_metric_data")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect/paginator/GetMetricData.html#Connect.Paginator.GetMetricData)

```python
# GetMetricDataPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_connect.paginator import GetMetricDataPaginator

session = get_session()
async with session.create_client("connect") as client:  # (1)
    paginator: GetMetricDataPaginator = client.get_paginator("get_metric_data")  # (2)
    async for item in paginator.paginate(...):
        item: GetMetricDataResponseTypeDef
        print(item)  # (3)
```

1. client: [ConnectClient](./client.md)
2. paginator: [GetMetricDataPaginator](./paginators.md#getmetricdatapaginator)
3. item: `AioPageIterator[GetMetricDataResponseTypeDef]`


### paginate

Type annotations and code completion for `#!python GetMetricDataPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    InstanceId: str,
    StartTime: TimestampTypeDef,
    EndTime: TimestampTypeDef,
    Filters: FiltersTypeDef,  # (1)
    HistoricalMetrics: Sequence[HistoricalMetricTypeDef],  # (2)
    Groupings: Sequence[GroupingType] = ...,  # (3)
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (4)
) -> aiobotocore.paginate.AioPageIterator[GetMetricDataResponseTypeDef]:  # (5)
    ...
```

1. See [:material-code-braces: FiltersTypeDef](./type_defs.md#filterstypedef)
2. See `Sequence[HistoricalMetricTypeDef]`
3. See `Sequence[GroupingType]`
4. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
5. See `AioPageIterator[GetMetricDataResponseTypeDef]`


```python
# paginate method usage example with argument unpacking

kwargs: GetMetricDataRequestPaginateTypeDef = {  # (1)
    "InstanceId": ...,
    "StartTime": ...,
    "EndTime": ...,
    "Filters": ...,
    "HistoricalMetrics": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: GetMetricDataRequestPaginateTypeDef](./type_defs.md#getmetricdatarequestpaginatetypedef)
## ListAgentStatusesPaginator

Type annotations and code completion for `#!python session.create_client("connect").get_paginator("list_agent_statuses")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect/paginator/ListAgentStatuses.html#Connect.Paginator.ListAgentStatuses)

```python
# ListAgentStatusesPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_connect.paginator import ListAgentStatusesPaginator

session = get_session()
async with session.create_client("connect") as client:  # (1)
    paginator: ListAgentStatusesPaginator = client.get_paginator("list_agent_statuses")  # (2)
    async for item in paginator.paginate(...):
        item: ListAgentStatusResponseTypeDef
        print(item)  # (3)
```

1. client: [ConnectClient](./client.md)
2. paginator: [ListAgentStatusesPaginator](./paginators.md#listagentstatusespaginator)
3. item: `AioPageIterator[ListAgentStatusResponseTypeDef]`


### paginate

Type annotations and code completion for `#!python ListAgentStatusesPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    InstanceId: str,
    AgentStatusTypes: Sequence[AgentStatusTypeType] = ...,  # (1)
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (2)
) -> aiobotocore.paginate.AioPageIterator[ListAgentStatusResponseTypeDef]:  # (3)
    ...
```

1. See `Sequence[AgentStatusTypeType]`
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
3. See `AioPageIterator[ListAgentStatusResponseTypeDef]`


```python
# paginate method usage example with argument unpacking

kwargs: ListAgentStatusRequestPaginateTypeDef = {  # (1)
    "InstanceId": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListAgentStatusRequestPaginateTypeDef](./type_defs.md#listagentstatusrequestpaginatetypedef)
## ListApprovedOriginsPaginator

Type annotations and code completion for `#!python session.create_client("connect").get_paginator("list_approved_origins")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect/paginator/ListApprovedOrigins.html#Connect.Paginator.ListApprovedOrigins)

```python
# ListApprovedOriginsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_connect.paginator import ListApprovedOriginsPaginator

session = get_session()
async with session.create_client("connect") as client:  # (1)
    paginator: ListApprovedOriginsPaginator = client.get_paginator("list_approved_origins")  # (2)
    async for item in paginator.paginate(...):
        item: ListApprovedOriginsResponseTypeDef
        print(item)  # (3)
```

1. client: [ConnectClient](./client.md)
2. paginator: [ListApprovedOriginsPaginator](./paginators.md#listapprovedoriginspaginator)
3. item: `AioPageIterator[ListApprovedOriginsResponseTypeDef]`


### paginate

Type annotations and code completion for `#!python ListApprovedOriginsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    InstanceId: str,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> aiobotocore.paginate.AioPageIterator[ListApprovedOriginsResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
2. See `AioPageIterator[ListApprovedOriginsResponseTypeDef]`


```python
# paginate method usage example with argument unpacking

kwargs: ListApprovedOriginsRequestPaginateTypeDef = {  # (1)
    "InstanceId": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListApprovedOriginsRequestPaginateTypeDef](./type_defs.md#listapprovedoriginsrequestpaginatetypedef)
## ListAuthenticationProfilesPaginator

Type annotations and code completion for `#!python session.create_client("connect").get_paginator("list_authentication_profiles")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect/paginator/ListAuthenticationProfiles.html#Connect.Paginator.ListAuthenticationProfiles)

```python
# ListAuthenticationProfilesPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_connect.paginator import ListAuthenticationProfilesPaginator

session = get_session()
async with session.create_client("connect") as client:  # (1)
    paginator: ListAuthenticationProfilesPaginator = client.get_paginator("list_authentication_profiles")  # (2)
    async for item in paginator.paginate(...):
        item: ListAuthenticationProfilesResponseTypeDef
        print(item)  # (3)
```

1. client: [ConnectClient](./client.md)
2. paginator: [ListAuthenticationProfilesPaginator](./paginators.md#listauthenticationprofilespaginator)
3. item: `AioPageIterator[ListAuthenticationProfilesResponseTypeDef]`


### paginate

Type annotations and code completion for `#!python ListAuthenticationProfilesPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    InstanceId: str,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> aiobotocore.paginate.AioPageIterator[ListAuthenticationProfilesResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
2. See `AioPageIterator[ListAuthenticationProfilesResponseTypeDef]`


```python
# paginate method usage example with argument unpacking

kwargs: ListAuthenticationProfilesRequestPaginateTypeDef = {  # (1)
    "InstanceId": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListAuthenticationProfilesRequestPaginateTypeDef](./type_defs.md#listauthenticationprofilesrequestpaginatetypedef)
## ListBotsPaginator

Type annotations and code completion for `#!python session.create_client("connect").get_paginator("list_bots")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect/paginator/ListBots.html#Connect.Paginator.ListBots)

```python
# ListBotsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_connect.paginator import ListBotsPaginator

session = get_session()
async with session.create_client("connect") as client:  # (1)
    paginator: ListBotsPaginator = client.get_paginator("list_bots")  # (2)
    async for item in paginator.paginate(...):
        item: ListBotsResponseTypeDef
        print(item)  # (3)
```

1. client: [ConnectClient](./client.md)
2. paginator: [ListBotsPaginator](./paginators.md#listbotspaginator)
3. item: `AioPageIterator[ListBotsResponseTypeDef]`


### paginate

Type annotations and code completion for `#!python ListBotsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    InstanceId: str,
    LexVersion: LexVersionType,  # (1)
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (2)
) -> aiobotocore.paginate.AioPageIterator[ListBotsResponseTypeDef]:  # (3)
    ...
```

1. See [:material-code-brackets: LexVersionType](./literals.md#lexversiontype)
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
3. See `AioPageIterator[ListBotsResponseTypeDef]`


```python
# paginate method usage example with argument unpacking

kwargs: ListBotsRequestPaginateTypeDef = {  # (1)
    "InstanceId": ...,
    "LexVersion": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListBotsRequestPaginateTypeDef](./type_defs.md#listbotsrequestpaginatetypedef)
## ListChildHoursOfOperationsPaginator

Type annotations and code completion for `#!python session.create_client("connect").get_paginator("list_child_hours_of_operations")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect/paginator/ListChildHoursOfOperations.html#Connect.Paginator.ListChildHoursOfOperations)

```python
# ListChildHoursOfOperationsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_connect.paginator import ListChildHoursOfOperationsPaginator

session = get_session()
async with session.create_client("connect") as client:  # (1)
    paginator: ListChildHoursOfOperationsPaginator = client.get_paginator("list_child_hours_of_operations")  # (2)
    async for item in paginator.paginate(...):
        item: ListChildHoursOfOperationsResponseTypeDef
        print(item)  # (3)
```

1. client: [ConnectClient](./client.md)
2. paginator: [ListChildHoursOfOperationsPaginator](./paginators.md#listchildhoursofoperationspaginator)
3. item: `AioPageIterator[ListChildHoursOfOperationsResponseTypeDef]`


### paginate

Type annotations and code completion for `#!python ListChildHoursOfOperationsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    InstanceId: str,
    HoursOfOperationId: str,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> aiobotocore.paginate.AioPageIterator[ListChildHoursOfOperationsResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
2. See `AioPageIterator[ListChildHoursOfOperationsResponseTypeDef]`


```python
# paginate method usage example with argument unpacking

kwargs: ListChildHoursOfOperationsRequestPaginateTypeDef = {  # (1)
    "InstanceId": ...,
    "HoursOfOperationId": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListChildHoursOfOperationsRequestPaginateTypeDef](./type_defs.md#listchildhoursofoperationsrequestpaginatetypedef)
## ListContactEvaluationsPaginator

Type annotations and code completion for `#!python session.create_client("connect").get_paginator("list_contact_evaluations")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect/paginator/ListContactEvaluations.html#Connect.Paginator.ListContactEvaluations)

```python
# ListContactEvaluationsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_connect.paginator import ListContactEvaluationsPaginator

session = get_session()
async with session.create_client("connect") as client:  # (1)
    paginator: ListContactEvaluationsPaginator = client.get_paginator("list_contact_evaluations")  # (2)
    async for item in paginator.paginate(...):
        item: ListContactEvaluationsResponseTypeDef
        print(item)  # (3)
```

1. client: [ConnectClient](./client.md)
2. paginator: [ListContactEvaluationsPaginator](./paginators.md#listcontactevaluationspaginator)
3. item: `AioPageIterator[ListContactEvaluationsResponseTypeDef]`


### paginate

Type annotations and code completion for `#!python ListContactEvaluationsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    InstanceId: str,
    ContactId: str,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> aiobotocore.paginate.AioPageIterator[ListContactEvaluationsResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
2. See `AioPageIterator[ListContactEvaluationsResponseTypeDef]`


```python
# paginate method usage example with argument unpacking

kwargs: ListContactEvaluationsRequestPaginateTypeDef = {  # (1)
    "InstanceId": ...,
    "ContactId": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListContactEvaluationsRequestPaginateTypeDef](./type_defs.md#listcontactevaluationsrequestpaginatetypedef)
## ListContactFlowModuleAliasesPaginator

Type annotations and code completion for `#!python session.create_client("connect").get_paginator("list_contact_flow_module_aliases")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect/paginator/ListContactFlowModuleAliases.html#Connect.Paginator.ListContactFlowModuleAliases)

```python
# ListContactFlowModuleAliasesPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_connect.paginator import ListContactFlowModuleAliasesPaginator

session = get_session()
async with session.create_client("connect") as client:  # (1)
    paginator: ListContactFlowModuleAliasesPaginator = client.get_paginator("list_contact_flow_module_aliases")  # (2)
    async for item in paginator.paginate(...):
        item: ListContactFlowModuleAliasesResponseTypeDef
        print(item)  # (3)
```

1. client: [ConnectClient](./client.md)
2. paginator: [ListContactFlowModuleAliasesPaginator](./paginators.md#listcontactflowmodulealiasespaginator)
3. item: `AioPageIterator[ListContactFlowModuleAliasesResponseTypeDef]`


### paginate

Type annotations and code completion for `#!python ListContactFlowModuleAliasesPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    InstanceId: str,
    ContactFlowModuleId: str,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> aiobotocore.paginate.AioPageIterator[ListContactFlowModuleAliasesResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
2. See `AioPageIterator[ListContactFlowModuleAliasesResponseTypeDef]`


```python
# paginate method usage example with argument unpacking

kwargs: ListContactFlowModuleAliasesRequestPaginateTypeDef = {  # (1)
    "InstanceId": ...,
    "ContactFlowModuleId": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListContactFlowModuleAliasesRequestPaginateTypeDef](./type_defs.md#listcontactflowmodulealiasesrequestpaginatetypedef)
## ListContactFlowModuleVersionsPaginator

Type annotations and code completion for `#!python session.create_client("connect").get_paginator("list_contact_flow_module_versions")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect/paginator/ListContactFlowModuleVersions.html#Connect.Paginator.ListContactFlowModuleVersions)

```python
# ListContactFlowModuleVersionsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_connect.paginator import ListContactFlowModuleVersionsPaginator

session = get_session()
async with session.create_client("connect") as client:  # (1)
    paginator: ListContactFlowModuleVersionsPaginator = client.get_paginator("list_contact_flow_module_versions")  # (2)
    async for item in paginator.paginate(...):
        item: ListContactFlowModuleVersionsResponseTypeDef
        print(item)  # (3)
```

1. client: [ConnectClient](./client.md)
2. paginator: [ListContactFlowModuleVersionsPaginator](./paginators.md#listcontactflowmoduleversionspaginator)
3. item: `AioPageIterator[ListContactFlowModuleVersionsResponseTypeDef]`


### paginate

Type annotations and code completion for `#!python ListContactFlowModuleVersionsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    InstanceId: str,
    ContactFlowModuleId: str,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> aiobotocore.paginate.AioPageIterator[ListContactFlowModuleVersionsResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
2. See `AioPageIterator[ListContactFlowModuleVersionsResponseTypeDef]`


```python
# paginate method usage example with argument unpacking

kwargs: ListContactFlowModuleVersionsRequestPaginateTypeDef = {  # (1)
    "InstanceId": ...,
    "ContactFlowModuleId": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListContactFlowModuleVersionsRequestPaginateTypeDef](./type_defs.md#listcontactflowmoduleversionsrequestpaginatetypedef)
## ListContactFlowModulesPaginator

Type annotations and code completion for `#!python session.create_client("connect").get_paginator("list_contact_flow_modules")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect/paginator/ListContactFlowModules.html#Connect.Paginator.ListContactFlowModules)

```python
# ListContactFlowModulesPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_connect.paginator import ListContactFlowModulesPaginator

session = get_session()
async with session.create_client("connect") as client:  # (1)
    paginator: ListContactFlowModulesPaginator = client.get_paginator("list_contact_flow_modules")  # (2)
    async for item in paginator.paginate(...):
        item: ListContactFlowModulesResponseTypeDef
        print(item)  # (3)
```

1. client: [ConnectClient](./client.md)
2. paginator: [ListContactFlowModulesPaginator](./paginators.md#listcontactflowmodulespaginator)
3. item: `AioPageIterator[ListContactFlowModulesResponseTypeDef]`


### paginate

Type annotations and code completion for `#!python ListContactFlowModulesPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    InstanceId: str,
    ContactFlowModuleState: ContactFlowModuleStateType = ...,  # (1)
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (2)
) -> aiobotocore.paginate.AioPageIterator[ListContactFlowModulesResponseTypeDef]:  # (3)
    ...
```

1. See [:material-code-brackets: ContactFlowModuleStateType](./literals.md#contactflowmodulestatetype)
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
3. See `AioPageIterator[ListContactFlowModulesResponseTypeDef]`


```python
# paginate method usage example with argument unpacking

kwargs: ListContactFlowModulesRequestPaginateTypeDef = {  # (1)
    "InstanceId": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListContactFlowModulesRequestPaginateTypeDef](./type_defs.md#listcontactflowmodulesrequestpaginatetypedef)
## ListContactFlowVersionsPaginator

Type annotations and code completion for `#!python session.create_client("connect").get_paginator("list_contact_flow_versions")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect/paginator/ListContactFlowVersions.html#Connect.Paginator.ListContactFlowVersions)

```python
# ListContactFlowVersionsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_connect.paginator import ListContactFlowVersionsPaginator

session = get_session()
async with session.create_client("connect") as client:  # (1)
    paginator: ListContactFlowVersionsPaginator = client.get_paginator("list_contact_flow_versions")  # (2)
    async for item in paginator.paginate(...):
        item: ListContactFlowVersionsResponseTypeDef
        print(item)  # (3)
```

1. client: [ConnectClient](./client.md)
2. paginator: [ListContactFlowVersionsPaginator](./paginators.md#listcontactflowversionspaginator)
3. item: `AioPageIterator[ListContactFlowVersionsResponseTypeDef]`


### paginate

Type annotations and code completion for `#!python ListContactFlowVersionsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    InstanceId: str,
    ContactFlowId: str,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> aiobotocore.paginate.AioPageIterator[ListContactFlowVersionsResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
2. See `AioPageIterator[ListContactFlowVersionsResponseTypeDef]`


```python
# paginate method usage example with argument unpacking

kwargs: ListContactFlowVersionsRequestPaginateTypeDef = {  # (1)
    "InstanceId": ...,
    "ContactFlowId": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListContactFlowVersionsRequestPaginateTypeDef](./type_defs.md#listcontactflowversionsrequestpaginatetypedef)
## ListContactFlowsPaginator

Type annotations and code completion for `#!python session.create_client("connect").get_paginator("list_contact_flows")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect/paginator/ListContactFlows.html#Connect.Paginator.ListContactFlows)

```python
# ListContactFlowsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_connect.paginator import ListContactFlowsPaginator

session = get_session()
async with session.create_client("connect") as client:  # (1)
    paginator: ListContactFlowsPaginator = client.get_paginator("list_contact_flows")  # (2)
    async for item in paginator.paginate(...):
        item: ListContactFlowsResponseTypeDef
        print(item)  # (3)
```

1. client: [ConnectClient](./client.md)
2. paginator: [ListContactFlowsPaginator](./paginators.md#listcontactflowspaginator)
3. item: `AioPageIterator[ListContactFlowsResponseTypeDef]`


### paginate

Type annotations and code completion for `#!python ListContactFlowsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    InstanceId: str,
    ContactFlowTypes: Sequence[ContactFlowTypeType] = ...,  # (1)
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (2)
) -> aiobotocore.paginate.AioPageIterator[ListContactFlowsResponseTypeDef]:  # (3)
    ...
```

1. See `Sequence[ContactFlowTypeType]`
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
3. See `AioPageIterator[ListContactFlowsResponseTypeDef]`


```python
# paginate method usage example with argument unpacking

kwargs: ListContactFlowsRequestPaginateTypeDef = {  # (1)
    "InstanceId": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListContactFlowsRequestPaginateTypeDef](./type_defs.md#listcontactflowsrequestpaginatetypedef)
## ListContactReferencesPaginator

Type annotations and code completion for `#!python session.create_client("connect").get_paginator("list_contact_references")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect/paginator/ListContactReferences.html#Connect.Paginator.ListContactReferences)

```python
# ListContactReferencesPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_connect.paginator import ListContactReferencesPaginator

session = get_session()
async with session.create_client("connect") as client:  # (1)
    paginator: ListContactReferencesPaginator = client.get_paginator("list_contact_references")  # (2)
    async for item in paginator.paginate(...):
        item: ListContactReferencesResponseTypeDef
        print(item)  # (3)
```

1. client: [ConnectClient](./client.md)
2. paginator: [ListContactReferencesPaginator](./paginators.md#listcontactreferencespaginator)
3. item: `AioPageIterator[ListContactReferencesResponseTypeDef]`


### paginate

Type annotations and code completion for `#!python ListContactReferencesPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    InstanceId: str,
    ContactId: str,
    ReferenceTypes: Sequence[ReferenceTypeType],  # (1)
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (2)
) -> aiobotocore.paginate.AioPageIterator[ListContactReferencesResponseTypeDef]:  # (3)
    ...
```

1. See `Sequence[ReferenceTypeType]`
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
3. See `AioPageIterator[ListContactReferencesResponseTypeDef]`


```python
# paginate method usage example with argument unpacking

kwargs: ListContactReferencesRequestPaginateTypeDef = {  # (1)
    "InstanceId": ...,
    "ContactId": ...,
    "ReferenceTypes": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListContactReferencesRequestPaginateTypeDef](./type_defs.md#listcontactreferencesrequestpaginatetypedef)
## ListDataTableAttributesPaginator

Type annotations and code completion for `#!python session.create_client("connect").get_paginator("list_data_table_attributes")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect/paginator/ListDataTableAttributes.html#Connect.Paginator.ListDataTableAttributes)

```python
# ListDataTableAttributesPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_connect.paginator import ListDataTableAttributesPaginator

session = get_session()
async with session.create_client("connect") as client:  # (1)
    paginator: ListDataTableAttributesPaginator = client.get_paginator("list_data_table_attributes")  # (2)
    async for item in paginator.paginate(...):
        item: ListDataTableAttributesResponseTypeDef
        print(item)  # (3)
```

1. client: [ConnectClient](./client.md)
2. paginator: [ListDataTableAttributesPaginator](./paginators.md#listdatatableattributespaginator)
3. item: `AioPageIterator[ListDataTableAttributesResponseTypeDef]`


### paginate

Type annotations and code completion for `#!python ListDataTableAttributesPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    InstanceId: str,
    DataTableId: str,
    AttributeIds: Sequence[str] = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> aiobotocore.paginate.AioPageIterator[ListDataTableAttributesResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
2. See `AioPageIterator[ListDataTableAttributesResponseTypeDef]`


```python
# paginate method usage example with argument unpacking

kwargs: ListDataTableAttributesRequestPaginateTypeDef = {  # (1)
    "InstanceId": ...,
    "DataTableId": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListDataTableAttributesRequestPaginateTypeDef](./type_defs.md#listdatatableattributesrequestpaginatetypedef)
## ListDataTablePrimaryValuesPaginator

Type annotations and code completion for `#!python session.create_client("connect").get_paginator("list_data_table_primary_values")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect/paginator/ListDataTablePrimaryValues.html#Connect.Paginator.ListDataTablePrimaryValues)

```python
# ListDataTablePrimaryValuesPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_connect.paginator import ListDataTablePrimaryValuesPaginator

session = get_session()
async with session.create_client("connect") as client:  # (1)
    paginator: ListDataTablePrimaryValuesPaginator = client.get_paginator("list_data_table_primary_values")  # (2)
    async for item in paginator.paginate(...):
        item: ListDataTablePrimaryValuesResponseTypeDef
        print(item)  # (3)
```

1. client: [ConnectClient](./client.md)
2. paginator: [ListDataTablePrimaryValuesPaginator](./paginators.md#listdatatableprimaryvaluespaginator)
3. item: `AioPageIterator[ListDataTablePrimaryValuesResponseTypeDef]`


### paginate

Type annotations and code completion for `#!python ListDataTablePrimaryValuesPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    InstanceId: str,
    DataTableId: str,
    RecordIds: Sequence[str] = ...,
    PrimaryAttributeValues: Sequence[PrimaryAttributeValueFilterTypeDef] = ...,  # (1)
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (2)
) -> aiobotocore.paginate.AioPageIterator[ListDataTablePrimaryValuesResponseTypeDef]:  # (3)
    ...
```

1. See `Sequence[PrimaryAttributeValueFilterTypeDef]`
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
3. See `AioPageIterator[ListDataTablePrimaryValuesResponseTypeDef]`


```python
# paginate method usage example with argument unpacking

kwargs: ListDataTablePrimaryValuesRequestPaginateTypeDef = {  # (1)
    "InstanceId": ...,
    "DataTableId": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListDataTablePrimaryValuesRequestPaginateTypeDef](./type_defs.md#listdatatableprimaryvaluesrequestpaginatetypedef)
## ListDataTableValuesPaginator

Type annotations and code completion for `#!python session.create_client("connect").get_paginator("list_data_table_values")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect/paginator/ListDataTableValues.html#Connect.Paginator.ListDataTableValues)

```python
# ListDataTableValuesPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_connect.paginator import ListDataTableValuesPaginator

session = get_session()
async with session.create_client("connect") as client:  # (1)
    paginator: ListDataTableValuesPaginator = client.get_paginator("list_data_table_values")  # (2)
    async for item in paginator.paginate(...):
        item: ListDataTableValuesResponseTypeDef
        print(item)  # (3)
```

1. client: [ConnectClient](./client.md)
2. paginator: [ListDataTableValuesPaginator](./paginators.md#listdatatablevaluespaginator)
3. item: `AioPageIterator[ListDataTableValuesResponseTypeDef]`


### paginate

Type annotations and code completion for `#!python ListDataTableValuesPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    InstanceId: str,
    DataTableId: str,
    RecordIds: Sequence[str] = ...,
    PrimaryAttributeValues: Sequence[PrimaryAttributeValueFilterTypeDef] = ...,  # (1)
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (2)
) -> aiobotocore.paginate.AioPageIterator[ListDataTableValuesResponseTypeDef]:  # (3)
    ...
```

1. See `Sequence[PrimaryAttributeValueFilterTypeDef]`
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
3. See `AioPageIterator[ListDataTableValuesResponseTypeDef]`


```python
# paginate method usage example with argument unpacking

kwargs: ListDataTableValuesRequestPaginateTypeDef = {  # (1)
    "InstanceId": ...,
    "DataTableId": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListDataTableValuesRequestPaginateTypeDef](./type_defs.md#listdatatablevaluesrequestpaginatetypedef)
## ListDataTablesPaginator

Type annotations and code completion for `#!python session.create_client("connect").get_paginator("list_data_tables")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect/paginator/ListDataTables.html#Connect.Paginator.ListDataTables)

```python
# ListDataTablesPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_connect.paginator import ListDataTablesPaginator

session = get_session()
async with session.create_client("connect") as client:  # (1)
    paginator: ListDataTablesPaginator = client.get_paginator("list_data_tables")  # (2)
    async for item in paginator.paginate(...):
        item: ListDataTablesResponseTypeDef
        print(item)  # (3)
```

1. client: [ConnectClient](./client.md)
2. paginator: [ListDataTablesPaginator](./paginators.md#listdatatablespaginator)
3. item: `AioPageIterator[ListDataTablesResponseTypeDef]`


### paginate

Type annotations and code completion for `#!python ListDataTablesPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    InstanceId: str,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> aiobotocore.paginate.AioPageIterator[ListDataTablesResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
2. See `AioPageIterator[ListDataTablesResponseTypeDef]`


```python
# paginate method usage example with argument unpacking

kwargs: ListDataTablesRequestPaginateTypeDef = {  # (1)
    "InstanceId": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListDataTablesRequestPaginateTypeDef](./type_defs.md#listdatatablesrequestpaginatetypedef)
## ListDefaultVocabulariesPaginator

Type annotations and code completion for `#!python session.create_client("connect").get_paginator("list_default_vocabularies")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect/paginator/ListDefaultVocabularies.html#Connect.Paginator.ListDefaultVocabularies)

```python
# ListDefaultVocabulariesPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_connect.paginator import ListDefaultVocabulariesPaginator

session = get_session()
async with session.create_client("connect") as client:  # (1)
    paginator: ListDefaultVocabulariesPaginator = client.get_paginator("list_default_vocabularies")  # (2)
    async for item in paginator.paginate(...):
        item: ListDefaultVocabulariesResponseTypeDef
        print(item)  # (3)
```

1. client: [ConnectClient](./client.md)
2. paginator: [ListDefaultVocabulariesPaginator](./paginators.md#listdefaultvocabulariespaginator)
3. item: `AioPageIterator[ListDefaultVocabulariesResponseTypeDef]`


### paginate

Type annotations and code completion for `#!python ListDefaultVocabulariesPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    InstanceId: str,
    LanguageCode: VocabularyLanguageCodeType = ...,  # (1)
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (2)
) -> aiobotocore.paginate.AioPageIterator[ListDefaultVocabulariesResponseTypeDef]:  # (3)
    ...
```

1. See [:material-code-brackets: VocabularyLanguageCodeType](./literals.md#vocabularylanguagecodetype)
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
3. See `AioPageIterator[ListDefaultVocabulariesResponseTypeDef]`


```python
# paginate method usage example with argument unpacking

kwargs: ListDefaultVocabulariesRequestPaginateTypeDef = {  # (1)
    "InstanceId": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListDefaultVocabulariesRequestPaginateTypeDef](./type_defs.md#listdefaultvocabulariesrequestpaginatetypedef)
## ListEntitySecurityProfilesPaginator

Type annotations and code completion for `#!python session.create_client("connect").get_paginator("list_entity_security_profiles")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect/paginator/ListEntitySecurityProfiles.html#Connect.Paginator.ListEntitySecurityProfiles)

```python
# ListEntitySecurityProfilesPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_connect.paginator import ListEntitySecurityProfilesPaginator

session = get_session()
async with session.create_client("connect") as client:  # (1)
    paginator: ListEntitySecurityProfilesPaginator = client.get_paginator("list_entity_security_profiles")  # (2)
    async for item in paginator.paginate(...):
        item: ListEntitySecurityProfilesResponseTypeDef
        print(item)  # (3)
```

1. client: [ConnectClient](./client.md)
2. paginator: [ListEntitySecurityProfilesPaginator](./paginators.md#listentitysecurityprofilespaginator)
3. item: `AioPageIterator[ListEntitySecurityProfilesResponseTypeDef]`


### paginate

Type annotations and code completion for `#!python ListEntitySecurityProfilesPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    InstanceId: str,
    EntityType: EntityTypeType,  # (1)
    EntityArn: str,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (2)
) -> aiobotocore.paginate.AioPageIterator[ListEntitySecurityProfilesResponseTypeDef]:  # (3)
    ...
```

1. See [:material-code-brackets: EntityTypeType](./literals.md#entitytypetype)
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
3. See `AioPageIterator[ListEntitySecurityProfilesResponseTypeDef]`


```python
# paginate method usage example with argument unpacking

kwargs: ListEntitySecurityProfilesRequestPaginateTypeDef = {  # (1)
    "InstanceId": ...,
    "EntityType": ...,
    "EntityArn": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListEntitySecurityProfilesRequestPaginateTypeDef](./type_defs.md#listentitysecurityprofilesrequestpaginatetypedef)
## ListEvaluationFormVersionsPaginator

Type annotations and code completion for `#!python session.create_client("connect").get_paginator("list_evaluation_form_versions")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect/paginator/ListEvaluationFormVersions.html#Connect.Paginator.ListEvaluationFormVersions)

```python
# ListEvaluationFormVersionsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_connect.paginator import ListEvaluationFormVersionsPaginator

session = get_session()
async with session.create_client("connect") as client:  # (1)
    paginator: ListEvaluationFormVersionsPaginator = client.get_paginator("list_evaluation_form_versions")  # (2)
    async for item in paginator.paginate(...):
        item: ListEvaluationFormVersionsResponseTypeDef
        print(item)  # (3)
```

1. client: [ConnectClient](./client.md)
2. paginator: [ListEvaluationFormVersionsPaginator](./paginators.md#listevaluationformversionspaginator)
3. item: `AioPageIterator[ListEvaluationFormVersionsResponseTypeDef]`


### paginate

Type annotations and code completion for `#!python ListEvaluationFormVersionsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    InstanceId: str,
    EvaluationFormId: str,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> aiobotocore.paginate.AioPageIterator[ListEvaluationFormVersionsResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
2. See `AioPageIterator[ListEvaluationFormVersionsResponseTypeDef]`


```python
# paginate method usage example with argument unpacking

kwargs: ListEvaluationFormVersionsRequestPaginateTypeDef = {  # (1)
    "InstanceId": ...,
    "EvaluationFormId": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListEvaluationFormVersionsRequestPaginateTypeDef](./type_defs.md#listevaluationformversionsrequestpaginatetypedef)
## ListEvaluationFormsPaginator

Type annotations and code completion for `#!python session.create_client("connect").get_paginator("list_evaluation_forms")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect/paginator/ListEvaluationForms.html#Connect.Paginator.ListEvaluationForms)

```python
# ListEvaluationFormsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_connect.paginator import ListEvaluationFormsPaginator

session = get_session()
async with session.create_client("connect") as client:  # (1)
    paginator: ListEvaluationFormsPaginator = client.get_paginator("list_evaluation_forms")  # (2)
    async for item in paginator.paginate(...):
        item: ListEvaluationFormsResponseTypeDef
        print(item)  # (3)
```

1. client: [ConnectClient](./client.md)
2. paginator: [ListEvaluationFormsPaginator](./paginators.md#listevaluationformspaginator)
3. item: `AioPageIterator[ListEvaluationFormsResponseTypeDef]`


### paginate

Type annotations and code completion for `#!python ListEvaluationFormsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    InstanceId: str,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> aiobotocore.paginate.AioPageIterator[ListEvaluationFormsResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
2. See `AioPageIterator[ListEvaluationFormsResponseTypeDef]`


```python
# paginate method usage example with argument unpacking

kwargs: ListEvaluationFormsRequestPaginateTypeDef = {  # (1)
    "InstanceId": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListEvaluationFormsRequestPaginateTypeDef](./type_defs.md#listevaluationformsrequestpaginatetypedef)
## ListFlowAssociationsPaginator

Type annotations and code completion for `#!python session.create_client("connect").get_paginator("list_flow_associations")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect/paginator/ListFlowAssociations.html#Connect.Paginator.ListFlowAssociations)

```python
# ListFlowAssociationsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_connect.paginator import ListFlowAssociationsPaginator

session = get_session()
async with session.create_client("connect") as client:  # (1)
    paginator: ListFlowAssociationsPaginator = client.get_paginator("list_flow_associations")  # (2)
    async for item in paginator.paginate(...):
        item: ListFlowAssociationsResponseTypeDef
        print(item)  # (3)
```

1. client: [ConnectClient](./client.md)
2. paginator: [ListFlowAssociationsPaginator](./paginators.md#listflowassociationspaginator)
3. item: `AioPageIterator[ListFlowAssociationsResponseTypeDef]`


### paginate

Type annotations and code completion for `#!python ListFlowAssociationsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    InstanceId: str,
    ResourceType: ListFlowAssociationResourceTypeType = ...,  # (1)
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (2)
) -> aiobotocore.paginate.AioPageIterator[ListFlowAssociationsResponseTypeDef]:  # (3)
    ...
```

1. See [:material-code-brackets: ListFlowAssociationResourceTypeType](./literals.md#listflowassociationresourcetypetype)
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
3. See `AioPageIterator[ListFlowAssociationsResponseTypeDef]`


```python
# paginate method usage example with argument unpacking

kwargs: ListFlowAssociationsRequestPaginateTypeDef = {  # (1)
    "InstanceId": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListFlowAssociationsRequestPaginateTypeDef](./type_defs.md#listflowassociationsrequestpaginatetypedef)
## ListHoursOfOperationOverridesPaginator

Type annotations and code completion for `#!python session.create_client("connect").get_paginator("list_hours_of_operation_overrides")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect/paginator/ListHoursOfOperationOverrides.html#Connect.Paginator.ListHoursOfOperationOverrides)

```python
# ListHoursOfOperationOverridesPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_connect.paginator import ListHoursOfOperationOverridesPaginator

session = get_session()
async with session.create_client("connect") as client:  # (1)
    paginator: ListHoursOfOperationOverridesPaginator = client.get_paginator("list_hours_of_operation_overrides")  # (2)
    async for item in paginator.paginate(...):
        item: ListHoursOfOperationOverridesResponseTypeDef
        print(item)  # (3)
```

1. client: [ConnectClient](./client.md)
2. paginator: [ListHoursOfOperationOverridesPaginator](./paginators.md#listhoursofoperationoverridespaginator)
3. item: `AioPageIterator[ListHoursOfOperationOverridesResponseTypeDef]`


### paginate

Type annotations and code completion for `#!python ListHoursOfOperationOverridesPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    InstanceId: str,
    HoursOfOperationId: str,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> aiobotocore.paginate.AioPageIterator[ListHoursOfOperationOverridesResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
2. See `AioPageIterator[ListHoursOfOperationOverridesResponseTypeDef]`


```python
# paginate method usage example with argument unpacking

kwargs: ListHoursOfOperationOverridesRequestPaginateTypeDef = {  # (1)
    "InstanceId": ...,
    "HoursOfOperationId": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListHoursOfOperationOverridesRequestPaginateTypeDef](./type_defs.md#listhoursofoperationoverridesrequestpaginatetypedef)
## ListHoursOfOperationsPaginator

Type annotations and code completion for `#!python session.create_client("connect").get_paginator("list_hours_of_operations")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect/paginator/ListHoursOfOperations.html#Connect.Paginator.ListHoursOfOperations)

```python
# ListHoursOfOperationsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_connect.paginator import ListHoursOfOperationsPaginator

session = get_session()
async with session.create_client("connect") as client:  # (1)
    paginator: ListHoursOfOperationsPaginator = client.get_paginator("list_hours_of_operations")  # (2)
    async for item in paginator.paginate(...):
        item: ListHoursOfOperationsResponseTypeDef
        print(item)  # (3)
```

1. client: [ConnectClient](./client.md)
2. paginator: [ListHoursOfOperationsPaginator](./paginators.md#listhoursofoperationspaginator)
3. item: `AioPageIterator[ListHoursOfOperationsResponseTypeDef]`


### paginate

Type annotations and code completion for `#!python ListHoursOfOperationsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    InstanceId: str,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> aiobotocore.paginate.AioPageIterator[ListHoursOfOperationsResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
2. See `AioPageIterator[ListHoursOfOperationsResponseTypeDef]`


```python
# paginate method usage example with argument unpacking

kwargs: ListHoursOfOperationsRequestPaginateTypeDef = {  # (1)
    "InstanceId": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListHoursOfOperationsRequestPaginateTypeDef](./type_defs.md#listhoursofoperationsrequestpaginatetypedef)
## ListInstanceAttributesPaginator

Type annotations and code completion for `#!python session.create_client("connect").get_paginator("list_instance_attributes")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect/paginator/ListInstanceAttributes.html#Connect.Paginator.ListInstanceAttributes)

```python
# ListInstanceAttributesPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_connect.paginator import ListInstanceAttributesPaginator

session = get_session()
async with session.create_client("connect") as client:  # (1)
    paginator: ListInstanceAttributesPaginator = client.get_paginator("list_instance_attributes")  # (2)
    async for item in paginator.paginate(...):
        item: ListInstanceAttributesResponseTypeDef
        print(item)  # (3)
```

1. client: [ConnectClient](./client.md)
2. paginator: [ListInstanceAttributesPaginator](./paginators.md#listinstanceattributespaginator)
3. item: `AioPageIterator[ListInstanceAttributesResponseTypeDef]`


### paginate

Type annotations and code completion for `#!python ListInstanceAttributesPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    InstanceId: str,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> aiobotocore.paginate.AioPageIterator[ListInstanceAttributesResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
2. See `AioPageIterator[ListInstanceAttributesResponseTypeDef]`


```python
# paginate method usage example with argument unpacking

kwargs: ListInstanceAttributesRequestPaginateTypeDef = {  # (1)
    "InstanceId": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListInstanceAttributesRequestPaginateTypeDef](./type_defs.md#listinstanceattributesrequestpaginatetypedef)
## ListInstanceStorageConfigsPaginator

Type annotations and code completion for `#!python session.create_client("connect").get_paginator("list_instance_storage_configs")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect/paginator/ListInstanceStorageConfigs.html#Connect.Paginator.ListInstanceStorageConfigs)

```python
# ListInstanceStorageConfigsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_connect.paginator import ListInstanceStorageConfigsPaginator

session = get_session()
async with session.create_client("connect") as client:  # (1)
    paginator: ListInstanceStorageConfigsPaginator = client.get_paginator("list_instance_storage_configs")  # (2)
    async for item in paginator.paginate(...):
        item: ListInstanceStorageConfigsResponseTypeDef
        print(item)  # (3)
```

1. client: [ConnectClient](./client.md)
2. paginator: [ListInstanceStorageConfigsPaginator](./paginators.md#listinstancestorageconfigspaginator)
3. item: `AioPageIterator[ListInstanceStorageConfigsResponseTypeDef]`


### paginate

Type annotations and code completion for `#!python ListInstanceStorageConfigsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    InstanceId: str,
    ResourceType: InstanceStorageResourceTypeType,  # (1)
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (2)
) -> aiobotocore.paginate.AioPageIterator[ListInstanceStorageConfigsResponseTypeDef]:  # (3)
    ...
```

1. See [:material-code-brackets: InstanceStorageResourceTypeType](./literals.md#instancestorageresourcetypetype)
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
3. See `AioPageIterator[ListInstanceStorageConfigsResponseTypeDef]`


```python
# paginate method usage example with argument unpacking

kwargs: ListInstanceStorageConfigsRequestPaginateTypeDef = {  # (1)
    "InstanceId": ...,
    "ResourceType": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListInstanceStorageConfigsRequestPaginateTypeDef](./type_defs.md#listinstancestorageconfigsrequestpaginatetypedef)
## ListInstancesPaginator

Type annotations and code completion for `#!python session.create_client("connect").get_paginator("list_instances")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect/paginator/ListInstances.html#Connect.Paginator.ListInstances)

```python
# ListInstancesPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_connect.paginator import ListInstancesPaginator

session = get_session()
async with session.create_client("connect") as client:  # (1)
    paginator: ListInstancesPaginator = client.get_paginator("list_instances")  # (2)
    async for item in paginator.paginate(...):
        item: ListInstancesResponseTypeDef
        print(item)  # (3)
```

1. client: [ConnectClient](./client.md)
2. paginator: [ListInstancesPaginator](./paginators.md#listinstancespaginator)
3. item: `AioPageIterator[ListInstancesResponseTypeDef]`


### paginate

Type annotations and code completion for `#!python ListInstancesPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> aiobotocore.paginate.AioPageIterator[ListInstancesResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
2. See `AioPageIterator[ListInstancesResponseTypeDef]`


```python
# paginate method usage example with argument unpacking

kwargs: ListInstancesRequestPaginateTypeDef = {  # (1)
    "PaginationConfig": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListInstancesRequestPaginateTypeDef](./type_defs.md#listinstancesrequestpaginatetypedef)
## ListIntegrationAssociationsPaginator

Type annotations and code completion for `#!python session.create_client("connect").get_paginator("list_integration_associations")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect/paginator/ListIntegrationAssociations.html#Connect.Paginator.ListIntegrationAssociations)

```python
# ListIntegrationAssociationsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_connect.paginator import ListIntegrationAssociationsPaginator

session = get_session()
async with session.create_client("connect") as client:  # (1)
    paginator: ListIntegrationAssociationsPaginator = client.get_paginator("list_integration_associations")  # (2)
    async for item in paginator.paginate(...):
        item: ListIntegrationAssociationsResponseTypeDef
        print(item)  # (3)
```

1. client: [ConnectClient](./client.md)
2. paginator: [ListIntegrationAssociationsPaginator](./paginators.md#listintegrationassociationspaginator)
3. item: `AioPageIterator[ListIntegrationAssociationsResponseTypeDef]`


### paginate

Type annotations and code completion for `#!python ListIntegrationAssociationsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    InstanceId: str,
    IntegrationType: IntegrationTypeType = ...,  # (1)
    IntegrationArn: str = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (2)
) -> aiobotocore.paginate.AioPageIterator[ListIntegrationAssociationsResponseTypeDef]:  # (3)
    ...
```

1. See [:material-code-brackets: IntegrationTypeType](./literals.md#integrationtypetype)
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
3. See `AioPageIterator[ListIntegrationAssociationsResponseTypeDef]`


```python
# paginate method usage example with argument unpacking

kwargs: ListIntegrationAssociationsRequestPaginateTypeDef = {  # (1)
    "InstanceId": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListIntegrationAssociationsRequestPaginateTypeDef](./type_defs.md#listintegrationassociationsrequestpaginatetypedef)
## ListLambdaFunctionsPaginator

Type annotations and code completion for `#!python session.create_client("connect").get_paginator("list_lambda_functions")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect/paginator/ListLambdaFunctions.html#Connect.Paginator.ListLambdaFunctions)

```python
# ListLambdaFunctionsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_connect.paginator import ListLambdaFunctionsPaginator

session = get_session()
async with session.create_client("connect") as client:  # (1)
    paginator: ListLambdaFunctionsPaginator = client.get_paginator("list_lambda_functions")  # (2)
    async for item in paginator.paginate(...):
        item: ListLambdaFunctionsResponseTypeDef
        print(item)  # (3)
```

1. client: [ConnectClient](./client.md)
2. paginator: [ListLambdaFunctionsPaginator](./paginators.md#listlambdafunctionspaginator)
3. item: `AioPageIterator[ListLambdaFunctionsResponseTypeDef]`


### paginate

Type annotations and code completion for `#!python ListLambdaFunctionsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    InstanceId: str,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> aiobotocore.paginate.AioPageIterator[ListLambdaFunctionsResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
2. See `AioPageIterator[ListLambdaFunctionsResponseTypeDef]`


```python
# paginate method usage example with argument unpacking

kwargs: ListLambdaFunctionsRequestPaginateTypeDef = {  # (1)
    "InstanceId": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListLambdaFunctionsRequestPaginateTypeDef](./type_defs.md#listlambdafunctionsrequestpaginatetypedef)
## ListLexBotsPaginator

Type annotations and code completion for `#!python session.create_client("connect").get_paginator("list_lex_bots")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect/paginator/ListLexBots.html#Connect.Paginator.ListLexBots)

```python
# ListLexBotsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_connect.paginator import ListLexBotsPaginator

session = get_session()
async with session.create_client("connect") as client:  # (1)
    paginator: ListLexBotsPaginator = client.get_paginator("list_lex_bots")  # (2)
    async for item in paginator.paginate(...):
        item: ListLexBotsResponseTypeDef
        print(item)  # (3)
```

1. client: [ConnectClient](./client.md)
2. paginator: [ListLexBotsPaginator](./paginators.md#listlexbotspaginator)
3. item: `AioPageIterator[ListLexBotsResponseTypeDef]`


### paginate

Type annotations and code completion for `#!python ListLexBotsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    InstanceId: str,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> aiobotocore.paginate.AioPageIterator[ListLexBotsResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
2. See `AioPageIterator[ListLexBotsResponseTypeDef]`


```python
# paginate method usage example with argument unpacking

kwargs: ListLexBotsRequestPaginateTypeDef = {  # (1)
    "InstanceId": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListLexBotsRequestPaginateTypeDef](./type_defs.md#listlexbotsrequestpaginatetypedef)
## ListPhoneNumbersPaginator

Type annotations and code completion for `#!python session.create_client("connect").get_paginator("list_phone_numbers")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect/paginator/ListPhoneNumbers.html#Connect.Paginator.ListPhoneNumbers)

```python
# ListPhoneNumbersPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_connect.paginator import ListPhoneNumbersPaginator

session = get_session()
async with session.create_client("connect") as client:  # (1)
    paginator: ListPhoneNumbersPaginator = client.get_paginator("list_phone_numbers")  # (2)
    async for item in paginator.paginate(...):
        item: ListPhoneNumbersResponseTypeDef
        print(item)  # (3)
```

1. client: [ConnectClient](./client.md)
2. paginator: [ListPhoneNumbersPaginator](./paginators.md#listphonenumberspaginator)
3. item: `AioPageIterator[ListPhoneNumbersResponseTypeDef]`


### paginate

Type annotations and code completion for `#!python ListPhoneNumbersPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    InstanceId: str,
    PhoneNumberTypes: Sequence[PhoneNumberTypeType] = ...,  # (1)
    PhoneNumberCountryCodes: Sequence[PhoneNumberCountryCodeType] = ...,  # (2)
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (3)
) -> aiobotocore.paginate.AioPageIterator[ListPhoneNumbersResponseTypeDef]:  # (4)
    ...
```

1. See `Sequence[PhoneNumberTypeType]`
2. See `Sequence[PhoneNumberCountryCodeType]`
3. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
4. See `AioPageIterator[ListPhoneNumbersResponseTypeDef]`


```python
# paginate method usage example with argument unpacking

kwargs: ListPhoneNumbersRequestPaginateTypeDef = {  # (1)
    "InstanceId": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListPhoneNumbersRequestPaginateTypeDef](./type_defs.md#listphonenumbersrequestpaginatetypedef)
## ListPhoneNumbersV2Paginator

Type annotations and code completion for `#!python session.create_client("connect").get_paginator("list_phone_numbers_v2")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect/paginator/ListPhoneNumbersV2.html#Connect.Paginator.ListPhoneNumbersV2)

```python
# ListPhoneNumbersV2Paginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_connect.paginator import ListPhoneNumbersV2Paginator

session = get_session()
async with session.create_client("connect") as client:  # (1)
    paginator: ListPhoneNumbersV2Paginator = client.get_paginator("list_phone_numbers_v2")  # (2)
    async for item in paginator.paginate(...):
        item: ListPhoneNumbersV2ResponseTypeDef
        print(item)  # (3)
```

1. client: [ConnectClient](./client.md)
2. paginator: [ListPhoneNumbersV2Paginator](./paginators.md#listphonenumbersv2paginator)
3. item: `AioPageIterator[ListPhoneNumbersV2ResponseTypeDef]`


### paginate

Type annotations and code completion for `#!python ListPhoneNumbersV2Paginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    TargetArn: str = ...,
    InstanceId: str = ...,
    PhoneNumberCountryCodes: Sequence[PhoneNumberCountryCodeType] = ...,  # (1)
    PhoneNumberTypes: Sequence[PhoneNumberTypeType] = ...,  # (2)
    PhoneNumberPrefix: str = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (3)
) -> aiobotocore.paginate.AioPageIterator[ListPhoneNumbersV2ResponseTypeDef]:  # (4)
    ...
```

1. See `Sequence[PhoneNumberCountryCodeType]`
2. See `Sequence[PhoneNumberTypeType]`
3. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
4. See `AioPageIterator[ListPhoneNumbersV2ResponseTypeDef]`


```python
# paginate method usage example with argument unpacking

kwargs: ListPhoneNumbersV2RequestPaginateTypeDef = {  # (1)
    "TargetArn": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListPhoneNumbersV2RequestPaginateTypeDef](./type_defs.md#listphonenumbersv2requestpaginatetypedef)
## ListPredefinedAttributesPaginator

Type annotations and code completion for `#!python session.create_client("connect").get_paginator("list_predefined_attributes")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect/paginator/ListPredefinedAttributes.html#Connect.Paginator.ListPredefinedAttributes)

```python
# ListPredefinedAttributesPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_connect.paginator import ListPredefinedAttributesPaginator

session = get_session()
async with session.create_client("connect") as client:  # (1)
    paginator: ListPredefinedAttributesPaginator = client.get_paginator("list_predefined_attributes")  # (2)
    async for item in paginator.paginate(...):
        item: ListPredefinedAttributesResponseTypeDef
        print(item)  # (3)
```

1. client: [ConnectClient](./client.md)
2. paginator: [ListPredefinedAttributesPaginator](./paginators.md#listpredefinedattributespaginator)
3. item: `AioPageIterator[ListPredefinedAttributesResponseTypeDef]`


### paginate

Type annotations and code completion for `#!python ListPredefinedAttributesPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    InstanceId: str,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> aiobotocore.paginate.AioPageIterator[ListPredefinedAttributesResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
2. See `AioPageIterator[ListPredefinedAttributesResponseTypeDef]`


```python
# paginate method usage example with argument unpacking

kwargs: ListPredefinedAttributesRequestPaginateTypeDef = {  # (1)
    "InstanceId": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListPredefinedAttributesRequestPaginateTypeDef](./type_defs.md#listpredefinedattributesrequestpaginatetypedef)
## ListPromptsPaginator

Type annotations and code completion for `#!python session.create_client("connect").get_paginator("list_prompts")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect/paginator/ListPrompts.html#Connect.Paginator.ListPrompts)

```python
# ListPromptsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_connect.paginator import ListPromptsPaginator

session = get_session()
async with session.create_client("connect") as client:  # (1)
    paginator: ListPromptsPaginator = client.get_paginator("list_prompts")  # (2)
    async for item in paginator.paginate(...):
        item: ListPromptsResponseTypeDef
        print(item)  # (3)
```

1. client: [ConnectClient](./client.md)
2. paginator: [ListPromptsPaginator](./paginators.md#listpromptspaginator)
3. item: `AioPageIterator[ListPromptsResponseTypeDef]`


### paginate

Type annotations and code completion for `#!python ListPromptsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    InstanceId: str,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> aiobotocore.paginate.AioPageIterator[ListPromptsResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
2. See `AioPageIterator[ListPromptsResponseTypeDef]`


```python
# paginate method usage example with argument unpacking

kwargs: ListPromptsRequestPaginateTypeDef = {  # (1)
    "InstanceId": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListPromptsRequestPaginateTypeDef](./type_defs.md#listpromptsrequestpaginatetypedef)
## ListQueueQuickConnectsPaginator

Type annotations and code completion for `#!python session.create_client("connect").get_paginator("list_queue_quick_connects")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect/paginator/ListQueueQuickConnects.html#Connect.Paginator.ListQueueQuickConnects)

```python
# ListQueueQuickConnectsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_connect.paginator import ListQueueQuickConnectsPaginator

session = get_session()
async with session.create_client("connect") as client:  # (1)
    paginator: ListQueueQuickConnectsPaginator = client.get_paginator("list_queue_quick_connects")  # (2)
    async for item in paginator.paginate(...):
        item: ListQueueQuickConnectsResponseTypeDef
        print(item)  # (3)
```

1. client: [ConnectClient](./client.md)
2. paginator: [ListQueueQuickConnectsPaginator](./paginators.md#listqueuequickconnectspaginator)
3. item: `AioPageIterator[ListQueueQuickConnectsResponseTypeDef]`


### paginate

Type annotations and code completion for `#!python ListQueueQuickConnectsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    InstanceId: str,
    QueueId: str,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> aiobotocore.paginate.AioPageIterator[ListQueueQuickConnectsResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
2. See `AioPageIterator[ListQueueQuickConnectsResponseTypeDef]`


```python
# paginate method usage example with argument unpacking

kwargs: ListQueueQuickConnectsRequestPaginateTypeDef = {  # (1)
    "InstanceId": ...,
    "QueueId": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListQueueQuickConnectsRequestPaginateTypeDef](./type_defs.md#listqueuequickconnectsrequestpaginatetypedef)
## ListQueuesPaginator

Type annotations and code completion for `#!python session.create_client("connect").get_paginator("list_queues")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect/paginator/ListQueues.html#Connect.Paginator.ListQueues)

```python
# ListQueuesPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_connect.paginator import ListQueuesPaginator

session = get_session()
async with session.create_client("connect") as client:  # (1)
    paginator: ListQueuesPaginator = client.get_paginator("list_queues")  # (2)
    async for item in paginator.paginate(...):
        item: ListQueuesResponseTypeDef
        print(item)  # (3)
```

1. client: [ConnectClient](./client.md)
2. paginator: [ListQueuesPaginator](./paginators.md#listqueuespaginator)
3. item: `AioPageIterator[ListQueuesResponseTypeDef]`


### paginate

Type annotations and code completion for `#!python ListQueuesPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    InstanceId: str,
    QueueTypes: Sequence[QueueTypeType] = ...,  # (1)
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (2)
) -> aiobotocore.paginate.AioPageIterator[ListQueuesResponseTypeDef]:  # (3)
    ...
```

1. See `Sequence[QueueTypeType]`
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
3. See `AioPageIterator[ListQueuesResponseTypeDef]`


```python
# paginate method usage example with argument unpacking

kwargs: ListQueuesRequestPaginateTypeDef = {  # (1)
    "InstanceId": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListQueuesRequestPaginateTypeDef](./type_defs.md#listqueuesrequestpaginatetypedef)
## ListQuickConnectsPaginator

Type annotations and code completion for `#!python session.create_client("connect").get_paginator("list_quick_connects")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect/paginator/ListQuickConnects.html#Connect.Paginator.ListQuickConnects)

```python
# ListQuickConnectsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_connect.paginator import ListQuickConnectsPaginator

session = get_session()
async with session.create_client("connect") as client:  # (1)
    paginator: ListQuickConnectsPaginator = client.get_paginator("list_quick_connects")  # (2)
    async for item in paginator.paginate(...):
        item: ListQuickConnectsResponseTypeDef
        print(item)  # (3)
```

1. client: [ConnectClient](./client.md)
2. paginator: [ListQuickConnectsPaginator](./paginators.md#listquickconnectspaginator)
3. item: `AioPageIterator[ListQuickConnectsResponseTypeDef]`


### paginate

Type annotations and code completion for `#!python ListQuickConnectsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    InstanceId: str,
    QuickConnectTypes: Sequence[QuickConnectTypeType] = ...,  # (1)
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (2)
) -> aiobotocore.paginate.AioPageIterator[ListQuickConnectsResponseTypeDef]:  # (3)
    ...
```

1. See `Sequence[QuickConnectTypeType]`
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
3. See `AioPageIterator[ListQuickConnectsResponseTypeDef]`


```python
# paginate method usage example with argument unpacking

kwargs: ListQuickConnectsRequestPaginateTypeDef = {  # (1)
    "InstanceId": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListQuickConnectsRequestPaginateTypeDef](./type_defs.md#listquickconnectsrequestpaginatetypedef)
## ListRoutingProfileManualAssignmentQueuesPaginator

Type annotations and code completion for `#!python session.create_client("connect").get_paginator("list_routing_profile_manual_assignment_queues")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect/paginator/ListRoutingProfileManualAssignmentQueues.html#Connect.Paginator.ListRoutingProfileManualAssignmentQueues)

```python
# ListRoutingProfileManualAssignmentQueuesPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_connect.paginator import ListRoutingProfileManualAssignmentQueuesPaginator

session = get_session()
async with session.create_client("connect") as client:  # (1)
    paginator: ListRoutingProfileManualAssignmentQueuesPaginator = client.get_paginator("list_routing_profile_manual_assignment_queues")  # (2)
    async for item in paginator.paginate(...):
        item: ListRoutingProfileManualAssignmentQueuesResponseTypeDef
        print(item)  # (3)
```

1. client: [ConnectClient](./client.md)
2. paginator: [ListRoutingProfileManualAssignmentQueuesPaginator](./paginators.md#listroutingprofilemanualassignmentqueuespaginator)
3. item: `AioPageIterator[ListRoutingProfileManualAssignmentQueuesResponseTypeDef]`


### paginate

Type annotations and code completion for `#!python ListRoutingProfileManualAssignmentQueuesPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    InstanceId: str,
    RoutingProfileId: str,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> aiobotocore.paginate.AioPageIterator[ListRoutingProfileManualAssignmentQueuesResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
2. See `AioPageIterator[ListRoutingProfileManualAssignmentQueuesResponseTypeDef]`


```python
# paginate method usage example with argument unpacking

kwargs: ListRoutingProfileManualAssignmentQueuesRequestPaginateTypeDef = {  # (1)
    "InstanceId": ...,
    "RoutingProfileId": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListRoutingProfileManualAssignmentQueuesRequestPaginateTypeDef](./type_defs.md#listroutingprofilemanualassignmentqueuesrequestpaginatetypedef)
## ListRoutingProfileQueuesPaginator

Type annotations and code completion for `#!python session.create_client("connect").get_paginator("list_routing_profile_queues")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect/paginator/ListRoutingProfileQueues.html#Connect.Paginator.ListRoutingProfileQueues)

```python
# ListRoutingProfileQueuesPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_connect.paginator import ListRoutingProfileQueuesPaginator

session = get_session()
async with session.create_client("connect") as client:  # (1)
    paginator: ListRoutingProfileQueuesPaginator = client.get_paginator("list_routing_profile_queues")  # (2)
    async for item in paginator.paginate(...):
        item: ListRoutingProfileQueuesResponseTypeDef
        print(item)  # (3)
```

1. client: [ConnectClient](./client.md)
2. paginator: [ListRoutingProfileQueuesPaginator](./paginators.md#listroutingprofilequeuespaginator)
3. item: `AioPageIterator[ListRoutingProfileQueuesResponseTypeDef]`


### paginate

Type annotations and code completion for `#!python ListRoutingProfileQueuesPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    InstanceId: str,
    RoutingProfileId: str,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> aiobotocore.paginate.AioPageIterator[ListRoutingProfileQueuesResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
2. See `AioPageIterator[ListRoutingProfileQueuesResponseTypeDef]`


```python
# paginate method usage example with argument unpacking

kwargs: ListRoutingProfileQueuesRequestPaginateTypeDef = {  # (1)
    "InstanceId": ...,
    "RoutingProfileId": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListRoutingProfileQueuesRequestPaginateTypeDef](./type_defs.md#listroutingprofilequeuesrequestpaginatetypedef)
## ListRoutingProfilesPaginator

Type annotations and code completion for `#!python session.create_client("connect").get_paginator("list_routing_profiles")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect/paginator/ListRoutingProfiles.html#Connect.Paginator.ListRoutingProfiles)

```python
# ListRoutingProfilesPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_connect.paginator import ListRoutingProfilesPaginator

session = get_session()
async with session.create_client("connect") as client:  # (1)
    paginator: ListRoutingProfilesPaginator = client.get_paginator("list_routing_profiles")  # (2)
    async for item in paginator.paginate(...):
        item: ListRoutingProfilesResponseTypeDef
        print(item)  # (3)
```

1. client: [ConnectClient](./client.md)
2. paginator: [ListRoutingProfilesPaginator](./paginators.md#listroutingprofilespaginator)
3. item: `AioPageIterator[ListRoutingProfilesResponseTypeDef]`


### paginate

Type annotations and code completion for `#!python ListRoutingProfilesPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    InstanceId: str,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> aiobotocore.paginate.AioPageIterator[ListRoutingProfilesResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
2. See `AioPageIterator[ListRoutingProfilesResponseTypeDef]`


```python
# paginate method usage example with argument unpacking

kwargs: ListRoutingProfilesRequestPaginateTypeDef = {  # (1)
    "InstanceId": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListRoutingProfilesRequestPaginateTypeDef](./type_defs.md#listroutingprofilesrequestpaginatetypedef)
## ListRulesPaginator

Type annotations and code completion for `#!python session.create_client("connect").get_paginator("list_rules")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect/paginator/ListRules.html#Connect.Paginator.ListRules)

```python
# ListRulesPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_connect.paginator import ListRulesPaginator

session = get_session()
async with session.create_client("connect") as client:  # (1)
    paginator: ListRulesPaginator = client.get_paginator("list_rules")  # (2)
    async for item in paginator.paginate(...):
        item: ListRulesResponseTypeDef
        print(item)  # (3)
```

1. client: [ConnectClient](./client.md)
2. paginator: [ListRulesPaginator](./paginators.md#listrulespaginator)
3. item: `AioPageIterator[ListRulesResponseTypeDef]`


### paginate

Type annotations and code completion for `#!python ListRulesPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    InstanceId: str,
    PublishStatus: RulePublishStatusType = ...,  # (1)
    EventSourceName: EventSourceNameType = ...,  # (2)
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (3)
) -> aiobotocore.paginate.AioPageIterator[ListRulesResponseTypeDef]:  # (4)
    ...
```

1. See [:material-code-brackets: RulePublishStatusType](./literals.md#rulepublishstatustype)
2. See [:material-code-brackets: EventSourceNameType](./literals.md#eventsourcenametype)
3. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
4. See `AioPageIterator[ListRulesResponseTypeDef]`


```python
# paginate method usage example with argument unpacking

kwargs: ListRulesRequestPaginateTypeDef = {  # (1)
    "InstanceId": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListRulesRequestPaginateTypeDef](./type_defs.md#listrulesrequestpaginatetypedef)
## ListSecurityKeysPaginator

Type annotations and code completion for `#!python session.create_client("connect").get_paginator("list_security_keys")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect/paginator/ListSecurityKeys.html#Connect.Paginator.ListSecurityKeys)

```python
# ListSecurityKeysPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_connect.paginator import ListSecurityKeysPaginator

session = get_session()
async with session.create_client("connect") as client:  # (1)
    paginator: ListSecurityKeysPaginator = client.get_paginator("list_security_keys")  # (2)
    async for item in paginator.paginate(...):
        item: ListSecurityKeysResponseTypeDef
        print(item)  # (3)
```

1. client: [ConnectClient](./client.md)
2. paginator: [ListSecurityKeysPaginator](./paginators.md#listsecuritykeyspaginator)
3. item: `AioPageIterator[ListSecurityKeysResponseTypeDef]`


### paginate

Type annotations and code completion for `#!python ListSecurityKeysPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    InstanceId: str,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> aiobotocore.paginate.AioPageIterator[ListSecurityKeysResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
2. See `AioPageIterator[ListSecurityKeysResponseTypeDef]`


```python
# paginate method usage example with argument unpacking

kwargs: ListSecurityKeysRequestPaginateTypeDef = {  # (1)
    "InstanceId": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListSecurityKeysRequestPaginateTypeDef](./type_defs.md#listsecuritykeysrequestpaginatetypedef)
## ListSecurityProfileApplicationsPaginator

Type annotations and code completion for `#!python session.create_client("connect").get_paginator("list_security_profile_applications")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect/paginator/ListSecurityProfileApplications.html#Connect.Paginator.ListSecurityProfileApplications)

```python
# ListSecurityProfileApplicationsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_connect.paginator import ListSecurityProfileApplicationsPaginator

session = get_session()
async with session.create_client("connect") as client:  # (1)
    paginator: ListSecurityProfileApplicationsPaginator = client.get_paginator("list_security_profile_applications")  # (2)
    async for item in paginator.paginate(...):
        item: ListSecurityProfileApplicationsResponseTypeDef
        print(item)  # (3)
```

1. client: [ConnectClient](./client.md)
2. paginator: [ListSecurityProfileApplicationsPaginator](./paginators.md#listsecurityprofileapplicationspaginator)
3. item: `AioPageIterator[ListSecurityProfileApplicationsResponseTypeDef]`


### paginate

Type annotations and code completion for `#!python ListSecurityProfileApplicationsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    SecurityProfileId: str,
    InstanceId: str,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> aiobotocore.paginate.AioPageIterator[ListSecurityProfileApplicationsResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
2. See `AioPageIterator[ListSecurityProfileApplicationsResponseTypeDef]`


```python
# paginate method usage example with argument unpacking

kwargs: ListSecurityProfileApplicationsRequestPaginateTypeDef = {  # (1)
    "SecurityProfileId": ...,
    "InstanceId": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListSecurityProfileApplicationsRequestPaginateTypeDef](./type_defs.md#listsecurityprofileapplicationsrequestpaginatetypedef)
## ListSecurityProfileFlowModulesPaginator

Type annotations and code completion for `#!python session.create_client("connect").get_paginator("list_security_profile_flow_modules")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect/paginator/ListSecurityProfileFlowModules.html#Connect.Paginator.ListSecurityProfileFlowModules)

```python
# ListSecurityProfileFlowModulesPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_connect.paginator import ListSecurityProfileFlowModulesPaginator

session = get_session()
async with session.create_client("connect") as client:  # (1)
    paginator: ListSecurityProfileFlowModulesPaginator = client.get_paginator("list_security_profile_flow_modules")  # (2)
    async for item in paginator.paginate(...):
        item: ListSecurityProfileFlowModulesResponseTypeDef
        print(item)  # (3)
```

1. client: [ConnectClient](./client.md)
2. paginator: [ListSecurityProfileFlowModulesPaginator](./paginators.md#listsecurityprofileflowmodulespaginator)
3. item: `AioPageIterator[ListSecurityProfileFlowModulesResponseTypeDef]`


### paginate

Type annotations and code completion for `#!python ListSecurityProfileFlowModulesPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    SecurityProfileId: str,
    InstanceId: str,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> aiobotocore.paginate.AioPageIterator[ListSecurityProfileFlowModulesResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
2. See `AioPageIterator[ListSecurityProfileFlowModulesResponseTypeDef]`


```python
# paginate method usage example with argument unpacking

kwargs: ListSecurityProfileFlowModulesRequestPaginateTypeDef = {  # (1)
    "SecurityProfileId": ...,
    "InstanceId": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListSecurityProfileFlowModulesRequestPaginateTypeDef](./type_defs.md#listsecurityprofileflowmodulesrequestpaginatetypedef)
## ListSecurityProfilePermissionsPaginator

Type annotations and code completion for `#!python session.create_client("connect").get_paginator("list_security_profile_permissions")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect/paginator/ListSecurityProfilePermissions.html#Connect.Paginator.ListSecurityProfilePermissions)

```python
# ListSecurityProfilePermissionsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_connect.paginator import ListSecurityProfilePermissionsPaginator

session = get_session()
async with session.create_client("connect") as client:  # (1)
    paginator: ListSecurityProfilePermissionsPaginator = client.get_paginator("list_security_profile_permissions")  # (2)
    async for item in paginator.paginate(...):
        item: ListSecurityProfilePermissionsResponseTypeDef
        print(item)  # (3)
```

1. client: [ConnectClient](./client.md)
2. paginator: [ListSecurityProfilePermissionsPaginator](./paginators.md#listsecurityprofilepermissionspaginator)
3. item: `AioPageIterator[ListSecurityProfilePermissionsResponseTypeDef]`


### paginate

Type annotations and code completion for `#!python ListSecurityProfilePermissionsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    SecurityProfileId: str,
    InstanceId: str,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> aiobotocore.paginate.AioPageIterator[ListSecurityProfilePermissionsResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
2. See `AioPageIterator[ListSecurityProfilePermissionsResponseTypeDef]`


```python
# paginate method usage example with argument unpacking

kwargs: ListSecurityProfilePermissionsRequestPaginateTypeDef = {  # (1)
    "SecurityProfileId": ...,
    "InstanceId": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListSecurityProfilePermissionsRequestPaginateTypeDef](./type_defs.md#listsecurityprofilepermissionsrequestpaginatetypedef)
## ListSecurityProfilesPaginator

Type annotations and code completion for `#!python session.create_client("connect").get_paginator("list_security_profiles")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect/paginator/ListSecurityProfiles.html#Connect.Paginator.ListSecurityProfiles)

```python
# ListSecurityProfilesPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_connect.paginator import ListSecurityProfilesPaginator

session = get_session()
async with session.create_client("connect") as client:  # (1)
    paginator: ListSecurityProfilesPaginator = client.get_paginator("list_security_profiles")  # (2)
    async for item in paginator.paginate(...):
        item: ListSecurityProfilesResponseTypeDef
        print(item)  # (3)
```

1. client: [ConnectClient](./client.md)
2. paginator: [ListSecurityProfilesPaginator](./paginators.md#listsecurityprofilespaginator)
3. item: `AioPageIterator[ListSecurityProfilesResponseTypeDef]`


### paginate

Type annotations and code completion for `#!python ListSecurityProfilesPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    InstanceId: str,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> aiobotocore.paginate.AioPageIterator[ListSecurityProfilesResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
2. See `AioPageIterator[ListSecurityProfilesResponseTypeDef]`


```python
# paginate method usage example with argument unpacking

kwargs: ListSecurityProfilesRequestPaginateTypeDef = {  # (1)
    "InstanceId": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListSecurityProfilesRequestPaginateTypeDef](./type_defs.md#listsecurityprofilesrequestpaginatetypedef)
## ListTaskTemplatesPaginator

Type annotations and code completion for `#!python session.create_client("connect").get_paginator("list_task_templates")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect/paginator/ListTaskTemplates.html#Connect.Paginator.ListTaskTemplates)

```python
# ListTaskTemplatesPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_connect.paginator import ListTaskTemplatesPaginator

session = get_session()
async with session.create_client("connect") as client:  # (1)
    paginator: ListTaskTemplatesPaginator = client.get_paginator("list_task_templates")  # (2)
    async for item in paginator.paginate(...):
        item: ListTaskTemplatesResponseTypeDef
        print(item)  # (3)
```

1. client: [ConnectClient](./client.md)
2. paginator: [ListTaskTemplatesPaginator](./paginators.md#listtasktemplatespaginator)
3. item: `AioPageIterator[ListTaskTemplatesResponseTypeDef]`


### paginate

Type annotations and code completion for `#!python ListTaskTemplatesPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    InstanceId: str,
    Status: TaskTemplateStatusType = ...,  # (1)
    Name: str = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (2)
) -> aiobotocore.paginate.AioPageIterator[ListTaskTemplatesResponseTypeDef]:  # (3)
    ...
```

1. See [:material-code-brackets: TaskTemplateStatusType](./literals.md#tasktemplatestatustype)
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
3. See `AioPageIterator[ListTaskTemplatesResponseTypeDef]`


```python
# paginate method usage example with argument unpacking

kwargs: ListTaskTemplatesRequestPaginateTypeDef = {  # (1)
    "InstanceId": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListTaskTemplatesRequestPaginateTypeDef](./type_defs.md#listtasktemplatesrequestpaginatetypedef)
## ListTrafficDistributionGroupUsersPaginator

Type annotations and code completion for `#!python session.create_client("connect").get_paginator("list_traffic_distribution_group_users")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect/paginator/ListTrafficDistributionGroupUsers.html#Connect.Paginator.ListTrafficDistributionGroupUsers)

```python
# ListTrafficDistributionGroupUsersPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_connect.paginator import ListTrafficDistributionGroupUsersPaginator

session = get_session()
async with session.create_client("connect") as client:  # (1)
    paginator: ListTrafficDistributionGroupUsersPaginator = client.get_paginator("list_traffic_distribution_group_users")  # (2)
    async for item in paginator.paginate(...):
        item: ListTrafficDistributionGroupUsersResponseTypeDef
        print(item)  # (3)
```

1. client: [ConnectClient](./client.md)
2. paginator: [ListTrafficDistributionGroupUsersPaginator](./paginators.md#listtrafficdistributiongroupuserspaginator)
3. item: `AioPageIterator[ListTrafficDistributionGroupUsersResponseTypeDef]`


### paginate

Type annotations and code completion for `#!python ListTrafficDistributionGroupUsersPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    TrafficDistributionGroupId: str,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> aiobotocore.paginate.AioPageIterator[ListTrafficDistributionGroupUsersResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
2. See `AioPageIterator[ListTrafficDistributionGroupUsersResponseTypeDef]`


```python
# paginate method usage example with argument unpacking

kwargs: ListTrafficDistributionGroupUsersRequestPaginateTypeDef = {  # (1)
    "TrafficDistributionGroupId": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListTrafficDistributionGroupUsersRequestPaginateTypeDef](./type_defs.md#listtrafficdistributiongroupusersrequestpaginatetypedef)
## ListTrafficDistributionGroupsPaginator

Type annotations and code completion for `#!python session.create_client("connect").get_paginator("list_traffic_distribution_groups")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect/paginator/ListTrafficDistributionGroups.html#Connect.Paginator.ListTrafficDistributionGroups)

```python
# ListTrafficDistributionGroupsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_connect.paginator import ListTrafficDistributionGroupsPaginator

session = get_session()
async with session.create_client("connect") as client:  # (1)
    paginator: ListTrafficDistributionGroupsPaginator = client.get_paginator("list_traffic_distribution_groups")  # (2)
    async for item in paginator.paginate(...):
        item: ListTrafficDistributionGroupsResponseTypeDef
        print(item)  # (3)
```

1. client: [ConnectClient](./client.md)
2. paginator: [ListTrafficDistributionGroupsPaginator](./paginators.md#listtrafficdistributiongroupspaginator)
3. item: `AioPageIterator[ListTrafficDistributionGroupsResponseTypeDef]`


### paginate

Type annotations and code completion for `#!python ListTrafficDistributionGroupsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    InstanceId: str = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> aiobotocore.paginate.AioPageIterator[ListTrafficDistributionGroupsResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
2. See `AioPageIterator[ListTrafficDistributionGroupsResponseTypeDef]`


```python
# paginate method usage example with argument unpacking

kwargs: ListTrafficDistributionGroupsRequestPaginateTypeDef = {  # (1)
    "InstanceId": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListTrafficDistributionGroupsRequestPaginateTypeDef](./type_defs.md#listtrafficdistributiongroupsrequestpaginatetypedef)
## ListUseCasesPaginator

Type annotations and code completion for `#!python session.create_client("connect").get_paginator("list_use_cases")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect/paginator/ListUseCases.html#Connect.Paginator.ListUseCases)

```python
# ListUseCasesPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_connect.paginator import ListUseCasesPaginator

session = get_session()
async with session.create_client("connect") as client:  # (1)
    paginator: ListUseCasesPaginator = client.get_paginator("list_use_cases")  # (2)
    async for item in paginator.paginate(...):
        item: ListUseCasesResponseTypeDef
        print(item)  # (3)
```

1. client: [ConnectClient](./client.md)
2. paginator: [ListUseCasesPaginator](./paginators.md#listusecasespaginator)
3. item: `AioPageIterator[ListUseCasesResponseTypeDef]`


### paginate

Type annotations and code completion for `#!python ListUseCasesPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    InstanceId: str,
    IntegrationAssociationId: str,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> aiobotocore.paginate.AioPageIterator[ListUseCasesResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
2. See `AioPageIterator[ListUseCasesResponseTypeDef]`


```python
# paginate method usage example with argument unpacking

kwargs: ListUseCasesRequestPaginateTypeDef = {  # (1)
    "InstanceId": ...,
    "IntegrationAssociationId": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListUseCasesRequestPaginateTypeDef](./type_defs.md#listusecasesrequestpaginatetypedef)
## ListUserHierarchyGroupsPaginator

Type annotations and code completion for `#!python session.create_client("connect").get_paginator("list_user_hierarchy_groups")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect/paginator/ListUserHierarchyGroups.html#Connect.Paginator.ListUserHierarchyGroups)

```python
# ListUserHierarchyGroupsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_connect.paginator import ListUserHierarchyGroupsPaginator

session = get_session()
async with session.create_client("connect") as client:  # (1)
    paginator: ListUserHierarchyGroupsPaginator = client.get_paginator("list_user_hierarchy_groups")  # (2)
    async for item in paginator.paginate(...):
        item: ListUserHierarchyGroupsResponseTypeDef
        print(item)  # (3)
```

1. client: [ConnectClient](./client.md)
2. paginator: [ListUserHierarchyGroupsPaginator](./paginators.md#listuserhierarchygroupspaginator)
3. item: `AioPageIterator[ListUserHierarchyGroupsResponseTypeDef]`


### paginate

Type annotations and code completion for `#!python ListUserHierarchyGroupsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    InstanceId: str,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> aiobotocore.paginate.AioPageIterator[ListUserHierarchyGroupsResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
2. See `AioPageIterator[ListUserHierarchyGroupsResponseTypeDef]`


```python
# paginate method usage example with argument unpacking

kwargs: ListUserHierarchyGroupsRequestPaginateTypeDef = {  # (1)
    "InstanceId": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListUserHierarchyGroupsRequestPaginateTypeDef](./type_defs.md#listuserhierarchygroupsrequestpaginatetypedef)
## ListUserProficienciesPaginator

Type annotations and code completion for `#!python session.create_client("connect").get_paginator("list_user_proficiencies")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect/paginator/ListUserProficiencies.html#Connect.Paginator.ListUserProficiencies)

```python
# ListUserProficienciesPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_connect.paginator import ListUserProficienciesPaginator

session = get_session()
async with session.create_client("connect") as client:  # (1)
    paginator: ListUserProficienciesPaginator = client.get_paginator("list_user_proficiencies")  # (2)
    async for item in paginator.paginate(...):
        item: ListUserProficienciesResponseTypeDef
        print(item)  # (3)
```

1. client: [ConnectClient](./client.md)
2. paginator: [ListUserProficienciesPaginator](./paginators.md#listuserproficienciespaginator)
3. item: `AioPageIterator[ListUserProficienciesResponseTypeDef]`


### paginate

Type annotations and code completion for `#!python ListUserProficienciesPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    InstanceId: str,
    UserId: str,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> aiobotocore.paginate.AioPageIterator[ListUserProficienciesResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
2. See `AioPageIterator[ListUserProficienciesResponseTypeDef]`


```python
# paginate method usage example with argument unpacking

kwargs: ListUserProficienciesRequestPaginateTypeDef = {  # (1)
    "InstanceId": ...,
    "UserId": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListUserProficienciesRequestPaginateTypeDef](./type_defs.md#listuserproficienciesrequestpaginatetypedef)
## ListUsersPaginator

Type annotations and code completion for `#!python session.create_client("connect").get_paginator("list_users")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect/paginator/ListUsers.html#Connect.Paginator.ListUsers)

```python
# ListUsersPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_connect.paginator import ListUsersPaginator

session = get_session()
async with session.create_client("connect") as client:  # (1)
    paginator: ListUsersPaginator = client.get_paginator("list_users")  # (2)
    async for item in paginator.paginate(...):
        item: ListUsersResponseTypeDef
        print(item)  # (3)
```

1. client: [ConnectClient](./client.md)
2. paginator: [ListUsersPaginator](./paginators.md#listuserspaginator)
3. item: `AioPageIterator[ListUsersResponseTypeDef]`


### paginate

Type annotations and code completion for `#!python ListUsersPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    InstanceId: str,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> aiobotocore.paginate.AioPageIterator[ListUsersResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
2. See `AioPageIterator[ListUsersResponseTypeDef]`


```python
# paginate method usage example with argument unpacking

kwargs: ListUsersRequestPaginateTypeDef = {  # (1)
    "InstanceId": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListUsersRequestPaginateTypeDef](./type_defs.md#listusersrequestpaginatetypedef)
## ListViewVersionsPaginator

Type annotations and code completion for `#!python session.create_client("connect").get_paginator("list_view_versions")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect/paginator/ListViewVersions.html#Connect.Paginator.ListViewVersions)

```python
# ListViewVersionsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_connect.paginator import ListViewVersionsPaginator

session = get_session()
async with session.create_client("connect") as client:  # (1)
    paginator: ListViewVersionsPaginator = client.get_paginator("list_view_versions")  # (2)
    async for item in paginator.paginate(...):
        item: ListViewVersionsResponseTypeDef
        print(item)  # (3)
```

1. client: [ConnectClient](./client.md)
2. paginator: [ListViewVersionsPaginator](./paginators.md#listviewversionspaginator)
3. item: `AioPageIterator[ListViewVersionsResponseTypeDef]`


### paginate

Type annotations and code completion for `#!python ListViewVersionsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    InstanceId: str,
    ViewId: str,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> aiobotocore.paginate.AioPageIterator[ListViewVersionsResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
2. See `AioPageIterator[ListViewVersionsResponseTypeDef]`


```python
# paginate method usage example with argument unpacking

kwargs: ListViewVersionsRequestPaginateTypeDef = {  # (1)
    "InstanceId": ...,
    "ViewId": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListViewVersionsRequestPaginateTypeDef](./type_defs.md#listviewversionsrequestpaginatetypedef)
## ListViewsPaginator

Type annotations and code completion for `#!python session.create_client("connect").get_paginator("list_views")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect/paginator/ListViews.html#Connect.Paginator.ListViews)

```python
# ListViewsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_connect.paginator import ListViewsPaginator

session = get_session()
async with session.create_client("connect") as client:  # (1)
    paginator: ListViewsPaginator = client.get_paginator("list_views")  # (2)
    async for item in paginator.paginate(...):
        item: ListViewsResponseTypeDef
        print(item)  # (3)
```

1. client: [ConnectClient](./client.md)
2. paginator: [ListViewsPaginator](./paginators.md#listviewspaginator)
3. item: `AioPageIterator[ListViewsResponseTypeDef]`


### paginate

Type annotations and code completion for `#!python ListViewsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    InstanceId: str,
    Type: ViewTypeType = ...,  # (1)
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (2)
) -> aiobotocore.paginate.AioPageIterator[ListViewsResponseTypeDef]:  # (3)
    ...
```

1. See [:material-code-brackets: ViewTypeType](./literals.md#viewtypetype)
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
3. See `AioPageIterator[ListViewsResponseTypeDef]`


```python
# paginate method usage example with argument unpacking

kwargs: ListViewsRequestPaginateTypeDef = {  # (1)
    "InstanceId": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListViewsRequestPaginateTypeDef](./type_defs.md#listviewsrequestpaginatetypedef)
## ListWorkspacePagesPaginator

Type annotations and code completion for `#!python session.create_client("connect").get_paginator("list_workspace_pages")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect/paginator/ListWorkspacePages.html#Connect.Paginator.ListWorkspacePages)

```python
# ListWorkspacePagesPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_connect.paginator import ListWorkspacePagesPaginator

session = get_session()
async with session.create_client("connect") as client:  # (1)
    paginator: ListWorkspacePagesPaginator = client.get_paginator("list_workspace_pages")  # (2)
    async for item in paginator.paginate(...):
        item: ListWorkspacePagesResponseTypeDef
        print(item)  # (3)
```

1. client: [ConnectClient](./client.md)
2. paginator: [ListWorkspacePagesPaginator](./paginators.md#listworkspacepagespaginator)
3. item: `AioPageIterator[ListWorkspacePagesResponseTypeDef]`


### paginate

Type annotations and code completion for `#!python ListWorkspacePagesPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    InstanceId: str,
    WorkspaceId: str,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> aiobotocore.paginate.AioPageIterator[ListWorkspacePagesResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
2. See `AioPageIterator[ListWorkspacePagesResponseTypeDef]`


```python
# paginate method usage example with argument unpacking

kwargs: ListWorkspacePagesRequestPaginateTypeDef = {  # (1)
    "InstanceId": ...,
    "WorkspaceId": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListWorkspacePagesRequestPaginateTypeDef](./type_defs.md#listworkspacepagesrequestpaginatetypedef)
## ListWorkspacesPaginator

Type annotations and code completion for `#!python session.create_client("connect").get_paginator("list_workspaces")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect/paginator/ListWorkspaces.html#Connect.Paginator.ListWorkspaces)

```python
# ListWorkspacesPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_connect.paginator import ListWorkspacesPaginator

session = get_session()
async with session.create_client("connect") as client:  # (1)
    paginator: ListWorkspacesPaginator = client.get_paginator("list_workspaces")  # (2)
    async for item in paginator.paginate(...):
        item: ListWorkspacesResponseTypeDef
        print(item)  # (3)
```

1. client: [ConnectClient](./client.md)
2. paginator: [ListWorkspacesPaginator](./paginators.md#listworkspacespaginator)
3. item: `AioPageIterator[ListWorkspacesResponseTypeDef]`


### paginate

Type annotations and code completion for `#!python ListWorkspacesPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    InstanceId: str,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> aiobotocore.paginate.AioPageIterator[ListWorkspacesResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
2. See `AioPageIterator[ListWorkspacesResponseTypeDef]`


```python
# paginate method usage example with argument unpacking

kwargs: ListWorkspacesRequestPaginateTypeDef = {  # (1)
    "InstanceId": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListWorkspacesRequestPaginateTypeDef](./type_defs.md#listworkspacesrequestpaginatetypedef)
## SearchAgentStatusesPaginator

Type annotations and code completion for `#!python session.create_client("connect").get_paginator("search_agent_statuses")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect/paginator/SearchAgentStatuses.html#Connect.Paginator.SearchAgentStatuses)

```python
# SearchAgentStatusesPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_connect.paginator import SearchAgentStatusesPaginator

session = get_session()
async with session.create_client("connect") as client:  # (1)
    paginator: SearchAgentStatusesPaginator = client.get_paginator("search_agent_statuses")  # (2)
    async for item in paginator.paginate(...):
        item: SearchAgentStatusesResponseTypeDef
        print(item)  # (3)
```

1. client: [ConnectClient](./client.md)
2. paginator: [SearchAgentStatusesPaginator](./paginators.md#searchagentstatusespaginator)
3. item: `AioPageIterator[SearchAgentStatusesResponseTypeDef]`


### paginate

Type annotations and code completion for `#!python SearchAgentStatusesPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    InstanceId: str,
    SearchFilter: AgentStatusSearchFilterTypeDef = ...,  # (1)
    SearchCriteria: AgentStatusSearchCriteriaPaginatorTypeDef = ...,  # (2)
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (3)
) -> aiobotocore.paginate.AioPageIterator[SearchAgentStatusesResponseTypeDef]:  # (4)
    ...
```

1. See [:material-code-braces: AgentStatusSearchFilterTypeDef](./type_defs.md#agentstatussearchfiltertypedef)
2. See [:material-code-braces: AgentStatusSearchCriteriaPaginatorTypeDef](./type_defs.md#agentstatussearchcriteriapaginatortypedef)
3. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
4. See `AioPageIterator[SearchAgentStatusesResponseTypeDef]`


```python
# paginate method usage example with argument unpacking

kwargs: SearchAgentStatusesRequestPaginateTypeDef = {  # (1)
    "InstanceId": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: SearchAgentStatusesRequestPaginateTypeDef](./type_defs.md#searchagentstatusesrequestpaginatetypedef)
## SearchAvailablePhoneNumbersPaginator

Type annotations and code completion for `#!python session.create_client("connect").get_paginator("search_available_phone_numbers")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect/paginator/SearchAvailablePhoneNumbers.html#Connect.Paginator.SearchAvailablePhoneNumbers)

```python
# SearchAvailablePhoneNumbersPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_connect.paginator import SearchAvailablePhoneNumbersPaginator

session = get_session()
async with session.create_client("connect") as client:  # (1)
    paginator: SearchAvailablePhoneNumbersPaginator = client.get_paginator("search_available_phone_numbers")  # (2)
    async for item in paginator.paginate(...):
        item: SearchAvailablePhoneNumbersResponseTypeDef
        print(item)  # (3)
```

1. client: [ConnectClient](./client.md)
2. paginator: [SearchAvailablePhoneNumbersPaginator](./paginators.md#searchavailablephonenumberspaginator)
3. item: `AioPageIterator[SearchAvailablePhoneNumbersResponseTypeDef]`


### paginate

Type annotations and code completion for `#!python SearchAvailablePhoneNumbersPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    PhoneNumberCountryCode: PhoneNumberCountryCodeType,  # (1)
    PhoneNumberType: PhoneNumberTypeType,  # (2)
    TargetArn: str = ...,
    InstanceId: str = ...,
    PhoneNumberPrefix: str = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (3)
) -> aiobotocore.paginate.AioPageIterator[SearchAvailablePhoneNumbersResponseTypeDef]:  # (4)
    ...
```

1. See [:material-code-brackets: PhoneNumberCountryCodeType](./literals.md#phonenumbercountrycodetype)
2. See [:material-code-brackets: PhoneNumberTypeType](./literals.md#phonenumbertypetype)
3. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
4. See `AioPageIterator[SearchAvailablePhoneNumbersResponseTypeDef]`


```python
# paginate method usage example with argument unpacking

kwargs: SearchAvailablePhoneNumbersRequestPaginateTypeDef = {  # (1)
    "PhoneNumberCountryCode": ...,
    "PhoneNumberType": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: SearchAvailablePhoneNumbersRequestPaginateTypeDef](./type_defs.md#searchavailablephonenumbersrequestpaginatetypedef)
## SearchContactFlowModulesPaginator

Type annotations and code completion for `#!python session.create_client("connect").get_paginator("search_contact_flow_modules")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect/paginator/SearchContactFlowModules.html#Connect.Paginator.SearchContactFlowModules)

```python
# SearchContactFlowModulesPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_connect.paginator import SearchContactFlowModulesPaginator

session = get_session()
async with session.create_client("connect") as client:  # (1)
    paginator: SearchContactFlowModulesPaginator = client.get_paginator("search_contact_flow_modules")  # (2)
    async for item in paginator.paginate(...):
        item: SearchContactFlowModulesResponseTypeDef
        print(item)  # (3)
```

1. client: [ConnectClient](./client.md)
2. paginator: [SearchContactFlowModulesPaginator](./paginators.md#searchcontactflowmodulespaginator)
3. item: `AioPageIterator[SearchContactFlowModulesResponseTypeDef]`


### paginate

Type annotations and code completion for `#!python SearchContactFlowModulesPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    InstanceId: str,
    SearchFilter: ContactFlowModuleSearchFilterTypeDef = ...,  # (1)
    SearchCriteria: ContactFlowModuleSearchCriteriaPaginatorTypeDef = ...,  # (2)
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (3)
) -> aiobotocore.paginate.AioPageIterator[SearchContactFlowModulesResponseTypeDef]:  # (4)
    ...
```

1. See [:material-code-braces: ContactFlowModuleSearchFilterTypeDef](./type_defs.md#contactflowmodulesearchfiltertypedef)
2. See [:material-code-braces: ContactFlowModuleSearchCriteriaPaginatorTypeDef](./type_defs.md#contactflowmodulesearchcriteriapaginatortypedef)
3. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
4. See `AioPageIterator[SearchContactFlowModulesResponseTypeDef]`


```python
# paginate method usage example with argument unpacking

kwargs: SearchContactFlowModulesRequestPaginateTypeDef = {  # (1)
    "InstanceId": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: SearchContactFlowModulesRequestPaginateTypeDef](./type_defs.md#searchcontactflowmodulesrequestpaginatetypedef)
## SearchContactFlowsPaginator

Type annotations and code completion for `#!python session.create_client("connect").get_paginator("search_contact_flows")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect/paginator/SearchContactFlows.html#Connect.Paginator.SearchContactFlows)

```python
# SearchContactFlowsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_connect.paginator import SearchContactFlowsPaginator

session = get_session()
async with session.create_client("connect") as client:  # (1)
    paginator: SearchContactFlowsPaginator = client.get_paginator("search_contact_flows")  # (2)
    async for item in paginator.paginate(...):
        item: SearchContactFlowsResponseTypeDef
        print(item)  # (3)
```

1. client: [ConnectClient](./client.md)
2. paginator: [SearchContactFlowsPaginator](./paginators.md#searchcontactflowspaginator)
3. item: `AioPageIterator[SearchContactFlowsResponseTypeDef]`


### paginate

Type annotations and code completion for `#!python SearchContactFlowsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    InstanceId: str,
    SearchFilter: ContactFlowSearchFilterTypeDef = ...,  # (1)
    SearchCriteria: ContactFlowSearchCriteriaPaginatorTypeDef = ...,  # (2)
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (3)
) -> aiobotocore.paginate.AioPageIterator[SearchContactFlowsResponseTypeDef]:  # (4)
    ...
```

1. See [:material-code-braces: ContactFlowSearchFilterTypeDef](./type_defs.md#contactflowsearchfiltertypedef)
2. See [:material-code-braces: ContactFlowSearchCriteriaPaginatorTypeDef](./type_defs.md#contactflowsearchcriteriapaginatortypedef)
3. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
4. See `AioPageIterator[SearchContactFlowsResponseTypeDef]`


```python
# paginate method usage example with argument unpacking

kwargs: SearchContactFlowsRequestPaginateTypeDef = {  # (1)
    "InstanceId": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: SearchContactFlowsRequestPaginateTypeDef](./type_defs.md#searchcontactflowsrequestpaginatetypedef)
## SearchContactsPaginator

Type annotations and code completion for `#!python session.create_client("connect").get_paginator("search_contacts")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect/paginator/SearchContacts.html#Connect.Paginator.SearchContacts)

```python
# SearchContactsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_connect.paginator import SearchContactsPaginator

session = get_session()
async with session.create_client("connect") as client:  # (1)
    paginator: SearchContactsPaginator = client.get_paginator("search_contacts")  # (2)
    async for item in paginator.paginate(...):
        item: SearchContactsResponsePaginatorTypeDef
        print(item)  # (3)
```

1. client: [ConnectClient](./client.md)
2. paginator: [SearchContactsPaginator](./paginators.md#searchcontactspaginator)
3. item: `AioPageIterator[SearchContactsResponsePaginatorTypeDef]`


### paginate

Type annotations and code completion for `#!python SearchContactsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    InstanceId: str,
    TimeRange: SearchContactsTimeRangeTypeDef,  # (1)
    SearchCriteria: SearchCriteriaTypeDef = ...,  # (2)
    Sort: SortTypeDef = ...,  # (3)
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (4)
) -> aiobotocore.paginate.AioPageIterator[SearchContactsResponsePaginatorTypeDef]:  # (5)
    ...
```

1. See [:material-code-braces: SearchContactsTimeRangeTypeDef](./type_defs.md#searchcontactstimerangetypedef)
2. See [:material-code-braces: SearchCriteriaTypeDef](./type_defs.md#searchcriteriatypedef)
3. See [:material-code-braces: SortTypeDef](./type_defs.md#sorttypedef)
4. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
5. See `AioPageIterator[SearchContactsResponsePaginatorTypeDef]`


```python
# paginate method usage example with argument unpacking

kwargs: SearchContactsRequestPaginateTypeDef = {  # (1)
    "InstanceId": ...,
    "TimeRange": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: SearchContactsRequestPaginateTypeDef](./type_defs.md#searchcontactsrequestpaginatetypedef)
## SearchDataTablesPaginator

Type annotations and code completion for `#!python session.create_client("connect").get_paginator("search_data_tables")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect/paginator/SearchDataTables.html#Connect.Paginator.SearchDataTables)

```python
# SearchDataTablesPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_connect.paginator import SearchDataTablesPaginator

session = get_session()
async with session.create_client("connect") as client:  # (1)
    paginator: SearchDataTablesPaginator = client.get_paginator("search_data_tables")  # (2)
    async for item in paginator.paginate(...):
        item: SearchDataTablesResponseTypeDef
        print(item)  # (3)
```

1. client: [ConnectClient](./client.md)
2. paginator: [SearchDataTablesPaginator](./paginators.md#searchdatatablespaginator)
3. item: `AioPageIterator[SearchDataTablesResponseTypeDef]`


### paginate

Type annotations and code completion for `#!python SearchDataTablesPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    InstanceId: str,
    SearchFilter: DataTableSearchFilterTypeDef = ...,  # (1)
    SearchCriteria: DataTableSearchCriteriaPaginatorTypeDef = ...,  # (2)
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (3)
) -> aiobotocore.paginate.AioPageIterator[SearchDataTablesResponseTypeDef]:  # (4)
    ...
```

1. See [:material-code-braces: DataTableSearchFilterTypeDef](./type_defs.md#datatablesearchfiltertypedef)
2. See [:material-code-braces: DataTableSearchCriteriaPaginatorTypeDef](./type_defs.md#datatablesearchcriteriapaginatortypedef)
3. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
4. See `AioPageIterator[SearchDataTablesResponseTypeDef]`


```python
# paginate method usage example with argument unpacking

kwargs: SearchDataTablesRequestPaginateTypeDef = {  # (1)
    "InstanceId": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: SearchDataTablesRequestPaginateTypeDef](./type_defs.md#searchdatatablesrequestpaginatetypedef)
## SearchHoursOfOperationOverridesPaginator

Type annotations and code completion for `#!python session.create_client("connect").get_paginator("search_hours_of_operation_overrides")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect/paginator/SearchHoursOfOperationOverrides.html#Connect.Paginator.SearchHoursOfOperationOverrides)

```python
# SearchHoursOfOperationOverridesPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_connect.paginator import SearchHoursOfOperationOverridesPaginator

session = get_session()
async with session.create_client("connect") as client:  # (1)
    paginator: SearchHoursOfOperationOverridesPaginator = client.get_paginator("search_hours_of_operation_overrides")  # (2)
    async for item in paginator.paginate(...):
        item: SearchHoursOfOperationOverridesResponseTypeDef
        print(item)  # (3)
```

1. client: [ConnectClient](./client.md)
2. paginator: [SearchHoursOfOperationOverridesPaginator](./paginators.md#searchhoursofoperationoverridespaginator)
3. item: `AioPageIterator[SearchHoursOfOperationOverridesResponseTypeDef]`


### paginate

Type annotations and code completion for `#!python SearchHoursOfOperationOverridesPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    InstanceId: str,
    SearchFilter: HoursOfOperationSearchFilterTypeDef = ...,  # (1)
    SearchCriteria: HoursOfOperationOverrideSearchCriteriaPaginatorTypeDef = ...,  # (2)
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (3)
) -> aiobotocore.paginate.AioPageIterator[SearchHoursOfOperationOverridesResponseTypeDef]:  # (4)
    ...
```

1. See [:material-code-braces: HoursOfOperationSearchFilterTypeDef](./type_defs.md#hoursofoperationsearchfiltertypedef)
2. See [:material-code-braces: HoursOfOperationOverrideSearchCriteriaPaginatorTypeDef](./type_defs.md#hoursofoperationoverridesearchcriteriapaginatortypedef)
3. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
4. See `AioPageIterator[SearchHoursOfOperationOverridesResponseTypeDef]`


```python
# paginate method usage example with argument unpacking

kwargs: SearchHoursOfOperationOverridesRequestPaginateTypeDef = {  # (1)
    "InstanceId": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: SearchHoursOfOperationOverridesRequestPaginateTypeDef](./type_defs.md#searchhoursofoperationoverridesrequestpaginatetypedef)
## SearchHoursOfOperationsPaginator

Type annotations and code completion for `#!python session.create_client("connect").get_paginator("search_hours_of_operations")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect/paginator/SearchHoursOfOperations.html#Connect.Paginator.SearchHoursOfOperations)

```python
# SearchHoursOfOperationsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_connect.paginator import SearchHoursOfOperationsPaginator

session = get_session()
async with session.create_client("connect") as client:  # (1)
    paginator: SearchHoursOfOperationsPaginator = client.get_paginator("search_hours_of_operations")  # (2)
    async for item in paginator.paginate(...):
        item: SearchHoursOfOperationsResponseTypeDef
        print(item)  # (3)
```

1. client: [ConnectClient](./client.md)
2. paginator: [SearchHoursOfOperationsPaginator](./paginators.md#searchhoursofoperationspaginator)
3. item: `AioPageIterator[SearchHoursOfOperationsResponseTypeDef]`


### paginate

Type annotations and code completion for `#!python SearchHoursOfOperationsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    InstanceId: str,
    SearchFilter: HoursOfOperationSearchFilterTypeDef = ...,  # (1)
    SearchCriteria: HoursOfOperationSearchCriteriaPaginatorTypeDef = ...,  # (2)
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (3)
) -> aiobotocore.paginate.AioPageIterator[SearchHoursOfOperationsResponseTypeDef]:  # (4)
    ...
```

1. See [:material-code-braces: HoursOfOperationSearchFilterTypeDef](./type_defs.md#hoursofoperationsearchfiltertypedef)
2. See [:material-code-braces: HoursOfOperationSearchCriteriaPaginatorTypeDef](./type_defs.md#hoursofoperationsearchcriteriapaginatortypedef)
3. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
4. See `AioPageIterator[SearchHoursOfOperationsResponseTypeDef]`


```python
# paginate method usage example with argument unpacking

kwargs: SearchHoursOfOperationsRequestPaginateTypeDef = {  # (1)
    "InstanceId": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: SearchHoursOfOperationsRequestPaginateTypeDef](./type_defs.md#searchhoursofoperationsrequestpaginatetypedef)
## SearchPredefinedAttributesPaginator

Type annotations and code completion for `#!python session.create_client("connect").get_paginator("search_predefined_attributes")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect/paginator/SearchPredefinedAttributes.html#Connect.Paginator.SearchPredefinedAttributes)

```python
# SearchPredefinedAttributesPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_connect.paginator import SearchPredefinedAttributesPaginator

session = get_session()
async with session.create_client("connect") as client:  # (1)
    paginator: SearchPredefinedAttributesPaginator = client.get_paginator("search_predefined_attributes")  # (2)
    async for item in paginator.paginate(...):
        item: SearchPredefinedAttributesResponseTypeDef
        print(item)  # (3)
```

1. client: [ConnectClient](./client.md)
2. paginator: [SearchPredefinedAttributesPaginator](./paginators.md#searchpredefinedattributespaginator)
3. item: `AioPageIterator[SearchPredefinedAttributesResponseTypeDef]`


### paginate

Type annotations and code completion for `#!python SearchPredefinedAttributesPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    InstanceId: str,
    SearchCriteria: PredefinedAttributeSearchCriteriaPaginatorTypeDef = ...,  # (1)
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (2)
) -> aiobotocore.paginate.AioPageIterator[SearchPredefinedAttributesResponseTypeDef]:  # (3)
    ...
```

1. See [:material-code-braces: PredefinedAttributeSearchCriteriaPaginatorTypeDef](./type_defs.md#predefinedattributesearchcriteriapaginatortypedef)
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
3. See `AioPageIterator[SearchPredefinedAttributesResponseTypeDef]`


```python
# paginate method usage example with argument unpacking

kwargs: SearchPredefinedAttributesRequestPaginateTypeDef = {  # (1)
    "InstanceId": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: SearchPredefinedAttributesRequestPaginateTypeDef](./type_defs.md#searchpredefinedattributesrequestpaginatetypedef)
## SearchPromptsPaginator

Type annotations and code completion for `#!python session.create_client("connect").get_paginator("search_prompts")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect/paginator/SearchPrompts.html#Connect.Paginator.SearchPrompts)

```python
# SearchPromptsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_connect.paginator import SearchPromptsPaginator

session = get_session()
async with session.create_client("connect") as client:  # (1)
    paginator: SearchPromptsPaginator = client.get_paginator("search_prompts")  # (2)
    async for item in paginator.paginate(...):
        item: SearchPromptsResponseTypeDef
        print(item)  # (3)
```

1. client: [ConnectClient](./client.md)
2. paginator: [SearchPromptsPaginator](./paginators.md#searchpromptspaginator)
3. item: `AioPageIterator[SearchPromptsResponseTypeDef]`


### paginate

Type annotations and code completion for `#!python SearchPromptsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    InstanceId: str,
    SearchFilter: PromptSearchFilterTypeDef = ...,  # (1)
    SearchCriteria: PromptSearchCriteriaPaginatorTypeDef = ...,  # (2)
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (3)
) -> aiobotocore.paginate.AioPageIterator[SearchPromptsResponseTypeDef]:  # (4)
    ...
```

1. See [:material-code-braces: PromptSearchFilterTypeDef](./type_defs.md#promptsearchfiltertypedef)
2. See [:material-code-braces: PromptSearchCriteriaPaginatorTypeDef](./type_defs.md#promptsearchcriteriapaginatortypedef)
3. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
4. See `AioPageIterator[SearchPromptsResponseTypeDef]`


```python
# paginate method usage example with argument unpacking

kwargs: SearchPromptsRequestPaginateTypeDef = {  # (1)
    "InstanceId": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: SearchPromptsRequestPaginateTypeDef](./type_defs.md#searchpromptsrequestpaginatetypedef)
## SearchQueuesPaginator

Type annotations and code completion for `#!python session.create_client("connect").get_paginator("search_queues")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect/paginator/SearchQueues.html#Connect.Paginator.SearchQueues)

```python
# SearchQueuesPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_connect.paginator import SearchQueuesPaginator

session = get_session()
async with session.create_client("connect") as client:  # (1)
    paginator: SearchQueuesPaginator = client.get_paginator("search_queues")  # (2)
    async for item in paginator.paginate(...):
        item: SearchQueuesResponseTypeDef
        print(item)  # (3)
```

1. client: [ConnectClient](./client.md)
2. paginator: [SearchQueuesPaginator](./paginators.md#searchqueuespaginator)
3. item: `AioPageIterator[SearchQueuesResponseTypeDef]`


### paginate

Type annotations and code completion for `#!python SearchQueuesPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    InstanceId: str,
    SearchFilter: QueueSearchFilterTypeDef = ...,  # (1)
    SearchCriteria: QueueSearchCriteriaPaginatorTypeDef = ...,  # (2)
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (3)
) -> aiobotocore.paginate.AioPageIterator[SearchQueuesResponseTypeDef]:  # (4)
    ...
```

1. See [:material-code-braces: QueueSearchFilterTypeDef](./type_defs.md#queuesearchfiltertypedef)
2. See [:material-code-braces: QueueSearchCriteriaPaginatorTypeDef](./type_defs.md#queuesearchcriteriapaginatortypedef)
3. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
4. See `AioPageIterator[SearchQueuesResponseTypeDef]`


```python
# paginate method usage example with argument unpacking

kwargs: SearchQueuesRequestPaginateTypeDef = {  # (1)
    "InstanceId": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: SearchQueuesRequestPaginateTypeDef](./type_defs.md#searchqueuesrequestpaginatetypedef)
## SearchQuickConnectsPaginator

Type annotations and code completion for `#!python session.create_client("connect").get_paginator("search_quick_connects")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect/paginator/SearchQuickConnects.html#Connect.Paginator.SearchQuickConnects)

```python
# SearchQuickConnectsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_connect.paginator import SearchQuickConnectsPaginator

session = get_session()
async with session.create_client("connect") as client:  # (1)
    paginator: SearchQuickConnectsPaginator = client.get_paginator("search_quick_connects")  # (2)
    async for item in paginator.paginate(...):
        item: SearchQuickConnectsResponseTypeDef
        print(item)  # (3)
```

1. client: [ConnectClient](./client.md)
2. paginator: [SearchQuickConnectsPaginator](./paginators.md#searchquickconnectspaginator)
3. item: `AioPageIterator[SearchQuickConnectsResponseTypeDef]`


### paginate

Type annotations and code completion for `#!python SearchQuickConnectsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    InstanceId: str,
    SearchFilter: QuickConnectSearchFilterTypeDef = ...,  # (1)
    SearchCriteria: QuickConnectSearchCriteriaPaginatorTypeDef = ...,  # (2)
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (3)
) -> aiobotocore.paginate.AioPageIterator[SearchQuickConnectsResponseTypeDef]:  # (4)
    ...
```

1. See [:material-code-braces: QuickConnectSearchFilterTypeDef](./type_defs.md#quickconnectsearchfiltertypedef)
2. See [:material-code-braces: QuickConnectSearchCriteriaPaginatorTypeDef](./type_defs.md#quickconnectsearchcriteriapaginatortypedef)
3. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
4. See `AioPageIterator[SearchQuickConnectsResponseTypeDef]`


```python
# paginate method usage example with argument unpacking

kwargs: SearchQuickConnectsRequestPaginateTypeDef = {  # (1)
    "InstanceId": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: SearchQuickConnectsRequestPaginateTypeDef](./type_defs.md#searchquickconnectsrequestpaginatetypedef)
## SearchResourceTagsPaginator

Type annotations and code completion for `#!python session.create_client("connect").get_paginator("search_resource_tags")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect/paginator/SearchResourceTags.html#Connect.Paginator.SearchResourceTags)

```python
# SearchResourceTagsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_connect.paginator import SearchResourceTagsPaginator

session = get_session()
async with session.create_client("connect") as client:  # (1)
    paginator: SearchResourceTagsPaginator = client.get_paginator("search_resource_tags")  # (2)
    async for item in paginator.paginate(...):
        item: SearchResourceTagsResponseTypeDef
        print(item)  # (3)
```

1. client: [ConnectClient](./client.md)
2. paginator: [SearchResourceTagsPaginator](./paginators.md#searchresourcetagspaginator)
3. item: `AioPageIterator[SearchResourceTagsResponseTypeDef]`


### paginate

Type annotations and code completion for `#!python SearchResourceTagsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    InstanceId: str,
    ResourceTypes: Sequence[str] = ...,
    SearchCriteria: ResourceTagsSearchCriteriaTypeDef = ...,  # (1)
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (2)
) -> aiobotocore.paginate.AioPageIterator[SearchResourceTagsResponseTypeDef]:  # (3)
    ...
```

1. See [:material-code-braces: ResourceTagsSearchCriteriaTypeDef](./type_defs.md#resourcetagssearchcriteriatypedef)
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
3. See `AioPageIterator[SearchResourceTagsResponseTypeDef]`


```python
# paginate method usage example with argument unpacking

kwargs: SearchResourceTagsRequestPaginateTypeDef = {  # (1)
    "InstanceId": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: SearchResourceTagsRequestPaginateTypeDef](./type_defs.md#searchresourcetagsrequestpaginatetypedef)
## SearchRoutingProfilesPaginator

Type annotations and code completion for `#!python session.create_client("connect").get_paginator("search_routing_profiles")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect/paginator/SearchRoutingProfiles.html#Connect.Paginator.SearchRoutingProfiles)

```python
# SearchRoutingProfilesPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_connect.paginator import SearchRoutingProfilesPaginator

session = get_session()
async with session.create_client("connect") as client:  # (1)
    paginator: SearchRoutingProfilesPaginator = client.get_paginator("search_routing_profiles")  # (2)
    async for item in paginator.paginate(...):
        item: SearchRoutingProfilesResponseTypeDef
        print(item)  # (3)
```

1. client: [ConnectClient](./client.md)
2. paginator: [SearchRoutingProfilesPaginator](./paginators.md#searchroutingprofilespaginator)
3. item: `AioPageIterator[SearchRoutingProfilesResponseTypeDef]`


### paginate

Type annotations and code completion for `#!python SearchRoutingProfilesPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    InstanceId: str,
    SearchFilter: RoutingProfileSearchFilterTypeDef = ...,  # (1)
    SearchCriteria: RoutingProfileSearchCriteriaPaginatorTypeDef = ...,  # (2)
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (3)
) -> aiobotocore.paginate.AioPageIterator[SearchRoutingProfilesResponseTypeDef]:  # (4)
    ...
```

1. See [:material-code-braces: RoutingProfileSearchFilterTypeDef](./type_defs.md#routingprofilesearchfiltertypedef)
2. See [:material-code-braces: RoutingProfileSearchCriteriaPaginatorTypeDef](./type_defs.md#routingprofilesearchcriteriapaginatortypedef)
3. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
4. See `AioPageIterator[SearchRoutingProfilesResponseTypeDef]`


```python
# paginate method usage example with argument unpacking

kwargs: SearchRoutingProfilesRequestPaginateTypeDef = {  # (1)
    "InstanceId": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: SearchRoutingProfilesRequestPaginateTypeDef](./type_defs.md#searchroutingprofilesrequestpaginatetypedef)
## SearchSecurityProfilesPaginator

Type annotations and code completion for `#!python session.create_client("connect").get_paginator("search_security_profiles")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect/paginator/SearchSecurityProfiles.html#Connect.Paginator.SearchSecurityProfiles)

```python
# SearchSecurityProfilesPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_connect.paginator import SearchSecurityProfilesPaginator

session = get_session()
async with session.create_client("connect") as client:  # (1)
    paginator: SearchSecurityProfilesPaginator = client.get_paginator("search_security_profiles")  # (2)
    async for item in paginator.paginate(...):
        item: SearchSecurityProfilesResponseTypeDef
        print(item)  # (3)
```

1. client: [ConnectClient](./client.md)
2. paginator: [SearchSecurityProfilesPaginator](./paginators.md#searchsecurityprofilespaginator)
3. item: `AioPageIterator[SearchSecurityProfilesResponseTypeDef]`


### paginate

Type annotations and code completion for `#!python SearchSecurityProfilesPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    InstanceId: str,
    SearchCriteria: SecurityProfileSearchCriteriaPaginatorTypeDef = ...,  # (1)
    SearchFilter: SecurityProfilesSearchFilterTypeDef = ...,  # (2)
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (3)
) -> aiobotocore.paginate.AioPageIterator[SearchSecurityProfilesResponseTypeDef]:  # (4)
    ...
```

1. See [:material-code-braces: SecurityProfileSearchCriteriaPaginatorTypeDef](./type_defs.md#securityprofilesearchcriteriapaginatortypedef)
2. See [:material-code-braces: SecurityProfilesSearchFilterTypeDef](./type_defs.md#securityprofilessearchfiltertypedef)
3. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
4. See `AioPageIterator[SearchSecurityProfilesResponseTypeDef]`


```python
# paginate method usage example with argument unpacking

kwargs: SearchSecurityProfilesRequestPaginateTypeDef = {  # (1)
    "InstanceId": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: SearchSecurityProfilesRequestPaginateTypeDef](./type_defs.md#searchsecurityprofilesrequestpaginatetypedef)
## SearchUserHierarchyGroupsPaginator

Type annotations and code completion for `#!python session.create_client("connect").get_paginator("search_user_hierarchy_groups")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect/paginator/SearchUserHierarchyGroups.html#Connect.Paginator.SearchUserHierarchyGroups)

```python
# SearchUserHierarchyGroupsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_connect.paginator import SearchUserHierarchyGroupsPaginator

session = get_session()
async with session.create_client("connect") as client:  # (1)
    paginator: SearchUserHierarchyGroupsPaginator = client.get_paginator("search_user_hierarchy_groups")  # (2)
    async for item in paginator.paginate(...):
        item: SearchUserHierarchyGroupsResponseTypeDef
        print(item)  # (3)
```

1. client: [ConnectClient](./client.md)
2. paginator: [SearchUserHierarchyGroupsPaginator](./paginators.md#searchuserhierarchygroupspaginator)
3. item: `AioPageIterator[SearchUserHierarchyGroupsResponseTypeDef]`


### paginate

Type annotations and code completion for `#!python SearchUserHierarchyGroupsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    InstanceId: str,
    SearchFilter: UserHierarchyGroupSearchFilterTypeDef = ...,  # (1)
    SearchCriteria: UserHierarchyGroupSearchCriteriaPaginatorTypeDef = ...,  # (2)
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (3)
) -> aiobotocore.paginate.AioPageIterator[SearchUserHierarchyGroupsResponseTypeDef]:  # (4)
    ...
```

1. See [:material-code-braces: UserHierarchyGroupSearchFilterTypeDef](./type_defs.md#userhierarchygroupsearchfiltertypedef)
2. See [:material-code-braces: UserHierarchyGroupSearchCriteriaPaginatorTypeDef](./type_defs.md#userhierarchygroupsearchcriteriapaginatortypedef)
3. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
4. See `AioPageIterator[SearchUserHierarchyGroupsResponseTypeDef]`


```python
# paginate method usage example with argument unpacking

kwargs: SearchUserHierarchyGroupsRequestPaginateTypeDef = {  # (1)
    "InstanceId": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: SearchUserHierarchyGroupsRequestPaginateTypeDef](./type_defs.md#searchuserhierarchygroupsrequestpaginatetypedef)
## SearchUsersPaginator

Type annotations and code completion for `#!python session.create_client("connect").get_paginator("search_users")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect/paginator/SearchUsers.html#Connect.Paginator.SearchUsers)

```python
# SearchUsersPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_connect.paginator import SearchUsersPaginator

session = get_session()
async with session.create_client("connect") as client:  # (1)
    paginator: SearchUsersPaginator = client.get_paginator("search_users")  # (2)
    async for item in paginator.paginate(...):
        item: SearchUsersResponseTypeDef
        print(item)  # (3)
```

1. client: [ConnectClient](./client.md)
2. paginator: [SearchUsersPaginator](./paginators.md#searchuserspaginator)
3. item: `AioPageIterator[SearchUsersResponseTypeDef]`


### paginate

Type annotations and code completion for `#!python SearchUsersPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    InstanceId: str,
    SearchFilter: UserSearchFilterTypeDef = ...,  # (1)
    SearchCriteria: UserSearchCriteriaPaginatorTypeDef = ...,  # (2)
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (3)
) -> aiobotocore.paginate.AioPageIterator[SearchUsersResponseTypeDef]:  # (4)
    ...
```

1. See [:material-code-braces: UserSearchFilterTypeDef](./type_defs.md#usersearchfiltertypedef)
2. See [:material-code-braces: UserSearchCriteriaPaginatorTypeDef](./type_defs.md#usersearchcriteriapaginatortypedef)
3. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
4. See `AioPageIterator[SearchUsersResponseTypeDef]`


```python
# paginate method usage example with argument unpacking

kwargs: SearchUsersRequestPaginateTypeDef = {  # (1)
    "InstanceId": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: SearchUsersRequestPaginateTypeDef](./type_defs.md#searchusersrequestpaginatetypedef)
## SearchViewsPaginator

Type annotations and code completion for `#!python session.create_client("connect").get_paginator("search_views")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect/paginator/SearchViews.html#Connect.Paginator.SearchViews)

```python
# SearchViewsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_connect.paginator import SearchViewsPaginator

session = get_session()
async with session.create_client("connect") as client:  # (1)
    paginator: SearchViewsPaginator = client.get_paginator("search_views")  # (2)
    async for item in paginator.paginate(...):
        item: SearchViewsResponseTypeDef
        print(item)  # (3)
```

1. client: [ConnectClient](./client.md)
2. paginator: [SearchViewsPaginator](./paginators.md#searchviewspaginator)
3. item: `AioPageIterator[SearchViewsResponseTypeDef]`


### paginate

Type annotations and code completion for `#!python SearchViewsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    InstanceId: str,
    SearchFilter: ViewSearchFilterTypeDef = ...,  # (1)
    SearchCriteria: ViewSearchCriteriaPaginatorTypeDef = ...,  # (2)
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (3)
) -> aiobotocore.paginate.AioPageIterator[SearchViewsResponseTypeDef]:  # (4)
    ...
```

1. See [:material-code-braces: ViewSearchFilterTypeDef](./type_defs.md#viewsearchfiltertypedef)
2. See [:material-code-braces: ViewSearchCriteriaPaginatorTypeDef](./type_defs.md#viewsearchcriteriapaginatortypedef)
3. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
4. See `AioPageIterator[SearchViewsResponseTypeDef]`


```python
# paginate method usage example with argument unpacking

kwargs: SearchViewsRequestPaginateTypeDef = {  # (1)
    "InstanceId": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: SearchViewsRequestPaginateTypeDef](./type_defs.md#searchviewsrequestpaginatetypedef)
## SearchVocabulariesPaginator

Type annotations and code completion for `#!python session.create_client("connect").get_paginator("search_vocabularies")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect/paginator/SearchVocabularies.html#Connect.Paginator.SearchVocabularies)

```python
# SearchVocabulariesPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_connect.paginator import SearchVocabulariesPaginator

session = get_session()
async with session.create_client("connect") as client:  # (1)
    paginator: SearchVocabulariesPaginator = client.get_paginator("search_vocabularies")  # (2)
    async for item in paginator.paginate(...):
        item: SearchVocabulariesResponseTypeDef
        print(item)  # (3)
```

1. client: [ConnectClient](./client.md)
2. paginator: [SearchVocabulariesPaginator](./paginators.md#searchvocabulariespaginator)
3. item: `AioPageIterator[SearchVocabulariesResponseTypeDef]`


### paginate

Type annotations and code completion for `#!python SearchVocabulariesPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    InstanceId: str,
    State: VocabularyStateType = ...,  # (1)
    NameStartsWith: str = ...,
    LanguageCode: VocabularyLanguageCodeType = ...,  # (2)
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (3)
) -> aiobotocore.paginate.AioPageIterator[SearchVocabulariesResponseTypeDef]:  # (4)
    ...
```

1. See [:material-code-brackets: VocabularyStateType](./literals.md#vocabularystatetype)
2. See [:material-code-brackets: VocabularyLanguageCodeType](./literals.md#vocabularylanguagecodetype)
3. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
4. See `AioPageIterator[SearchVocabulariesResponseTypeDef]`


```python
# paginate method usage example with argument unpacking

kwargs: SearchVocabulariesRequestPaginateTypeDef = {  # (1)
    "InstanceId": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: SearchVocabulariesRequestPaginateTypeDef](./type_defs.md#searchvocabulariesrequestpaginatetypedef)
## SearchWorkspaceAssociationsPaginator

Type annotations and code completion for `#!python session.create_client("connect").get_paginator("search_workspace_associations")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect/paginator/SearchWorkspaceAssociations.html#Connect.Paginator.SearchWorkspaceAssociations)

```python
# SearchWorkspaceAssociationsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_connect.paginator import SearchWorkspaceAssociationsPaginator

session = get_session()
async with session.create_client("connect") as client:  # (1)
    paginator: SearchWorkspaceAssociationsPaginator = client.get_paginator("search_workspace_associations")  # (2)
    async for item in paginator.paginate(...):
        item: SearchWorkspaceAssociationsResponseTypeDef
        print(item)  # (3)
```

1. client: [ConnectClient](./client.md)
2. paginator: [SearchWorkspaceAssociationsPaginator](./paginators.md#searchworkspaceassociationspaginator)
3. item: `AioPageIterator[SearchWorkspaceAssociationsResponseTypeDef]`


### paginate

Type annotations and code completion for `#!python SearchWorkspaceAssociationsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    InstanceId: str,
    SearchFilter: WorkspaceAssociationSearchFilterTypeDef = ...,  # (1)
    SearchCriteria: WorkspaceAssociationSearchCriteriaPaginatorTypeDef = ...,  # (2)
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (3)
) -> aiobotocore.paginate.AioPageIterator[SearchWorkspaceAssociationsResponseTypeDef]:  # (4)
    ...
```

1. See [:material-code-braces: WorkspaceAssociationSearchFilterTypeDef](./type_defs.md#workspaceassociationsearchfiltertypedef)
2. See [:material-code-braces: WorkspaceAssociationSearchCriteriaPaginatorTypeDef](./type_defs.md#workspaceassociationsearchcriteriapaginatortypedef)
3. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
4. See `AioPageIterator[SearchWorkspaceAssociationsResponseTypeDef]`


```python
# paginate method usage example with argument unpacking

kwargs: SearchWorkspaceAssociationsRequestPaginateTypeDef = {  # (1)
    "InstanceId": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: SearchWorkspaceAssociationsRequestPaginateTypeDef](./type_defs.md#searchworkspaceassociationsrequestpaginatetypedef)
## SearchWorkspacesPaginator

Type annotations and code completion for `#!python session.create_client("connect").get_paginator("search_workspaces")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect/paginator/SearchWorkspaces.html#Connect.Paginator.SearchWorkspaces)

```python
# SearchWorkspacesPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_connect.paginator import SearchWorkspacesPaginator

session = get_session()
async with session.create_client("connect") as client:  # (1)
    paginator: SearchWorkspacesPaginator = client.get_paginator("search_workspaces")  # (2)
    async for item in paginator.paginate(...):
        item: SearchWorkspacesResponseTypeDef
        print(item)  # (3)
```

1. client: [ConnectClient](./client.md)
2. paginator: [SearchWorkspacesPaginator](./paginators.md#searchworkspacespaginator)
3. item: `AioPageIterator[SearchWorkspacesResponseTypeDef]`


### paginate

Type annotations and code completion for `#!python SearchWorkspacesPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    InstanceId: str,
    SearchFilter: WorkspaceSearchFilterTypeDef = ...,  # (1)
    SearchCriteria: WorkspaceSearchCriteriaPaginatorTypeDef = ...,  # (2)
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (3)
) -> aiobotocore.paginate.AioPageIterator[SearchWorkspacesResponseTypeDef]:  # (4)
    ...
```

1. See [:material-code-braces: WorkspaceSearchFilterTypeDef](./type_defs.md#workspacesearchfiltertypedef)
2. See [:material-code-braces: WorkspaceSearchCriteriaPaginatorTypeDef](./type_defs.md#workspacesearchcriteriapaginatortypedef)
3. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
4. See `AioPageIterator[SearchWorkspacesResponseTypeDef]`


```python
# paginate method usage example with argument unpacking

kwargs: SearchWorkspacesRequestPaginateTypeDef = {  # (1)
    "InstanceId": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: SearchWorkspacesRequestPaginateTypeDef](./type_defs.md#searchworkspacesrequestpaginatetypedef)
