# Paginators

> [Index](../README.md) > [SNS](./README.md) > Paginators

!!! note ""

    Auto-generated documentation for [SNS](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sns.html#sns)
    type annotations stubs module [types-aiobotocore-sns](https://pypi.org/project/types-aiobotocore-sns/).

## ListEndpointsByPlatformApplicationPaginator

Type annotations and code completion for `#!python session.create_client("sns").get_paginator("list_endpoints_by_platform_application")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sns/paginator/ListEndpointsByPlatformApplication.html#SNS.Paginator.ListEndpointsByPlatformApplication)

```python
# ListEndpointsByPlatformApplicationPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_sns.paginator import ListEndpointsByPlatformApplicationPaginator

session = get_session()
async with session.create_client("sns") as client:  # (1)
    paginator: ListEndpointsByPlatformApplicationPaginator = client.get_paginator("list_endpoints_by_platform_application")  # (2)
    async for item in paginator.paginate(...):
        item: ListEndpointsByPlatformApplicationResponseTypeDef
        print(item)  # (3)
```

1. client: [SNSClient](./client.md)
2. paginator: [ListEndpointsByPlatformApplicationPaginator](./paginators.md#listendpointsbyplatformapplicationpaginator)
3. item: [:material-code-braces: ListEndpointsByPlatformApplicationResponseTypeDef](./type_defs.md#listendpointsbyplatformapplicationresponsetypedef) 


### paginate

Type annotations and code completion for `#!python ListEndpointsByPlatformApplicationPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    PlatformApplicationArn: str,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AioPageIterator[ListEndpointsByPlatformApplicationResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListEndpointsByPlatformApplicationResponseTypeDef](./type_defs.md#listendpointsbyplatformapplicationresponsetypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: ListEndpointsByPlatformApplicationInputPaginateTypeDef = {  # (1)
    "PlatformApplicationArn": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListEndpointsByPlatformApplicationInputPaginateTypeDef](./type_defs.md#listendpointsbyplatformapplicationinputpaginatetypedef) 
## ListOriginationNumbersPaginator

Type annotations and code completion for `#!python session.create_client("sns").get_paginator("list_origination_numbers")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sns/paginator/ListOriginationNumbers.html#SNS.Paginator.ListOriginationNumbers)

```python
# ListOriginationNumbersPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_sns.paginator import ListOriginationNumbersPaginator

session = get_session()
async with session.create_client("sns") as client:  # (1)
    paginator: ListOriginationNumbersPaginator = client.get_paginator("list_origination_numbers")  # (2)
    async for item in paginator.paginate(...):
        item: ListOriginationNumbersResultTypeDef
        print(item)  # (3)
```

1. client: [SNSClient](./client.md)
2. paginator: [ListOriginationNumbersPaginator](./paginators.md#listoriginationnumberspaginator)
3. item: [:material-code-braces: ListOriginationNumbersResultTypeDef](./type_defs.md#listoriginationnumbersresulttypedef) 


### paginate

Type annotations and code completion for `#!python ListOriginationNumbersPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AioPageIterator[ListOriginationNumbersResultTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListOriginationNumbersResultTypeDef](./type_defs.md#listoriginationnumbersresulttypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: ListOriginationNumbersRequestPaginateTypeDef = {  # (1)
    "PaginationConfig": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListOriginationNumbersRequestPaginateTypeDef](./type_defs.md#listoriginationnumbersrequestpaginatetypedef) 
## ListPhoneNumbersOptedOutPaginator

Type annotations and code completion for `#!python session.create_client("sns").get_paginator("list_phone_numbers_opted_out")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sns/paginator/ListPhoneNumbersOptedOut.html#SNS.Paginator.ListPhoneNumbersOptedOut)

```python
# ListPhoneNumbersOptedOutPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_sns.paginator import ListPhoneNumbersOptedOutPaginator

session = get_session()
async with session.create_client("sns") as client:  # (1)
    paginator: ListPhoneNumbersOptedOutPaginator = client.get_paginator("list_phone_numbers_opted_out")  # (2)
    async for item in paginator.paginate(...):
        item: ListPhoneNumbersOptedOutResponseTypeDef
        print(item)  # (3)
```

1. client: [SNSClient](./client.md)
2. paginator: [ListPhoneNumbersOptedOutPaginator](./paginators.md#listphonenumbersoptedoutpaginator)
3. item: [:material-code-braces: ListPhoneNumbersOptedOutResponseTypeDef](./type_defs.md#listphonenumbersoptedoutresponsetypedef) 


### paginate

Type annotations and code completion for `#!python ListPhoneNumbersOptedOutPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AioPageIterator[ListPhoneNumbersOptedOutResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListPhoneNumbersOptedOutResponseTypeDef](./type_defs.md#listphonenumbersoptedoutresponsetypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: ListPhoneNumbersOptedOutInputPaginateTypeDef = {  # (1)
    "PaginationConfig": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListPhoneNumbersOptedOutInputPaginateTypeDef](./type_defs.md#listphonenumbersoptedoutinputpaginatetypedef) 
## ListPlatformApplicationsPaginator

Type annotations and code completion for `#!python session.create_client("sns").get_paginator("list_platform_applications")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sns/paginator/ListPlatformApplications.html#SNS.Paginator.ListPlatformApplications)

```python
# ListPlatformApplicationsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_sns.paginator import ListPlatformApplicationsPaginator

session = get_session()
async with session.create_client("sns") as client:  # (1)
    paginator: ListPlatformApplicationsPaginator = client.get_paginator("list_platform_applications")  # (2)
    async for item in paginator.paginate(...):
        item: ListPlatformApplicationsResponseTypeDef
        print(item)  # (3)
```

1. client: [SNSClient](./client.md)
2. paginator: [ListPlatformApplicationsPaginator](./paginators.md#listplatformapplicationspaginator)
3. item: [:material-code-braces: ListPlatformApplicationsResponseTypeDef](./type_defs.md#listplatformapplicationsresponsetypedef) 


### paginate

Type annotations and code completion for `#!python ListPlatformApplicationsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AioPageIterator[ListPlatformApplicationsResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListPlatformApplicationsResponseTypeDef](./type_defs.md#listplatformapplicationsresponsetypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: ListPlatformApplicationsInputPaginateTypeDef = {  # (1)
    "PaginationConfig": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListPlatformApplicationsInputPaginateTypeDef](./type_defs.md#listplatformapplicationsinputpaginatetypedef) 
## ListSMSSandboxPhoneNumbersPaginator

Type annotations and code completion for `#!python session.create_client("sns").get_paginator("list_sms_sandbox_phone_numbers")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sns/paginator/ListSMSSandboxPhoneNumbers.html#SNS.Paginator.ListSMSSandboxPhoneNumbers)

```python
# ListSMSSandboxPhoneNumbersPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_sns.paginator import ListSMSSandboxPhoneNumbersPaginator

session = get_session()
async with session.create_client("sns") as client:  # (1)
    paginator: ListSMSSandboxPhoneNumbersPaginator = client.get_paginator("list_sms_sandbox_phone_numbers")  # (2)
    async for item in paginator.paginate(...):
        item: ListSMSSandboxPhoneNumbersResultTypeDef
        print(item)  # (3)
```

1. client: [SNSClient](./client.md)
2. paginator: [ListSMSSandboxPhoneNumbersPaginator](./paginators.md#listsmssandboxphonenumberspaginator)
3. item: [:material-code-braces: ListSMSSandboxPhoneNumbersResultTypeDef](./type_defs.md#listsmssandboxphonenumbersresulttypedef) 


### paginate

Type annotations and code completion for `#!python ListSMSSandboxPhoneNumbersPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AioPageIterator[ListSMSSandboxPhoneNumbersResultTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListSMSSandboxPhoneNumbersResultTypeDef](./type_defs.md#listsmssandboxphonenumbersresulttypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: ListSMSSandboxPhoneNumbersInputPaginateTypeDef = {  # (1)
    "PaginationConfig": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListSMSSandboxPhoneNumbersInputPaginateTypeDef](./type_defs.md#listsmssandboxphonenumbersinputpaginatetypedef) 
## ListSubscriptionsByTopicPaginator

Type annotations and code completion for `#!python session.create_client("sns").get_paginator("list_subscriptions_by_topic")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sns/paginator/ListSubscriptionsByTopic.html#SNS.Paginator.ListSubscriptionsByTopic)

```python
# ListSubscriptionsByTopicPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_sns.paginator import ListSubscriptionsByTopicPaginator

session = get_session()
async with session.create_client("sns") as client:  # (1)
    paginator: ListSubscriptionsByTopicPaginator = client.get_paginator("list_subscriptions_by_topic")  # (2)
    async for item in paginator.paginate(...):
        item: ListSubscriptionsByTopicResponseTypeDef
        print(item)  # (3)
```

1. client: [SNSClient](./client.md)
2. paginator: [ListSubscriptionsByTopicPaginator](./paginators.md#listsubscriptionsbytopicpaginator)
3. item: [:material-code-braces: ListSubscriptionsByTopicResponseTypeDef](./type_defs.md#listsubscriptionsbytopicresponsetypedef) 


### paginate

Type annotations and code completion for `#!python ListSubscriptionsByTopicPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    TopicArn: str,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AioPageIterator[ListSubscriptionsByTopicResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListSubscriptionsByTopicResponseTypeDef](./type_defs.md#listsubscriptionsbytopicresponsetypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: ListSubscriptionsByTopicInputPaginateTypeDef = {  # (1)
    "TopicArn": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListSubscriptionsByTopicInputPaginateTypeDef](./type_defs.md#listsubscriptionsbytopicinputpaginatetypedef) 
## ListSubscriptionsPaginator

Type annotations and code completion for `#!python session.create_client("sns").get_paginator("list_subscriptions")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sns/paginator/ListSubscriptions.html#SNS.Paginator.ListSubscriptions)

```python
# ListSubscriptionsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_sns.paginator import ListSubscriptionsPaginator

session = get_session()
async with session.create_client("sns") as client:  # (1)
    paginator: ListSubscriptionsPaginator = client.get_paginator("list_subscriptions")  # (2)
    async for item in paginator.paginate(...):
        item: ListSubscriptionsResponseTypeDef
        print(item)  # (3)
```

1. client: [SNSClient](./client.md)
2. paginator: [ListSubscriptionsPaginator](./paginators.md#listsubscriptionspaginator)
3. item: [:material-code-braces: ListSubscriptionsResponseTypeDef](./type_defs.md#listsubscriptionsresponsetypedef) 


### paginate

Type annotations and code completion for `#!python ListSubscriptionsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AioPageIterator[ListSubscriptionsResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListSubscriptionsResponseTypeDef](./type_defs.md#listsubscriptionsresponsetypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: ListSubscriptionsInputPaginateTypeDef = {  # (1)
    "PaginationConfig": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListSubscriptionsInputPaginateTypeDef](./type_defs.md#listsubscriptionsinputpaginatetypedef) 
## ListTopicsPaginator

Type annotations and code completion for `#!python session.create_client("sns").get_paginator("list_topics")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sns/paginator/ListTopics.html#SNS.Paginator.ListTopics)

```python
# ListTopicsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_sns.paginator import ListTopicsPaginator

session = get_session()
async with session.create_client("sns") as client:  # (1)
    paginator: ListTopicsPaginator = client.get_paginator("list_topics")  # (2)
    async for item in paginator.paginate(...):
        item: ListTopicsResponseTypeDef
        print(item)  # (3)
```

1. client: [SNSClient](./client.md)
2. paginator: [ListTopicsPaginator](./paginators.md#listtopicspaginator)
3. item: [:material-code-braces: ListTopicsResponseTypeDef](./type_defs.md#listtopicsresponsetypedef) 


### paginate

Type annotations and code completion for `#!python ListTopicsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AioPageIterator[ListTopicsResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListTopicsResponseTypeDef](./type_defs.md#listtopicsresponsetypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: ListTopicsInputPaginateTypeDef = {  # (1)
    "PaginationConfig": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListTopicsInputPaginateTypeDef](./type_defs.md#listtopicsinputpaginatetypedef) 
