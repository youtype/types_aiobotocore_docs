# Waiters

> [Index](../README.md) > [EC2](./README.md) > Waiters

!!! note ""

    Auto-generated documentation for [EC2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ec2.html#ec2)
    type annotations stubs module [types-aiobotocore-ec2](https://pypi.org/project/types-aiobotocore-ec2/).

## BundleTaskCompleteWaiter

Type annotations and code completion for `#!python session.create_client("ec2").get_waiter("bundle_task_complete")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ec2/waiter/BundleTaskComplete.html#EC2.Waiter.BundleTaskComplete)

```python
# BundleTaskCompleteWaiter usage example

from aiobotocore.session import Session

from types_aiobotocore_ec2.waiter import BundleTaskCompleteWaiter

session = get_session()
async with session.create_client("ec2") as client:  # (1)
    waiter: BundleTaskCompleteWaiter = client.get_waiter("bundle_task_complete")  # (2)
    await waiter.wait()
```

1. client: [EC2Client](./client.md)
2. waiter: [BundleTaskCompleteWaiter](./waiters.md#bundletaskcompletewaiter)


### wait

Type annotations and code completion for `#!python BundleTaskCompleteWaiter.wait` method.

```python
# wait method definition

await def wait(
    self,
    *,
    BundleIds: Sequence[str] = ...,
    DryRun: bool = ...,
    Filters: Sequence[FilterTypeDef] = ...,  # (1)
    WaiterConfig: WaiterConfigTypeDef = ...,  # (2)
) -> None:
    ...
```

1. See [:material-code-braces: FilterTypeDef](./type_defs.md#filtertypedef) 
2. See [:material-code-braces: WaiterConfigTypeDef](./type_defs.md#waiterconfigtypedef) 


```python
# wait method usage example with argument unpacking

kwargs: DescribeBundleTasksRequestWaitTypeDef = {  # (1)
    "BundleIds": ...,
}

parent.wait(**kwargs)
```

1. See [:material-code-braces: DescribeBundleTasksRequestWaitTypeDef](./type_defs.md#describebundletasksrequestwaittypedef) 
## ConversionTaskCancelledWaiter

Type annotations and code completion for `#!python session.create_client("ec2").get_waiter("conversion_task_cancelled")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ec2/waiter/ConversionTaskCancelled.html#EC2.Waiter.ConversionTaskCancelled)

```python
# ConversionTaskCancelledWaiter usage example

from aiobotocore.session import Session

from types_aiobotocore_ec2.waiter import ConversionTaskCancelledWaiter

session = get_session()
async with session.create_client("ec2") as client:  # (1)
    waiter: ConversionTaskCancelledWaiter = client.get_waiter("conversion_task_cancelled")  # (2)
    await waiter.wait()
```

1. client: [EC2Client](./client.md)
2. waiter: [ConversionTaskCancelledWaiter](./waiters.md#conversiontaskcancelledwaiter)


### wait

Type annotations and code completion for `#!python ConversionTaskCancelledWaiter.wait` method.

```python
# wait method definition

await def wait(
    self,
    *,
    DryRun: bool = ...,
    ConversionTaskIds: Sequence[str] = ...,
    WaiterConfig: WaiterConfigTypeDef = ...,  # (1)
) -> None:
    ...
```

1. See [:material-code-braces: WaiterConfigTypeDef](./type_defs.md#waiterconfigtypedef) 


```python
# wait method usage example with argument unpacking

kwargs: DescribeConversionTasksRequestWaitTypeDef = {  # (1)
    "DryRun": ...,
}

parent.wait(**kwargs)
```

1. See [:material-code-braces: DescribeConversionTasksRequestWaitTypeDef](./type_defs.md#describeconversiontasksrequestwaittypedef) 
## ConversionTaskCompletedWaiter

Type annotations and code completion for `#!python session.create_client("ec2").get_waiter("conversion_task_completed")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ec2/waiter/ConversionTaskCompleted.html#EC2.Waiter.ConversionTaskCompleted)

```python
# ConversionTaskCompletedWaiter usage example

from aiobotocore.session import Session

from types_aiobotocore_ec2.waiter import ConversionTaskCompletedWaiter

session = get_session()
async with session.create_client("ec2") as client:  # (1)
    waiter: ConversionTaskCompletedWaiter = client.get_waiter("conversion_task_completed")  # (2)
    await waiter.wait()
```

1. client: [EC2Client](./client.md)
2. waiter: [ConversionTaskCompletedWaiter](./waiters.md#conversiontaskcompletedwaiter)


### wait

Type annotations and code completion for `#!python ConversionTaskCompletedWaiter.wait` method.

```python
# wait method definition

await def wait(
    self,
    *,
    DryRun: bool = ...,
    ConversionTaskIds: Sequence[str] = ...,
    WaiterConfig: WaiterConfigTypeDef = ...,  # (1)
) -> None:
    ...
```

1. See [:material-code-braces: WaiterConfigTypeDef](./type_defs.md#waiterconfigtypedef) 


```python
# wait method usage example with argument unpacking

kwargs: DescribeConversionTasksRequestWaitExtraTypeDef = {  # (1)
    "DryRun": ...,
}

parent.wait(**kwargs)
```

1. See [:material-code-braces: DescribeConversionTasksRequestWaitExtraTypeDef](./type_defs.md#describeconversiontasksrequestwaitextratypedef) 
## ConversionTaskDeletedWaiter

Type annotations and code completion for `#!python session.create_client("ec2").get_waiter("conversion_task_deleted")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ec2/waiter/ConversionTaskDeleted.html#EC2.Waiter.ConversionTaskDeleted)

```python
# ConversionTaskDeletedWaiter usage example

from aiobotocore.session import Session

from types_aiobotocore_ec2.waiter import ConversionTaskDeletedWaiter

session = get_session()
async with session.create_client("ec2") as client:  # (1)
    waiter: ConversionTaskDeletedWaiter = client.get_waiter("conversion_task_deleted")  # (2)
    await waiter.wait()
```

1. client: [EC2Client](./client.md)
2. waiter: [ConversionTaskDeletedWaiter](./waiters.md#conversiontaskdeletedwaiter)


### wait

Type annotations and code completion for `#!python ConversionTaskDeletedWaiter.wait` method.

```python
# wait method definition

await def wait(
    self,
    *,
    DryRun: bool = ...,
    ConversionTaskIds: Sequence[str] = ...,
    WaiterConfig: WaiterConfigTypeDef = ...,  # (1)
) -> None:
    ...
```

1. See [:material-code-braces: WaiterConfigTypeDef](./type_defs.md#waiterconfigtypedef) 


```python
# wait method usage example with argument unpacking

kwargs: DescribeConversionTasksRequestWaitExtraExtraTypeDef = {  # (1)
    "DryRun": ...,
}

parent.wait(**kwargs)
```

1. See [:material-code-braces: DescribeConversionTasksRequestWaitExtraExtraTypeDef](./type_defs.md#describeconversiontasksrequestwaitextraextratypedef) 
## CustomerGatewayAvailableWaiter

Type annotations and code completion for `#!python session.create_client("ec2").get_waiter("customer_gateway_available")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ec2/waiter/CustomerGatewayAvailable.html#EC2.Waiter.CustomerGatewayAvailable)

```python
# CustomerGatewayAvailableWaiter usage example

from aiobotocore.session import Session

from types_aiobotocore_ec2.waiter import CustomerGatewayAvailableWaiter

session = get_session()
async with session.create_client("ec2") as client:  # (1)
    waiter: CustomerGatewayAvailableWaiter = client.get_waiter("customer_gateway_available")  # (2)
    await waiter.wait()
```

1. client: [EC2Client](./client.md)
2. waiter: [CustomerGatewayAvailableWaiter](./waiters.md#customergatewayavailablewaiter)


### wait

Type annotations and code completion for `#!python CustomerGatewayAvailableWaiter.wait` method.

```python
# wait method definition

await def wait(
    self,
    *,
    CustomerGatewayIds: Sequence[str] = ...,
    Filters: Sequence[FilterTypeDef] = ...,  # (1)
    DryRun: bool = ...,
    WaiterConfig: WaiterConfigTypeDef = ...,  # (2)
) -> None:
    ...
```

1. See [:material-code-braces: FilterTypeDef](./type_defs.md#filtertypedef) 
2. See [:material-code-braces: WaiterConfigTypeDef](./type_defs.md#waiterconfigtypedef) 


```python
# wait method usage example with argument unpacking

kwargs: DescribeCustomerGatewaysRequestWaitTypeDef = {  # (1)
    "CustomerGatewayIds": ...,
}

parent.wait(**kwargs)
```

1. See [:material-code-braces: DescribeCustomerGatewaysRequestWaitTypeDef](./type_defs.md#describecustomergatewaysrequestwaittypedef) 
## ExportTaskCancelledWaiter

Type annotations and code completion for `#!python session.create_client("ec2").get_waiter("export_task_cancelled")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ec2/waiter/ExportTaskCancelled.html#EC2.Waiter.ExportTaskCancelled)

```python
# ExportTaskCancelledWaiter usage example

from aiobotocore.session import Session

from types_aiobotocore_ec2.waiter import ExportTaskCancelledWaiter

session = get_session()
async with session.create_client("ec2") as client:  # (1)
    waiter: ExportTaskCancelledWaiter = client.get_waiter("export_task_cancelled")  # (2)
    await waiter.wait()
```

1. client: [EC2Client](./client.md)
2. waiter: [ExportTaskCancelledWaiter](./waiters.md#exporttaskcancelledwaiter)


### wait

Type annotations and code completion for `#!python ExportTaskCancelledWaiter.wait` method.

```python
# wait method definition

await def wait(
    self,
    *,
    Filters: Sequence[FilterTypeDef] = ...,  # (1)
    ExportTaskIds: Sequence[str] = ...,
    WaiterConfig: WaiterConfigTypeDef = ...,  # (2)
) -> None:
    ...
```

1. See [:material-code-braces: FilterTypeDef](./type_defs.md#filtertypedef) 
2. See [:material-code-braces: WaiterConfigTypeDef](./type_defs.md#waiterconfigtypedef) 


```python
# wait method usage example with argument unpacking

kwargs: DescribeExportTasksRequestWaitTypeDef = {  # (1)
    "Filters": ...,
}

parent.wait(**kwargs)
```

1. See [:material-code-braces: DescribeExportTasksRequestWaitTypeDef](./type_defs.md#describeexporttasksrequestwaittypedef) 
## ExportTaskCompletedWaiter

Type annotations and code completion for `#!python session.create_client("ec2").get_waiter("export_task_completed")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ec2/waiter/ExportTaskCompleted.html#EC2.Waiter.ExportTaskCompleted)

```python
# ExportTaskCompletedWaiter usage example

from aiobotocore.session import Session

from types_aiobotocore_ec2.waiter import ExportTaskCompletedWaiter

session = get_session()
async with session.create_client("ec2") as client:  # (1)
    waiter: ExportTaskCompletedWaiter = client.get_waiter("export_task_completed")  # (2)
    await waiter.wait()
```

1. client: [EC2Client](./client.md)
2. waiter: [ExportTaskCompletedWaiter](./waiters.md#exporttaskcompletedwaiter)


### wait

Type annotations and code completion for `#!python ExportTaskCompletedWaiter.wait` method.

```python
# wait method definition

await def wait(
    self,
    *,
    Filters: Sequence[FilterTypeDef] = ...,  # (1)
    ExportTaskIds: Sequence[str] = ...,
    WaiterConfig: WaiterConfigTypeDef = ...,  # (2)
) -> None:
    ...
```

1. See [:material-code-braces: FilterTypeDef](./type_defs.md#filtertypedef) 
2. See [:material-code-braces: WaiterConfigTypeDef](./type_defs.md#waiterconfigtypedef) 


```python
# wait method usage example with argument unpacking

kwargs: DescribeExportTasksRequestWaitExtraTypeDef = {  # (1)
    "Filters": ...,
}

parent.wait(**kwargs)
```

1. See [:material-code-braces: DescribeExportTasksRequestWaitExtraTypeDef](./type_defs.md#describeexporttasksrequestwaitextratypedef) 
## ImageAvailableWaiter

Type annotations and code completion for `#!python session.create_client("ec2").get_waiter("image_available")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ec2/waiter/ImageAvailable.html#EC2.Waiter.ImageAvailable)

```python
# ImageAvailableWaiter usage example

from aiobotocore.session import Session

from types_aiobotocore_ec2.waiter import ImageAvailableWaiter

session = get_session()
async with session.create_client("ec2") as client:  # (1)
    waiter: ImageAvailableWaiter = client.get_waiter("image_available")  # (2)
    await waiter.wait()
```

1. client: [EC2Client](./client.md)
2. waiter: [ImageAvailableWaiter](./waiters.md#imageavailablewaiter)


### wait

Type annotations and code completion for `#!python ImageAvailableWaiter.wait` method.

```python
# wait method definition

await def wait(
    self,
    *,
    ExecutableUsers: Sequence[str] = ...,
    ImageIds: Sequence[str] = ...,
    Owners: Sequence[str] = ...,
    IncludeDeprecated: bool = ...,
    IncludeDisabled: bool = ...,
    MaxResults: int = ...,
    NextToken: str = ...,
    DryRun: bool = ...,
    Filters: Sequence[FilterTypeDef] = ...,  # (1)
    WaiterConfig: WaiterConfigTypeDef = ...,  # (2)
) -> None:
    ...
```

1. See [:material-code-braces: FilterTypeDef](./type_defs.md#filtertypedef) 
2. See [:material-code-braces: WaiterConfigTypeDef](./type_defs.md#waiterconfigtypedef) 


```python
# wait method usage example with argument unpacking

kwargs: DescribeImagesRequestWaitExtraTypeDef = {  # (1)
    "ExecutableUsers": ...,
}

parent.wait(**kwargs)
```

1. See [:material-code-braces: DescribeImagesRequestWaitExtraTypeDef](./type_defs.md#describeimagesrequestwaitextratypedef) 
## ImageExistsWaiter

Type annotations and code completion for `#!python session.create_client("ec2").get_waiter("image_exists")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ec2/waiter/ImageExists.html#EC2.Waiter.ImageExists)

```python
# ImageExistsWaiter usage example

from aiobotocore.session import Session

from types_aiobotocore_ec2.waiter import ImageExistsWaiter

session = get_session()
async with session.create_client("ec2") as client:  # (1)
    waiter: ImageExistsWaiter = client.get_waiter("image_exists")  # (2)
    await waiter.wait()
```

1. client: [EC2Client](./client.md)
2. waiter: [ImageExistsWaiter](./waiters.md#imageexistswaiter)


### wait

Type annotations and code completion for `#!python ImageExistsWaiter.wait` method.

```python
# wait method definition

await def wait(
    self,
    *,
    ExecutableUsers: Sequence[str] = ...,
    ImageIds: Sequence[str] = ...,
    Owners: Sequence[str] = ...,
    IncludeDeprecated: bool = ...,
    IncludeDisabled: bool = ...,
    MaxResults: int = ...,
    NextToken: str = ...,
    DryRun: bool = ...,
    Filters: Sequence[FilterTypeDef] = ...,  # (1)
    WaiterConfig: WaiterConfigTypeDef = ...,  # (2)
) -> None:
    ...
```

1. See [:material-code-braces: FilterTypeDef](./type_defs.md#filtertypedef) 
2. See [:material-code-braces: WaiterConfigTypeDef](./type_defs.md#waiterconfigtypedef) 


```python
# wait method usage example with argument unpacking

kwargs: DescribeImagesRequestWaitTypeDef = {  # (1)
    "ExecutableUsers": ...,
}

parent.wait(**kwargs)
```

1. See [:material-code-braces: DescribeImagesRequestWaitTypeDef](./type_defs.md#describeimagesrequestwaittypedef) 
## InstanceExistsWaiter

Type annotations and code completion for `#!python session.create_client("ec2").get_waiter("instance_exists")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ec2/waiter/InstanceExists.html#EC2.Waiter.InstanceExists)

```python
# InstanceExistsWaiter usage example

from aiobotocore.session import Session

from types_aiobotocore_ec2.waiter import InstanceExistsWaiter

session = get_session()
async with session.create_client("ec2") as client:  # (1)
    waiter: InstanceExistsWaiter = client.get_waiter("instance_exists")  # (2)
    await waiter.wait()
```

1. client: [EC2Client](./client.md)
2. waiter: [InstanceExistsWaiter](./waiters.md#instanceexistswaiter)


### wait

Type annotations and code completion for `#!python InstanceExistsWaiter.wait` method.

```python
# wait method definition

await def wait(
    self,
    *,
    InstanceIds: Sequence[str] = ...,
    DryRun: bool = ...,
    Filters: Sequence[FilterTypeDef] = ...,  # (1)
    NextToken: str = ...,
    MaxResults: int = ...,
    WaiterConfig: WaiterConfigTypeDef = ...,  # (2)
) -> None:
    ...
```

1. See [:material-code-braces: FilterTypeDef](./type_defs.md#filtertypedef) 
2. See [:material-code-braces: WaiterConfigTypeDef](./type_defs.md#waiterconfigtypedef) 


```python
# wait method usage example with argument unpacking

kwargs: DescribeInstancesRequestWaitTypeDef = {  # (1)
    "InstanceIds": ...,
}

parent.wait(**kwargs)
```

1. See [:material-code-braces: DescribeInstancesRequestWaitTypeDef](./type_defs.md#describeinstancesrequestwaittypedef) 
## InstanceRunningWaiter

Type annotations and code completion for `#!python session.create_client("ec2").get_waiter("instance_running")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ec2/waiter/InstanceRunning.html#EC2.Waiter.InstanceRunning)

```python
# InstanceRunningWaiter usage example

from aiobotocore.session import Session

from types_aiobotocore_ec2.waiter import InstanceRunningWaiter

session = get_session()
async with session.create_client("ec2") as client:  # (1)
    waiter: InstanceRunningWaiter = client.get_waiter("instance_running")  # (2)
    await waiter.wait()
```

1. client: [EC2Client](./client.md)
2. waiter: [InstanceRunningWaiter](./waiters.md#instancerunningwaiter)


### wait

Type annotations and code completion for `#!python InstanceRunningWaiter.wait` method.

```python
# wait method definition

await def wait(
    self,
    *,
    InstanceIds: Sequence[str] = ...,
    DryRun: bool = ...,
    Filters: Sequence[FilterTypeDef] = ...,  # (1)
    NextToken: str = ...,
    MaxResults: int = ...,
    WaiterConfig: WaiterConfigTypeDef = ...,  # (2)
) -> None:
    ...
```

1. See [:material-code-braces: FilterTypeDef](./type_defs.md#filtertypedef) 
2. See [:material-code-braces: WaiterConfigTypeDef](./type_defs.md#waiterconfigtypedef) 


```python
# wait method usage example with argument unpacking

kwargs: DescribeInstancesRequestWaitExtraTypeDef = {  # (1)
    "InstanceIds": ...,
}

parent.wait(**kwargs)
```

1. See [:material-code-braces: DescribeInstancesRequestWaitExtraTypeDef](./type_defs.md#describeinstancesrequestwaitextratypedef) 
## InstanceStatusOkWaiter

Type annotations and code completion for `#!python session.create_client("ec2").get_waiter("instance_status_ok")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ec2/waiter/InstanceStatusOk.html#EC2.Waiter.InstanceStatusOk)

```python
# InstanceStatusOkWaiter usage example

from aiobotocore.session import Session

from types_aiobotocore_ec2.waiter import InstanceStatusOkWaiter

session = get_session()
async with session.create_client("ec2") as client:  # (1)
    waiter: InstanceStatusOkWaiter = client.get_waiter("instance_status_ok")  # (2)
    await waiter.wait()
```

1. client: [EC2Client](./client.md)
2. waiter: [InstanceStatusOkWaiter](./waiters.md#instancestatusokwaiter)


### wait

Type annotations and code completion for `#!python InstanceStatusOkWaiter.wait` method.

```python
# wait method definition

await def wait(
    self,
    *,
    InstanceIds: Sequence[str] = ...,
    MaxResults: int = ...,
    NextToken: str = ...,
    DryRun: bool = ...,
    Filters: Sequence[FilterTypeDef] = ...,  # (1)
    IncludeAllInstances: bool = ...,
    WaiterConfig: WaiterConfigTypeDef = ...,  # (2)
) -> None:
    ...
```

1. See [:material-code-braces: FilterTypeDef](./type_defs.md#filtertypedef) 
2. See [:material-code-braces: WaiterConfigTypeDef](./type_defs.md#waiterconfigtypedef) 


```python
# wait method usage example with argument unpacking

kwargs: DescribeInstanceStatusRequestWaitTypeDef = {  # (1)
    "InstanceIds": ...,
}

parent.wait(**kwargs)
```

1. See [:material-code-braces: DescribeInstanceStatusRequestWaitTypeDef](./type_defs.md#describeinstancestatusrequestwaittypedef) 
## InstanceStoppedWaiter

Type annotations and code completion for `#!python session.create_client("ec2").get_waiter("instance_stopped")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ec2/waiter/InstanceStopped.html#EC2.Waiter.InstanceStopped)

```python
# InstanceStoppedWaiter usage example

from aiobotocore.session import Session

from types_aiobotocore_ec2.waiter import InstanceStoppedWaiter

session = get_session()
async with session.create_client("ec2") as client:  # (1)
    waiter: InstanceStoppedWaiter = client.get_waiter("instance_stopped")  # (2)
    await waiter.wait()
```

1. client: [EC2Client](./client.md)
2. waiter: [InstanceStoppedWaiter](./waiters.md#instancestoppedwaiter)


### wait

Type annotations and code completion for `#!python InstanceStoppedWaiter.wait` method.

```python
# wait method definition

await def wait(
    self,
    *,
    InstanceIds: Sequence[str] = ...,
    DryRun: bool = ...,
    Filters: Sequence[FilterTypeDef] = ...,  # (1)
    NextToken: str = ...,
    MaxResults: int = ...,
    WaiterConfig: WaiterConfigTypeDef = ...,  # (2)
) -> None:
    ...
```

1. See [:material-code-braces: FilterTypeDef](./type_defs.md#filtertypedef) 
2. See [:material-code-braces: WaiterConfigTypeDef](./type_defs.md#waiterconfigtypedef) 


```python
# wait method usage example with argument unpacking

kwargs: DescribeInstancesRequestWaitExtraExtraTypeDef = {  # (1)
    "InstanceIds": ...,
}

parent.wait(**kwargs)
```

1. See [:material-code-braces: DescribeInstancesRequestWaitExtraExtraTypeDef](./type_defs.md#describeinstancesrequestwaitextraextratypedef) 
## InstanceTerminatedWaiter

Type annotations and code completion for `#!python session.create_client("ec2").get_waiter("instance_terminated")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ec2/waiter/InstanceTerminated.html#EC2.Waiter.InstanceTerminated)

```python
# InstanceTerminatedWaiter usage example

from aiobotocore.session import Session

from types_aiobotocore_ec2.waiter import InstanceTerminatedWaiter

session = get_session()
async with session.create_client("ec2") as client:  # (1)
    waiter: InstanceTerminatedWaiter = client.get_waiter("instance_terminated")  # (2)
    await waiter.wait()
```

1. client: [EC2Client](./client.md)
2. waiter: [InstanceTerminatedWaiter](./waiters.md#instanceterminatedwaiter)


### wait

Type annotations and code completion for `#!python InstanceTerminatedWaiter.wait` method.

```python
# wait method definition

await def wait(
    self,
    *,
    InstanceIds: Sequence[str] = ...,
    DryRun: bool = ...,
    Filters: Sequence[FilterTypeDef] = ...,  # (1)
    NextToken: str = ...,
    MaxResults: int = ...,
    WaiterConfig: WaiterConfigTypeDef = ...,  # (2)
) -> None:
    ...
```

1. See [:material-code-braces: FilterTypeDef](./type_defs.md#filtertypedef) 
2. See [:material-code-braces: WaiterConfigTypeDef](./type_defs.md#waiterconfigtypedef) 


```python
# wait method usage example with argument unpacking

kwargs: DescribeInstancesRequestWaitExtraExtraExtraTypeDef = {  # (1)
    "InstanceIds": ...,
}

parent.wait(**kwargs)
```

1. See [:material-code-braces: DescribeInstancesRequestWaitExtraExtraExtraTypeDef](./type_defs.md#describeinstancesrequestwaitextraextraextratypedef) 
## InternetGatewayExistsWaiter

Type annotations and code completion for `#!python session.create_client("ec2").get_waiter("internet_gateway_exists")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ec2/waiter/InternetGatewayExists.html#EC2.Waiter.InternetGatewayExists)

```python
# InternetGatewayExistsWaiter usage example

from aiobotocore.session import Session

from types_aiobotocore_ec2.waiter import InternetGatewayExistsWaiter

session = get_session()
async with session.create_client("ec2") as client:  # (1)
    waiter: InternetGatewayExistsWaiter = client.get_waiter("internet_gateway_exists")  # (2)
    await waiter.wait()
```

1. client: [EC2Client](./client.md)
2. waiter: [InternetGatewayExistsWaiter](./waiters.md#internetgatewayexistswaiter)


### wait

Type annotations and code completion for `#!python InternetGatewayExistsWaiter.wait` method.

```python
# wait method definition

await def wait(
    self,
    *,
    NextToken: str = ...,
    MaxResults: int = ...,
    DryRun: bool = ...,
    InternetGatewayIds: Sequence[str] = ...,
    Filters: Sequence[FilterTypeDef] = ...,  # (1)
    WaiterConfig: WaiterConfigTypeDef = ...,  # (2)
) -> None:
    ...
```

1. See [:material-code-braces: FilterTypeDef](./type_defs.md#filtertypedef) 
2. See [:material-code-braces: WaiterConfigTypeDef](./type_defs.md#waiterconfigtypedef) 


```python
# wait method usage example with argument unpacking

kwargs: DescribeInternetGatewaysRequestWaitTypeDef = {  # (1)
    "NextToken": ...,
}

parent.wait(**kwargs)
```

1. See [:material-code-braces: DescribeInternetGatewaysRequestWaitTypeDef](./type_defs.md#describeinternetgatewaysrequestwaittypedef) 
## KeyPairExistsWaiter

Type annotations and code completion for `#!python session.create_client("ec2").get_waiter("key_pair_exists")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ec2/waiter/KeyPairExists.html#EC2.Waiter.KeyPairExists)

```python
# KeyPairExistsWaiter usage example

from aiobotocore.session import Session

from types_aiobotocore_ec2.waiter import KeyPairExistsWaiter

session = get_session()
async with session.create_client("ec2") as client:  # (1)
    waiter: KeyPairExistsWaiter = client.get_waiter("key_pair_exists")  # (2)
    await waiter.wait()
```

1. client: [EC2Client](./client.md)
2. waiter: [KeyPairExistsWaiter](./waiters.md#keypairexistswaiter)


### wait

Type annotations and code completion for `#!python KeyPairExistsWaiter.wait` method.

```python
# wait method definition

await def wait(
    self,
    *,
    KeyNames: Sequence[str] = ...,
    KeyPairIds: Sequence[str] = ...,
    IncludePublicKey: bool = ...,
    DryRun: bool = ...,
    Filters: Sequence[FilterTypeDef] = ...,  # (1)
    WaiterConfig: WaiterConfigTypeDef = ...,  # (2)
) -> None:
    ...
```

1. See [:material-code-braces: FilterTypeDef](./type_defs.md#filtertypedef) 
2. See [:material-code-braces: WaiterConfigTypeDef](./type_defs.md#waiterconfigtypedef) 


```python
# wait method usage example with argument unpacking

kwargs: DescribeKeyPairsRequestWaitTypeDef = {  # (1)
    "KeyNames": ...,
}

parent.wait(**kwargs)
```

1. See [:material-code-braces: DescribeKeyPairsRequestWaitTypeDef](./type_defs.md#describekeypairsrequestwaittypedef) 
## NatGatewayAvailableWaiter

Type annotations and code completion for `#!python session.create_client("ec2").get_waiter("nat_gateway_available")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ec2/waiter/NatGatewayAvailable.html#EC2.Waiter.NatGatewayAvailable)

```python
# NatGatewayAvailableWaiter usage example

from aiobotocore.session import Session

from types_aiobotocore_ec2.waiter import NatGatewayAvailableWaiter

session = get_session()
async with session.create_client("ec2") as client:  # (1)
    waiter: NatGatewayAvailableWaiter = client.get_waiter("nat_gateway_available")  # (2)
    await waiter.wait()
```

1. client: [EC2Client](./client.md)
2. waiter: [NatGatewayAvailableWaiter](./waiters.md#natgatewayavailablewaiter)


### wait

Type annotations and code completion for `#!python NatGatewayAvailableWaiter.wait` method.

```python
# wait method definition

await def wait(
    self,
    *,
    DryRun: bool = ...,
    Filters: Sequence[FilterTypeDef] = ...,  # (1)
    MaxResults: int = ...,
    NatGatewayIds: Sequence[str] = ...,
    NextToken: str = ...,
    WaiterConfig: WaiterConfigTypeDef = ...,  # (2)
) -> None:
    ...
```

1. See [:material-code-braces: FilterTypeDef](./type_defs.md#filtertypedef) 
2. See [:material-code-braces: WaiterConfigTypeDef](./type_defs.md#waiterconfigtypedef) 


```python
# wait method usage example with argument unpacking

kwargs: DescribeNatGatewaysRequestWaitTypeDef = {  # (1)
    "DryRun": ...,
}

parent.wait(**kwargs)
```

1. See [:material-code-braces: DescribeNatGatewaysRequestWaitTypeDef](./type_defs.md#describenatgatewaysrequestwaittypedef) 
## NatGatewayDeletedWaiter

Type annotations and code completion for `#!python session.create_client("ec2").get_waiter("nat_gateway_deleted")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ec2/waiter/NatGatewayDeleted.html#EC2.Waiter.NatGatewayDeleted)

```python
# NatGatewayDeletedWaiter usage example

from aiobotocore.session import Session

from types_aiobotocore_ec2.waiter import NatGatewayDeletedWaiter

session = get_session()
async with session.create_client("ec2") as client:  # (1)
    waiter: NatGatewayDeletedWaiter = client.get_waiter("nat_gateway_deleted")  # (2)
    await waiter.wait()
```

1. client: [EC2Client](./client.md)
2. waiter: [NatGatewayDeletedWaiter](./waiters.md#natgatewaydeletedwaiter)


### wait

Type annotations and code completion for `#!python NatGatewayDeletedWaiter.wait` method.

```python
# wait method definition

await def wait(
    self,
    *,
    DryRun: bool = ...,
    Filters: Sequence[FilterTypeDef] = ...,  # (1)
    MaxResults: int = ...,
    NatGatewayIds: Sequence[str] = ...,
    NextToken: str = ...,
    WaiterConfig: WaiterConfigTypeDef = ...,  # (2)
) -> None:
    ...
```

1. See [:material-code-braces: FilterTypeDef](./type_defs.md#filtertypedef) 
2. See [:material-code-braces: WaiterConfigTypeDef](./type_defs.md#waiterconfigtypedef) 


```python
# wait method usage example with argument unpacking

kwargs: DescribeNatGatewaysRequestWaitExtraTypeDef = {  # (1)
    "DryRun": ...,
}

parent.wait(**kwargs)
```

1. See [:material-code-braces: DescribeNatGatewaysRequestWaitExtraTypeDef](./type_defs.md#describenatgatewaysrequestwaitextratypedef) 
## NetworkInterfaceAvailableWaiter

Type annotations and code completion for `#!python session.create_client("ec2").get_waiter("network_interface_available")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ec2/waiter/NetworkInterfaceAvailable.html#EC2.Waiter.NetworkInterfaceAvailable)

```python
# NetworkInterfaceAvailableWaiter usage example

from aiobotocore.session import Session

from types_aiobotocore_ec2.waiter import NetworkInterfaceAvailableWaiter

session = get_session()
async with session.create_client("ec2") as client:  # (1)
    waiter: NetworkInterfaceAvailableWaiter = client.get_waiter("network_interface_available")  # (2)
    await waiter.wait()
```

1. client: [EC2Client](./client.md)
2. waiter: [NetworkInterfaceAvailableWaiter](./waiters.md#networkinterfaceavailablewaiter)


### wait

Type annotations and code completion for `#!python NetworkInterfaceAvailableWaiter.wait` method.

```python
# wait method definition

await def wait(
    self,
    *,
    NextToken: str = ...,
    MaxResults: int = ...,
    DryRun: bool = ...,
    NetworkInterfaceIds: Sequence[str] = ...,
    Filters: Sequence[FilterTypeDef] = ...,  # (1)
    WaiterConfig: WaiterConfigTypeDef = ...,  # (2)
) -> None:
    ...
```

1. See [:material-code-braces: FilterTypeDef](./type_defs.md#filtertypedef) 
2. See [:material-code-braces: WaiterConfigTypeDef](./type_defs.md#waiterconfigtypedef) 


```python
# wait method usage example with argument unpacking

kwargs: DescribeNetworkInterfacesRequestWaitTypeDef = {  # (1)
    "NextToken": ...,
}

parent.wait(**kwargs)
```

1. See [:material-code-braces: DescribeNetworkInterfacesRequestWaitTypeDef](./type_defs.md#describenetworkinterfacesrequestwaittypedef) 
## PasswordDataAvailableWaiter

Type annotations and code completion for `#!python session.create_client("ec2").get_waiter("password_data_available")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ec2/waiter/PasswordDataAvailable.html#EC2.Waiter.PasswordDataAvailable)

```python
# PasswordDataAvailableWaiter usage example

from aiobotocore.session import Session

from types_aiobotocore_ec2.waiter import PasswordDataAvailableWaiter

session = get_session()
async with session.create_client("ec2") as client:  # (1)
    waiter: PasswordDataAvailableWaiter = client.get_waiter("password_data_available")  # (2)
    await waiter.wait()
```

1. client: [EC2Client](./client.md)
2. waiter: [PasswordDataAvailableWaiter](./waiters.md#passworddataavailablewaiter)


### wait

Type annotations and code completion for `#!python PasswordDataAvailableWaiter.wait` method.

```python
# wait method definition

await def wait(
    self,
    *,
    InstanceId: str,
    DryRun: bool = ...,
    WaiterConfig: WaiterConfigTypeDef = ...,  # (1)
) -> None:
    ...
```

1. See [:material-code-braces: WaiterConfigTypeDef](./type_defs.md#waiterconfigtypedef) 


```python
# wait method usage example with argument unpacking

kwargs: GetPasswordDataRequestWaitTypeDef = {  # (1)
    "InstanceId": ...,
}

parent.wait(**kwargs)
```

1. See [:material-code-braces: GetPasswordDataRequestWaitTypeDef](./type_defs.md#getpassworddatarequestwaittypedef) 
## SecurityGroupExistsWaiter

Type annotations and code completion for `#!python session.create_client("ec2").get_waiter("security_group_exists")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ec2/waiter/SecurityGroupExists.html#EC2.Waiter.SecurityGroupExists)

```python
# SecurityGroupExistsWaiter usage example

from aiobotocore.session import Session

from types_aiobotocore_ec2.waiter import SecurityGroupExistsWaiter

session = get_session()
async with session.create_client("ec2") as client:  # (1)
    waiter: SecurityGroupExistsWaiter = client.get_waiter("security_group_exists")  # (2)
    await waiter.wait()
```

1. client: [EC2Client](./client.md)
2. waiter: [SecurityGroupExistsWaiter](./waiters.md#securitygroupexistswaiter)


### wait

Type annotations and code completion for `#!python SecurityGroupExistsWaiter.wait` method.

```python
# wait method definition

await def wait(
    self,
    *,
    GroupIds: Sequence[str] = ...,
    GroupNames: Sequence[str] = ...,
    NextToken: str = ...,
    MaxResults: int = ...,
    DryRun: bool = ...,
    Filters: Sequence[FilterTypeDef] = ...,  # (1)
    WaiterConfig: WaiterConfigTypeDef = ...,  # (2)
) -> None:
    ...
```

1. See [:material-code-braces: FilterTypeDef](./type_defs.md#filtertypedef) 
2. See [:material-code-braces: WaiterConfigTypeDef](./type_defs.md#waiterconfigtypedef) 


```python
# wait method usage example with argument unpacking

kwargs: DescribeSecurityGroupsRequestWaitTypeDef = {  # (1)
    "GroupIds": ...,
}

parent.wait(**kwargs)
```

1. See [:material-code-braces: DescribeSecurityGroupsRequestWaitTypeDef](./type_defs.md#describesecuritygroupsrequestwaittypedef) 
## SnapshotCompletedWaiter

Type annotations and code completion for `#!python session.create_client("ec2").get_waiter("snapshot_completed")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ec2/waiter/SnapshotCompleted.html#EC2.Waiter.SnapshotCompleted)

```python
# SnapshotCompletedWaiter usage example

from aiobotocore.session import Session

from types_aiobotocore_ec2.waiter import SnapshotCompletedWaiter

session = get_session()
async with session.create_client("ec2") as client:  # (1)
    waiter: SnapshotCompletedWaiter = client.get_waiter("snapshot_completed")  # (2)
    await waiter.wait()
```

1. client: [EC2Client](./client.md)
2. waiter: [SnapshotCompletedWaiter](./waiters.md#snapshotcompletedwaiter)


### wait

Type annotations and code completion for `#!python SnapshotCompletedWaiter.wait` method.

```python
# wait method definition

await def wait(
    self,
    *,
    MaxResults: int = ...,
    NextToken: str = ...,
    OwnerIds: Sequence[str] = ...,
    RestorableByUserIds: Sequence[str] = ...,
    SnapshotIds: Sequence[str] = ...,
    DryRun: bool = ...,
    Filters: Sequence[FilterTypeDef] = ...,  # (1)
    WaiterConfig: WaiterConfigTypeDef = ...,  # (2)
) -> None:
    ...
```

1. See [:material-code-braces: FilterTypeDef](./type_defs.md#filtertypedef) 
2. See [:material-code-braces: WaiterConfigTypeDef](./type_defs.md#waiterconfigtypedef) 


```python
# wait method usage example with argument unpacking

kwargs: DescribeSnapshotsRequestWaitTypeDef = {  # (1)
    "MaxResults": ...,
}

parent.wait(**kwargs)
```

1. See [:material-code-braces: DescribeSnapshotsRequestWaitTypeDef](./type_defs.md#describesnapshotsrequestwaittypedef) 
## SnapshotImportedWaiter

Type annotations and code completion for `#!python session.create_client("ec2").get_waiter("snapshot_imported")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ec2/waiter/SnapshotImported.html#EC2.Waiter.SnapshotImported)

```python
# SnapshotImportedWaiter usage example

from aiobotocore.session import Session

from types_aiobotocore_ec2.waiter import SnapshotImportedWaiter

session = get_session()
async with session.create_client("ec2") as client:  # (1)
    waiter: SnapshotImportedWaiter = client.get_waiter("snapshot_imported")  # (2)
    await waiter.wait()
```

1. client: [EC2Client](./client.md)
2. waiter: [SnapshotImportedWaiter](./waiters.md#snapshotimportedwaiter)


### wait

Type annotations and code completion for `#!python SnapshotImportedWaiter.wait` method.

```python
# wait method definition

await def wait(
    self,
    *,
    DryRun: bool = ...,
    Filters: Sequence[FilterTypeDef] = ...,  # (1)
    ImportTaskIds: Sequence[str] = ...,
    MaxResults: int = ...,
    NextToken: str = ...,
    WaiterConfig: WaiterConfigTypeDef = ...,  # (2)
) -> None:
    ...
```

1. See [:material-code-braces: FilterTypeDef](./type_defs.md#filtertypedef) 
2. See [:material-code-braces: WaiterConfigTypeDef](./type_defs.md#waiterconfigtypedef) 


```python
# wait method usage example with argument unpacking

kwargs: DescribeImportSnapshotTasksRequestWaitTypeDef = {  # (1)
    "DryRun": ...,
}

parent.wait(**kwargs)
```

1. See [:material-code-braces: DescribeImportSnapshotTasksRequestWaitTypeDef](./type_defs.md#describeimportsnapshottasksrequestwaittypedef) 
## SpotInstanceRequestFulfilledWaiter

Type annotations and code completion for `#!python session.create_client("ec2").get_waiter("spot_instance_request_fulfilled")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ec2/waiter/SpotInstanceRequestFulfilled.html#EC2.Waiter.SpotInstanceRequestFulfilled)

```python
# SpotInstanceRequestFulfilledWaiter usage example

from aiobotocore.session import Session

from types_aiobotocore_ec2.waiter import SpotInstanceRequestFulfilledWaiter

session = get_session()
async with session.create_client("ec2") as client:  # (1)
    waiter: SpotInstanceRequestFulfilledWaiter = client.get_waiter("spot_instance_request_fulfilled")  # (2)
    await waiter.wait()
```

1. client: [EC2Client](./client.md)
2. waiter: [SpotInstanceRequestFulfilledWaiter](./waiters.md#spotinstancerequestfulfilledwaiter)


### wait

Type annotations and code completion for `#!python SpotInstanceRequestFulfilledWaiter.wait` method.

```python
# wait method definition

await def wait(
    self,
    *,
    NextToken: str = ...,
    MaxResults: int = ...,
    DryRun: bool = ...,
    SpotInstanceRequestIds: Sequence[str] = ...,
    Filters: Sequence[FilterTypeDef] = ...,  # (1)
    WaiterConfig: WaiterConfigTypeDef = ...,  # (2)
) -> None:
    ...
```

1. See [:material-code-braces: FilterTypeDef](./type_defs.md#filtertypedef) 
2. See [:material-code-braces: WaiterConfigTypeDef](./type_defs.md#waiterconfigtypedef) 


```python
# wait method usage example with argument unpacking

kwargs: DescribeSpotInstanceRequestsRequestWaitTypeDef = {  # (1)
    "NextToken": ...,
}

parent.wait(**kwargs)
```

1. See [:material-code-braces: DescribeSpotInstanceRequestsRequestWaitTypeDef](./type_defs.md#describespotinstancerequestsrequestwaittypedef) 
## StoreImageTaskCompleteWaiter

Type annotations and code completion for `#!python session.create_client("ec2").get_waiter("store_image_task_complete")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ec2/waiter/StoreImageTaskComplete.html#EC2.Waiter.StoreImageTaskComplete)

```python
# StoreImageTaskCompleteWaiter usage example

from aiobotocore.session import Session

from types_aiobotocore_ec2.waiter import StoreImageTaskCompleteWaiter

session = get_session()
async with session.create_client("ec2") as client:  # (1)
    waiter: StoreImageTaskCompleteWaiter = client.get_waiter("store_image_task_complete")  # (2)
    await waiter.wait()
```

1. client: [EC2Client](./client.md)
2. waiter: [StoreImageTaskCompleteWaiter](./waiters.md#storeimagetaskcompletewaiter)


### wait

Type annotations and code completion for `#!python StoreImageTaskCompleteWaiter.wait` method.

```python
# wait method definition

await def wait(
    self,
    *,
    ImageIds: Sequence[str] = ...,
    DryRun: bool = ...,
    Filters: Sequence[FilterTypeDef] = ...,  # (1)
    NextToken: str = ...,
    MaxResults: int = ...,
    WaiterConfig: WaiterConfigTypeDef = ...,  # (2)
) -> None:
    ...
```

1. See [:material-code-braces: FilterTypeDef](./type_defs.md#filtertypedef) 
2. See [:material-code-braces: WaiterConfigTypeDef](./type_defs.md#waiterconfigtypedef) 


```python
# wait method usage example with argument unpacking

kwargs: DescribeStoreImageTasksRequestWaitTypeDef = {  # (1)
    "ImageIds": ...,
}

parent.wait(**kwargs)
```

1. See [:material-code-braces: DescribeStoreImageTasksRequestWaitTypeDef](./type_defs.md#describestoreimagetasksrequestwaittypedef) 
## SubnetAvailableWaiter

Type annotations and code completion for `#!python session.create_client("ec2").get_waiter("subnet_available")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ec2/waiter/SubnetAvailable.html#EC2.Waiter.SubnetAvailable)

```python
# SubnetAvailableWaiter usage example

from aiobotocore.session import Session

from types_aiobotocore_ec2.waiter import SubnetAvailableWaiter

session = get_session()
async with session.create_client("ec2") as client:  # (1)
    waiter: SubnetAvailableWaiter = client.get_waiter("subnet_available")  # (2)
    await waiter.wait()
```

1. client: [EC2Client](./client.md)
2. waiter: [SubnetAvailableWaiter](./waiters.md#subnetavailablewaiter)


### wait

Type annotations and code completion for `#!python SubnetAvailableWaiter.wait` method.

```python
# wait method definition

await def wait(
    self,
    *,
    Filters: Sequence[FilterTypeDef] = ...,  # (1)
    SubnetIds: Sequence[str] = ...,
    NextToken: str = ...,
    MaxResults: int = ...,
    DryRun: bool = ...,
    WaiterConfig: WaiterConfigTypeDef = ...,  # (2)
) -> None:
    ...
```

1. See [:material-code-braces: FilterTypeDef](./type_defs.md#filtertypedef) 
2. See [:material-code-braces: WaiterConfigTypeDef](./type_defs.md#waiterconfigtypedef) 


```python
# wait method usage example with argument unpacking

kwargs: DescribeSubnetsRequestWaitTypeDef = {  # (1)
    "Filters": ...,
}

parent.wait(**kwargs)
```

1. See [:material-code-braces: DescribeSubnetsRequestWaitTypeDef](./type_defs.md#describesubnetsrequestwaittypedef) 
## SystemStatusOkWaiter

Type annotations and code completion for `#!python session.create_client("ec2").get_waiter("system_status_ok")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ec2/waiter/SystemStatusOk.html#EC2.Waiter.SystemStatusOk)

```python
# SystemStatusOkWaiter usage example

from aiobotocore.session import Session

from types_aiobotocore_ec2.waiter import SystemStatusOkWaiter

session = get_session()
async with session.create_client("ec2") as client:  # (1)
    waiter: SystemStatusOkWaiter = client.get_waiter("system_status_ok")  # (2)
    await waiter.wait()
```

1. client: [EC2Client](./client.md)
2. waiter: [SystemStatusOkWaiter](./waiters.md#systemstatusokwaiter)


### wait

Type annotations and code completion for `#!python SystemStatusOkWaiter.wait` method.

```python
# wait method definition

await def wait(
    self,
    *,
    InstanceIds: Sequence[str] = ...,
    MaxResults: int = ...,
    NextToken: str = ...,
    DryRun: bool = ...,
    Filters: Sequence[FilterTypeDef] = ...,  # (1)
    IncludeAllInstances: bool = ...,
    WaiterConfig: WaiterConfigTypeDef = ...,  # (2)
) -> None:
    ...
```

1. See [:material-code-braces: FilterTypeDef](./type_defs.md#filtertypedef) 
2. See [:material-code-braces: WaiterConfigTypeDef](./type_defs.md#waiterconfigtypedef) 


```python
# wait method usage example with argument unpacking

kwargs: DescribeInstanceStatusRequestWaitExtraTypeDef = {  # (1)
    "InstanceIds": ...,
}

parent.wait(**kwargs)
```

1. See [:material-code-braces: DescribeInstanceStatusRequestWaitExtraTypeDef](./type_defs.md#describeinstancestatusrequestwaitextratypedef) 
## VolumeAvailableWaiter

Type annotations and code completion for `#!python session.create_client("ec2").get_waiter("volume_available")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ec2/waiter/VolumeAvailable.html#EC2.Waiter.VolumeAvailable)

```python
# VolumeAvailableWaiter usage example

from aiobotocore.session import Session

from types_aiobotocore_ec2.waiter import VolumeAvailableWaiter

session = get_session()
async with session.create_client("ec2") as client:  # (1)
    waiter: VolumeAvailableWaiter = client.get_waiter("volume_available")  # (2)
    await waiter.wait()
```

1. client: [EC2Client](./client.md)
2. waiter: [VolumeAvailableWaiter](./waiters.md#volumeavailablewaiter)


### wait

Type annotations and code completion for `#!python VolumeAvailableWaiter.wait` method.

```python
# wait method definition

await def wait(
    self,
    *,
    VolumeIds: Sequence[str] = ...,
    DryRun: bool = ...,
    Filters: Sequence[FilterTypeDef] = ...,  # (1)
    NextToken: str = ...,
    MaxResults: int = ...,
    WaiterConfig: WaiterConfigTypeDef = ...,  # (2)
) -> None:
    ...
```

1. See [:material-code-braces: FilterTypeDef](./type_defs.md#filtertypedef) 
2. See [:material-code-braces: WaiterConfigTypeDef](./type_defs.md#waiterconfigtypedef) 


```python
# wait method usage example with argument unpacking

kwargs: DescribeVolumesRequestWaitTypeDef = {  # (1)
    "VolumeIds": ...,
}

parent.wait(**kwargs)
```

1. See [:material-code-braces: DescribeVolumesRequestWaitTypeDef](./type_defs.md#describevolumesrequestwaittypedef) 
## VolumeDeletedWaiter

Type annotations and code completion for `#!python session.create_client("ec2").get_waiter("volume_deleted")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ec2/waiter/VolumeDeleted.html#EC2.Waiter.VolumeDeleted)

```python
# VolumeDeletedWaiter usage example

from aiobotocore.session import Session

from types_aiobotocore_ec2.waiter import VolumeDeletedWaiter

session = get_session()
async with session.create_client("ec2") as client:  # (1)
    waiter: VolumeDeletedWaiter = client.get_waiter("volume_deleted")  # (2)
    await waiter.wait()
```

1. client: [EC2Client](./client.md)
2. waiter: [VolumeDeletedWaiter](./waiters.md#volumedeletedwaiter)


### wait

Type annotations and code completion for `#!python VolumeDeletedWaiter.wait` method.

```python
# wait method definition

await def wait(
    self,
    *,
    VolumeIds: Sequence[str] = ...,
    DryRun: bool = ...,
    Filters: Sequence[FilterTypeDef] = ...,  # (1)
    NextToken: str = ...,
    MaxResults: int = ...,
    WaiterConfig: WaiterConfigTypeDef = ...,  # (2)
) -> None:
    ...
```

1. See [:material-code-braces: FilterTypeDef](./type_defs.md#filtertypedef) 
2. See [:material-code-braces: WaiterConfigTypeDef](./type_defs.md#waiterconfigtypedef) 


```python
# wait method usage example with argument unpacking

kwargs: DescribeVolumesRequestWaitExtraTypeDef = {  # (1)
    "VolumeIds": ...,
}

parent.wait(**kwargs)
```

1. See [:material-code-braces: DescribeVolumesRequestWaitExtraTypeDef](./type_defs.md#describevolumesrequestwaitextratypedef) 
## VolumeInUseWaiter

Type annotations and code completion for `#!python session.create_client("ec2").get_waiter("volume_in_use")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ec2/waiter/VolumeInUse.html#EC2.Waiter.VolumeInUse)

```python
# VolumeInUseWaiter usage example

from aiobotocore.session import Session

from types_aiobotocore_ec2.waiter import VolumeInUseWaiter

session = get_session()
async with session.create_client("ec2") as client:  # (1)
    waiter: VolumeInUseWaiter = client.get_waiter("volume_in_use")  # (2)
    await waiter.wait()
```

1. client: [EC2Client](./client.md)
2. waiter: [VolumeInUseWaiter](./waiters.md#volumeinusewaiter)


### wait

Type annotations and code completion for `#!python VolumeInUseWaiter.wait` method.

```python
# wait method definition

await def wait(
    self,
    *,
    VolumeIds: Sequence[str] = ...,
    DryRun: bool = ...,
    Filters: Sequence[FilterTypeDef] = ...,  # (1)
    NextToken: str = ...,
    MaxResults: int = ...,
    WaiterConfig: WaiterConfigTypeDef = ...,  # (2)
) -> None:
    ...
```

1. See [:material-code-braces: FilterTypeDef](./type_defs.md#filtertypedef) 
2. See [:material-code-braces: WaiterConfigTypeDef](./type_defs.md#waiterconfigtypedef) 


```python
# wait method usage example with argument unpacking

kwargs: DescribeVolumesRequestWaitExtraExtraTypeDef = {  # (1)
    "VolumeIds": ...,
}

parent.wait(**kwargs)
```

1. See [:material-code-braces: DescribeVolumesRequestWaitExtraExtraTypeDef](./type_defs.md#describevolumesrequestwaitextraextratypedef) 
## VpcAvailableWaiter

Type annotations and code completion for `#!python session.create_client("ec2").get_waiter("vpc_available")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ec2/waiter/VpcAvailable.html#EC2.Waiter.VpcAvailable)

```python
# VpcAvailableWaiter usage example

from aiobotocore.session import Session

from types_aiobotocore_ec2.waiter import VpcAvailableWaiter

session = get_session()
async with session.create_client("ec2") as client:  # (1)
    waiter: VpcAvailableWaiter = client.get_waiter("vpc_available")  # (2)
    await waiter.wait()
```

1. client: [EC2Client](./client.md)
2. waiter: [VpcAvailableWaiter](./waiters.md#vpcavailablewaiter)


### wait

Type annotations and code completion for `#!python VpcAvailableWaiter.wait` method.

```python
# wait method definition

await def wait(
    self,
    *,
    Filters: Sequence[FilterTypeDef] = ...,  # (1)
    VpcIds: Sequence[str] = ...,
    NextToken: str = ...,
    MaxResults: int = ...,
    DryRun: bool = ...,
    WaiterConfig: WaiterConfigTypeDef = ...,  # (2)
) -> None:
    ...
```

1. See [:material-code-braces: FilterTypeDef](./type_defs.md#filtertypedef) 
2. See [:material-code-braces: WaiterConfigTypeDef](./type_defs.md#waiterconfigtypedef) 


```python
# wait method usage example with argument unpacking

kwargs: DescribeVpcsRequestWaitTypeDef = {  # (1)
    "Filters": ...,
}

parent.wait(**kwargs)
```

1. See [:material-code-braces: DescribeVpcsRequestWaitTypeDef](./type_defs.md#describevpcsrequestwaittypedef) 
## VpcExistsWaiter

Type annotations and code completion for `#!python session.create_client("ec2").get_waiter("vpc_exists")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ec2/waiter/VpcExists.html#EC2.Waiter.VpcExists)

```python
# VpcExistsWaiter usage example

from aiobotocore.session import Session

from types_aiobotocore_ec2.waiter import VpcExistsWaiter

session = get_session()
async with session.create_client("ec2") as client:  # (1)
    waiter: VpcExistsWaiter = client.get_waiter("vpc_exists")  # (2)
    await waiter.wait()
```

1. client: [EC2Client](./client.md)
2. waiter: [VpcExistsWaiter](./waiters.md#vpcexistswaiter)


### wait

Type annotations and code completion for `#!python VpcExistsWaiter.wait` method.

```python
# wait method definition

await def wait(
    self,
    *,
    Filters: Sequence[FilterTypeDef] = ...,  # (1)
    VpcIds: Sequence[str] = ...,
    NextToken: str = ...,
    MaxResults: int = ...,
    DryRun: bool = ...,
    WaiterConfig: WaiterConfigTypeDef = ...,  # (2)
) -> None:
    ...
```

1. See [:material-code-braces: FilterTypeDef](./type_defs.md#filtertypedef) 
2. See [:material-code-braces: WaiterConfigTypeDef](./type_defs.md#waiterconfigtypedef) 


```python
# wait method usage example with argument unpacking

kwargs: DescribeVpcsRequestWaitExtraTypeDef = {  # (1)
    "Filters": ...,
}

parent.wait(**kwargs)
```

1. See [:material-code-braces: DescribeVpcsRequestWaitExtraTypeDef](./type_defs.md#describevpcsrequestwaitextratypedef) 
## VpcPeeringConnectionDeletedWaiter

Type annotations and code completion for `#!python session.create_client("ec2").get_waiter("vpc_peering_connection_deleted")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ec2/waiter/VpcPeeringConnectionDeleted.html#EC2.Waiter.VpcPeeringConnectionDeleted)

```python
# VpcPeeringConnectionDeletedWaiter usage example

from aiobotocore.session import Session

from types_aiobotocore_ec2.waiter import VpcPeeringConnectionDeletedWaiter

session = get_session()
async with session.create_client("ec2") as client:  # (1)
    waiter: VpcPeeringConnectionDeletedWaiter = client.get_waiter("vpc_peering_connection_deleted")  # (2)
    await waiter.wait()
```

1. client: [EC2Client](./client.md)
2. waiter: [VpcPeeringConnectionDeletedWaiter](./waiters.md#vpcpeeringconnectiondeletedwaiter)


### wait

Type annotations and code completion for `#!python VpcPeeringConnectionDeletedWaiter.wait` method.

```python
# wait method definition

await def wait(
    self,
    *,
    NextToken: str = ...,
    MaxResults: int = ...,
    DryRun: bool = ...,
    VpcPeeringConnectionIds: Sequence[str] = ...,
    Filters: Sequence[FilterTypeDef] = ...,  # (1)
    WaiterConfig: WaiterConfigTypeDef = ...,  # (2)
) -> None:
    ...
```

1. See [:material-code-braces: FilterTypeDef](./type_defs.md#filtertypedef) 
2. See [:material-code-braces: WaiterConfigTypeDef](./type_defs.md#waiterconfigtypedef) 


```python
# wait method usage example with argument unpacking

kwargs: DescribeVpcPeeringConnectionsRequestWaitExtraTypeDef = {  # (1)
    "NextToken": ...,
}

parent.wait(**kwargs)
```

1. See [:material-code-braces: DescribeVpcPeeringConnectionsRequestWaitExtraTypeDef](./type_defs.md#describevpcpeeringconnectionsrequestwaitextratypedef) 
## VpcPeeringConnectionExistsWaiter

Type annotations and code completion for `#!python session.create_client("ec2").get_waiter("vpc_peering_connection_exists")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ec2/waiter/VpcPeeringConnectionExists.html#EC2.Waiter.VpcPeeringConnectionExists)

```python
# VpcPeeringConnectionExistsWaiter usage example

from aiobotocore.session import Session

from types_aiobotocore_ec2.waiter import VpcPeeringConnectionExistsWaiter

session = get_session()
async with session.create_client("ec2") as client:  # (1)
    waiter: VpcPeeringConnectionExistsWaiter = client.get_waiter("vpc_peering_connection_exists")  # (2)
    await waiter.wait()
```

1. client: [EC2Client](./client.md)
2. waiter: [VpcPeeringConnectionExistsWaiter](./waiters.md#vpcpeeringconnectionexistswaiter)


### wait

Type annotations and code completion for `#!python VpcPeeringConnectionExistsWaiter.wait` method.

```python
# wait method definition

await def wait(
    self,
    *,
    NextToken: str = ...,
    MaxResults: int = ...,
    DryRun: bool = ...,
    VpcPeeringConnectionIds: Sequence[str] = ...,
    Filters: Sequence[FilterTypeDef] = ...,  # (1)
    WaiterConfig: WaiterConfigTypeDef = ...,  # (2)
) -> None:
    ...
```

1. See [:material-code-braces: FilterTypeDef](./type_defs.md#filtertypedef) 
2. See [:material-code-braces: WaiterConfigTypeDef](./type_defs.md#waiterconfigtypedef) 


```python
# wait method usage example with argument unpacking

kwargs: DescribeVpcPeeringConnectionsRequestWaitTypeDef = {  # (1)
    "NextToken": ...,
}

parent.wait(**kwargs)
```

1. See [:material-code-braces: DescribeVpcPeeringConnectionsRequestWaitTypeDef](./type_defs.md#describevpcpeeringconnectionsrequestwaittypedef) 
## VpnConnectionAvailableWaiter

Type annotations and code completion for `#!python session.create_client("ec2").get_waiter("vpn_connection_available")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ec2/waiter/VpnConnectionAvailable.html#EC2.Waiter.VpnConnectionAvailable)

```python
# VpnConnectionAvailableWaiter usage example

from aiobotocore.session import Session

from types_aiobotocore_ec2.waiter import VpnConnectionAvailableWaiter

session = get_session()
async with session.create_client("ec2") as client:  # (1)
    waiter: VpnConnectionAvailableWaiter = client.get_waiter("vpn_connection_available")  # (2)
    await waiter.wait()
```

1. client: [EC2Client](./client.md)
2. waiter: [VpnConnectionAvailableWaiter](./waiters.md#vpnconnectionavailablewaiter)


### wait

Type annotations and code completion for `#!python VpnConnectionAvailableWaiter.wait` method.

```python
# wait method definition

await def wait(
    self,
    *,
    Filters: Sequence[FilterTypeDef] = ...,  # (1)
    VpnConnectionIds: Sequence[str] = ...,
    DryRun: bool = ...,
    WaiterConfig: WaiterConfigTypeDef = ...,  # (2)
) -> None:
    ...
```

1. See [:material-code-braces: FilterTypeDef](./type_defs.md#filtertypedef) 
2. See [:material-code-braces: WaiterConfigTypeDef](./type_defs.md#waiterconfigtypedef) 


```python
# wait method usage example with argument unpacking

kwargs: DescribeVpnConnectionsRequestWaitTypeDef = {  # (1)
    "Filters": ...,
}

parent.wait(**kwargs)
```

1. See [:material-code-braces: DescribeVpnConnectionsRequestWaitTypeDef](./type_defs.md#describevpnconnectionsrequestwaittypedef) 
## VpnConnectionDeletedWaiter

Type annotations and code completion for `#!python session.create_client("ec2").get_waiter("vpn_connection_deleted")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ec2/waiter/VpnConnectionDeleted.html#EC2.Waiter.VpnConnectionDeleted)

```python
# VpnConnectionDeletedWaiter usage example

from aiobotocore.session import Session

from types_aiobotocore_ec2.waiter import VpnConnectionDeletedWaiter

session = get_session()
async with session.create_client("ec2") as client:  # (1)
    waiter: VpnConnectionDeletedWaiter = client.get_waiter("vpn_connection_deleted")  # (2)
    await waiter.wait()
```

1. client: [EC2Client](./client.md)
2. waiter: [VpnConnectionDeletedWaiter](./waiters.md#vpnconnectiondeletedwaiter)


### wait

Type annotations and code completion for `#!python VpnConnectionDeletedWaiter.wait` method.

```python
# wait method definition

await def wait(
    self,
    *,
    Filters: Sequence[FilterTypeDef] = ...,  # (1)
    VpnConnectionIds: Sequence[str] = ...,
    DryRun: bool = ...,
    WaiterConfig: WaiterConfigTypeDef = ...,  # (2)
) -> None:
    ...
```

1. See [:material-code-braces: FilterTypeDef](./type_defs.md#filtertypedef) 
2. See [:material-code-braces: WaiterConfigTypeDef](./type_defs.md#waiterconfigtypedef) 


```python
# wait method usage example with argument unpacking

kwargs: DescribeVpnConnectionsRequestWaitExtraTypeDef = {  # (1)
    "Filters": ...,
}

parent.wait(**kwargs)
```

1. See [:material-code-braces: DescribeVpnConnectionsRequestWaitExtraTypeDef](./type_defs.md#describevpnconnectionsrequestwaitextratypedef) 
