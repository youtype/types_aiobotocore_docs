# Paginators

> [Index](../README.md) > [WAF](./README.md) > Paginators

!!! note ""

    Auto-generated documentation for [WAF](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/waf.html#waf)
    type annotations stubs module [types-aiobotocore-waf](https://pypi.org/project/types-aiobotocore-waf/).

## GetRateBasedRuleManagedKeysPaginator

Type annotations and code completion for `#!python session.create_client("waf").get_paginator("get_rate_based_rule_managed_keys")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/waf/paginator/GetRateBasedRuleManagedKeys.html#WAF.Paginator.GetRateBasedRuleManagedKeys)

```python
# GetRateBasedRuleManagedKeysPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_waf.paginator import GetRateBasedRuleManagedKeysPaginator

session = get_session()
async with session.create_client("waf") as client:  # (1)
    paginator: GetRateBasedRuleManagedKeysPaginator = client.get_paginator("get_rate_based_rule_managed_keys")  # (2)
    async for item in paginator.paginate(...):
        item: GetRateBasedRuleManagedKeysResponseTypeDef
        print(item)  # (3)
```

1. client: [WAFClient](./client.md)
2. paginator: [GetRateBasedRuleManagedKeysPaginator](./paginators.md#getratebasedrulemanagedkeyspaginator)
3. item: [:material-code-braces: GetRateBasedRuleManagedKeysResponseTypeDef](./type_defs.md#getratebasedrulemanagedkeysresponsetypedef) 


### paginate

Type annotations and code completion for `#!python GetRateBasedRuleManagedKeysPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    RuleId: str,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AioPageIterator[GetRateBasedRuleManagedKeysResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: GetRateBasedRuleManagedKeysResponseTypeDef](./type_defs.md#getratebasedrulemanagedkeysresponsetypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: GetRateBasedRuleManagedKeysRequestPaginateTypeDef = {  # (1)
    "RuleId": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: GetRateBasedRuleManagedKeysRequestPaginateTypeDef](./type_defs.md#getratebasedrulemanagedkeysrequestpaginatetypedef) 
## ListActivatedRulesInRuleGroupPaginator

Type annotations and code completion for `#!python session.create_client("waf").get_paginator("list_activated_rules_in_rule_group")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/waf/paginator/ListActivatedRulesInRuleGroup.html#WAF.Paginator.ListActivatedRulesInRuleGroup)

```python
# ListActivatedRulesInRuleGroupPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_waf.paginator import ListActivatedRulesInRuleGroupPaginator

session = get_session()
async with session.create_client("waf") as client:  # (1)
    paginator: ListActivatedRulesInRuleGroupPaginator = client.get_paginator("list_activated_rules_in_rule_group")  # (2)
    async for item in paginator.paginate(...):
        item: ListActivatedRulesInRuleGroupResponseTypeDef
        print(item)  # (3)
```

1. client: [WAFClient](./client.md)
2. paginator: [ListActivatedRulesInRuleGroupPaginator](./paginators.md#listactivatedrulesinrulegrouppaginator)
3. item: [:material-code-braces: ListActivatedRulesInRuleGroupResponseTypeDef](./type_defs.md#listactivatedrulesinrulegroupresponsetypedef) 


### paginate

Type annotations and code completion for `#!python ListActivatedRulesInRuleGroupPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    RuleGroupId: str = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AioPageIterator[ListActivatedRulesInRuleGroupResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListActivatedRulesInRuleGroupResponseTypeDef](./type_defs.md#listactivatedrulesinrulegroupresponsetypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: ListActivatedRulesInRuleGroupRequestPaginateTypeDef = {  # (1)
    "RuleGroupId": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListActivatedRulesInRuleGroupRequestPaginateTypeDef](./type_defs.md#listactivatedrulesinrulegrouprequestpaginatetypedef) 
## ListByteMatchSetsPaginator

Type annotations and code completion for `#!python session.create_client("waf").get_paginator("list_byte_match_sets")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/waf/paginator/ListByteMatchSets.html#WAF.Paginator.ListByteMatchSets)

```python
# ListByteMatchSetsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_waf.paginator import ListByteMatchSetsPaginator

session = get_session()
async with session.create_client("waf") as client:  # (1)
    paginator: ListByteMatchSetsPaginator = client.get_paginator("list_byte_match_sets")  # (2)
    async for item in paginator.paginate(...):
        item: ListByteMatchSetsResponseTypeDef
        print(item)  # (3)
```

1. client: [WAFClient](./client.md)
2. paginator: [ListByteMatchSetsPaginator](./paginators.md#listbytematchsetspaginator)
3. item: [:material-code-braces: ListByteMatchSetsResponseTypeDef](./type_defs.md#listbytematchsetsresponsetypedef) 


### paginate

Type annotations and code completion for `#!python ListByteMatchSetsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AioPageIterator[ListByteMatchSetsResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListByteMatchSetsResponseTypeDef](./type_defs.md#listbytematchsetsresponsetypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: ListByteMatchSetsRequestPaginateTypeDef = {  # (1)
    "PaginationConfig": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListByteMatchSetsRequestPaginateTypeDef](./type_defs.md#listbytematchsetsrequestpaginatetypedef) 
## ListGeoMatchSetsPaginator

Type annotations and code completion for `#!python session.create_client("waf").get_paginator("list_geo_match_sets")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/waf/paginator/ListGeoMatchSets.html#WAF.Paginator.ListGeoMatchSets)

```python
# ListGeoMatchSetsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_waf.paginator import ListGeoMatchSetsPaginator

session = get_session()
async with session.create_client("waf") as client:  # (1)
    paginator: ListGeoMatchSetsPaginator = client.get_paginator("list_geo_match_sets")  # (2)
    async for item in paginator.paginate(...):
        item: ListGeoMatchSetsResponseTypeDef
        print(item)  # (3)
```

1. client: [WAFClient](./client.md)
2. paginator: [ListGeoMatchSetsPaginator](./paginators.md#listgeomatchsetspaginator)
3. item: [:material-code-braces: ListGeoMatchSetsResponseTypeDef](./type_defs.md#listgeomatchsetsresponsetypedef) 


### paginate

Type annotations and code completion for `#!python ListGeoMatchSetsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AioPageIterator[ListGeoMatchSetsResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListGeoMatchSetsResponseTypeDef](./type_defs.md#listgeomatchsetsresponsetypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: ListGeoMatchSetsRequestPaginateTypeDef = {  # (1)
    "PaginationConfig": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListGeoMatchSetsRequestPaginateTypeDef](./type_defs.md#listgeomatchsetsrequestpaginatetypedef) 
## ListIPSetsPaginator

Type annotations and code completion for `#!python session.create_client("waf").get_paginator("list_ip_sets")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/waf/paginator/ListIPSets.html#WAF.Paginator.ListIPSets)

```python
# ListIPSetsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_waf.paginator import ListIPSetsPaginator

session = get_session()
async with session.create_client("waf") as client:  # (1)
    paginator: ListIPSetsPaginator = client.get_paginator("list_ip_sets")  # (2)
    async for item in paginator.paginate(...):
        item: ListIPSetsResponseTypeDef
        print(item)  # (3)
```

1. client: [WAFClient](./client.md)
2. paginator: [ListIPSetsPaginator](./paginators.md#listipsetspaginator)
3. item: [:material-code-braces: ListIPSetsResponseTypeDef](./type_defs.md#listipsetsresponsetypedef) 


### paginate

Type annotations and code completion for `#!python ListIPSetsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AioPageIterator[ListIPSetsResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListIPSetsResponseTypeDef](./type_defs.md#listipsetsresponsetypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: ListIPSetsRequestPaginateTypeDef = {  # (1)
    "PaginationConfig": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListIPSetsRequestPaginateTypeDef](./type_defs.md#listipsetsrequestpaginatetypedef) 
## ListLoggingConfigurationsPaginator

Type annotations and code completion for `#!python session.create_client("waf").get_paginator("list_logging_configurations")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/waf/paginator/ListLoggingConfigurations.html#WAF.Paginator.ListLoggingConfigurations)

```python
# ListLoggingConfigurationsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_waf.paginator import ListLoggingConfigurationsPaginator

session = get_session()
async with session.create_client("waf") as client:  # (1)
    paginator: ListLoggingConfigurationsPaginator = client.get_paginator("list_logging_configurations")  # (2)
    async for item in paginator.paginate(...):
        item: ListLoggingConfigurationsResponseTypeDef
        print(item)  # (3)
```

1. client: [WAFClient](./client.md)
2. paginator: [ListLoggingConfigurationsPaginator](./paginators.md#listloggingconfigurationspaginator)
3. item: [:material-code-braces: ListLoggingConfigurationsResponseTypeDef](./type_defs.md#listloggingconfigurationsresponsetypedef) 


### paginate

Type annotations and code completion for `#!python ListLoggingConfigurationsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AioPageIterator[ListLoggingConfigurationsResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListLoggingConfigurationsResponseTypeDef](./type_defs.md#listloggingconfigurationsresponsetypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: ListLoggingConfigurationsRequestPaginateTypeDef = {  # (1)
    "PaginationConfig": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListLoggingConfigurationsRequestPaginateTypeDef](./type_defs.md#listloggingconfigurationsrequestpaginatetypedef) 
## ListRateBasedRulesPaginator

Type annotations and code completion for `#!python session.create_client("waf").get_paginator("list_rate_based_rules")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/waf/paginator/ListRateBasedRules.html#WAF.Paginator.ListRateBasedRules)

```python
# ListRateBasedRulesPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_waf.paginator import ListRateBasedRulesPaginator

session = get_session()
async with session.create_client("waf") as client:  # (1)
    paginator: ListRateBasedRulesPaginator = client.get_paginator("list_rate_based_rules")  # (2)
    async for item in paginator.paginate(...):
        item: ListRateBasedRulesResponseTypeDef
        print(item)  # (3)
```

1. client: [WAFClient](./client.md)
2. paginator: [ListRateBasedRulesPaginator](./paginators.md#listratebasedrulespaginator)
3. item: [:material-code-braces: ListRateBasedRulesResponseTypeDef](./type_defs.md#listratebasedrulesresponsetypedef) 


### paginate

Type annotations and code completion for `#!python ListRateBasedRulesPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AioPageIterator[ListRateBasedRulesResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListRateBasedRulesResponseTypeDef](./type_defs.md#listratebasedrulesresponsetypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: ListRateBasedRulesRequestPaginateTypeDef = {  # (1)
    "PaginationConfig": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListRateBasedRulesRequestPaginateTypeDef](./type_defs.md#listratebasedrulesrequestpaginatetypedef) 
## ListRegexMatchSetsPaginator

Type annotations and code completion for `#!python session.create_client("waf").get_paginator("list_regex_match_sets")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/waf/paginator/ListRegexMatchSets.html#WAF.Paginator.ListRegexMatchSets)

```python
# ListRegexMatchSetsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_waf.paginator import ListRegexMatchSetsPaginator

session = get_session()
async with session.create_client("waf") as client:  # (1)
    paginator: ListRegexMatchSetsPaginator = client.get_paginator("list_regex_match_sets")  # (2)
    async for item in paginator.paginate(...):
        item: ListRegexMatchSetsResponseTypeDef
        print(item)  # (3)
```

1. client: [WAFClient](./client.md)
2. paginator: [ListRegexMatchSetsPaginator](./paginators.md#listregexmatchsetspaginator)
3. item: [:material-code-braces: ListRegexMatchSetsResponseTypeDef](./type_defs.md#listregexmatchsetsresponsetypedef) 


### paginate

Type annotations and code completion for `#!python ListRegexMatchSetsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AioPageIterator[ListRegexMatchSetsResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListRegexMatchSetsResponseTypeDef](./type_defs.md#listregexmatchsetsresponsetypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: ListRegexMatchSetsRequestPaginateTypeDef = {  # (1)
    "PaginationConfig": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListRegexMatchSetsRequestPaginateTypeDef](./type_defs.md#listregexmatchsetsrequestpaginatetypedef) 
## ListRegexPatternSetsPaginator

Type annotations and code completion for `#!python session.create_client("waf").get_paginator("list_regex_pattern_sets")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/waf/paginator/ListRegexPatternSets.html#WAF.Paginator.ListRegexPatternSets)

```python
# ListRegexPatternSetsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_waf.paginator import ListRegexPatternSetsPaginator

session = get_session()
async with session.create_client("waf") as client:  # (1)
    paginator: ListRegexPatternSetsPaginator = client.get_paginator("list_regex_pattern_sets")  # (2)
    async for item in paginator.paginate(...):
        item: ListRegexPatternSetsResponseTypeDef
        print(item)  # (3)
```

1. client: [WAFClient](./client.md)
2. paginator: [ListRegexPatternSetsPaginator](./paginators.md#listregexpatternsetspaginator)
3. item: [:material-code-braces: ListRegexPatternSetsResponseTypeDef](./type_defs.md#listregexpatternsetsresponsetypedef) 


### paginate

Type annotations and code completion for `#!python ListRegexPatternSetsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AioPageIterator[ListRegexPatternSetsResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListRegexPatternSetsResponseTypeDef](./type_defs.md#listregexpatternsetsresponsetypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: ListRegexPatternSetsRequestPaginateTypeDef = {  # (1)
    "PaginationConfig": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListRegexPatternSetsRequestPaginateTypeDef](./type_defs.md#listregexpatternsetsrequestpaginatetypedef) 
## ListRuleGroupsPaginator

Type annotations and code completion for `#!python session.create_client("waf").get_paginator("list_rule_groups")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/waf/paginator/ListRuleGroups.html#WAF.Paginator.ListRuleGroups)

```python
# ListRuleGroupsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_waf.paginator import ListRuleGroupsPaginator

session = get_session()
async with session.create_client("waf") as client:  # (1)
    paginator: ListRuleGroupsPaginator = client.get_paginator("list_rule_groups")  # (2)
    async for item in paginator.paginate(...):
        item: ListRuleGroupsResponseTypeDef
        print(item)  # (3)
```

1. client: [WAFClient](./client.md)
2. paginator: [ListRuleGroupsPaginator](./paginators.md#listrulegroupspaginator)
3. item: [:material-code-braces: ListRuleGroupsResponseTypeDef](./type_defs.md#listrulegroupsresponsetypedef) 


### paginate

Type annotations and code completion for `#!python ListRuleGroupsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AioPageIterator[ListRuleGroupsResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListRuleGroupsResponseTypeDef](./type_defs.md#listrulegroupsresponsetypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: ListRuleGroupsRequestPaginateTypeDef = {  # (1)
    "PaginationConfig": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListRuleGroupsRequestPaginateTypeDef](./type_defs.md#listrulegroupsrequestpaginatetypedef) 
## ListRulesPaginator

Type annotations and code completion for `#!python session.create_client("waf").get_paginator("list_rules")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/waf/paginator/ListRules.html#WAF.Paginator.ListRules)

```python
# ListRulesPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_waf.paginator import ListRulesPaginator

session = get_session()
async with session.create_client("waf") as client:  # (1)
    paginator: ListRulesPaginator = client.get_paginator("list_rules")  # (2)
    async for item in paginator.paginate(...):
        item: ListRulesResponseTypeDef
        print(item)  # (3)
```

1. client: [WAFClient](./client.md)
2. paginator: [ListRulesPaginator](./paginators.md#listrulespaginator)
3. item: [:material-code-braces: ListRulesResponseTypeDef](./type_defs.md#listrulesresponsetypedef) 


### paginate

Type annotations and code completion for `#!python ListRulesPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AioPageIterator[ListRulesResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListRulesResponseTypeDef](./type_defs.md#listrulesresponsetypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: ListRulesRequestPaginateTypeDef = {  # (1)
    "PaginationConfig": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListRulesRequestPaginateTypeDef](./type_defs.md#listrulesrequestpaginatetypedef) 
## ListSizeConstraintSetsPaginator

Type annotations and code completion for `#!python session.create_client("waf").get_paginator("list_size_constraint_sets")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/waf/paginator/ListSizeConstraintSets.html#WAF.Paginator.ListSizeConstraintSets)

```python
# ListSizeConstraintSetsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_waf.paginator import ListSizeConstraintSetsPaginator

session = get_session()
async with session.create_client("waf") as client:  # (1)
    paginator: ListSizeConstraintSetsPaginator = client.get_paginator("list_size_constraint_sets")  # (2)
    async for item in paginator.paginate(...):
        item: ListSizeConstraintSetsResponseTypeDef
        print(item)  # (3)
```

1. client: [WAFClient](./client.md)
2. paginator: [ListSizeConstraintSetsPaginator](./paginators.md#listsizeconstraintsetspaginator)
3. item: [:material-code-braces: ListSizeConstraintSetsResponseTypeDef](./type_defs.md#listsizeconstraintsetsresponsetypedef) 


### paginate

Type annotations and code completion for `#!python ListSizeConstraintSetsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AioPageIterator[ListSizeConstraintSetsResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListSizeConstraintSetsResponseTypeDef](./type_defs.md#listsizeconstraintsetsresponsetypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: ListSizeConstraintSetsRequestPaginateTypeDef = {  # (1)
    "PaginationConfig": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListSizeConstraintSetsRequestPaginateTypeDef](./type_defs.md#listsizeconstraintsetsrequestpaginatetypedef) 
## ListSqlInjectionMatchSetsPaginator

Type annotations and code completion for `#!python session.create_client("waf").get_paginator("list_sql_injection_match_sets")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/waf/paginator/ListSqlInjectionMatchSets.html#WAF.Paginator.ListSqlInjectionMatchSets)

```python
# ListSqlInjectionMatchSetsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_waf.paginator import ListSqlInjectionMatchSetsPaginator

session = get_session()
async with session.create_client("waf") as client:  # (1)
    paginator: ListSqlInjectionMatchSetsPaginator = client.get_paginator("list_sql_injection_match_sets")  # (2)
    async for item in paginator.paginate(...):
        item: ListSqlInjectionMatchSetsResponseTypeDef
        print(item)  # (3)
```

1. client: [WAFClient](./client.md)
2. paginator: [ListSqlInjectionMatchSetsPaginator](./paginators.md#listsqlinjectionmatchsetspaginator)
3. item: [:material-code-braces: ListSqlInjectionMatchSetsResponseTypeDef](./type_defs.md#listsqlinjectionmatchsetsresponsetypedef) 


### paginate

Type annotations and code completion for `#!python ListSqlInjectionMatchSetsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AioPageIterator[ListSqlInjectionMatchSetsResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListSqlInjectionMatchSetsResponseTypeDef](./type_defs.md#listsqlinjectionmatchsetsresponsetypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: ListSqlInjectionMatchSetsRequestPaginateTypeDef = {  # (1)
    "PaginationConfig": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListSqlInjectionMatchSetsRequestPaginateTypeDef](./type_defs.md#listsqlinjectionmatchsetsrequestpaginatetypedef) 
## ListSubscribedRuleGroupsPaginator

Type annotations and code completion for `#!python session.create_client("waf").get_paginator("list_subscribed_rule_groups")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/waf/paginator/ListSubscribedRuleGroups.html#WAF.Paginator.ListSubscribedRuleGroups)

```python
# ListSubscribedRuleGroupsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_waf.paginator import ListSubscribedRuleGroupsPaginator

session = get_session()
async with session.create_client("waf") as client:  # (1)
    paginator: ListSubscribedRuleGroupsPaginator = client.get_paginator("list_subscribed_rule_groups")  # (2)
    async for item in paginator.paginate(...):
        item: ListSubscribedRuleGroupsResponseTypeDef
        print(item)  # (3)
```

1. client: [WAFClient](./client.md)
2. paginator: [ListSubscribedRuleGroupsPaginator](./paginators.md#listsubscribedrulegroupspaginator)
3. item: [:material-code-braces: ListSubscribedRuleGroupsResponseTypeDef](./type_defs.md#listsubscribedrulegroupsresponsetypedef) 


### paginate

Type annotations and code completion for `#!python ListSubscribedRuleGroupsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AioPageIterator[ListSubscribedRuleGroupsResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListSubscribedRuleGroupsResponseTypeDef](./type_defs.md#listsubscribedrulegroupsresponsetypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: ListSubscribedRuleGroupsRequestPaginateTypeDef = {  # (1)
    "PaginationConfig": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListSubscribedRuleGroupsRequestPaginateTypeDef](./type_defs.md#listsubscribedrulegroupsrequestpaginatetypedef) 
## ListWebACLsPaginator

Type annotations and code completion for `#!python session.create_client("waf").get_paginator("list_web_acls")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/waf/paginator/ListWebACLs.html#WAF.Paginator.ListWebACLs)

```python
# ListWebACLsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_waf.paginator import ListWebACLsPaginator

session = get_session()
async with session.create_client("waf") as client:  # (1)
    paginator: ListWebACLsPaginator = client.get_paginator("list_web_acls")  # (2)
    async for item in paginator.paginate(...):
        item: ListWebACLsResponseTypeDef
        print(item)  # (3)
```

1. client: [WAFClient](./client.md)
2. paginator: [ListWebACLsPaginator](./paginators.md#listwebaclspaginator)
3. item: [:material-code-braces: ListWebACLsResponseTypeDef](./type_defs.md#listwebaclsresponsetypedef) 


### paginate

Type annotations and code completion for `#!python ListWebACLsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AioPageIterator[ListWebACLsResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListWebACLsResponseTypeDef](./type_defs.md#listwebaclsresponsetypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: ListWebACLsRequestPaginateTypeDef = {  # (1)
    "PaginationConfig": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListWebACLsRequestPaginateTypeDef](./type_defs.md#listwebaclsrequestpaginatetypedef) 
## ListXssMatchSetsPaginator

Type annotations and code completion for `#!python session.create_client("waf").get_paginator("list_xss_match_sets")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/waf/paginator/ListXssMatchSets.html#WAF.Paginator.ListXssMatchSets)

```python
# ListXssMatchSetsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_waf.paginator import ListXssMatchSetsPaginator

session = get_session()
async with session.create_client("waf") as client:  # (1)
    paginator: ListXssMatchSetsPaginator = client.get_paginator("list_xss_match_sets")  # (2)
    async for item in paginator.paginate(...):
        item: ListXssMatchSetsResponseTypeDef
        print(item)  # (3)
```

1. client: [WAFClient](./client.md)
2. paginator: [ListXssMatchSetsPaginator](./paginators.md#listxssmatchsetspaginator)
3. item: [:material-code-braces: ListXssMatchSetsResponseTypeDef](./type_defs.md#listxssmatchsetsresponsetypedef) 


### paginate

Type annotations and code completion for `#!python ListXssMatchSetsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AioPageIterator[ListXssMatchSetsResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListXssMatchSetsResponseTypeDef](./type_defs.md#listxssmatchsetsresponsetypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: ListXssMatchSetsRequestPaginateTypeDef = {  # (1)
    "PaginationConfig": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListXssMatchSetsRequestPaginateTypeDef](./type_defs.md#listxssmatchsetsrequestpaginatetypedef) 
