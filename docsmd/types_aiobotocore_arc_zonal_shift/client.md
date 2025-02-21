# ARCZonalShiftClient

> [Index](../README.md) > [ARCZonalShift](./README.md) > ARCZonalShiftClient

!!! note ""

    Auto-generated documentation for [ARCZonalShift](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/arc-zonal-shift.html#arczonalshift)
    type annotations stubs module [types-aiobotocore-arc-zonal-shift](https://pypi.org/project/types-aiobotocore-arc-zonal-shift/).

## ARCZonalShiftClient

Type annotations and code completion for `#!python session.create_client("arc-zonal-shift")`
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/arc-zonal-shift.html#ARCZonalShift.Client)

```python
# ARCZonalShiftClient usage example

from aiobotocore.session import get_session
from types_aiobotocore_arc_zonal_shift.client import ARCZonalShiftClient

session = get_session()
async with session.create_client("arc-zonal-shift") as client:
    client: ARCZonalShiftClient
```

## Exceptions


`aiobotocore` client exceptions are generated in runtime.
This class provides code completion for `#!python session.create_client("arc-zonal-shift").exceptions` structure.

```python
# ARCZonalShiftClient.exceptions usage example

async with session.create_client("arc-zonal-shift") as client:
    try:
        do_something(client)
    except (
            client.AccessDeniedException,
        client.ClientError,
        client.ConflictException,
        client.InternalServerException,
        client.ResourceNotFoundException,
        client.ThrottlingException,
        client.ValidationException,
    ) as e:
        print(e)
```

```python
# ARCZonalShiftClient usage type checking example

from types_aiobotocore_arc_zonal_shift.client import Exceptions

def handle_error(exc: Exceptions.AccessDeniedException) -> None:
    ...
```


## Methods


### can\_paginate



Type annotations and code completion for `#!python session.create_client("arc-zonal-shift").can_paginate` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/arc-zonal-shift/client/can_paginate.html)

```python
# can_paginate method definition

def can_paginate(
    self,
    operation_name: str,
) -> bool:
    ...
```


### generate\_presigned\_url



Type annotations and code completion for `#!python session.create_client("arc-zonal-shift").generate_presigned_url` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/arc-zonal-shift/client/generate_presigned_url.html)

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


### cancel\_zonal\_shift

Cancel a zonal shift in Amazon Route 53 Application Recovery Controller.

Type annotations and code completion for `#!python session.create_client("arc-zonal-shift").cancel_zonal_shift` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/arc-zonal-shift/client/cancel_zonal_shift.html)

```python
# cancel_zonal_shift method definition

await def cancel_zonal_shift(
    self,
    *,
    zonalShiftId: str,
) -> ZonalShiftTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ZonalShiftTypeDef](./type_defs.md#zonalshifttypedef) 


```python
# cancel_zonal_shift method usage example with argument unpacking

kwargs: CancelZonalShiftRequestTypeDef = {  # (1)
    "zonalShiftId": ...,
}

parent.cancel_zonal_shift(**kwargs)
```

1. See [:material-code-braces: CancelZonalShiftRequestTypeDef](./type_defs.md#cancelzonalshiftrequesttypedef) 

### create\_practice\_run\_configuration

A practice run configuration for zonal autoshift is required when you enable
zonal autoshift.

Type annotations and code completion for `#!python session.create_client("arc-zonal-shift").create_practice_run_configuration` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/arc-zonal-shift/client/create_practice_run_configuration.html)

```python
# create_practice_run_configuration method definition

await def create_practice_run_configuration(
    self,
    *,
    outcomeAlarms: Sequence[ControlConditionTypeDef],  # (1)
    resourceIdentifier: str,
    blockedDates: Sequence[str] = ...,
    blockedWindows: Sequence[str] = ...,
    blockingAlarms: Sequence[ControlConditionTypeDef] = ...,  # (1)
) -> CreatePracticeRunConfigurationResponseTypeDef:  # (3)
    ...
```

1. See [:material-code-braces: ControlConditionTypeDef](./type_defs.md#controlconditiontypedef) 
2. See [:material-code-braces: ControlConditionTypeDef](./type_defs.md#controlconditiontypedef) 
3. See [:material-code-braces: CreatePracticeRunConfigurationResponseTypeDef](./type_defs.md#createpracticerunconfigurationresponsetypedef) 


```python
# create_practice_run_configuration method usage example with argument unpacking

kwargs: CreatePracticeRunConfigurationRequestTypeDef = {  # (1)
    "outcomeAlarms": ...,
    "resourceIdentifier": ...,
}

parent.create_practice_run_configuration(**kwargs)
```

1. See [:material-code-braces: CreatePracticeRunConfigurationRequestTypeDef](./type_defs.md#createpracticerunconfigurationrequesttypedef) 

### delete\_practice\_run\_configuration

Deletes the practice run configuration for a resource.

Type annotations and code completion for `#!python session.create_client("arc-zonal-shift").delete_practice_run_configuration` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/arc-zonal-shift/client/delete_practice_run_configuration.html)

```python
# delete_practice_run_configuration method definition

await def delete_practice_run_configuration(
    self,
    *,
    resourceIdentifier: str,
) -> DeletePracticeRunConfigurationResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DeletePracticeRunConfigurationResponseTypeDef](./type_defs.md#deletepracticerunconfigurationresponsetypedef) 


```python
# delete_practice_run_configuration method usage example with argument unpacking

kwargs: DeletePracticeRunConfigurationRequestTypeDef = {  # (1)
    "resourceIdentifier": ...,
}

parent.delete_practice_run_configuration(**kwargs)
```

1. See [:material-code-braces: DeletePracticeRunConfigurationRequestTypeDef](./type_defs.md#deletepracticerunconfigurationrequesttypedef) 

### get\_autoshift\_observer\_notification\_status

Returns the status of autoshift observer notification.

Type annotations and code completion for `#!python session.create_client("arc-zonal-shift").get_autoshift_observer_notification_status` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/arc-zonal-shift/client/get_autoshift_observer_notification_status.html)

```python
# get_autoshift_observer_notification_status method definition

await def get_autoshift_observer_notification_status(
    self,
) -> GetAutoshiftObserverNotificationStatusResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetAutoshiftObserverNotificationStatusResponseTypeDef](./type_defs.md#getautoshiftobservernotificationstatusresponsetypedef) 

### get\_managed\_resource

Get information about a resource that's been registered for zonal shifts with
Amazon Route 53 Application Recovery Controller in this Amazon Web Services
Region.

Type annotations and code completion for `#!python session.create_client("arc-zonal-shift").get_managed_resource` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/arc-zonal-shift/client/get_managed_resource.html)

```python
# get_managed_resource method definition

await def get_managed_resource(
    self,
    *,
    resourceIdentifier: str,
) -> GetManagedResourceResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetManagedResourceResponseTypeDef](./type_defs.md#getmanagedresourceresponsetypedef) 


```python
# get_managed_resource method usage example with argument unpacking

kwargs: GetManagedResourceRequestTypeDef = {  # (1)
    "resourceIdentifier": ...,
}

parent.get_managed_resource(**kwargs)
```

1. See [:material-code-braces: GetManagedResourceRequestTypeDef](./type_defs.md#getmanagedresourcerequesttypedef) 

### list\_autoshifts

Returns a list of autoshifts for an Amazon Web Services Region.

Type annotations and code completion for `#!python session.create_client("arc-zonal-shift").list_autoshifts` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/arc-zonal-shift/client/list_autoshifts.html)

```python
# list_autoshifts method definition

await def list_autoshifts(
    self,
    *,
    maxResults: int = ...,
    nextToken: str = ...,
    status: AutoshiftExecutionStatusType = ...,  # (1)
) -> ListAutoshiftsResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-brackets: AutoshiftExecutionStatusType](./literals.md#autoshiftexecutionstatustype) 
2. See [:material-code-braces: ListAutoshiftsResponseTypeDef](./type_defs.md#listautoshiftsresponsetypedef) 


```python
# list_autoshifts method usage example with argument unpacking

kwargs: ListAutoshiftsRequestTypeDef = {  # (1)
    "maxResults": ...,
}

parent.list_autoshifts(**kwargs)
```

1. See [:material-code-braces: ListAutoshiftsRequestTypeDef](./type_defs.md#listautoshiftsrequesttypedef) 

### list\_managed\_resources

Lists all the resources in your Amazon Web Services account in this Amazon Web
Services Region that are managed for zonal shifts in Amazon Route 53
Application Recovery Controller, and information about them.

Type annotations and code completion for `#!python session.create_client("arc-zonal-shift").list_managed_resources` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/arc-zonal-shift/client/list_managed_resources.html)

```python
# list_managed_resources method definition

await def list_managed_resources(
    self,
    *,
    maxResults: int = ...,
    nextToken: str = ...,
) -> ListManagedResourcesResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListManagedResourcesResponseTypeDef](./type_defs.md#listmanagedresourcesresponsetypedef) 


```python
# list_managed_resources method usage example with argument unpacking

kwargs: ListManagedResourcesRequestTypeDef = {  # (1)
    "maxResults": ...,
}

parent.list_managed_resources(**kwargs)
```

1. See [:material-code-braces: ListManagedResourcesRequestTypeDef](./type_defs.md#listmanagedresourcesrequesttypedef) 

### list\_zonal\_shifts

Lists all active and completed zonal shifts in Amazon Route 53 Application
Recovery Controller in your Amazon Web Services account in this Amazon Web
Services Region.

Type annotations and code completion for `#!python session.create_client("arc-zonal-shift").list_zonal_shifts` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/arc-zonal-shift/client/list_zonal_shifts.html)

```python
# list_zonal_shifts method definition

await def list_zonal_shifts(
    self,
    *,
    maxResults: int = ...,
    nextToken: str = ...,
    resourceIdentifier: str = ...,
    status: ZonalShiftStatusType = ...,  # (1)
) -> ListZonalShiftsResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-brackets: ZonalShiftStatusType](./literals.md#zonalshiftstatustype) 
2. See [:material-code-braces: ListZonalShiftsResponseTypeDef](./type_defs.md#listzonalshiftsresponsetypedef) 


```python
# list_zonal_shifts method usage example with argument unpacking

kwargs: ListZonalShiftsRequestTypeDef = {  # (1)
    "maxResults": ...,
}

parent.list_zonal_shifts(**kwargs)
```

1. See [:material-code-braces: ListZonalShiftsRequestTypeDef](./type_defs.md#listzonalshiftsrequesttypedef) 

### start\_zonal\_shift

You start a zonal shift to temporarily move load balancer traffic away from an
Availability Zone in an Amazon Web Services Region, to help your application
recover immediately, for example, from a developer's bad code deployment or
from an Amazon Web Services infrastructure failure in a single Av...

Type annotations and code completion for `#!python session.create_client("arc-zonal-shift").start_zonal_shift` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/arc-zonal-shift/client/start_zonal_shift.html)

```python
# start_zonal_shift method definition

await def start_zonal_shift(
    self,
    *,
    awayFrom: str,
    comment: str,
    expiresIn: str,
    resourceIdentifier: str,
) -> ZonalShiftTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ZonalShiftTypeDef](./type_defs.md#zonalshifttypedef) 


```python
# start_zonal_shift method usage example with argument unpacking

kwargs: StartZonalShiftRequestTypeDef = {  # (1)
    "awayFrom": ...,
    "comment": ...,
    "expiresIn": ...,
    "resourceIdentifier": ...,
}

parent.start_zonal_shift(**kwargs)
```

1. See [:material-code-braces: StartZonalShiftRequestTypeDef](./type_defs.md#startzonalshiftrequesttypedef) 

### update\_autoshift\_observer\_notification\_status

Update the status of autoshift observer notification.

Type annotations and code completion for `#!python session.create_client("arc-zonal-shift").update_autoshift_observer_notification_status` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/arc-zonal-shift/client/update_autoshift_observer_notification_status.html)

```python
# update_autoshift_observer_notification_status method definition

await def update_autoshift_observer_notification_status(
    self,
    *,
    status: AutoshiftObserverNotificationStatusType,  # (1)
) -> UpdateAutoshiftObserverNotificationStatusResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-brackets: AutoshiftObserverNotificationStatusType](./literals.md#autoshiftobservernotificationstatustype) 
2. See [:material-code-braces: UpdateAutoshiftObserverNotificationStatusResponseTypeDef](./type_defs.md#updateautoshiftobservernotificationstatusresponsetypedef) 


```python
# update_autoshift_observer_notification_status method usage example with argument unpacking

kwargs: UpdateAutoshiftObserverNotificationStatusRequestTypeDef = {  # (1)
    "status": ...,
}

parent.update_autoshift_observer_notification_status(**kwargs)
```

1. See [:material-code-braces: UpdateAutoshiftObserverNotificationStatusRequestTypeDef](./type_defs.md#updateautoshiftobservernotificationstatusrequesttypedef) 

### update\_practice\_run\_configuration

Update a practice run configuration to change one or more of the following:
add, change, or remove the blocking alarm; change the outcome alarm; or add,
change, or remove blocking dates or time windows.

Type annotations and code completion for `#!python session.create_client("arc-zonal-shift").update_practice_run_configuration` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/arc-zonal-shift/client/update_practice_run_configuration.html)

```python
# update_practice_run_configuration method definition

await def update_practice_run_configuration(
    self,
    *,
    resourceIdentifier: str,
    blockedDates: Sequence[str] = ...,
    blockedWindows: Sequence[str] = ...,
    blockingAlarms: Sequence[ControlConditionTypeDef] = ...,  # (1)
    outcomeAlarms: Sequence[ControlConditionTypeDef] = ...,  # (1)
) -> UpdatePracticeRunConfigurationResponseTypeDef:  # (3)
    ...
```

1. See [:material-code-braces: ControlConditionTypeDef](./type_defs.md#controlconditiontypedef) 
2. See [:material-code-braces: ControlConditionTypeDef](./type_defs.md#controlconditiontypedef) 
3. See [:material-code-braces: UpdatePracticeRunConfigurationResponseTypeDef](./type_defs.md#updatepracticerunconfigurationresponsetypedef) 


```python
# update_practice_run_configuration method usage example with argument unpacking

kwargs: UpdatePracticeRunConfigurationRequestTypeDef = {  # (1)
    "resourceIdentifier": ...,
}

parent.update_practice_run_configuration(**kwargs)
```

1. See [:material-code-braces: UpdatePracticeRunConfigurationRequestTypeDef](./type_defs.md#updatepracticerunconfigurationrequesttypedef) 

### update\_zonal\_autoshift\_configuration

The zonal autoshift configuration for a resource includes the practice run
configuration and the status for running autoshifts, zonal autoshift status.

Type annotations and code completion for `#!python session.create_client("arc-zonal-shift").update_zonal_autoshift_configuration` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/arc-zonal-shift/client/update_zonal_autoshift_configuration.html)

```python
# update_zonal_autoshift_configuration method definition

await def update_zonal_autoshift_configuration(
    self,
    *,
    resourceIdentifier: str,
    zonalAutoshiftStatus: ZonalAutoshiftStatusType,  # (1)
) -> UpdateZonalAutoshiftConfigurationResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-brackets: ZonalAutoshiftStatusType](./literals.md#zonalautoshiftstatustype) 
2. See [:material-code-braces: UpdateZonalAutoshiftConfigurationResponseTypeDef](./type_defs.md#updatezonalautoshiftconfigurationresponsetypedef) 


```python
# update_zonal_autoshift_configuration method usage example with argument unpacking

kwargs: UpdateZonalAutoshiftConfigurationRequestTypeDef = {  # (1)
    "resourceIdentifier": ...,
    "zonalAutoshiftStatus": ...,
}

parent.update_zonal_autoshift_configuration(**kwargs)
```

1. See [:material-code-braces: UpdateZonalAutoshiftConfigurationRequestTypeDef](./type_defs.md#updatezonalautoshiftconfigurationrequesttypedef) 

### update\_zonal\_shift

Update an active zonal shift in Amazon Route 53 Application Recovery Controller
in your Amazon Web Services account.

Type annotations and code completion for `#!python session.create_client("arc-zonal-shift").update_zonal_shift` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/arc-zonal-shift/client/update_zonal_shift.html)

```python
# update_zonal_shift method definition

await def update_zonal_shift(
    self,
    *,
    zonalShiftId: str,
    comment: str = ...,
    expiresIn: str = ...,
) -> ZonalShiftTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ZonalShiftTypeDef](./type_defs.md#zonalshifttypedef) 


```python
# update_zonal_shift method usage example with argument unpacking

kwargs: UpdateZonalShiftRequestTypeDef = {  # (1)
    "zonalShiftId": ...,
}

parent.update_zonal_shift(**kwargs)
```

1. See [:material-code-braces: UpdateZonalShiftRequestTypeDef](./type_defs.md#updatezonalshiftrequesttypedef) 

### \_\_aenter\_\_



Type annotations and code completion for `#!python session.create_client("arc-zonal-shift").__aenter__` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/arc-zonal-shift.html#ARCZonalShift.Client)

```python
# __aenter__ method definition

await def __aenter__(
    self,
) -> Self:
    ...
```


### \_\_aexit\_\_



Type annotations and code completion for `#!python session.create_client("arc-zonal-shift").__aexit__` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/arc-zonal-shift.html#ARCZonalShift.Client)

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

Type annotations and code completion for `#!python session.create_client("arc-zonal-shift").get_paginator` method with overloads.

- `client.get_paginator("list_autoshifts")` -> [ListAutoshiftsPaginator](./paginators.md#listautoshiftspaginator)
- `client.get_paginator("list_managed_resources")` -> [ListManagedResourcesPaginator](./paginators.md#listmanagedresourcespaginator)
- `client.get_paginator("list_zonal_shifts")` -> [ListZonalShiftsPaginator](./paginators.md#listzonalshiftspaginator)



