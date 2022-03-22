<a id="paginators-for-aiobotocore-eventbridge-module"></a>

# Paginators for aiobotocore EventBridge module

> [Index](../README.md) > [EventBridge](./README.md) > Paginators

Auto-generated documentation for
[EventBridge](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/events.html#EventBridge)
type annotations stubs module
[types-aiobotocore-events](https://pypi.org/project/types-aiobotocore-events/).

- [Paginators for aiobotocore EventBridge module](#paginators-for-aiobotocore-eventbridge-module)
  - [ListRuleNamesByTargetPaginator](#listrulenamesbytargetpaginator)
  - [ListRulesPaginator](#listrulespaginator)
  - [ListTargetsByRulePaginator](#listtargetsbyrulepaginator)

<a id="listrulenamesbytargetpaginator"></a>

## ListRuleNamesByTargetPaginator

Type annotations for
`session.create_client("events").get_paginator("list_rule_names_by_target")`.

Can be used directly:

```python
from aiobotocore.session import get_session

from types_aiobotocore_events.paginator import ListRuleNamesByTargetPaginator

session = get_session()
async with session.create_client("events") as client:
    client: EventBridgeClient
    paginator: ListRuleNamesByTargetPaginator = client.get_paginator("list_rule_names_by_target")
```

Boto3 documentation:
[EventBridge.Paginator.ListRuleNamesByTarget](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/events.html#EventBridge.Paginator.ListRuleNamesByTarget)

Arguments for `ListRuleNamesByTargetPaginator.paginate` method:

- `TargetArn`: `str` *(required)*
- `EventBusName`: `str`
- `PaginationConfig`:
  [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)

`ListRuleNamesByTargetPaginator.paginate` returns
`AsyncIterator`\[[ListRuleNamesByTargetResponseTypeDef](./type_defs.md#listrulenamesbytargetresponsetypedef)\].

<a id="listrulespaginator"></a>

## ListRulesPaginator

Type annotations for
`session.create_client("events").get_paginator("list_rules")`.

Can be used directly:

```python
from aiobotocore.session import get_session

from types_aiobotocore_events.paginator import ListRulesPaginator

session = get_session()
async with session.create_client("events") as client:
    client: EventBridgeClient
    paginator: ListRulesPaginator = client.get_paginator("list_rules")
```

Boto3 documentation:
[EventBridge.Paginator.ListRules](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/events.html#EventBridge.Paginator.ListRules)

Arguments for `ListRulesPaginator.paginate` method:

- `NamePrefix`: `str`
- `EventBusName`: `str`
- `PaginationConfig`:
  [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)

`ListRulesPaginator.paginate` returns
`AsyncIterator`\[[ListRulesResponseTypeDef](./type_defs.md#listrulesresponsetypedef)\].

<a id="listtargetsbyrulepaginator"></a>

## ListTargetsByRulePaginator

Type annotations for
`session.create_client("events").get_paginator("list_targets_by_rule")`.

Can be used directly:

```python
from aiobotocore.session import get_session

from types_aiobotocore_events.paginator import ListTargetsByRulePaginator

session = get_session()
async with session.create_client("events") as client:
    client: EventBridgeClient
    paginator: ListTargetsByRulePaginator = client.get_paginator("list_targets_by_rule")
```

Boto3 documentation:
[EventBridge.Paginator.ListTargetsByRule](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/events.html#EventBridge.Paginator.ListTargetsByRule)

Arguments for `ListTargetsByRulePaginator.paginate` method:

- `Rule`: `str` *(required)*
- `EventBusName`: `str`
- `PaginationConfig`:
  [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)

`ListTargetsByRulePaginator.paginate` returns
`AsyncIterator`\[[ListTargetsByRuleResponseTypeDef](./type_defs.md#listtargetsbyruleresponsetypedef)\].
