# Examples

> [Index](../README.md) > [TrustedAdvisorPublicAPI](./README.md) > Examples

!!! note ""

    Auto-generated documentation for [TrustedAdvisorPublicAPI](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/trustedadvisor.html#trustedadvisorpublicapi)
    type annotations stubs module [types-aiobotocore-trustedadvisor](https://pypi.org/project/types-aiobotocore-trustedadvisor/).

## Client

### Implicit type annotations

Can be used with `types-aiobotocore[trustedadvisor]` package installed.

Write your `TrustedAdvisorPublicAPI` code as usual,
type checking and code completion should work out of the box.



```python
# TrustedAdvisorPublicAPIClient usage example

from aiobotocore.session import get_session


session = get_session()

async with session.create_client("trustedadvisor") as client:  # (1)
    result = await client.batch_update_recommendation_resource_exclusion()  # (2)
```

1. client: [TrustedAdvisorPublicAPIClient](./client.md)
2. result: [:material-code-braces: BatchUpdateRecommendationResourceExclusionResponseTypeDef](./type_defs.md#batchupdaterecommendationresourceexclusionresponsetypedef) 



```python
# ListChecksPaginator usage example

from aiobotocore.session import get_session


session = get_session()

async with session.create_client("trustedadvisor") as client:  # (1)
    paginator = client.get_paginator("list_checks")  # (2)
    async for item in paginator.paginate(...):
        print(item)  # (3)
```

1. client: [TrustedAdvisorPublicAPIClient](./client.md)
2. paginator: [ListChecksPaginator](./paginators.md#listcheckspaginator)
3. item: [:material-code-braces: ListChecksResponseTypeDef](./type_defs.md#listchecksresponsetypedef) 




### Explicit type annotations

With `types-aiobotocore-lite[trustedadvisor]`
or a standalone `types_aiobotocore_trustedadvisor` package, you have to explicitly specify
`client: TrustedAdvisorPublicAPIClient` type annotation.

All other type annotations are optional, as types should be discovered automatically.
However, these type annotations can be helpful in your functions and methods.


```python
# TrustedAdvisorPublicAPIClient usage example with type annotations

from aiobotocore.session import get_session

from types_aiobotocore_trustedadvisor.client import TrustedAdvisorPublicAPIClient
from types_aiobotocore_trustedadvisor.type_defs import BatchUpdateRecommendationResourceExclusionResponseTypeDef
from types_aiobotocore_trustedadvisor.type_defs import BatchUpdateRecommendationResourceExclusionRequestTypeDef


session = get_session()

async with session.create_client("trustedadvisor") as client:
    client: TrustedAdvisorPublicAPIClient
    kwargs: BatchUpdateRecommendationResourceExclusionRequestTypeDef = {...}
    result: BatchUpdateRecommendationResourceExclusionResponseTypeDef = await client.batch_update_recommendation_resource_exclusion(**kwargs)
```



```python
# ListChecksPaginator usage example with type annotations

from aiobotocore.session import get_session

from types_aiobotocore_trustedadvisor.client import TrustedAdvisorPublicAPIClient
from types_aiobotocore_trustedadvisor.paginator import ListChecksPaginator
from types_aiobotocore_trustedadvisor.type_defs import ListChecksResponseTypeDef


session = get_session()

async with session.create_client("trustedadvisor") as client:
    client: TrustedAdvisorPublicAPIClient
    paginator: ListChecksPaginator = client.get_paginator("list_checks")
    async for item in paginator.paginate(...):
        item: ListChecksResponseTypeDef
        print(item)
```


