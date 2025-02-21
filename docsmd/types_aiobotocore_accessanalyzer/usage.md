# Examples

> [Index](../README.md) > [AccessAnalyzer](./README.md) > Examples

!!! note ""

    Auto-generated documentation for [AccessAnalyzer](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/accessanalyzer.html#accessanalyzer)
    type annotations stubs module [types-aiobotocore-accessanalyzer](https://pypi.org/project/types-aiobotocore-accessanalyzer/).

## Client

### Implicit type annotations

Can be used with `types-aiobotocore[accessanalyzer]` package installed.

Write your `AccessAnalyzer` code as usual,
type checking and code completion should work out of the box.



```python
# AccessAnalyzerClient usage example

from aiobotocore.session import get_session


session = get_session()

async with session.create_client("accessanalyzer") as client:  # (1)
    result = await client.apply_archive_rule()  # (2)
```

1. client: [AccessAnalyzerClient](./client.md)
2. result: [:material-code-braces: EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef) 



```python
# GetFindingRecommendationPaginator usage example

from aiobotocore.session import get_session


session = get_session()

async with session.create_client("accessanalyzer") as client:  # (1)
    paginator = client.get_paginator("get_finding_recommendation")  # (2)
    async for item in paginator.paginate(...):
        print(item)  # (3)
```

1. client: [AccessAnalyzerClient](./client.md)
2. paginator: [GetFindingRecommendationPaginator](./paginators.md#getfindingrecommendationpaginator)
3. item: [:material-code-braces: GetFindingRecommendationResponseTypeDef](./type_defs.md#getfindingrecommendationresponsetypedef) 




### Explicit type annotations

With `types-aiobotocore-lite[accessanalyzer]`
or a standalone `types_aiobotocore_accessanalyzer` package, you have to explicitly specify
`client: AccessAnalyzerClient` type annotation.

All other type annotations are optional, as types should be discovered automatically.
However, these type annotations can be helpful in your functions and methods.


```python
# AccessAnalyzerClient usage example with type annotations

from aiobotocore.session import get_session

from types_aiobotocore_accessanalyzer.client import AccessAnalyzerClient
from types_aiobotocore_accessanalyzer.type_defs import EmptyResponseMetadataTypeDef
from types_aiobotocore_accessanalyzer.type_defs import ApplyArchiveRuleRequestTypeDef


session = get_session()

async with session.create_client("accessanalyzer") as client:
    client: AccessAnalyzerClient
    kwargs: ApplyArchiveRuleRequestTypeDef = {...}
    result: EmptyResponseMetadataTypeDef = await client.apply_archive_rule(**kwargs)
```



```python
# GetFindingRecommendationPaginator usage example with type annotations

from aiobotocore.session import get_session

from types_aiobotocore_accessanalyzer.client import AccessAnalyzerClient
from types_aiobotocore_accessanalyzer.paginator import GetFindingRecommendationPaginator
from types_aiobotocore_accessanalyzer.type_defs import GetFindingRecommendationResponseTypeDef


session = get_session()

async with session.create_client("accessanalyzer") as client:
    client: AccessAnalyzerClient
    paginator: GetFindingRecommendationPaginator = client.get_paginator("get_finding_recommendation")
    async for item in paginator.paginate(...):
        item: GetFindingRecommendationResponseTypeDef
        print(item)
```


