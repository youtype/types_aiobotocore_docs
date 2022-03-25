<a id="paginators-for-aiobotocore-sns-module"></a>

# Paginators for aiobotocore SNS module

> [Index](../README.md) > [SNS](./README.md) > Paginators

Auto-generated documentation for
[SNS](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sns.html#SNS)
type annotations stubs module
[types-aiobotocore-sns](https://pypi.org/project/types-aiobotocore-sns/).

- [Paginators for aiobotocore SNS module](#paginators-for-aiobotocore-sns-module)
  - [ListEndpointsByPlatformApplicationPaginator](#listendpointsbyplatformapplicationpaginator)
  - [ListOriginationNumbersPaginator](#listoriginationnumberspaginator)
  - [ListPhoneNumbersOptedOutPaginator](#listphonenumbersoptedoutpaginator)
  - [ListPlatformApplicationsPaginator](#listplatformapplicationspaginator)
  - [ListSMSSandboxPhoneNumbersPaginator](#listsmssandboxphonenumberspaginator)
  - [ListSubscriptionsPaginator](#listsubscriptionspaginator)
  - [ListSubscriptionsByTopicPaginator](#listsubscriptionsbytopicpaginator)
  - [ListTopicsPaginator](#listtopicspaginator)

<a id="listendpointsbyplatformapplicationpaginator"></a>

## ListEndpointsByPlatformApplicationPaginator

Type annotations for
`session.create_client("sns").get_paginator("list_endpoints_by_platform_application")`.

Can be used directly:

```python
from aiobotocore.session import get_session

from types_aiobotocore_sns.paginator import ListEndpointsByPlatformApplicationPaginator

session = get_session()
async with session.create_client("sns") as client:
    client: SNSClient
    paginator: ListEndpointsByPlatformApplicationPaginator = client.get_paginator("list_endpoints_by_platform_application")
```

Boto3 documentation:
[SNS.Paginator.ListEndpointsByPlatformApplication](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sns.html#SNS.Paginator.ListEndpointsByPlatformApplication)

Arguments for `ListEndpointsByPlatformApplicationPaginator.paginate` method:

- `PlatformApplicationArn`: `str` *(required)*
- `PaginationConfig`:
  [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)

`ListEndpointsByPlatformApplicationPaginator.paginate` returns
`AsyncIterator`\[[ListEndpointsByPlatformApplicationResponseTypeDef](./type_defs.md#listendpointsbyplatformapplicationresponsetypedef)\].

<a id="listoriginationnumberspaginator"></a>

## ListOriginationNumbersPaginator

Type annotations for
`session.create_client("sns").get_paginator("list_origination_numbers")`.

Can be used directly:

```python
from aiobotocore.session import get_session

from types_aiobotocore_sns.paginator import ListOriginationNumbersPaginator

session = get_session()
async with session.create_client("sns") as client:
    client: SNSClient
    paginator: ListOriginationNumbersPaginator = client.get_paginator("list_origination_numbers")
```

Boto3 documentation:
[SNS.Paginator.ListOriginationNumbers](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sns.html#SNS.Paginator.ListOriginationNumbers)

Arguments for `ListOriginationNumbersPaginator.paginate` method:

- `PaginationConfig`:
  [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)

`ListOriginationNumbersPaginator.paginate` returns
`AsyncIterator`\[[ListOriginationNumbersResultTypeDef](./type_defs.md#listoriginationnumbersresulttypedef)\].

<a id="listphonenumbersoptedoutpaginator"></a>

## ListPhoneNumbersOptedOutPaginator

Type annotations for
`session.create_client("sns").get_paginator("list_phone_numbers_opted_out")`.

Can be used directly:

```python
from aiobotocore.session import get_session

from types_aiobotocore_sns.paginator import ListPhoneNumbersOptedOutPaginator

session = get_session()
async with session.create_client("sns") as client:
    client: SNSClient
    paginator: ListPhoneNumbersOptedOutPaginator = client.get_paginator("list_phone_numbers_opted_out")
```

Boto3 documentation:
[SNS.Paginator.ListPhoneNumbersOptedOut](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sns.html#SNS.Paginator.ListPhoneNumbersOptedOut)

Arguments for `ListPhoneNumbersOptedOutPaginator.paginate` method:

- `PaginationConfig`:
  [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)

`ListPhoneNumbersOptedOutPaginator.paginate` returns
`AsyncIterator`\[[ListPhoneNumbersOptedOutResponseTypeDef](./type_defs.md#listphonenumbersoptedoutresponsetypedef)\].

<a id="listplatformapplicationspaginator"></a>

## ListPlatformApplicationsPaginator

Type annotations for
`session.create_client("sns").get_paginator("list_platform_applications")`.

Can be used directly:

```python
from aiobotocore.session import get_session

from types_aiobotocore_sns.paginator import ListPlatformApplicationsPaginator

session = get_session()
async with session.create_client("sns") as client:
    client: SNSClient
    paginator: ListPlatformApplicationsPaginator = client.get_paginator("list_platform_applications")
```

Boto3 documentation:
[SNS.Paginator.ListPlatformApplications](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sns.html#SNS.Paginator.ListPlatformApplications)

Arguments for `ListPlatformApplicationsPaginator.paginate` method:

- `PaginationConfig`:
  [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)

`ListPlatformApplicationsPaginator.paginate` returns
`AsyncIterator`\[[ListPlatformApplicationsResponseTypeDef](./type_defs.md#listplatformapplicationsresponsetypedef)\].

<a id="listsmssandboxphonenumberspaginator"></a>

## ListSMSSandboxPhoneNumbersPaginator

Type annotations for
`session.create_client("sns").get_paginator("list_sms_sandbox_phone_numbers")`.

Can be used directly:

```python
from aiobotocore.session import get_session

from types_aiobotocore_sns.paginator import ListSMSSandboxPhoneNumbersPaginator

session = get_session()
async with session.create_client("sns") as client:
    client: SNSClient
    paginator: ListSMSSandboxPhoneNumbersPaginator = client.get_paginator("list_sms_sandbox_phone_numbers")
```

Boto3 documentation:
[SNS.Paginator.ListSMSSandboxPhoneNumbers](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sns.html#SNS.Paginator.ListSMSSandboxPhoneNumbers)

Arguments for `ListSMSSandboxPhoneNumbersPaginator.paginate` method:

- `PaginationConfig`:
  [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)

`ListSMSSandboxPhoneNumbersPaginator.paginate` returns
`AsyncIterator`\[[ListSMSSandboxPhoneNumbersResultTypeDef](./type_defs.md#listsmssandboxphonenumbersresulttypedef)\].

<a id="listsubscriptionspaginator"></a>

## ListSubscriptionsPaginator

Type annotations for
`session.create_client("sns").get_paginator("list_subscriptions")`.

Can be used directly:

```python
from aiobotocore.session import get_session

from types_aiobotocore_sns.paginator import ListSubscriptionsPaginator

session = get_session()
async with session.create_client("sns") as client:
    client: SNSClient
    paginator: ListSubscriptionsPaginator = client.get_paginator("list_subscriptions")
```

Boto3 documentation:
[SNS.Paginator.ListSubscriptions](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sns.html#SNS.Paginator.ListSubscriptions)

Arguments for `ListSubscriptionsPaginator.paginate` method:

- `PaginationConfig`:
  [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)

`ListSubscriptionsPaginator.paginate` returns
`AsyncIterator`\[[ListSubscriptionsResponseTypeDef](./type_defs.md#listsubscriptionsresponsetypedef)\].

<a id="listsubscriptionsbytopicpaginator"></a>

## ListSubscriptionsByTopicPaginator

Type annotations for
`session.create_client("sns").get_paginator("list_subscriptions_by_topic")`.

Can be used directly:

```python
from aiobotocore.session import get_session

from types_aiobotocore_sns.paginator import ListSubscriptionsByTopicPaginator

session = get_session()
async with session.create_client("sns") as client:
    client: SNSClient
    paginator: ListSubscriptionsByTopicPaginator = client.get_paginator("list_subscriptions_by_topic")
```

Boto3 documentation:
[SNS.Paginator.ListSubscriptionsByTopic](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sns.html#SNS.Paginator.ListSubscriptionsByTopic)

Arguments for `ListSubscriptionsByTopicPaginator.paginate` method:

- `TopicArn`: `str` *(required)*
- `PaginationConfig`:
  [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)

`ListSubscriptionsByTopicPaginator.paginate` returns
`AsyncIterator`\[[ListSubscriptionsByTopicResponseTypeDef](./type_defs.md#listsubscriptionsbytopicresponsetypedef)\].

<a id="listtopicspaginator"></a>

## ListTopicsPaginator

Type annotations for
`session.create_client("sns").get_paginator("list_topics")`.

Can be used directly:

```python
from aiobotocore.session import get_session

from types_aiobotocore_sns.paginator import ListTopicsPaginator

session = get_session()
async with session.create_client("sns") as client:
    client: SNSClient
    paginator: ListTopicsPaginator = client.get_paginator("list_topics")
```

Boto3 documentation:
[SNS.Paginator.ListTopics](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sns.html#SNS.Paginator.ListTopics)

Arguments for `ListTopicsPaginator.paginate` method:

- `PaginationConfig`:
  [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)

`ListTopicsPaginator.paginate` returns
`AsyncIterator`\[[ListTopicsResponseTypeDef](./type_defs.md#listtopicsresponsetypedef)\].