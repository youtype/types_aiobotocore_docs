# PersonalizeRuntimeClient

> [Index](../README.md) > [PersonalizeRuntime](./README.md) > PersonalizeRuntimeClient

!!! note ""

    Auto-generated documentation for [PersonalizeRuntime](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/personalize-runtime.html#personalizeruntime)
    type annotations stubs module [types-aiobotocore-personalize-runtime](https://pypi.org/project/types-aiobotocore-personalize-runtime/).

## PersonalizeRuntimeClient

Type annotations and code completion for `#!python session.create_client("personalize-runtime")`
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/personalize-runtime.html#PersonalizeRuntime.Client)

```python
# PersonalizeRuntimeClient usage example

from aiobotocore.session import get_session
from types_aiobotocore_personalize_runtime.client import PersonalizeRuntimeClient

session = get_session()
async with session.create_client("personalize-runtime") as client:
    client: PersonalizeRuntimeClient
```

## Exceptions


`aiobotocore` client exceptions are generated in runtime.
This class provides code completion for `#!python session.create_client("personalize-runtime").exceptions` structure.

```python
# PersonalizeRuntimeClient.exceptions usage example

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

```python
# PersonalizeRuntimeClient usage type checking example

from types_aiobotocore_personalize_runtime.client import Exceptions

def handle_error(exc: Exceptions.ClientError) -> None:
    ...
```


## Methods


### can\_paginate



Type annotations and code completion for `#!python session.create_client("personalize-runtime").can_paginate` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/personalize-runtime/client/can_paginate.html)

```python
# can_paginate method definition

def can_paginate(
    self,
    operation_name: str,
) -> bool:
    ...
```


### generate\_presigned\_url



Type annotations and code completion for `#!python session.create_client("personalize-runtime").generate_presigned_url` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/personalize-runtime/client/generate_presigned_url.html)

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


### get\_action\_recommendations

Returns a list of recommended actions in sorted in descending order by
prediction score.

Type annotations and code completion for `#!python session.create_client("personalize-runtime").get_action_recommendations` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/personalize-runtime/client/get_action_recommendations.html)

```python
# get_action_recommendations method definition

await def get_action_recommendations(
    self,
    *,
    campaignArn: str = ...,
    userId: str = ...,
    numResults: int = ...,
    filterArn: str = ...,
    filterValues: Mapping[str, str] = ...,
) -> GetActionRecommendationsResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetActionRecommendationsResponseTypeDef](./type_defs.md#getactionrecommendationsresponsetypedef) 


```python
# get_action_recommendations method usage example with argument unpacking

kwargs: GetActionRecommendationsRequestTypeDef = {  # (1)
    "campaignArn": ...,
}

parent.get_action_recommendations(**kwargs)
```

1. See [:material-code-braces: GetActionRecommendationsRequestTypeDef](./type_defs.md#getactionrecommendationsrequesttypedef) 

### get\_personalized\_ranking

Re-ranks a list of recommended items for the given user.

Type annotations and code completion for `#!python session.create_client("personalize-runtime").get_personalized_ranking` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/personalize-runtime/client/get_personalized_ranking.html)

```python
# get_personalized_ranking method definition

await def get_personalized_ranking(
    self,
    *,
    campaignArn: str,
    inputList: Sequence[str],
    userId: str,
    context: Mapping[str, str] = ...,
    filterArn: str = ...,
    filterValues: Mapping[str, str] = ...,
    metadataColumns: Mapping[str, Sequence[str]] = ...,
) -> GetPersonalizedRankingResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetPersonalizedRankingResponseTypeDef](./type_defs.md#getpersonalizedrankingresponsetypedef) 


```python
# get_personalized_ranking method usage example with argument unpacking

kwargs: GetPersonalizedRankingRequestTypeDef = {  # (1)
    "campaignArn": ...,
    "inputList": ...,
    "userId": ...,
}

parent.get_personalized_ranking(**kwargs)
```

1. See [:material-code-braces: GetPersonalizedRankingRequestTypeDef](./type_defs.md#getpersonalizedrankingrequesttypedef) 

### get\_recommendations

Returns a list of recommended items.

Type annotations and code completion for `#!python session.create_client("personalize-runtime").get_recommendations` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/personalize-runtime/client/get_recommendations.html)

```python
# get_recommendations method definition

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
    metadataColumns: Mapping[str, Sequence[str]] = ...,
) -> GetRecommendationsResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: PromotionTypeDef](./type_defs.md#promotiontypedef) 
2. See [:material-code-braces: GetRecommendationsResponseTypeDef](./type_defs.md#getrecommendationsresponsetypedef) 


```python
# get_recommendations method usage example with argument unpacking

kwargs: GetRecommendationsRequestTypeDef = {  # (1)
    "campaignArn": ...,
}

parent.get_recommendations(**kwargs)
```

1. See [:material-code-braces: GetRecommendationsRequestTypeDef](./type_defs.md#getrecommendationsrequesttypedef) 

### \_\_aenter\_\_



Type annotations and code completion for `#!python session.create_client("personalize-runtime").__aenter__` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/personalize-runtime.html#PersonalizeRuntime.Client)

```python
# __aenter__ method definition

await def __aenter__(
    self,
) -> Self:
    ...
```


### \_\_aexit\_\_



Type annotations and code completion for `#!python session.create_client("personalize-runtime").__aexit__` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/personalize-runtime.html#PersonalizeRuntime.Client)

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





