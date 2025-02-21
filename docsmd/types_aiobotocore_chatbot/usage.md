# Examples

> [Index](../README.md) > [Chatbot](./README.md) > Examples

!!! note ""

    Auto-generated documentation for [Chatbot](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chatbot.html#chatbot)
    type annotations stubs module [types-aiobotocore-chatbot](https://pypi.org/project/types-aiobotocore-chatbot/).

## Client

### Implicit type annotations

Can be used with `types-aiobotocore[chatbot]` package installed.

Write your `Chatbot` code as usual,
type checking and code completion should work out of the box.



```python
# ChatbotClient usage example

from aiobotocore.session import get_session


session = get_session()

async with session.create_client("chatbot") as client:  # (1)
    result = await client.create_chime_webhook_configuration()  # (2)
```

1. client: [ChatbotClient](./client.md)
2. result: [:material-code-braces: CreateChimeWebhookConfigurationResultTypeDef](./type_defs.md#createchimewebhookconfigurationresulttypedef) 



```python
# DescribeChimeWebhookConfigurationsPaginator usage example

from aiobotocore.session import get_session


session = get_session()

async with session.create_client("chatbot") as client:  # (1)
    paginator = client.get_paginator("describe_chime_webhook_configurations")  # (2)
    async for item in paginator.paginate(...):
        print(item)  # (3)
```

1. client: [ChatbotClient](./client.md)
2. paginator: [DescribeChimeWebhookConfigurationsPaginator](./paginators.md#describechimewebhookconfigurationspaginator)
3. item: [:material-code-braces: DescribeChimeWebhookConfigurationsResultTypeDef](./type_defs.md#describechimewebhookconfigurationsresulttypedef) 




### Explicit type annotations

With `types-aiobotocore-lite[chatbot]`
or a standalone `types_aiobotocore_chatbot` package, you have to explicitly specify
`client: ChatbotClient` type annotation.

All other type annotations are optional, as types should be discovered automatically.
However, these type annotations can be helpful in your functions and methods.


```python
# ChatbotClient usage example with type annotations

from aiobotocore.session import get_session

from types_aiobotocore_chatbot.client import ChatbotClient
from types_aiobotocore_chatbot.type_defs import CreateChimeWebhookConfigurationResultTypeDef
from types_aiobotocore_chatbot.type_defs import CreateChimeWebhookConfigurationRequestTypeDef


session = get_session()

async with session.create_client("chatbot") as client:
    client: ChatbotClient
    kwargs: CreateChimeWebhookConfigurationRequestTypeDef = {...}
    result: CreateChimeWebhookConfigurationResultTypeDef = await client.create_chime_webhook_configuration(**kwargs)
```



```python
# DescribeChimeWebhookConfigurationsPaginator usage example with type annotations

from aiobotocore.session import get_session

from types_aiobotocore_chatbot.client import ChatbotClient
from types_aiobotocore_chatbot.paginator import DescribeChimeWebhookConfigurationsPaginator
from types_aiobotocore_chatbot.type_defs import DescribeChimeWebhookConfigurationsResultTypeDef


session = get_session()

async with session.create_client("chatbot") as client:
    client: ChatbotClient
    paginator: DescribeChimeWebhookConfigurationsPaginator = client.get_paginator("describe_chime_webhook_configurations")
    async for item in paginator.paginate(...):
        item: DescribeChimeWebhookConfigurationsResultTypeDef
        print(item)
```


