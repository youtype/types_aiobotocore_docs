# Paginators

> [Index](../README.md) > [EventBridge](./README.md) > Paginators

!!! note ""

    Auto-generated documentation for [EventBridge](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/events.html#eventbridge)
    type annotations stubs module [types-aiobotocore-events](https://pypi.org/project/types-aiobotocore-events/).

## ListRuleNamesByTargetPaginator

Type annotations and code completion for `#!python session.create_client("events").get_paginator("list_rule_names_by_target")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/events/paginator/ListRuleNamesByTarget.html#EventBridge.Paginator.ListRuleNamesByTarget)

```python
# ListRuleNamesByTargetPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_events.paginator import ListRuleNamesByTargetPaginator

session = get_session()
async with session.create_client("events") as client:  # (1)
    paginator: ListRuleNamesByTargetPaginator = client.get_paginator("list_rule_names_by_target")  # (2)
    async for item in paginator.paginate(...):
        item: ListRuleNamesByTargetResponseTypeDef
        print(item)  # (3)
```

1. client: [EventBridgeClient](./client.md)
2. paginator: [ListRuleNamesByTargetPaginator](./paginators.md#listrulenamesbytargetpaginator)
3. item: `AioPageIterator[ListRuleNamesByTargetResponseTypeDef]`


### paginate

Type annotations and code completion for `#!python ListRuleNamesByTargetPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    TargetArn: str,
    EventBusName: str = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> aiobotocore.paginate.AioPageIterator[ListRuleNamesByTargetResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
2. See `AioPageIterator[ListRuleNamesByTargetResponseTypeDef]`


```python
# paginate method usage example with argument unpacking

kwargs: ListRuleNamesByTargetRequestPaginateTypeDef = {  # (1)
    "TargetArn": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListRuleNamesByTargetRequestPaginateTypeDef](./type_defs.md#listrulenamesbytargetrequestpaginatetypedef)
## ListRulesPaginator

Type annotations and code completion for `#!python session.create_client("events").get_paginator("list_rules")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/events/paginator/ListRules.html#EventBridge.Paginator.ListRules)

```python
# ListRulesPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_events.paginator import ListRulesPaginator

session = get_session()
async with session.create_client("events") as client:  # (1)
    paginator: ListRulesPaginator = client.get_paginator("list_rules")  # (2)
    async for item in paginator.paginate(...):
        item: ListRulesResponseTypeDef
        print(item)  # (3)
```

1. client: [EventBridgeClient](./client.md)
2. paginator: [ListRulesPaginator](./paginators.md#listrulespaginator)
3. item: `AioPageIterator[ListRulesResponseTypeDef]`


### paginate

Type annotations and code completion for `#!python ListRulesPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    NamePrefix: str = ...,
    EventBusName: str = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> aiobotocore.paginate.AioPageIterator[ListRulesResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
2. See `AioPageIterator[ListRulesResponseTypeDef]`


```python
# paginate method usage example with argument unpacking

kwargs: ListRulesRequestPaginateTypeDef = {  # (1)
    "NamePrefix": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListRulesRequestPaginateTypeDef](./type_defs.md#listrulesrequestpaginatetypedef)
## ListTargetsByRulePaginator

Type annotations and code completion for `#!python session.create_client("events").get_paginator("list_targets_by_rule")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/events/paginator/ListTargetsByRule.html#EventBridge.Paginator.ListTargetsByRule)

```python
# ListTargetsByRulePaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_events.paginator import ListTargetsByRulePaginator

session = get_session()
async with session.create_client("events") as client:  # (1)
    paginator: ListTargetsByRulePaginator = client.get_paginator("list_targets_by_rule")  # (2)
    async for item in paginator.paginate(...):
        item: ListTargetsByRuleResponseTypeDef
        print(item)  # (3)
```

1. client: [EventBridgeClient](./client.md)
2. paginator: [ListTargetsByRulePaginator](./paginators.md#listtargetsbyrulepaginator)
3. item: `AioPageIterator[ListTargetsByRuleResponseTypeDef]`


### paginate

Type annotations and code completion for `#!python ListTargetsByRulePaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    Rule: str,
    EventBusName: str = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> aiobotocore.paginate.AioPageIterator[ListTargetsByRuleResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
2. See `AioPageIterator[ListTargetsByRuleResponseTypeDef]`


```python
# paginate method usage example with argument unpacking

kwargs: ListTargetsByRuleRequestPaginateTypeDef = {  # (1)
    "Rule": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListTargetsByRuleRequestPaginateTypeDef](./type_defs.md#listtargetsbyrulerequestpaginatetypedef)
