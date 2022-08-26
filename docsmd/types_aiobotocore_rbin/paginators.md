# Paginators

> [Index](../README.md) > [RecycleBin](./README.md) > Paginators

!!! note ""

    Auto-generated documentation for [RecycleBin](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rbin.html#RecycleBin)
    type annotations stubs module [types-aiobotocore-rbin](https://pypi.org/project/types-aiobotocore-rbin/).

## ListRulesPaginator

Type annotations and code completion for `#!python session.create_client("rbin").get_paginator("list_rules")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rbin.html#RecycleBin.Paginator.ListRules)

```python title="Usage example"
from aiobotocore.session import get_session

from types_aiobotocore_rbin.paginator import ListRulesPaginator

session = get_session()
async with session.create_client("rbin") as client:  # (1)
    paginator: ListRulesPaginator = client.get_paginator("list_rules")  # (2)
    async for item in paginator.paginate(...):
        item: ListRulesResponseTypeDef
        print(item)  # (3)
```

1. client: [RecycleBinClient](./client.md)
2. paginator: [ListRulesPaginator](./paginators.md#listrulespaginator)
3. item: [:material-code-braces: ListRulesResponseTypeDef](./type_defs.md#listrulesresponsetypedef) 


### paginate

Type annotations and code completion for `#!python ListRulesPaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    ResourceType: ResourceTypeType,  # (1)
    ResourceTags: Sequence[ResourceTagTypeDef] = ...,  # (2)
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (3)
) -> AsyncIterator[ListRulesResponseTypeDef]:  # (4)
    ...
```

1. See [:material-code-brackets: ResourceTypeType](./literals.md#resourcetypetype) 
2. See [:material-code-braces: ResourceTagTypeDef](./type_defs.md#resourcetagtypedef) 
3. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
4. See [:material-code-braces: ListRulesResponseTypeDef](./type_defs.md#listrulesresponsetypedef) 


```python title="Usage example with kwargs"
kwargs: ListRulesRequestListRulesPaginateTypeDef = {  # (1)
    "ResourceType": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListRulesRequestListRulesPaginateTypeDef](./type_defs.md#listrulesrequestlistrulespaginatetypedef) 
