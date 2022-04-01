# AugmentedAIRuntimeClient

> [Index](../README.md) > [AugmentedAIRuntime](./README.md) > AugmentedAIRuntimeClient

!!! note ""

    Auto-generated documentation for [AugmentedAIRuntime](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker-a2i-runtime.html#AugmentedAIRuntime)
    type annotations stubs module [types-aiobotocore-sagemaker-a2i-runtime](https://pypi.org/project/types-aiobotocore-sagemaker-a2i-runtime/).

## AugmentedAIRuntimeClient

Type annotations and code completion for `#!python session.create_client("sagemaker-a2i-runtime")`
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker-a2i-runtime.html#AugmentedAIRuntime.Client)

```python title="Usage example"
from aiobotocore.session import get_session
from types_aiobotocore_sagemaker_a2i_runtime.client import AugmentedAIRuntimeClient

session = get_session()
async with session.create_client("sagemaker-a2i-runtime") as client:
    client: AugmentedAIRuntimeClient
```

## Exceptions


`aiobotocore` client exceptions are generated in runtime.
This class provides code completion for `#!python session.create_client("sagemaker-a2i-runtime").exceptions` structure.

```python title="Usage example"
async with session.create_client("sagemaker-a2i-runtime") as client:
    try:
        do_something(client)
    except (
            client.ClientError,
        client.ConflictException,
        client.InternalServerException,
        client.ResourceNotFoundException,
        client.ServiceQuotaExceededException,
        client.ThrottlingException,
        client.ValidationException,
    ) as e:
        print(e)
```

```python title="Type checking example"
from types_aiobotocore_sagemaker_a2i_runtime.client import Exceptions

def handle_error(exc: Exceptions.ClientError) -> None:
    ...
```


## Methods


### can\_paginate

Check if an operation can be paginated.

Type annotations and code completion for `#!python session.create_client("sagemaker-a2i-runtime").can_paginate` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker-a2i-runtime.html#AugmentedAIRuntime.Client.can_paginate)

```python title="Method definition"
def can_paginate(
    self,
    operation_name: str,
) -> bool:
    ...
```


### delete\_human\_loop

Deletes the specified human loop for a flow definition.

Type annotations and code completion for `#!python session.create_client("sagemaker-a2i-runtime").delete_human_loop` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker-a2i-runtime.html#AugmentedAIRuntime.Client.delete_human_loop)

```python title="Method definition"
await def delete_human_loop(
    self,
    *,
    HumanLoopName: str,
) -> Dict[str, Any]:
    ...
```



```python title="Usage example with kwargs"
kwargs: DeleteHumanLoopRequestRequestTypeDef = {  # (1)
    "HumanLoopName": ...,
}

parent.delete_human_loop(**kwargs)
```

1. See [:material-code-braces: DeleteHumanLoopRequestRequestTypeDef](./type_defs.md#deletehumanlooprequestrequesttypedef) 

### describe\_human\_loop

Returns information about the specified human loop.

Type annotations and code completion for `#!python session.create_client("sagemaker-a2i-runtime").describe_human_loop` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker-a2i-runtime.html#AugmentedAIRuntime.Client.describe_human_loop)

```python title="Method definition"
await def describe_human_loop(
    self,
    *,
    HumanLoopName: str,
) -> DescribeHumanLoopResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DescribeHumanLoopResponseTypeDef](./type_defs.md#describehumanloopresponsetypedef) 


```python title="Usage example with kwargs"
kwargs: DescribeHumanLoopRequestRequestTypeDef = {  # (1)
    "HumanLoopName": ...,
}

parent.describe_human_loop(**kwargs)
```

1. See [:material-code-braces: DescribeHumanLoopRequestRequestTypeDef](./type_defs.md#describehumanlooprequestrequesttypedef) 

### generate\_presigned\_url

Generate a presigned url given a client, its method, and arguments.

Type annotations and code completion for `#!python session.create_client("sagemaker-a2i-runtime").generate_presigned_url` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker-a2i-runtime.html#AugmentedAIRuntime.Client.generate_presigned_url)

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


### list\_human\_loops

Returns information about human loops, given the specified parameters.

Type annotations and code completion for `#!python session.create_client("sagemaker-a2i-runtime").list_human_loops` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker-a2i-runtime.html#AugmentedAIRuntime.Client.list_human_loops)

```python title="Method definition"
await def list_human_loops(
    self,
    *,
    FlowDefinitionArn: str,
    CreationTimeAfter: Union[datetime, str] = ...,
    CreationTimeBefore: Union[datetime, str] = ...,
    SortOrder: SortOrderType = ...,  # (1)
    NextToken: str = ...,
    MaxResults: int = ...,
) -> ListHumanLoopsResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-brackets: SortOrderType](./literals.md#sortordertype) 
2. See [:material-code-braces: ListHumanLoopsResponseTypeDef](./type_defs.md#listhumanloopsresponsetypedef) 


```python title="Usage example with kwargs"
kwargs: ListHumanLoopsRequestRequestTypeDef = {  # (1)
    "FlowDefinitionArn": ...,
}

parent.list_human_loops(**kwargs)
```

1. See [:material-code-braces: ListHumanLoopsRequestRequestTypeDef](./type_defs.md#listhumanloopsrequestrequesttypedef) 

### start\_human\_loop

Starts a human loop, provided that at least one activation condition is met.

Type annotations and code completion for `#!python session.create_client("sagemaker-a2i-runtime").start_human_loop` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker-a2i-runtime.html#AugmentedAIRuntime.Client.start_human_loop)

```python title="Method definition"
await def start_human_loop(
    self,
    *,
    HumanLoopName: str,
    FlowDefinitionArn: str,
    HumanLoopInput: HumanLoopInputTypeDef,  # (1)
    DataAttributes: HumanLoopDataAttributesTypeDef = ...,  # (2)
) -> StartHumanLoopResponseTypeDef:  # (3)
    ...
```

1. See [:material-code-braces: HumanLoopInputTypeDef](./type_defs.md#humanloopinputtypedef) 
2. See [:material-code-braces: HumanLoopDataAttributesTypeDef](./type_defs.md#humanloopdataattributestypedef) 
3. See [:material-code-braces: StartHumanLoopResponseTypeDef](./type_defs.md#starthumanloopresponsetypedef) 


```python title="Usage example with kwargs"
kwargs: StartHumanLoopRequestRequestTypeDef = {  # (1)
    "HumanLoopName": ...,
    "FlowDefinitionArn": ...,
    "HumanLoopInput": ...,
}

parent.start_human_loop(**kwargs)
```

1. See [:material-code-braces: StartHumanLoopRequestRequestTypeDef](./type_defs.md#starthumanlooprequestrequesttypedef) 

### stop\_human\_loop

Stops the specified human loop.

Type annotations and code completion for `#!python session.create_client("sagemaker-a2i-runtime").stop_human_loop` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker-a2i-runtime.html#AugmentedAIRuntime.Client.stop_human_loop)

```python title="Method definition"
await def stop_human_loop(
    self,
    *,
    HumanLoopName: str,
) -> Dict[str, Any]:
    ...
```



```python title="Usage example with kwargs"
kwargs: StopHumanLoopRequestRequestTypeDef = {  # (1)
    "HumanLoopName": ...,
}

parent.stop_human_loop(**kwargs)
```

1. See [:material-code-braces: StopHumanLoopRequestRequestTypeDef](./type_defs.md#stophumanlooprequestrequesttypedef) 

### \_\_aenter\_\_



Type annotations and code completion for `#!python session.create_client("sagemaker-a2i-runtime").__aenter__` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker-a2i-runtime.html#AugmentedAIRuntime.Client.__aenter__)

```python title="Method definition"
await def __aenter__(
    self,
) -> AugmentedAIRuntimeClient:
    ...
```


### \_\_aexit\_\_



Type annotations and code completion for `#!python session.create_client("sagemaker-a2i-runtime").__aexit__` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker-a2i-runtime.html#AugmentedAIRuntime.Client.__aexit__)

```python title="Method definition"
await def __aexit__(
    self,
    exc_type: Any,
    exc_val: Any,
    exc_tb: Any,
) -> Any:
    ...
```




### get_paginator

Type annotations and code completion for `#!python session.create_client("sagemaker-a2i-runtime").get_paginator` method with overloads.

- `client.get_paginator("list_human_loops")` -> [ListHumanLoopsPaginator](./paginators.md#listhumanloopspaginator)



