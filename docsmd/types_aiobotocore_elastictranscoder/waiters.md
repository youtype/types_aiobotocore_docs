# Waiters

> [Index](../README.md) > [ElasticTranscoder](./README.md) > Waiters

!!! note ""

    Auto-generated documentation for [ElasticTranscoder](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elastictranscoder.html#elastictranscoder)
    type annotations stubs module [types-aiobotocore-elastictranscoder](https://pypi.org/project/types-aiobotocore-elastictranscoder/).

## JobCompleteWaiter

Type annotations and code completion for `#!python session.create_client("elastictranscoder").get_waiter("job_complete")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elastictranscoder/waiter/JobComplete.html#ElasticTranscoder.Waiter.JobComplete)

```python
# JobCompleteWaiter usage example

from aiobotocore.session import Session

from types_aiobotocore_elastictranscoder.waiter import JobCompleteWaiter

session = get_session()
async with session.create_client("elastictranscoder") as client:  # (1)
    waiter: JobCompleteWaiter = client.get_waiter("job_complete")  # (2)
    await waiter.wait()
```

1. client: [ElasticTranscoderClient](./client.md)
2. waiter: [JobCompleteWaiter](./waiters.md#jobcompletewaiter)


### wait

Type annotations and code completion for `#!python JobCompleteWaiter.wait` method.

```python
# wait method definition

await def wait(
    self,
    *,
    Id: str,
    WaiterConfig: WaiterConfigTypeDef = ...,  # (1)
) -> None:
    ...
```

1. See [:material-code-braces: WaiterConfigTypeDef](./type_defs.md#waiterconfigtypedef) 


```python
# wait method usage example with argument unpacking

kwargs: ReadJobRequestWaitTypeDef = {  # (1)
    "Id": ...,
}

parent.wait(**kwargs)
```

1. See [:material-code-braces: ReadJobRequestWaitTypeDef](./type_defs.md#readjobrequestwaittypedef) 
