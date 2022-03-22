<a id="examples-for-aiobotocore-sagemakerfeaturestoreruntime-module"></a>

# Examples for aiobotocore SageMakerFeatureStoreRuntime module

> [Index](../README.md) > [SageMakerFeatureStoreRuntime](./README.md) >
> Examples

- [Examples for aiobotocore SageMakerFeatureStoreRuntime module](#examples-for-aiobotocore-sagemakerfeaturestoreruntime-module)
  - [Client](#client)
    - [Implicit type annotations](#implicit-type-annotations)
    - [Explicit type annotations](#explicit-type-annotations)

<a id="client"></a>

## Client

<a id="implicit-type-annotations"></a>

### Implicit type annotations

Can be used with `types-aiobotocore[sagemaker-featurestore-runtime]` package
installed.

Write your `SageMakerFeatureStoreRuntime` code as usual, type checking and code
completion should work out of the box.

```python
from aiobotocore.session import get_session


session = get_session()

# client has type SageMakerFeatureStoreRuntimeClient
# and provides type checking and code completion
async with session.create_client("sagemaker-featurestore-runtime") as client:
    
    # result has type BatchGetRecordResponseTypeDef
    # and provides type checking and code completion
    # IDE should show a hint with argument names and types
    result = await client.batch_get_record()
    

    

    
```

<a id="explicit-type-annotations"></a>

### Explicit type annotations

With `types-aiobotocore-lite[sagemaker-featurestore-runtime]` or a standalone
`types_aiobotocore_sagemaker_featurestore_runtime` package, you have to
explicitly specify `client: SageMakerFeatureStoreRuntimeClient` type
annotation.

All other type annotations are optional, as types should be discovered
automatically. However, these type annotations can be helpful in your functions
and methods.

```python
from aiobotocore.session import get_session

from types_aiobotocore_sagemaker_featurestore_runtime.client import SageMakerFeatureStoreRuntimeClient
from types_aiobotocore_sagemaker_featurestore_runtime.type_defs import BatchGetRecordResponseTypeDef






session = get_session()

async with session.create_client("sagemaker-featurestore-runtime") as client:
    client: SageMakerFeatureStoreRuntimeClient

    
    result: BatchGetRecordResponseTypeDef = client.batch_get_record()
    

    

    
```
