<a id="waiters-for-aiobotocore-cloudwatch-module"></a>

# Waiters for aiobotocore CloudWatch module

> [Index](../README.md) > [CloudWatch](./README.md) > Waiters

Auto-generated documentation for
[CloudWatch](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudwatch.html#CloudWatch)
type annotations stubs module
[types-aiobotocore-cloudwatch](https://pypi.org/project/types-aiobotocore-cloudwatch/).

- [Waiters for aiobotocore CloudWatch module](#waiters-for-aiobotocore-cloudwatch-module)
  - [AlarmExistsWaiter](#alarmexistswaiter)
  - [CompositeAlarmExistsWaiter](#compositealarmexistswaiter)

<a id="alarmexistswaiter"></a>

## AlarmExistsWaiter

Type annotations for
`session.create_client("cloudwatch").get_waiter("alarm_exists")`.

Can be used directly:

```python
from aiobotocore.session import Session

from types_aiobotocore_cloudwatch.waiter import AlarmExistsWaiter

def get_alarm_exists_waiter() -> AlarmExistsWaiter:
    return Session().client("cloudwatch").get_waiter("alarm_exists")
```

Boto3 documentation:
[CloudWatch.Waiter.alarm_exists](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudwatch.html#CloudWatch.Waiter.AlarmExists)

Arguments for `AlarmExistsWaiter.wait` method:

- `AlarmNames`: `Sequence`\[`str`\]
- `AlarmNamePrefix`: `str`
- `AlarmTypes`: `Sequence`\[[AlarmTypeType](./literals.md#alarmtypetype)\]
- `ChildrenOfAlarmName`: `str`
- `ParentsOfAlarmName`: `str`
- `StateValue`: [StateValueType](./literals.md#statevaluetype)
- `ActionPrefix`: `str`
- `MaxRecords`: `int`
- `NextToken`: `str`
- `WaiterConfig`: [WaiterConfigTypeDef](./type_defs.md#waiterconfigtypedef)

<a id="compositealarmexistswaiter"></a>

## CompositeAlarmExistsWaiter

Type annotations for
`session.create_client("cloudwatch").get_waiter("composite_alarm_exists")`.

Can be used directly:

```python
from aiobotocore.session import Session

from types_aiobotocore_cloudwatch.waiter import CompositeAlarmExistsWaiter

def get_composite_alarm_exists_waiter() -> CompositeAlarmExistsWaiter:
    return Session().client("cloudwatch").get_waiter("composite_alarm_exists")
```

Boto3 documentation:
[CloudWatch.Waiter.composite_alarm_exists](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudwatch.html#CloudWatch.Waiter.CompositeAlarmExists)

Arguments for `CompositeAlarmExistsWaiter.wait` method:

- `AlarmNames`: `Sequence`\[`str`\]
- `AlarmNamePrefix`: `str`
- `AlarmTypes`: `Sequence`\[[AlarmTypeType](./literals.md#alarmtypetype)\]
- `ChildrenOfAlarmName`: `str`
- `ParentsOfAlarmName`: `str`
- `StateValue`: [StateValueType](./literals.md#statevaluetype)
- `ActionPrefix`: `str`
- `MaxRecords`: `int`
- `NextToken`: `str`
- `WaiterConfig`: [WaiterConfigTypeDef](./type_defs.md#waiterconfigtypedef)
