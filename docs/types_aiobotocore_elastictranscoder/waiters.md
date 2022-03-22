<a id="waiters-for-aiobotocore-elastictranscoder-module"></a>

# Waiters for aiobotocore ElasticTranscoder module

> [Index](../README.md) > [ElasticTranscoder](./README.md) > Waiters

Auto-generated documentation for
[ElasticTranscoder](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elastictranscoder.html#ElasticTranscoder)
type annotations stubs module
[types-aiobotocore-elastictranscoder](https://pypi.org/project/types-aiobotocore-elastictranscoder/).

- [Waiters for aiobotocore ElasticTranscoder module](#waiters-for-aiobotocore-elastictranscoder-module)
  - [JobCompleteWaiter](#jobcompletewaiter)

<a id="jobcompletewaiter"></a>

## JobCompleteWaiter

Type annotations for
`session.create_client("elastictranscoder").get_waiter("job_complete")`.

Can be used directly:

```python
from aiobotocore.session import Session

from types_aiobotocore_elastictranscoder.waiter import JobCompleteWaiter

def get_job_complete_waiter() -> JobCompleteWaiter:
    return Session().client("elastictranscoder").get_waiter("job_complete")
```

Boto3 documentation:
[ElasticTranscoder.Waiter.job_complete](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elastictranscoder.html#ElasticTranscoder.Waiter.JobComplete)

Arguments for `JobCompleteWaiter.wait` method:

- `Id`: `str` *(required)*
- `WaiterConfig`: [WaiterConfigTypeDef](./type_defs.md#waiterconfigtypedef)
