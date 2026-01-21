# Paginators

> [Index](../README.md) > [ComputeOptimizerAutomation](./README.md) > Paginators

!!! note ""

    Auto-generated documentation for [ComputeOptimizerAutomation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/compute-optimizer-automation.html#computeoptimizerautomation)
    type annotations stubs module [types-aiobotocore-compute-optimizer-automation](https://pypi.org/project/types-aiobotocore-compute-optimizer-automation/).

## ListAccountsPaginator

Type annotations and code completion for `#!python session.create_client("compute-optimizer-automation").get_paginator("list_accounts")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/compute-optimizer-automation/paginator/ListAccounts.html#ComputeOptimizerAutomation.Paginator.ListAccounts)

```python
# ListAccountsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_compute_optimizer_automation.paginator import ListAccountsPaginator

session = get_session()
async with session.create_client("compute-optimizer-automation") as client:  # (1)
    paginator: ListAccountsPaginator = client.get_paginator("list_accounts")  # (2)
    async for item in paginator.paginate(...):
        item: ListAccountsResponseTypeDef
        print(item)  # (3)
```

1. client: [ComputeOptimizerAutomationClient](./client.md)
2. paginator: [ListAccountsPaginator](./paginators.md#listaccountspaginator)
3. item: `AioPageIterator[ListAccountsResponseTypeDef]`


### paginate

Type annotations and code completion for `#!python ListAccountsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> aiobotocore.paginate.AioPageIterator[ListAccountsResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
2. See `AioPageIterator[ListAccountsResponseTypeDef]`


```python
# paginate method usage example with argument unpacking

kwargs: ListAccountsRequestPaginateTypeDef = {  # (1)
    "PaginationConfig": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListAccountsRequestPaginateTypeDef](./type_defs.md#listaccountsrequestpaginatetypedef)
## ListAutomationEventStepsPaginator

Type annotations and code completion for `#!python session.create_client("compute-optimizer-automation").get_paginator("list_automation_event_steps")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/compute-optimizer-automation/paginator/ListAutomationEventSteps.html#ComputeOptimizerAutomation.Paginator.ListAutomationEventSteps)

```python
# ListAutomationEventStepsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_compute_optimizer_automation.paginator import ListAutomationEventStepsPaginator

session = get_session()
async with session.create_client("compute-optimizer-automation") as client:  # (1)
    paginator: ListAutomationEventStepsPaginator = client.get_paginator("list_automation_event_steps")  # (2)
    async for item in paginator.paginate(...):
        item: ListAutomationEventStepsResponseTypeDef
        print(item)  # (3)
```

1. client: [ComputeOptimizerAutomationClient](./client.md)
2. paginator: [ListAutomationEventStepsPaginator](./paginators.md#listautomationeventstepspaginator)
3. item: `AioPageIterator[ListAutomationEventStepsResponseTypeDef]`


### paginate

Type annotations and code completion for `#!python ListAutomationEventStepsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    eventId: str,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> aiobotocore.paginate.AioPageIterator[ListAutomationEventStepsResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
2. See `AioPageIterator[ListAutomationEventStepsResponseTypeDef]`


```python
# paginate method usage example with argument unpacking

kwargs: ListAutomationEventStepsRequestPaginateTypeDef = {  # (1)
    "eventId": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListAutomationEventStepsRequestPaginateTypeDef](./type_defs.md#listautomationeventstepsrequestpaginatetypedef)
## ListAutomationEventSummariesPaginator

Type annotations and code completion for `#!python session.create_client("compute-optimizer-automation").get_paginator("list_automation_event_summaries")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/compute-optimizer-automation/paginator/ListAutomationEventSummaries.html#ComputeOptimizerAutomation.Paginator.ListAutomationEventSummaries)

```python
# ListAutomationEventSummariesPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_compute_optimizer_automation.paginator import ListAutomationEventSummariesPaginator

session = get_session()
async with session.create_client("compute-optimizer-automation") as client:  # (1)
    paginator: ListAutomationEventSummariesPaginator = client.get_paginator("list_automation_event_summaries")  # (2)
    async for item in paginator.paginate(...):
        item: ListAutomationEventSummariesResponseTypeDef
        print(item)  # (3)
```

1. client: [ComputeOptimizerAutomationClient](./client.md)
2. paginator: [ListAutomationEventSummariesPaginator](./paginators.md#listautomationeventsummariespaginator)
3. item: `AioPageIterator[ListAutomationEventSummariesResponseTypeDef]`


### paginate

Type annotations and code completion for `#!python ListAutomationEventSummariesPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    filters: Sequence[AutomationEventFilterTypeDef] = ...,  # (1)
    startDateInclusive: str = ...,
    endDateExclusive: str = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (2)
) -> aiobotocore.paginate.AioPageIterator[ListAutomationEventSummariesResponseTypeDef]:  # (3)
    ...
```

1. See `Sequence[AutomationEventFilterTypeDef]`
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
3. See `AioPageIterator[ListAutomationEventSummariesResponseTypeDef]`


```python
# paginate method usage example with argument unpacking

kwargs: ListAutomationEventSummariesRequestPaginateTypeDef = {  # (1)
    "filters": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListAutomationEventSummariesRequestPaginateTypeDef](./type_defs.md#listautomationeventsummariesrequestpaginatetypedef)
## ListAutomationEventsPaginator

Type annotations and code completion for `#!python session.create_client("compute-optimizer-automation").get_paginator("list_automation_events")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/compute-optimizer-automation/paginator/ListAutomationEvents.html#ComputeOptimizerAutomation.Paginator.ListAutomationEvents)

```python
# ListAutomationEventsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_compute_optimizer_automation.paginator import ListAutomationEventsPaginator

session = get_session()
async with session.create_client("compute-optimizer-automation") as client:  # (1)
    paginator: ListAutomationEventsPaginator = client.get_paginator("list_automation_events")  # (2)
    async for item in paginator.paginate(...):
        item: ListAutomationEventsResponseTypeDef
        print(item)  # (3)
```

1. client: [ComputeOptimizerAutomationClient](./client.md)
2. paginator: [ListAutomationEventsPaginator](./paginators.md#listautomationeventspaginator)
3. item: `AioPageIterator[ListAutomationEventsResponseTypeDef]`


### paginate

Type annotations and code completion for `#!python ListAutomationEventsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    filters: Sequence[AutomationEventFilterTypeDef] = ...,  # (1)
    startTimeInclusive: TimestampTypeDef = ...,
    endTimeExclusive: TimestampTypeDef = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (2)
) -> aiobotocore.paginate.AioPageIterator[ListAutomationEventsResponseTypeDef]:  # (3)
    ...
```

1. See `Sequence[AutomationEventFilterTypeDef]`
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
3. See `AioPageIterator[ListAutomationEventsResponseTypeDef]`


```python
# paginate method usage example with argument unpacking

kwargs: ListAutomationEventsRequestPaginateTypeDef = {  # (1)
    "filters": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListAutomationEventsRequestPaginateTypeDef](./type_defs.md#listautomationeventsrequestpaginatetypedef)
## ListAutomationRulePreviewPaginator

Type annotations and code completion for `#!python session.create_client("compute-optimizer-automation").get_paginator("list_automation_rule_preview")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/compute-optimizer-automation/paginator/ListAutomationRulePreview.html#ComputeOptimizerAutomation.Paginator.ListAutomationRulePreview)

```python
# ListAutomationRulePreviewPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_compute_optimizer_automation.paginator import ListAutomationRulePreviewPaginator

session = get_session()
async with session.create_client("compute-optimizer-automation") as client:  # (1)
    paginator: ListAutomationRulePreviewPaginator = client.get_paginator("list_automation_rule_preview")  # (2)
    async for item in paginator.paginate(...):
        item: ListAutomationRulePreviewResponseTypeDef
        print(item)  # (3)
```

1. client: [ComputeOptimizerAutomationClient](./client.md)
2. paginator: [ListAutomationRulePreviewPaginator](./paginators.md#listautomationrulepreviewpaginator)
3. item: `AioPageIterator[ListAutomationRulePreviewResponseTypeDef]`


### paginate

Type annotations and code completion for `#!python ListAutomationRulePreviewPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    ruleType: RuleTypeType,  # (1)
    recommendedActionTypes: Sequence[RecommendedActionTypeType],  # (2)
    organizationScope: OrganizationScopeTypeDef = ...,  # (3)
    criteria: CriteriaUnionTypeDef = ...,  # (4)
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (5)
) -> aiobotocore.paginate.AioPageIterator[ListAutomationRulePreviewResponseTypeDef]:  # (6)
    ...
```

1. See [:material-code-brackets: RuleTypeType](./literals.md#ruletypetype)
2. See `Sequence[RecommendedActionTypeType]`
3. See [:material-code-braces: OrganizationScopeTypeDef](./type_defs.md#organizationscopetypedef)
4. See [:material-code-braces: CriteriaUnionTypeDef](#criteriauniontypedef)
5. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
6. See `AioPageIterator[ListAutomationRulePreviewResponseTypeDef]`


```python
# paginate method usage example with argument unpacking

kwargs: ListAutomationRulePreviewRequestPaginateTypeDef = {  # (1)
    "ruleType": ...,
    "recommendedActionTypes": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListAutomationRulePreviewRequestPaginateTypeDef](./type_defs.md#listautomationrulepreviewrequestpaginatetypedef)
## ListAutomationRulePreviewSummariesPaginator

Type annotations and code completion for `#!python session.create_client("compute-optimizer-automation").get_paginator("list_automation_rule_preview_summaries")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/compute-optimizer-automation/paginator/ListAutomationRulePreviewSummaries.html#ComputeOptimizerAutomation.Paginator.ListAutomationRulePreviewSummaries)

```python
# ListAutomationRulePreviewSummariesPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_compute_optimizer_automation.paginator import ListAutomationRulePreviewSummariesPaginator

session = get_session()
async with session.create_client("compute-optimizer-automation") as client:  # (1)
    paginator: ListAutomationRulePreviewSummariesPaginator = client.get_paginator("list_automation_rule_preview_summaries")  # (2)
    async for item in paginator.paginate(...):
        item: ListAutomationRulePreviewSummariesResponseTypeDef
        print(item)  # (3)
```

1. client: [ComputeOptimizerAutomationClient](./client.md)
2. paginator: [ListAutomationRulePreviewSummariesPaginator](./paginators.md#listautomationrulepreviewsummariespaginator)
3. item: `AioPageIterator[ListAutomationRulePreviewSummariesResponseTypeDef]`


### paginate

Type annotations and code completion for `#!python ListAutomationRulePreviewSummariesPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    ruleType: RuleTypeType,  # (1)
    recommendedActionTypes: Sequence[RecommendedActionTypeType],  # (2)
    organizationScope: OrganizationScopeTypeDef = ...,  # (3)
    criteria: CriteriaUnionTypeDef = ...,  # (4)
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (5)
) -> aiobotocore.paginate.AioPageIterator[ListAutomationRulePreviewSummariesResponseTypeDef]:  # (6)
    ...
```

1. See [:material-code-brackets: RuleTypeType](./literals.md#ruletypetype)
2. See `Sequence[RecommendedActionTypeType]`
3. See [:material-code-braces: OrganizationScopeTypeDef](./type_defs.md#organizationscopetypedef)
4. See [:material-code-braces: CriteriaUnionTypeDef](#criteriauniontypedef)
5. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
6. See `AioPageIterator[ListAutomationRulePreviewSummariesResponseTypeDef]`


```python
# paginate method usage example with argument unpacking

kwargs: ListAutomationRulePreviewSummariesRequestPaginateTypeDef = {  # (1)
    "ruleType": ...,
    "recommendedActionTypes": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListAutomationRulePreviewSummariesRequestPaginateTypeDef](./type_defs.md#listautomationrulepreviewsummariesrequestpaginatetypedef)
## ListAutomationRulesPaginator

Type annotations and code completion for `#!python session.create_client("compute-optimizer-automation").get_paginator("list_automation_rules")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/compute-optimizer-automation/paginator/ListAutomationRules.html#ComputeOptimizerAutomation.Paginator.ListAutomationRules)

```python
# ListAutomationRulesPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_compute_optimizer_automation.paginator import ListAutomationRulesPaginator

session = get_session()
async with session.create_client("compute-optimizer-automation") as client:  # (1)
    paginator: ListAutomationRulesPaginator = client.get_paginator("list_automation_rules")  # (2)
    async for item in paginator.paginate(...):
        item: ListAutomationRulesResponseTypeDef
        print(item)  # (3)
```

1. client: [ComputeOptimizerAutomationClient](./client.md)
2. paginator: [ListAutomationRulesPaginator](./paginators.md#listautomationrulespaginator)
3. item: `AioPageIterator[ListAutomationRulesResponseTypeDef]`


### paginate

Type annotations and code completion for `#!python ListAutomationRulesPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    filters: Sequence[FilterTypeDef] = ...,  # (1)
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (2)
) -> aiobotocore.paginate.AioPageIterator[ListAutomationRulesResponseTypeDef]:  # (3)
    ...
```

1. See `Sequence[FilterTypeDef]`
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
3. See `AioPageIterator[ListAutomationRulesResponseTypeDef]`


```python
# paginate method usage example with argument unpacking

kwargs: ListAutomationRulesRequestPaginateTypeDef = {  # (1)
    "filters": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListAutomationRulesRequestPaginateTypeDef](./type_defs.md#listautomationrulesrequestpaginatetypedef)
## ListRecommendedActionSummariesPaginator

Type annotations and code completion for `#!python session.create_client("compute-optimizer-automation").get_paginator("list_recommended_action_summaries")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/compute-optimizer-automation/paginator/ListRecommendedActionSummaries.html#ComputeOptimizerAutomation.Paginator.ListRecommendedActionSummaries)

```python
# ListRecommendedActionSummariesPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_compute_optimizer_automation.paginator import ListRecommendedActionSummariesPaginator

session = get_session()
async with session.create_client("compute-optimizer-automation") as client:  # (1)
    paginator: ListRecommendedActionSummariesPaginator = client.get_paginator("list_recommended_action_summaries")  # (2)
    async for item in paginator.paginate(...):
        item: ListRecommendedActionSummariesResponseTypeDef
        print(item)  # (3)
```

1. client: [ComputeOptimizerAutomationClient](./client.md)
2. paginator: [ListRecommendedActionSummariesPaginator](./paginators.md#listrecommendedactionsummariespaginator)
3. item: `AioPageIterator[ListRecommendedActionSummariesResponseTypeDef]`


### paginate

Type annotations and code completion for `#!python ListRecommendedActionSummariesPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    filters: Sequence[RecommendedActionFilterTypeDef] = ...,  # (1)
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (2)
) -> aiobotocore.paginate.AioPageIterator[ListRecommendedActionSummariesResponseTypeDef]:  # (3)
    ...
```

1. See `Sequence[RecommendedActionFilterTypeDef]`
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
3. See `AioPageIterator[ListRecommendedActionSummariesResponseTypeDef]`


```python
# paginate method usage example with argument unpacking

kwargs: ListRecommendedActionSummariesRequestPaginateTypeDef = {  # (1)
    "filters": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListRecommendedActionSummariesRequestPaginateTypeDef](./type_defs.md#listrecommendedactionsummariesrequestpaginatetypedef)
## ListRecommendedActionsPaginator

Type annotations and code completion for `#!python session.create_client("compute-optimizer-automation").get_paginator("list_recommended_actions")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/compute-optimizer-automation/paginator/ListRecommendedActions.html#ComputeOptimizerAutomation.Paginator.ListRecommendedActions)

```python
# ListRecommendedActionsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_compute_optimizer_automation.paginator import ListRecommendedActionsPaginator

session = get_session()
async with session.create_client("compute-optimizer-automation") as client:  # (1)
    paginator: ListRecommendedActionsPaginator = client.get_paginator("list_recommended_actions")  # (2)
    async for item in paginator.paginate(...):
        item: ListRecommendedActionsResponseTypeDef
        print(item)  # (3)
```

1. client: [ComputeOptimizerAutomationClient](./client.md)
2. paginator: [ListRecommendedActionsPaginator](./paginators.md#listrecommendedactionspaginator)
3. item: `AioPageIterator[ListRecommendedActionsResponseTypeDef]`


### paginate

Type annotations and code completion for `#!python ListRecommendedActionsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    filters: Sequence[RecommendedActionFilterTypeDef] = ...,  # (1)
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (2)
) -> aiobotocore.paginate.AioPageIterator[ListRecommendedActionsResponseTypeDef]:  # (3)
    ...
```

1. See `Sequence[RecommendedActionFilterTypeDef]`
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
3. See `AioPageIterator[ListRecommendedActionsResponseTypeDef]`


```python
# paginate method usage example with argument unpacking

kwargs: ListRecommendedActionsRequestPaginateTypeDef = {  # (1)
    "filters": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListRecommendedActionsRequestPaginateTypeDef](./type_defs.md#listrecommendedactionsrequestpaginatetypedef)
