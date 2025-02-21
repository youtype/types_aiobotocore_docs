# Waiters

> [Index](../README.md) > [CloudWatch](./README.md) > Waiters

!!! note ""

    Auto-generated documentation for [CloudWatch](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudwatch.html#cloudwatch)
    type annotations stubs module [types-aiobotocore-cloudwatch](https://pypi.org/project/types-aiobotocore-cloudwatch/).

## AlarmExistsWaiter

Type annotations and code completion for `#!python session.create_client("cloudwatch").get_waiter("alarm_exists")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudwatch/waiter/AlarmExists.html#CloudWatch.Waiter.AlarmExists)

```python
# AlarmExistsWaiter usage example

from aiobotocore.session import Session

from types_aiobotocore_cloudwatch.waiter import AlarmExistsWaiter

session = get_session()
async with session.create_client("cloudwatch") as client:  # (1)
    waiter: AlarmExistsWaiter = client.get_waiter("alarm_exists")  # (2)
    await waiter.wait()
```

1. client: [CloudWatchClient](./client.md)
2. waiter: [AlarmExistsWaiter](./waiters.md#alarmexistswaiter)


### wait

Type annotations and code completion for `#!python AlarmExistsWaiter.wait` method.

```python
# wait method definition

await def wait(
    self,
    *,
    AlarmNames: Sequence[str] = ...,
    AlarmNamePrefix: str = ...,
    AlarmTypes: Sequence[AlarmTypeType] = ...,  # (1)
    ChildrenOfAlarmName: str = ...,
    ParentsOfAlarmName: str = ...,
    StateValue: StateValueType = ...,  # (2)
    ActionPrefix: str = ...,
    MaxRecords: int = ...,
    NextToken: str = ...,
    WaiterConfig: WaiterConfigTypeDef = ...,  # (3)
) -> None:
    ...
```

1. See [:material-code-brackets: AlarmTypeType](./literals.md#alarmtypetype) 
2. See [:material-code-brackets: StateValueType](./literals.md#statevaluetype) 
3. See [:material-code-braces: WaiterConfigTypeDef](./type_defs.md#waiterconfigtypedef) 


```python
# wait method usage example with argument unpacking

kwargs: DescribeAlarmsInputWaitTypeDef = {  # (1)
    "AlarmNames": ...,
}

parent.wait(**kwargs)
```

1. See [:material-code-braces: DescribeAlarmsInputWaitTypeDef](./type_defs.md#describealarmsinputwaittypedef) 
## CompositeAlarmExistsWaiter

Type annotations and code completion for `#!python session.create_client("cloudwatch").get_waiter("composite_alarm_exists")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudwatch/waiter/CompositeAlarmExists.html#CloudWatch.Waiter.CompositeAlarmExists)

```python
# CompositeAlarmExistsWaiter usage example

from aiobotocore.session import Session

from types_aiobotocore_cloudwatch.waiter import CompositeAlarmExistsWaiter

session = get_session()
async with session.create_client("cloudwatch") as client:  # (1)
    waiter: CompositeAlarmExistsWaiter = client.get_waiter("composite_alarm_exists")  # (2)
    await waiter.wait()
```

1. client: [CloudWatchClient](./client.md)
2. waiter: [CompositeAlarmExistsWaiter](./waiters.md#compositealarmexistswaiter)


### wait

Type annotations and code completion for `#!python CompositeAlarmExistsWaiter.wait` method.

```python
# wait method definition

await def wait(
    self,
    *,
    AlarmNames: Sequence[str] = ...,
    AlarmNamePrefix: str = ...,
    AlarmTypes: Sequence[AlarmTypeType] = ...,  # (1)
    ChildrenOfAlarmName: str = ...,
    ParentsOfAlarmName: str = ...,
    StateValue: StateValueType = ...,  # (2)
    ActionPrefix: str = ...,
    MaxRecords: int = ...,
    NextToken: str = ...,
    WaiterConfig: WaiterConfigTypeDef = ...,  # (3)
) -> None:
    ...
```

1. See [:material-code-brackets: AlarmTypeType](./literals.md#alarmtypetype) 
2. See [:material-code-brackets: StateValueType](./literals.md#statevaluetype) 
3. See [:material-code-braces: WaiterConfigTypeDef](./type_defs.md#waiterconfigtypedef) 


```python
# wait method usage example with argument unpacking

kwargs: DescribeAlarmsInputWaitExtraTypeDef = {  # (1)
    "AlarmNames": ...,
}

parent.wait(**kwargs)
```

1. See [:material-code-braces: DescribeAlarmsInputWaitExtraTypeDef](./type_defs.md#describealarmsinputwaitextratypedef) 
