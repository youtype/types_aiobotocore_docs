<a id="waiters-for-aiobotocore-elasticbeanstalk-module"></a>

# Waiters for aiobotocore ElasticBeanstalk module

> [Index](..) > [ElasticBeanstalk](.) > Waiters

Auto-generated documentation for
[ElasticBeanstalk](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elasticbeanstalk.html#ElasticBeanstalk)
type annotations stubs module
[types-aiobotocore-elasticbeanstalk](https://pypi.org/project/types-aiobotocore-elasticbeanstalk/).

- [Waiters for aiobotocore ElasticBeanstalk module](#waiters-for-aiobotocore-elasticbeanstalk-module)
  - [EnvironmentExistsWaiter](#environmentexistswaiter)
  - [EnvironmentTerminatedWaiter](#environmentterminatedwaiter)
  - [EnvironmentUpdatedWaiter](#environmentupdatedwaiter)

<a id="environmentexistswaiter"></a>

## EnvironmentExistsWaiter

Type annotations for
`aiobotocore.create_client("elasticbeanstalk").get_waiter("environment_exists")`.

Can be used directly:

```python
from aiobotocore.session import Session

from types_aiobotocore_elasticbeanstalk.waiter import EnvironmentExistsWaiter

def get_environment_exists_waiter() -> EnvironmentExistsWaiter:
    return Session().create_client("elasticbeanstalk").get_waiter("environment_exists")
```

Boto3 documentation:
[ElasticBeanstalk.Waiter.environment_exists](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elasticbeanstalk.html#ElasticBeanstalk.Waiter.EnvironmentExists)

Arguments for `EnvironmentExistsWaiter.wait` method:

- `ApplicationName`: `str`
- `VersionLabel`: `str`
- `EnvironmentIds`: `Sequence`\[`str`\]
- `EnvironmentNames`: `Sequence`\[`str`\]
- `IncludeDeleted`: `bool`
- `IncludedDeletedBackTo`: `Union`\[`datetime`, `str`\]
- `MaxRecords`: `int`
- `NextToken`: `str`
- `WaiterConfig`: [WaiterConfigTypeDef](./type_defs.md#waiterconfigtypedef)

<a id="environmentterminatedwaiter"></a>

## EnvironmentTerminatedWaiter

Type annotations for
`aiobotocore.create_client("elasticbeanstalk").get_waiter("environment_terminated")`.

Can be used directly:

```python
from aiobotocore.session import Session

from types_aiobotocore_elasticbeanstalk.waiter import EnvironmentTerminatedWaiter

def get_environment_terminated_waiter() -> EnvironmentTerminatedWaiter:
    return Session().create_client("elasticbeanstalk").get_waiter("environment_terminated")
```

Boto3 documentation:
[ElasticBeanstalk.Waiter.environment_terminated](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elasticbeanstalk.html#ElasticBeanstalk.Waiter.EnvironmentTerminated)

Arguments for `EnvironmentTerminatedWaiter.wait` method:

- `ApplicationName`: `str`
- `VersionLabel`: `str`
- `EnvironmentIds`: `Sequence`\[`str`\]
- `EnvironmentNames`: `Sequence`\[`str`\]
- `IncludeDeleted`: `bool`
- `IncludedDeletedBackTo`: `Union`\[`datetime`, `str`\]
- `MaxRecords`: `int`
- `NextToken`: `str`
- `WaiterConfig`: [WaiterConfigTypeDef](./type_defs.md#waiterconfigtypedef)

<a id="environmentupdatedwaiter"></a>

## EnvironmentUpdatedWaiter

Type annotations for
`aiobotocore.create_client("elasticbeanstalk").get_waiter("environment_updated")`.

Can be used directly:

```python
from aiobotocore.session import Session

from types_aiobotocore_elasticbeanstalk.waiter import EnvironmentUpdatedWaiter

def get_environment_updated_waiter() -> EnvironmentUpdatedWaiter:
    return Session().create_client("elasticbeanstalk").get_waiter("environment_updated")
```

Boto3 documentation:
[ElasticBeanstalk.Waiter.environment_updated](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elasticbeanstalk.html#ElasticBeanstalk.Waiter.EnvironmentUpdated)

Arguments for `EnvironmentUpdatedWaiter.wait` method:

- `ApplicationName`: `str`
- `VersionLabel`: `str`
- `EnvironmentIds`: `Sequence`\[`str`\]
- `EnvironmentNames`: `Sequence`\[`str`\]
- `IncludeDeleted`: `bool`
- `IncludedDeletedBackTo`: `Union`\[`datetime`, `str`\]
- `MaxRecords`: `int`
- `NextToken`: `str`
- `WaiterConfig`: [WaiterConfigTypeDef](./type_defs.md#waiterconfigtypedef)
