# ARCZonalShiftClient

> [Index](../README.md) > [ARCZonalShift](./README.md) > ARCZonalShiftClient

!!! note ""

    Auto-generated documentation for [ARCZonalShift](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/arc-zonal-shift.html#ARCZonalShift)
    type annotations stubs module [types-aiobotocore-arc-zonal-shift](https://pypi.org/project/types-aiobotocore-arc-zonal-shift/).

## ARCZonalShiftClient

Type annotations and code completion for `#!python session.create_client("arc-zonal-shift")`
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/arc-zonal-shift.html#ARCZonalShift.Client)

```python
ARCZonalShiftClient usage example

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
ARCZonalShiftClient.exceptions usage example

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
ARCZonalShiftClient usage type checking example

from types_aiobotocore_arc_zonal_shift.client import Exceptions

def handle_error(exc: Exceptions.AccessDeniedException) -> None:
    ...
```


## Methods


### can\_paginate

Check if an operation can be paginated.

Type annotations and code completion for `#!python session.create_client("arc-zonal-shift").can_paginate` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/arc-zonal-shift.html#ARCZonalShift.Client.can_paginate)

```python
# can_paginate method definition

def can_paginate(
    self,
    operation_name: str,
) -> bool:
    ...
```


### cancel\_zonal\_shift

Cancel a zonal shift in Amazon Route 53 Application Recovery Controller that
you've started for a resource in your AWS account in an AWS Region.

Type annotations and code completion for `#!python session.create_client("arc-zonal-shift").cancel_zonal_shift` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/arc-zonal-shift.html#ARCZonalShift.Client.cancel_zonal_shift)

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

kwargs: CancelZonalShiftRequestRequestTypeDef = {  # (1)
    "zonalShiftId": ...,
}

parent.cancel_zonal_shift(**kwargs)
```

1. See [:material-code-braces: CancelZonalShiftRequestRequestTypeDef](./type_defs.md#cancelzonalshiftrequestrequesttypedef) 

### close

Closes underlying endpoint connections.

Type annotations and code completion for `#!python session.create_client("arc-zonal-shift").close` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/arc-zonal-shift.html#ARCZonalShift.Client.close)

```python
# close method definition

await def close(
    self,
) -> None:
    ...
```


### generate\_presigned\_url

Generate a presigned url given a client, its method, and arguments.

Type annotations and code completion for `#!python session.create_client("arc-zonal-shift").generate_presigned_url` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/arc-zonal-shift.html#ARCZonalShift.Client.generate_presigned_url)

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


### get\_managed\_resource

Get information about a resource that's been registered for zonal shifts with
Amazon Route 53 Application Recovery Controller in this AWS Region.

Type annotations and code completion for `#!python session.create_client("arc-zonal-shift").get_managed_resource` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/arc-zonal-shift.html#ARCZonalShift.Client.get_managed_resource)

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

kwargs: GetManagedResourceRequestRequestTypeDef = {  # (1)
    "resourceIdentifier": ...,
}

parent.get_managed_resource(**kwargs)
```

1. See [:material-code-braces: GetManagedResourceRequestRequestTypeDef](./type_defs.md#getmanagedresourcerequestrequesttypedef) 

### list\_managed\_resources

Lists all the resources in your AWS account in this AWS Region that are managed
for zonal shifts in Amazon Route 53 Application Recovery Controller, and
information about them.

Type annotations and code completion for `#!python session.create_client("arc-zonal-shift").list_managed_resources` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/arc-zonal-shift.html#ARCZonalShift.Client.list_managed_resources)

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

kwargs: ListManagedResourcesRequestRequestTypeDef = {  # (1)
    "maxResults": ...,
}

parent.list_managed_resources(**kwargs)
```

1. See [:material-code-braces: ListManagedResourcesRequestRequestTypeDef](./type_defs.md#listmanagedresourcesrequestrequesttypedef) 

### list\_zonal\_shifts

Lists all the active zonal shifts in Amazon Route 53 Application Recovery
Controller in your AWS account in this AWS Region.

Type annotations and code completion for `#!python session.create_client("arc-zonal-shift").list_zonal_shifts` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/arc-zonal-shift.html#ARCZonalShift.Client.list_zonal_shifts)

```python
# list_zonal_shifts method definition

await def list_zonal_shifts(
    self,
    *,
    maxResults: int = ...,
    nextToken: str = ...,
    status: ZonalShiftStatusType = ...,  # (1)
) -> ListZonalShiftsResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-brackets: ZonalShiftStatusType](./literals.md#zonalshiftstatustype) 
2. See [:material-code-braces: ListZonalShiftsResponseTypeDef](./type_defs.md#listzonalshiftsresponsetypedef) 


```python
# list_zonal_shifts method usage example with argument unpacking

kwargs: ListZonalShiftsRequestRequestTypeDef = {  # (1)
    "maxResults": ...,
}

parent.list_zonal_shifts(**kwargs)
```

1. See [:material-code-braces: ListZonalShiftsRequestRequestTypeDef](./type_defs.md#listzonalshiftsrequestrequesttypedef) 

### start\_zonal\_shift

You start a zonal shift to temporarily move load balancer traffic away from an
Availability Zone in a AWS Region, to help your application recover immediately,
for example, from a developer's bad code deployment or from an AWS
infrastructure failure in a single Availability Zone.

Type annotations and code completion for `#!python session.create_client("arc-zonal-shift").start_zonal_shift` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/arc-zonal-shift.html#ARCZonalShift.Client.start_zonal_shift)

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

kwargs: StartZonalShiftRequestRequestTypeDef = {  # (1)
    "awayFrom": ...,
    "comment": ...,
    "expiresIn": ...,
    "resourceIdentifier": ...,
}

parent.start_zonal_shift(**kwargs)
```

1. See [:material-code-braces: StartZonalShiftRequestRequestTypeDef](./type_defs.md#startzonalshiftrequestrequesttypedef) 

### update\_zonal\_shift

Update an active zonal shift in Amazon Route 53 Application Recovery Controller
in your AWS account.

Type annotations and code completion for `#!python session.create_client("arc-zonal-shift").update_zonal_shift` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/arc-zonal-shift.html#ARCZonalShift.Client.update_zonal_shift)

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

kwargs: UpdateZonalShiftRequestRequestTypeDef = {  # (1)
    "zonalShiftId": ...,
}

parent.update_zonal_shift(**kwargs)
```

1. See [:material-code-braces: UpdateZonalShiftRequestRequestTypeDef](./type_defs.md#updatezonalshiftrequestrequesttypedef) 

### \_\_aenter\_\_



Type annotations and code completion for `#!python session.create_client("arc-zonal-shift").__aenter__` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/arc-zonal-shift.html#ARCZonalShift.Client.__aenter__)

```python
# __aenter__ method definition

await def __aenter__(
    self,
) -> ARCZonalShiftClient:
    ...
```


### \_\_aexit\_\_



Type annotations and code completion for `#!python session.create_client("arc-zonal-shift").__aexit__` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/arc-zonal-shift.html#ARCZonalShift.Client.__aexit__)

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

Type annotations and code completion for `#!python session.create_client("arc-zonal-shift").get_paginator` method with overloads.

- `client.get_paginator("list_managed_resources")` -> [ListManagedResourcesPaginator](./paginators.md#listmanagedresourcespaginator)
- `client.get_paginator("list_zonal_shifts")` -> [ListZonalShiftsPaginator](./paginators.md#listzonalshiftspaginator)



