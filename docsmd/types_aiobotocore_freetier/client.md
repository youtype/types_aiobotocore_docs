# FreeTierClient

> [Index](../README.md) > [FreeTier](./README.md) > FreeTierClient

!!! note ""

    Auto-generated documentation for [FreeTier](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/freetier.html#freetier)
    type annotations stubs module [types-aiobotocore-freetier](https://pypi.org/project/types-aiobotocore-freetier/).

## FreeTierClient

Type annotations and code completion for `#!python session.create_client("freetier")`
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/freetier.html#FreeTier.Client)

```python
# FreeTierClient usage example

from aiobotocore.session import get_session
from types_aiobotocore_freetier.client import FreeTierClient

session = get_session()
async with session.create_client("freetier") as client:
    client: FreeTierClient
```

## Exceptions


`aiobotocore` client exceptions are generated in runtime.
This class provides code completion for `#!python session.create_client("freetier").exceptions` structure.

```python
# FreeTierClient.exceptions usage example

async with session.create_client("freetier") as client:
    try:
        do_something(client)
    except (
            client.ClientError,
        client.InternalServerException,
        client.ThrottlingException,
        client.ValidationException,
    ) as e:
        print(e)
```

```python
# FreeTierClient usage type checking example

from types_aiobotocore_freetier.client import Exceptions

def handle_error(exc: Exceptions.ClientError) -> None:
    ...
```


## Methods


### can\_paginate



Type annotations and code completion for `#!python session.create_client("freetier").can_paginate` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/freetier/client/can_paginate.html)

```python
# can_paginate method definition

def can_paginate(
    self,
    operation_name: str,
) -> bool:
    ...
```


### generate\_presigned\_url



Type annotations and code completion for `#!python session.create_client("freetier").generate_presigned_url` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/freetier/client/generate_presigned_url.html)

```python
# generate_presigned_url method definition

await def generate_presigned_url(
    self,
    ClientMethod: str,
    Params: Mapping[str, Any] = ...,
    ExpiresIn: int = 3600,
    HttpMethod: str = ...,
) -> str:
    ...
```


### get\_free\_tier\_usage

Returns a list of all Free Tier usage objects that match your filters.

Type annotations and code completion for `#!python session.create_client("freetier").get_free_tier_usage` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/freetier/client/get_free_tier_usage.html)

```python
# get_free_tier_usage method definition

await def get_free_tier_usage(
    self,
    *,
    filter: ExpressionTypeDef = ...,  # (1)
    maxResults: int = ...,
    nextToken: str = ...,
) -> GetFreeTierUsageResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: ExpressionTypeDef](./type_defs.md#expressiontypedef) 
2. See [:material-code-braces: GetFreeTierUsageResponseTypeDef](./type_defs.md#getfreetierusageresponsetypedef) 


```python
# get_free_tier_usage method usage example with argument unpacking

kwargs: GetFreeTierUsageRequestTypeDef = {  # (1)
    "filter": ...,
}

parent.get_free_tier_usage(**kwargs)
```

1. See [:material-code-braces: GetFreeTierUsageRequestTypeDef](./type_defs.md#getfreetierusagerequesttypedef) 

### \_\_aenter\_\_



Type annotations and code completion for `#!python session.create_client("freetier").__aenter__` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/freetier.html#FreeTier.Client)

```python
# __aenter__ method definition

await def __aenter__(
    self,
) -> Self:
    ...
```


### \_\_aexit\_\_



Type annotations and code completion for `#!python session.create_client("freetier").__aexit__` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/freetier.html#FreeTier.Client)

```python
# __aexit__ method definition

await def __aexit__(
    self,
    exc_type: Union[Type[BaseException], None],
    exc_val: Union[BaseException, None],
    exc_tb: Union[TracebackType, None],
) -> None:
    ...
```




### get_paginator

Type annotations and code completion for `#!python session.create_client("freetier").get_paginator` method with overloads.

- `client.get_paginator("get_free_tier_usage")` -> [GetFreeTierUsagePaginator](./paginators.md#getfreetierusagepaginator)



