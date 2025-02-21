# SimSpaceWeaverClient

> [Index](../README.md) > [SimSpaceWeaver](./README.md) > SimSpaceWeaverClient

!!! note ""

    Auto-generated documentation for [SimSpaceWeaver](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/simspaceweaver.html#simspaceweaver)
    type annotations stubs module [types-aiobotocore-simspaceweaver](https://pypi.org/project/types-aiobotocore-simspaceweaver/).

## SimSpaceWeaverClient

Type annotations and code completion for `#!python session.create_client("simspaceweaver")`
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/simspaceweaver.html#SimSpaceWeaver.Client)

```python
# SimSpaceWeaverClient usage example

from aiobotocore.session import get_session
from types_aiobotocore_simspaceweaver.client import SimSpaceWeaverClient

session = get_session()
async with session.create_client("simspaceweaver") as client:
    client: SimSpaceWeaverClient
```

## Exceptions


`aiobotocore` client exceptions are generated in runtime.
This class provides code completion for `#!python session.create_client("simspaceweaver").exceptions` structure.

```python
# SimSpaceWeaverClient.exceptions usage example

async with session.create_client("simspaceweaver") as client:
    try:
        do_something(client)
    except (
            client.AccessDeniedException,
        client.ClientError,
        client.ConflictException,
        client.InternalServerException,
        client.ResourceNotFoundException,
        client.ServiceQuotaExceededException,
        client.TooManyTagsException,
        client.ValidationException,
    ) as e:
        print(e)
```

```python
# SimSpaceWeaverClient usage type checking example

from types_aiobotocore_simspaceweaver.client import Exceptions

def handle_error(exc: Exceptions.AccessDeniedException) -> None:
    ...
```


## Methods


### can\_paginate



Type annotations and code completion for `#!python session.create_client("simspaceweaver").can_paginate` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/simspaceweaver/client/can_paginate.html)

```python
# can_paginate method definition

def can_paginate(
    self,
    operation_name: str,
) -> bool:
    ...
```


### generate\_presigned\_url



Type annotations and code completion for `#!python session.create_client("simspaceweaver").generate_presigned_url` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/simspaceweaver/client/generate_presigned_url.html)

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


### create\_snapshot

Creates a snapshot of the specified simulation.

Type annotations and code completion for `#!python session.create_client("simspaceweaver").create_snapshot` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/simspaceweaver/client/create_snapshot.html)

```python
# create_snapshot method definition

await def create_snapshot(
    self,
    *,
    Destination: S3DestinationTypeDef,  # (1)
    Simulation: str,
) -> Dict[str, Any]:
    ...
```

1. See [:material-code-braces: S3DestinationTypeDef](./type_defs.md#s3destinationtypedef) 


```python
# create_snapshot method usage example with argument unpacking

kwargs: CreateSnapshotInputTypeDef = {  # (1)
    "Destination": ...,
    "Simulation": ...,
}

parent.create_snapshot(**kwargs)
```

1. See [:material-code-braces: CreateSnapshotInputTypeDef](./type_defs.md#createsnapshotinputtypedef) 

### delete\_app

Deletes the instance of the given custom app.

Type annotations and code completion for `#!python session.create_client("simspaceweaver").delete_app` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/simspaceweaver/client/delete_app.html)

```python
# delete_app method definition

await def delete_app(
    self,
    *,
    App: str,
    Domain: str,
    Simulation: str,
) -> Dict[str, Any]:
    ...
```



```python
# delete_app method usage example with argument unpacking

kwargs: DeleteAppInputTypeDef = {  # (1)
    "App": ...,
    "Domain": ...,
    "Simulation": ...,
}

parent.delete_app(**kwargs)
```

1. See [:material-code-braces: DeleteAppInputTypeDef](./type_defs.md#deleteappinputtypedef) 

### delete\_simulation

Deletes all SimSpace Weaver resources assigned to the given simulation.

Type annotations and code completion for `#!python session.create_client("simspaceweaver").delete_simulation` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/simspaceweaver/client/delete_simulation.html)

```python
# delete_simulation method definition

await def delete_simulation(
    self,
    *,
    Simulation: str,
) -> Dict[str, Any]:
    ...
```



```python
# delete_simulation method usage example with argument unpacking

kwargs: DeleteSimulationInputTypeDef = {  # (1)
    "Simulation": ...,
}

parent.delete_simulation(**kwargs)
```

1. See [:material-code-braces: DeleteSimulationInputTypeDef](./type_defs.md#deletesimulationinputtypedef) 

### describe\_app

Returns the state of the given custom app.

Type annotations and code completion for `#!python session.create_client("simspaceweaver").describe_app` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/simspaceweaver/client/describe_app.html)

```python
# describe_app method definition

await def describe_app(
    self,
    *,
    App: str,
    Domain: str,
    Simulation: str,
) -> DescribeAppOutputTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DescribeAppOutputTypeDef](./type_defs.md#describeappoutputtypedef) 


```python
# describe_app method usage example with argument unpacking

kwargs: DescribeAppInputTypeDef = {  # (1)
    "App": ...,
    "Domain": ...,
    "Simulation": ...,
}

parent.describe_app(**kwargs)
```

1. See [:material-code-braces: DescribeAppInputTypeDef](./type_defs.md#describeappinputtypedef) 

### describe\_simulation

Returns the current state of the given simulation.

Type annotations and code completion for `#!python session.create_client("simspaceweaver").describe_simulation` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/simspaceweaver/client/describe_simulation.html)

```python
# describe_simulation method definition

await def describe_simulation(
    self,
    *,
    Simulation: str,
) -> DescribeSimulationOutputTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DescribeSimulationOutputTypeDef](./type_defs.md#describesimulationoutputtypedef) 


```python
# describe_simulation method usage example with argument unpacking

kwargs: DescribeSimulationInputTypeDef = {  # (1)
    "Simulation": ...,
}

parent.describe_simulation(**kwargs)
```

1. See [:material-code-braces: DescribeSimulationInputTypeDef](./type_defs.md#describesimulationinputtypedef) 

### list\_apps

Lists all custom apps or service apps for the given simulation and domain.

Type annotations and code completion for `#!python session.create_client("simspaceweaver").list_apps` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/simspaceweaver/client/list_apps.html)

```python
# list_apps method definition

await def list_apps(
    self,
    *,
    Simulation: str,
    Domain: str = ...,
    MaxResults: int = ...,
    NextToken: str = ...,
) -> ListAppsOutputTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListAppsOutputTypeDef](./type_defs.md#listappsoutputtypedef) 


```python
# list_apps method usage example with argument unpacking

kwargs: ListAppsInputTypeDef = {  # (1)
    "Simulation": ...,
}

parent.list_apps(**kwargs)
```

1. See [:material-code-braces: ListAppsInputTypeDef](./type_defs.md#listappsinputtypedef) 

### list\_simulations

Lists the SimSpace Weaver simulations in the Amazon Web Services account used
to make the API call.

Type annotations and code completion for `#!python session.create_client("simspaceweaver").list_simulations` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/simspaceweaver/client/list_simulations.html)

```python
# list_simulations method definition

await def list_simulations(
    self,
    *,
    MaxResults: int = ...,
    NextToken: str = ...,
) -> ListSimulationsOutputTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListSimulationsOutputTypeDef](./type_defs.md#listsimulationsoutputtypedef) 


```python
# list_simulations method usage example with argument unpacking

kwargs: ListSimulationsInputTypeDef = {  # (1)
    "MaxResults": ...,
}

parent.list_simulations(**kwargs)
```

1. See [:material-code-braces: ListSimulationsInputTypeDef](./type_defs.md#listsimulationsinputtypedef) 

### list\_tags\_for\_resource

Lists all tags on a SimSpace Weaver resource.

Type annotations and code completion for `#!python session.create_client("simspaceweaver").list_tags_for_resource` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/simspaceweaver/client/list_tags_for_resource.html)

```python
# list_tags_for_resource method definition

await def list_tags_for_resource(
    self,
    *,
    ResourceArn: str,
) -> ListTagsForResourceOutputTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListTagsForResourceOutputTypeDef](./type_defs.md#listtagsforresourceoutputtypedef) 


```python
# list_tags_for_resource method usage example with argument unpacking

kwargs: ListTagsForResourceInputTypeDef = {  # (1)
    "ResourceArn": ...,
}

parent.list_tags_for_resource(**kwargs)
```

1. See [:material-code-braces: ListTagsForResourceInputTypeDef](./type_defs.md#listtagsforresourceinputtypedef) 

### start\_app

Starts a custom app with the configuration specified in the simulation schema.

Type annotations and code completion for `#!python session.create_client("simspaceweaver").start_app` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/simspaceweaver/client/start_app.html)

```python
# start_app method definition

await def start_app(
    self,
    *,
    Domain: str,
    Name: str,
    Simulation: str,
    ClientToken: str = ...,
    Description: str = ...,
    LaunchOverrides: LaunchOverridesUnionTypeDef = ...,  # (1)
) -> StartAppOutputTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: LaunchOverridesTypeDef](./type_defs.md#launchoverridestypedef) [:material-code-braces: LaunchOverridesOutputTypeDef](./type_defs.md#launchoverridesoutputtypedef) 
2. See [:material-code-braces: StartAppOutputTypeDef](./type_defs.md#startappoutputtypedef) 


```python
# start_app method usage example with argument unpacking

kwargs: StartAppInputTypeDef = {  # (1)
    "Domain": ...,
    "Name": ...,
    "Simulation": ...,
}

parent.start_app(**kwargs)
```

1. See [:material-code-braces: StartAppInputTypeDef](./type_defs.md#startappinputtypedef) 

### start\_clock

Starts the simulation clock.

Type annotations and code completion for `#!python session.create_client("simspaceweaver").start_clock` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/simspaceweaver/client/start_clock.html)

```python
# start_clock method definition

await def start_clock(
    self,
    *,
    Simulation: str,
) -> Dict[str, Any]:
    ...
```



```python
# start_clock method usage example with argument unpacking

kwargs: StartClockInputTypeDef = {  # (1)
    "Simulation": ...,
}

parent.start_clock(**kwargs)
```

1. See [:material-code-braces: StartClockInputTypeDef](./type_defs.md#startclockinputtypedef) 

### start\_simulation

Starts a simulation with the given name.

Type annotations and code completion for `#!python session.create_client("simspaceweaver").start_simulation` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/simspaceweaver/client/start_simulation.html)

```python
# start_simulation method definition

await def start_simulation(
    self,
    *,
    Name: str,
    RoleArn: str,
    ClientToken: str = ...,
    Description: str = ...,
    MaximumDuration: str = ...,
    SchemaS3Location: S3LocationTypeDef = ...,  # (1)
    SnapshotS3Location: S3LocationTypeDef = ...,  # (1)
    Tags: Mapping[str, str] = ...,
) -> StartSimulationOutputTypeDef:  # (3)
    ...
```

1. See [:material-code-braces: S3LocationTypeDef](./type_defs.md#s3locationtypedef) 
2. See [:material-code-braces: S3LocationTypeDef](./type_defs.md#s3locationtypedef) 
3. See [:material-code-braces: StartSimulationOutputTypeDef](./type_defs.md#startsimulationoutputtypedef) 


```python
# start_simulation method usage example with argument unpacking

kwargs: StartSimulationInputTypeDef = {  # (1)
    "Name": ...,
    "RoleArn": ...,
}

parent.start_simulation(**kwargs)
```

1. See [:material-code-braces: StartSimulationInputTypeDef](./type_defs.md#startsimulationinputtypedef) 

### stop\_app

Stops the given custom app and shuts down all of its allocated compute
resources.

Type annotations and code completion for `#!python session.create_client("simspaceweaver").stop_app` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/simspaceweaver/client/stop_app.html)

```python
# stop_app method definition

await def stop_app(
    self,
    *,
    App: str,
    Domain: str,
    Simulation: str,
) -> Dict[str, Any]:
    ...
```



```python
# stop_app method usage example with argument unpacking

kwargs: StopAppInputTypeDef = {  # (1)
    "App": ...,
    "Domain": ...,
    "Simulation": ...,
}

parent.stop_app(**kwargs)
```

1. See [:material-code-braces: StopAppInputTypeDef](./type_defs.md#stopappinputtypedef) 

### stop\_clock

Stops the simulation clock.

Type annotations and code completion for `#!python session.create_client("simspaceweaver").stop_clock` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/simspaceweaver/client/stop_clock.html)

```python
# stop_clock method definition

await def stop_clock(
    self,
    *,
    Simulation: str,
) -> Dict[str, Any]:
    ...
```



```python
# stop_clock method usage example with argument unpacking

kwargs: StopClockInputTypeDef = {  # (1)
    "Simulation": ...,
}

parent.stop_clock(**kwargs)
```

1. See [:material-code-braces: StopClockInputTypeDef](./type_defs.md#stopclockinputtypedef) 

### stop\_simulation

Stops the given simulation.

Type annotations and code completion for `#!python session.create_client("simspaceweaver").stop_simulation` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/simspaceweaver/client/stop_simulation.html)

```python
# stop_simulation method definition

await def stop_simulation(
    self,
    *,
    Simulation: str,
) -> Dict[str, Any]:
    ...
```



```python
# stop_simulation method usage example with argument unpacking

kwargs: StopSimulationInputTypeDef = {  # (1)
    "Simulation": ...,
}

parent.stop_simulation(**kwargs)
```

1. See [:material-code-braces: StopSimulationInputTypeDef](./type_defs.md#stopsimulationinputtypedef) 

### tag\_resource

Adds tags to a SimSpace Weaver resource.

Type annotations and code completion for `#!python session.create_client("simspaceweaver").tag_resource` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/simspaceweaver/client/tag_resource.html)

```python
# tag_resource method definition

await def tag_resource(
    self,
    *,
    ResourceArn: str,
    Tags: Mapping[str, str],
) -> Dict[str, Any]:
    ...
```



```python
# tag_resource method usage example with argument unpacking

kwargs: TagResourceInputTypeDef = {  # (1)
    "ResourceArn": ...,
    "Tags": ...,
}

parent.tag_resource(**kwargs)
```

1. See [:material-code-braces: TagResourceInputTypeDef](./type_defs.md#tagresourceinputtypedef) 

### untag\_resource

Removes tags from a SimSpace Weaver resource.

Type annotations and code completion for `#!python session.create_client("simspaceweaver").untag_resource` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/simspaceweaver/client/untag_resource.html)

```python
# untag_resource method definition

await def untag_resource(
    self,
    *,
    ResourceArn: str,
    TagKeys: Sequence[str],
) -> Dict[str, Any]:
    ...
```



```python
# untag_resource method usage example with argument unpacking

kwargs: UntagResourceInputTypeDef = {  # (1)
    "ResourceArn": ...,
    "TagKeys": ...,
}

parent.untag_resource(**kwargs)
```

1. See [:material-code-braces: UntagResourceInputTypeDef](./type_defs.md#untagresourceinputtypedef) 

### \_\_aenter\_\_



Type annotations and code completion for `#!python session.create_client("simspaceweaver").__aenter__` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/simspaceweaver.html#SimSpaceWeaver.Client)

```python
# __aenter__ method definition

await def __aenter__(
    self,
) -> Self:
    ...
```


### \_\_aexit\_\_



Type annotations and code completion for `#!python session.create_client("simspaceweaver").__aexit__` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/simspaceweaver.html#SimSpaceWeaver.Client)

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





