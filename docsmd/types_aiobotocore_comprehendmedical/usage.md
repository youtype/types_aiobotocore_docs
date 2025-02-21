# Examples

> [Index](../README.md) > [ComprehendMedical](./README.md) > Examples

!!! note ""

    Auto-generated documentation for [ComprehendMedical](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/comprehendmedical.html#comprehendmedical)
    type annotations stubs module [types-aiobotocore-comprehendmedical](https://pypi.org/project/types-aiobotocore-comprehendmedical/).

## Client

### Implicit type annotations

Can be used with `types-aiobotocore[comprehendmedical]` package installed.

Write your `ComprehendMedical` code as usual,
type checking and code completion should work out of the box.



```python
# ComprehendMedicalClient usage example

from aiobotocore.session import get_session


session = get_session()

async with session.create_client("comprehendmedical") as client:  # (1)
    result = await client.describe_entities_detection_v2_job()  # (2)
```

1. client: [ComprehendMedicalClient](./client.md)
2. result: [:material-code-braces: DescribeEntitiesDetectionV2JobResponseTypeDef](./type_defs.md#describeentitiesdetectionv2jobresponsetypedef) 






### Explicit type annotations

With `types-aiobotocore-lite[comprehendmedical]`
or a standalone `types_aiobotocore_comprehendmedical` package, you have to explicitly specify
`client: ComprehendMedicalClient` type annotation.

All other type annotations are optional, as types should be discovered automatically.
However, these type annotations can be helpful in your functions and methods.


```python
# ComprehendMedicalClient usage example with type annotations

from aiobotocore.session import get_session

from types_aiobotocore_comprehendmedical.client import ComprehendMedicalClient
from types_aiobotocore_comprehendmedical.type_defs import DescribeEntitiesDetectionV2JobResponseTypeDef
from types_aiobotocore_comprehendmedical.type_defs import DescribeEntitiesDetectionV2JobRequestTypeDef


session = get_session()

async with session.create_client("comprehendmedical") as client:
    client: ComprehendMedicalClient
    kwargs: DescribeEntitiesDetectionV2JobRequestTypeDef = {...}
    result: DescribeEntitiesDetectionV2JobResponseTypeDef = await client.describe_entities_detection_v2_job(**kwargs)
```




