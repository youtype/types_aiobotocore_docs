# CodeStarNotifications module

> [Index](../README.md) > CodeStarNotifications


!!! note ""

    Auto-generated documentation for [CodeStarNotifications](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codestar-notifications.html#codestarnotifications)
    type annotations stubs module [types-aiobotocore-codestar-notifications](https://pypi.org/project/types-aiobotocore-codestar-notifications/).

## How to install

### Generate locally (recommended)

You can generate type annotations for `aiobotocore` package locally with `mypy-boto3-builder`.
Use [uv](https://docs.astral.sh/uv/getting-started/installation/) for build isolation.

1. Run mypy-boto3-builder in your package root directory: `uvx --with 'aiobotocore==3.1.1' mypy-boto3-builder`
1. Select `aiobotocore` AWS SDK.
1. Add `CodeStarNotifications` service.
1. Use provided commands to install generated packages.



### From PyPI with pip

Install `types-aiobotocore` for `CodeStarNotifications` service.

```bash
# install with aiobotocore type annotations
python -m pip install 'types-aiobotocore[codestar-notifications]'

# Lite version does not provide session.client/resource overloads
# it is more RAM-friendly, but requires explicit type annotations
python -m pip install 'types-aiobotocore-lite[codestar-notifications]'

# standalone installation
python -m pip install types-aiobotocore-codestar-notifications
```



## How to uninstall

```bash
python -m pip uninstall -y types-aiobotocore-codestar-notifications
```

## Usage

Code samples can be found in [Examples](./usage.md).

## CodeStarNotificationsClient

Type annotations and code completion for  `#!python session.create_client("codestar-notifications")` as [CodeStarNotificationsClient](./client.md)
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codestar-notifications.html#CodeStarNotifications.Client)

```python
# CodeStarNotificationsClient usage example

from aiobotocore.session import get_session

from types_aiobotocore_codestar_notifications.client import CodeStarNotificationsClient


session = get_session()
async with session.create_client("codestar-notifications") as client:
    client: CodeStarNotificationsClient
```


## Paginators

Type annotations and code completion for
[paginators](./paginators.md)
from `#!python session.create_client("codestar-notifications").get_paginator("...")`.

```python
# ListEventTypesPaginator usage example

from types_aiobotocore_codestar_notifications.paginator import ListEventTypesPaginator

def get_list_event_types_paginator() -> ListEventTypesPaginator:
    return client.get_paginator("list_event_types"))
```

- [ListEventTypesPaginator](./paginators.md#listeventtypespaginator)
- [ListNotificationRulesPaginator](./paginators.md#listnotificationrulespaginator)
- [ListTargetsPaginator](./paginators.md#listtargetspaginator)








## Literals

Type annotations for [literals](./literals.md) used in methods and schema.

```python
# DetailTypeType usage example

from types_aiobotocore_codestar_notifications.literals import DetailTypeType

def get_value() -> DetailTypeType:
    return "BASIC"
```

- [DetailTypeType](./literals.md#detailtypetype)
- [ListEventTypesFilterNameType](./literals.md#listeventtypesfilternametype)
- [ListEventTypesPaginatorName](./literals.md#listeventtypespaginatorname)
- [ListNotificationRulesFilterNameType](./literals.md#listnotificationrulesfilternametype)
- [ListNotificationRulesPaginatorName](./literals.md#listnotificationrulespaginatorname)
- [ListTargetsFilterNameType](./literals.md#listtargetsfilternametype)
- [ListTargetsPaginatorName](./literals.md#listtargetspaginatorname)
- [NotificationRuleStatusType](./literals.md#notificationrulestatustype)
- [TargetStatusType](./literals.md#targetstatustype)
- [CodeStarNotificationsServiceName](./literals.md#codestarnotificationsservicename)
- [ServiceName](./literals.md#servicename)
- [ResourceServiceName](./literals.md#resourceservicename)
- [PaginatorName](./literals.md#paginatorname)
- [RegionName](./literals.md#regionname)




## Type definitions

Type annotations for [type definitions](./type_defs.md) used in methods and schema.

- [TargetTypeDef](./type_defs.md#targettypedef)
- [ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef)
- [DeleteNotificationRuleRequestTypeDef](./type_defs.md#deletenotificationrulerequesttypedef)
- [DeleteTargetRequestTypeDef](./type_defs.md#deletetargetrequesttypedef)
- [DescribeNotificationRuleRequestTypeDef](./type_defs.md#describenotificationrulerequesttypedef)
- [EventTypeSummaryTypeDef](./type_defs.md#eventtypesummarytypedef)
- [TargetSummaryTypeDef](./type_defs.md#targetsummarytypedef)
- [ListEventTypesFilterTypeDef](./type_defs.md#listeventtypesfiltertypedef)
- [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
- [ListNotificationRulesFilterTypeDef](./type_defs.md#listnotificationrulesfiltertypedef)
- [NotificationRuleSummaryTypeDef](./type_defs.md#notificationrulesummarytypedef)
- [ListTagsForResourceRequestTypeDef](./type_defs.md#listtagsforresourcerequesttypedef)
- [ListTargetsFilterTypeDef](./type_defs.md#listtargetsfiltertypedef)
- [TagResourceRequestTypeDef](./type_defs.md#tagresourcerequesttypedef)
- [UnsubscribeRequestTypeDef](./type_defs.md#unsubscriberequesttypedef)
- [UntagResourceRequestTypeDef](./type_defs.md#untagresourcerequesttypedef)
- [CreateNotificationRuleRequestTypeDef](./type_defs.md#createnotificationrulerequesttypedef)
- [SubscribeRequestTypeDef](./type_defs.md#subscriberequesttypedef)
- [UpdateNotificationRuleRequestTypeDef](./type_defs.md#updatenotificationrulerequesttypedef)
- [CreateNotificationRuleResultTypeDef](./type_defs.md#createnotificationruleresulttypedef)
- [DeleteNotificationRuleResultTypeDef](./type_defs.md#deletenotificationruleresulttypedef)
- [ListTagsForResourceResultTypeDef](./type_defs.md#listtagsforresourceresulttypedef)
- [SubscribeResultTypeDef](./type_defs.md#subscriberesulttypedef)
- [TagResourceResultTypeDef](./type_defs.md#tagresourceresulttypedef)
- [UnsubscribeResultTypeDef](./type_defs.md#unsubscriberesulttypedef)
- [ListEventTypesResultTypeDef](./type_defs.md#listeventtypesresulttypedef)
- [DescribeNotificationRuleResultTypeDef](./type_defs.md#describenotificationruleresulttypedef)
- [ListTargetsResultTypeDef](./type_defs.md#listtargetsresulttypedef)
- [ListEventTypesRequestTypeDef](./type_defs.md#listeventtypesrequesttypedef)
- [ListEventTypesRequestPaginateTypeDef](./type_defs.md#listeventtypesrequestpaginatetypedef)
- [ListNotificationRulesRequestPaginateTypeDef](./type_defs.md#listnotificationrulesrequestpaginatetypedef)
- [ListNotificationRulesRequestTypeDef](./type_defs.md#listnotificationrulesrequesttypedef)
- [ListNotificationRulesResultTypeDef](./type_defs.md#listnotificationrulesresulttypedef)
- [ListTargetsRequestPaginateTypeDef](./type_defs.md#listtargetsrequestpaginatetypedef)
- [ListTargetsRequestTypeDef](./type_defs.md#listtargetsrequesttypedef)

