# Waiters

> [Index](../README.md) > [ECR](./README.md) > Waiters

!!! note ""

    Auto-generated documentation for [ECR](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ecr.html#ecr)
    type annotations stubs module [types-aiobotocore-ecr](https://pypi.org/project/types-aiobotocore-ecr/).

## ImageScanCompleteWaiter

Type annotations and code completion for `#!python session.create_client("ecr").get_waiter("image_scan_complete")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ecr/waiter/ImageScanComplete.html#ECR.Waiter.ImageScanComplete)

```python
# ImageScanCompleteWaiter usage example

from aiobotocore.session import Session

from types_aiobotocore_ecr.waiter import ImageScanCompleteWaiter

session = get_session()
async with session.create_client("ecr") as client:  # (1)
    waiter: ImageScanCompleteWaiter = client.get_waiter("image_scan_complete")  # (2)
    await waiter.wait()
```

1. client: [ECRClient](./client.md)
2. waiter: [ImageScanCompleteWaiter](./waiters.md#imagescancompletewaiter)


### wait

Type annotations and code completion for `#!python ImageScanCompleteWaiter.wait` method.

```python
# wait method definition

await def wait(
    self,
    *,
    repositoryName: str,
    imageId: ImageIdentifierTypeDef,  # (1)
    registryId: str = ...,
    nextToken: str = ...,
    maxResults: int = ...,
    WaiterConfig: WaiterConfigTypeDef = ...,  # (2)
) -> None:
    ...
```

1. See [:material-code-braces: ImageIdentifierTypeDef](./type_defs.md#imageidentifiertypedef) 
2. See [:material-code-braces: WaiterConfigTypeDef](./type_defs.md#waiterconfigtypedef) 


```python
# wait method usage example with argument unpacking

kwargs: DescribeImageScanFindingsRequestWaitTypeDef = {  # (1)
    "repositoryName": ...,
    "imageId": ...,
}

parent.wait(**kwargs)
```

1. See [:material-code-braces: DescribeImageScanFindingsRequestWaitTypeDef](./type_defs.md#describeimagescanfindingsrequestwaittypedef) 
## LifecyclePolicyPreviewCompleteWaiter

Type annotations and code completion for `#!python session.create_client("ecr").get_waiter("lifecycle_policy_preview_complete")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ecr/waiter/LifecyclePolicyPreviewComplete.html#ECR.Waiter.LifecyclePolicyPreviewComplete)

```python
# LifecyclePolicyPreviewCompleteWaiter usage example

from aiobotocore.session import Session

from types_aiobotocore_ecr.waiter import LifecyclePolicyPreviewCompleteWaiter

session = get_session()
async with session.create_client("ecr") as client:  # (1)
    waiter: LifecyclePolicyPreviewCompleteWaiter = client.get_waiter("lifecycle_policy_preview_complete")  # (2)
    await waiter.wait()
```

1. client: [ECRClient](./client.md)
2. waiter: [LifecyclePolicyPreviewCompleteWaiter](./waiters.md#lifecyclepolicypreviewcompletewaiter)


### wait

Type annotations and code completion for `#!python LifecyclePolicyPreviewCompleteWaiter.wait` method.

```python
# wait method definition

await def wait(
    self,
    *,
    repositoryName: str,
    registryId: str = ...,
    imageIds: Sequence[ImageIdentifierTypeDef] = ...,  # (1)
    nextToken: str = ...,
    maxResults: int = ...,
    filter: LifecyclePolicyPreviewFilterTypeDef = ...,  # (2)
    WaiterConfig: WaiterConfigTypeDef = ...,  # (3)
) -> None:
    ...
```

1. See [:material-code-braces: ImageIdentifierTypeDef](./type_defs.md#imageidentifiertypedef) 
2. See [:material-code-braces: LifecyclePolicyPreviewFilterTypeDef](./type_defs.md#lifecyclepolicypreviewfiltertypedef) 
3. See [:material-code-braces: WaiterConfigTypeDef](./type_defs.md#waiterconfigtypedef) 


```python
# wait method usage example with argument unpacking

kwargs: GetLifecyclePolicyPreviewRequestWaitTypeDef = {  # (1)
    "repositoryName": ...,
}

parent.wait(**kwargs)
```

1. See [:material-code-braces: GetLifecyclePolicyPreviewRequestWaitTypeDef](./type_defs.md#getlifecyclepolicypreviewrequestwaittypedef) 
