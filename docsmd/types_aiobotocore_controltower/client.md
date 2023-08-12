# ControlTowerClient

> [Index](../README.md) > [ControlTower](./README.md) > ControlTowerClient

!!! note ""

    Auto-generated documentation for [ControlTower](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/controltower.html#ControlTower)
    type annotations stubs module [types-aiobotocore-controltower](https://pypi.org/project/types-aiobotocore-controltower/).

## ControlTowerClient

Type annotations and code completion for `#!python session.create_client("controltower")`
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/controltower.html#ControlTower.Client)

```python
ControlTowerClient usage example

from aiobotocore.session import get_session
from types_aiobotocore_controltower.client import ControlTowerClient

session = get_session()
async with session.create_client("controltower") as client:
    client: ControlTowerClient
```

## Exceptions


`aiobotocore` client exceptions are generated in runtime.
This class provides code completion for `#!python session.create_client("controltower").exceptions` structure.

```python
ControlTowerClient.exceptions usage example

async with session.create_client("controltower") as client:
    try:
        do_something(client)
    except (
            client.AccessDeniedException,
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

```python
ControlTowerClient usage type checking example

from types_aiobotocore_controltower.client import Exceptions

def handle_error(exc: Exceptions.AccessDeniedException) -> None:
    ...
```


## Methods


### can\_paginate

Check if an operation can be paginated.

Type annotations and code completion for `#!python session.create_client("controltower").can_paginate` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/controltower.html#ControlTower.Client.can_paginate)

```python
# can_paginate method definition

def can_paginate(
    self,
    operation_name: str,
) -> bool:
    ...
```


### close

Closes underlying endpoint connections.

Type annotations and code completion for `#!python session.create_client("controltower").close` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/controltower.html#ControlTower.Client.close)

```python
# close method definition

await def close(
    self,
) -> None:
    ...
```


### disable\_control

This API call turns off a control.

Type annotations and code completion for `#!python session.create_client("controltower").disable_control` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/controltower.html#ControlTower.Client.disable_control)

```python
# disable_control method definition

await def disable_control(
    self,
    *,
    controlIdentifier: str,
    targetIdentifier: str,
) -> DisableControlOutputTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DisableControlOutputTypeDef](./type_defs.md#disablecontroloutputtypedef) 


```python
# disable_control method usage example with argument unpacking

kwargs: DisableControlInputRequestTypeDef = {  # (1)
    "controlIdentifier": ...,
    "targetIdentifier": ...,
}

parent.disable_control(**kwargs)
```

1. See [:material-code-braces: DisableControlInputRequestTypeDef](./type_defs.md#disablecontrolinputrequesttypedef) 

### enable\_control

This API call activates a control.

Type annotations and code completion for `#!python session.create_client("controltower").enable_control` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/controltower.html#ControlTower.Client.enable_control)

```python
# enable_control method definition

await def enable_control(
    self,
    *,
    controlIdentifier: str,
    targetIdentifier: str,
) -> EnableControlOutputTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: EnableControlOutputTypeDef](./type_defs.md#enablecontroloutputtypedef) 


```python
# enable_control method usage example with argument unpacking

kwargs: EnableControlInputRequestTypeDef = {  # (1)
    "controlIdentifier": ...,
    "targetIdentifier": ...,
}

parent.enable_control(**kwargs)
```

1. See [:material-code-braces: EnableControlInputRequestTypeDef](./type_defs.md#enablecontrolinputrequesttypedef) 

### generate\_presigned\_url

Generate a presigned url given a client, its method, and arguments.

Type annotations and code completion for `#!python session.create_client("controltower").generate_presigned_url` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/controltower.html#ControlTower.Client.generate_presigned_url)

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


### get\_control\_operation

Returns the status of a particular `EnableControl` or `DisableControl`
operation.

Type annotations and code completion for `#!python session.create_client("controltower").get_control_operation` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/controltower.html#ControlTower.Client.get_control_operation)

```python
# get_control_operation method definition

await def get_control_operation(
    self,
    *,
    operationIdentifier: str,
) -> GetControlOperationOutputTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetControlOperationOutputTypeDef](./type_defs.md#getcontroloperationoutputtypedef) 


```python
# get_control_operation method usage example with argument unpacking

kwargs: GetControlOperationInputRequestTypeDef = {  # (1)
    "operationIdentifier": ...,
}

parent.get_control_operation(**kwargs)
```

1. See [:material-code-braces: GetControlOperationInputRequestTypeDef](./type_defs.md#getcontroloperationinputrequesttypedef) 

### list\_enabled\_controls

Lists the controls enabled by AWS Control Tower on the specified organizational
unit and the accounts it contains.

Type annotations and code completion for `#!python session.create_client("controltower").list_enabled_controls` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/controltower.html#ControlTower.Client.list_enabled_controls)

```python
# list_enabled_controls method definition

await def list_enabled_controls(
    self,
    *,
    targetIdentifier: str,
    maxResults: int = ...,
    nextToken: str = ...,
) -> ListEnabledControlsOutputTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListEnabledControlsOutputTypeDef](./type_defs.md#listenabledcontrolsoutputtypedef) 


```python
# list_enabled_controls method usage example with argument unpacking

kwargs: ListEnabledControlsInputRequestTypeDef = {  # (1)
    "targetIdentifier": ...,
}

parent.list_enabled_controls(**kwargs)
```

1. See [:material-code-braces: ListEnabledControlsInputRequestTypeDef](./type_defs.md#listenabledcontrolsinputrequesttypedef) 

### \_\_aenter\_\_



Type annotations and code completion for `#!python session.create_client("controltower").__aenter__` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/controltower.html#ControlTower.Client.__aenter__)

```python
# __aenter__ method definition

await def __aenter__(
    self,
) -> ControlTowerClient:
    ...
```


### \_\_aexit\_\_



Type annotations and code completion for `#!python session.create_client("controltower").__aexit__` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/controltower.html#ControlTower.Client.__aexit__)

```python
# __aexit__ method definition

await def __aexit__(
    self,
    exc_type: Any,
    exc_val: Any,
    exc_tb: Any,
) -> Any:
    ...
```




### get_paginator

Type annotations and code completion for `#!python session.create_client("controltower").get_paginator` method with overloads.

- `client.get_paginator("list_enabled_controls")` -> [ListEnabledControlsPaginator](./paginators.md#listenabledcontrolspaginator)



