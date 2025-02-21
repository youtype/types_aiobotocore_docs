# Examples

> [Index](../README.md) > [ElasticBeanstalk](./README.md) > Examples

!!! note ""

    Auto-generated documentation for [ElasticBeanstalk](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elasticbeanstalk.html#elasticbeanstalk)
    type annotations stubs module [types-aiobotocore-elasticbeanstalk](https://pypi.org/project/types-aiobotocore-elasticbeanstalk/).

## Client

### Implicit type annotations

Can be used with `types-aiobotocore[elasticbeanstalk]` package installed.

Write your `ElasticBeanstalk` code as usual,
type checking and code completion should work out of the box.



```python
# ElasticBeanstalkClient usage example

from aiobotocore.session import get_session


session = get_session()

async with session.create_client("elasticbeanstalk") as client:  # (1)
    result = await client.abort_environment_update()  # (2)
```

1. client: [ElasticBeanstalkClient](./client.md)
2. result: [:material-code-braces: EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef) 



```python
# DescribeApplicationVersionsPaginator usage example

from aiobotocore.session import get_session


session = get_session()

async with session.create_client("elasticbeanstalk") as client:  # (1)
    paginator = client.get_paginator("describe_application_versions")  # (2)
    async for item in paginator.paginate(...):
        print(item)  # (3)
```

1. client: [ElasticBeanstalkClient](./client.md)
2. paginator: [DescribeApplicationVersionsPaginator](./paginators.md#describeapplicationversionspaginator)
3. item: [:material-code-braces: ApplicationVersionDescriptionsMessageTypeDef](./type_defs.md#applicationversiondescriptionsmessagetypedef) 



```python
# EnvironmentExistsWaiter usage example

from aiobotocore.session import get_session


session = get_session()

async with session.create_client("elasticbeanstalk") as client:  # (1)
    waiter = client.get_waiter("environment_exists")  # (2)
    await waiter.wait()
```

1. client: [ElasticBeanstalkClient](./client.md)
2. waiter: [EnvironmentExistsWaiter](./waiters.md#environmentexistswaiter)


### Explicit type annotations

With `types-aiobotocore-lite[elasticbeanstalk]`
or a standalone `types_aiobotocore_elasticbeanstalk` package, you have to explicitly specify
`client: ElasticBeanstalkClient` type annotation.

All other type annotations are optional, as types should be discovered automatically.
However, these type annotations can be helpful in your functions and methods.


```python
# ElasticBeanstalkClient usage example with type annotations

from aiobotocore.session import get_session

from types_aiobotocore_elasticbeanstalk.client import ElasticBeanstalkClient
from types_aiobotocore_elasticbeanstalk.type_defs import EmptyResponseMetadataTypeDef
from types_aiobotocore_elasticbeanstalk.type_defs import AbortEnvironmentUpdateMessageTypeDef


session = get_session()

async with session.create_client("elasticbeanstalk") as client:
    client: ElasticBeanstalkClient
    kwargs: AbortEnvironmentUpdateMessageTypeDef = {...}
    result: EmptyResponseMetadataTypeDef = await client.abort_environment_update(**kwargs)
```



```python
# DescribeApplicationVersionsPaginator usage example with type annotations

from aiobotocore.session import get_session

from types_aiobotocore_elasticbeanstalk.client import ElasticBeanstalkClient
from types_aiobotocore_elasticbeanstalk.paginator import DescribeApplicationVersionsPaginator
from types_aiobotocore_elasticbeanstalk.type_defs import ApplicationVersionDescriptionsMessageTypeDef


session = get_session()

async with session.create_client("elasticbeanstalk") as client:
    client: ElasticBeanstalkClient
    paginator: DescribeApplicationVersionsPaginator = client.get_paginator("describe_application_versions")
    async for item in paginator.paginate(...):
        item: ApplicationVersionDescriptionsMessageTypeDef
        print(item)
```



```python
# EnvironmentExistsWaiter usage example with type annotations

from aiobotocore.session import get_session

from types_aiobotocore_elasticbeanstalk.client import ElasticBeanstalkClient
from types_aiobotocore_elasticbeanstalk.waiter import EnvironmentExistsWaiter


session = get_session()

async with session.create_client("elasticbeanstalk") as client:
    client: ElasticBeanstalkClient
    waiter: EnvironmentExistsWaiter = client.get_waiter("environment_exists")
    await waiter.wait()
```
