# PersonalizeEventsClient

> [Index](../README.md) > [PersonalizeEvents](./README.md) > PersonalizeEventsClient

!!! note ""

    Auto-generated documentation for [PersonalizeEvents](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/personalize-events.html#personalizeevents)
    type annotations stubs module [types-aiobotocore-personalize-events](https://pypi.org/project/types-aiobotocore-personalize-events/).

## PersonalizeEventsClient

Type annotations and code completion for `#!python session.create_client("personalize-events")`
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/personalize-events.html#PersonalizeEvents.Client)

```python
# PersonalizeEventsClient usage example

from aiobotocore.session import get_session
from types_aiobotocore_personalize_events.client import PersonalizeEventsClient

session = get_session()
async with session.create_client("personalize-events") as client:
    client: PersonalizeEventsClient
```

## Exceptions


`aiobotocore` client exceptions are generated in runtime.
This class provides code completion for `#!python session.create_client("personalize-events").exceptions` structure.

```python
# PersonalizeEventsClient.exceptions usage example

async with session.create_client("personalize-events") as client:
    try:
        do_something(client)
    except (
            client.ClientError,
        client.InvalidInputException,
        client.ResourceInUseException,
        client.ResourceNotFoundException,
    ) as e:
        print(e)
```

```python
# PersonalizeEventsClient usage type checking example

from types_aiobotocore_personalize_events.client import Exceptions

def handle_error(exc: Exceptions.ClientError) -> None:
    ...
```


## Methods


### can\_paginate



Type annotations and code completion for `#!python session.create_client("personalize-events").can_paginate` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/personalize-events/client/can_paginate.html)

```python
# can_paginate method definition

def can_paginate(
    self,
    operation_name: str,
) -> bool:
    ...
```


### generate\_presigned\_url



Type annotations and code completion for `#!python session.create_client("personalize-events").generate_presigned_url` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/personalize-events/client/generate_presigned_url.html)

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


### put\_action\_interactions

Records action interaction event data.

Type annotations and code completion for `#!python session.create_client("personalize-events").put_action_interactions` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/personalize-events/client/put_action_interactions.html)

```python
# put_action_interactions method definition

await def put_action_interactions(
    self,
    *,
    trackingId: str,
    actionInteractions: Sequence[ActionInteractionTypeDef],  # (1)
) -> EmptyResponseMetadataTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: ActionInteractionTypeDef](./type_defs.md#actioninteractiontypedef) 
2. See [:material-code-braces: EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef) 


```python
# put_action_interactions method usage example with argument unpacking

kwargs: PutActionInteractionsRequestTypeDef = {  # (1)
    "trackingId": ...,
    "actionInteractions": ...,
}

parent.put_action_interactions(**kwargs)
```

1. See [:material-code-braces: PutActionInteractionsRequestTypeDef](./type_defs.md#putactioninteractionsrequesttypedef) 

### put\_actions

Adds one or more actions to an Actions dataset.

Type annotations and code completion for `#!python session.create_client("personalize-events").put_actions` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/personalize-events/client/put_actions.html)

```python
# put_actions method definition

await def put_actions(
    self,
    *,
    datasetArn: str,
    actions: Sequence[ActionTypeDef],  # (1)
) -> EmptyResponseMetadataTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: ActionTypeDef](./type_defs.md#actiontypedef) 
2. See [:material-code-braces: EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef) 


```python
# put_actions method usage example with argument unpacking

kwargs: PutActionsRequestTypeDef = {  # (1)
    "datasetArn": ...,
    "actions": ...,
}

parent.put_actions(**kwargs)
```

1. See [:material-code-braces: PutActionsRequestTypeDef](./type_defs.md#putactionsrequesttypedef) 

### put\_events

Records item interaction event data.

Type annotations and code completion for `#!python session.create_client("personalize-events").put_events` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/personalize-events/client/put_events.html)

```python
# put_events method definition

await def put_events(
    self,
    *,
    trackingId: str,
    sessionId: str,
    eventList: Sequence[EventTypeDef],  # (1)
    userId: str = ...,
) -> EmptyResponseMetadataTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: EventTypeDef](./type_defs.md#eventtypedef) 
2. See [:material-code-braces: EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef) 


```python
# put_events method usage example with argument unpacking

kwargs: PutEventsRequestTypeDef = {  # (1)
    "trackingId": ...,
    "sessionId": ...,
    "eventList": ...,
}

parent.put_events(**kwargs)
```

1. See [:material-code-braces: PutEventsRequestTypeDef](./type_defs.md#puteventsrequesttypedef) 

### put\_items

Adds one or more items to an Items dataset.

Type annotations and code completion for `#!python session.create_client("personalize-events").put_items` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/personalize-events/client/put_items.html)

```python
# put_items method definition

await def put_items(
    self,
    *,
    datasetArn: str,
    items: Sequence[ItemTypeDef],  # (1)
) -> EmptyResponseMetadataTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: ItemTypeDef](./type_defs.md#itemtypedef) 
2. See [:material-code-braces: EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef) 


```python
# put_items method usage example with argument unpacking

kwargs: PutItemsRequestTypeDef = {  # (1)
    "datasetArn": ...,
    "items": ...,
}

parent.put_items(**kwargs)
```

1. See [:material-code-braces: PutItemsRequestTypeDef](./type_defs.md#putitemsrequesttypedef) 

### put\_users

Adds one or more users to a Users dataset.

Type annotations and code completion for `#!python session.create_client("personalize-events").put_users` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/personalize-events/client/put_users.html)

```python
# put_users method definition

await def put_users(
    self,
    *,
    datasetArn: str,
    users: Sequence[UserTypeDef],  # (1)
) -> EmptyResponseMetadataTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: UserTypeDef](./type_defs.md#usertypedef) 
2. See [:material-code-braces: EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef) 


```python
# put_users method usage example with argument unpacking

kwargs: PutUsersRequestTypeDef = {  # (1)
    "datasetArn": ...,
    "users": ...,
}

parent.put_users(**kwargs)
```

1. See [:material-code-braces: PutUsersRequestTypeDef](./type_defs.md#putusersrequesttypedef) 

### \_\_aenter\_\_



Type annotations and code completion for `#!python session.create_client("personalize-events").__aenter__` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/personalize-events.html#PersonalizeEvents.Client)

```python
# __aenter__ method definition

await def __aenter__(
    self,
) -> Self:
    ...
```


### \_\_aexit\_\_



Type annotations and code completion for `#!python session.create_client("personalize-events").__aexit__` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/personalize-events.html#PersonalizeEvents.Client)

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





