# Examples

> [Index](../README.md) > [SageMakerFeatureStoreRuntime](./README.md) > Examples

!!! note ""

    Auto-generated documentation for [SageMakerFeatureStoreRuntime](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker-featurestore-runtime.html#sagemakerfeaturestoreruntime)
    type annotations stubs module [types-aiobotocore-sagemaker-featurestore-runtime](https://pypi.org/project/types-aiobotocore-sagemaker-featurestore-runtime/).

## Client

### Implicit type annotations

Can be used with `types-aiobotocore[sagemaker-featurestore-runtime]` package installed.

Write your `SageMakerFeatureStoreRuntime` code as usual,
type checking and code completion should work out of the box.



```python
# SageMakerFeatureStoreRuntimeClient usage example

from aiobotocore.session import get_session


session = get_session()

async with session.create_client("sagemaker-featurestore-runtime") as client:  # (1)
    result = await client.batch_get_record()  # (2)
```

1. client: [SageMakerFeatureStoreRuntimeClient](./client.md)
2. result: [:material-code-braces: BatchGetRecordResponseTypeDef](./type_defs.md#batchgetrecordresponsetypedef) 






### Explicit type annotations

With `types-aiobotocore-lite[sagemaker-featurestore-runtime]`
or a standalone `types_aiobotocore_sagemaker_featurestore_runtime` package, you have to explicitly specify
`client: SageMakerFeatureStoreRuntimeClient` type annotation.

All other type annotations are optional, as types should be discovered automatically.
However, these type annotations can be helpful in your functions and methods.


```python
# SageMakerFeatureStoreRuntimeClient usage example with type annotations

from aiobotocore.session import get_session

from types_aiobotocore_sagemaker_featurestore_runtime.client import SageMakerFeatureStoreRuntimeClient
from types_aiobotocore_sagemaker_featurestore_runtime.type_defs import BatchGetRecordResponseTypeDef
from types_aiobotocore_sagemaker_featurestore_runtime.type_defs import BatchGetRecordRequestTypeDef


session = get_session()

async with session.create_client("sagemaker-featurestore-runtime") as client:
    client: SageMakerFeatureStoreRuntimeClient
    kwargs: BatchGetRecordRequestTypeDef = {...}
    result: BatchGetRecordResponseTypeDef = await client.batch_get_record(**kwargs)
```




