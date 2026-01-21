# Paginators

> [Index](../README.md) > [DeviceFarm](./README.md) > Paginators

!!! note ""

    Auto-generated documentation for [DeviceFarm](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/devicefarm.html#devicefarm)
    type annotations stubs module [types-aiobotocore-devicefarm](https://pypi.org/project/types-aiobotocore-devicefarm/).

## GetOfferingStatusPaginator

Type annotations and code completion for `#!python session.create_client("devicefarm").get_paginator("get_offering_status")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/devicefarm/paginator/GetOfferingStatus.html#DeviceFarm.Paginator.GetOfferingStatus)

```python
# GetOfferingStatusPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_devicefarm.paginator import GetOfferingStatusPaginator

session = get_session()
async with session.create_client("devicefarm") as client:  # (1)
    paginator: GetOfferingStatusPaginator = client.get_paginator("get_offering_status")  # (2)
    async for item in paginator.paginate(...):
        item: GetOfferingStatusResultTypeDef
        print(item)  # (3)
```

1. client: [DeviceFarmClient](./client.md)
2. paginator: [GetOfferingStatusPaginator](./paginators.md#getofferingstatuspaginator)
3. item: `AioPageIterator[GetOfferingStatusResultTypeDef]`


### paginate

Type annotations and code completion for `#!python GetOfferingStatusPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> aiobotocore.paginate.AioPageIterator[GetOfferingStatusResultTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
2. See `AioPageIterator[GetOfferingStatusResultTypeDef]`


```python
# paginate method usage example with argument unpacking

kwargs: GetOfferingStatusRequestPaginateTypeDef = {  # (1)
    "PaginationConfig": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: GetOfferingStatusRequestPaginateTypeDef](./type_defs.md#getofferingstatusrequestpaginatetypedef)
## ListArtifactsPaginator

Type annotations and code completion for `#!python session.create_client("devicefarm").get_paginator("list_artifacts")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/devicefarm/paginator/ListArtifacts.html#DeviceFarm.Paginator.ListArtifacts)

```python
# ListArtifactsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_devicefarm.paginator import ListArtifactsPaginator

session = get_session()
async with session.create_client("devicefarm") as client:  # (1)
    paginator: ListArtifactsPaginator = client.get_paginator("list_artifacts")  # (2)
    async for item in paginator.paginate(...):
        item: ListArtifactsResultTypeDef
        print(item)  # (3)
```

1. client: [DeviceFarmClient](./client.md)
2. paginator: [ListArtifactsPaginator](./paginators.md#listartifactspaginator)
3. item: `AioPageIterator[ListArtifactsResultTypeDef]`


### paginate

Type annotations and code completion for `#!python ListArtifactsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    arn: str,
    type: ArtifactCategoryType,  # (1)
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (2)
) -> aiobotocore.paginate.AioPageIterator[ListArtifactsResultTypeDef]:  # (3)
    ...
```

1. See [:material-code-brackets: ArtifactCategoryType](./literals.md#artifactcategorytype)
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
3. See `AioPageIterator[ListArtifactsResultTypeDef]`


```python
# paginate method usage example with argument unpacking

kwargs: ListArtifactsRequestPaginateTypeDef = {  # (1)
    "arn": ...,
    "type": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListArtifactsRequestPaginateTypeDef](./type_defs.md#listartifactsrequestpaginatetypedef)
## ListDeviceInstancesPaginator

Type annotations and code completion for `#!python session.create_client("devicefarm").get_paginator("list_device_instances")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/devicefarm/paginator/ListDeviceInstances.html#DeviceFarm.Paginator.ListDeviceInstances)

```python
# ListDeviceInstancesPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_devicefarm.paginator import ListDeviceInstancesPaginator

session = get_session()
async with session.create_client("devicefarm") as client:  # (1)
    paginator: ListDeviceInstancesPaginator = client.get_paginator("list_device_instances")  # (2)
    async for item in paginator.paginate(...):
        item: ListDeviceInstancesResultTypeDef
        print(item)  # (3)
```

1. client: [DeviceFarmClient](./client.md)
2. paginator: [ListDeviceInstancesPaginator](./paginators.md#listdeviceinstancespaginator)
3. item: `AioPageIterator[ListDeviceInstancesResultTypeDef]`


### paginate

Type annotations and code completion for `#!python ListDeviceInstancesPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> aiobotocore.paginate.AioPageIterator[ListDeviceInstancesResultTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
2. See `AioPageIterator[ListDeviceInstancesResultTypeDef]`


```python
# paginate method usage example with argument unpacking

kwargs: ListDeviceInstancesRequestPaginateTypeDef = {  # (1)
    "PaginationConfig": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListDeviceInstancesRequestPaginateTypeDef](./type_defs.md#listdeviceinstancesrequestpaginatetypedef)
## ListDevicePoolsPaginator

Type annotations and code completion for `#!python session.create_client("devicefarm").get_paginator("list_device_pools")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/devicefarm/paginator/ListDevicePools.html#DeviceFarm.Paginator.ListDevicePools)

```python
# ListDevicePoolsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_devicefarm.paginator import ListDevicePoolsPaginator

session = get_session()
async with session.create_client("devicefarm") as client:  # (1)
    paginator: ListDevicePoolsPaginator = client.get_paginator("list_device_pools")  # (2)
    async for item in paginator.paginate(...):
        item: ListDevicePoolsResultTypeDef
        print(item)  # (3)
```

1. client: [DeviceFarmClient](./client.md)
2. paginator: [ListDevicePoolsPaginator](./paginators.md#listdevicepoolspaginator)
3. item: `AioPageIterator[ListDevicePoolsResultTypeDef]`


### paginate

Type annotations and code completion for `#!python ListDevicePoolsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    arn: str,
    type: DevicePoolTypeType = ...,  # (1)
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (2)
) -> aiobotocore.paginate.AioPageIterator[ListDevicePoolsResultTypeDef]:  # (3)
    ...
```

1. See [:material-code-brackets: DevicePoolTypeType](./literals.md#devicepooltypetype)
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
3. See `AioPageIterator[ListDevicePoolsResultTypeDef]`


```python
# paginate method usage example with argument unpacking

kwargs: ListDevicePoolsRequestPaginateTypeDef = {  # (1)
    "arn": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListDevicePoolsRequestPaginateTypeDef](./type_defs.md#listdevicepoolsrequestpaginatetypedef)
## ListDevicesPaginator

Type annotations and code completion for `#!python session.create_client("devicefarm").get_paginator("list_devices")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/devicefarm/paginator/ListDevices.html#DeviceFarm.Paginator.ListDevices)

```python
# ListDevicesPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_devicefarm.paginator import ListDevicesPaginator

session = get_session()
async with session.create_client("devicefarm") as client:  # (1)
    paginator: ListDevicesPaginator = client.get_paginator("list_devices")  # (2)
    async for item in paginator.paginate(...):
        item: ListDevicesResultTypeDef
        print(item)  # (3)
```

1. client: [DeviceFarmClient](./client.md)
2. paginator: [ListDevicesPaginator](./paginators.md#listdevicespaginator)
3. item: `AioPageIterator[ListDevicesResultTypeDef]`


### paginate

Type annotations and code completion for `#!python ListDevicesPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    arn: str = ...,
    filters: Sequence[DeviceFilterUnionTypeDef] = ...,  # (1)
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (2)
) -> aiobotocore.paginate.AioPageIterator[ListDevicesResultTypeDef]:  # (3)
    ...
```

1. See `Sequence[DeviceFilterUnionTypeDef]`
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
3. See `AioPageIterator[ListDevicesResultTypeDef]`


```python
# paginate method usage example with argument unpacking

kwargs: ListDevicesRequestPaginateTypeDef = {  # (1)
    "arn": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListDevicesRequestPaginateTypeDef](./type_defs.md#listdevicesrequestpaginatetypedef)
## ListInstanceProfilesPaginator

Type annotations and code completion for `#!python session.create_client("devicefarm").get_paginator("list_instance_profiles")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/devicefarm/paginator/ListInstanceProfiles.html#DeviceFarm.Paginator.ListInstanceProfiles)

```python
# ListInstanceProfilesPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_devicefarm.paginator import ListInstanceProfilesPaginator

session = get_session()
async with session.create_client("devicefarm") as client:  # (1)
    paginator: ListInstanceProfilesPaginator = client.get_paginator("list_instance_profiles")  # (2)
    async for item in paginator.paginate(...):
        item: ListInstanceProfilesResultTypeDef
        print(item)  # (3)
```

1. client: [DeviceFarmClient](./client.md)
2. paginator: [ListInstanceProfilesPaginator](./paginators.md#listinstanceprofilespaginator)
3. item: `AioPageIterator[ListInstanceProfilesResultTypeDef]`


### paginate

Type annotations and code completion for `#!python ListInstanceProfilesPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> aiobotocore.paginate.AioPageIterator[ListInstanceProfilesResultTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
2. See `AioPageIterator[ListInstanceProfilesResultTypeDef]`


```python
# paginate method usage example with argument unpacking

kwargs: ListInstanceProfilesRequestPaginateTypeDef = {  # (1)
    "PaginationConfig": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListInstanceProfilesRequestPaginateTypeDef](./type_defs.md#listinstanceprofilesrequestpaginatetypedef)
## ListJobsPaginator

Type annotations and code completion for `#!python session.create_client("devicefarm").get_paginator("list_jobs")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/devicefarm/paginator/ListJobs.html#DeviceFarm.Paginator.ListJobs)

```python
# ListJobsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_devicefarm.paginator import ListJobsPaginator

session = get_session()
async with session.create_client("devicefarm") as client:  # (1)
    paginator: ListJobsPaginator = client.get_paginator("list_jobs")  # (2)
    async for item in paginator.paginate(...):
        item: ListJobsResultTypeDef
        print(item)  # (3)
```

1. client: [DeviceFarmClient](./client.md)
2. paginator: [ListJobsPaginator](./paginators.md#listjobspaginator)
3. item: `AioPageIterator[ListJobsResultTypeDef]`


### paginate

Type annotations and code completion for `#!python ListJobsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    arn: str,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> aiobotocore.paginate.AioPageIterator[ListJobsResultTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
2. See `AioPageIterator[ListJobsResultTypeDef]`


```python
# paginate method usage example with argument unpacking

kwargs: ListJobsRequestPaginateTypeDef = {  # (1)
    "arn": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListJobsRequestPaginateTypeDef](./type_defs.md#listjobsrequestpaginatetypedef)
## ListNetworkProfilesPaginator

Type annotations and code completion for `#!python session.create_client("devicefarm").get_paginator("list_network_profiles")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/devicefarm/paginator/ListNetworkProfiles.html#DeviceFarm.Paginator.ListNetworkProfiles)

```python
# ListNetworkProfilesPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_devicefarm.paginator import ListNetworkProfilesPaginator

session = get_session()
async with session.create_client("devicefarm") as client:  # (1)
    paginator: ListNetworkProfilesPaginator = client.get_paginator("list_network_profiles")  # (2)
    async for item in paginator.paginate(...):
        item: ListNetworkProfilesResultTypeDef
        print(item)  # (3)
```

1. client: [DeviceFarmClient](./client.md)
2. paginator: [ListNetworkProfilesPaginator](./paginators.md#listnetworkprofilespaginator)
3. item: `AioPageIterator[ListNetworkProfilesResultTypeDef]`


### paginate

Type annotations and code completion for `#!python ListNetworkProfilesPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    arn: str,
    type: NetworkProfileTypeType = ...,  # (1)
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (2)
) -> aiobotocore.paginate.AioPageIterator[ListNetworkProfilesResultTypeDef]:  # (3)
    ...
```

1. See [:material-code-brackets: NetworkProfileTypeType](./literals.md#networkprofiletypetype)
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
3. See `AioPageIterator[ListNetworkProfilesResultTypeDef]`


```python
# paginate method usage example with argument unpacking

kwargs: ListNetworkProfilesRequestPaginateTypeDef = {  # (1)
    "arn": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListNetworkProfilesRequestPaginateTypeDef](./type_defs.md#listnetworkprofilesrequestpaginatetypedef)
## ListOfferingPromotionsPaginator

Type annotations and code completion for `#!python session.create_client("devicefarm").get_paginator("list_offering_promotions")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/devicefarm/paginator/ListOfferingPromotions.html#DeviceFarm.Paginator.ListOfferingPromotions)

```python
# ListOfferingPromotionsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_devicefarm.paginator import ListOfferingPromotionsPaginator

session = get_session()
async with session.create_client("devicefarm") as client:  # (1)
    paginator: ListOfferingPromotionsPaginator = client.get_paginator("list_offering_promotions")  # (2)
    async for item in paginator.paginate(...):
        item: ListOfferingPromotionsResultTypeDef
        print(item)  # (3)
```

1. client: [DeviceFarmClient](./client.md)
2. paginator: [ListOfferingPromotionsPaginator](./paginators.md#listofferingpromotionspaginator)
3. item: `AioPageIterator[ListOfferingPromotionsResultTypeDef]`


### paginate

Type annotations and code completion for `#!python ListOfferingPromotionsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> aiobotocore.paginate.AioPageIterator[ListOfferingPromotionsResultTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
2. See `AioPageIterator[ListOfferingPromotionsResultTypeDef]`


```python
# paginate method usage example with argument unpacking

kwargs: ListOfferingPromotionsRequestPaginateTypeDef = {  # (1)
    "PaginationConfig": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListOfferingPromotionsRequestPaginateTypeDef](./type_defs.md#listofferingpromotionsrequestpaginatetypedef)
## ListOfferingTransactionsPaginator

Type annotations and code completion for `#!python session.create_client("devicefarm").get_paginator("list_offering_transactions")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/devicefarm/paginator/ListOfferingTransactions.html#DeviceFarm.Paginator.ListOfferingTransactions)

```python
# ListOfferingTransactionsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_devicefarm.paginator import ListOfferingTransactionsPaginator

session = get_session()
async with session.create_client("devicefarm") as client:  # (1)
    paginator: ListOfferingTransactionsPaginator = client.get_paginator("list_offering_transactions")  # (2)
    async for item in paginator.paginate(...):
        item: ListOfferingTransactionsResultTypeDef
        print(item)  # (3)
```

1. client: [DeviceFarmClient](./client.md)
2. paginator: [ListOfferingTransactionsPaginator](./paginators.md#listofferingtransactionspaginator)
3. item: `AioPageIterator[ListOfferingTransactionsResultTypeDef]`


### paginate

Type annotations and code completion for `#!python ListOfferingTransactionsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> aiobotocore.paginate.AioPageIterator[ListOfferingTransactionsResultTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
2. See `AioPageIterator[ListOfferingTransactionsResultTypeDef]`


```python
# paginate method usage example with argument unpacking

kwargs: ListOfferingTransactionsRequestPaginateTypeDef = {  # (1)
    "PaginationConfig": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListOfferingTransactionsRequestPaginateTypeDef](./type_defs.md#listofferingtransactionsrequestpaginatetypedef)
## ListOfferingsPaginator

Type annotations and code completion for `#!python session.create_client("devicefarm").get_paginator("list_offerings")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/devicefarm/paginator/ListOfferings.html#DeviceFarm.Paginator.ListOfferings)

```python
# ListOfferingsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_devicefarm.paginator import ListOfferingsPaginator

session = get_session()
async with session.create_client("devicefarm") as client:  # (1)
    paginator: ListOfferingsPaginator = client.get_paginator("list_offerings")  # (2)
    async for item in paginator.paginate(...):
        item: ListOfferingsResultTypeDef
        print(item)  # (3)
```

1. client: [DeviceFarmClient](./client.md)
2. paginator: [ListOfferingsPaginator](./paginators.md#listofferingspaginator)
3. item: `AioPageIterator[ListOfferingsResultTypeDef]`


### paginate

Type annotations and code completion for `#!python ListOfferingsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> aiobotocore.paginate.AioPageIterator[ListOfferingsResultTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
2. See `AioPageIterator[ListOfferingsResultTypeDef]`


```python
# paginate method usage example with argument unpacking

kwargs: ListOfferingsRequestPaginateTypeDef = {  # (1)
    "PaginationConfig": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListOfferingsRequestPaginateTypeDef](./type_defs.md#listofferingsrequestpaginatetypedef)
## ListProjectsPaginator

Type annotations and code completion for `#!python session.create_client("devicefarm").get_paginator("list_projects")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/devicefarm/paginator/ListProjects.html#DeviceFarm.Paginator.ListProjects)

```python
# ListProjectsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_devicefarm.paginator import ListProjectsPaginator

session = get_session()
async with session.create_client("devicefarm") as client:  # (1)
    paginator: ListProjectsPaginator = client.get_paginator("list_projects")  # (2)
    async for item in paginator.paginate(...):
        item: ListProjectsResultTypeDef
        print(item)  # (3)
```

1. client: [DeviceFarmClient](./client.md)
2. paginator: [ListProjectsPaginator](./paginators.md#listprojectspaginator)
3. item: `AioPageIterator[ListProjectsResultTypeDef]`


### paginate

Type annotations and code completion for `#!python ListProjectsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    arn: str = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> aiobotocore.paginate.AioPageIterator[ListProjectsResultTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
2. See `AioPageIterator[ListProjectsResultTypeDef]`


```python
# paginate method usage example with argument unpacking

kwargs: ListProjectsRequestPaginateTypeDef = {  # (1)
    "arn": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListProjectsRequestPaginateTypeDef](./type_defs.md#listprojectsrequestpaginatetypedef)
## ListRemoteAccessSessionsPaginator

Type annotations and code completion for `#!python session.create_client("devicefarm").get_paginator("list_remote_access_sessions")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/devicefarm/paginator/ListRemoteAccessSessions.html#DeviceFarm.Paginator.ListRemoteAccessSessions)

```python
# ListRemoteAccessSessionsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_devicefarm.paginator import ListRemoteAccessSessionsPaginator

session = get_session()
async with session.create_client("devicefarm") as client:  # (1)
    paginator: ListRemoteAccessSessionsPaginator = client.get_paginator("list_remote_access_sessions")  # (2)
    async for item in paginator.paginate(...):
        item: ListRemoteAccessSessionsResultTypeDef
        print(item)  # (3)
```

1. client: [DeviceFarmClient](./client.md)
2. paginator: [ListRemoteAccessSessionsPaginator](./paginators.md#listremoteaccesssessionspaginator)
3. item: `AioPageIterator[ListRemoteAccessSessionsResultTypeDef]`


### paginate

Type annotations and code completion for `#!python ListRemoteAccessSessionsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    arn: str,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> aiobotocore.paginate.AioPageIterator[ListRemoteAccessSessionsResultTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
2. See `AioPageIterator[ListRemoteAccessSessionsResultTypeDef]`


```python
# paginate method usage example with argument unpacking

kwargs: ListRemoteAccessSessionsRequestPaginateTypeDef = {  # (1)
    "arn": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListRemoteAccessSessionsRequestPaginateTypeDef](./type_defs.md#listremoteaccesssessionsrequestpaginatetypedef)
## ListRunsPaginator

Type annotations and code completion for `#!python session.create_client("devicefarm").get_paginator("list_runs")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/devicefarm/paginator/ListRuns.html#DeviceFarm.Paginator.ListRuns)

```python
# ListRunsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_devicefarm.paginator import ListRunsPaginator

session = get_session()
async with session.create_client("devicefarm") as client:  # (1)
    paginator: ListRunsPaginator = client.get_paginator("list_runs")  # (2)
    async for item in paginator.paginate(...):
        item: ListRunsResultTypeDef
        print(item)  # (3)
```

1. client: [DeviceFarmClient](./client.md)
2. paginator: [ListRunsPaginator](./paginators.md#listrunspaginator)
3. item: `AioPageIterator[ListRunsResultTypeDef]`


### paginate

Type annotations and code completion for `#!python ListRunsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    arn: str,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> aiobotocore.paginate.AioPageIterator[ListRunsResultTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
2. See `AioPageIterator[ListRunsResultTypeDef]`


```python
# paginate method usage example with argument unpacking

kwargs: ListRunsRequestPaginateTypeDef = {  # (1)
    "arn": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListRunsRequestPaginateTypeDef](./type_defs.md#listrunsrequestpaginatetypedef)
## ListSamplesPaginator

Type annotations and code completion for `#!python session.create_client("devicefarm").get_paginator("list_samples")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/devicefarm/paginator/ListSamples.html#DeviceFarm.Paginator.ListSamples)

```python
# ListSamplesPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_devicefarm.paginator import ListSamplesPaginator

session = get_session()
async with session.create_client("devicefarm") as client:  # (1)
    paginator: ListSamplesPaginator = client.get_paginator("list_samples")  # (2)
    async for item in paginator.paginate(...):
        item: ListSamplesResultTypeDef
        print(item)  # (3)
```

1. client: [DeviceFarmClient](./client.md)
2. paginator: [ListSamplesPaginator](./paginators.md#listsamplespaginator)
3. item: `AioPageIterator[ListSamplesResultTypeDef]`


### paginate

Type annotations and code completion for `#!python ListSamplesPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    arn: str,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> aiobotocore.paginate.AioPageIterator[ListSamplesResultTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
2. See `AioPageIterator[ListSamplesResultTypeDef]`


```python
# paginate method usage example with argument unpacking

kwargs: ListSamplesRequestPaginateTypeDef = {  # (1)
    "arn": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListSamplesRequestPaginateTypeDef](./type_defs.md#listsamplesrequestpaginatetypedef)
## ListSuitesPaginator

Type annotations and code completion for `#!python session.create_client("devicefarm").get_paginator("list_suites")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/devicefarm/paginator/ListSuites.html#DeviceFarm.Paginator.ListSuites)

```python
# ListSuitesPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_devicefarm.paginator import ListSuitesPaginator

session = get_session()
async with session.create_client("devicefarm") as client:  # (1)
    paginator: ListSuitesPaginator = client.get_paginator("list_suites")  # (2)
    async for item in paginator.paginate(...):
        item: ListSuitesResultTypeDef
        print(item)  # (3)
```

1. client: [DeviceFarmClient](./client.md)
2. paginator: [ListSuitesPaginator](./paginators.md#listsuitespaginator)
3. item: `AioPageIterator[ListSuitesResultTypeDef]`


### paginate

Type annotations and code completion for `#!python ListSuitesPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    arn: str,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> aiobotocore.paginate.AioPageIterator[ListSuitesResultTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
2. See `AioPageIterator[ListSuitesResultTypeDef]`


```python
# paginate method usage example with argument unpacking

kwargs: ListSuitesRequestPaginateTypeDef = {  # (1)
    "arn": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListSuitesRequestPaginateTypeDef](./type_defs.md#listsuitesrequestpaginatetypedef)
## ListTestsPaginator

Type annotations and code completion for `#!python session.create_client("devicefarm").get_paginator("list_tests")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/devicefarm/paginator/ListTests.html#DeviceFarm.Paginator.ListTests)

```python
# ListTestsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_devicefarm.paginator import ListTestsPaginator

session = get_session()
async with session.create_client("devicefarm") as client:  # (1)
    paginator: ListTestsPaginator = client.get_paginator("list_tests")  # (2)
    async for item in paginator.paginate(...):
        item: ListTestsResultTypeDef
        print(item)  # (3)
```

1. client: [DeviceFarmClient](./client.md)
2. paginator: [ListTestsPaginator](./paginators.md#listtestspaginator)
3. item: `AioPageIterator[ListTestsResultTypeDef]`


### paginate

Type annotations and code completion for `#!python ListTestsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    arn: str,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> aiobotocore.paginate.AioPageIterator[ListTestsResultTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
2. See `AioPageIterator[ListTestsResultTypeDef]`


```python
# paginate method usage example with argument unpacking

kwargs: ListTestsRequestPaginateTypeDef = {  # (1)
    "arn": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListTestsRequestPaginateTypeDef](./type_defs.md#listtestsrequestpaginatetypedef)
## ListUniqueProblemsPaginator

Type annotations and code completion for `#!python session.create_client("devicefarm").get_paginator("list_unique_problems")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/devicefarm/paginator/ListUniqueProblems.html#DeviceFarm.Paginator.ListUniqueProblems)

```python
# ListUniqueProblemsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_devicefarm.paginator import ListUniqueProblemsPaginator

session = get_session()
async with session.create_client("devicefarm") as client:  # (1)
    paginator: ListUniqueProblemsPaginator = client.get_paginator("list_unique_problems")  # (2)
    async for item in paginator.paginate(...):
        item: ListUniqueProblemsResultTypeDef
        print(item)  # (3)
```

1. client: [DeviceFarmClient](./client.md)
2. paginator: [ListUniqueProblemsPaginator](./paginators.md#listuniqueproblemspaginator)
3. item: `AioPageIterator[ListUniqueProblemsResultTypeDef]`


### paginate

Type annotations and code completion for `#!python ListUniqueProblemsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    arn: str,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> aiobotocore.paginate.AioPageIterator[ListUniqueProblemsResultTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
2. See `AioPageIterator[ListUniqueProblemsResultTypeDef]`


```python
# paginate method usage example with argument unpacking

kwargs: ListUniqueProblemsRequestPaginateTypeDef = {  # (1)
    "arn": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListUniqueProblemsRequestPaginateTypeDef](./type_defs.md#listuniqueproblemsrequestpaginatetypedef)
## ListUploadsPaginator

Type annotations and code completion for `#!python session.create_client("devicefarm").get_paginator("list_uploads")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/devicefarm/paginator/ListUploads.html#DeviceFarm.Paginator.ListUploads)

```python
# ListUploadsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_devicefarm.paginator import ListUploadsPaginator

session = get_session()
async with session.create_client("devicefarm") as client:  # (1)
    paginator: ListUploadsPaginator = client.get_paginator("list_uploads")  # (2)
    async for item in paginator.paginate(...):
        item: ListUploadsResultTypeDef
        print(item)  # (3)
```

1. client: [DeviceFarmClient](./client.md)
2. paginator: [ListUploadsPaginator](./paginators.md#listuploadspaginator)
3. item: `AioPageIterator[ListUploadsResultTypeDef]`


### paginate

Type annotations and code completion for `#!python ListUploadsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    arn: str,
    type: UploadTypeType = ...,  # (1)
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (2)
) -> aiobotocore.paginate.AioPageIterator[ListUploadsResultTypeDef]:  # (3)
    ...
```

1. See [:material-code-brackets: UploadTypeType](./literals.md#uploadtypetype)
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
3. See `AioPageIterator[ListUploadsResultTypeDef]`


```python
# paginate method usage example with argument unpacking

kwargs: ListUploadsRequestPaginateTypeDef = {  # (1)
    "arn": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListUploadsRequestPaginateTypeDef](./type_defs.md#listuploadsrequestpaginatetypedef)
## ListVPCEConfigurationsPaginator

Type annotations and code completion for `#!python session.create_client("devicefarm").get_paginator("list_vpce_configurations")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/devicefarm/paginator/ListVPCEConfigurations.html#DeviceFarm.Paginator.ListVPCEConfigurations)

```python
# ListVPCEConfigurationsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_devicefarm.paginator import ListVPCEConfigurationsPaginator

session = get_session()
async with session.create_client("devicefarm") as client:  # (1)
    paginator: ListVPCEConfigurationsPaginator = client.get_paginator("list_vpce_configurations")  # (2)
    async for item in paginator.paginate(...):
        item: ListVPCEConfigurationsResultTypeDef
        print(item)  # (3)
```

1. client: [DeviceFarmClient](./client.md)
2. paginator: [ListVPCEConfigurationsPaginator](./paginators.md#listvpceconfigurationspaginator)
3. item: `AioPageIterator[ListVPCEConfigurationsResultTypeDef]`


### paginate

Type annotations and code completion for `#!python ListVPCEConfigurationsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> aiobotocore.paginate.AioPageIterator[ListVPCEConfigurationsResultTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
2. See `AioPageIterator[ListVPCEConfigurationsResultTypeDef]`


```python
# paginate method usage example with argument unpacking

kwargs: ListVPCEConfigurationsRequestPaginateTypeDef = {  # (1)
    "PaginationConfig": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListVPCEConfigurationsRequestPaginateTypeDef](./type_defs.md#listvpceconfigurationsrequestpaginatetypedef)
