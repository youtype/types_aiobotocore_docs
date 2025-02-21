# Examples

> [Index](../README.md) > [CloudWatchLogs](./README.md) > Examples

!!! note ""

    Auto-generated documentation for [CloudWatchLogs](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/logs.html#cloudwatchlogs)
    type annotations stubs module [types-aiobotocore-logs](https://pypi.org/project/types-aiobotocore-logs/).

## Client

### Implicit type annotations

Can be used with `types-aiobotocore[logs]` package installed.

Write your `CloudWatchLogs` code as usual,
type checking and code completion should work out of the box.



```python
# CloudWatchLogsClient usage example

from aiobotocore.session import get_session


session = get_session()

async with session.create_client("logs") as client:  # (1)
    result = await client.associate_kms_key()  # (2)
```

1. client: [CloudWatchLogsClient](./client.md)
2. result: [:material-code-braces: EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef) 



```python
# DescribeConfigurationTemplatesPaginator usage example

from aiobotocore.session import get_session


session = get_session()

async with session.create_client("logs") as client:  # (1)
    paginator = client.get_paginator("describe_configuration_templates")  # (2)
    async for item in paginator.paginate(...):
        print(item)  # (3)
```

1. client: [CloudWatchLogsClient](./client.md)
2. paginator: [DescribeConfigurationTemplatesPaginator](./paginators.md#describeconfigurationtemplatespaginator)
3. item: [:material-code-braces: DescribeConfigurationTemplatesResponseTypeDef](./type_defs.md#describeconfigurationtemplatesresponsetypedef) 




### Explicit type annotations

With `types-aiobotocore-lite[logs]`
or a standalone `types_aiobotocore_logs` package, you have to explicitly specify
`client: CloudWatchLogsClient` type annotation.

All other type annotations are optional, as types should be discovered automatically.
However, these type annotations can be helpful in your functions and methods.


```python
# CloudWatchLogsClient usage example with type annotations

from aiobotocore.session import get_session

from types_aiobotocore_logs.client import CloudWatchLogsClient
from types_aiobotocore_logs.type_defs import EmptyResponseMetadataTypeDef
from types_aiobotocore_logs.type_defs import AssociateKmsKeyRequestTypeDef


session = get_session()

async with session.create_client("logs") as client:
    client: CloudWatchLogsClient
    kwargs: AssociateKmsKeyRequestTypeDef = {...}
    result: EmptyResponseMetadataTypeDef = await client.associate_kms_key(**kwargs)
```



```python
# DescribeConfigurationTemplatesPaginator usage example with type annotations

from aiobotocore.session import get_session

from types_aiobotocore_logs.client import CloudWatchLogsClient
from types_aiobotocore_logs.paginator import DescribeConfigurationTemplatesPaginator
from types_aiobotocore_logs.type_defs import DescribeConfigurationTemplatesResponseTypeDef


session = get_session()

async with session.create_client("logs") as client:
    client: CloudWatchLogsClient
    paginator: DescribeConfigurationTemplatesPaginator = client.get_paginator("describe_configuration_templates")
    async for item in paginator.paginate(...):
        item: DescribeConfigurationTemplatesResponseTypeDef
        print(item)
```


