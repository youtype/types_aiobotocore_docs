# PersonalizeRuntimeClient

> [Index](../README.md) > [PersonalizeRuntime](./README.md) > PersonalizeRuntimeClient

!!! note ""

    Auto-generated documentation for [PersonalizeRuntime](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/personalize-runtime.html#PersonalizeRuntime)
    type annotations stubs module [types-aiobotocore-personalize-runtime](https://pypi.org/project/types-aiobotocore-personalize-runtime/).

## PersonalizeRuntimeClient

Type annotations and code completion for `#!python session.create_client("personalize-runtime")`
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/personalize-runtime.html#PersonalizeRuntime.Client)

```python title="Usage example"
from aiobotocore.session import get_session
from types_aiobotocore_personalize_runtime.client import PersonalizeRuntimeClient

session = get_session()
async with session.create_client("personalize-runtime") as client:
    client: PersonalizeRuntimeClient
```

## Exceptions


`aiobotocore` client exceptions are generated in runtime.
This class provides code completion for `#!python session.create_client("personalize-runtime").exceptions` structure.

```python title="Usage example"
async with session.create_client("personalize-runtime") as client:
    try:
        do_something(client)
    except (
            client.ClientError,
        client.InvalidInputException,
        client.ResourceNotFoundException,
    ) as e:
        print(e)
```

```python title="Type checking example"
from types_aiobotocore_personalize_runtime.client import Exceptions

def handle_error(exc: Exceptions.ClientError) -> None:
    ...
```


## Methods


### can\_paginate

Check if an operation can be paginated.

Type annotations and code completion for `#!python session.create_client("personalize-runtime").can_paginate` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/personalize-runtime.html#PersonalizeRuntime.Client.can_paginate)

```python title="Method definition"
def can_paginate(
    self,
    operation_name: str,
) -> bool:
    ...
```


### close

Closes underlying endpoint connections.

Type annotations and code completion for `#!python session.create_client("personalize-runtime").close` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/personalize-runtime.html#PersonalizeRuntime.Client.close)

```python title="Method definition"
await def close(
    self,
) -> None:
    ...
```


### generate\_presigned\_url

Generate a presigned url given a client, its method, and arguments.

Type annotations and code completion for `#!python session.create_client("personalize-runtime").generate_presigned_url` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/personalize-runtime.html#PersonalizeRuntime.Client.generate_presigned_url)

```python title="Method definition"
await def generate_presigned_url(
    self,
    ClientMethod: str,
    Params: Mapping[str, Any] = ...,
    ExpiresIn: int = 3600,
    HttpMethod: str = ...,
) -> str:
    ...
```


### get\_personalized\_ranking

Re-ranks a list of recommended items for the given user.

Type annotations and code completion for `#!python session.create_client("personalize-runtime").get_personalized_ranking` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/personalize-runtime.html#PersonalizeRuntime.Client.get_personalized_ranking)

```python title="Method definition"
await def get_personalized_ranking(
    self,
    *,
    campaignArn: str,
    inputList: Sequence[str],
    userId: str,
    context: Mapping[str, str] = ...,
    filterArn: str = ...,
    filterValues: Mapping[str, str] = ...,
) -> GetPersonalizedRankingResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetPersonalizedRankingResponseTypeDef](./type_defs.md#getpersonalizedrankingresponsetypedef) 


```python title="Usage example with kwargs"
kwargs: GetPersonalizedRankingRequestRequestTypeDef = {  # (1)
    "campaignArn": ...,
    "inputList": ...,
    "userId": ...,
}

parent.get_personalized_ranking(**kwargs)
```

1. See [:material-code-braces: GetPersonalizedRankingRequestRequestTypeDef](./type_defs.md#getpersonalizedrankingrequestrequesttypedef) 

### get\_recommendations

Returns a list of recommended items.

Type annotations and code completion for `#!python session.create_client("personalize-runtime").get_recommendations` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/personalize-runtime.html#PersonalizeRuntime.Client.get_recommendations)

```python title="Method definition"
await def get_recommendations(
    self,
    *,
    campaignArn: str = ...,
    itemId: str = ...,
    userId: str = ...,
    numResults: int = ...,
    context: Mapping[str, str] = ...,
    filterArn: str = ...,
    filterValues: Mapping[str, str] = ...,
    recommenderArn: str = ...,
    promotions: Sequence[PromotionTypeDef] = ...,  # (1)
) -> GetRecommendationsResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: PromotionTypeDef](./type_defs.md#promotiontypedef) 
2. See [:material-code-braces: GetRecommendationsResponseTypeDef](./type_defs.md#getrecommendationsresponsetypedef) 


```python title="Usage example with kwargs"
kwargs: GetRecommendationsRequestRequestTypeDef = {  # (1)
    "campaignArn": ...,
}

parent.get_recommendations(**kwargs)
```

1. See [:material-code-braces: GetRecommendationsRequestRequestTypeDef](./type_defs.md#getrecommendationsrequestrequesttypedef) 

### \_\_aenter\_\_



Type annotations and code completion for `#!python session.create_client("personalize-runtime").__aenter__` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/personalize-runtime.html#PersonalizeRuntime.Client.__aenter__)

```python title="Method definition"
await def __aenter__(
    self,
) -> PersonalizeRuntimeClient:
    ...
```


### \_\_aexit\_\_



Type annotations and code completion for `#!python session.create_client("personalize-runtime").__aexit__` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/personalize-runtime.html#PersonalizeRuntime.Client.__aexit__)

```python title="Method definition"
await def __aexit__(
    self,
    exc_type: Any,
    exc_val: Any,
    exc_tb: Any,
) -> Any:
    ...
```





