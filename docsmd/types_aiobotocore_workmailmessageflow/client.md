# WorkMailMessageFlowClient

> [Index](../README.md) > [WorkMailMessageFlow](./README.md) > WorkMailMessageFlowClient

!!! note ""

    Auto-generated documentation for [WorkMailMessageFlow](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workmailmessageflow.html#WorkMailMessageFlow)
    type annotations stubs module [types-aiobotocore-workmailmessageflow](https://pypi.org/project/types-aiobotocore-workmailmessageflow/).

## WorkMailMessageFlowClient

Type annotations and code completion for `#!python session.create_client("workmailmessageflow")`
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workmailmessageflow.html#WorkMailMessageFlow.Client)

```python title="Usage example"
from aiobotocore.session import get_session
from types_aiobotocore_workmailmessageflow.client import WorkMailMessageFlowClient

session = get_session()
async with session.create_client("workmailmessageflow") as client:
    client: WorkMailMessageFlowClient
```

## Exceptions


`aiobotocore` client exceptions are generated in runtime.
This class provides code completion for `#!python session.create_client("workmailmessageflow").exceptions` structure.

```python title="Usage example"
async with session.create_client("workmailmessageflow") as client:
    try:
        do_something(client)
    except (
            client.ClientError,
        client.InvalidContentLocation,
        client.MessageFrozen,
        client.MessageRejected,
        client.ResourceNotFoundException,
    ) as e:
        print(e)
```

```python title="Type checking example"
from types_aiobotocore_workmailmessageflow.client import Exceptions

def handle_error(exc: Exceptions.ClientError) -> None:
    ...
```


## Methods


### can\_paginate

Check if an operation can be paginated.

Type annotations and code completion for `#!python session.create_client("workmailmessageflow").can_paginate` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workmailmessageflow.html#WorkMailMessageFlow.Client.can_paginate)

```python title="Method definition"
def can_paginate(
    self,
    operation_name: str,
) -> bool:
    ...
```


### generate\_presigned\_url

Generate a presigned url given a client, its method, and arguments.

Type annotations and code completion for `#!python session.create_client("workmailmessageflow").generate_presigned_url` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workmailmessageflow.html#WorkMailMessageFlow.Client.generate_presigned_url)

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


### get\_raw\_message\_content

Retrieves the raw content of an in-transit email message, in MIME format.

Type annotations and code completion for `#!python session.create_client("workmailmessageflow").get_raw_message_content` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workmailmessageflow.html#WorkMailMessageFlow.Client.get_raw_message_content)

```python title="Method definition"
await def get_raw_message_content(
    self,
    *,
    messageId: str,
) -> GetRawMessageContentResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetRawMessageContentResponseTypeDef](./type_defs.md#getrawmessagecontentresponsetypedef) 


```python title="Usage example with kwargs"
kwargs: GetRawMessageContentRequestRequestTypeDef = {  # (1)
    "messageId": ...,
}

parent.get_raw_message_content(**kwargs)
```

1. See [:material-code-braces: GetRawMessageContentRequestRequestTypeDef](./type_defs.md#getrawmessagecontentrequestrequesttypedef) 

### put\_raw\_message\_content

Updates the raw content of an in-transit email message, in MIME format.

Type annotations and code completion for `#!python session.create_client("workmailmessageflow").put_raw_message_content` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workmailmessageflow.html#WorkMailMessageFlow.Client.put_raw_message_content)

```python title="Method definition"
await def put_raw_message_content(
    self,
    *,
    messageId: str,
    content: RawMessageContentTypeDef,  # (1)
) -> Dict[str, Any]:
    ...
```

1. See [:material-code-braces: RawMessageContentTypeDef](./type_defs.md#rawmessagecontenttypedef) 


```python title="Usage example with kwargs"
kwargs: PutRawMessageContentRequestRequestTypeDef = {  # (1)
    "messageId": ...,
    "content": ...,
}

parent.put_raw_message_content(**kwargs)
```

1. See [:material-code-braces: PutRawMessageContentRequestRequestTypeDef](./type_defs.md#putrawmessagecontentrequestrequesttypedef) 

### \_\_aenter\_\_



Type annotations and code completion for `#!python session.create_client("workmailmessageflow").__aenter__` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workmailmessageflow.html#WorkMailMessageFlow.Client.__aenter__)

```python title="Method definition"
await def __aenter__(
    self,
) -> WorkMailMessageFlowClient:
    ...
```


### \_\_aexit\_\_



Type annotations and code completion for `#!python session.create_client("workmailmessageflow").__aexit__` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workmailmessageflow.html#WorkMailMessageFlow.Client.__aexit__)

```python title="Method definition"
await def __aexit__(
    self,
    exc_type: Any,
    exc_val: Any,
    exc_tb: Any,
) -> Any:
    ...
```





