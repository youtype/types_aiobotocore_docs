# Waiters

> [Index](../README.md) > [Signer](./README.md) > Waiters

!!! note ""

    Auto-generated documentation for [Signer](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/signer.html#signer)
    type annotations stubs module [types-aiobotocore-signer](https://pypi.org/project/types-aiobotocore-signer/).

## SuccessfulSigningJobWaiter

Type annotations and code completion for `#!python session.create_client("signer").get_waiter("successful_signing_job")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/signer/waiter/SuccessfulSigningJob.html#Signer.Waiter.SuccessfulSigningJob)

```python
# SuccessfulSigningJobWaiter usage example

from aiobotocore.session import Session

from types_aiobotocore_signer.waiter import SuccessfulSigningJobWaiter

session = get_session()
async with session.create_client("signer") as client:  # (1)
    waiter: SuccessfulSigningJobWaiter = client.get_waiter("successful_signing_job")  # (2)
    await waiter.wait()
```

1. client: [SignerClient](./client.md)
2. waiter: [SuccessfulSigningJobWaiter](./waiters.md#successfulsigningjobwaiter)


### wait

Type annotations and code completion for `#!python SuccessfulSigningJobWaiter.wait` method.

```python
# wait method definition

await def wait(
    self,
    *,
    jobId: str,
    WaiterConfig: WaiterConfigTypeDef = ...,  # (1)
) -> None:
    ...
```

1. See [:material-code-braces: WaiterConfigTypeDef](./type_defs.md#waiterconfigtypedef) 


```python
# wait method usage example with argument unpacking

kwargs: DescribeSigningJobRequestWaitTypeDef = {  # (1)
    "jobId": ...,
}

parent.wait(**kwargs)
```

1. See [:material-code-braces: DescribeSigningJobRequestWaitTypeDef](./type_defs.md#describesigningjobrequestwaittypedef) 
