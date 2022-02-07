<a id="waiters-for-aiobotocore-rekognition-module"></a>

# Waiters for aiobotocore Rekognition module

> [Index](..) > [Rekognition](.) > Waiters

Auto-generated documentation for
[Rekognition](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rekognition.html#Rekognition)
type annotations stubs module
[types-aiobotocore-rekognition](https://pypi.org/project/types-aiobotocore-rekognition/).

- [Waiters for aiobotocore Rekognition module](#waiters-for-aiobotocore-rekognition-module)
  - [ProjectVersionRunningWaiter](#projectversionrunningwaiter)
  - [ProjectVersionTrainingCompletedWaiter](#projectversiontrainingcompletedwaiter)

<a id="projectversionrunningwaiter"></a>

## ProjectVersionRunningWaiter

Type annotations for
`session.create_client("rekognition").get_waiter("project_version_running")`.

Can be used directly:

```python
from aiobotocore.session import Session

from types_aiobotocore_rekognition.waiter import ProjectVersionRunningWaiter

def get_project_version_running_waiter() -> ProjectVersionRunningWaiter:
    return Session().client("rekognition").get_waiter("project_version_running")
```

Boto3 documentation:
[Rekognition.Waiter.project_version_running](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rekognition.html#Rekognition.Waiter.ProjectVersionRunning)

Arguments for `ProjectVersionRunningWaiter.wait` method:

- `ProjectArn`: `str` *(required)*
- `VersionNames`: `Sequence`\[`str`\]
- `NextToken`: `str`
- `MaxResults`: `int`
- `WaiterConfig`: [WaiterConfigTypeDef](./type_defs.md#waiterconfigtypedef)

<a id="projectversiontrainingcompletedwaiter"></a>

## ProjectVersionTrainingCompletedWaiter

Type annotations for
`session.create_client("rekognition").get_waiter("project_version_training_completed")`.

Can be used directly:

```python
from aiobotocore.session import Session

from types_aiobotocore_rekognition.waiter import ProjectVersionTrainingCompletedWaiter

def get_project_version_training_completed_waiter() -> ProjectVersionTrainingCompletedWaiter:
    return Session().client("rekognition").get_waiter("project_version_training_completed")
```

Boto3 documentation:
[Rekognition.Waiter.project_version_training_completed](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rekognition.html#Rekognition.Waiter.ProjectVersionTrainingCompleted)

Arguments for `ProjectVersionTrainingCompletedWaiter.wait` method:

- `ProjectArn`: `str` *(required)*
- `VersionNames`: `Sequence`\[`str`\]
- `NextToken`: `str`
- `MaxResults`: `int`
- `WaiterConfig`: [WaiterConfigTypeDef](./type_defs.md#waiterconfigtypedef)
