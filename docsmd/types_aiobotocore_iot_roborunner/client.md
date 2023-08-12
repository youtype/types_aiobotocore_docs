# IoTRoboRunnerClient

> [Index](../README.md) > [IoTRoboRunner](./README.md) > IoTRoboRunnerClient

!!! note ""

    Auto-generated documentation for [IoTRoboRunner](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot-roborunner.html#IoTRoboRunner)
    type annotations stubs module [types-aiobotocore-iot-roborunner](https://pypi.org/project/types-aiobotocore-iot-roborunner/).

## IoTRoboRunnerClient

Type annotations and code completion for `#!python session.create_client("iot-roborunner")`
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot-roborunner.html#IoTRoboRunner.Client)

```python
IoTRoboRunnerClient usage example

from aiobotocore.session import get_session
from types_aiobotocore_iot_roborunner.client import IoTRoboRunnerClient

session = get_session()
async with session.create_client("iot-roborunner") as client:
    client: IoTRoboRunnerClient
```

## Exceptions


`aiobotocore` client exceptions are generated in runtime.
This class provides code completion for `#!python session.create_client("iot-roborunner").exceptions` structure.

```python
IoTRoboRunnerClient.exceptions usage example

async with session.create_client("iot-roborunner") as client:
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
IoTRoboRunnerClient usage type checking example

from types_aiobotocore_iot_roborunner.client import Exceptions

def handle_error(exc: Exceptions.AccessDeniedException) -> None:
    ...
```


## Methods


### can\_paginate

Check if an operation can be paginated.

Type annotations and code completion for `#!python session.create_client("iot-roborunner").can_paginate` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot-roborunner.html#IoTRoboRunner.Client.can_paginate)

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

Type annotations and code completion for `#!python session.create_client("iot-roborunner").close` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot-roborunner.html#IoTRoboRunner.Client.close)

```python
# close method definition

await def close(
    self,
) -> None:
    ...
```


### create\_destination

Grants permission to create a destination See also: [AWS API
Documentation](https://docs.aws.amazon.com/goto/WebAPI/iot-
roborunner-2018-05-10/CreateDestination).

Type annotations and code completion for `#!python session.create_client("iot-roborunner").create_destination` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot-roborunner.html#IoTRoboRunner.Client.create_destination)

```python
# create_destination method definition

await def create_destination(
    self,
    *,
    name: str,
    site: str,
    clientToken: str = ...,
    state: DestinationStateType = ...,  # (1)
    additionalFixedProperties: str = ...,
) -> CreateDestinationResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-brackets: DestinationStateType](./literals.md#destinationstatetype) 
2. See [:material-code-braces: CreateDestinationResponseTypeDef](./type_defs.md#createdestinationresponsetypedef) 


```python
# create_destination method usage example with argument unpacking

kwargs: CreateDestinationRequestRequestTypeDef = {  # (1)
    "name": ...,
    "site": ...,
}

parent.create_destination(**kwargs)
```

1. See [:material-code-braces: CreateDestinationRequestRequestTypeDef](./type_defs.md#createdestinationrequestrequesttypedef) 

### create\_site

Grants permission to create a site See also: [AWS API
Documentation](https://docs.aws.amazon.com/goto/WebAPI/iot-
roborunner-2018-05-10/CreateSite).

Type annotations and code completion for `#!python session.create_client("iot-roborunner").create_site` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot-roborunner.html#IoTRoboRunner.Client.create_site)

```python
# create_site method definition

await def create_site(
    self,
    *,
    name: str,
    countryCode: str,
    clientToken: str = ...,
    description: str = ...,
) -> CreateSiteResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: CreateSiteResponseTypeDef](./type_defs.md#createsiteresponsetypedef) 


```python
# create_site method usage example with argument unpacking

kwargs: CreateSiteRequestRequestTypeDef = {  # (1)
    "name": ...,
    "countryCode": ...,
}

parent.create_site(**kwargs)
```

1. See [:material-code-braces: CreateSiteRequestRequestTypeDef](./type_defs.md#createsiterequestrequesttypedef) 

### create\_worker

Grants permission to create a worker See also: [AWS API
Documentation](https://docs.aws.amazon.com/goto/WebAPI/iot-
roborunner-2018-05-10/CreateWorker).

Type annotations and code completion for `#!python session.create_client("iot-roborunner").create_worker` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot-roborunner.html#IoTRoboRunner.Client.create_worker)

```python
# create_worker method definition

await def create_worker(
    self,
    *,
    name: str,
    fleet: str,
    clientToken: str = ...,
    additionalTransientProperties: str = ...,
    additionalFixedProperties: str = ...,
    vendorProperties: VendorPropertiesTypeDef = ...,  # (1)
    position: PositionCoordinatesTypeDef = ...,  # (2)
    orientation: OrientationTypeDef = ...,  # (3)
) -> CreateWorkerResponseTypeDef:  # (4)
    ...
```

1. See [:material-code-braces: VendorPropertiesTypeDef](./type_defs.md#vendorpropertiestypedef) 
2. See [:material-code-braces: PositionCoordinatesTypeDef](./type_defs.md#positioncoordinatestypedef) 
3. See [:material-code-braces: OrientationTypeDef](./type_defs.md#orientationtypedef) 
4. See [:material-code-braces: CreateWorkerResponseTypeDef](./type_defs.md#createworkerresponsetypedef) 


```python
# create_worker method usage example with argument unpacking

kwargs: CreateWorkerRequestRequestTypeDef = {  # (1)
    "name": ...,
    "fleet": ...,
}

parent.create_worker(**kwargs)
```

1. See [:material-code-braces: CreateWorkerRequestRequestTypeDef](./type_defs.md#createworkerrequestrequesttypedef) 

### create\_worker\_fleet

Grants permission to create a worker fleet See also: [AWS API
Documentation](https://docs.aws.amazon.com/goto/WebAPI/iot-
roborunner-2018-05-10/CreateWorkerFleet).

Type annotations and code completion for `#!python session.create_client("iot-roborunner").create_worker_fleet` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot-roborunner.html#IoTRoboRunner.Client.create_worker_fleet)

```python
# create_worker_fleet method definition

await def create_worker_fleet(
    self,
    *,
    name: str,
    site: str,
    clientToken: str = ...,
    additionalFixedProperties: str = ...,
) -> CreateWorkerFleetResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: CreateWorkerFleetResponseTypeDef](./type_defs.md#createworkerfleetresponsetypedef) 


```python
# create_worker_fleet method usage example with argument unpacking

kwargs: CreateWorkerFleetRequestRequestTypeDef = {  # (1)
    "name": ...,
    "site": ...,
}

parent.create_worker_fleet(**kwargs)
```

1. See [:material-code-braces: CreateWorkerFleetRequestRequestTypeDef](./type_defs.md#createworkerfleetrequestrequesttypedef) 

### delete\_destination

Grants permission to delete a destination See also: [AWS API
Documentation](https://docs.aws.amazon.com/goto/WebAPI/iot-
roborunner-2018-05-10/DeleteDestination).

Type annotations and code completion for `#!python session.create_client("iot-roborunner").delete_destination` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot-roborunner.html#IoTRoboRunner.Client.delete_destination)

```python
# delete_destination method definition

await def delete_destination(
    self,
    *,
    id: str,
) -> Dict[str, Any]:
    ...
```



```python
# delete_destination method usage example with argument unpacking

kwargs: DeleteDestinationRequestRequestTypeDef = {  # (1)
    "id": ...,
}

parent.delete_destination(**kwargs)
```

1. See [:material-code-braces: DeleteDestinationRequestRequestTypeDef](./type_defs.md#deletedestinationrequestrequesttypedef) 

### delete\_site

Grants permission to delete a site See also: [AWS API
Documentation](https://docs.aws.amazon.com/goto/WebAPI/iot-
roborunner-2018-05-10/DeleteSite).

Type annotations and code completion for `#!python session.create_client("iot-roborunner").delete_site` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot-roborunner.html#IoTRoboRunner.Client.delete_site)

```python
# delete_site method definition

await def delete_site(
    self,
    *,
    id: str,
) -> Dict[str, Any]:
    ...
```



```python
# delete_site method usage example with argument unpacking

kwargs: DeleteSiteRequestRequestTypeDef = {  # (1)
    "id": ...,
}

parent.delete_site(**kwargs)
```

1. See [:material-code-braces: DeleteSiteRequestRequestTypeDef](./type_defs.md#deletesiterequestrequesttypedef) 

### delete\_worker

Grants permission to delete a worker See also: [AWS API
Documentation](https://docs.aws.amazon.com/goto/WebAPI/iot-
roborunner-2018-05-10/DeleteWorker).

Type annotations and code completion for `#!python session.create_client("iot-roborunner").delete_worker` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot-roborunner.html#IoTRoboRunner.Client.delete_worker)

```python
# delete_worker method definition

await def delete_worker(
    self,
    *,
    id: str,
) -> Dict[str, Any]:
    ...
```



```python
# delete_worker method usage example with argument unpacking

kwargs: DeleteWorkerRequestRequestTypeDef = {  # (1)
    "id": ...,
}

parent.delete_worker(**kwargs)
```

1. See [:material-code-braces: DeleteWorkerRequestRequestTypeDef](./type_defs.md#deleteworkerrequestrequesttypedef) 

### delete\_worker\_fleet

Grants permission to delete a worker fleet See also: [AWS API
Documentation](https://docs.aws.amazon.com/goto/WebAPI/iot-
roborunner-2018-05-10/DeleteWorkerFleet).

Type annotations and code completion for `#!python session.create_client("iot-roborunner").delete_worker_fleet` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot-roborunner.html#IoTRoboRunner.Client.delete_worker_fleet)

```python
# delete_worker_fleet method definition

await def delete_worker_fleet(
    self,
    *,
    id: str,
) -> Dict[str, Any]:
    ...
```



```python
# delete_worker_fleet method usage example with argument unpacking

kwargs: DeleteWorkerFleetRequestRequestTypeDef = {  # (1)
    "id": ...,
}

parent.delete_worker_fleet(**kwargs)
```

1. See [:material-code-braces: DeleteWorkerFleetRequestRequestTypeDef](./type_defs.md#deleteworkerfleetrequestrequesttypedef) 

### generate\_presigned\_url

Generate a presigned url given a client, its method, and arguments.

Type annotations and code completion for `#!python session.create_client("iot-roborunner").generate_presigned_url` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot-roborunner.html#IoTRoboRunner.Client.generate_presigned_url)

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


### get\_destination

Grants permission to get a destination See also: [AWS API
Documentation](https://docs.aws.amazon.com/goto/WebAPI/iot-
roborunner-2018-05-10/GetDestination).

Type annotations and code completion for `#!python session.create_client("iot-roborunner").get_destination` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot-roborunner.html#IoTRoboRunner.Client.get_destination)

```python
# get_destination method definition

await def get_destination(
    self,
    *,
    id: str,
) -> GetDestinationResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetDestinationResponseTypeDef](./type_defs.md#getdestinationresponsetypedef) 


```python
# get_destination method usage example with argument unpacking

kwargs: GetDestinationRequestRequestTypeDef = {  # (1)
    "id": ...,
}

parent.get_destination(**kwargs)
```

1. See [:material-code-braces: GetDestinationRequestRequestTypeDef](./type_defs.md#getdestinationrequestrequesttypedef) 

### get\_site

Grants permission to get a site See also: [AWS API
Documentation](https://docs.aws.amazon.com/goto/WebAPI/iot-
roborunner-2018-05-10/GetSite).

Type annotations and code completion for `#!python session.create_client("iot-roborunner").get_site` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot-roborunner.html#IoTRoboRunner.Client.get_site)

```python
# get_site method definition

await def get_site(
    self,
    *,
    id: str,
) -> GetSiteResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetSiteResponseTypeDef](./type_defs.md#getsiteresponsetypedef) 


```python
# get_site method usage example with argument unpacking

kwargs: GetSiteRequestRequestTypeDef = {  # (1)
    "id": ...,
}

parent.get_site(**kwargs)
```

1. See [:material-code-braces: GetSiteRequestRequestTypeDef](./type_defs.md#getsiterequestrequesttypedef) 

### get\_worker

Grants permission to get a worker See also: [AWS API
Documentation](https://docs.aws.amazon.com/goto/WebAPI/iot-
roborunner-2018-05-10/GetWorker).

Type annotations and code completion for `#!python session.create_client("iot-roborunner").get_worker` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot-roborunner.html#IoTRoboRunner.Client.get_worker)

```python
# get_worker method definition

await def get_worker(
    self,
    *,
    id: str,
) -> GetWorkerResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetWorkerResponseTypeDef](./type_defs.md#getworkerresponsetypedef) 


```python
# get_worker method usage example with argument unpacking

kwargs: GetWorkerRequestRequestTypeDef = {  # (1)
    "id": ...,
}

parent.get_worker(**kwargs)
```

1. See [:material-code-braces: GetWorkerRequestRequestTypeDef](./type_defs.md#getworkerrequestrequesttypedef) 

### get\_worker\_fleet

Grants permission to get a worker fleet See also: [AWS API
Documentation](https://docs.aws.amazon.com/goto/WebAPI/iot-
roborunner-2018-05-10/GetWorkerFleet).

Type annotations and code completion for `#!python session.create_client("iot-roborunner").get_worker_fleet` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot-roborunner.html#IoTRoboRunner.Client.get_worker_fleet)

```python
# get_worker_fleet method definition

await def get_worker_fleet(
    self,
    *,
    id: str,
) -> GetWorkerFleetResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetWorkerFleetResponseTypeDef](./type_defs.md#getworkerfleetresponsetypedef) 


```python
# get_worker_fleet method usage example with argument unpacking

kwargs: GetWorkerFleetRequestRequestTypeDef = {  # (1)
    "id": ...,
}

parent.get_worker_fleet(**kwargs)
```

1. See [:material-code-braces: GetWorkerFleetRequestRequestTypeDef](./type_defs.md#getworkerfleetrequestrequesttypedef) 

### list\_destinations

Grants permission to list destinations See also: [AWS API
Documentation](https://docs.aws.amazon.com/goto/WebAPI/iot-
roborunner-2018-05-10/ListDestinations).

Type annotations and code completion for `#!python session.create_client("iot-roborunner").list_destinations` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot-roborunner.html#IoTRoboRunner.Client.list_destinations)

```python
# list_destinations method definition

await def list_destinations(
    self,
    *,
    site: str,
    maxResults: int = ...,
    nextToken: str = ...,
    state: DestinationStateType = ...,  # (1)
) -> ListDestinationsResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-brackets: DestinationStateType](./literals.md#destinationstatetype) 
2. See [:material-code-braces: ListDestinationsResponseTypeDef](./type_defs.md#listdestinationsresponsetypedef) 


```python
# list_destinations method usage example with argument unpacking

kwargs: ListDestinationsRequestRequestTypeDef = {  # (1)
    "site": ...,
}

parent.list_destinations(**kwargs)
```

1. See [:material-code-braces: ListDestinationsRequestRequestTypeDef](./type_defs.md#listdestinationsrequestrequesttypedef) 

### list\_sites

Grants permission to list sites See also: [AWS API
Documentation](https://docs.aws.amazon.com/goto/WebAPI/iot-
roborunner-2018-05-10/ListSites).

Type annotations and code completion for `#!python session.create_client("iot-roborunner").list_sites` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot-roborunner.html#IoTRoboRunner.Client.list_sites)

```python
# list_sites method definition

await def list_sites(
    self,
    *,
    maxResults: int = ...,
    nextToken: str = ...,
) -> ListSitesResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListSitesResponseTypeDef](./type_defs.md#listsitesresponsetypedef) 


```python
# list_sites method usage example with argument unpacking

kwargs: ListSitesRequestRequestTypeDef = {  # (1)
    "maxResults": ...,
}

parent.list_sites(**kwargs)
```

1. See [:material-code-braces: ListSitesRequestRequestTypeDef](./type_defs.md#listsitesrequestrequesttypedef) 

### list\_worker\_fleets

Grants permission to list worker fleets See also: [AWS API
Documentation](https://docs.aws.amazon.com/goto/WebAPI/iot-
roborunner-2018-05-10/ListWorkerFleets).

Type annotations and code completion for `#!python session.create_client("iot-roborunner").list_worker_fleets` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot-roborunner.html#IoTRoboRunner.Client.list_worker_fleets)

```python
# list_worker_fleets method definition

await def list_worker_fleets(
    self,
    *,
    site: str,
    maxResults: int = ...,
    nextToken: str = ...,
) -> ListWorkerFleetsResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListWorkerFleetsResponseTypeDef](./type_defs.md#listworkerfleetsresponsetypedef) 


```python
# list_worker_fleets method usage example with argument unpacking

kwargs: ListWorkerFleetsRequestRequestTypeDef = {  # (1)
    "site": ...,
}

parent.list_worker_fleets(**kwargs)
```

1. See [:material-code-braces: ListWorkerFleetsRequestRequestTypeDef](./type_defs.md#listworkerfleetsrequestrequesttypedef) 

### list\_workers

Grants permission to list workers See also: [AWS API
Documentation](https://docs.aws.amazon.com/goto/WebAPI/iot-
roborunner-2018-05-10/ListWorkers).

Type annotations and code completion for `#!python session.create_client("iot-roborunner").list_workers` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot-roborunner.html#IoTRoboRunner.Client.list_workers)

```python
# list_workers method definition

await def list_workers(
    self,
    *,
    site: str,
    maxResults: int = ...,
    nextToken: str = ...,
    fleet: str = ...,
) -> ListWorkersResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListWorkersResponseTypeDef](./type_defs.md#listworkersresponsetypedef) 


```python
# list_workers method usage example with argument unpacking

kwargs: ListWorkersRequestRequestTypeDef = {  # (1)
    "site": ...,
}

parent.list_workers(**kwargs)
```

1. See [:material-code-braces: ListWorkersRequestRequestTypeDef](./type_defs.md#listworkersrequestrequesttypedef) 

### update\_destination

Grants permission to update a destination See also: [AWS API
Documentation](https://docs.aws.amazon.com/goto/WebAPI/iot-
roborunner-2018-05-10/UpdateDestination).

Type annotations and code completion for `#!python session.create_client("iot-roborunner").update_destination` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot-roborunner.html#IoTRoboRunner.Client.update_destination)

```python
# update_destination method definition

await def update_destination(
    self,
    *,
    id: str,
    name: str = ...,
    state: DestinationStateType = ...,  # (1)
    additionalFixedProperties: str = ...,
) -> UpdateDestinationResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-brackets: DestinationStateType](./literals.md#destinationstatetype) 
2. See [:material-code-braces: UpdateDestinationResponseTypeDef](./type_defs.md#updatedestinationresponsetypedef) 


```python
# update_destination method usage example with argument unpacking

kwargs: UpdateDestinationRequestRequestTypeDef = {  # (1)
    "id": ...,
}

parent.update_destination(**kwargs)
```

1. See [:material-code-braces: UpdateDestinationRequestRequestTypeDef](./type_defs.md#updatedestinationrequestrequesttypedef) 

### update\_site

Grants permission to update a site See also: [AWS API
Documentation](https://docs.aws.amazon.com/goto/WebAPI/iot-
roborunner-2018-05-10/UpdateSite).

Type annotations and code completion for `#!python session.create_client("iot-roborunner").update_site` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot-roborunner.html#IoTRoboRunner.Client.update_site)

```python
# update_site method definition

await def update_site(
    self,
    *,
    id: str,
    name: str = ...,
    countryCode: str = ...,
    description: str = ...,
) -> UpdateSiteResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: UpdateSiteResponseTypeDef](./type_defs.md#updatesiteresponsetypedef) 


```python
# update_site method usage example with argument unpacking

kwargs: UpdateSiteRequestRequestTypeDef = {  # (1)
    "id": ...,
}

parent.update_site(**kwargs)
```

1. See [:material-code-braces: UpdateSiteRequestRequestTypeDef](./type_defs.md#updatesiterequestrequesttypedef) 

### update\_worker

Grants permission to update a worker See also: [AWS API
Documentation](https://docs.aws.amazon.com/goto/WebAPI/iot-
roborunner-2018-05-10/UpdateWorker).

Type annotations and code completion for `#!python session.create_client("iot-roborunner").update_worker` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot-roborunner.html#IoTRoboRunner.Client.update_worker)

```python
# update_worker method definition

await def update_worker(
    self,
    *,
    id: str,
    name: str = ...,
    additionalTransientProperties: str = ...,
    additionalFixedProperties: str = ...,
    vendorProperties: VendorPropertiesTypeDef = ...,  # (1)
    position: PositionCoordinatesTypeDef = ...,  # (2)
    orientation: OrientationTypeDef = ...,  # (3)
) -> UpdateWorkerResponseTypeDef:  # (4)
    ...
```

1. See [:material-code-braces: VendorPropertiesTypeDef](./type_defs.md#vendorpropertiestypedef) 
2. See [:material-code-braces: PositionCoordinatesTypeDef](./type_defs.md#positioncoordinatestypedef) 
3. See [:material-code-braces: OrientationTypeDef](./type_defs.md#orientationtypedef) 
4. See [:material-code-braces: UpdateWorkerResponseTypeDef](./type_defs.md#updateworkerresponsetypedef) 


```python
# update_worker method usage example with argument unpacking

kwargs: UpdateWorkerRequestRequestTypeDef = {  # (1)
    "id": ...,
}

parent.update_worker(**kwargs)
```

1. See [:material-code-braces: UpdateWorkerRequestRequestTypeDef](./type_defs.md#updateworkerrequestrequesttypedef) 

### update\_worker\_fleet

Grants permission to update a worker fleet See also: [AWS API
Documentation](https://docs.aws.amazon.com/goto/WebAPI/iot-
roborunner-2018-05-10/UpdateWorkerFleet).

Type annotations and code completion for `#!python session.create_client("iot-roborunner").update_worker_fleet` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot-roborunner.html#IoTRoboRunner.Client.update_worker_fleet)

```python
# update_worker_fleet method definition

await def update_worker_fleet(
    self,
    *,
    id: str,
    name: str = ...,
    additionalFixedProperties: str = ...,
) -> UpdateWorkerFleetResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: UpdateWorkerFleetResponseTypeDef](./type_defs.md#updateworkerfleetresponsetypedef) 


```python
# update_worker_fleet method usage example with argument unpacking

kwargs: UpdateWorkerFleetRequestRequestTypeDef = {  # (1)
    "id": ...,
}

parent.update_worker_fleet(**kwargs)
```

1. See [:material-code-braces: UpdateWorkerFleetRequestRequestTypeDef](./type_defs.md#updateworkerfleetrequestrequesttypedef) 

### \_\_aenter\_\_



Type annotations and code completion for `#!python session.create_client("iot-roborunner").__aenter__` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot-roborunner.html#IoTRoboRunner.Client.__aenter__)

```python
# __aenter__ method definition

await def __aenter__(
    self,
) -> IoTRoboRunnerClient:
    ...
```


### \_\_aexit\_\_



Type annotations and code completion for `#!python session.create_client("iot-roborunner").__aexit__` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot-roborunner.html#IoTRoboRunner.Client.__aexit__)

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

Type annotations and code completion for `#!python session.create_client("iot-roborunner").get_paginator` method with overloads.

- `client.get_paginator("list_destinations")` -> [ListDestinationsPaginator](./paginators.md#listdestinationspaginator)
- `client.get_paginator("list_sites")` -> [ListSitesPaginator](./paginators.md#listsitespaginator)
- `client.get_paginator("list_worker_fleets")` -> [ListWorkerFleetsPaginator](./paginators.md#listworkerfleetspaginator)
- `client.get_paginator("list_workers")` -> [ListWorkersPaginator](./paginators.md#listworkerspaginator)



