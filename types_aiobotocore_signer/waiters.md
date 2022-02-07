<a id="waiters-for-aiobotocore-signer-module"></a>

# Waiters for aiobotocore signer module

> [Index](..) > [signer](.) > Waiters

Auto-generated documentation for
[signer](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/signer.html#signer)
type annotations stubs module
[types-aiobotocore-signer](https://pypi.org/project/types-aiobotocore-signer/).

- [Waiters for aiobotocore signer module](#waiters-for-aiobotocore-signer-module)
  - [SuccessfulSigningJobWaiter](#successfulsigningjobwaiter)

<a id="successfulsigningjobwaiter"></a>

## SuccessfulSigningJobWaiter

Type annotations for
`session.create_client("signer").get_waiter("successful_signing_job")`.

Can be used directly:

```python
from aiobotocore.session import Session

from types_aiobotocore_signer.waiter import SuccessfulSigningJobWaiter

def get_successful_signing_job_waiter() -> SuccessfulSigningJobWaiter:
    return Session().client("signer").get_waiter("successful_signing_job")
```

Boto3 documentation:
[signer.Waiter.successful_signing_job](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/signer.html#signer.Waiter.SuccessfulSigningJob)

Arguments for `SuccessfulSigningJobWaiter.wait` method:

- `jobId`: `str` *(required)*
- `WaiterConfig`: [WaiterConfigTypeDef](./type_defs.md#waiterconfigtypedef)
