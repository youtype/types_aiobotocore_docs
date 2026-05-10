# Waiters

> [Index](../README.md) > [ElementalInference](./README.md) > Waiters

!!! note ""

    Auto-generated documentation for [ElementalInference](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elementalinference.html#elementalinference)
    type annotations stubs module [types-aiobotocore-elementalinference](https://pypi.org/project/types-aiobotocore-elementalinference/).

## FeedDeletedWaiter

Type annotations and code completion for `#!python session.create_client("elementalinference").get_waiter("feed_deleted")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elementalinference/waiter/FeedDeleted.html#ElementalInference.Waiter.FeedDeleted)

```python
# FeedDeletedWaiter usage example

from aiobotocore.session import Session

from types_aiobotocore_elementalinference.waiter import FeedDeletedWaiter

session = get_session()
async with session.create_client("elementalinference") as client:  # (1)
    waiter: FeedDeletedWaiter = client.get_waiter("feed_deleted")  # (2)
    await waiter.wait(...)
```

1. client: [ElementalInferenceClient](./client.md)
2. waiter: [FeedDeletedWaiter](./waiters.md#feeddeletedwaiter)


### wait

Type annotations and code completion for `#!python FeedDeletedWaiter.wait` method.

```python
# wait method definition

await def wait(
    self,
    *,
    id: str,
    WaiterConfig: WaiterConfigTypeDef = ...,  # (1)
) -> None:
    ...
```

1. See [:material-code-braces: WaiterConfigTypeDef](./type_defs.md#waiterconfigtypedef)


```python
# wait method usage example with argument unpacking

kwargs: GetFeedRequestWaitTypeDef = {  # (1)
    "id": ...,
}

parent.wait(**kwargs)
```

1. See [:material-code-braces: GetFeedRequestWaitTypeDef](./type_defs.md#getfeedrequestwaittypedef)
