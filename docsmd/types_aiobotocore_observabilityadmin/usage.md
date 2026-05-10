# Examples

> [Index](../README.md) > [CloudWatchObservabilityAdminService](./README.md) > Examples

!!! note ""

    Auto-generated documentation for [CloudWatchObservabilityAdminService](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/observabilityadmin.html#cloudwatchobservabilityadminservice)
    type annotations stubs module [types-aiobotocore-observabilityadmin](https://pypi.org/project/types-aiobotocore-observabilityadmin/).

## Client

### Implicit type annotations

Can be used with `types-aiobotocore[observabilityadmin]` package installed.

Write your `CloudWatchObservabilityAdminService` code as usual,
type checking and code completion should work out of the box.



#### Client method usage example

```python
# CloudWatchObservabilityAdminServiceClient usage example

from aiobotocore.session import get_session


session = get_session()

async with session.create_client("observabilityadmin") as client:  # (1)
    result = await client.create_centralization_rule_for_organization()  # (2)
```

1. client: [CloudWatchObservabilityAdminServiceClient](./client.md)
2. result: [:material-code-braces: CreateCentralizationRuleForOrganizationOutputTypeDef](./type_defs.md#createcentralizationrulefororganizationoutputtypedef)



#### Paginator usage example

```python
# ListCentralizationRulesForOrganizationPaginator usage example

from aiobotocore.session import get_session


session = get_session()

async with session.create_client("observabilityadmin") as client:  # (1)
    paginator = client.get_paginator("list_centralization_rules_for_organization")  # (2)
    async for item in paginator.paginate(...):
        print(item)  # (3)
```

1. client: [CloudWatchObservabilityAdminServiceClient](./client.md)
2. paginator: [ListCentralizationRulesForOrganizationPaginator](./paginators.md#listcentralizationrulesfororganizationpaginator)
3. item: [:material-code-braces: ListCentralizationRulesForOrganizationOutputTypeDef](./type_defs.md#listcentralizationrulesfororganizationoutputtypedef)




### Explicit type annotations

With `types-aiobotocore-lite[observabilityadmin]`
or a standalone `types_aiobotocore_observabilityadmin` package, you have to explicitly specify
`client: CloudWatchObservabilityAdminServiceClient` type annotation.

All other type annotations are optional, as types should be discovered automatically.
However, these type annotations can be helpful in your functions and methods.


#### Client method usage example

```python
# CloudWatchObservabilityAdminServiceClient usage example with type annotations

from aiobotocore.session import get_session

from types_aiobotocore_observabilityadmin.client import CloudWatchObservabilityAdminServiceClient
from types_aiobotocore_observabilityadmin.type_defs import CreateCentralizationRuleForOrganizationOutputTypeDef
from types_aiobotocore_observabilityadmin.type_defs import CreateCentralizationRuleForOrganizationInputTypeDef


session = get_session()

async with session.create_client("observabilityadmin") as client:
    client: CloudWatchObservabilityAdminServiceClient
    kwargs: CreateCentralizationRuleForOrganizationInputTypeDef = {...}
    result: CreateCentralizationRuleForOrganizationOutputTypeDef = await client.create_centralization_rule_for_organization(**kwargs)
```



#### Paginator usage example

```python
# ListCentralizationRulesForOrganizationPaginator usage example with type annotations

from aiobotocore.session import get_session

from types_aiobotocore_observabilityadmin.client import CloudWatchObservabilityAdminServiceClient
from types_aiobotocore_observabilityadmin.paginator import ListCentralizationRulesForOrganizationPaginator
from types_aiobotocore_observabilityadmin.type_defs import ListCentralizationRulesForOrganizationOutputTypeDef


session = get_session()

async with session.create_client("observabilityadmin") as client:
    client: CloudWatchObservabilityAdminServiceClient
    paginator: ListCentralizationRulesForOrganizationPaginator = client.get_paginator("list_centralization_rules_for_organization")
    async for item in paginator.paginate(...):
        item: ListCentralizationRulesForOrganizationOutputTypeDef
        print(item)
```


