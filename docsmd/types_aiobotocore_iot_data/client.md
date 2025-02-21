# IoTDataPlaneClient

> [Index](../README.md) > [IoTDataPlane](./README.md) > IoTDataPlaneClient

!!! note ""

    Auto-generated documentation for [IoTDataPlane](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot-data.html#iotdataplane)
    type annotations stubs module [types-aiobotocore-iot-data](https://pypi.org/project/types-aiobotocore-iot-data/).

## IoTDataPlaneClient

Type annotations and code completion for `#!python session.create_client("iot-data")`
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot-data.html#IoTDataPlane.Client)

```python
# IoTDataPlaneClient usage example

from aiobotocore.session import get_session
from types_aiobotocore_iot_data.client import IoTDataPlaneClient

session = get_session()
async with session.create_client("iot-data") as client:
    client: IoTDataPlaneClient
```

## Exceptions


`aiobotocore` client exceptions are generated in runtime.
This class provides code completion for `#!python session.create_client("iot-data").exceptions` structure.

```python
# IoTDataPlaneClient.exceptions usage example

async with session.create_client("iot-data") as client:
    try:
        do_something(client)
    except (
            client.ClientError,
        client.ConflictException,
        client.InternalFailureException,
        client.InvalidRequestException,
        client.MethodNotAllowedException,
        client.RequestEntityTooLargeException,
        client.ResourceNotFoundException,
        client.ServiceUnavailableException,
        client.ThrottlingException,
        client.UnauthorizedException,
        client.UnsupportedDocumentEncodingException,
    ) as e:
        print(e)
```

```python
# IoTDataPlaneClient usage type checking example

from types_aiobotocore_iot_data.client import Exceptions

def handle_error(exc: Exceptions.ClientError) -> None:
    ...
```


## Methods


### can\_paginate



Type annotations and code completion for `#!python session.create_client("iot-data").can_paginate` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot-data/client/can_paginate.html)

```python
# can_paginate method definition

def can_paginate(
    self,
    operation_name: str,
) -> bool:
    ...
```


### generate\_presigned\_url



Type annotations and code completion for `#!python session.create_client("iot-data").generate_presigned_url` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot-data/client/generate_presigned_url.html)

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


### delete\_thing\_shadow

Deletes the shadow for the specified thing.

Type annotations and code completion for `#!python session.create_client("iot-data").delete_thing_shadow` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot-data/client/delete_thing_shadow.html)

```python
# delete_thing_shadow method definition

await def delete_thing_shadow(
    self,
    *,
    thingName: str,
    shadowName: str = ...,
) -> DeleteThingShadowResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DeleteThingShadowResponseTypeDef](./type_defs.md#deletethingshadowresponsetypedef) 


```python
# delete_thing_shadow method usage example with argument unpacking

kwargs: DeleteThingShadowRequestTypeDef = {  # (1)
    "thingName": ...,
}

parent.delete_thing_shadow(**kwargs)
```

1. See [:material-code-braces: DeleteThingShadowRequestTypeDef](./type_defs.md#deletethingshadowrequesttypedef) 

### get\_retained\_message

Gets the details of a single retained message for the specified topic.

Type annotations and code completion for `#!python session.create_client("iot-data").get_retained_message` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot-data/client/get_retained_message.html)

```python
# get_retained_message method definition

await def get_retained_message(
    self,
    *,
    topic: str,
) -> GetRetainedMessageResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetRetainedMessageResponseTypeDef](./type_defs.md#getretainedmessageresponsetypedef) 


```python
# get_retained_message method usage example with argument unpacking

kwargs: GetRetainedMessageRequestTypeDef = {  # (1)
    "topic": ...,
}

parent.get_retained_message(**kwargs)
```

1. See [:material-code-braces: GetRetainedMessageRequestTypeDef](./type_defs.md#getretainedmessagerequesttypedef) 

### get\_thing\_shadow

Gets the shadow for the specified thing.

Type annotations and code completion for `#!python session.create_client("iot-data").get_thing_shadow` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot-data/client/get_thing_shadow.html)

```python
# get_thing_shadow method definition

await def get_thing_shadow(
    self,
    *,
    thingName: str,
    shadowName: str = ...,
) -> GetThingShadowResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetThingShadowResponseTypeDef](./type_defs.md#getthingshadowresponsetypedef) 


```python
# get_thing_shadow method usage example with argument unpacking

kwargs: GetThingShadowRequestTypeDef = {  # (1)
    "thingName": ...,
}

parent.get_thing_shadow(**kwargs)
```

1. See [:material-code-braces: GetThingShadowRequestTypeDef](./type_defs.md#getthingshadowrequesttypedef) 

### list\_named\_shadows\_for\_thing

Lists the shadows for the specified thing.

Type annotations and code completion for `#!python session.create_client("iot-data").list_named_shadows_for_thing` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot-data/client/list_named_shadows_for_thing.html)

```python
# list_named_shadows_for_thing method definition

await def list_named_shadows_for_thing(
    self,
    *,
    thingName: str,
    nextToken: str = ...,
    pageSize: int = ...,
) -> ListNamedShadowsForThingResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListNamedShadowsForThingResponseTypeDef](./type_defs.md#listnamedshadowsforthingresponsetypedef) 


```python
# list_named_shadows_for_thing method usage example with argument unpacking

kwargs: ListNamedShadowsForThingRequestTypeDef = {  # (1)
    "thingName": ...,
}

parent.list_named_shadows_for_thing(**kwargs)
```

1. See [:material-code-braces: ListNamedShadowsForThingRequestTypeDef](./type_defs.md#listnamedshadowsforthingrequesttypedef) 

### list\_retained\_messages

Lists summary information about the retained messages stored for the account.

Type annotations and code completion for `#!python session.create_client("iot-data").list_retained_messages` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot-data/client/list_retained_messages.html)

```python
# list_retained_messages method definition

await def list_retained_messages(
    self,
    *,
    nextToken: str = ...,
    maxResults: int = ...,
) -> ListRetainedMessagesResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListRetainedMessagesResponseTypeDef](./type_defs.md#listretainedmessagesresponsetypedef) 


```python
# list_retained_messages method usage example with argument unpacking

kwargs: ListRetainedMessagesRequestTypeDef = {  # (1)
    "nextToken": ...,
}

parent.list_retained_messages(**kwargs)
```

1. See [:material-code-braces: ListRetainedMessagesRequestTypeDef](./type_defs.md#listretainedmessagesrequesttypedef) 

### publish

Publishes an MQTT message.

Type annotations and code completion for `#!python session.create_client("iot-data").publish` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot-data/client/publish.html)

```python
# publish method definition

await def publish(
    self,
    *,
    topic: str,
    qos: int = ...,
    retain: bool = ...,
    payload: BlobTypeDef = ...,
    userProperties: str = ...,
    payloadFormatIndicator: PayloadFormatIndicatorType = ...,  # (1)
    contentType: str = ...,
    responseTopic: str = ...,
    correlationData: str = ...,
    messageExpiry: int = ...,
) -> EmptyResponseMetadataTypeDef:  # (2)
    ...
```

1. See [:material-code-brackets: PayloadFormatIndicatorType](./literals.md#payloadformatindicatortype) 
2. See [:material-code-braces: EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef) 


```python
# publish method usage example with argument unpacking

kwargs: PublishRequestTypeDef = {  # (1)
    "topic": ...,
}

parent.publish(**kwargs)
```

1. See [:material-code-braces: PublishRequestTypeDef](./type_defs.md#publishrequesttypedef) 

### update\_thing\_shadow

Updates the shadow for the specified thing.

Type annotations and code completion for `#!python session.create_client("iot-data").update_thing_shadow` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot-data/client/update_thing_shadow.html)

```python
# update_thing_shadow method definition

await def update_thing_shadow(
    self,
    *,
    thingName: str,
    payload: BlobTypeDef,
    shadowName: str = ...,
) -> UpdateThingShadowResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: UpdateThingShadowResponseTypeDef](./type_defs.md#updatethingshadowresponsetypedef) 


```python
# update_thing_shadow method usage example with argument unpacking

kwargs: UpdateThingShadowRequestTypeDef = {  # (1)
    "thingName": ...,
    "payload": ...,
}

parent.update_thing_shadow(**kwargs)
```

1. See [:material-code-braces: UpdateThingShadowRequestTypeDef](./type_defs.md#updatethingshadowrequesttypedef) 

### \_\_aenter\_\_



Type annotations and code completion for `#!python session.create_client("iot-data").__aenter__` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot-data.html#IoTDataPlane.Client)

```python
# __aenter__ method definition

await def __aenter__(
    self,
) -> Self:
    ...
```


### \_\_aexit\_\_



Type annotations and code completion for `#!python session.create_client("iot-data").__aexit__` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot-data.html#IoTDataPlane.Client)

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

Type annotations and code completion for `#!python session.create_client("iot-data").get_paginator` method with overloads.

- `client.get_paginator("list_retained_messages")` -> [ListRetainedMessagesPaginator](./paginators.md#listretainedmessagespaginator)



