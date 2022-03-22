<a id="examples-for-aiobotocore-elasticbeanstalk-module"></a>

# Examples for aiobotocore ElasticBeanstalk module

> [Index](../README.md) > [ElasticBeanstalk](./README.md) > Examples

- [Examples for aiobotocore ElasticBeanstalk module](#examples-for-aiobotocore-elasticbeanstalk-module)
  - [Client](#client)
    - [Implicit type annotations](#implicit-type-annotations)
    - [Explicit type annotations](#explicit-type-annotations)

<a id="client"></a>

## Client

<a id="implicit-type-annotations"></a>

### Implicit type annotations

Can be used with `types-aiobotocore[elasticbeanstalk]` package installed.

Write your `ElasticBeanstalk` code as usual, type checking and code completion
should work out of the box.

```python
from aiobotocore.session import get_session


session = get_session()

# client has type ElasticBeanstalkClient
# and provides type checking and code completion
async with session.create_client("elasticbeanstalk") as client:
    
    # result has type None
    # and provides type checking and code completion
    # IDE should show a hint with argument names and types
    result = await client.abort_environment_update()
    

    
    # paginator has type DescribeApplicationVersionsPaginator and provides type checking
    # and code completion for paginate method
    paginator = client.get_paginator("describe_application_versions")
    async for item in paginator.paginate(...):
        # item has type ApplicationVersionDescriptionsMessageTypeDef
        print(item)
    

    
    # waiter has type EnvironmentExistsWaiter and provides type checking
    # and code completion for wait method
    waiter = client.get_waiter("environment_exists")
    await waiter.wait()
    
```

<a id="explicit-type-annotations"></a>

### Explicit type annotations

With `types-aiobotocore-lite[elasticbeanstalk]` or a standalone
`types_aiobotocore_elasticbeanstalk` package, you have to explicitly specify
`client: ElasticBeanstalkClient` type annotation.

All other type annotations are optional, as types should be discovered
automatically. However, these type annotations can be helpful in your functions
and methods.

```python
from aiobotocore.session import get_session

from types_aiobotocore_elasticbeanstalk.client import ElasticBeanstalkClient
from types_aiobotocore_elasticbeanstalk.type_defs import None
from types_aiobotocore_elasticbeanstalk.paginator import DescribeApplicationVersionsPaginator
from types_aiobotocore_elasticbeanstalk.waiter import EnvironmentExistsWaiter
from types_aiobotocore_elasticbeanstalk.literals import PaginatorName
from types_aiobotocore_elasticbeanstalk.literals import WaiterName


session = get_session()

async with session.create_client("elasticbeanstalk") as client:
    client: ElasticBeanstalkClient

    
    result: None = client.abort_environment_update()
    

    
    paginator_name: PaginatorName = "describe_application_versions"
    paginator: DescribeApplicationVersionsPaginator = client.get_paginator(paginator_name)
    async for item in paginator.paginate(...):
        item: ApplicationVersionDescriptionsMessageTypeDef
        print(item)
    

    
    waiter_name: WaiterName = "environment_exists"
    waiter: EnvironmentExistsWaiter = client.get_waiter(waiter_name)
    await waiter.wait()
    
```
