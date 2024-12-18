# Waiters

> [Index](../README.md) > [DeadlineCloud](./README.md) > Waiters

!!! note ""

    Auto-generated documentation for [DeadlineCloud](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/deadline.html#deadlinecloud)
    type annotations stubs module [types-aiobotocore-deadline](https://pypi.org/project/types-aiobotocore-deadline/).

## FleetActiveWaiter

Type annotations and code completion for `#!python session.create_client("deadline").get_waiter("fleet_active")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/deadline/waiter/FleetActive.html#DeadlineCloud.Waiter.FleetActive)

```python
# FleetActiveWaiter usage example

from aiobotocore.session import Session

from types_aiobotocore_deadline.waiter import FleetActiveWaiter

session = get_session()
async with session.create_client("deadline") as client:  # (1)
    waiter: FleetActiveWaiter = client.get_waiter("fleet_active")  # (2)
    await waiter.wait()
```

1. client: [DeadlineCloudClient](./client.md)
2. waiter: [FleetActiveWaiter](./waiters.md#fleetactivewaiter)


### wait

Type annotations and code completion for `#!python FleetActiveWaiter.wait` method.

```python
# wait method definition

await def wait(
    self,
    *,
    farmId: str,
    fleetId: str,
    WaiterConfig: WaiterConfigTypeDef = ...,  # (1)
) -> None:
    ...
```

1. See [:material-code-braces: WaiterConfigTypeDef](./type_defs.md#waiterconfigtypedef) 


```python
# wait method usage example with argument unpacking

kwargs: GetFleetRequestFleetActiveWaitTypeDef = {  # (1)
    "farmId": ...,
    "fleetId": ...,
}

parent.wait(**kwargs)
```

1. See [:material-code-braces: GetFleetRequestFleetActiveWaitTypeDef](./type_defs.md#getfleetrequestfleetactivewaittypedef) 
## JobCreateCompleteWaiter

Type annotations and code completion for `#!python session.create_client("deadline").get_waiter("job_create_complete")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/deadline/waiter/JobCreateComplete.html#DeadlineCloud.Waiter.JobCreateComplete)

```python
# JobCreateCompleteWaiter usage example

from aiobotocore.session import Session

from types_aiobotocore_deadline.waiter import JobCreateCompleteWaiter

session = get_session()
async with session.create_client("deadline") as client:  # (1)
    waiter: JobCreateCompleteWaiter = client.get_waiter("job_create_complete")  # (2)
    await waiter.wait()
```

1. client: [DeadlineCloudClient](./client.md)
2. waiter: [JobCreateCompleteWaiter](./waiters.md#jobcreatecompletewaiter)


### wait

Type annotations and code completion for `#!python JobCreateCompleteWaiter.wait` method.

```python
# wait method definition

await def wait(
    self,
    *,
    farmId: str,
    jobId: str,
    queueId: str,
    WaiterConfig: WaiterConfigTypeDef = ...,  # (1)
) -> None:
    ...
```

1. See [:material-code-braces: WaiterConfigTypeDef](./type_defs.md#waiterconfigtypedef) 


```python
# wait method usage example with argument unpacking

kwargs: GetJobRequestJobCreateCompleteWaitTypeDef = {  # (1)
    "farmId": ...,
    "jobId": ...,
    "queueId": ...,
}

parent.wait(**kwargs)
```

1. See [:material-code-braces: GetJobRequestJobCreateCompleteWaitTypeDef](./type_defs.md#getjobrequestjobcreatecompletewaittypedef) 
## LicenseEndpointDeletedWaiter

Type annotations and code completion for `#!python session.create_client("deadline").get_waiter("license_endpoint_deleted")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/deadline/waiter/LicenseEndpointDeleted.html#DeadlineCloud.Waiter.LicenseEndpointDeleted)

```python
# LicenseEndpointDeletedWaiter usage example

from aiobotocore.session import Session

from types_aiobotocore_deadline.waiter import LicenseEndpointDeletedWaiter

session = get_session()
async with session.create_client("deadline") as client:  # (1)
    waiter: LicenseEndpointDeletedWaiter = client.get_waiter("license_endpoint_deleted")  # (2)
    await waiter.wait()
```

1. client: [DeadlineCloudClient](./client.md)
2. waiter: [LicenseEndpointDeletedWaiter](./waiters.md#licenseendpointdeletedwaiter)


### wait

Type annotations and code completion for `#!python LicenseEndpointDeletedWaiter.wait` method.

```python
# wait method definition

await def wait(
    self,
    *,
    licenseEndpointId: str,
    WaiterConfig: WaiterConfigTypeDef = ...,  # (1)
) -> None:
    ...
```

1. See [:material-code-braces: WaiterConfigTypeDef](./type_defs.md#waiterconfigtypedef) 


```python
# wait method usage example with argument unpacking

kwargs: GetLicenseEndpointRequestLicenseEndpointDeletedWaitTypeDef = {  # (1)
    "licenseEndpointId": ...,
}

parent.wait(**kwargs)
```

1. See [:material-code-braces: GetLicenseEndpointRequestLicenseEndpointDeletedWaitTypeDef](./type_defs.md#getlicenseendpointrequestlicenseendpointdeletedwaittypedef) 
## LicenseEndpointValidWaiter

Type annotations and code completion for `#!python session.create_client("deadline").get_waiter("license_endpoint_valid")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/deadline/waiter/LicenseEndpointValid.html#DeadlineCloud.Waiter.LicenseEndpointValid)

```python
# LicenseEndpointValidWaiter usage example

from aiobotocore.session import Session

from types_aiobotocore_deadline.waiter import LicenseEndpointValidWaiter

session = get_session()
async with session.create_client("deadline") as client:  # (1)
    waiter: LicenseEndpointValidWaiter = client.get_waiter("license_endpoint_valid")  # (2)
    await waiter.wait()
```

1. client: [DeadlineCloudClient](./client.md)
2. waiter: [LicenseEndpointValidWaiter](./waiters.md#licenseendpointvalidwaiter)


### wait

Type annotations and code completion for `#!python LicenseEndpointValidWaiter.wait` method.

```python
# wait method definition

await def wait(
    self,
    *,
    licenseEndpointId: str,
    WaiterConfig: WaiterConfigTypeDef = ...,  # (1)
) -> None:
    ...
```

1. See [:material-code-braces: WaiterConfigTypeDef](./type_defs.md#waiterconfigtypedef) 


```python
# wait method usage example with argument unpacking

kwargs: GetLicenseEndpointRequestLicenseEndpointValidWaitTypeDef = {  # (1)
    "licenseEndpointId": ...,
}

parent.wait(**kwargs)
```

1. See [:material-code-braces: GetLicenseEndpointRequestLicenseEndpointValidWaitTypeDef](./type_defs.md#getlicenseendpointrequestlicenseendpointvalidwaittypedef) 
## QueueFleetAssociationStoppedWaiter

Type annotations and code completion for `#!python session.create_client("deadline").get_waiter("queue_fleet_association_stopped")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/deadline/waiter/QueueFleetAssociationStopped.html#DeadlineCloud.Waiter.QueueFleetAssociationStopped)

```python
# QueueFleetAssociationStoppedWaiter usage example

from aiobotocore.session import Session

from types_aiobotocore_deadline.waiter import QueueFleetAssociationStoppedWaiter

session = get_session()
async with session.create_client("deadline") as client:  # (1)
    waiter: QueueFleetAssociationStoppedWaiter = client.get_waiter("queue_fleet_association_stopped")  # (2)
    await waiter.wait()
```

1. client: [DeadlineCloudClient](./client.md)
2. waiter: [QueueFleetAssociationStoppedWaiter](./waiters.md#queuefleetassociationstoppedwaiter)


### wait

Type annotations and code completion for `#!python QueueFleetAssociationStoppedWaiter.wait` method.

```python
# wait method definition

await def wait(
    self,
    *,
    farmId: str,
    queueId: str,
    fleetId: str,
    WaiterConfig: WaiterConfigTypeDef = ...,  # (1)
) -> None:
    ...
```

1. See [:material-code-braces: WaiterConfigTypeDef](./type_defs.md#waiterconfigtypedef) 


```python
# wait method usage example with argument unpacking

kwargs: GetQueueFleetAssociationRequestQueueFleetAssociationStoppedWaitTypeDef = {  # (1)
    "farmId": ...,
    "queueId": ...,
    "fleetId": ...,
}

parent.wait(**kwargs)
```

1. See [:material-code-braces: GetQueueFleetAssociationRequestQueueFleetAssociationStoppedWaitTypeDef](./type_defs.md#getqueuefleetassociationrequestqueuefleetassociationstoppedwaittypedef) 
## QueueSchedulingBlockedWaiter

Type annotations and code completion for `#!python session.create_client("deadline").get_waiter("queue_scheduling_blocked")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/deadline/waiter/QueueSchedulingBlocked.html#DeadlineCloud.Waiter.QueueSchedulingBlocked)

```python
# QueueSchedulingBlockedWaiter usage example

from aiobotocore.session import Session

from types_aiobotocore_deadline.waiter import QueueSchedulingBlockedWaiter

session = get_session()
async with session.create_client("deadline") as client:  # (1)
    waiter: QueueSchedulingBlockedWaiter = client.get_waiter("queue_scheduling_blocked")  # (2)
    await waiter.wait()
```

1. client: [DeadlineCloudClient](./client.md)
2. waiter: [QueueSchedulingBlockedWaiter](./waiters.md#queueschedulingblockedwaiter)


### wait

Type annotations and code completion for `#!python QueueSchedulingBlockedWaiter.wait` method.

```python
# wait method definition

await def wait(
    self,
    *,
    farmId: str,
    queueId: str,
    WaiterConfig: WaiterConfigTypeDef = ...,  # (1)
) -> None:
    ...
```

1. See [:material-code-braces: WaiterConfigTypeDef](./type_defs.md#waiterconfigtypedef) 


```python
# wait method usage example with argument unpacking

kwargs: GetQueueRequestQueueSchedulingBlockedWaitTypeDef = {  # (1)
    "farmId": ...,
    "queueId": ...,
}

parent.wait(**kwargs)
```

1. See [:material-code-braces: GetQueueRequestQueueSchedulingBlockedWaitTypeDef](./type_defs.md#getqueuerequestqueueschedulingblockedwaittypedef) 
## QueueSchedulingWaiter

Type annotations and code completion for `#!python session.create_client("deadline").get_waiter("queue_scheduling")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/deadline/waiter/QueueScheduling.html#DeadlineCloud.Waiter.QueueScheduling)

```python
# QueueSchedulingWaiter usage example

from aiobotocore.session import Session

from types_aiobotocore_deadline.waiter import QueueSchedulingWaiter

session = get_session()
async with session.create_client("deadline") as client:  # (1)
    waiter: QueueSchedulingWaiter = client.get_waiter("queue_scheduling")  # (2)
    await waiter.wait()
```

1. client: [DeadlineCloudClient](./client.md)
2. waiter: [QueueSchedulingWaiter](./waiters.md#queueschedulingwaiter)


### wait

Type annotations and code completion for `#!python QueueSchedulingWaiter.wait` method.

```python
# wait method definition

await def wait(
    self,
    *,
    farmId: str,
    queueId: str,
    WaiterConfig: WaiterConfigTypeDef = ...,  # (1)
) -> None:
    ...
```

1. See [:material-code-braces: WaiterConfigTypeDef](./type_defs.md#waiterconfigtypedef) 


```python
# wait method usage example with argument unpacking

kwargs: GetQueueRequestQueueSchedulingWaitTypeDef = {  # (1)
    "farmId": ...,
    "queueId": ...,
}

parent.wait(**kwargs)
```

1. See [:material-code-braces: GetQueueRequestQueueSchedulingWaitTypeDef](./type_defs.md#getqueuerequestqueueschedulingwaittypedef) 
