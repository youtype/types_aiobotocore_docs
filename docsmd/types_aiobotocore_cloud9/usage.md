# Examples

> [Index](../README.md) > [Cloud9](./README.md) > Examples

!!! note ""

    Auto-generated documentation for [Cloud9](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloud9.html#cloud9)
    type annotations stubs module [types-aiobotocore-cloud9](https://pypi.org/project/types-aiobotocore-cloud9/).

## Client

### Implicit type annotations

Can be used with `types-aiobotocore[cloud9]` package installed.

Write your `Cloud9` code as usual,
type checking and code completion should work out of the box.



```python
# Cloud9Client usage example

from aiobotocore.session import get_session


session = get_session()

async with session.create_client("cloud9") as client:  # (1)
    result = await client.create_environment_ec2()  # (2)
```

1. client: [Cloud9Client](./client.md)
2. result: [:material-code-braces: CreateEnvironmentEC2ResultTypeDef](./type_defs.md#createenvironmentec2resulttypedef) 



```python
# DescribeEnvironmentMembershipsPaginator usage example

from aiobotocore.session import get_session


session = get_session()

async with session.create_client("cloud9") as client:  # (1)
    paginator = client.get_paginator("describe_environment_memberships")  # (2)
    async for item in paginator.paginate(...):
        print(item)  # (3)
```

1. client: [Cloud9Client](./client.md)
2. paginator: [DescribeEnvironmentMembershipsPaginator](./paginators.md#describeenvironmentmembershipspaginator)
3. item: [:material-code-braces: DescribeEnvironmentMembershipsResultTypeDef](./type_defs.md#describeenvironmentmembershipsresulttypedef) 




### Explicit type annotations

With `types-aiobotocore-lite[cloud9]`
or a standalone `types_aiobotocore_cloud9` package, you have to explicitly specify
`client: Cloud9Client` type annotation.

All other type annotations are optional, as types should be discovered automatically.
However, these type annotations can be helpful in your functions and methods.


```python
# Cloud9Client usage example with type annotations

from aiobotocore.session import get_session

from types_aiobotocore_cloud9.client import Cloud9Client
from types_aiobotocore_cloud9.type_defs import CreateEnvironmentEC2ResultTypeDef
from types_aiobotocore_cloud9.type_defs import CreateEnvironmentEC2RequestTypeDef


session = get_session()

async with session.create_client("cloud9") as client:
    client: Cloud9Client
    kwargs: CreateEnvironmentEC2RequestTypeDef = {...}
    result: CreateEnvironmentEC2ResultTypeDef = await client.create_environment_ec2(**kwargs)
```



```python
# DescribeEnvironmentMembershipsPaginator usage example with type annotations

from aiobotocore.session import get_session

from types_aiobotocore_cloud9.client import Cloud9Client
from types_aiobotocore_cloud9.paginator import DescribeEnvironmentMembershipsPaginator
from types_aiobotocore_cloud9.type_defs import DescribeEnvironmentMembershipsResultTypeDef


session = get_session()

async with session.create_client("cloud9") as client:
    client: Cloud9Client
    paginator: DescribeEnvironmentMembershipsPaginator = client.get_paginator("describe_environment_memberships")
    async for item in paginator.paginate(...):
        item: DescribeEnvironmentMembershipsResultTypeDef
        print(item)
```


