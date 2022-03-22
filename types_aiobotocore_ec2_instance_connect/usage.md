<a id="examples-for-aiobotocore-ec2instanceconnect-module"></a>

# Examples for aiobotocore EC2InstanceConnect module

> [Index](../README.md) > [EC2InstanceConnect](./README.md) > Examples

- [Examples for aiobotocore EC2InstanceConnect module](#examples-for-aiobotocore-ec2instanceconnect-module)
  - [Client](#client)
    - [Implicit type annotations](#implicit-type-annotations)
    - [Explicit type annotations](#explicit-type-annotations)

<a id="client"></a>

## Client

<a id="implicit-type-annotations"></a>

### Implicit type annotations

Can be used with `types-aiobotocore[ec2-instance-connect]` package installed.

Write your `EC2InstanceConnect` code as usual, type checking and code
completion should work out of the box.

```python
from aiobotocore.session import get_session


session = get_session()

# client has type EC2InstanceConnectClient
# and provides type checking and code completion
async with session.create_client("ec2-instance-connect") as client:
    
    # result has type bool
    # and provides type checking and code completion
    # IDE should show a hint with argument names and types
    result = await client.can_paginate()
    

    

    
```

<a id="explicit-type-annotations"></a>

### Explicit type annotations

With `types-aiobotocore-lite[ec2-instance-connect]` or a standalone
`types_aiobotocore_ec2_instance_connect` package, you have to explicitly
specify `client: EC2InstanceConnectClient` type annotation.

All other type annotations are optional, as types should be discovered
automatically. However, these type annotations can be helpful in your functions
and methods.

```python
from aiobotocore.session import get_session

from types_aiobotocore_ec2_instance_connect.client import EC2InstanceConnectClient
from types_aiobotocore_ec2_instance_connect.type_defs import bool






session = get_session()

async with session.create_client("ec2-instance-connect") as client:
    client: EC2InstanceConnectClient

    
    result: bool = client.can_paginate()
    

    

    
```
