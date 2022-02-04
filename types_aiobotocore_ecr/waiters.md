<a id="waiters-for-aiobotocore-ecr-module"></a>

# Waiters for aiobotocore ECR module

> [Index](..) > [ECR](.) > Waiters

Auto-generated documentation for
[ECR](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ecr.html#ECR)
type annotations stubs module
[types-aiobotocore-ecr](https://pypi.org/project/types-aiobotocore-ecr/).

- [Waiters for aiobotocore ECR module](#waiters-for-aiobotocore-ecr-module)
  - [ImageScanCompleteWaiter](#imagescancompletewaiter)
  - [LifecyclePolicyPreviewCompleteWaiter](#lifecyclepolicypreviewcompletewaiter)

<a id="imagescancompletewaiter"></a>

## ImageScanCompleteWaiter

Type annotations for
`aiobotocore.create_client("ecr").get_waiter("image_scan_complete")`.

Can be used directly:

```python
from aiobotocore.session import Session

from types_aiobotocore_ecr.waiter import ImageScanCompleteWaiter

def get_image_scan_complete_waiter() -> ImageScanCompleteWaiter:
    return Session().create_client("ecr").get_waiter("image_scan_complete")
```

Boto3 documentation:
[ECR.Waiter.image_scan_complete](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ecr.html#ECR.Waiter.ImageScanComplete)

Arguments for `ImageScanCompleteWaiter.wait` method:

- `repositoryName`: `str` *(required)*
- `imageId`: [ImageIdentifierTypeDef](./type_defs.md#imageidentifiertypedef)
  *(required)*
- `registryId`: `str`
- `nextToken`: `str`
- `maxResults`: `int`
- `WaiterConfig`: [WaiterConfigTypeDef](./type_defs.md#waiterconfigtypedef)

<a id="lifecyclepolicypreviewcompletewaiter"></a>

## LifecyclePolicyPreviewCompleteWaiter

Type annotations for
`aiobotocore.create_client("ecr").get_waiter("lifecycle_policy_preview_complete")`.

Can be used directly:

```python
from aiobotocore.session import Session

from types_aiobotocore_ecr.waiter import LifecyclePolicyPreviewCompleteWaiter

def get_lifecycle_policy_preview_complete_waiter() -> LifecyclePolicyPreviewCompleteWaiter:
    return Session().create_client("ecr").get_waiter("lifecycle_policy_preview_complete")
```

Boto3 documentation:
[ECR.Waiter.lifecycle_policy_preview_complete](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ecr.html#ECR.Waiter.LifecyclePolicyPreviewComplete)

Arguments for `LifecyclePolicyPreviewCompleteWaiter.wait` method:

- `repositoryName`: `str` *(required)*
- `registryId`: `str`
- `imageIds`:
  `Sequence`\[[ImageIdentifierTypeDef](./type_defs.md#imageidentifiertypedef)\]
- `nextToken`: `str`
- `maxResults`: `int`
- `filter`:
  [LifecyclePolicyPreviewFilterTypeDef](./type_defs.md#lifecyclepolicypreviewfiltertypedef)
- `WaiterConfig`: [WaiterConfigTypeDef](./type_defs.md#waiterconfigtypedef)
