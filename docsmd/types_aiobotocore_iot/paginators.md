# Paginators

> [Index](../README.md) > [IoT](./README.md) > Paginators

!!! note ""

    Auto-generated documentation for [IoT](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot.html#iot)
    type annotations stubs module [types-aiobotocore-iot](https://pypi.org/project/types-aiobotocore-iot/).

## GetBehaviorModelTrainingSummariesPaginator

Type annotations and code completion for `#!python session.create_client("iot").get_paginator("get_behavior_model_training_summaries")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot/paginator/GetBehaviorModelTrainingSummaries.html#IoT.Paginator.GetBehaviorModelTrainingSummaries)

```python
# GetBehaviorModelTrainingSummariesPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_iot.paginator import GetBehaviorModelTrainingSummariesPaginator

session = get_session()
async with session.create_client("iot") as client:  # (1)
    paginator: GetBehaviorModelTrainingSummariesPaginator = client.get_paginator("get_behavior_model_training_summaries")  # (2)
    async for item in paginator.paginate(...):
        item: GetBehaviorModelTrainingSummariesResponseTypeDef
        print(item)  # (3)
```

1. client: [IoTClient](./client.md)
2. paginator: [GetBehaviorModelTrainingSummariesPaginator](./paginators.md#getbehaviormodeltrainingsummariespaginator)
3. item: `AioPageIterator[GetBehaviorModelTrainingSummariesResponseTypeDef]`


### paginate

Type annotations and code completion for `#!python GetBehaviorModelTrainingSummariesPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    securityProfileName: str = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> aiobotocore.paginate.AioPageIterator[GetBehaviorModelTrainingSummariesResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
2. See `AioPageIterator[GetBehaviorModelTrainingSummariesResponseTypeDef]`


```python
# paginate method usage example with argument unpacking

kwargs: GetBehaviorModelTrainingSummariesRequestPaginateTypeDef = {  # (1)
    "securityProfileName": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: GetBehaviorModelTrainingSummariesRequestPaginateTypeDef](./type_defs.md#getbehaviormodeltrainingsummariesrequestpaginatetypedef)
## ListActiveViolationsPaginator

Type annotations and code completion for `#!python session.create_client("iot").get_paginator("list_active_violations")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot/paginator/ListActiveViolations.html#IoT.Paginator.ListActiveViolations)

```python
# ListActiveViolationsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_iot.paginator import ListActiveViolationsPaginator

session = get_session()
async with session.create_client("iot") as client:  # (1)
    paginator: ListActiveViolationsPaginator = client.get_paginator("list_active_violations")  # (2)
    async for item in paginator.paginate(...):
        item: ListActiveViolationsResponseTypeDef
        print(item)  # (3)
```

1. client: [IoTClient](./client.md)
2. paginator: [ListActiveViolationsPaginator](./paginators.md#listactiveviolationspaginator)
3. item: `AioPageIterator[ListActiveViolationsResponseTypeDef]`


### paginate

Type annotations and code completion for `#!python ListActiveViolationsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    thingName: str = ...,
    securityProfileName: str = ...,
    behaviorCriteriaType: BehaviorCriteriaTypeType = ...,  # (1)
    listSuppressedAlerts: bool = ...,
    verificationState: VerificationStateType = ...,  # (2)
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (3)
) -> aiobotocore.paginate.AioPageIterator[ListActiveViolationsResponseTypeDef]:  # (4)
    ...
```

1. See [:material-code-brackets: BehaviorCriteriaTypeType](./literals.md#behaviorcriteriatypetype)
2. See [:material-code-brackets: VerificationStateType](./literals.md#verificationstatetype)
3. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
4. See `AioPageIterator[ListActiveViolationsResponseTypeDef]`


```python
# paginate method usage example with argument unpacking

kwargs: ListActiveViolationsRequestPaginateTypeDef = {  # (1)
    "thingName": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListActiveViolationsRequestPaginateTypeDef](./type_defs.md#listactiveviolationsrequestpaginatetypedef)
## ListAttachedPoliciesPaginator

Type annotations and code completion for `#!python session.create_client("iot").get_paginator("list_attached_policies")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot/paginator/ListAttachedPolicies.html#IoT.Paginator.ListAttachedPolicies)

```python
# ListAttachedPoliciesPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_iot.paginator import ListAttachedPoliciesPaginator

session = get_session()
async with session.create_client("iot") as client:  # (1)
    paginator: ListAttachedPoliciesPaginator = client.get_paginator("list_attached_policies")  # (2)
    async for item in paginator.paginate(...):
        item: ListAttachedPoliciesResponseTypeDef
        print(item)  # (3)
```

1. client: [IoTClient](./client.md)
2. paginator: [ListAttachedPoliciesPaginator](./paginators.md#listattachedpoliciespaginator)
3. item: `AioPageIterator[ListAttachedPoliciesResponseTypeDef]`


### paginate

Type annotations and code completion for `#!python ListAttachedPoliciesPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    target: str,
    recursive: bool = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> aiobotocore.paginate.AioPageIterator[ListAttachedPoliciesResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
2. See `AioPageIterator[ListAttachedPoliciesResponseTypeDef]`


```python
# paginate method usage example with argument unpacking

kwargs: ListAttachedPoliciesRequestPaginateTypeDef = {  # (1)
    "target": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListAttachedPoliciesRequestPaginateTypeDef](./type_defs.md#listattachedpoliciesrequestpaginatetypedef)
## ListAuditFindingsPaginator

Type annotations and code completion for `#!python session.create_client("iot").get_paginator("list_audit_findings")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot/paginator/ListAuditFindings.html#IoT.Paginator.ListAuditFindings)

```python
# ListAuditFindingsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_iot.paginator import ListAuditFindingsPaginator

session = get_session()
async with session.create_client("iot") as client:  # (1)
    paginator: ListAuditFindingsPaginator = client.get_paginator("list_audit_findings")  # (2)
    async for item in paginator.paginate(...):
        item: ListAuditFindingsResponseTypeDef
        print(item)  # (3)
```

1. client: [IoTClient](./client.md)
2. paginator: [ListAuditFindingsPaginator](./paginators.md#listauditfindingspaginator)
3. item: `AioPageIterator[ListAuditFindingsResponseTypeDef]`


### paginate

Type annotations and code completion for `#!python ListAuditFindingsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    taskId: str = ...,
    checkName: str = ...,
    resourceIdentifier: ResourceIdentifierTypeDef = ...,  # (1)
    startTime: TimestampTypeDef = ...,
    endTime: TimestampTypeDef = ...,
    listSuppressedFindings: bool = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (2)
) -> aiobotocore.paginate.AioPageIterator[ListAuditFindingsResponseTypeDef]:  # (3)
    ...
```

1. See [:material-code-braces: ResourceIdentifierTypeDef](./type_defs.md#resourceidentifiertypedef)
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
3. See `AioPageIterator[ListAuditFindingsResponseTypeDef]`


```python
# paginate method usage example with argument unpacking

kwargs: ListAuditFindingsRequestPaginateTypeDef = {  # (1)
    "taskId": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListAuditFindingsRequestPaginateTypeDef](./type_defs.md#listauditfindingsrequestpaginatetypedef)
## ListAuditMitigationActionsExecutionsPaginator

Type annotations and code completion for `#!python session.create_client("iot").get_paginator("list_audit_mitigation_actions_executions")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot/paginator/ListAuditMitigationActionsExecutions.html#IoT.Paginator.ListAuditMitigationActionsExecutions)

```python
# ListAuditMitigationActionsExecutionsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_iot.paginator import ListAuditMitigationActionsExecutionsPaginator

session = get_session()
async with session.create_client("iot") as client:  # (1)
    paginator: ListAuditMitigationActionsExecutionsPaginator = client.get_paginator("list_audit_mitigation_actions_executions")  # (2)
    async for item in paginator.paginate(...):
        item: ListAuditMitigationActionsExecutionsResponseTypeDef
        print(item)  # (3)
```

1. client: [IoTClient](./client.md)
2. paginator: [ListAuditMitigationActionsExecutionsPaginator](./paginators.md#listauditmitigationactionsexecutionspaginator)
3. item: `AioPageIterator[ListAuditMitigationActionsExecutionsResponseTypeDef]`


### paginate

Type annotations and code completion for `#!python ListAuditMitigationActionsExecutionsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    taskId: str,
    findingId: str,
    actionStatus: AuditMitigationActionsExecutionStatusType = ...,  # (1)
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (2)
) -> aiobotocore.paginate.AioPageIterator[ListAuditMitigationActionsExecutionsResponseTypeDef]:  # (3)
    ...
```

1. See [:material-code-brackets: AuditMitigationActionsExecutionStatusType](./literals.md#auditmitigationactionsexecutionstatustype)
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
3. See `AioPageIterator[ListAuditMitigationActionsExecutionsResponseTypeDef]`


```python
# paginate method usage example with argument unpacking

kwargs: ListAuditMitigationActionsExecutionsRequestPaginateTypeDef = {  # (1)
    "taskId": ...,
    "findingId": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListAuditMitigationActionsExecutionsRequestPaginateTypeDef](./type_defs.md#listauditmitigationactionsexecutionsrequestpaginatetypedef)
## ListAuditMitigationActionsTasksPaginator

Type annotations and code completion for `#!python session.create_client("iot").get_paginator("list_audit_mitigation_actions_tasks")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot/paginator/ListAuditMitigationActionsTasks.html#IoT.Paginator.ListAuditMitigationActionsTasks)

```python
# ListAuditMitigationActionsTasksPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_iot.paginator import ListAuditMitigationActionsTasksPaginator

session = get_session()
async with session.create_client("iot") as client:  # (1)
    paginator: ListAuditMitigationActionsTasksPaginator = client.get_paginator("list_audit_mitigation_actions_tasks")  # (2)
    async for item in paginator.paginate(...):
        item: ListAuditMitigationActionsTasksResponseTypeDef
        print(item)  # (3)
```

1. client: [IoTClient](./client.md)
2. paginator: [ListAuditMitigationActionsTasksPaginator](./paginators.md#listauditmitigationactionstaskspaginator)
3. item: `AioPageIterator[ListAuditMitigationActionsTasksResponseTypeDef]`


### paginate

Type annotations and code completion for `#!python ListAuditMitigationActionsTasksPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    startTime: TimestampTypeDef,
    endTime: TimestampTypeDef,
    auditTaskId: str = ...,
    findingId: str = ...,
    taskStatus: AuditMitigationActionsTaskStatusType = ...,  # (1)
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (2)
) -> aiobotocore.paginate.AioPageIterator[ListAuditMitigationActionsTasksResponseTypeDef]:  # (3)
    ...
```

1. See [:material-code-brackets: AuditMitigationActionsTaskStatusType](./literals.md#auditmitigationactionstaskstatustype)
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
3. See `AioPageIterator[ListAuditMitigationActionsTasksResponseTypeDef]`


```python
# paginate method usage example with argument unpacking

kwargs: ListAuditMitigationActionsTasksRequestPaginateTypeDef = {  # (1)
    "startTime": ...,
    "endTime": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListAuditMitigationActionsTasksRequestPaginateTypeDef](./type_defs.md#listauditmitigationactionstasksrequestpaginatetypedef)
## ListAuditSuppressionsPaginator

Type annotations and code completion for `#!python session.create_client("iot").get_paginator("list_audit_suppressions")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot/paginator/ListAuditSuppressions.html#IoT.Paginator.ListAuditSuppressions)

```python
# ListAuditSuppressionsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_iot.paginator import ListAuditSuppressionsPaginator

session = get_session()
async with session.create_client("iot") as client:  # (1)
    paginator: ListAuditSuppressionsPaginator = client.get_paginator("list_audit_suppressions")  # (2)
    async for item in paginator.paginate(...):
        item: ListAuditSuppressionsResponseTypeDef
        print(item)  # (3)
```

1. client: [IoTClient](./client.md)
2. paginator: [ListAuditSuppressionsPaginator](./paginators.md#listauditsuppressionspaginator)
3. item: `AioPageIterator[ListAuditSuppressionsResponseTypeDef]`


### paginate

Type annotations and code completion for `#!python ListAuditSuppressionsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    checkName: str = ...,
    resourceIdentifier: ResourceIdentifierTypeDef = ...,  # (1)
    ascendingOrder: bool = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (2)
) -> aiobotocore.paginate.AioPageIterator[ListAuditSuppressionsResponseTypeDef]:  # (3)
    ...
```

1. See [:material-code-braces: ResourceIdentifierTypeDef](./type_defs.md#resourceidentifiertypedef)
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
3. See `AioPageIterator[ListAuditSuppressionsResponseTypeDef]`


```python
# paginate method usage example with argument unpacking

kwargs: ListAuditSuppressionsRequestPaginateTypeDef = {  # (1)
    "checkName": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListAuditSuppressionsRequestPaginateTypeDef](./type_defs.md#listauditsuppressionsrequestpaginatetypedef)
## ListAuditTasksPaginator

Type annotations and code completion for `#!python session.create_client("iot").get_paginator("list_audit_tasks")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot/paginator/ListAuditTasks.html#IoT.Paginator.ListAuditTasks)

```python
# ListAuditTasksPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_iot.paginator import ListAuditTasksPaginator

session = get_session()
async with session.create_client("iot") as client:  # (1)
    paginator: ListAuditTasksPaginator = client.get_paginator("list_audit_tasks")  # (2)
    async for item in paginator.paginate(...):
        item: ListAuditTasksResponseTypeDef
        print(item)  # (3)
```

1. client: [IoTClient](./client.md)
2. paginator: [ListAuditTasksPaginator](./paginators.md#listaudittaskspaginator)
3. item: `AioPageIterator[ListAuditTasksResponseTypeDef]`


### paginate

Type annotations and code completion for `#!python ListAuditTasksPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    startTime: TimestampTypeDef,
    endTime: TimestampTypeDef,
    taskType: AuditTaskTypeType = ...,  # (1)
    taskStatus: AuditTaskStatusType = ...,  # (2)
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (3)
) -> aiobotocore.paginate.AioPageIterator[ListAuditTasksResponseTypeDef]:  # (4)
    ...
```

1. See [:material-code-brackets: AuditTaskTypeType](./literals.md#audittasktypetype)
2. See [:material-code-brackets: AuditTaskStatusType](./literals.md#audittaskstatustype)
3. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
4. See `AioPageIterator[ListAuditTasksResponseTypeDef]`


```python
# paginate method usage example with argument unpacking

kwargs: ListAuditTasksRequestPaginateTypeDef = {  # (1)
    "startTime": ...,
    "endTime": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListAuditTasksRequestPaginateTypeDef](./type_defs.md#listaudittasksrequestpaginatetypedef)
## ListAuthorizersPaginator

Type annotations and code completion for `#!python session.create_client("iot").get_paginator("list_authorizers")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot/paginator/ListAuthorizers.html#IoT.Paginator.ListAuthorizers)

```python
# ListAuthorizersPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_iot.paginator import ListAuthorizersPaginator

session = get_session()
async with session.create_client("iot") as client:  # (1)
    paginator: ListAuthorizersPaginator = client.get_paginator("list_authorizers")  # (2)
    async for item in paginator.paginate(...):
        item: ListAuthorizersResponseTypeDef
        print(item)  # (3)
```

1. client: [IoTClient](./client.md)
2. paginator: [ListAuthorizersPaginator](./paginators.md#listauthorizerspaginator)
3. item: `AioPageIterator[ListAuthorizersResponseTypeDef]`


### paginate

Type annotations and code completion for `#!python ListAuthorizersPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    ascendingOrder: bool = ...,
    status: AuthorizerStatusType = ...,  # (1)
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (2)
) -> aiobotocore.paginate.AioPageIterator[ListAuthorizersResponseTypeDef]:  # (3)
    ...
```

1. See [:material-code-brackets: AuthorizerStatusType](./literals.md#authorizerstatustype)
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
3. See `AioPageIterator[ListAuthorizersResponseTypeDef]`


```python
# paginate method usage example with argument unpacking

kwargs: ListAuthorizersRequestPaginateTypeDef = {  # (1)
    "ascendingOrder": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListAuthorizersRequestPaginateTypeDef](./type_defs.md#listauthorizersrequestpaginatetypedef)
## ListBillingGroupsPaginator

Type annotations and code completion for `#!python session.create_client("iot").get_paginator("list_billing_groups")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot/paginator/ListBillingGroups.html#IoT.Paginator.ListBillingGroups)

```python
# ListBillingGroupsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_iot.paginator import ListBillingGroupsPaginator

session = get_session()
async with session.create_client("iot") as client:  # (1)
    paginator: ListBillingGroupsPaginator = client.get_paginator("list_billing_groups")  # (2)
    async for item in paginator.paginate(...):
        item: ListBillingGroupsResponseTypeDef
        print(item)  # (3)
```

1. client: [IoTClient](./client.md)
2. paginator: [ListBillingGroupsPaginator](./paginators.md#listbillinggroupspaginator)
3. item: `AioPageIterator[ListBillingGroupsResponseTypeDef]`


### paginate

Type annotations and code completion for `#!python ListBillingGroupsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    namePrefixFilter: str = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> aiobotocore.paginate.AioPageIterator[ListBillingGroupsResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
2. See `AioPageIterator[ListBillingGroupsResponseTypeDef]`


```python
# paginate method usage example with argument unpacking

kwargs: ListBillingGroupsRequestPaginateTypeDef = {  # (1)
    "namePrefixFilter": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListBillingGroupsRequestPaginateTypeDef](./type_defs.md#listbillinggroupsrequestpaginatetypedef)
## ListCACertificatesPaginator

Type annotations and code completion for `#!python session.create_client("iot").get_paginator("list_ca_certificates")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot/paginator/ListCACertificates.html#IoT.Paginator.ListCACertificates)

```python
# ListCACertificatesPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_iot.paginator import ListCACertificatesPaginator

session = get_session()
async with session.create_client("iot") as client:  # (1)
    paginator: ListCACertificatesPaginator = client.get_paginator("list_ca_certificates")  # (2)
    async for item in paginator.paginate(...):
        item: ListCACertificatesResponseTypeDef
        print(item)  # (3)
```

1. client: [IoTClient](./client.md)
2. paginator: [ListCACertificatesPaginator](./paginators.md#listcacertificatespaginator)
3. item: `AioPageIterator[ListCACertificatesResponseTypeDef]`


### paginate

Type annotations and code completion for `#!python ListCACertificatesPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    ascendingOrder: bool = ...,
    templateName: str = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> aiobotocore.paginate.AioPageIterator[ListCACertificatesResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
2. See `AioPageIterator[ListCACertificatesResponseTypeDef]`


```python
# paginate method usage example with argument unpacking

kwargs: ListCACertificatesRequestPaginateTypeDef = {  # (1)
    "ascendingOrder": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListCACertificatesRequestPaginateTypeDef](./type_defs.md#listcacertificatesrequestpaginatetypedef)
## ListCertificatesByCAPaginator

Type annotations and code completion for `#!python session.create_client("iot").get_paginator("list_certificates_by_ca")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot/paginator/ListCertificatesByCA.html#IoT.Paginator.ListCertificatesByCA)

```python
# ListCertificatesByCAPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_iot.paginator import ListCertificatesByCAPaginator

session = get_session()
async with session.create_client("iot") as client:  # (1)
    paginator: ListCertificatesByCAPaginator = client.get_paginator("list_certificates_by_ca")  # (2)
    async for item in paginator.paginate(...):
        item: ListCertificatesByCAResponseTypeDef
        print(item)  # (3)
```

1. client: [IoTClient](./client.md)
2. paginator: [ListCertificatesByCAPaginator](./paginators.md#listcertificatesbycapaginator)
3. item: `AioPageIterator[ListCertificatesByCAResponseTypeDef]`


### paginate

Type annotations and code completion for `#!python ListCertificatesByCAPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    caCertificateId: str,
    ascendingOrder: bool = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> aiobotocore.paginate.AioPageIterator[ListCertificatesByCAResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
2. See `AioPageIterator[ListCertificatesByCAResponseTypeDef]`


```python
# paginate method usage example with argument unpacking

kwargs: ListCertificatesByCARequestPaginateTypeDef = {  # (1)
    "caCertificateId": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListCertificatesByCARequestPaginateTypeDef](./type_defs.md#listcertificatesbycarequestpaginatetypedef)
## ListCertificatesPaginator

Type annotations and code completion for `#!python session.create_client("iot").get_paginator("list_certificates")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot/paginator/ListCertificates.html#IoT.Paginator.ListCertificates)

```python
# ListCertificatesPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_iot.paginator import ListCertificatesPaginator

session = get_session()
async with session.create_client("iot") as client:  # (1)
    paginator: ListCertificatesPaginator = client.get_paginator("list_certificates")  # (2)
    async for item in paginator.paginate(...):
        item: ListCertificatesResponseTypeDef
        print(item)  # (3)
```

1. client: [IoTClient](./client.md)
2. paginator: [ListCertificatesPaginator](./paginators.md#listcertificatespaginator)
3. item: `AioPageIterator[ListCertificatesResponseTypeDef]`


### paginate

Type annotations and code completion for `#!python ListCertificatesPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    ascendingOrder: bool = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> aiobotocore.paginate.AioPageIterator[ListCertificatesResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
2. See `AioPageIterator[ListCertificatesResponseTypeDef]`


```python
# paginate method usage example with argument unpacking

kwargs: ListCertificatesRequestPaginateTypeDef = {  # (1)
    "ascendingOrder": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListCertificatesRequestPaginateTypeDef](./type_defs.md#listcertificatesrequestpaginatetypedef)
## ListCommandExecutionsPaginator

Type annotations and code completion for `#!python session.create_client("iot").get_paginator("list_command_executions")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot/paginator/ListCommandExecutions.html#IoT.Paginator.ListCommandExecutions)

```python
# ListCommandExecutionsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_iot.paginator import ListCommandExecutionsPaginator

session = get_session()
async with session.create_client("iot") as client:  # (1)
    paginator: ListCommandExecutionsPaginator = client.get_paginator("list_command_executions")  # (2)
    async for item in paginator.paginate(...):
        item: ListCommandExecutionsResponseTypeDef
        print(item)  # (3)
```

1. client: [IoTClient](./client.md)
2. paginator: [ListCommandExecutionsPaginator](./paginators.md#listcommandexecutionspaginator)
3. item: `AioPageIterator[ListCommandExecutionsResponseTypeDef]`


### paginate

Type annotations and code completion for `#!python ListCommandExecutionsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    namespace: CommandNamespaceType = ...,  # (1)
    status: CommandExecutionStatusType = ...,  # (2)
    sortOrder: SortOrderType = ...,  # (3)
    startedTimeFilter: TimeFilterTypeDef = ...,  # (4)
    completedTimeFilter: TimeFilterTypeDef = ...,  # (4)
    targetArn: str = ...,
    commandArn: str = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (6)
) -> aiobotocore.paginate.AioPageIterator[ListCommandExecutionsResponseTypeDef]:  # (7)
    ...
```

1. See [:material-code-brackets: CommandNamespaceType](./literals.md#commandnamespacetype)
2. See [:material-code-brackets: CommandExecutionStatusType](./literals.md#commandexecutionstatustype)
3. See [:material-code-brackets: SortOrderType](./literals.md#sortordertype)
4. See [:material-code-braces: TimeFilterTypeDef](./type_defs.md#timefiltertypedef)
5. See [:material-code-braces: TimeFilterTypeDef](./type_defs.md#timefiltertypedef)
6. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
7. See `AioPageIterator[ListCommandExecutionsResponseTypeDef]`


```python
# paginate method usage example with argument unpacking

kwargs: ListCommandExecutionsRequestPaginateTypeDef = {  # (1)
    "namespace": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListCommandExecutionsRequestPaginateTypeDef](./type_defs.md#listcommandexecutionsrequestpaginatetypedef)
## ListCommandsPaginator

Type annotations and code completion for `#!python session.create_client("iot").get_paginator("list_commands")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot/paginator/ListCommands.html#IoT.Paginator.ListCommands)

```python
# ListCommandsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_iot.paginator import ListCommandsPaginator

session = get_session()
async with session.create_client("iot") as client:  # (1)
    paginator: ListCommandsPaginator = client.get_paginator("list_commands")  # (2)
    async for item in paginator.paginate(...):
        item: ListCommandsResponseTypeDef
        print(item)  # (3)
```

1. client: [IoTClient](./client.md)
2. paginator: [ListCommandsPaginator](./paginators.md#listcommandspaginator)
3. item: `AioPageIterator[ListCommandsResponseTypeDef]`


### paginate

Type annotations and code completion for `#!python ListCommandsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    namespace: CommandNamespaceType = ...,  # (1)
    commandParameterName: str = ...,
    sortOrder: SortOrderType = ...,  # (2)
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (3)
) -> aiobotocore.paginate.AioPageIterator[ListCommandsResponseTypeDef]:  # (4)
    ...
```

1. See [:material-code-brackets: CommandNamespaceType](./literals.md#commandnamespacetype)
2. See [:material-code-brackets: SortOrderType](./literals.md#sortordertype)
3. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
4. See `AioPageIterator[ListCommandsResponseTypeDef]`


```python
# paginate method usage example with argument unpacking

kwargs: ListCommandsRequestPaginateTypeDef = {  # (1)
    "namespace": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListCommandsRequestPaginateTypeDef](./type_defs.md#listcommandsrequestpaginatetypedef)
## ListCustomMetricsPaginator

Type annotations and code completion for `#!python session.create_client("iot").get_paginator("list_custom_metrics")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot/paginator/ListCustomMetrics.html#IoT.Paginator.ListCustomMetrics)

```python
# ListCustomMetricsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_iot.paginator import ListCustomMetricsPaginator

session = get_session()
async with session.create_client("iot") as client:  # (1)
    paginator: ListCustomMetricsPaginator = client.get_paginator("list_custom_metrics")  # (2)
    async for item in paginator.paginate(...):
        item: ListCustomMetricsResponseTypeDef
        print(item)  # (3)
```

1. client: [IoTClient](./client.md)
2. paginator: [ListCustomMetricsPaginator](./paginators.md#listcustommetricspaginator)
3. item: `AioPageIterator[ListCustomMetricsResponseTypeDef]`


### paginate

Type annotations and code completion for `#!python ListCustomMetricsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> aiobotocore.paginate.AioPageIterator[ListCustomMetricsResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
2. See `AioPageIterator[ListCustomMetricsResponseTypeDef]`


```python
# paginate method usage example with argument unpacking

kwargs: ListCustomMetricsRequestPaginateTypeDef = {  # (1)
    "PaginationConfig": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListCustomMetricsRequestPaginateTypeDef](./type_defs.md#listcustommetricsrequestpaginatetypedef)
## ListDetectMitigationActionsExecutionsPaginator

Type annotations and code completion for `#!python session.create_client("iot").get_paginator("list_detect_mitigation_actions_executions")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot/paginator/ListDetectMitigationActionsExecutions.html#IoT.Paginator.ListDetectMitigationActionsExecutions)

```python
# ListDetectMitigationActionsExecutionsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_iot.paginator import ListDetectMitigationActionsExecutionsPaginator

session = get_session()
async with session.create_client("iot") as client:  # (1)
    paginator: ListDetectMitigationActionsExecutionsPaginator = client.get_paginator("list_detect_mitigation_actions_executions")  # (2)
    async for item in paginator.paginate(...):
        item: ListDetectMitigationActionsExecutionsResponseTypeDef
        print(item)  # (3)
```

1. client: [IoTClient](./client.md)
2. paginator: [ListDetectMitigationActionsExecutionsPaginator](./paginators.md#listdetectmitigationactionsexecutionspaginator)
3. item: `AioPageIterator[ListDetectMitigationActionsExecutionsResponseTypeDef]`


### paginate

Type annotations and code completion for `#!python ListDetectMitigationActionsExecutionsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    taskId: str = ...,
    violationId: str = ...,
    thingName: str = ...,
    startTime: TimestampTypeDef = ...,
    endTime: TimestampTypeDef = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> aiobotocore.paginate.AioPageIterator[ListDetectMitigationActionsExecutionsResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
2. See `AioPageIterator[ListDetectMitigationActionsExecutionsResponseTypeDef]`


```python
# paginate method usage example with argument unpacking

kwargs: ListDetectMitigationActionsExecutionsRequestPaginateTypeDef = {  # (1)
    "taskId": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListDetectMitigationActionsExecutionsRequestPaginateTypeDef](./type_defs.md#listdetectmitigationactionsexecutionsrequestpaginatetypedef)
## ListDetectMitigationActionsTasksPaginator

Type annotations and code completion for `#!python session.create_client("iot").get_paginator("list_detect_mitigation_actions_tasks")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot/paginator/ListDetectMitigationActionsTasks.html#IoT.Paginator.ListDetectMitigationActionsTasks)

```python
# ListDetectMitigationActionsTasksPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_iot.paginator import ListDetectMitigationActionsTasksPaginator

session = get_session()
async with session.create_client("iot") as client:  # (1)
    paginator: ListDetectMitigationActionsTasksPaginator = client.get_paginator("list_detect_mitigation_actions_tasks")  # (2)
    async for item in paginator.paginate(...):
        item: ListDetectMitigationActionsTasksResponseTypeDef
        print(item)  # (3)
```

1. client: [IoTClient](./client.md)
2. paginator: [ListDetectMitigationActionsTasksPaginator](./paginators.md#listdetectmitigationactionstaskspaginator)
3. item: `AioPageIterator[ListDetectMitigationActionsTasksResponseTypeDef]`


### paginate

Type annotations and code completion for `#!python ListDetectMitigationActionsTasksPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    startTime: TimestampTypeDef,
    endTime: TimestampTypeDef,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> aiobotocore.paginate.AioPageIterator[ListDetectMitigationActionsTasksResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
2. See `AioPageIterator[ListDetectMitigationActionsTasksResponseTypeDef]`


```python
# paginate method usage example with argument unpacking

kwargs: ListDetectMitigationActionsTasksRequestPaginateTypeDef = {  # (1)
    "startTime": ...,
    "endTime": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListDetectMitigationActionsTasksRequestPaginateTypeDef](./type_defs.md#listdetectmitigationactionstasksrequestpaginatetypedef)
## ListDimensionsPaginator

Type annotations and code completion for `#!python session.create_client("iot").get_paginator("list_dimensions")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot/paginator/ListDimensions.html#IoT.Paginator.ListDimensions)

```python
# ListDimensionsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_iot.paginator import ListDimensionsPaginator

session = get_session()
async with session.create_client("iot") as client:  # (1)
    paginator: ListDimensionsPaginator = client.get_paginator("list_dimensions")  # (2)
    async for item in paginator.paginate(...):
        item: ListDimensionsResponseTypeDef
        print(item)  # (3)
```

1. client: [IoTClient](./client.md)
2. paginator: [ListDimensionsPaginator](./paginators.md#listdimensionspaginator)
3. item: `AioPageIterator[ListDimensionsResponseTypeDef]`


### paginate

Type annotations and code completion for `#!python ListDimensionsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> aiobotocore.paginate.AioPageIterator[ListDimensionsResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
2. See `AioPageIterator[ListDimensionsResponseTypeDef]`


```python
# paginate method usage example with argument unpacking

kwargs: ListDimensionsRequestPaginateTypeDef = {  # (1)
    "PaginationConfig": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListDimensionsRequestPaginateTypeDef](./type_defs.md#listdimensionsrequestpaginatetypedef)
## ListDomainConfigurationsPaginator

Type annotations and code completion for `#!python session.create_client("iot").get_paginator("list_domain_configurations")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot/paginator/ListDomainConfigurations.html#IoT.Paginator.ListDomainConfigurations)

```python
# ListDomainConfigurationsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_iot.paginator import ListDomainConfigurationsPaginator

session = get_session()
async with session.create_client("iot") as client:  # (1)
    paginator: ListDomainConfigurationsPaginator = client.get_paginator("list_domain_configurations")  # (2)
    async for item in paginator.paginate(...):
        item: ListDomainConfigurationsResponseTypeDef
        print(item)  # (3)
```

1. client: [IoTClient](./client.md)
2. paginator: [ListDomainConfigurationsPaginator](./paginators.md#listdomainconfigurationspaginator)
3. item: `AioPageIterator[ListDomainConfigurationsResponseTypeDef]`


### paginate

Type annotations and code completion for `#!python ListDomainConfigurationsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    serviceType: ServiceTypeType = ...,  # (1)
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (2)
) -> aiobotocore.paginate.AioPageIterator[ListDomainConfigurationsResponseTypeDef]:  # (3)
    ...
```

1. See [:material-code-brackets: ServiceTypeType](./literals.md#servicetypetype)
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
3. See `AioPageIterator[ListDomainConfigurationsResponseTypeDef]`


```python
# paginate method usage example with argument unpacking

kwargs: ListDomainConfigurationsRequestPaginateTypeDef = {  # (1)
    "serviceType": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListDomainConfigurationsRequestPaginateTypeDef](./type_defs.md#listdomainconfigurationsrequestpaginatetypedef)
## ListFleetMetricsPaginator

Type annotations and code completion for `#!python session.create_client("iot").get_paginator("list_fleet_metrics")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot/paginator/ListFleetMetrics.html#IoT.Paginator.ListFleetMetrics)

```python
# ListFleetMetricsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_iot.paginator import ListFleetMetricsPaginator

session = get_session()
async with session.create_client("iot") as client:  # (1)
    paginator: ListFleetMetricsPaginator = client.get_paginator("list_fleet_metrics")  # (2)
    async for item in paginator.paginate(...):
        item: ListFleetMetricsResponseTypeDef
        print(item)  # (3)
```

1. client: [IoTClient](./client.md)
2. paginator: [ListFleetMetricsPaginator](./paginators.md#listfleetmetricspaginator)
3. item: `AioPageIterator[ListFleetMetricsResponseTypeDef]`


### paginate

Type annotations and code completion for `#!python ListFleetMetricsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> aiobotocore.paginate.AioPageIterator[ListFleetMetricsResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
2. See `AioPageIterator[ListFleetMetricsResponseTypeDef]`


```python
# paginate method usage example with argument unpacking

kwargs: ListFleetMetricsRequestPaginateTypeDef = {  # (1)
    "PaginationConfig": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListFleetMetricsRequestPaginateTypeDef](./type_defs.md#listfleetmetricsrequestpaginatetypedef)
## ListIndicesPaginator

Type annotations and code completion for `#!python session.create_client("iot").get_paginator("list_indices")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot/paginator/ListIndices.html#IoT.Paginator.ListIndices)

```python
# ListIndicesPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_iot.paginator import ListIndicesPaginator

session = get_session()
async with session.create_client("iot") as client:  # (1)
    paginator: ListIndicesPaginator = client.get_paginator("list_indices")  # (2)
    async for item in paginator.paginate(...):
        item: ListIndicesResponseTypeDef
        print(item)  # (3)
```

1. client: [IoTClient](./client.md)
2. paginator: [ListIndicesPaginator](./paginators.md#listindicespaginator)
3. item: `AioPageIterator[ListIndicesResponseTypeDef]`


### paginate

Type annotations and code completion for `#!python ListIndicesPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> aiobotocore.paginate.AioPageIterator[ListIndicesResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
2. See `AioPageIterator[ListIndicesResponseTypeDef]`


```python
# paginate method usage example with argument unpacking

kwargs: ListIndicesRequestPaginateTypeDef = {  # (1)
    "PaginationConfig": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListIndicesRequestPaginateTypeDef](./type_defs.md#listindicesrequestpaginatetypedef)
## ListJobExecutionsForJobPaginator

Type annotations and code completion for `#!python session.create_client("iot").get_paginator("list_job_executions_for_job")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot/paginator/ListJobExecutionsForJob.html#IoT.Paginator.ListJobExecutionsForJob)

```python
# ListJobExecutionsForJobPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_iot.paginator import ListJobExecutionsForJobPaginator

session = get_session()
async with session.create_client("iot") as client:  # (1)
    paginator: ListJobExecutionsForJobPaginator = client.get_paginator("list_job_executions_for_job")  # (2)
    async for item in paginator.paginate(...):
        item: ListJobExecutionsForJobResponseTypeDef
        print(item)  # (3)
```

1. client: [IoTClient](./client.md)
2. paginator: [ListJobExecutionsForJobPaginator](./paginators.md#listjobexecutionsforjobpaginator)
3. item: `AioPageIterator[ListJobExecutionsForJobResponseTypeDef]`


### paginate

Type annotations and code completion for `#!python ListJobExecutionsForJobPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    jobId: str,
    status: JobExecutionStatusType = ...,  # (1)
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (2)
) -> aiobotocore.paginate.AioPageIterator[ListJobExecutionsForJobResponseTypeDef]:  # (3)
    ...
```

1. See [:material-code-brackets: JobExecutionStatusType](./literals.md#jobexecutionstatustype)
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
3. See `AioPageIterator[ListJobExecutionsForJobResponseTypeDef]`


```python
# paginate method usage example with argument unpacking

kwargs: ListJobExecutionsForJobRequestPaginateTypeDef = {  # (1)
    "jobId": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListJobExecutionsForJobRequestPaginateTypeDef](./type_defs.md#listjobexecutionsforjobrequestpaginatetypedef)
## ListJobExecutionsForThingPaginator

Type annotations and code completion for `#!python session.create_client("iot").get_paginator("list_job_executions_for_thing")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot/paginator/ListJobExecutionsForThing.html#IoT.Paginator.ListJobExecutionsForThing)

```python
# ListJobExecutionsForThingPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_iot.paginator import ListJobExecutionsForThingPaginator

session = get_session()
async with session.create_client("iot") as client:  # (1)
    paginator: ListJobExecutionsForThingPaginator = client.get_paginator("list_job_executions_for_thing")  # (2)
    async for item in paginator.paginate(...):
        item: ListJobExecutionsForThingResponseTypeDef
        print(item)  # (3)
```

1. client: [IoTClient](./client.md)
2. paginator: [ListJobExecutionsForThingPaginator](./paginators.md#listjobexecutionsforthingpaginator)
3. item: `AioPageIterator[ListJobExecutionsForThingResponseTypeDef]`


### paginate

Type annotations and code completion for `#!python ListJobExecutionsForThingPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    thingName: str,
    status: JobExecutionStatusType = ...,  # (1)
    namespaceId: str = ...,
    jobId: str = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (2)
) -> aiobotocore.paginate.AioPageIterator[ListJobExecutionsForThingResponseTypeDef]:  # (3)
    ...
```

1. See [:material-code-brackets: JobExecutionStatusType](./literals.md#jobexecutionstatustype)
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
3. See `AioPageIterator[ListJobExecutionsForThingResponseTypeDef]`


```python
# paginate method usage example with argument unpacking

kwargs: ListJobExecutionsForThingRequestPaginateTypeDef = {  # (1)
    "thingName": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListJobExecutionsForThingRequestPaginateTypeDef](./type_defs.md#listjobexecutionsforthingrequestpaginatetypedef)
## ListJobTemplatesPaginator

Type annotations and code completion for `#!python session.create_client("iot").get_paginator("list_job_templates")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot/paginator/ListJobTemplates.html#IoT.Paginator.ListJobTemplates)

```python
# ListJobTemplatesPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_iot.paginator import ListJobTemplatesPaginator

session = get_session()
async with session.create_client("iot") as client:  # (1)
    paginator: ListJobTemplatesPaginator = client.get_paginator("list_job_templates")  # (2)
    async for item in paginator.paginate(...):
        item: ListJobTemplatesResponseTypeDef
        print(item)  # (3)
```

1. client: [IoTClient](./client.md)
2. paginator: [ListJobTemplatesPaginator](./paginators.md#listjobtemplatespaginator)
3. item: `AioPageIterator[ListJobTemplatesResponseTypeDef]`


### paginate

Type annotations and code completion for `#!python ListJobTemplatesPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> aiobotocore.paginate.AioPageIterator[ListJobTemplatesResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
2. See `AioPageIterator[ListJobTemplatesResponseTypeDef]`


```python
# paginate method usage example with argument unpacking

kwargs: ListJobTemplatesRequestPaginateTypeDef = {  # (1)
    "PaginationConfig": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListJobTemplatesRequestPaginateTypeDef](./type_defs.md#listjobtemplatesrequestpaginatetypedef)
## ListJobsPaginator

Type annotations and code completion for `#!python session.create_client("iot").get_paginator("list_jobs")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot/paginator/ListJobs.html#IoT.Paginator.ListJobs)

```python
# ListJobsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_iot.paginator import ListJobsPaginator

session = get_session()
async with session.create_client("iot") as client:  # (1)
    paginator: ListJobsPaginator = client.get_paginator("list_jobs")  # (2)
    async for item in paginator.paginate(...):
        item: ListJobsResponseTypeDef
        print(item)  # (3)
```

1. client: [IoTClient](./client.md)
2. paginator: [ListJobsPaginator](./paginators.md#listjobspaginator)
3. item: `AioPageIterator[ListJobsResponseTypeDef]`


### paginate

Type annotations and code completion for `#!python ListJobsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    status: JobStatusType = ...,  # (1)
    targetSelection: TargetSelectionType = ...,  # (2)
    thingGroupName: str = ...,
    thingGroupId: str = ...,
    namespaceId: str = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (3)
) -> aiobotocore.paginate.AioPageIterator[ListJobsResponseTypeDef]:  # (4)
    ...
```

1. See [:material-code-brackets: JobStatusType](./literals.md#jobstatustype)
2. See [:material-code-brackets: TargetSelectionType](./literals.md#targetselectiontype)
3. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
4. See `AioPageIterator[ListJobsResponseTypeDef]`


```python
# paginate method usage example with argument unpacking

kwargs: ListJobsRequestPaginateTypeDef = {  # (1)
    "status": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListJobsRequestPaginateTypeDef](./type_defs.md#listjobsrequestpaginatetypedef)
## ListManagedJobTemplatesPaginator

Type annotations and code completion for `#!python session.create_client("iot").get_paginator("list_managed_job_templates")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot/paginator/ListManagedJobTemplates.html#IoT.Paginator.ListManagedJobTemplates)

```python
# ListManagedJobTemplatesPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_iot.paginator import ListManagedJobTemplatesPaginator

session = get_session()
async with session.create_client("iot") as client:  # (1)
    paginator: ListManagedJobTemplatesPaginator = client.get_paginator("list_managed_job_templates")  # (2)
    async for item in paginator.paginate(...):
        item: ListManagedJobTemplatesResponseTypeDef
        print(item)  # (3)
```

1. client: [IoTClient](./client.md)
2. paginator: [ListManagedJobTemplatesPaginator](./paginators.md#listmanagedjobtemplatespaginator)
3. item: `AioPageIterator[ListManagedJobTemplatesResponseTypeDef]`


### paginate

Type annotations and code completion for `#!python ListManagedJobTemplatesPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    templateName: str = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> aiobotocore.paginate.AioPageIterator[ListManagedJobTemplatesResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
2. See `AioPageIterator[ListManagedJobTemplatesResponseTypeDef]`


```python
# paginate method usage example with argument unpacking

kwargs: ListManagedJobTemplatesRequestPaginateTypeDef = {  # (1)
    "templateName": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListManagedJobTemplatesRequestPaginateTypeDef](./type_defs.md#listmanagedjobtemplatesrequestpaginatetypedef)
## ListMetricValuesPaginator

Type annotations and code completion for `#!python session.create_client("iot").get_paginator("list_metric_values")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot/paginator/ListMetricValues.html#IoT.Paginator.ListMetricValues)

```python
# ListMetricValuesPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_iot.paginator import ListMetricValuesPaginator

session = get_session()
async with session.create_client("iot") as client:  # (1)
    paginator: ListMetricValuesPaginator = client.get_paginator("list_metric_values")  # (2)
    async for item in paginator.paginate(...):
        item: ListMetricValuesResponseTypeDef
        print(item)  # (3)
```

1. client: [IoTClient](./client.md)
2. paginator: [ListMetricValuesPaginator](./paginators.md#listmetricvaluespaginator)
3. item: `AioPageIterator[ListMetricValuesResponseTypeDef]`


### paginate

Type annotations and code completion for `#!python ListMetricValuesPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    thingName: str,
    metricName: str,
    startTime: TimestampTypeDef,
    endTime: TimestampTypeDef,
    dimensionName: str = ...,
    dimensionValueOperator: DimensionValueOperatorType = ...,  # (1)
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (2)
) -> aiobotocore.paginate.AioPageIterator[ListMetricValuesResponseTypeDef]:  # (3)
    ...
```

1. See [:material-code-brackets: DimensionValueOperatorType](./literals.md#dimensionvalueoperatortype)
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
3. See `AioPageIterator[ListMetricValuesResponseTypeDef]`


```python
# paginate method usage example with argument unpacking

kwargs: ListMetricValuesRequestPaginateTypeDef = {  # (1)
    "thingName": ...,
    "metricName": ...,
    "startTime": ...,
    "endTime": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListMetricValuesRequestPaginateTypeDef](./type_defs.md#listmetricvaluesrequestpaginatetypedef)
## ListMitigationActionsPaginator

Type annotations and code completion for `#!python session.create_client("iot").get_paginator("list_mitigation_actions")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot/paginator/ListMitigationActions.html#IoT.Paginator.ListMitigationActions)

```python
# ListMitigationActionsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_iot.paginator import ListMitigationActionsPaginator

session = get_session()
async with session.create_client("iot") as client:  # (1)
    paginator: ListMitigationActionsPaginator = client.get_paginator("list_mitigation_actions")  # (2)
    async for item in paginator.paginate(...):
        item: ListMitigationActionsResponseTypeDef
        print(item)  # (3)
```

1. client: [IoTClient](./client.md)
2. paginator: [ListMitigationActionsPaginator](./paginators.md#listmitigationactionspaginator)
3. item: `AioPageIterator[ListMitigationActionsResponseTypeDef]`


### paginate

Type annotations and code completion for `#!python ListMitigationActionsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    actionType: MitigationActionTypeType = ...,  # (1)
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (2)
) -> aiobotocore.paginate.AioPageIterator[ListMitigationActionsResponseTypeDef]:  # (3)
    ...
```

1. See [:material-code-brackets: MitigationActionTypeType](./literals.md#mitigationactiontypetype)
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
3. See `AioPageIterator[ListMitigationActionsResponseTypeDef]`


```python
# paginate method usage example with argument unpacking

kwargs: ListMitigationActionsRequestPaginateTypeDef = {  # (1)
    "actionType": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListMitigationActionsRequestPaginateTypeDef](./type_defs.md#listmitigationactionsrequestpaginatetypedef)
## ListOTAUpdatesPaginator

Type annotations and code completion for `#!python session.create_client("iot").get_paginator("list_ota_updates")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot/paginator/ListOTAUpdates.html#IoT.Paginator.ListOTAUpdates)

```python
# ListOTAUpdatesPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_iot.paginator import ListOTAUpdatesPaginator

session = get_session()
async with session.create_client("iot") as client:  # (1)
    paginator: ListOTAUpdatesPaginator = client.get_paginator("list_ota_updates")  # (2)
    async for item in paginator.paginate(...):
        item: ListOTAUpdatesResponseTypeDef
        print(item)  # (3)
```

1. client: [IoTClient](./client.md)
2. paginator: [ListOTAUpdatesPaginator](./paginators.md#listotaupdatespaginator)
3. item: `AioPageIterator[ListOTAUpdatesResponseTypeDef]`


### paginate

Type annotations and code completion for `#!python ListOTAUpdatesPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    otaUpdateStatus: OTAUpdateStatusType = ...,  # (1)
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (2)
) -> aiobotocore.paginate.AioPageIterator[ListOTAUpdatesResponseTypeDef]:  # (3)
    ...
```

1. See [:material-code-brackets: OTAUpdateStatusType](./literals.md#otaupdatestatustype)
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
3. See `AioPageIterator[ListOTAUpdatesResponseTypeDef]`


```python
# paginate method usage example with argument unpacking

kwargs: ListOTAUpdatesRequestPaginateTypeDef = {  # (1)
    "otaUpdateStatus": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListOTAUpdatesRequestPaginateTypeDef](./type_defs.md#listotaupdatesrequestpaginatetypedef)
## ListOutgoingCertificatesPaginator

Type annotations and code completion for `#!python session.create_client("iot").get_paginator("list_outgoing_certificates")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot/paginator/ListOutgoingCertificates.html#IoT.Paginator.ListOutgoingCertificates)

```python
# ListOutgoingCertificatesPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_iot.paginator import ListOutgoingCertificatesPaginator

session = get_session()
async with session.create_client("iot") as client:  # (1)
    paginator: ListOutgoingCertificatesPaginator = client.get_paginator("list_outgoing_certificates")  # (2)
    async for item in paginator.paginate(...):
        item: ListOutgoingCertificatesResponseTypeDef
        print(item)  # (3)
```

1. client: [IoTClient](./client.md)
2. paginator: [ListOutgoingCertificatesPaginator](./paginators.md#listoutgoingcertificatespaginator)
3. item: `AioPageIterator[ListOutgoingCertificatesResponseTypeDef]`


### paginate

Type annotations and code completion for `#!python ListOutgoingCertificatesPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    ascendingOrder: bool = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> aiobotocore.paginate.AioPageIterator[ListOutgoingCertificatesResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
2. See `AioPageIterator[ListOutgoingCertificatesResponseTypeDef]`


```python
# paginate method usage example with argument unpacking

kwargs: ListOutgoingCertificatesRequestPaginateTypeDef = {  # (1)
    "ascendingOrder": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListOutgoingCertificatesRequestPaginateTypeDef](./type_defs.md#listoutgoingcertificatesrequestpaginatetypedef)
## ListPackageVersionsPaginator

Type annotations and code completion for `#!python session.create_client("iot").get_paginator("list_package_versions")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot/paginator/ListPackageVersions.html#IoT.Paginator.ListPackageVersions)

```python
# ListPackageVersionsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_iot.paginator import ListPackageVersionsPaginator

session = get_session()
async with session.create_client("iot") as client:  # (1)
    paginator: ListPackageVersionsPaginator = client.get_paginator("list_package_versions")  # (2)
    async for item in paginator.paginate(...):
        item: ListPackageVersionsResponseTypeDef
        print(item)  # (3)
```

1. client: [IoTClient](./client.md)
2. paginator: [ListPackageVersionsPaginator](./paginators.md#listpackageversionspaginator)
3. item: `AioPageIterator[ListPackageVersionsResponseTypeDef]`


### paginate

Type annotations and code completion for `#!python ListPackageVersionsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    packageName: str,
    status: PackageVersionStatusType = ...,  # (1)
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (2)
) -> aiobotocore.paginate.AioPageIterator[ListPackageVersionsResponseTypeDef]:  # (3)
    ...
```

1. See [:material-code-brackets: PackageVersionStatusType](./literals.md#packageversionstatustype)
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
3. See `AioPageIterator[ListPackageVersionsResponseTypeDef]`


```python
# paginate method usage example with argument unpacking

kwargs: ListPackageVersionsRequestPaginateTypeDef = {  # (1)
    "packageName": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListPackageVersionsRequestPaginateTypeDef](./type_defs.md#listpackageversionsrequestpaginatetypedef)
## ListPackagesPaginator

Type annotations and code completion for `#!python session.create_client("iot").get_paginator("list_packages")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot/paginator/ListPackages.html#IoT.Paginator.ListPackages)

```python
# ListPackagesPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_iot.paginator import ListPackagesPaginator

session = get_session()
async with session.create_client("iot") as client:  # (1)
    paginator: ListPackagesPaginator = client.get_paginator("list_packages")  # (2)
    async for item in paginator.paginate(...):
        item: ListPackagesResponseTypeDef
        print(item)  # (3)
```

1. client: [IoTClient](./client.md)
2. paginator: [ListPackagesPaginator](./paginators.md#listpackagespaginator)
3. item: `AioPageIterator[ListPackagesResponseTypeDef]`


### paginate

Type annotations and code completion for `#!python ListPackagesPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> aiobotocore.paginate.AioPageIterator[ListPackagesResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
2. See `AioPageIterator[ListPackagesResponseTypeDef]`


```python
# paginate method usage example with argument unpacking

kwargs: ListPackagesRequestPaginateTypeDef = {  # (1)
    "PaginationConfig": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListPackagesRequestPaginateTypeDef](./type_defs.md#listpackagesrequestpaginatetypedef)
## ListPoliciesPaginator

Type annotations and code completion for `#!python session.create_client("iot").get_paginator("list_policies")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot/paginator/ListPolicies.html#IoT.Paginator.ListPolicies)

```python
# ListPoliciesPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_iot.paginator import ListPoliciesPaginator

session = get_session()
async with session.create_client("iot") as client:  # (1)
    paginator: ListPoliciesPaginator = client.get_paginator("list_policies")  # (2)
    async for item in paginator.paginate(...):
        item: ListPoliciesResponseTypeDef
        print(item)  # (3)
```

1. client: [IoTClient](./client.md)
2. paginator: [ListPoliciesPaginator](./paginators.md#listpoliciespaginator)
3. item: `AioPageIterator[ListPoliciesResponseTypeDef]`


### paginate

Type annotations and code completion for `#!python ListPoliciesPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    ascendingOrder: bool = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> aiobotocore.paginate.AioPageIterator[ListPoliciesResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
2. See `AioPageIterator[ListPoliciesResponseTypeDef]`


```python
# paginate method usage example with argument unpacking

kwargs: ListPoliciesRequestPaginateTypeDef = {  # (1)
    "ascendingOrder": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListPoliciesRequestPaginateTypeDef](./type_defs.md#listpoliciesrequestpaginatetypedef)
## ListPolicyPrincipalsPaginator

Type annotations and code completion for `#!python session.create_client("iot").get_paginator("list_policy_principals")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot/paginator/ListPolicyPrincipals.html#IoT.Paginator.ListPolicyPrincipals)

```python
# ListPolicyPrincipalsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_iot.paginator import ListPolicyPrincipalsPaginator

session = get_session()
async with session.create_client("iot") as client:  # (1)
    paginator: ListPolicyPrincipalsPaginator = client.get_paginator("list_policy_principals")  # (2)
    async for item in paginator.paginate(...):
        item: ListPolicyPrincipalsResponseTypeDef
        print(item)  # (3)
```

1. client: [IoTClient](./client.md)
2. paginator: [ListPolicyPrincipalsPaginator](./paginators.md#listpolicyprincipalspaginator)
3. item: `AioPageIterator[ListPolicyPrincipalsResponseTypeDef]`


### paginate

Type annotations and code completion for `#!python ListPolicyPrincipalsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    policyName: str,
    ascendingOrder: bool = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> aiobotocore.paginate.AioPageIterator[ListPolicyPrincipalsResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
2. See `AioPageIterator[ListPolicyPrincipalsResponseTypeDef]`


```python
# paginate method usage example with argument unpacking

kwargs: ListPolicyPrincipalsRequestPaginateTypeDef = {  # (1)
    "policyName": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListPolicyPrincipalsRequestPaginateTypeDef](./type_defs.md#listpolicyprincipalsrequestpaginatetypedef)
## ListPrincipalPoliciesPaginator

Type annotations and code completion for `#!python session.create_client("iot").get_paginator("list_principal_policies")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot/paginator/ListPrincipalPolicies.html#IoT.Paginator.ListPrincipalPolicies)

```python
# ListPrincipalPoliciesPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_iot.paginator import ListPrincipalPoliciesPaginator

session = get_session()
async with session.create_client("iot") as client:  # (1)
    paginator: ListPrincipalPoliciesPaginator = client.get_paginator("list_principal_policies")  # (2)
    async for item in paginator.paginate(...):
        item: ListPrincipalPoliciesResponseTypeDef
        print(item)  # (3)
```

1. client: [IoTClient](./client.md)
2. paginator: [ListPrincipalPoliciesPaginator](./paginators.md#listprincipalpoliciespaginator)
3. item: `AioPageIterator[ListPrincipalPoliciesResponseTypeDef]`


### paginate

Type annotations and code completion for `#!python ListPrincipalPoliciesPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    principal: str,
    ascendingOrder: bool = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> aiobotocore.paginate.AioPageIterator[ListPrincipalPoliciesResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
2. See `AioPageIterator[ListPrincipalPoliciesResponseTypeDef]`


```python
# paginate method usage example with argument unpacking

kwargs: ListPrincipalPoliciesRequestPaginateTypeDef = {  # (1)
    "principal": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListPrincipalPoliciesRequestPaginateTypeDef](./type_defs.md#listprincipalpoliciesrequestpaginatetypedef)
## ListPrincipalThingsPaginator

Type annotations and code completion for `#!python session.create_client("iot").get_paginator("list_principal_things")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot/paginator/ListPrincipalThings.html#IoT.Paginator.ListPrincipalThings)

```python
# ListPrincipalThingsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_iot.paginator import ListPrincipalThingsPaginator

session = get_session()
async with session.create_client("iot") as client:  # (1)
    paginator: ListPrincipalThingsPaginator = client.get_paginator("list_principal_things")  # (2)
    async for item in paginator.paginate(...):
        item: ListPrincipalThingsResponseTypeDef
        print(item)  # (3)
```

1. client: [IoTClient](./client.md)
2. paginator: [ListPrincipalThingsPaginator](./paginators.md#listprincipalthingspaginator)
3. item: `AioPageIterator[ListPrincipalThingsResponseTypeDef]`


### paginate

Type annotations and code completion for `#!python ListPrincipalThingsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    principal: str,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> aiobotocore.paginate.AioPageIterator[ListPrincipalThingsResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
2. See `AioPageIterator[ListPrincipalThingsResponseTypeDef]`


```python
# paginate method usage example with argument unpacking

kwargs: ListPrincipalThingsRequestPaginateTypeDef = {  # (1)
    "principal": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListPrincipalThingsRequestPaginateTypeDef](./type_defs.md#listprincipalthingsrequestpaginatetypedef)
## ListPrincipalThingsV2Paginator

Type annotations and code completion for `#!python session.create_client("iot").get_paginator("list_principal_things_v2")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot/paginator/ListPrincipalThingsV2.html#IoT.Paginator.ListPrincipalThingsV2)

```python
# ListPrincipalThingsV2Paginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_iot.paginator import ListPrincipalThingsV2Paginator

session = get_session()
async with session.create_client("iot") as client:  # (1)
    paginator: ListPrincipalThingsV2Paginator = client.get_paginator("list_principal_things_v2")  # (2)
    async for item in paginator.paginate(...):
        item: ListPrincipalThingsV2ResponseTypeDef
        print(item)  # (3)
```

1. client: [IoTClient](./client.md)
2. paginator: [ListPrincipalThingsV2Paginator](./paginators.md#listprincipalthingsv2paginator)
3. item: `AioPageIterator[ListPrincipalThingsV2ResponseTypeDef]`


### paginate

Type annotations and code completion for `#!python ListPrincipalThingsV2Paginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    principal: str,
    thingPrincipalType: ThingPrincipalTypeType = ...,  # (1)
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (2)
) -> aiobotocore.paginate.AioPageIterator[ListPrincipalThingsV2ResponseTypeDef]:  # (3)
    ...
```

1. See [:material-code-brackets: ThingPrincipalTypeType](./literals.md#thingprincipaltypetype)
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
3. See `AioPageIterator[ListPrincipalThingsV2ResponseTypeDef]`


```python
# paginate method usage example with argument unpacking

kwargs: ListPrincipalThingsV2RequestPaginateTypeDef = {  # (1)
    "principal": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListPrincipalThingsV2RequestPaginateTypeDef](./type_defs.md#listprincipalthingsv2requestpaginatetypedef)
## ListProvisioningTemplateVersionsPaginator

Type annotations and code completion for `#!python session.create_client("iot").get_paginator("list_provisioning_template_versions")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot/paginator/ListProvisioningTemplateVersions.html#IoT.Paginator.ListProvisioningTemplateVersions)

```python
# ListProvisioningTemplateVersionsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_iot.paginator import ListProvisioningTemplateVersionsPaginator

session = get_session()
async with session.create_client("iot") as client:  # (1)
    paginator: ListProvisioningTemplateVersionsPaginator = client.get_paginator("list_provisioning_template_versions")  # (2)
    async for item in paginator.paginate(...):
        item: ListProvisioningTemplateVersionsResponseTypeDef
        print(item)  # (3)
```

1. client: [IoTClient](./client.md)
2. paginator: [ListProvisioningTemplateVersionsPaginator](./paginators.md#listprovisioningtemplateversionspaginator)
3. item: `AioPageIterator[ListProvisioningTemplateVersionsResponseTypeDef]`


### paginate

Type annotations and code completion for `#!python ListProvisioningTemplateVersionsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    templateName: str,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> aiobotocore.paginate.AioPageIterator[ListProvisioningTemplateVersionsResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
2. See `AioPageIterator[ListProvisioningTemplateVersionsResponseTypeDef]`


```python
# paginate method usage example with argument unpacking

kwargs: ListProvisioningTemplateVersionsRequestPaginateTypeDef = {  # (1)
    "templateName": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListProvisioningTemplateVersionsRequestPaginateTypeDef](./type_defs.md#listprovisioningtemplateversionsrequestpaginatetypedef)
## ListProvisioningTemplatesPaginator

Type annotations and code completion for `#!python session.create_client("iot").get_paginator("list_provisioning_templates")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot/paginator/ListProvisioningTemplates.html#IoT.Paginator.ListProvisioningTemplates)

```python
# ListProvisioningTemplatesPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_iot.paginator import ListProvisioningTemplatesPaginator

session = get_session()
async with session.create_client("iot") as client:  # (1)
    paginator: ListProvisioningTemplatesPaginator = client.get_paginator("list_provisioning_templates")  # (2)
    async for item in paginator.paginate(...):
        item: ListProvisioningTemplatesResponseTypeDef
        print(item)  # (3)
```

1. client: [IoTClient](./client.md)
2. paginator: [ListProvisioningTemplatesPaginator](./paginators.md#listprovisioningtemplatespaginator)
3. item: `AioPageIterator[ListProvisioningTemplatesResponseTypeDef]`


### paginate

Type annotations and code completion for `#!python ListProvisioningTemplatesPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> aiobotocore.paginate.AioPageIterator[ListProvisioningTemplatesResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
2. See `AioPageIterator[ListProvisioningTemplatesResponseTypeDef]`


```python
# paginate method usage example with argument unpacking

kwargs: ListProvisioningTemplatesRequestPaginateTypeDef = {  # (1)
    "PaginationConfig": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListProvisioningTemplatesRequestPaginateTypeDef](./type_defs.md#listprovisioningtemplatesrequestpaginatetypedef)
## ListRelatedResourcesForAuditFindingPaginator

Type annotations and code completion for `#!python session.create_client("iot").get_paginator("list_related_resources_for_audit_finding")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot/paginator/ListRelatedResourcesForAuditFinding.html#IoT.Paginator.ListRelatedResourcesForAuditFinding)

```python
# ListRelatedResourcesForAuditFindingPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_iot.paginator import ListRelatedResourcesForAuditFindingPaginator

session = get_session()
async with session.create_client("iot") as client:  # (1)
    paginator: ListRelatedResourcesForAuditFindingPaginator = client.get_paginator("list_related_resources_for_audit_finding")  # (2)
    async for item in paginator.paginate(...):
        item: ListRelatedResourcesForAuditFindingResponseTypeDef
        print(item)  # (3)
```

1. client: [IoTClient](./client.md)
2. paginator: [ListRelatedResourcesForAuditFindingPaginator](./paginators.md#listrelatedresourcesforauditfindingpaginator)
3. item: `AioPageIterator[ListRelatedResourcesForAuditFindingResponseTypeDef]`


### paginate

Type annotations and code completion for `#!python ListRelatedResourcesForAuditFindingPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    findingId: str,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> aiobotocore.paginate.AioPageIterator[ListRelatedResourcesForAuditFindingResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
2. See `AioPageIterator[ListRelatedResourcesForAuditFindingResponseTypeDef]`


```python
# paginate method usage example with argument unpacking

kwargs: ListRelatedResourcesForAuditFindingRequestPaginateTypeDef = {  # (1)
    "findingId": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListRelatedResourcesForAuditFindingRequestPaginateTypeDef](./type_defs.md#listrelatedresourcesforauditfindingrequestpaginatetypedef)
## ListRoleAliasesPaginator

Type annotations and code completion for `#!python session.create_client("iot").get_paginator("list_role_aliases")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot/paginator/ListRoleAliases.html#IoT.Paginator.ListRoleAliases)

```python
# ListRoleAliasesPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_iot.paginator import ListRoleAliasesPaginator

session = get_session()
async with session.create_client("iot") as client:  # (1)
    paginator: ListRoleAliasesPaginator = client.get_paginator("list_role_aliases")  # (2)
    async for item in paginator.paginate(...):
        item: ListRoleAliasesResponseTypeDef
        print(item)  # (3)
```

1. client: [IoTClient](./client.md)
2. paginator: [ListRoleAliasesPaginator](./paginators.md#listrolealiasespaginator)
3. item: `AioPageIterator[ListRoleAliasesResponseTypeDef]`


### paginate

Type annotations and code completion for `#!python ListRoleAliasesPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    ascendingOrder: bool = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> aiobotocore.paginate.AioPageIterator[ListRoleAliasesResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
2. See `AioPageIterator[ListRoleAliasesResponseTypeDef]`


```python
# paginate method usage example with argument unpacking

kwargs: ListRoleAliasesRequestPaginateTypeDef = {  # (1)
    "ascendingOrder": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListRoleAliasesRequestPaginateTypeDef](./type_defs.md#listrolealiasesrequestpaginatetypedef)
## ListSbomValidationResultsPaginator

Type annotations and code completion for `#!python session.create_client("iot").get_paginator("list_sbom_validation_results")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot/paginator/ListSbomValidationResults.html#IoT.Paginator.ListSbomValidationResults)

```python
# ListSbomValidationResultsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_iot.paginator import ListSbomValidationResultsPaginator

session = get_session()
async with session.create_client("iot") as client:  # (1)
    paginator: ListSbomValidationResultsPaginator = client.get_paginator("list_sbom_validation_results")  # (2)
    async for item in paginator.paginate(...):
        item: ListSbomValidationResultsResponseTypeDef
        print(item)  # (3)
```

1. client: [IoTClient](./client.md)
2. paginator: [ListSbomValidationResultsPaginator](./paginators.md#listsbomvalidationresultspaginator)
3. item: `AioPageIterator[ListSbomValidationResultsResponseTypeDef]`


### paginate

Type annotations and code completion for `#!python ListSbomValidationResultsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    packageName: str,
    versionName: str,
    validationResult: SbomValidationResultType = ...,  # (1)
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (2)
) -> aiobotocore.paginate.AioPageIterator[ListSbomValidationResultsResponseTypeDef]:  # (3)
    ...
```

1. See [:material-code-brackets: SbomValidationResultType](./literals.md#sbomvalidationresulttype)
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
3. See `AioPageIterator[ListSbomValidationResultsResponseTypeDef]`


```python
# paginate method usage example with argument unpacking

kwargs: ListSbomValidationResultsRequestPaginateTypeDef = {  # (1)
    "packageName": ...,
    "versionName": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListSbomValidationResultsRequestPaginateTypeDef](./type_defs.md#listsbomvalidationresultsrequestpaginatetypedef)
## ListScheduledAuditsPaginator

Type annotations and code completion for `#!python session.create_client("iot").get_paginator("list_scheduled_audits")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot/paginator/ListScheduledAudits.html#IoT.Paginator.ListScheduledAudits)

```python
# ListScheduledAuditsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_iot.paginator import ListScheduledAuditsPaginator

session = get_session()
async with session.create_client("iot") as client:  # (1)
    paginator: ListScheduledAuditsPaginator = client.get_paginator("list_scheduled_audits")  # (2)
    async for item in paginator.paginate(...):
        item: ListScheduledAuditsResponseTypeDef
        print(item)  # (3)
```

1. client: [IoTClient](./client.md)
2. paginator: [ListScheduledAuditsPaginator](./paginators.md#listscheduledauditspaginator)
3. item: `AioPageIterator[ListScheduledAuditsResponseTypeDef]`


### paginate

Type annotations and code completion for `#!python ListScheduledAuditsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> aiobotocore.paginate.AioPageIterator[ListScheduledAuditsResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
2. See `AioPageIterator[ListScheduledAuditsResponseTypeDef]`


```python
# paginate method usage example with argument unpacking

kwargs: ListScheduledAuditsRequestPaginateTypeDef = {  # (1)
    "PaginationConfig": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListScheduledAuditsRequestPaginateTypeDef](./type_defs.md#listscheduledauditsrequestpaginatetypedef)
## ListSecurityProfilesForTargetPaginator

Type annotations and code completion for `#!python session.create_client("iot").get_paginator("list_security_profiles_for_target")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot/paginator/ListSecurityProfilesForTarget.html#IoT.Paginator.ListSecurityProfilesForTarget)

```python
# ListSecurityProfilesForTargetPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_iot.paginator import ListSecurityProfilesForTargetPaginator

session = get_session()
async with session.create_client("iot") as client:  # (1)
    paginator: ListSecurityProfilesForTargetPaginator = client.get_paginator("list_security_profiles_for_target")  # (2)
    async for item in paginator.paginate(...):
        item: ListSecurityProfilesForTargetResponseTypeDef
        print(item)  # (3)
```

1. client: [IoTClient](./client.md)
2. paginator: [ListSecurityProfilesForTargetPaginator](./paginators.md#listsecurityprofilesfortargetpaginator)
3. item: `AioPageIterator[ListSecurityProfilesForTargetResponseTypeDef]`


### paginate

Type annotations and code completion for `#!python ListSecurityProfilesForTargetPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    securityProfileTargetArn: str,
    recursive: bool = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> aiobotocore.paginate.AioPageIterator[ListSecurityProfilesForTargetResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
2. See `AioPageIterator[ListSecurityProfilesForTargetResponseTypeDef]`


```python
# paginate method usage example with argument unpacking

kwargs: ListSecurityProfilesForTargetRequestPaginateTypeDef = {  # (1)
    "securityProfileTargetArn": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListSecurityProfilesForTargetRequestPaginateTypeDef](./type_defs.md#listsecurityprofilesfortargetrequestpaginatetypedef)
## ListSecurityProfilesPaginator

Type annotations and code completion for `#!python session.create_client("iot").get_paginator("list_security_profiles")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot/paginator/ListSecurityProfiles.html#IoT.Paginator.ListSecurityProfiles)

```python
# ListSecurityProfilesPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_iot.paginator import ListSecurityProfilesPaginator

session = get_session()
async with session.create_client("iot") as client:  # (1)
    paginator: ListSecurityProfilesPaginator = client.get_paginator("list_security_profiles")  # (2)
    async for item in paginator.paginate(...):
        item: ListSecurityProfilesResponseTypeDef
        print(item)  # (3)
```

1. client: [IoTClient](./client.md)
2. paginator: [ListSecurityProfilesPaginator](./paginators.md#listsecurityprofilespaginator)
3. item: `AioPageIterator[ListSecurityProfilesResponseTypeDef]`


### paginate

Type annotations and code completion for `#!python ListSecurityProfilesPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    dimensionName: str = ...,
    metricName: str = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> aiobotocore.paginate.AioPageIterator[ListSecurityProfilesResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
2. See `AioPageIterator[ListSecurityProfilesResponseTypeDef]`


```python
# paginate method usage example with argument unpacking

kwargs: ListSecurityProfilesRequestPaginateTypeDef = {  # (1)
    "dimensionName": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListSecurityProfilesRequestPaginateTypeDef](./type_defs.md#listsecurityprofilesrequestpaginatetypedef)
## ListStreamsPaginator

Type annotations and code completion for `#!python session.create_client("iot").get_paginator("list_streams")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot/paginator/ListStreams.html#IoT.Paginator.ListStreams)

```python
# ListStreamsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_iot.paginator import ListStreamsPaginator

session = get_session()
async with session.create_client("iot") as client:  # (1)
    paginator: ListStreamsPaginator = client.get_paginator("list_streams")  # (2)
    async for item in paginator.paginate(...):
        item: ListStreamsResponseTypeDef
        print(item)  # (3)
```

1. client: [IoTClient](./client.md)
2. paginator: [ListStreamsPaginator](./paginators.md#liststreamspaginator)
3. item: `AioPageIterator[ListStreamsResponseTypeDef]`


### paginate

Type annotations and code completion for `#!python ListStreamsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    ascendingOrder: bool = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> aiobotocore.paginate.AioPageIterator[ListStreamsResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
2. See `AioPageIterator[ListStreamsResponseTypeDef]`


```python
# paginate method usage example with argument unpacking

kwargs: ListStreamsRequestPaginateTypeDef = {  # (1)
    "ascendingOrder": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListStreamsRequestPaginateTypeDef](./type_defs.md#liststreamsrequestpaginatetypedef)
## ListTagsForResourcePaginator

Type annotations and code completion for `#!python session.create_client("iot").get_paginator("list_tags_for_resource")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot/paginator/ListTagsForResource.html#IoT.Paginator.ListTagsForResource)

```python
# ListTagsForResourcePaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_iot.paginator import ListTagsForResourcePaginator

session = get_session()
async with session.create_client("iot") as client:  # (1)
    paginator: ListTagsForResourcePaginator = client.get_paginator("list_tags_for_resource")  # (2)
    async for item in paginator.paginate(...):
        item: ListTagsForResourceResponseTypeDef
        print(item)  # (3)
```

1. client: [IoTClient](./client.md)
2. paginator: [ListTagsForResourcePaginator](./paginators.md#listtagsforresourcepaginator)
3. item: `AioPageIterator[ListTagsForResourceResponseTypeDef]`


### paginate

Type annotations and code completion for `#!python ListTagsForResourcePaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    resourceArn: str,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> aiobotocore.paginate.AioPageIterator[ListTagsForResourceResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
2. See `AioPageIterator[ListTagsForResourceResponseTypeDef]`


```python
# paginate method usage example with argument unpacking

kwargs: ListTagsForResourceRequestPaginateTypeDef = {  # (1)
    "resourceArn": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListTagsForResourceRequestPaginateTypeDef](./type_defs.md#listtagsforresourcerequestpaginatetypedef)
## ListTargetsForPolicyPaginator

Type annotations and code completion for `#!python session.create_client("iot").get_paginator("list_targets_for_policy")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot/paginator/ListTargetsForPolicy.html#IoT.Paginator.ListTargetsForPolicy)

```python
# ListTargetsForPolicyPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_iot.paginator import ListTargetsForPolicyPaginator

session = get_session()
async with session.create_client("iot") as client:  # (1)
    paginator: ListTargetsForPolicyPaginator = client.get_paginator("list_targets_for_policy")  # (2)
    async for item in paginator.paginate(...):
        item: ListTargetsForPolicyResponseTypeDef
        print(item)  # (3)
```

1. client: [IoTClient](./client.md)
2. paginator: [ListTargetsForPolicyPaginator](./paginators.md#listtargetsforpolicypaginator)
3. item: `AioPageIterator[ListTargetsForPolicyResponseTypeDef]`


### paginate

Type annotations and code completion for `#!python ListTargetsForPolicyPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    policyName: str,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> aiobotocore.paginate.AioPageIterator[ListTargetsForPolicyResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
2. See `AioPageIterator[ListTargetsForPolicyResponseTypeDef]`


```python
# paginate method usage example with argument unpacking

kwargs: ListTargetsForPolicyRequestPaginateTypeDef = {  # (1)
    "policyName": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListTargetsForPolicyRequestPaginateTypeDef](./type_defs.md#listtargetsforpolicyrequestpaginatetypedef)
## ListTargetsForSecurityProfilePaginator

Type annotations and code completion for `#!python session.create_client("iot").get_paginator("list_targets_for_security_profile")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot/paginator/ListTargetsForSecurityProfile.html#IoT.Paginator.ListTargetsForSecurityProfile)

```python
# ListTargetsForSecurityProfilePaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_iot.paginator import ListTargetsForSecurityProfilePaginator

session = get_session()
async with session.create_client("iot") as client:  # (1)
    paginator: ListTargetsForSecurityProfilePaginator = client.get_paginator("list_targets_for_security_profile")  # (2)
    async for item in paginator.paginate(...):
        item: ListTargetsForSecurityProfileResponseTypeDef
        print(item)  # (3)
```

1. client: [IoTClient](./client.md)
2. paginator: [ListTargetsForSecurityProfilePaginator](./paginators.md#listtargetsforsecurityprofilepaginator)
3. item: `AioPageIterator[ListTargetsForSecurityProfileResponseTypeDef]`


### paginate

Type annotations and code completion for `#!python ListTargetsForSecurityProfilePaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    securityProfileName: str,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> aiobotocore.paginate.AioPageIterator[ListTargetsForSecurityProfileResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
2. See `AioPageIterator[ListTargetsForSecurityProfileResponseTypeDef]`


```python
# paginate method usage example with argument unpacking

kwargs: ListTargetsForSecurityProfileRequestPaginateTypeDef = {  # (1)
    "securityProfileName": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListTargetsForSecurityProfileRequestPaginateTypeDef](./type_defs.md#listtargetsforsecurityprofilerequestpaginatetypedef)
## ListThingGroupsForThingPaginator

Type annotations and code completion for `#!python session.create_client("iot").get_paginator("list_thing_groups_for_thing")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot/paginator/ListThingGroupsForThing.html#IoT.Paginator.ListThingGroupsForThing)

```python
# ListThingGroupsForThingPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_iot.paginator import ListThingGroupsForThingPaginator

session = get_session()
async with session.create_client("iot") as client:  # (1)
    paginator: ListThingGroupsForThingPaginator = client.get_paginator("list_thing_groups_for_thing")  # (2)
    async for item in paginator.paginate(...):
        item: ListThingGroupsForThingResponseTypeDef
        print(item)  # (3)
```

1. client: [IoTClient](./client.md)
2. paginator: [ListThingGroupsForThingPaginator](./paginators.md#listthinggroupsforthingpaginator)
3. item: `AioPageIterator[ListThingGroupsForThingResponseTypeDef]`


### paginate

Type annotations and code completion for `#!python ListThingGroupsForThingPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    thingName: str,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> aiobotocore.paginate.AioPageIterator[ListThingGroupsForThingResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
2. See `AioPageIterator[ListThingGroupsForThingResponseTypeDef]`


```python
# paginate method usage example with argument unpacking

kwargs: ListThingGroupsForThingRequestPaginateTypeDef = {  # (1)
    "thingName": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListThingGroupsForThingRequestPaginateTypeDef](./type_defs.md#listthinggroupsforthingrequestpaginatetypedef)
## ListThingGroupsPaginator

Type annotations and code completion for `#!python session.create_client("iot").get_paginator("list_thing_groups")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot/paginator/ListThingGroups.html#IoT.Paginator.ListThingGroups)

```python
# ListThingGroupsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_iot.paginator import ListThingGroupsPaginator

session = get_session()
async with session.create_client("iot") as client:  # (1)
    paginator: ListThingGroupsPaginator = client.get_paginator("list_thing_groups")  # (2)
    async for item in paginator.paginate(...):
        item: ListThingGroupsResponseTypeDef
        print(item)  # (3)
```

1. client: [IoTClient](./client.md)
2. paginator: [ListThingGroupsPaginator](./paginators.md#listthinggroupspaginator)
3. item: `AioPageIterator[ListThingGroupsResponseTypeDef]`


### paginate

Type annotations and code completion for `#!python ListThingGroupsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    parentGroup: str = ...,
    namePrefixFilter: str = ...,
    recursive: bool = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> aiobotocore.paginate.AioPageIterator[ListThingGroupsResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
2. See `AioPageIterator[ListThingGroupsResponseTypeDef]`


```python
# paginate method usage example with argument unpacking

kwargs: ListThingGroupsRequestPaginateTypeDef = {  # (1)
    "parentGroup": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListThingGroupsRequestPaginateTypeDef](./type_defs.md#listthinggroupsrequestpaginatetypedef)
## ListThingPrincipalsPaginator

Type annotations and code completion for `#!python session.create_client("iot").get_paginator("list_thing_principals")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot/paginator/ListThingPrincipals.html#IoT.Paginator.ListThingPrincipals)

```python
# ListThingPrincipalsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_iot.paginator import ListThingPrincipalsPaginator

session = get_session()
async with session.create_client("iot") as client:  # (1)
    paginator: ListThingPrincipalsPaginator = client.get_paginator("list_thing_principals")  # (2)
    async for item in paginator.paginate(...):
        item: ListThingPrincipalsResponseTypeDef
        print(item)  # (3)
```

1. client: [IoTClient](./client.md)
2. paginator: [ListThingPrincipalsPaginator](./paginators.md#listthingprincipalspaginator)
3. item: `AioPageIterator[ListThingPrincipalsResponseTypeDef]`


### paginate

Type annotations and code completion for `#!python ListThingPrincipalsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    thingName: str,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> aiobotocore.paginate.AioPageIterator[ListThingPrincipalsResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
2. See `AioPageIterator[ListThingPrincipalsResponseTypeDef]`


```python
# paginate method usage example with argument unpacking

kwargs: ListThingPrincipalsRequestPaginateTypeDef = {  # (1)
    "thingName": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListThingPrincipalsRequestPaginateTypeDef](./type_defs.md#listthingprincipalsrequestpaginatetypedef)
## ListThingPrincipalsV2Paginator

Type annotations and code completion for `#!python session.create_client("iot").get_paginator("list_thing_principals_v2")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot/paginator/ListThingPrincipalsV2.html#IoT.Paginator.ListThingPrincipalsV2)

```python
# ListThingPrincipalsV2Paginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_iot.paginator import ListThingPrincipalsV2Paginator

session = get_session()
async with session.create_client("iot") as client:  # (1)
    paginator: ListThingPrincipalsV2Paginator = client.get_paginator("list_thing_principals_v2")  # (2)
    async for item in paginator.paginate(...):
        item: ListThingPrincipalsV2ResponseTypeDef
        print(item)  # (3)
```

1. client: [IoTClient](./client.md)
2. paginator: [ListThingPrincipalsV2Paginator](./paginators.md#listthingprincipalsv2paginator)
3. item: `AioPageIterator[ListThingPrincipalsV2ResponseTypeDef]`


### paginate

Type annotations and code completion for `#!python ListThingPrincipalsV2Paginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    thingName: str,
    thingPrincipalType: ThingPrincipalTypeType = ...,  # (1)
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (2)
) -> aiobotocore.paginate.AioPageIterator[ListThingPrincipalsV2ResponseTypeDef]:  # (3)
    ...
```

1. See [:material-code-brackets: ThingPrincipalTypeType](./literals.md#thingprincipaltypetype)
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
3. See `AioPageIterator[ListThingPrincipalsV2ResponseTypeDef]`


```python
# paginate method usage example with argument unpacking

kwargs: ListThingPrincipalsV2RequestPaginateTypeDef = {  # (1)
    "thingName": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListThingPrincipalsV2RequestPaginateTypeDef](./type_defs.md#listthingprincipalsv2requestpaginatetypedef)
## ListThingRegistrationTaskReportsPaginator

Type annotations and code completion for `#!python session.create_client("iot").get_paginator("list_thing_registration_task_reports")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot/paginator/ListThingRegistrationTaskReports.html#IoT.Paginator.ListThingRegistrationTaskReports)

```python
# ListThingRegistrationTaskReportsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_iot.paginator import ListThingRegistrationTaskReportsPaginator

session = get_session()
async with session.create_client("iot") as client:  # (1)
    paginator: ListThingRegistrationTaskReportsPaginator = client.get_paginator("list_thing_registration_task_reports")  # (2)
    async for item in paginator.paginate(...):
        item: ListThingRegistrationTaskReportsResponseTypeDef
        print(item)  # (3)
```

1. client: [IoTClient](./client.md)
2. paginator: [ListThingRegistrationTaskReportsPaginator](./paginators.md#listthingregistrationtaskreportspaginator)
3. item: `AioPageIterator[ListThingRegistrationTaskReportsResponseTypeDef]`


### paginate

Type annotations and code completion for `#!python ListThingRegistrationTaskReportsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    taskId: str,
    reportType: ReportTypeType,  # (1)
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (2)
) -> aiobotocore.paginate.AioPageIterator[ListThingRegistrationTaskReportsResponseTypeDef]:  # (3)
    ...
```

1. See [:material-code-brackets: ReportTypeType](./literals.md#reporttypetype)
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
3. See `AioPageIterator[ListThingRegistrationTaskReportsResponseTypeDef]`


```python
# paginate method usage example with argument unpacking

kwargs: ListThingRegistrationTaskReportsRequestPaginateTypeDef = {  # (1)
    "taskId": ...,
    "reportType": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListThingRegistrationTaskReportsRequestPaginateTypeDef](./type_defs.md#listthingregistrationtaskreportsrequestpaginatetypedef)
## ListThingRegistrationTasksPaginator

Type annotations and code completion for `#!python session.create_client("iot").get_paginator("list_thing_registration_tasks")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot/paginator/ListThingRegistrationTasks.html#IoT.Paginator.ListThingRegistrationTasks)

```python
# ListThingRegistrationTasksPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_iot.paginator import ListThingRegistrationTasksPaginator

session = get_session()
async with session.create_client("iot") as client:  # (1)
    paginator: ListThingRegistrationTasksPaginator = client.get_paginator("list_thing_registration_tasks")  # (2)
    async for item in paginator.paginate(...):
        item: ListThingRegistrationTasksResponseTypeDef
        print(item)  # (3)
```

1. client: [IoTClient](./client.md)
2. paginator: [ListThingRegistrationTasksPaginator](./paginators.md#listthingregistrationtaskspaginator)
3. item: `AioPageIterator[ListThingRegistrationTasksResponseTypeDef]`


### paginate

Type annotations and code completion for `#!python ListThingRegistrationTasksPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    status: StatusType = ...,  # (1)
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (2)
) -> aiobotocore.paginate.AioPageIterator[ListThingRegistrationTasksResponseTypeDef]:  # (3)
    ...
```

1. See [:material-code-brackets: StatusType](./literals.md#statustype)
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
3. See `AioPageIterator[ListThingRegistrationTasksResponseTypeDef]`


```python
# paginate method usage example with argument unpacking

kwargs: ListThingRegistrationTasksRequestPaginateTypeDef = {  # (1)
    "status": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListThingRegistrationTasksRequestPaginateTypeDef](./type_defs.md#listthingregistrationtasksrequestpaginatetypedef)
## ListThingTypesPaginator

Type annotations and code completion for `#!python session.create_client("iot").get_paginator("list_thing_types")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot/paginator/ListThingTypes.html#IoT.Paginator.ListThingTypes)

```python
# ListThingTypesPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_iot.paginator import ListThingTypesPaginator

session = get_session()
async with session.create_client("iot") as client:  # (1)
    paginator: ListThingTypesPaginator = client.get_paginator("list_thing_types")  # (2)
    async for item in paginator.paginate(...):
        item: ListThingTypesResponseTypeDef
        print(item)  # (3)
```

1. client: [IoTClient](./client.md)
2. paginator: [ListThingTypesPaginator](./paginators.md#listthingtypespaginator)
3. item: `AioPageIterator[ListThingTypesResponseTypeDef]`


### paginate

Type annotations and code completion for `#!python ListThingTypesPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    thingTypeName: str = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> aiobotocore.paginate.AioPageIterator[ListThingTypesResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
2. See `AioPageIterator[ListThingTypesResponseTypeDef]`


```python
# paginate method usage example with argument unpacking

kwargs: ListThingTypesRequestPaginateTypeDef = {  # (1)
    "thingTypeName": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListThingTypesRequestPaginateTypeDef](./type_defs.md#listthingtypesrequestpaginatetypedef)
## ListThingsInBillingGroupPaginator

Type annotations and code completion for `#!python session.create_client("iot").get_paginator("list_things_in_billing_group")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot/paginator/ListThingsInBillingGroup.html#IoT.Paginator.ListThingsInBillingGroup)

```python
# ListThingsInBillingGroupPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_iot.paginator import ListThingsInBillingGroupPaginator

session = get_session()
async with session.create_client("iot") as client:  # (1)
    paginator: ListThingsInBillingGroupPaginator = client.get_paginator("list_things_in_billing_group")  # (2)
    async for item in paginator.paginate(...):
        item: ListThingsInBillingGroupResponseTypeDef
        print(item)  # (3)
```

1. client: [IoTClient](./client.md)
2. paginator: [ListThingsInBillingGroupPaginator](./paginators.md#listthingsinbillinggrouppaginator)
3. item: `AioPageIterator[ListThingsInBillingGroupResponseTypeDef]`


### paginate

Type annotations and code completion for `#!python ListThingsInBillingGroupPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    billingGroupName: str,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> aiobotocore.paginate.AioPageIterator[ListThingsInBillingGroupResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
2. See `AioPageIterator[ListThingsInBillingGroupResponseTypeDef]`


```python
# paginate method usage example with argument unpacking

kwargs: ListThingsInBillingGroupRequestPaginateTypeDef = {  # (1)
    "billingGroupName": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListThingsInBillingGroupRequestPaginateTypeDef](./type_defs.md#listthingsinbillinggrouprequestpaginatetypedef)
## ListThingsInThingGroupPaginator

Type annotations and code completion for `#!python session.create_client("iot").get_paginator("list_things_in_thing_group")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot/paginator/ListThingsInThingGroup.html#IoT.Paginator.ListThingsInThingGroup)

```python
# ListThingsInThingGroupPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_iot.paginator import ListThingsInThingGroupPaginator

session = get_session()
async with session.create_client("iot") as client:  # (1)
    paginator: ListThingsInThingGroupPaginator = client.get_paginator("list_things_in_thing_group")  # (2)
    async for item in paginator.paginate(...):
        item: ListThingsInThingGroupResponseTypeDef
        print(item)  # (3)
```

1. client: [IoTClient](./client.md)
2. paginator: [ListThingsInThingGroupPaginator](./paginators.md#listthingsinthinggrouppaginator)
3. item: `AioPageIterator[ListThingsInThingGroupResponseTypeDef]`


### paginate

Type annotations and code completion for `#!python ListThingsInThingGroupPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    thingGroupName: str,
    recursive: bool = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> aiobotocore.paginate.AioPageIterator[ListThingsInThingGroupResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
2. See `AioPageIterator[ListThingsInThingGroupResponseTypeDef]`


```python
# paginate method usage example with argument unpacking

kwargs: ListThingsInThingGroupRequestPaginateTypeDef = {  # (1)
    "thingGroupName": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListThingsInThingGroupRequestPaginateTypeDef](./type_defs.md#listthingsinthinggrouprequestpaginatetypedef)
## ListThingsPaginator

Type annotations and code completion for `#!python session.create_client("iot").get_paginator("list_things")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot/paginator/ListThings.html#IoT.Paginator.ListThings)

```python
# ListThingsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_iot.paginator import ListThingsPaginator

session = get_session()
async with session.create_client("iot") as client:  # (1)
    paginator: ListThingsPaginator = client.get_paginator("list_things")  # (2)
    async for item in paginator.paginate(...):
        item: ListThingsResponseTypeDef
        print(item)  # (3)
```

1. client: [IoTClient](./client.md)
2. paginator: [ListThingsPaginator](./paginators.md#listthingspaginator)
3. item: `AioPageIterator[ListThingsResponseTypeDef]`


### paginate

Type annotations and code completion for `#!python ListThingsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    attributeName: str = ...,
    attributeValue: str = ...,
    thingTypeName: str = ...,
    usePrefixAttributeValue: bool = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> aiobotocore.paginate.AioPageIterator[ListThingsResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
2. See `AioPageIterator[ListThingsResponseTypeDef]`


```python
# paginate method usage example with argument unpacking

kwargs: ListThingsRequestPaginateTypeDef = {  # (1)
    "attributeName": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListThingsRequestPaginateTypeDef](./type_defs.md#listthingsrequestpaginatetypedef)
## ListTopicRuleDestinationsPaginator

Type annotations and code completion for `#!python session.create_client("iot").get_paginator("list_topic_rule_destinations")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot/paginator/ListTopicRuleDestinations.html#IoT.Paginator.ListTopicRuleDestinations)

```python
# ListTopicRuleDestinationsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_iot.paginator import ListTopicRuleDestinationsPaginator

session = get_session()
async with session.create_client("iot") as client:  # (1)
    paginator: ListTopicRuleDestinationsPaginator = client.get_paginator("list_topic_rule_destinations")  # (2)
    async for item in paginator.paginate(...):
        item: ListTopicRuleDestinationsResponseTypeDef
        print(item)  # (3)
```

1. client: [IoTClient](./client.md)
2. paginator: [ListTopicRuleDestinationsPaginator](./paginators.md#listtopicruledestinationspaginator)
3. item: `AioPageIterator[ListTopicRuleDestinationsResponseTypeDef]`


### paginate

Type annotations and code completion for `#!python ListTopicRuleDestinationsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> aiobotocore.paginate.AioPageIterator[ListTopicRuleDestinationsResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
2. See `AioPageIterator[ListTopicRuleDestinationsResponseTypeDef]`


```python
# paginate method usage example with argument unpacking

kwargs: ListTopicRuleDestinationsRequestPaginateTypeDef = {  # (1)
    "PaginationConfig": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListTopicRuleDestinationsRequestPaginateTypeDef](./type_defs.md#listtopicruledestinationsrequestpaginatetypedef)
## ListTopicRulesPaginator

Type annotations and code completion for `#!python session.create_client("iot").get_paginator("list_topic_rules")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot/paginator/ListTopicRules.html#IoT.Paginator.ListTopicRules)

```python
# ListTopicRulesPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_iot.paginator import ListTopicRulesPaginator

session = get_session()
async with session.create_client("iot") as client:  # (1)
    paginator: ListTopicRulesPaginator = client.get_paginator("list_topic_rules")  # (2)
    async for item in paginator.paginate(...):
        item: ListTopicRulesResponseTypeDef
        print(item)  # (3)
```

1. client: [IoTClient](./client.md)
2. paginator: [ListTopicRulesPaginator](./paginators.md#listtopicrulespaginator)
3. item: `AioPageIterator[ListTopicRulesResponseTypeDef]`


### paginate

Type annotations and code completion for `#!python ListTopicRulesPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    topic: str = ...,
    ruleDisabled: bool = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> aiobotocore.paginate.AioPageIterator[ListTopicRulesResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
2. See `AioPageIterator[ListTopicRulesResponseTypeDef]`


```python
# paginate method usage example with argument unpacking

kwargs: ListTopicRulesRequestPaginateTypeDef = {  # (1)
    "topic": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListTopicRulesRequestPaginateTypeDef](./type_defs.md#listtopicrulesrequestpaginatetypedef)
## ListV2LoggingLevelsPaginator

Type annotations and code completion for `#!python session.create_client("iot").get_paginator("list_v2_logging_levels")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot/paginator/ListV2LoggingLevels.html#IoT.Paginator.ListV2LoggingLevels)

```python
# ListV2LoggingLevelsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_iot.paginator import ListV2LoggingLevelsPaginator

session = get_session()
async with session.create_client("iot") as client:  # (1)
    paginator: ListV2LoggingLevelsPaginator = client.get_paginator("list_v2_logging_levels")  # (2)
    async for item in paginator.paginate(...):
        item: ListV2LoggingLevelsResponseTypeDef
        print(item)  # (3)
```

1. client: [IoTClient](./client.md)
2. paginator: [ListV2LoggingLevelsPaginator](./paginators.md#listv2logginglevelspaginator)
3. item: `AioPageIterator[ListV2LoggingLevelsResponseTypeDef]`


### paginate

Type annotations and code completion for `#!python ListV2LoggingLevelsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    targetType: LogTargetTypeType = ...,  # (1)
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (2)
) -> aiobotocore.paginate.AioPageIterator[ListV2LoggingLevelsResponseTypeDef]:  # (3)
    ...
```

1. See [:material-code-brackets: LogTargetTypeType](./literals.md#logtargettypetype)
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
3. See `AioPageIterator[ListV2LoggingLevelsResponseTypeDef]`


```python
# paginate method usage example with argument unpacking

kwargs: ListV2LoggingLevelsRequestPaginateTypeDef = {  # (1)
    "targetType": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListV2LoggingLevelsRequestPaginateTypeDef](./type_defs.md#listv2logginglevelsrequestpaginatetypedef)
## ListViolationEventsPaginator

Type annotations and code completion for `#!python session.create_client("iot").get_paginator("list_violation_events")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot/paginator/ListViolationEvents.html#IoT.Paginator.ListViolationEvents)

```python
# ListViolationEventsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_iot.paginator import ListViolationEventsPaginator

session = get_session()
async with session.create_client("iot") as client:  # (1)
    paginator: ListViolationEventsPaginator = client.get_paginator("list_violation_events")  # (2)
    async for item in paginator.paginate(...):
        item: ListViolationEventsResponseTypeDef
        print(item)  # (3)
```

1. client: [IoTClient](./client.md)
2. paginator: [ListViolationEventsPaginator](./paginators.md#listviolationeventspaginator)
3. item: `AioPageIterator[ListViolationEventsResponseTypeDef]`


### paginate

Type annotations and code completion for `#!python ListViolationEventsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    startTime: TimestampTypeDef,
    endTime: TimestampTypeDef,
    thingName: str = ...,
    securityProfileName: str = ...,
    behaviorCriteriaType: BehaviorCriteriaTypeType = ...,  # (1)
    listSuppressedAlerts: bool = ...,
    verificationState: VerificationStateType = ...,  # (2)
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (3)
) -> aiobotocore.paginate.AioPageIterator[ListViolationEventsResponseTypeDef]:  # (4)
    ...
```

1. See [:material-code-brackets: BehaviorCriteriaTypeType](./literals.md#behaviorcriteriatypetype)
2. See [:material-code-brackets: VerificationStateType](./literals.md#verificationstatetype)
3. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
4. See `AioPageIterator[ListViolationEventsResponseTypeDef]`


```python
# paginate method usage example with argument unpacking

kwargs: ListViolationEventsRequestPaginateTypeDef = {  # (1)
    "startTime": ...,
    "endTime": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListViolationEventsRequestPaginateTypeDef](./type_defs.md#listviolationeventsrequestpaginatetypedef)
