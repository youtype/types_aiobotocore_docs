<a id="paginators-for-aiobotocore-iot-module"></a>

# Paginators for aiobotocore IoT module

> [Index](..) > [IoT](.) > Paginators

Auto-generated documentation for
[IoT](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot.html#IoT)
type annotations stubs module
[types-aiobotocore-iot](https://pypi.org/project/types-aiobotocore-iot/).

- [Paginators for aiobotocore IoT module](#paginators-for-aiobotocore-iot-module)
  - [GetBehaviorModelTrainingSummariesPaginator](#getbehaviormodeltrainingsummariespaginator)
  - [ListActiveViolationsPaginator](#listactiveviolationspaginator)
  - [ListAttachedPoliciesPaginator](#listattachedpoliciespaginator)
  - [ListAuditFindingsPaginator](#listauditfindingspaginator)
  - [ListAuditMitigationActionsExecutionsPaginator](#listauditmitigationactionsexecutionspaginator)
  - [ListAuditMitigationActionsTasksPaginator](#listauditmitigationactionstaskspaginator)
  - [ListAuditSuppressionsPaginator](#listauditsuppressionspaginator)
  - [ListAuditTasksPaginator](#listaudittaskspaginator)
  - [ListAuthorizersPaginator](#listauthorizerspaginator)
  - [ListBillingGroupsPaginator](#listbillinggroupspaginator)
  - [ListCACertificatesPaginator](#listcacertificatespaginator)
  - [ListCertificatesPaginator](#listcertificatespaginator)
  - [ListCertificatesByCAPaginator](#listcertificatesbycapaginator)
  - [ListCustomMetricsPaginator](#listcustommetricspaginator)
  - [ListDetectMitigationActionsExecutionsPaginator](#listdetectmitigationactionsexecutionspaginator)
  - [ListDetectMitigationActionsTasksPaginator](#listdetectmitigationactionstaskspaginator)
  - [ListDimensionsPaginator](#listdimensionspaginator)
  - [ListDomainConfigurationsPaginator](#listdomainconfigurationspaginator)
  - [ListFleetMetricsPaginator](#listfleetmetricspaginator)
  - [ListIndicesPaginator](#listindicespaginator)
  - [ListJobExecutionsForJobPaginator](#listjobexecutionsforjobpaginator)
  - [ListJobExecutionsForThingPaginator](#listjobexecutionsforthingpaginator)
  - [ListJobTemplatesPaginator](#listjobtemplatespaginator)
  - [ListJobsPaginator](#listjobspaginator)
  - [ListMitigationActionsPaginator](#listmitigationactionspaginator)
  - [ListOTAUpdatesPaginator](#listotaupdatespaginator)
  - [ListOutgoingCertificatesPaginator](#listoutgoingcertificatespaginator)
  - [ListPoliciesPaginator](#listpoliciespaginator)
  - [ListPolicyPrincipalsPaginator](#listpolicyprincipalspaginator)
  - [ListPrincipalPoliciesPaginator](#listprincipalpoliciespaginator)
  - [ListPrincipalThingsPaginator](#listprincipalthingspaginator)
  - [ListProvisioningTemplateVersionsPaginator](#listprovisioningtemplateversionspaginator)
  - [ListProvisioningTemplatesPaginator](#listprovisioningtemplatespaginator)
  - [ListRoleAliasesPaginator](#listrolealiasespaginator)
  - [ListScheduledAuditsPaginator](#listscheduledauditspaginator)
  - [ListSecurityProfilesPaginator](#listsecurityprofilespaginator)
  - [ListSecurityProfilesForTargetPaginator](#listsecurityprofilesfortargetpaginator)
  - [ListStreamsPaginator](#liststreamspaginator)
  - [ListTagsForResourcePaginator](#listtagsforresourcepaginator)
  - [ListTargetsForPolicyPaginator](#listtargetsforpolicypaginator)
  - [ListTargetsForSecurityProfilePaginator](#listtargetsforsecurityprofilepaginator)
  - [ListThingGroupsPaginator](#listthinggroupspaginator)
  - [ListThingGroupsForThingPaginator](#listthinggroupsforthingpaginator)
  - [ListThingPrincipalsPaginator](#listthingprincipalspaginator)
  - [ListThingRegistrationTaskReportsPaginator](#listthingregistrationtaskreportspaginator)
  - [ListThingRegistrationTasksPaginator](#listthingregistrationtaskspaginator)
  - [ListThingTypesPaginator](#listthingtypespaginator)
  - [ListThingsPaginator](#listthingspaginator)
  - [ListThingsInBillingGroupPaginator](#listthingsinbillinggrouppaginator)
  - [ListThingsInThingGroupPaginator](#listthingsinthinggrouppaginator)
  - [ListTopicRuleDestinationsPaginator](#listtopicruledestinationspaginator)
  - [ListTopicRulesPaginator](#listtopicrulespaginator)
  - [ListV2LoggingLevelsPaginator](#listv2logginglevelspaginator)
  - [ListViolationEventsPaginator](#listviolationeventspaginator)

<a id="getbehaviormodeltrainingsummariespaginator"></a>

## GetBehaviorModelTrainingSummariesPaginator

Type annotations for
`session.create_client("iot").get_paginator("get_behavior_model_training_summaries")`.

Can be used directly:

```python
from aiobotocore.session import get_session

from types_aiobotocore_iot.paginator import GetBehaviorModelTrainingSummariesPaginator

session = get_session()
async with session.create_client("iot") as client:
    client: IoTClient
    paginator: GetBehaviorModelTrainingSummariesPaginator = client.get_paginator("get_behavior_model_training_summaries")
```

Boto3 documentation:
[IoT.Paginator.GetBehaviorModelTrainingSummaries](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot.html#IoT.Paginator.GetBehaviorModelTrainingSummaries)

Arguments for `GetBehaviorModelTrainingSummariesPaginator.paginate` method:

- `securityProfileName`: `str`
- `PaginationConfig`:
  [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)

`GetBehaviorModelTrainingSummariesPaginator.paginate` returns
`AsyncIterable`\[[GetBehaviorModelTrainingSummariesResponseTypeDef](./type_defs.md#getbehaviormodeltrainingsummariesresponsetypedef)\].

<a id="listactiveviolationspaginator"></a>

## ListActiveViolationsPaginator

Type annotations for
`session.create_client("iot").get_paginator("list_active_violations")`.

Can be used directly:

```python
from aiobotocore.session import get_session

from types_aiobotocore_iot.paginator import ListActiveViolationsPaginator

session = get_session()
async with session.create_client("iot") as client:
    client: IoTClient
    paginator: ListActiveViolationsPaginator = client.get_paginator("list_active_violations")
```

Boto3 documentation:
[IoT.Paginator.ListActiveViolations](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot.html#IoT.Paginator.ListActiveViolations)

Arguments for `ListActiveViolationsPaginator.paginate` method:

- `thingName`: `str`
- `securityProfileName`: `str`
- `behaviorCriteriaType`:
  [BehaviorCriteriaTypeType](./literals.md#behaviorcriteriatypetype)
- `listSuppressedAlerts`: `bool`
- `verificationState`:
  [VerificationStateType](./literals.md#verificationstatetype)
- `PaginationConfig`:
  [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)

`ListActiveViolationsPaginator.paginate` returns
`AsyncIterable`\[[ListActiveViolationsResponseTypeDef](./type_defs.md#listactiveviolationsresponsetypedef)\].

<a id="listattachedpoliciespaginator"></a>

## ListAttachedPoliciesPaginator

Type annotations for
`session.create_client("iot").get_paginator("list_attached_policies")`.

Can be used directly:

```python
from aiobotocore.session import get_session

from types_aiobotocore_iot.paginator import ListAttachedPoliciesPaginator

session = get_session()
async with session.create_client("iot") as client:
    client: IoTClient
    paginator: ListAttachedPoliciesPaginator = client.get_paginator("list_attached_policies")
```

Boto3 documentation:
[IoT.Paginator.ListAttachedPolicies](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot.html#IoT.Paginator.ListAttachedPolicies)

Arguments for `ListAttachedPoliciesPaginator.paginate` method:

- `target`: `str` *(required)*
- `recursive`: `bool`
- `PaginationConfig`:
  [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)

`ListAttachedPoliciesPaginator.paginate` returns
`AsyncIterable`\[[ListAttachedPoliciesResponseTypeDef](./type_defs.md#listattachedpoliciesresponsetypedef)\].

<a id="listauditfindingspaginator"></a>

## ListAuditFindingsPaginator

Type annotations for
`session.create_client("iot").get_paginator("list_audit_findings")`.

Can be used directly:

```python
from aiobotocore.session import get_session

from types_aiobotocore_iot.paginator import ListAuditFindingsPaginator

session = get_session()
async with session.create_client("iot") as client:
    client: IoTClient
    paginator: ListAuditFindingsPaginator = client.get_paginator("list_audit_findings")
```

Boto3 documentation:
[IoT.Paginator.ListAuditFindings](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot.html#IoT.Paginator.ListAuditFindings)

Arguments for `ListAuditFindingsPaginator.paginate` method:

- `taskId`: `str`
- `checkName`: `str`
- `resourceIdentifier`:
  [ResourceIdentifierTypeDef](./type_defs.md#resourceidentifiertypedef)
- `startTime`: `Union`\[`datetime`, `str`\]
- `endTime`: `Union`\[`datetime`, `str`\]
- `listSuppressedFindings`: `bool`
- `PaginationConfig`:
  [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)

`ListAuditFindingsPaginator.paginate` returns
`AsyncIterable`\[[ListAuditFindingsResponseTypeDef](./type_defs.md#listauditfindingsresponsetypedef)\].

<a id="listauditmitigationactionsexecutionspaginator"></a>

## ListAuditMitigationActionsExecutionsPaginator

Type annotations for
`session.create_client("iot").get_paginator("list_audit_mitigation_actions_executions")`.

Can be used directly:

```python
from aiobotocore.session import get_session

from types_aiobotocore_iot.paginator import ListAuditMitigationActionsExecutionsPaginator

session = get_session()
async with session.create_client("iot") as client:
    client: IoTClient
    paginator: ListAuditMitigationActionsExecutionsPaginator = client.get_paginator("list_audit_mitigation_actions_executions")
```

Boto3 documentation:
[IoT.Paginator.ListAuditMitigationActionsExecutions](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot.html#IoT.Paginator.ListAuditMitigationActionsExecutions)

Arguments for `ListAuditMitigationActionsExecutionsPaginator.paginate` method:

- `taskId`: `str` *(required)*
- `findingId`: `str` *(required)*
- `actionStatus`:
  [AuditMitigationActionsExecutionStatusType](./literals.md#auditmitigationactionsexecutionstatustype)
- `PaginationConfig`:
  [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)

`ListAuditMitigationActionsExecutionsPaginator.paginate` returns
`AsyncIterable`\[[ListAuditMitigationActionsExecutionsResponseTypeDef](./type_defs.md#listauditmitigationactionsexecutionsresponsetypedef)\].

<a id="listauditmitigationactionstaskspaginator"></a>

## ListAuditMitigationActionsTasksPaginator

Type annotations for
`session.create_client("iot").get_paginator("list_audit_mitigation_actions_tasks")`.

Can be used directly:

```python
from aiobotocore.session import get_session

from types_aiobotocore_iot.paginator import ListAuditMitigationActionsTasksPaginator

session = get_session()
async with session.create_client("iot") as client:
    client: IoTClient
    paginator: ListAuditMitigationActionsTasksPaginator = client.get_paginator("list_audit_mitigation_actions_tasks")
```

Boto3 documentation:
[IoT.Paginator.ListAuditMitigationActionsTasks](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot.html#IoT.Paginator.ListAuditMitigationActionsTasks)

Arguments for `ListAuditMitigationActionsTasksPaginator.paginate` method:

- `startTime`: `Union`\[`datetime`, `str`\] *(required)*
- `endTime`: `Union`\[`datetime`, `str`\] *(required)*
- `auditTaskId`: `str`
- `findingId`: `str`
- `taskStatus`:
  [AuditMitigationActionsTaskStatusType](./literals.md#auditmitigationactionstaskstatustype)
- `PaginationConfig`:
  [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)

`ListAuditMitigationActionsTasksPaginator.paginate` returns
`AsyncIterable`\[[ListAuditMitigationActionsTasksResponseTypeDef](./type_defs.md#listauditmitigationactionstasksresponsetypedef)\].

<a id="listauditsuppressionspaginator"></a>

## ListAuditSuppressionsPaginator

Type annotations for
`session.create_client("iot").get_paginator("list_audit_suppressions")`.

Can be used directly:

```python
from aiobotocore.session import get_session

from types_aiobotocore_iot.paginator import ListAuditSuppressionsPaginator

session = get_session()
async with session.create_client("iot") as client:
    client: IoTClient
    paginator: ListAuditSuppressionsPaginator = client.get_paginator("list_audit_suppressions")
```

Boto3 documentation:
[IoT.Paginator.ListAuditSuppressions](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot.html#IoT.Paginator.ListAuditSuppressions)

Arguments for `ListAuditSuppressionsPaginator.paginate` method:

- `checkName`: `str`
- `resourceIdentifier`:
  [ResourceIdentifierTypeDef](./type_defs.md#resourceidentifiertypedef)
- `ascendingOrder`: `bool`
- `PaginationConfig`:
  [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)

`ListAuditSuppressionsPaginator.paginate` returns
`AsyncIterable`\[[ListAuditSuppressionsResponseTypeDef](./type_defs.md#listauditsuppressionsresponsetypedef)\].

<a id="listaudittaskspaginator"></a>

## ListAuditTasksPaginator

Type annotations for
`session.create_client("iot").get_paginator("list_audit_tasks")`.

Can be used directly:

```python
from aiobotocore.session import get_session

from types_aiobotocore_iot.paginator import ListAuditTasksPaginator

session = get_session()
async with session.create_client("iot") as client:
    client: IoTClient
    paginator: ListAuditTasksPaginator = client.get_paginator("list_audit_tasks")
```

Boto3 documentation:
[IoT.Paginator.ListAuditTasks](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot.html#IoT.Paginator.ListAuditTasks)

Arguments for `ListAuditTasksPaginator.paginate` method:

- `startTime`: `Union`\[`datetime`, `str`\] *(required)*
- `endTime`: `Union`\[`datetime`, `str`\] *(required)*
- `taskType`: [AuditTaskTypeType](./literals.md#audittasktypetype)
- `taskStatus`: [AuditTaskStatusType](./literals.md#audittaskstatustype)
- `PaginationConfig`:
  [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)

`ListAuditTasksPaginator.paginate` returns
`AsyncIterable`\[[ListAuditTasksResponseTypeDef](./type_defs.md#listaudittasksresponsetypedef)\].

<a id="listauthorizerspaginator"></a>

## ListAuthorizersPaginator

Type annotations for
`session.create_client("iot").get_paginator("list_authorizers")`.

Can be used directly:

```python
from aiobotocore.session import get_session

from types_aiobotocore_iot.paginator import ListAuthorizersPaginator

session = get_session()
async with session.create_client("iot") as client:
    client: IoTClient
    paginator: ListAuthorizersPaginator = client.get_paginator("list_authorizers")
```

Boto3 documentation:
[IoT.Paginator.ListAuthorizers](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot.html#IoT.Paginator.ListAuthorizers)

Arguments for `ListAuthorizersPaginator.paginate` method:

- `ascendingOrder`: `bool`
- `status`: [AuthorizerStatusType](./literals.md#authorizerstatustype)
- `PaginationConfig`:
  [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)

`ListAuthorizersPaginator.paginate` returns
`AsyncIterable`\[[ListAuthorizersResponseTypeDef](./type_defs.md#listauthorizersresponsetypedef)\].

<a id="listbillinggroupspaginator"></a>

## ListBillingGroupsPaginator

Type annotations for
`session.create_client("iot").get_paginator("list_billing_groups")`.

Can be used directly:

```python
from aiobotocore.session import get_session

from types_aiobotocore_iot.paginator import ListBillingGroupsPaginator

session = get_session()
async with session.create_client("iot") as client:
    client: IoTClient
    paginator: ListBillingGroupsPaginator = client.get_paginator("list_billing_groups")
```

Boto3 documentation:
[IoT.Paginator.ListBillingGroups](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot.html#IoT.Paginator.ListBillingGroups)

Arguments for `ListBillingGroupsPaginator.paginate` method:

- `namePrefixFilter`: `str`
- `PaginationConfig`:
  [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)

`ListBillingGroupsPaginator.paginate` returns
`AsyncIterable`\[[ListBillingGroupsResponseTypeDef](./type_defs.md#listbillinggroupsresponsetypedef)\].

<a id="listcacertificatespaginator"></a>

## ListCACertificatesPaginator

Type annotations for
`session.create_client("iot").get_paginator("list_ca_certificates")`.

Can be used directly:

```python
from aiobotocore.session import get_session

from types_aiobotocore_iot.paginator import ListCACertificatesPaginator

session = get_session()
async with session.create_client("iot") as client:
    client: IoTClient
    paginator: ListCACertificatesPaginator = client.get_paginator("list_ca_certificates")
```

Boto3 documentation:
[IoT.Paginator.ListCACertificates](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot.html#IoT.Paginator.ListCACertificates)

Arguments for `ListCACertificatesPaginator.paginate` method:

- `ascendingOrder`: `bool`
- `PaginationConfig`:
  [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)

`ListCACertificatesPaginator.paginate` returns
`AsyncIterable`\[[ListCACertificatesResponseTypeDef](./type_defs.md#listcacertificatesresponsetypedef)\].

<a id="listcertificatespaginator"></a>

## ListCertificatesPaginator

Type annotations for
`session.create_client("iot").get_paginator("list_certificates")`.

Can be used directly:

```python
from aiobotocore.session import get_session

from types_aiobotocore_iot.paginator import ListCertificatesPaginator

session = get_session()
async with session.create_client("iot") as client:
    client: IoTClient
    paginator: ListCertificatesPaginator = client.get_paginator("list_certificates")
```

Boto3 documentation:
[IoT.Paginator.ListCertificates](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot.html#IoT.Paginator.ListCertificates)

Arguments for `ListCertificatesPaginator.paginate` method:

- `ascendingOrder`: `bool`
- `PaginationConfig`:
  [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)

`ListCertificatesPaginator.paginate` returns
`AsyncIterable`\[[ListCertificatesResponseTypeDef](./type_defs.md#listcertificatesresponsetypedef)\].

<a id="listcertificatesbycapaginator"></a>

## ListCertificatesByCAPaginator

Type annotations for
`session.create_client("iot").get_paginator("list_certificates_by_ca")`.

Can be used directly:

```python
from aiobotocore.session import get_session

from types_aiobotocore_iot.paginator import ListCertificatesByCAPaginator

session = get_session()
async with session.create_client("iot") as client:
    client: IoTClient
    paginator: ListCertificatesByCAPaginator = client.get_paginator("list_certificates_by_ca")
```

Boto3 documentation:
[IoT.Paginator.ListCertificatesByCA](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot.html#IoT.Paginator.ListCertificatesByCA)

Arguments for `ListCertificatesByCAPaginator.paginate` method:

- `caCertificateId`: `str` *(required)*
- `ascendingOrder`: `bool`
- `PaginationConfig`:
  [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)

`ListCertificatesByCAPaginator.paginate` returns
`AsyncIterable`\[[ListCertificatesByCAResponseTypeDef](./type_defs.md#listcertificatesbycaresponsetypedef)\].

<a id="listcustommetricspaginator"></a>

## ListCustomMetricsPaginator

Type annotations for
`session.create_client("iot").get_paginator("list_custom_metrics")`.

Can be used directly:

```python
from aiobotocore.session import get_session

from types_aiobotocore_iot.paginator import ListCustomMetricsPaginator

session = get_session()
async with session.create_client("iot") as client:
    client: IoTClient
    paginator: ListCustomMetricsPaginator = client.get_paginator("list_custom_metrics")
```

Boto3 documentation:
[IoT.Paginator.ListCustomMetrics](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot.html#IoT.Paginator.ListCustomMetrics)

Arguments for `ListCustomMetricsPaginator.paginate` method:

- `PaginationConfig`:
  [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)

`ListCustomMetricsPaginator.paginate` returns
`AsyncIterable`\[[ListCustomMetricsResponseTypeDef](./type_defs.md#listcustommetricsresponsetypedef)\].

<a id="listdetectmitigationactionsexecutionspaginator"></a>

## ListDetectMitigationActionsExecutionsPaginator

Type annotations for
`session.create_client("iot").get_paginator("list_detect_mitigation_actions_executions")`.

Can be used directly:

```python
from aiobotocore.session import get_session

from types_aiobotocore_iot.paginator import ListDetectMitigationActionsExecutionsPaginator

session = get_session()
async with session.create_client("iot") as client:
    client: IoTClient
    paginator: ListDetectMitigationActionsExecutionsPaginator = client.get_paginator("list_detect_mitigation_actions_executions")
```

Boto3 documentation:
[IoT.Paginator.ListDetectMitigationActionsExecutions](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot.html#IoT.Paginator.ListDetectMitigationActionsExecutions)

Arguments for `ListDetectMitigationActionsExecutionsPaginator.paginate` method:

- `taskId`: `str`
- `violationId`: `str`
- `thingName`: `str`
- `startTime`: `Union`\[`datetime`, `str`\]
- `endTime`: `Union`\[`datetime`, `str`\]
- `PaginationConfig`:
  [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)

`ListDetectMitigationActionsExecutionsPaginator.paginate` returns
`AsyncIterable`\[[ListDetectMitigationActionsExecutionsResponseTypeDef](./type_defs.md#listdetectmitigationactionsexecutionsresponsetypedef)\].

<a id="listdetectmitigationactionstaskspaginator"></a>

## ListDetectMitigationActionsTasksPaginator

Type annotations for
`session.create_client("iot").get_paginator("list_detect_mitigation_actions_tasks")`.

Can be used directly:

```python
from aiobotocore.session import get_session

from types_aiobotocore_iot.paginator import ListDetectMitigationActionsTasksPaginator

session = get_session()
async with session.create_client("iot") as client:
    client: IoTClient
    paginator: ListDetectMitigationActionsTasksPaginator = client.get_paginator("list_detect_mitigation_actions_tasks")
```

Boto3 documentation:
[IoT.Paginator.ListDetectMitigationActionsTasks](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot.html#IoT.Paginator.ListDetectMitigationActionsTasks)

Arguments for `ListDetectMitigationActionsTasksPaginator.paginate` method:

- `startTime`: `Union`\[`datetime`, `str`\] *(required)*
- `endTime`: `Union`\[`datetime`, `str`\] *(required)*
- `PaginationConfig`:
  [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)

`ListDetectMitigationActionsTasksPaginator.paginate` returns
`AsyncIterable`\[[ListDetectMitigationActionsTasksResponseTypeDef](./type_defs.md#listdetectmitigationactionstasksresponsetypedef)\].

<a id="listdimensionspaginator"></a>

## ListDimensionsPaginator

Type annotations for
`session.create_client("iot").get_paginator("list_dimensions")`.

Can be used directly:

```python
from aiobotocore.session import get_session

from types_aiobotocore_iot.paginator import ListDimensionsPaginator

session = get_session()
async with session.create_client("iot") as client:
    client: IoTClient
    paginator: ListDimensionsPaginator = client.get_paginator("list_dimensions")
```

Boto3 documentation:
[IoT.Paginator.ListDimensions](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot.html#IoT.Paginator.ListDimensions)

Arguments for `ListDimensionsPaginator.paginate` method:

- `PaginationConfig`:
  [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)

`ListDimensionsPaginator.paginate` returns
`AsyncIterable`\[[ListDimensionsResponseTypeDef](./type_defs.md#listdimensionsresponsetypedef)\].

<a id="listdomainconfigurationspaginator"></a>

## ListDomainConfigurationsPaginator

Type annotations for
`session.create_client("iot").get_paginator("list_domain_configurations")`.

Can be used directly:

```python
from aiobotocore.session import get_session

from types_aiobotocore_iot.paginator import ListDomainConfigurationsPaginator

session = get_session()
async with session.create_client("iot") as client:
    client: IoTClient
    paginator: ListDomainConfigurationsPaginator = client.get_paginator("list_domain_configurations")
```

Boto3 documentation:
[IoT.Paginator.ListDomainConfigurations](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot.html#IoT.Paginator.ListDomainConfigurations)

Arguments for `ListDomainConfigurationsPaginator.paginate` method:

- `serviceType`: [ServiceTypeType](./literals.md#servicetypetype)
- `PaginationConfig`:
  [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)

`ListDomainConfigurationsPaginator.paginate` returns
`AsyncIterable`\[[ListDomainConfigurationsResponseTypeDef](./type_defs.md#listdomainconfigurationsresponsetypedef)\].

<a id="listfleetmetricspaginator"></a>

## ListFleetMetricsPaginator

Type annotations for
`session.create_client("iot").get_paginator("list_fleet_metrics")`.

Can be used directly:

```python
from aiobotocore.session import get_session

from types_aiobotocore_iot.paginator import ListFleetMetricsPaginator

session = get_session()
async with session.create_client("iot") as client:
    client: IoTClient
    paginator: ListFleetMetricsPaginator = client.get_paginator("list_fleet_metrics")
```

Boto3 documentation:
[IoT.Paginator.ListFleetMetrics](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot.html#IoT.Paginator.ListFleetMetrics)

Arguments for `ListFleetMetricsPaginator.paginate` method:

- `PaginationConfig`:
  [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)

`ListFleetMetricsPaginator.paginate` returns
`AsyncIterable`\[[ListFleetMetricsResponseTypeDef](./type_defs.md#listfleetmetricsresponsetypedef)\].

<a id="listindicespaginator"></a>

## ListIndicesPaginator

Type annotations for
`session.create_client("iot").get_paginator("list_indices")`.

Can be used directly:

```python
from aiobotocore.session import get_session

from types_aiobotocore_iot.paginator import ListIndicesPaginator

session = get_session()
async with session.create_client("iot") as client:
    client: IoTClient
    paginator: ListIndicesPaginator = client.get_paginator("list_indices")
```

Boto3 documentation:
[IoT.Paginator.ListIndices](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot.html#IoT.Paginator.ListIndices)

Arguments for `ListIndicesPaginator.paginate` method:

- `PaginationConfig`:
  [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)

`ListIndicesPaginator.paginate` returns
`AsyncIterable`\[[ListIndicesResponseTypeDef](./type_defs.md#listindicesresponsetypedef)\].

<a id="listjobexecutionsforjobpaginator"></a>

## ListJobExecutionsForJobPaginator

Type annotations for
`session.create_client("iot").get_paginator("list_job_executions_for_job")`.

Can be used directly:

```python
from aiobotocore.session import get_session

from types_aiobotocore_iot.paginator import ListJobExecutionsForJobPaginator

session = get_session()
async with session.create_client("iot") as client:
    client: IoTClient
    paginator: ListJobExecutionsForJobPaginator = client.get_paginator("list_job_executions_for_job")
```

Boto3 documentation:
[IoT.Paginator.ListJobExecutionsForJob](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot.html#IoT.Paginator.ListJobExecutionsForJob)

Arguments for `ListJobExecutionsForJobPaginator.paginate` method:

- `jobId`: `str` *(required)*
- `status`: [JobExecutionStatusType](./literals.md#jobexecutionstatustype)
- `PaginationConfig`:
  [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)

`ListJobExecutionsForJobPaginator.paginate` returns
`AsyncIterable`\[[ListJobExecutionsForJobResponseTypeDef](./type_defs.md#listjobexecutionsforjobresponsetypedef)\].

<a id="listjobexecutionsforthingpaginator"></a>

## ListJobExecutionsForThingPaginator

Type annotations for
`session.create_client("iot").get_paginator("list_job_executions_for_thing")`.

Can be used directly:

```python
from aiobotocore.session import get_session

from types_aiobotocore_iot.paginator import ListJobExecutionsForThingPaginator

session = get_session()
async with session.create_client("iot") as client:
    client: IoTClient
    paginator: ListJobExecutionsForThingPaginator = client.get_paginator("list_job_executions_for_thing")
```

Boto3 documentation:
[IoT.Paginator.ListJobExecutionsForThing](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot.html#IoT.Paginator.ListJobExecutionsForThing)

Arguments for `ListJobExecutionsForThingPaginator.paginate` method:

- `thingName`: `str` *(required)*
- `status`: [JobExecutionStatusType](./literals.md#jobexecutionstatustype)
- `namespaceId`: `str`
- `PaginationConfig`:
  [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)

`ListJobExecutionsForThingPaginator.paginate` returns
`AsyncIterable`\[[ListJobExecutionsForThingResponseTypeDef](./type_defs.md#listjobexecutionsforthingresponsetypedef)\].

<a id="listjobtemplatespaginator"></a>

## ListJobTemplatesPaginator

Type annotations for
`session.create_client("iot").get_paginator("list_job_templates")`.

Can be used directly:

```python
from aiobotocore.session import get_session

from types_aiobotocore_iot.paginator import ListJobTemplatesPaginator

session = get_session()
async with session.create_client("iot") as client:
    client: IoTClient
    paginator: ListJobTemplatesPaginator = client.get_paginator("list_job_templates")
```

Boto3 documentation:
[IoT.Paginator.ListJobTemplates](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot.html#IoT.Paginator.ListJobTemplates)

Arguments for `ListJobTemplatesPaginator.paginate` method:

- `PaginationConfig`:
  [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)

`ListJobTemplatesPaginator.paginate` returns
`AsyncIterable`\[[ListJobTemplatesResponseTypeDef](./type_defs.md#listjobtemplatesresponsetypedef)\].

<a id="listjobspaginator"></a>

## ListJobsPaginator

Type annotations for `session.create_client("iot").get_paginator("list_jobs")`.

Can be used directly:

```python
from aiobotocore.session import get_session

from types_aiobotocore_iot.paginator import ListJobsPaginator

session = get_session()
async with session.create_client("iot") as client:
    client: IoTClient
    paginator: ListJobsPaginator = client.get_paginator("list_jobs")
```

Boto3 documentation:
[IoT.Paginator.ListJobs](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot.html#IoT.Paginator.ListJobs)

Arguments for `ListJobsPaginator.paginate` method:

- `status`: [JobStatusType](./literals.md#jobstatustype)
- `targetSelection`: [TargetSelectionType](./literals.md#targetselectiontype)
- `thingGroupName`: `str`
- `thingGroupId`: `str`
- `namespaceId`: `str`
- `PaginationConfig`:
  [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)

`ListJobsPaginator.paginate` returns
`AsyncIterable`\[[ListJobsResponseTypeDef](./type_defs.md#listjobsresponsetypedef)\].

<a id="listmitigationactionspaginator"></a>

## ListMitigationActionsPaginator

Type annotations for
`session.create_client("iot").get_paginator("list_mitigation_actions")`.

Can be used directly:

```python
from aiobotocore.session import get_session

from types_aiobotocore_iot.paginator import ListMitigationActionsPaginator

session = get_session()
async with session.create_client("iot") as client:
    client: IoTClient
    paginator: ListMitigationActionsPaginator = client.get_paginator("list_mitigation_actions")
```

Boto3 documentation:
[IoT.Paginator.ListMitigationActions](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot.html#IoT.Paginator.ListMitigationActions)

Arguments for `ListMitigationActionsPaginator.paginate` method:

- `actionType`:
  [MitigationActionTypeType](./literals.md#mitigationactiontypetype)
- `PaginationConfig`:
  [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)

`ListMitigationActionsPaginator.paginate` returns
`AsyncIterable`\[[ListMitigationActionsResponseTypeDef](./type_defs.md#listmitigationactionsresponsetypedef)\].

<a id="listotaupdatespaginator"></a>

## ListOTAUpdatesPaginator

Type annotations for
`session.create_client("iot").get_paginator("list_ota_updates")`.

Can be used directly:

```python
from aiobotocore.session import get_session

from types_aiobotocore_iot.paginator import ListOTAUpdatesPaginator

session = get_session()
async with session.create_client("iot") as client:
    client: IoTClient
    paginator: ListOTAUpdatesPaginator = client.get_paginator("list_ota_updates")
```

Boto3 documentation:
[IoT.Paginator.ListOTAUpdates](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot.html#IoT.Paginator.ListOTAUpdates)

Arguments for `ListOTAUpdatesPaginator.paginate` method:

- `otaUpdateStatus`: [OTAUpdateStatusType](./literals.md#otaupdatestatustype)
- `PaginationConfig`:
  [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)

`ListOTAUpdatesPaginator.paginate` returns
`AsyncIterable`\[[ListOTAUpdatesResponseTypeDef](./type_defs.md#listotaupdatesresponsetypedef)\].

<a id="listoutgoingcertificatespaginator"></a>

## ListOutgoingCertificatesPaginator

Type annotations for
`session.create_client("iot").get_paginator("list_outgoing_certificates")`.

Can be used directly:

```python
from aiobotocore.session import get_session

from types_aiobotocore_iot.paginator import ListOutgoingCertificatesPaginator

session = get_session()
async with session.create_client("iot") as client:
    client: IoTClient
    paginator: ListOutgoingCertificatesPaginator = client.get_paginator("list_outgoing_certificates")
```

Boto3 documentation:
[IoT.Paginator.ListOutgoingCertificates](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot.html#IoT.Paginator.ListOutgoingCertificates)

Arguments for `ListOutgoingCertificatesPaginator.paginate` method:

- `ascendingOrder`: `bool`
- `PaginationConfig`:
  [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)

`ListOutgoingCertificatesPaginator.paginate` returns
`AsyncIterable`\[[ListOutgoingCertificatesResponseTypeDef](./type_defs.md#listoutgoingcertificatesresponsetypedef)\].

<a id="listpoliciespaginator"></a>

## ListPoliciesPaginator

Type annotations for
`session.create_client("iot").get_paginator("list_policies")`.

Can be used directly:

```python
from aiobotocore.session import get_session

from types_aiobotocore_iot.paginator import ListPoliciesPaginator

session = get_session()
async with session.create_client("iot") as client:
    client: IoTClient
    paginator: ListPoliciesPaginator = client.get_paginator("list_policies")
```

Boto3 documentation:
[IoT.Paginator.ListPolicies](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot.html#IoT.Paginator.ListPolicies)

Arguments for `ListPoliciesPaginator.paginate` method:

- `ascendingOrder`: `bool`
- `PaginationConfig`:
  [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)

`ListPoliciesPaginator.paginate` returns
`AsyncIterable`\[[ListPoliciesResponseTypeDef](./type_defs.md#listpoliciesresponsetypedef)\].

<a id="listpolicyprincipalspaginator"></a>

## ListPolicyPrincipalsPaginator

Type annotations for
`session.create_client("iot").get_paginator("list_policy_principals")`.

Can be used directly:

```python
from aiobotocore.session import get_session

from types_aiobotocore_iot.paginator import ListPolicyPrincipalsPaginator

session = get_session()
async with session.create_client("iot") as client:
    client: IoTClient
    paginator: ListPolicyPrincipalsPaginator = client.get_paginator("list_policy_principals")
```

Boto3 documentation:
[IoT.Paginator.ListPolicyPrincipals](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot.html#IoT.Paginator.ListPolicyPrincipals)

Arguments for `ListPolicyPrincipalsPaginator.paginate` method:

- `policyName`: `str` *(required)*
- `ascendingOrder`: `bool`
- `PaginationConfig`:
  [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)

`ListPolicyPrincipalsPaginator.paginate` returns
`AsyncIterable`\[[ListPolicyPrincipalsResponseTypeDef](./type_defs.md#listpolicyprincipalsresponsetypedef)\].

<a id="listprincipalpoliciespaginator"></a>

## ListPrincipalPoliciesPaginator

Type annotations for
`session.create_client("iot").get_paginator("list_principal_policies")`.

Can be used directly:

```python
from aiobotocore.session import get_session

from types_aiobotocore_iot.paginator import ListPrincipalPoliciesPaginator

session = get_session()
async with session.create_client("iot") as client:
    client: IoTClient
    paginator: ListPrincipalPoliciesPaginator = client.get_paginator("list_principal_policies")
```

Boto3 documentation:
[IoT.Paginator.ListPrincipalPolicies](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot.html#IoT.Paginator.ListPrincipalPolicies)

Arguments for `ListPrincipalPoliciesPaginator.paginate` method:

- `principal`: `str` *(required)*
- `ascendingOrder`: `bool`
- `PaginationConfig`:
  [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)

`ListPrincipalPoliciesPaginator.paginate` returns
`AsyncIterable`\[[ListPrincipalPoliciesResponseTypeDef](./type_defs.md#listprincipalpoliciesresponsetypedef)\].

<a id="listprincipalthingspaginator"></a>

## ListPrincipalThingsPaginator

Type annotations for
`session.create_client("iot").get_paginator("list_principal_things")`.

Can be used directly:

```python
from aiobotocore.session import get_session

from types_aiobotocore_iot.paginator import ListPrincipalThingsPaginator

session = get_session()
async with session.create_client("iot") as client:
    client: IoTClient
    paginator: ListPrincipalThingsPaginator = client.get_paginator("list_principal_things")
```

Boto3 documentation:
[IoT.Paginator.ListPrincipalThings](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot.html#IoT.Paginator.ListPrincipalThings)

Arguments for `ListPrincipalThingsPaginator.paginate` method:

- `principal`: `str` *(required)*
- `PaginationConfig`:
  [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)

`ListPrincipalThingsPaginator.paginate` returns
`AsyncIterable`\[[ListPrincipalThingsResponseTypeDef](./type_defs.md#listprincipalthingsresponsetypedef)\].

<a id="listprovisioningtemplateversionspaginator"></a>

## ListProvisioningTemplateVersionsPaginator

Type annotations for
`session.create_client("iot").get_paginator("list_provisioning_template_versions")`.

Can be used directly:

```python
from aiobotocore.session import get_session

from types_aiobotocore_iot.paginator import ListProvisioningTemplateVersionsPaginator

session = get_session()
async with session.create_client("iot") as client:
    client: IoTClient
    paginator: ListProvisioningTemplateVersionsPaginator = client.get_paginator("list_provisioning_template_versions")
```

Boto3 documentation:
[IoT.Paginator.ListProvisioningTemplateVersions](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot.html#IoT.Paginator.ListProvisioningTemplateVersions)

Arguments for `ListProvisioningTemplateVersionsPaginator.paginate` method:

- `templateName`: `str` *(required)*
- `PaginationConfig`:
  [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)

`ListProvisioningTemplateVersionsPaginator.paginate` returns
`AsyncIterable`\[[ListProvisioningTemplateVersionsResponseTypeDef](./type_defs.md#listprovisioningtemplateversionsresponsetypedef)\].

<a id="listprovisioningtemplatespaginator"></a>

## ListProvisioningTemplatesPaginator

Type annotations for
`session.create_client("iot").get_paginator("list_provisioning_templates")`.

Can be used directly:

```python
from aiobotocore.session import get_session

from types_aiobotocore_iot.paginator import ListProvisioningTemplatesPaginator

session = get_session()
async with session.create_client("iot") as client:
    client: IoTClient
    paginator: ListProvisioningTemplatesPaginator = client.get_paginator("list_provisioning_templates")
```

Boto3 documentation:
[IoT.Paginator.ListProvisioningTemplates](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot.html#IoT.Paginator.ListProvisioningTemplates)

Arguments for `ListProvisioningTemplatesPaginator.paginate` method:

- `PaginationConfig`:
  [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)

`ListProvisioningTemplatesPaginator.paginate` returns
`AsyncIterable`\[[ListProvisioningTemplatesResponseTypeDef](./type_defs.md#listprovisioningtemplatesresponsetypedef)\].

<a id="listrolealiasespaginator"></a>

## ListRoleAliasesPaginator

Type annotations for
`session.create_client("iot").get_paginator("list_role_aliases")`.

Can be used directly:

```python
from aiobotocore.session import get_session

from types_aiobotocore_iot.paginator import ListRoleAliasesPaginator

session = get_session()
async with session.create_client("iot") as client:
    client: IoTClient
    paginator: ListRoleAliasesPaginator = client.get_paginator("list_role_aliases")
```

Boto3 documentation:
[IoT.Paginator.ListRoleAliases](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot.html#IoT.Paginator.ListRoleAliases)

Arguments for `ListRoleAliasesPaginator.paginate` method:

- `ascendingOrder`: `bool`
- `PaginationConfig`:
  [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)

`ListRoleAliasesPaginator.paginate` returns
`AsyncIterable`\[[ListRoleAliasesResponseTypeDef](./type_defs.md#listrolealiasesresponsetypedef)\].

<a id="listscheduledauditspaginator"></a>

## ListScheduledAuditsPaginator

Type annotations for
`session.create_client("iot").get_paginator("list_scheduled_audits")`.

Can be used directly:

```python
from aiobotocore.session import get_session

from types_aiobotocore_iot.paginator import ListScheduledAuditsPaginator

session = get_session()
async with session.create_client("iot") as client:
    client: IoTClient
    paginator: ListScheduledAuditsPaginator = client.get_paginator("list_scheduled_audits")
```

Boto3 documentation:
[IoT.Paginator.ListScheduledAudits](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot.html#IoT.Paginator.ListScheduledAudits)

Arguments for `ListScheduledAuditsPaginator.paginate` method:

- `PaginationConfig`:
  [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)

`ListScheduledAuditsPaginator.paginate` returns
`AsyncIterable`\[[ListScheduledAuditsResponseTypeDef](./type_defs.md#listscheduledauditsresponsetypedef)\].

<a id="listsecurityprofilespaginator"></a>

## ListSecurityProfilesPaginator

Type annotations for
`session.create_client("iot").get_paginator("list_security_profiles")`.

Can be used directly:

```python
from aiobotocore.session import get_session

from types_aiobotocore_iot.paginator import ListSecurityProfilesPaginator

session = get_session()
async with session.create_client("iot") as client:
    client: IoTClient
    paginator: ListSecurityProfilesPaginator = client.get_paginator("list_security_profiles")
```

Boto3 documentation:
[IoT.Paginator.ListSecurityProfiles](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot.html#IoT.Paginator.ListSecurityProfiles)

Arguments for `ListSecurityProfilesPaginator.paginate` method:

- `dimensionName`: `str`
- `metricName`: `str`
- `PaginationConfig`:
  [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)

`ListSecurityProfilesPaginator.paginate` returns
`AsyncIterable`\[[ListSecurityProfilesResponseTypeDef](./type_defs.md#listsecurityprofilesresponsetypedef)\].

<a id="listsecurityprofilesfortargetpaginator"></a>

## ListSecurityProfilesForTargetPaginator

Type annotations for
`session.create_client("iot").get_paginator("list_security_profiles_for_target")`.

Can be used directly:

```python
from aiobotocore.session import get_session

from types_aiobotocore_iot.paginator import ListSecurityProfilesForTargetPaginator

session = get_session()
async with session.create_client("iot") as client:
    client: IoTClient
    paginator: ListSecurityProfilesForTargetPaginator = client.get_paginator("list_security_profiles_for_target")
```

Boto3 documentation:
[IoT.Paginator.ListSecurityProfilesForTarget](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot.html#IoT.Paginator.ListSecurityProfilesForTarget)

Arguments for `ListSecurityProfilesForTargetPaginator.paginate` method:

- `securityProfileTargetArn`: `str` *(required)*
- `recursive`: `bool`
- `PaginationConfig`:
  [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)

`ListSecurityProfilesForTargetPaginator.paginate` returns
`AsyncIterable`\[[ListSecurityProfilesForTargetResponseTypeDef](./type_defs.md#listsecurityprofilesfortargetresponsetypedef)\].

<a id="liststreamspaginator"></a>

## ListStreamsPaginator

Type annotations for
`session.create_client("iot").get_paginator("list_streams")`.

Can be used directly:

```python
from aiobotocore.session import get_session

from types_aiobotocore_iot.paginator import ListStreamsPaginator

session = get_session()
async with session.create_client("iot") as client:
    client: IoTClient
    paginator: ListStreamsPaginator = client.get_paginator("list_streams")
```

Boto3 documentation:
[IoT.Paginator.ListStreams](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot.html#IoT.Paginator.ListStreams)

Arguments for `ListStreamsPaginator.paginate` method:

- `ascendingOrder`: `bool`
- `PaginationConfig`:
  [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)

`ListStreamsPaginator.paginate` returns
`AsyncIterable`\[[ListStreamsResponseTypeDef](./type_defs.md#liststreamsresponsetypedef)\].

<a id="listtagsforresourcepaginator"></a>

## ListTagsForResourcePaginator

Type annotations for
`session.create_client("iot").get_paginator("list_tags_for_resource")`.

Can be used directly:

```python
from aiobotocore.session import get_session

from types_aiobotocore_iot.paginator import ListTagsForResourcePaginator

session = get_session()
async with session.create_client("iot") as client:
    client: IoTClient
    paginator: ListTagsForResourcePaginator = client.get_paginator("list_tags_for_resource")
```

Boto3 documentation:
[IoT.Paginator.ListTagsForResource](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot.html#IoT.Paginator.ListTagsForResource)

Arguments for `ListTagsForResourcePaginator.paginate` method:

- `resourceArn`: `str` *(required)*
- `PaginationConfig`:
  [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)

`ListTagsForResourcePaginator.paginate` returns
`AsyncIterable`\[[ListTagsForResourceResponseTypeDef](./type_defs.md#listtagsforresourceresponsetypedef)\].

<a id="listtargetsforpolicypaginator"></a>

## ListTargetsForPolicyPaginator

Type annotations for
`session.create_client("iot").get_paginator("list_targets_for_policy")`.

Can be used directly:

```python
from aiobotocore.session import get_session

from types_aiobotocore_iot.paginator import ListTargetsForPolicyPaginator

session = get_session()
async with session.create_client("iot") as client:
    client: IoTClient
    paginator: ListTargetsForPolicyPaginator = client.get_paginator("list_targets_for_policy")
```

Boto3 documentation:
[IoT.Paginator.ListTargetsForPolicy](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot.html#IoT.Paginator.ListTargetsForPolicy)

Arguments for `ListTargetsForPolicyPaginator.paginate` method:

- `policyName`: `str` *(required)*
- `PaginationConfig`:
  [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)

`ListTargetsForPolicyPaginator.paginate` returns
`AsyncIterable`\[[ListTargetsForPolicyResponseTypeDef](./type_defs.md#listtargetsforpolicyresponsetypedef)\].

<a id="listtargetsforsecurityprofilepaginator"></a>

## ListTargetsForSecurityProfilePaginator

Type annotations for
`session.create_client("iot").get_paginator("list_targets_for_security_profile")`.

Can be used directly:

```python
from aiobotocore.session import get_session

from types_aiobotocore_iot.paginator import ListTargetsForSecurityProfilePaginator

session = get_session()
async with session.create_client("iot") as client:
    client: IoTClient
    paginator: ListTargetsForSecurityProfilePaginator = client.get_paginator("list_targets_for_security_profile")
```

Boto3 documentation:
[IoT.Paginator.ListTargetsForSecurityProfile](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot.html#IoT.Paginator.ListTargetsForSecurityProfile)

Arguments for `ListTargetsForSecurityProfilePaginator.paginate` method:

- `securityProfileName`: `str` *(required)*
- `PaginationConfig`:
  [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)

`ListTargetsForSecurityProfilePaginator.paginate` returns
`AsyncIterable`\[[ListTargetsForSecurityProfileResponseTypeDef](./type_defs.md#listtargetsforsecurityprofileresponsetypedef)\].

<a id="listthinggroupspaginator"></a>

## ListThingGroupsPaginator

Type annotations for
`session.create_client("iot").get_paginator("list_thing_groups")`.

Can be used directly:

```python
from aiobotocore.session import get_session

from types_aiobotocore_iot.paginator import ListThingGroupsPaginator

session = get_session()
async with session.create_client("iot") as client:
    client: IoTClient
    paginator: ListThingGroupsPaginator = client.get_paginator("list_thing_groups")
```

Boto3 documentation:
[IoT.Paginator.ListThingGroups](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot.html#IoT.Paginator.ListThingGroups)

Arguments for `ListThingGroupsPaginator.paginate` method:

- `parentGroup`: `str`
- `namePrefixFilter`: `str`
- `recursive`: `bool`
- `PaginationConfig`:
  [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)

`ListThingGroupsPaginator.paginate` returns
`AsyncIterable`\[[ListThingGroupsResponseTypeDef](./type_defs.md#listthinggroupsresponsetypedef)\].

<a id="listthinggroupsforthingpaginator"></a>

## ListThingGroupsForThingPaginator

Type annotations for
`session.create_client("iot").get_paginator("list_thing_groups_for_thing")`.

Can be used directly:

```python
from aiobotocore.session import get_session

from types_aiobotocore_iot.paginator import ListThingGroupsForThingPaginator

session = get_session()
async with session.create_client("iot") as client:
    client: IoTClient
    paginator: ListThingGroupsForThingPaginator = client.get_paginator("list_thing_groups_for_thing")
```

Boto3 documentation:
[IoT.Paginator.ListThingGroupsForThing](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot.html#IoT.Paginator.ListThingGroupsForThing)

Arguments for `ListThingGroupsForThingPaginator.paginate` method:

- `thingName`: `str` *(required)*
- `PaginationConfig`:
  [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)

`ListThingGroupsForThingPaginator.paginate` returns
`AsyncIterable`\[[ListThingGroupsForThingResponseTypeDef](./type_defs.md#listthinggroupsforthingresponsetypedef)\].

<a id="listthingprincipalspaginator"></a>

## ListThingPrincipalsPaginator

Type annotations for
`session.create_client("iot").get_paginator("list_thing_principals")`.

Can be used directly:

```python
from aiobotocore.session import get_session

from types_aiobotocore_iot.paginator import ListThingPrincipalsPaginator

session = get_session()
async with session.create_client("iot") as client:
    client: IoTClient
    paginator: ListThingPrincipalsPaginator = client.get_paginator("list_thing_principals")
```

Boto3 documentation:
[IoT.Paginator.ListThingPrincipals](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot.html#IoT.Paginator.ListThingPrincipals)

Arguments for `ListThingPrincipalsPaginator.paginate` method:

- `thingName`: `str` *(required)*
- `PaginationConfig`:
  [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)

`ListThingPrincipalsPaginator.paginate` returns
`AsyncIterable`\[[ListThingPrincipalsResponseTypeDef](./type_defs.md#listthingprincipalsresponsetypedef)\].

<a id="listthingregistrationtaskreportspaginator"></a>

## ListThingRegistrationTaskReportsPaginator

Type annotations for
`session.create_client("iot").get_paginator("list_thing_registration_task_reports")`.

Can be used directly:

```python
from aiobotocore.session import get_session

from types_aiobotocore_iot.paginator import ListThingRegistrationTaskReportsPaginator

session = get_session()
async with session.create_client("iot") as client:
    client: IoTClient
    paginator: ListThingRegistrationTaskReportsPaginator = client.get_paginator("list_thing_registration_task_reports")
```

Boto3 documentation:
[IoT.Paginator.ListThingRegistrationTaskReports](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot.html#IoT.Paginator.ListThingRegistrationTaskReports)

Arguments for `ListThingRegistrationTaskReportsPaginator.paginate` method:

- `taskId`: `str` *(required)*
- `reportType`: [ReportTypeType](./literals.md#reporttypetype) *(required)*
- `PaginationConfig`:
  [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)

`ListThingRegistrationTaskReportsPaginator.paginate` returns
`AsyncIterable`\[[ListThingRegistrationTaskReportsResponseTypeDef](./type_defs.md#listthingregistrationtaskreportsresponsetypedef)\].

<a id="listthingregistrationtaskspaginator"></a>

## ListThingRegistrationTasksPaginator

Type annotations for
`session.create_client("iot").get_paginator("list_thing_registration_tasks")`.

Can be used directly:

```python
from aiobotocore.session import get_session

from types_aiobotocore_iot.paginator import ListThingRegistrationTasksPaginator

session = get_session()
async with session.create_client("iot") as client:
    client: IoTClient
    paginator: ListThingRegistrationTasksPaginator = client.get_paginator("list_thing_registration_tasks")
```

Boto3 documentation:
[IoT.Paginator.ListThingRegistrationTasks](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot.html#IoT.Paginator.ListThingRegistrationTasks)

Arguments for `ListThingRegistrationTasksPaginator.paginate` method:

- `status`: [StatusType](./literals.md#statustype)
- `PaginationConfig`:
  [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)

`ListThingRegistrationTasksPaginator.paginate` returns
`AsyncIterable`\[[ListThingRegistrationTasksResponseTypeDef](./type_defs.md#listthingregistrationtasksresponsetypedef)\].

<a id="listthingtypespaginator"></a>

## ListThingTypesPaginator

Type annotations for
`session.create_client("iot").get_paginator("list_thing_types")`.

Can be used directly:

```python
from aiobotocore.session import get_session

from types_aiobotocore_iot.paginator import ListThingTypesPaginator

session = get_session()
async with session.create_client("iot") as client:
    client: IoTClient
    paginator: ListThingTypesPaginator = client.get_paginator("list_thing_types")
```

Boto3 documentation:
[IoT.Paginator.ListThingTypes](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot.html#IoT.Paginator.ListThingTypes)

Arguments for `ListThingTypesPaginator.paginate` method:

- `thingTypeName`: `str`
- `PaginationConfig`:
  [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)

`ListThingTypesPaginator.paginate` returns
`AsyncIterable`\[[ListThingTypesResponseTypeDef](./type_defs.md#listthingtypesresponsetypedef)\].

<a id="listthingspaginator"></a>

## ListThingsPaginator

Type annotations for
`session.create_client("iot").get_paginator("list_things")`.

Can be used directly:

```python
from aiobotocore.session import get_session

from types_aiobotocore_iot.paginator import ListThingsPaginator

session = get_session()
async with session.create_client("iot") as client:
    client: IoTClient
    paginator: ListThingsPaginator = client.get_paginator("list_things")
```

Boto3 documentation:
[IoT.Paginator.ListThings](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot.html#IoT.Paginator.ListThings)

Arguments for `ListThingsPaginator.paginate` method:

- `attributeName`: `str`
- `attributeValue`: `str`
- `thingTypeName`: `str`
- `usePrefixAttributeValue`: `bool`
- `PaginationConfig`:
  [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)

`ListThingsPaginator.paginate` returns
`AsyncIterable`\[[ListThingsResponseTypeDef](./type_defs.md#listthingsresponsetypedef)\].

<a id="listthingsinbillinggrouppaginator"></a>

## ListThingsInBillingGroupPaginator

Type annotations for
`session.create_client("iot").get_paginator("list_things_in_billing_group")`.

Can be used directly:

```python
from aiobotocore.session import get_session

from types_aiobotocore_iot.paginator import ListThingsInBillingGroupPaginator

session = get_session()
async with session.create_client("iot") as client:
    client: IoTClient
    paginator: ListThingsInBillingGroupPaginator = client.get_paginator("list_things_in_billing_group")
```

Boto3 documentation:
[IoT.Paginator.ListThingsInBillingGroup](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot.html#IoT.Paginator.ListThingsInBillingGroup)

Arguments for `ListThingsInBillingGroupPaginator.paginate` method:

- `billingGroupName`: `str` *(required)*
- `PaginationConfig`:
  [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)

`ListThingsInBillingGroupPaginator.paginate` returns
`AsyncIterable`\[[ListThingsInBillingGroupResponseTypeDef](./type_defs.md#listthingsinbillinggroupresponsetypedef)\].

<a id="listthingsinthinggrouppaginator"></a>

## ListThingsInThingGroupPaginator

Type annotations for
`session.create_client("iot").get_paginator("list_things_in_thing_group")`.

Can be used directly:

```python
from aiobotocore.session import get_session

from types_aiobotocore_iot.paginator import ListThingsInThingGroupPaginator

session = get_session()
async with session.create_client("iot") as client:
    client: IoTClient
    paginator: ListThingsInThingGroupPaginator = client.get_paginator("list_things_in_thing_group")
```

Boto3 documentation:
[IoT.Paginator.ListThingsInThingGroup](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot.html#IoT.Paginator.ListThingsInThingGroup)

Arguments for `ListThingsInThingGroupPaginator.paginate` method:

- `thingGroupName`: `str` *(required)*
- `recursive`: `bool`
- `PaginationConfig`:
  [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)

`ListThingsInThingGroupPaginator.paginate` returns
`AsyncIterable`\[[ListThingsInThingGroupResponseTypeDef](./type_defs.md#listthingsinthinggroupresponsetypedef)\].

<a id="listtopicruledestinationspaginator"></a>

## ListTopicRuleDestinationsPaginator

Type annotations for
`session.create_client("iot").get_paginator("list_topic_rule_destinations")`.

Can be used directly:

```python
from aiobotocore.session import get_session

from types_aiobotocore_iot.paginator import ListTopicRuleDestinationsPaginator

session = get_session()
async with session.create_client("iot") as client:
    client: IoTClient
    paginator: ListTopicRuleDestinationsPaginator = client.get_paginator("list_topic_rule_destinations")
```

Boto3 documentation:
[IoT.Paginator.ListTopicRuleDestinations](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot.html#IoT.Paginator.ListTopicRuleDestinations)

Arguments for `ListTopicRuleDestinationsPaginator.paginate` method:

- `PaginationConfig`:
  [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)

`ListTopicRuleDestinationsPaginator.paginate` returns
`AsyncIterable`\[[ListTopicRuleDestinationsResponseTypeDef](./type_defs.md#listtopicruledestinationsresponsetypedef)\].

<a id="listtopicrulespaginator"></a>

## ListTopicRulesPaginator

Type annotations for
`session.create_client("iot").get_paginator("list_topic_rules")`.

Can be used directly:

```python
from aiobotocore.session import get_session

from types_aiobotocore_iot.paginator import ListTopicRulesPaginator

session = get_session()
async with session.create_client("iot") as client:
    client: IoTClient
    paginator: ListTopicRulesPaginator = client.get_paginator("list_topic_rules")
```

Boto3 documentation:
[IoT.Paginator.ListTopicRules](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot.html#IoT.Paginator.ListTopicRules)

Arguments for `ListTopicRulesPaginator.paginate` method:

- `topic`: `str`
- `ruleDisabled`: `bool`
- `PaginationConfig`:
  [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)

`ListTopicRulesPaginator.paginate` returns
`AsyncIterable`\[[ListTopicRulesResponseTypeDef](./type_defs.md#listtopicrulesresponsetypedef)\].

<a id="listv2logginglevelspaginator"></a>

## ListV2LoggingLevelsPaginator

Type annotations for
`session.create_client("iot").get_paginator("list_v2_logging_levels")`.

Can be used directly:

```python
from aiobotocore.session import get_session

from types_aiobotocore_iot.paginator import ListV2LoggingLevelsPaginator

session = get_session()
async with session.create_client("iot") as client:
    client: IoTClient
    paginator: ListV2LoggingLevelsPaginator = client.get_paginator("list_v2_logging_levels")
```

Boto3 documentation:
[IoT.Paginator.ListV2LoggingLevels](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot.html#IoT.Paginator.ListV2LoggingLevels)

Arguments for `ListV2LoggingLevelsPaginator.paginate` method:

- `targetType`: [LogTargetTypeType](./literals.md#logtargettypetype)
- `PaginationConfig`:
  [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)

`ListV2LoggingLevelsPaginator.paginate` returns
`AsyncIterable`\[[ListV2LoggingLevelsResponseTypeDef](./type_defs.md#listv2logginglevelsresponsetypedef)\].

<a id="listviolationeventspaginator"></a>

## ListViolationEventsPaginator

Type annotations for
`session.create_client("iot").get_paginator("list_violation_events")`.

Can be used directly:

```python
from aiobotocore.session import get_session

from types_aiobotocore_iot.paginator import ListViolationEventsPaginator

session = get_session()
async with session.create_client("iot") as client:
    client: IoTClient
    paginator: ListViolationEventsPaginator = client.get_paginator("list_violation_events")
```

Boto3 documentation:
[IoT.Paginator.ListViolationEvents](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot.html#IoT.Paginator.ListViolationEvents)

Arguments for `ListViolationEventsPaginator.paginate` method:

- `startTime`: `Union`\[`datetime`, `str`\] *(required)*
- `endTime`: `Union`\[`datetime`, `str`\] *(required)*
- `thingName`: `str`
- `securityProfileName`: `str`
- `behaviorCriteriaType`:
  [BehaviorCriteriaTypeType](./literals.md#behaviorcriteriatypetype)
- `listSuppressedAlerts`: `bool`
- `verificationState`:
  [VerificationStateType](./literals.md#verificationstatetype)
- `PaginationConfig`:
  [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)

`ListViolationEventsPaginator.paginate` returns
`AsyncIterable`\[[ListViolationEventsResponseTypeDef](./type_defs.md#listviolationeventsresponsetypedef)\].
