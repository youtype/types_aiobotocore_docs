# Paginators

> [Index](../README.md) > [IoT](./README.md) > Paginators

!!! note ""

    Auto-generated documentation for [IoT](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot.html#IoT)
    type annotations stubs module [types-aiobotocore-iot](https://pypi.org/project/types-aiobotocore-iot/).

## GetBehaviorModelTrainingSummariesPaginator

Type annotations and code completion for `#!python session.create_client("iot").get_paginator("get_behavior_model_training_summaries")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot.html#IoT.Paginator.GetBehaviorModelTrainingSummaries)

```python title="Usage example"
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
3. item: [:material-code-braces: GetBehaviorModelTrainingSummariesResponseTypeDef](./type_defs.md#getbehaviormodeltrainingsummariesresponsetypedef) 


### paginate

Type annotations and code completion for `#!python GetBehaviorModelTrainingSummariesPaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    securityProfileName: str = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AsyncIterator[GetBehaviorModelTrainingSummariesResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: GetBehaviorModelTrainingSummariesResponseTypeDef](./type_defs.md#getbehaviormodeltrainingsummariesresponsetypedef) 


```python title="Usage example with kwargs"
kwargs: GetBehaviorModelTrainingSummariesRequestGetBehaviorModelTrainingSummariesPaginateTypeDef = {  # (1)
    "securityProfileName": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: GetBehaviorModelTrainingSummariesRequestGetBehaviorModelTrainingSummariesPaginateTypeDef](./type_defs.md#getbehaviormodeltrainingsummariesrequestgetbehaviormodeltrainingsummariespaginatetypedef) 
## ListActiveViolationsPaginator

Type annotations and code completion for `#!python session.create_client("iot").get_paginator("list_active_violations")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot.html#IoT.Paginator.ListActiveViolations)

```python title="Usage example"
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
3. item: [:material-code-braces: ListActiveViolationsResponseTypeDef](./type_defs.md#listactiveviolationsresponsetypedef) 


### paginate

Type annotations and code completion for `#!python ListActiveViolationsPaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    thingName: str = ...,
    securityProfileName: str = ...,
    behaviorCriteriaType: BehaviorCriteriaTypeType = ...,  # (1)
    listSuppressedAlerts: bool = ...,
    verificationState: VerificationStateType = ...,  # (2)
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (3)
) -> AsyncIterator[ListActiveViolationsResponseTypeDef]:  # (4)
    ...
```

1. See [:material-code-brackets: BehaviorCriteriaTypeType](./literals.md#behaviorcriteriatypetype) 
2. See [:material-code-brackets: VerificationStateType](./literals.md#verificationstatetype) 
3. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
4. See [:material-code-braces: ListActiveViolationsResponseTypeDef](./type_defs.md#listactiveviolationsresponsetypedef) 


```python title="Usage example with kwargs"
kwargs: ListActiveViolationsRequestListActiveViolationsPaginateTypeDef = {  # (1)
    "thingName": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListActiveViolationsRequestListActiveViolationsPaginateTypeDef](./type_defs.md#listactiveviolationsrequestlistactiveviolationspaginatetypedef) 
## ListAttachedPoliciesPaginator

Type annotations and code completion for `#!python session.create_client("iot").get_paginator("list_attached_policies")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot.html#IoT.Paginator.ListAttachedPolicies)

```python title="Usage example"
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
3. item: [:material-code-braces: ListAttachedPoliciesResponseTypeDef](./type_defs.md#listattachedpoliciesresponsetypedef) 


### paginate

Type annotations and code completion for `#!python ListAttachedPoliciesPaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    target: str,
    recursive: bool = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AsyncIterator[ListAttachedPoliciesResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListAttachedPoliciesResponseTypeDef](./type_defs.md#listattachedpoliciesresponsetypedef) 


```python title="Usage example with kwargs"
kwargs: ListAttachedPoliciesRequestListAttachedPoliciesPaginateTypeDef = {  # (1)
    "target": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListAttachedPoliciesRequestListAttachedPoliciesPaginateTypeDef](./type_defs.md#listattachedpoliciesrequestlistattachedpoliciespaginatetypedef) 
## ListAuditFindingsPaginator

Type annotations and code completion for `#!python session.create_client("iot").get_paginator("list_audit_findings")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot.html#IoT.Paginator.ListAuditFindings)

```python title="Usage example"
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
3. item: [:material-code-braces: ListAuditFindingsResponseTypeDef](./type_defs.md#listauditfindingsresponsetypedef) 


### paginate

Type annotations and code completion for `#!python ListAuditFindingsPaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    taskId: str = ...,
    checkName: str = ...,
    resourceIdentifier: ResourceIdentifierTypeDef = ...,  # (1)
    startTime: Union[datetime, str] = ...,
    endTime: Union[datetime, str] = ...,
    listSuppressedFindings: bool = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (2)
) -> AsyncIterator[ListAuditFindingsResponseTypeDef]:  # (3)
    ...
```

1. See [:material-code-braces: ResourceIdentifierTypeDef](./type_defs.md#resourceidentifiertypedef) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
3. See [:material-code-braces: ListAuditFindingsResponseTypeDef](./type_defs.md#listauditfindingsresponsetypedef) 


```python title="Usage example with kwargs"
kwargs: ListAuditFindingsRequestListAuditFindingsPaginateTypeDef = {  # (1)
    "taskId": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListAuditFindingsRequestListAuditFindingsPaginateTypeDef](./type_defs.md#listauditfindingsrequestlistauditfindingspaginatetypedef) 
## ListAuditMitigationActionsExecutionsPaginator

Type annotations and code completion for `#!python session.create_client("iot").get_paginator("list_audit_mitigation_actions_executions")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot.html#IoT.Paginator.ListAuditMitigationActionsExecutions)

```python title="Usage example"
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
3. item: [:material-code-braces: ListAuditMitigationActionsExecutionsResponseTypeDef](./type_defs.md#listauditmitigationactionsexecutionsresponsetypedef) 


### paginate

Type annotations and code completion for `#!python ListAuditMitigationActionsExecutionsPaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    taskId: str,
    findingId: str,
    actionStatus: AuditMitigationActionsExecutionStatusType = ...,  # (1)
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (2)
) -> AsyncIterator[ListAuditMitigationActionsExecutionsResponseTypeDef]:  # (3)
    ...
```

1. See [:material-code-brackets: AuditMitigationActionsExecutionStatusType](./literals.md#auditmitigationactionsexecutionstatustype) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
3. See [:material-code-braces: ListAuditMitigationActionsExecutionsResponseTypeDef](./type_defs.md#listauditmitigationactionsexecutionsresponsetypedef) 


```python title="Usage example with kwargs"
kwargs: ListAuditMitigationActionsExecutionsRequestListAuditMitigationActionsExecutionsPaginateTypeDef = {  # (1)
    "taskId": ...,
    "findingId": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListAuditMitigationActionsExecutionsRequestListAuditMitigationActionsExecutionsPaginateTypeDef](./type_defs.md#listauditmitigationactionsexecutionsrequestlistauditmitigationactionsexecutionspaginatetypedef) 
## ListAuditMitigationActionsTasksPaginator

Type annotations and code completion for `#!python session.create_client("iot").get_paginator("list_audit_mitigation_actions_tasks")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot.html#IoT.Paginator.ListAuditMitigationActionsTasks)

```python title="Usage example"
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
3. item: [:material-code-braces: ListAuditMitigationActionsTasksResponseTypeDef](./type_defs.md#listauditmitigationactionstasksresponsetypedef) 


### paginate

Type annotations and code completion for `#!python ListAuditMitigationActionsTasksPaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    startTime: Union[datetime, str],
    endTime: Union[datetime, str],
    auditTaskId: str = ...,
    findingId: str = ...,
    taskStatus: AuditMitigationActionsTaskStatusType = ...,  # (1)
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (2)
) -> AsyncIterator[ListAuditMitigationActionsTasksResponseTypeDef]:  # (3)
    ...
```

1. See [:material-code-brackets: AuditMitigationActionsTaskStatusType](./literals.md#auditmitigationactionstaskstatustype) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
3. See [:material-code-braces: ListAuditMitigationActionsTasksResponseTypeDef](./type_defs.md#listauditmitigationactionstasksresponsetypedef) 


```python title="Usage example with kwargs"
kwargs: ListAuditMitigationActionsTasksRequestListAuditMitigationActionsTasksPaginateTypeDef = {  # (1)
    "startTime": ...,
    "endTime": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListAuditMitigationActionsTasksRequestListAuditMitigationActionsTasksPaginateTypeDef](./type_defs.md#listauditmitigationactionstasksrequestlistauditmitigationactionstaskspaginatetypedef) 
## ListAuditSuppressionsPaginator

Type annotations and code completion for `#!python session.create_client("iot").get_paginator("list_audit_suppressions")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot.html#IoT.Paginator.ListAuditSuppressions)

```python title="Usage example"
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
3. item: [:material-code-braces: ListAuditSuppressionsResponseTypeDef](./type_defs.md#listauditsuppressionsresponsetypedef) 


### paginate

Type annotations and code completion for `#!python ListAuditSuppressionsPaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    checkName: str = ...,
    resourceIdentifier: ResourceIdentifierTypeDef = ...,  # (1)
    ascendingOrder: bool = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (2)
) -> AsyncIterator[ListAuditSuppressionsResponseTypeDef]:  # (3)
    ...
```

1. See [:material-code-braces: ResourceIdentifierTypeDef](./type_defs.md#resourceidentifiertypedef) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
3. See [:material-code-braces: ListAuditSuppressionsResponseTypeDef](./type_defs.md#listauditsuppressionsresponsetypedef) 


```python title="Usage example with kwargs"
kwargs: ListAuditSuppressionsRequestListAuditSuppressionsPaginateTypeDef = {  # (1)
    "checkName": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListAuditSuppressionsRequestListAuditSuppressionsPaginateTypeDef](./type_defs.md#listauditsuppressionsrequestlistauditsuppressionspaginatetypedef) 
## ListAuditTasksPaginator

Type annotations and code completion for `#!python session.create_client("iot").get_paginator("list_audit_tasks")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot.html#IoT.Paginator.ListAuditTasks)

```python title="Usage example"
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
3. item: [:material-code-braces: ListAuditTasksResponseTypeDef](./type_defs.md#listaudittasksresponsetypedef) 


### paginate

Type annotations and code completion for `#!python ListAuditTasksPaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    startTime: Union[datetime, str],
    endTime: Union[datetime, str],
    taskType: AuditTaskTypeType = ...,  # (1)
    taskStatus: AuditTaskStatusType = ...,  # (2)
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (3)
) -> AsyncIterator[ListAuditTasksResponseTypeDef]:  # (4)
    ...
```

1. See [:material-code-brackets: AuditTaskTypeType](./literals.md#audittasktypetype) 
2. See [:material-code-brackets: AuditTaskStatusType](./literals.md#audittaskstatustype) 
3. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
4. See [:material-code-braces: ListAuditTasksResponseTypeDef](./type_defs.md#listaudittasksresponsetypedef) 


```python title="Usage example with kwargs"
kwargs: ListAuditTasksRequestListAuditTasksPaginateTypeDef = {  # (1)
    "startTime": ...,
    "endTime": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListAuditTasksRequestListAuditTasksPaginateTypeDef](./type_defs.md#listaudittasksrequestlistaudittaskspaginatetypedef) 
## ListAuthorizersPaginator

Type annotations and code completion for `#!python session.create_client("iot").get_paginator("list_authorizers")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot.html#IoT.Paginator.ListAuthorizers)

```python title="Usage example"
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
3. item: [:material-code-braces: ListAuthorizersResponseTypeDef](./type_defs.md#listauthorizersresponsetypedef) 


### paginate

Type annotations and code completion for `#!python ListAuthorizersPaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    ascendingOrder: bool = ...,
    status: AuthorizerStatusType = ...,  # (1)
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (2)
) -> AsyncIterator[ListAuthorizersResponseTypeDef]:  # (3)
    ...
```

1. See [:material-code-brackets: AuthorizerStatusType](./literals.md#authorizerstatustype) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
3. See [:material-code-braces: ListAuthorizersResponseTypeDef](./type_defs.md#listauthorizersresponsetypedef) 


```python title="Usage example with kwargs"
kwargs: ListAuthorizersRequestListAuthorizersPaginateTypeDef = {  # (1)
    "ascendingOrder": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListAuthorizersRequestListAuthorizersPaginateTypeDef](./type_defs.md#listauthorizersrequestlistauthorizerspaginatetypedef) 
## ListBillingGroupsPaginator

Type annotations and code completion for `#!python session.create_client("iot").get_paginator("list_billing_groups")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot.html#IoT.Paginator.ListBillingGroups)

```python title="Usage example"
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
3. item: [:material-code-braces: ListBillingGroupsResponseTypeDef](./type_defs.md#listbillinggroupsresponsetypedef) 


### paginate

Type annotations and code completion for `#!python ListBillingGroupsPaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    namePrefixFilter: str = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AsyncIterator[ListBillingGroupsResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListBillingGroupsResponseTypeDef](./type_defs.md#listbillinggroupsresponsetypedef) 


```python title="Usage example with kwargs"
kwargs: ListBillingGroupsRequestListBillingGroupsPaginateTypeDef = {  # (1)
    "namePrefixFilter": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListBillingGroupsRequestListBillingGroupsPaginateTypeDef](./type_defs.md#listbillinggroupsrequestlistbillinggroupspaginatetypedef) 
## ListCACertificatesPaginator

Type annotations and code completion for `#!python session.create_client("iot").get_paginator("list_ca_certificates")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot.html#IoT.Paginator.ListCACertificates)

```python title="Usage example"
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
3. item: [:material-code-braces: ListCACertificatesResponseTypeDef](./type_defs.md#listcacertificatesresponsetypedef) 


### paginate

Type annotations and code completion for `#!python ListCACertificatesPaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    ascendingOrder: bool = ...,
    templateName: str = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AsyncIterator[ListCACertificatesResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListCACertificatesResponseTypeDef](./type_defs.md#listcacertificatesresponsetypedef) 


```python title="Usage example with kwargs"
kwargs: ListCACertificatesRequestListCACertificatesPaginateTypeDef = {  # (1)
    "ascendingOrder": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListCACertificatesRequestListCACertificatesPaginateTypeDef](./type_defs.md#listcacertificatesrequestlistcacertificatespaginatetypedef) 
## ListCertificatesPaginator

Type annotations and code completion for `#!python session.create_client("iot").get_paginator("list_certificates")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot.html#IoT.Paginator.ListCertificates)

```python title="Usage example"
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
3. item: [:material-code-braces: ListCertificatesResponseTypeDef](./type_defs.md#listcertificatesresponsetypedef) 


### paginate

Type annotations and code completion for `#!python ListCertificatesPaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    ascendingOrder: bool = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AsyncIterator[ListCertificatesResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListCertificatesResponseTypeDef](./type_defs.md#listcertificatesresponsetypedef) 


```python title="Usage example with kwargs"
kwargs: ListCertificatesRequestListCertificatesPaginateTypeDef = {  # (1)
    "ascendingOrder": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListCertificatesRequestListCertificatesPaginateTypeDef](./type_defs.md#listcertificatesrequestlistcertificatespaginatetypedef) 
## ListCertificatesByCAPaginator

Type annotations and code completion for `#!python session.create_client("iot").get_paginator("list_certificates_by_ca")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot.html#IoT.Paginator.ListCertificatesByCA)

```python title="Usage example"
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
3. item: [:material-code-braces: ListCertificatesByCAResponseTypeDef](./type_defs.md#listcertificatesbycaresponsetypedef) 


### paginate

Type annotations and code completion for `#!python ListCertificatesByCAPaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    caCertificateId: str,
    ascendingOrder: bool = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AsyncIterator[ListCertificatesByCAResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListCertificatesByCAResponseTypeDef](./type_defs.md#listcertificatesbycaresponsetypedef) 


```python title="Usage example with kwargs"
kwargs: ListCertificatesByCARequestListCertificatesByCAPaginateTypeDef = {  # (1)
    "caCertificateId": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListCertificatesByCARequestListCertificatesByCAPaginateTypeDef](./type_defs.md#listcertificatesbycarequestlistcertificatesbycapaginatetypedef) 
## ListCustomMetricsPaginator

Type annotations and code completion for `#!python session.create_client("iot").get_paginator("list_custom_metrics")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot.html#IoT.Paginator.ListCustomMetrics)

```python title="Usage example"
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
3. item: [:material-code-braces: ListCustomMetricsResponseTypeDef](./type_defs.md#listcustommetricsresponsetypedef) 


### paginate

Type annotations and code completion for `#!python ListCustomMetricsPaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AsyncIterator[ListCustomMetricsResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListCustomMetricsResponseTypeDef](./type_defs.md#listcustommetricsresponsetypedef) 


```python title="Usage example with kwargs"
kwargs: ListCustomMetricsRequestListCustomMetricsPaginateTypeDef = {  # (1)
    "PaginationConfig": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListCustomMetricsRequestListCustomMetricsPaginateTypeDef](./type_defs.md#listcustommetricsrequestlistcustommetricspaginatetypedef) 
## ListDetectMitigationActionsExecutionsPaginator

Type annotations and code completion for `#!python session.create_client("iot").get_paginator("list_detect_mitigation_actions_executions")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot.html#IoT.Paginator.ListDetectMitigationActionsExecutions)

```python title="Usage example"
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
3. item: [:material-code-braces: ListDetectMitigationActionsExecutionsResponseTypeDef](./type_defs.md#listdetectmitigationactionsexecutionsresponsetypedef) 


### paginate

Type annotations and code completion for `#!python ListDetectMitigationActionsExecutionsPaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    taskId: str = ...,
    violationId: str = ...,
    thingName: str = ...,
    startTime: Union[datetime, str] = ...,
    endTime: Union[datetime, str] = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AsyncIterator[ListDetectMitigationActionsExecutionsResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListDetectMitigationActionsExecutionsResponseTypeDef](./type_defs.md#listdetectmitigationactionsexecutionsresponsetypedef) 


```python title="Usage example with kwargs"
kwargs: ListDetectMitigationActionsExecutionsRequestListDetectMitigationActionsExecutionsPaginateTypeDef = {  # (1)
    "taskId": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListDetectMitigationActionsExecutionsRequestListDetectMitigationActionsExecutionsPaginateTypeDef](./type_defs.md#listdetectmitigationactionsexecutionsrequestlistdetectmitigationactionsexecutionspaginatetypedef) 
## ListDetectMitigationActionsTasksPaginator

Type annotations and code completion for `#!python session.create_client("iot").get_paginator("list_detect_mitigation_actions_tasks")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot.html#IoT.Paginator.ListDetectMitigationActionsTasks)

```python title="Usage example"
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
3. item: [:material-code-braces: ListDetectMitigationActionsTasksResponseTypeDef](./type_defs.md#listdetectmitigationactionstasksresponsetypedef) 


### paginate

Type annotations and code completion for `#!python ListDetectMitigationActionsTasksPaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    startTime: Union[datetime, str],
    endTime: Union[datetime, str],
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AsyncIterator[ListDetectMitigationActionsTasksResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListDetectMitigationActionsTasksResponseTypeDef](./type_defs.md#listdetectmitigationactionstasksresponsetypedef) 


```python title="Usage example with kwargs"
kwargs: ListDetectMitigationActionsTasksRequestListDetectMitigationActionsTasksPaginateTypeDef = {  # (1)
    "startTime": ...,
    "endTime": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListDetectMitigationActionsTasksRequestListDetectMitigationActionsTasksPaginateTypeDef](./type_defs.md#listdetectmitigationactionstasksrequestlistdetectmitigationactionstaskspaginatetypedef) 
## ListDimensionsPaginator

Type annotations and code completion for `#!python session.create_client("iot").get_paginator("list_dimensions")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot.html#IoT.Paginator.ListDimensions)

```python title="Usage example"
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
3. item: [:material-code-braces: ListDimensionsResponseTypeDef](./type_defs.md#listdimensionsresponsetypedef) 


### paginate

Type annotations and code completion for `#!python ListDimensionsPaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AsyncIterator[ListDimensionsResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListDimensionsResponseTypeDef](./type_defs.md#listdimensionsresponsetypedef) 


```python title="Usage example with kwargs"
kwargs: ListDimensionsRequestListDimensionsPaginateTypeDef = {  # (1)
    "PaginationConfig": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListDimensionsRequestListDimensionsPaginateTypeDef](./type_defs.md#listdimensionsrequestlistdimensionspaginatetypedef) 
## ListDomainConfigurationsPaginator

Type annotations and code completion for `#!python session.create_client("iot").get_paginator("list_domain_configurations")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot.html#IoT.Paginator.ListDomainConfigurations)

```python title="Usage example"
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
3. item: [:material-code-braces: ListDomainConfigurationsResponseTypeDef](./type_defs.md#listdomainconfigurationsresponsetypedef) 


### paginate

Type annotations and code completion for `#!python ListDomainConfigurationsPaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    serviceType: ServiceTypeType = ...,  # (1)
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (2)
) -> AsyncIterator[ListDomainConfigurationsResponseTypeDef]:  # (3)
    ...
```

1. See [:material-code-brackets: ServiceTypeType](./literals.md#servicetypetype) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
3. See [:material-code-braces: ListDomainConfigurationsResponseTypeDef](./type_defs.md#listdomainconfigurationsresponsetypedef) 


```python title="Usage example with kwargs"
kwargs: ListDomainConfigurationsRequestListDomainConfigurationsPaginateTypeDef = {  # (1)
    "serviceType": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListDomainConfigurationsRequestListDomainConfigurationsPaginateTypeDef](./type_defs.md#listdomainconfigurationsrequestlistdomainconfigurationspaginatetypedef) 
## ListFleetMetricsPaginator

Type annotations and code completion for `#!python session.create_client("iot").get_paginator("list_fleet_metrics")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot.html#IoT.Paginator.ListFleetMetrics)

```python title="Usage example"
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
3. item: [:material-code-braces: ListFleetMetricsResponseTypeDef](./type_defs.md#listfleetmetricsresponsetypedef) 


### paginate

Type annotations and code completion for `#!python ListFleetMetricsPaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AsyncIterator[ListFleetMetricsResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListFleetMetricsResponseTypeDef](./type_defs.md#listfleetmetricsresponsetypedef) 


```python title="Usage example with kwargs"
kwargs: ListFleetMetricsRequestListFleetMetricsPaginateTypeDef = {  # (1)
    "PaginationConfig": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListFleetMetricsRequestListFleetMetricsPaginateTypeDef](./type_defs.md#listfleetmetricsrequestlistfleetmetricspaginatetypedef) 
## ListIndicesPaginator

Type annotations and code completion for `#!python session.create_client("iot").get_paginator("list_indices")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot.html#IoT.Paginator.ListIndices)

```python title="Usage example"
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
3. item: [:material-code-braces: ListIndicesResponseTypeDef](./type_defs.md#listindicesresponsetypedef) 


### paginate

Type annotations and code completion for `#!python ListIndicesPaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AsyncIterator[ListIndicesResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListIndicesResponseTypeDef](./type_defs.md#listindicesresponsetypedef) 


```python title="Usage example with kwargs"
kwargs: ListIndicesRequestListIndicesPaginateTypeDef = {  # (1)
    "PaginationConfig": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListIndicesRequestListIndicesPaginateTypeDef](./type_defs.md#listindicesrequestlistindicespaginatetypedef) 
## ListJobExecutionsForJobPaginator

Type annotations and code completion for `#!python session.create_client("iot").get_paginator("list_job_executions_for_job")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot.html#IoT.Paginator.ListJobExecutionsForJob)

```python title="Usage example"
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
3. item: [:material-code-braces: ListJobExecutionsForJobResponseTypeDef](./type_defs.md#listjobexecutionsforjobresponsetypedef) 


### paginate

Type annotations and code completion for `#!python ListJobExecutionsForJobPaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    jobId: str,
    status: JobExecutionStatusType = ...,  # (1)
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (2)
) -> AsyncIterator[ListJobExecutionsForJobResponseTypeDef]:  # (3)
    ...
```

1. See [:material-code-brackets: JobExecutionStatusType](./literals.md#jobexecutionstatustype) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
3. See [:material-code-braces: ListJobExecutionsForJobResponseTypeDef](./type_defs.md#listjobexecutionsforjobresponsetypedef) 


```python title="Usage example with kwargs"
kwargs: ListJobExecutionsForJobRequestListJobExecutionsForJobPaginateTypeDef = {  # (1)
    "jobId": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListJobExecutionsForJobRequestListJobExecutionsForJobPaginateTypeDef](./type_defs.md#listjobexecutionsforjobrequestlistjobexecutionsforjobpaginatetypedef) 
## ListJobExecutionsForThingPaginator

Type annotations and code completion for `#!python session.create_client("iot").get_paginator("list_job_executions_for_thing")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot.html#IoT.Paginator.ListJobExecutionsForThing)

```python title="Usage example"
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
3. item: [:material-code-braces: ListJobExecutionsForThingResponseTypeDef](./type_defs.md#listjobexecutionsforthingresponsetypedef) 


### paginate

Type annotations and code completion for `#!python ListJobExecutionsForThingPaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    thingName: str,
    status: JobExecutionStatusType = ...,  # (1)
    namespaceId: str = ...,
    jobId: str = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (2)
) -> AsyncIterator[ListJobExecutionsForThingResponseTypeDef]:  # (3)
    ...
```

1. See [:material-code-brackets: JobExecutionStatusType](./literals.md#jobexecutionstatustype) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
3. See [:material-code-braces: ListJobExecutionsForThingResponseTypeDef](./type_defs.md#listjobexecutionsforthingresponsetypedef) 


```python title="Usage example with kwargs"
kwargs: ListJobExecutionsForThingRequestListJobExecutionsForThingPaginateTypeDef = {  # (1)
    "thingName": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListJobExecutionsForThingRequestListJobExecutionsForThingPaginateTypeDef](./type_defs.md#listjobexecutionsforthingrequestlistjobexecutionsforthingpaginatetypedef) 
## ListJobTemplatesPaginator

Type annotations and code completion for `#!python session.create_client("iot").get_paginator("list_job_templates")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot.html#IoT.Paginator.ListJobTemplates)

```python title="Usage example"
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
3. item: [:material-code-braces: ListJobTemplatesResponseTypeDef](./type_defs.md#listjobtemplatesresponsetypedef) 


### paginate

Type annotations and code completion for `#!python ListJobTemplatesPaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AsyncIterator[ListJobTemplatesResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListJobTemplatesResponseTypeDef](./type_defs.md#listjobtemplatesresponsetypedef) 


```python title="Usage example with kwargs"
kwargs: ListJobTemplatesRequestListJobTemplatesPaginateTypeDef = {  # (1)
    "PaginationConfig": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListJobTemplatesRequestListJobTemplatesPaginateTypeDef](./type_defs.md#listjobtemplatesrequestlistjobtemplatespaginatetypedef) 
## ListJobsPaginator

Type annotations and code completion for `#!python session.create_client("iot").get_paginator("list_jobs")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot.html#IoT.Paginator.ListJobs)

```python title="Usage example"
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
3. item: [:material-code-braces: ListJobsResponseTypeDef](./type_defs.md#listjobsresponsetypedef) 


### paginate

Type annotations and code completion for `#!python ListJobsPaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    status: JobStatusType = ...,  # (1)
    targetSelection: TargetSelectionType = ...,  # (2)
    thingGroupName: str = ...,
    thingGroupId: str = ...,
    namespaceId: str = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (3)
) -> AsyncIterator[ListJobsResponseTypeDef]:  # (4)
    ...
```

1. See [:material-code-brackets: JobStatusType](./literals.md#jobstatustype) 
2. See [:material-code-brackets: TargetSelectionType](./literals.md#targetselectiontype) 
3. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
4. See [:material-code-braces: ListJobsResponseTypeDef](./type_defs.md#listjobsresponsetypedef) 


```python title="Usage example with kwargs"
kwargs: ListJobsRequestListJobsPaginateTypeDef = {  # (1)
    "status": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListJobsRequestListJobsPaginateTypeDef](./type_defs.md#listjobsrequestlistjobspaginatetypedef) 
## ListMetricValuesPaginator

Type annotations and code completion for `#!python session.create_client("iot").get_paginator("list_metric_values")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot.html#IoT.Paginator.ListMetricValues)

```python title="Usage example"
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
3. item: [:material-code-braces: ListMetricValuesResponseTypeDef](./type_defs.md#listmetricvaluesresponsetypedef) 


### paginate

Type annotations and code completion for `#!python ListMetricValuesPaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    thingName: str,
    metricName: str,
    startTime: Union[datetime, str],
    endTime: Union[datetime, str],
    dimensionName: str = ...,
    dimensionValueOperator: DimensionValueOperatorType = ...,  # (1)
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (2)
) -> AsyncIterator[ListMetricValuesResponseTypeDef]:  # (3)
    ...
```

1. See [:material-code-brackets: DimensionValueOperatorType](./literals.md#dimensionvalueoperatortype) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
3. See [:material-code-braces: ListMetricValuesResponseTypeDef](./type_defs.md#listmetricvaluesresponsetypedef) 


```python title="Usage example with kwargs"
kwargs: ListMetricValuesRequestListMetricValuesPaginateTypeDef = {  # (1)
    "thingName": ...,
    "metricName": ...,
    "startTime": ...,
    "endTime": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListMetricValuesRequestListMetricValuesPaginateTypeDef](./type_defs.md#listmetricvaluesrequestlistmetricvaluespaginatetypedef) 
## ListMitigationActionsPaginator

Type annotations and code completion for `#!python session.create_client("iot").get_paginator("list_mitigation_actions")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot.html#IoT.Paginator.ListMitigationActions)

```python title="Usage example"
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
3. item: [:material-code-braces: ListMitigationActionsResponseTypeDef](./type_defs.md#listmitigationactionsresponsetypedef) 


### paginate

Type annotations and code completion for `#!python ListMitigationActionsPaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    actionType: MitigationActionTypeType = ...,  # (1)
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (2)
) -> AsyncIterator[ListMitigationActionsResponseTypeDef]:  # (3)
    ...
```

1. See [:material-code-brackets: MitigationActionTypeType](./literals.md#mitigationactiontypetype) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
3. See [:material-code-braces: ListMitigationActionsResponseTypeDef](./type_defs.md#listmitigationactionsresponsetypedef) 


```python title="Usage example with kwargs"
kwargs: ListMitigationActionsRequestListMitigationActionsPaginateTypeDef = {  # (1)
    "actionType": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListMitigationActionsRequestListMitigationActionsPaginateTypeDef](./type_defs.md#listmitigationactionsrequestlistmitigationactionspaginatetypedef) 
## ListOTAUpdatesPaginator

Type annotations and code completion for `#!python session.create_client("iot").get_paginator("list_ota_updates")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot.html#IoT.Paginator.ListOTAUpdates)

```python title="Usage example"
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
3. item: [:material-code-braces: ListOTAUpdatesResponseTypeDef](./type_defs.md#listotaupdatesresponsetypedef) 


### paginate

Type annotations and code completion for `#!python ListOTAUpdatesPaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    otaUpdateStatus: OTAUpdateStatusType = ...,  # (1)
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (2)
) -> AsyncIterator[ListOTAUpdatesResponseTypeDef]:  # (3)
    ...
```

1. See [:material-code-brackets: OTAUpdateStatusType](./literals.md#otaupdatestatustype) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
3. See [:material-code-braces: ListOTAUpdatesResponseTypeDef](./type_defs.md#listotaupdatesresponsetypedef) 


```python title="Usage example with kwargs"
kwargs: ListOTAUpdatesRequestListOTAUpdatesPaginateTypeDef = {  # (1)
    "otaUpdateStatus": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListOTAUpdatesRequestListOTAUpdatesPaginateTypeDef](./type_defs.md#listotaupdatesrequestlistotaupdatespaginatetypedef) 
## ListOutgoingCertificatesPaginator

Type annotations and code completion for `#!python session.create_client("iot").get_paginator("list_outgoing_certificates")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot.html#IoT.Paginator.ListOutgoingCertificates)

```python title="Usage example"
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
3. item: [:material-code-braces: ListOutgoingCertificatesResponseTypeDef](./type_defs.md#listoutgoingcertificatesresponsetypedef) 


### paginate

Type annotations and code completion for `#!python ListOutgoingCertificatesPaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    ascendingOrder: bool = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AsyncIterator[ListOutgoingCertificatesResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListOutgoingCertificatesResponseTypeDef](./type_defs.md#listoutgoingcertificatesresponsetypedef) 


```python title="Usage example with kwargs"
kwargs: ListOutgoingCertificatesRequestListOutgoingCertificatesPaginateTypeDef = {  # (1)
    "ascendingOrder": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListOutgoingCertificatesRequestListOutgoingCertificatesPaginateTypeDef](./type_defs.md#listoutgoingcertificatesrequestlistoutgoingcertificatespaginatetypedef) 
## ListPoliciesPaginator

Type annotations and code completion for `#!python session.create_client("iot").get_paginator("list_policies")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot.html#IoT.Paginator.ListPolicies)

```python title="Usage example"
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
3. item: [:material-code-braces: ListPoliciesResponseTypeDef](./type_defs.md#listpoliciesresponsetypedef) 


### paginate

Type annotations and code completion for `#!python ListPoliciesPaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    ascendingOrder: bool = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AsyncIterator[ListPoliciesResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListPoliciesResponseTypeDef](./type_defs.md#listpoliciesresponsetypedef) 


```python title="Usage example with kwargs"
kwargs: ListPoliciesRequestListPoliciesPaginateTypeDef = {  # (1)
    "ascendingOrder": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListPoliciesRequestListPoliciesPaginateTypeDef](./type_defs.md#listpoliciesrequestlistpoliciespaginatetypedef) 
## ListPolicyPrincipalsPaginator

Type annotations and code completion for `#!python session.create_client("iot").get_paginator("list_policy_principals")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot.html#IoT.Paginator.ListPolicyPrincipals)

```python title="Usage example"
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
3. item: [:material-code-braces: ListPolicyPrincipalsResponseTypeDef](./type_defs.md#listpolicyprincipalsresponsetypedef) 


### paginate

Type annotations and code completion for `#!python ListPolicyPrincipalsPaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    policyName: str,
    ascendingOrder: bool = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AsyncIterator[ListPolicyPrincipalsResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListPolicyPrincipalsResponseTypeDef](./type_defs.md#listpolicyprincipalsresponsetypedef) 


```python title="Usage example with kwargs"
kwargs: ListPolicyPrincipalsRequestListPolicyPrincipalsPaginateTypeDef = {  # (1)
    "policyName": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListPolicyPrincipalsRequestListPolicyPrincipalsPaginateTypeDef](./type_defs.md#listpolicyprincipalsrequestlistpolicyprincipalspaginatetypedef) 
## ListPrincipalPoliciesPaginator

Type annotations and code completion for `#!python session.create_client("iot").get_paginator("list_principal_policies")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot.html#IoT.Paginator.ListPrincipalPolicies)

```python title="Usage example"
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
3. item: [:material-code-braces: ListPrincipalPoliciesResponseTypeDef](./type_defs.md#listprincipalpoliciesresponsetypedef) 


### paginate

Type annotations and code completion for `#!python ListPrincipalPoliciesPaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    principal: str,
    ascendingOrder: bool = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AsyncIterator[ListPrincipalPoliciesResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListPrincipalPoliciesResponseTypeDef](./type_defs.md#listprincipalpoliciesresponsetypedef) 


```python title="Usage example with kwargs"
kwargs: ListPrincipalPoliciesRequestListPrincipalPoliciesPaginateTypeDef = {  # (1)
    "principal": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListPrincipalPoliciesRequestListPrincipalPoliciesPaginateTypeDef](./type_defs.md#listprincipalpoliciesrequestlistprincipalpoliciespaginatetypedef) 
## ListPrincipalThingsPaginator

Type annotations and code completion for `#!python session.create_client("iot").get_paginator("list_principal_things")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot.html#IoT.Paginator.ListPrincipalThings)

```python title="Usage example"
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
3. item: [:material-code-braces: ListPrincipalThingsResponseTypeDef](./type_defs.md#listprincipalthingsresponsetypedef) 


### paginate

Type annotations and code completion for `#!python ListPrincipalThingsPaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    principal: str,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AsyncIterator[ListPrincipalThingsResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListPrincipalThingsResponseTypeDef](./type_defs.md#listprincipalthingsresponsetypedef) 


```python title="Usage example with kwargs"
kwargs: ListPrincipalThingsRequestListPrincipalThingsPaginateTypeDef = {  # (1)
    "principal": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListPrincipalThingsRequestListPrincipalThingsPaginateTypeDef](./type_defs.md#listprincipalthingsrequestlistprincipalthingspaginatetypedef) 
## ListProvisioningTemplateVersionsPaginator

Type annotations and code completion for `#!python session.create_client("iot").get_paginator("list_provisioning_template_versions")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot.html#IoT.Paginator.ListProvisioningTemplateVersions)

```python title="Usage example"
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
3. item: [:material-code-braces: ListProvisioningTemplateVersionsResponseTypeDef](./type_defs.md#listprovisioningtemplateversionsresponsetypedef) 


### paginate

Type annotations and code completion for `#!python ListProvisioningTemplateVersionsPaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    templateName: str,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AsyncIterator[ListProvisioningTemplateVersionsResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListProvisioningTemplateVersionsResponseTypeDef](./type_defs.md#listprovisioningtemplateversionsresponsetypedef) 


```python title="Usage example with kwargs"
kwargs: ListProvisioningTemplateVersionsRequestListProvisioningTemplateVersionsPaginateTypeDef = {  # (1)
    "templateName": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListProvisioningTemplateVersionsRequestListProvisioningTemplateVersionsPaginateTypeDef](./type_defs.md#listprovisioningtemplateversionsrequestlistprovisioningtemplateversionspaginatetypedef) 
## ListProvisioningTemplatesPaginator

Type annotations and code completion for `#!python session.create_client("iot").get_paginator("list_provisioning_templates")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot.html#IoT.Paginator.ListProvisioningTemplates)

```python title="Usage example"
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
3. item: [:material-code-braces: ListProvisioningTemplatesResponseTypeDef](./type_defs.md#listprovisioningtemplatesresponsetypedef) 


### paginate

Type annotations and code completion for `#!python ListProvisioningTemplatesPaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AsyncIterator[ListProvisioningTemplatesResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListProvisioningTemplatesResponseTypeDef](./type_defs.md#listprovisioningtemplatesresponsetypedef) 


```python title="Usage example with kwargs"
kwargs: ListProvisioningTemplatesRequestListProvisioningTemplatesPaginateTypeDef = {  # (1)
    "PaginationConfig": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListProvisioningTemplatesRequestListProvisioningTemplatesPaginateTypeDef](./type_defs.md#listprovisioningtemplatesrequestlistprovisioningtemplatespaginatetypedef) 
## ListRoleAliasesPaginator

Type annotations and code completion for `#!python session.create_client("iot").get_paginator("list_role_aliases")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot.html#IoT.Paginator.ListRoleAliases)

```python title="Usage example"
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
3. item: [:material-code-braces: ListRoleAliasesResponseTypeDef](./type_defs.md#listrolealiasesresponsetypedef) 


### paginate

Type annotations and code completion for `#!python ListRoleAliasesPaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    ascendingOrder: bool = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AsyncIterator[ListRoleAliasesResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListRoleAliasesResponseTypeDef](./type_defs.md#listrolealiasesresponsetypedef) 


```python title="Usage example with kwargs"
kwargs: ListRoleAliasesRequestListRoleAliasesPaginateTypeDef = {  # (1)
    "ascendingOrder": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListRoleAliasesRequestListRoleAliasesPaginateTypeDef](./type_defs.md#listrolealiasesrequestlistrolealiasespaginatetypedef) 
## ListScheduledAuditsPaginator

Type annotations and code completion for `#!python session.create_client("iot").get_paginator("list_scheduled_audits")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot.html#IoT.Paginator.ListScheduledAudits)

```python title="Usage example"
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
3. item: [:material-code-braces: ListScheduledAuditsResponseTypeDef](./type_defs.md#listscheduledauditsresponsetypedef) 


### paginate

Type annotations and code completion for `#!python ListScheduledAuditsPaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AsyncIterator[ListScheduledAuditsResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListScheduledAuditsResponseTypeDef](./type_defs.md#listscheduledauditsresponsetypedef) 


```python title="Usage example with kwargs"
kwargs: ListScheduledAuditsRequestListScheduledAuditsPaginateTypeDef = {  # (1)
    "PaginationConfig": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListScheduledAuditsRequestListScheduledAuditsPaginateTypeDef](./type_defs.md#listscheduledauditsrequestlistscheduledauditspaginatetypedef) 
## ListSecurityProfilesPaginator

Type annotations and code completion for `#!python session.create_client("iot").get_paginator("list_security_profiles")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot.html#IoT.Paginator.ListSecurityProfiles)

```python title="Usage example"
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
3. item: [:material-code-braces: ListSecurityProfilesResponseTypeDef](./type_defs.md#listsecurityprofilesresponsetypedef) 


### paginate

Type annotations and code completion for `#!python ListSecurityProfilesPaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    dimensionName: str = ...,
    metricName: str = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AsyncIterator[ListSecurityProfilesResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListSecurityProfilesResponseTypeDef](./type_defs.md#listsecurityprofilesresponsetypedef) 


```python title="Usage example with kwargs"
kwargs: ListSecurityProfilesRequestListSecurityProfilesPaginateTypeDef = {  # (1)
    "dimensionName": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListSecurityProfilesRequestListSecurityProfilesPaginateTypeDef](./type_defs.md#listsecurityprofilesrequestlistsecurityprofilespaginatetypedef) 
## ListSecurityProfilesForTargetPaginator

Type annotations and code completion for `#!python session.create_client("iot").get_paginator("list_security_profiles_for_target")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot.html#IoT.Paginator.ListSecurityProfilesForTarget)

```python title="Usage example"
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
3. item: [:material-code-braces: ListSecurityProfilesForTargetResponseTypeDef](./type_defs.md#listsecurityprofilesfortargetresponsetypedef) 


### paginate

Type annotations and code completion for `#!python ListSecurityProfilesForTargetPaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    securityProfileTargetArn: str,
    recursive: bool = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AsyncIterator[ListSecurityProfilesForTargetResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListSecurityProfilesForTargetResponseTypeDef](./type_defs.md#listsecurityprofilesfortargetresponsetypedef) 


```python title="Usage example with kwargs"
kwargs: ListSecurityProfilesForTargetRequestListSecurityProfilesForTargetPaginateTypeDef = {  # (1)
    "securityProfileTargetArn": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListSecurityProfilesForTargetRequestListSecurityProfilesForTargetPaginateTypeDef](./type_defs.md#listsecurityprofilesfortargetrequestlistsecurityprofilesfortargetpaginatetypedef) 
## ListStreamsPaginator

Type annotations and code completion for `#!python session.create_client("iot").get_paginator("list_streams")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot.html#IoT.Paginator.ListStreams)

```python title="Usage example"
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
3. item: [:material-code-braces: ListStreamsResponseTypeDef](./type_defs.md#liststreamsresponsetypedef) 


### paginate

Type annotations and code completion for `#!python ListStreamsPaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    ascendingOrder: bool = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AsyncIterator[ListStreamsResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListStreamsResponseTypeDef](./type_defs.md#liststreamsresponsetypedef) 


```python title="Usage example with kwargs"
kwargs: ListStreamsRequestListStreamsPaginateTypeDef = {  # (1)
    "ascendingOrder": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListStreamsRequestListStreamsPaginateTypeDef](./type_defs.md#liststreamsrequestliststreamspaginatetypedef) 
## ListTagsForResourcePaginator

Type annotations and code completion for `#!python session.create_client("iot").get_paginator("list_tags_for_resource")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot.html#IoT.Paginator.ListTagsForResource)

```python title="Usage example"
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
3. item: [:material-code-braces: ListTagsForResourceResponseTypeDef](./type_defs.md#listtagsforresourceresponsetypedef) 


### paginate

Type annotations and code completion for `#!python ListTagsForResourcePaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    resourceArn: str,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AsyncIterator[ListTagsForResourceResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListTagsForResourceResponseTypeDef](./type_defs.md#listtagsforresourceresponsetypedef) 


```python title="Usage example with kwargs"
kwargs: ListTagsForResourceRequestListTagsForResourcePaginateTypeDef = {  # (1)
    "resourceArn": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListTagsForResourceRequestListTagsForResourcePaginateTypeDef](./type_defs.md#listtagsforresourcerequestlisttagsforresourcepaginatetypedef) 
## ListTargetsForPolicyPaginator

Type annotations and code completion for `#!python session.create_client("iot").get_paginator("list_targets_for_policy")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot.html#IoT.Paginator.ListTargetsForPolicy)

```python title="Usage example"
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
3. item: [:material-code-braces: ListTargetsForPolicyResponseTypeDef](./type_defs.md#listtargetsforpolicyresponsetypedef) 


### paginate

Type annotations and code completion for `#!python ListTargetsForPolicyPaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    policyName: str,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AsyncIterator[ListTargetsForPolicyResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListTargetsForPolicyResponseTypeDef](./type_defs.md#listtargetsforpolicyresponsetypedef) 


```python title="Usage example with kwargs"
kwargs: ListTargetsForPolicyRequestListTargetsForPolicyPaginateTypeDef = {  # (1)
    "policyName": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListTargetsForPolicyRequestListTargetsForPolicyPaginateTypeDef](./type_defs.md#listtargetsforpolicyrequestlisttargetsforpolicypaginatetypedef) 
## ListTargetsForSecurityProfilePaginator

Type annotations and code completion for `#!python session.create_client("iot").get_paginator("list_targets_for_security_profile")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot.html#IoT.Paginator.ListTargetsForSecurityProfile)

```python title="Usage example"
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
3. item: [:material-code-braces: ListTargetsForSecurityProfileResponseTypeDef](./type_defs.md#listtargetsforsecurityprofileresponsetypedef) 


### paginate

Type annotations and code completion for `#!python ListTargetsForSecurityProfilePaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    securityProfileName: str,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AsyncIterator[ListTargetsForSecurityProfileResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListTargetsForSecurityProfileResponseTypeDef](./type_defs.md#listtargetsforsecurityprofileresponsetypedef) 


```python title="Usage example with kwargs"
kwargs: ListTargetsForSecurityProfileRequestListTargetsForSecurityProfilePaginateTypeDef = {  # (1)
    "securityProfileName": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListTargetsForSecurityProfileRequestListTargetsForSecurityProfilePaginateTypeDef](./type_defs.md#listtargetsforsecurityprofilerequestlisttargetsforsecurityprofilepaginatetypedef) 
## ListThingGroupsPaginator

Type annotations and code completion for `#!python session.create_client("iot").get_paginator("list_thing_groups")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot.html#IoT.Paginator.ListThingGroups)

```python title="Usage example"
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
3. item: [:material-code-braces: ListThingGroupsResponseTypeDef](./type_defs.md#listthinggroupsresponsetypedef) 


### paginate

Type annotations and code completion for `#!python ListThingGroupsPaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    parentGroup: str = ...,
    namePrefixFilter: str = ...,
    recursive: bool = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AsyncIterator[ListThingGroupsResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListThingGroupsResponseTypeDef](./type_defs.md#listthinggroupsresponsetypedef) 


```python title="Usage example with kwargs"
kwargs: ListThingGroupsRequestListThingGroupsPaginateTypeDef = {  # (1)
    "parentGroup": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListThingGroupsRequestListThingGroupsPaginateTypeDef](./type_defs.md#listthinggroupsrequestlistthinggroupspaginatetypedef) 
## ListThingGroupsForThingPaginator

Type annotations and code completion for `#!python session.create_client("iot").get_paginator("list_thing_groups_for_thing")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot.html#IoT.Paginator.ListThingGroupsForThing)

```python title="Usage example"
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
3. item: [:material-code-braces: ListThingGroupsForThingResponseTypeDef](./type_defs.md#listthinggroupsforthingresponsetypedef) 


### paginate

Type annotations and code completion for `#!python ListThingGroupsForThingPaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    thingName: str,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AsyncIterator[ListThingGroupsForThingResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListThingGroupsForThingResponseTypeDef](./type_defs.md#listthinggroupsforthingresponsetypedef) 


```python title="Usage example with kwargs"
kwargs: ListThingGroupsForThingRequestListThingGroupsForThingPaginateTypeDef = {  # (1)
    "thingName": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListThingGroupsForThingRequestListThingGroupsForThingPaginateTypeDef](./type_defs.md#listthinggroupsforthingrequestlistthinggroupsforthingpaginatetypedef) 
## ListThingPrincipalsPaginator

Type annotations and code completion for `#!python session.create_client("iot").get_paginator("list_thing_principals")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot.html#IoT.Paginator.ListThingPrincipals)

```python title="Usage example"
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
3. item: [:material-code-braces: ListThingPrincipalsResponseTypeDef](./type_defs.md#listthingprincipalsresponsetypedef) 


### paginate

Type annotations and code completion for `#!python ListThingPrincipalsPaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    thingName: str,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AsyncIterator[ListThingPrincipalsResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListThingPrincipalsResponseTypeDef](./type_defs.md#listthingprincipalsresponsetypedef) 


```python title="Usage example with kwargs"
kwargs: ListThingPrincipalsRequestListThingPrincipalsPaginateTypeDef = {  # (1)
    "thingName": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListThingPrincipalsRequestListThingPrincipalsPaginateTypeDef](./type_defs.md#listthingprincipalsrequestlistthingprincipalspaginatetypedef) 
## ListThingRegistrationTaskReportsPaginator

Type annotations and code completion for `#!python session.create_client("iot").get_paginator("list_thing_registration_task_reports")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot.html#IoT.Paginator.ListThingRegistrationTaskReports)

```python title="Usage example"
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
3. item: [:material-code-braces: ListThingRegistrationTaskReportsResponseTypeDef](./type_defs.md#listthingregistrationtaskreportsresponsetypedef) 


### paginate

Type annotations and code completion for `#!python ListThingRegistrationTaskReportsPaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    taskId: str,
    reportType: ReportTypeType,  # (1)
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (2)
) -> AsyncIterator[ListThingRegistrationTaskReportsResponseTypeDef]:  # (3)
    ...
```

1. See [:material-code-brackets: ReportTypeType](./literals.md#reporttypetype) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
3. See [:material-code-braces: ListThingRegistrationTaskReportsResponseTypeDef](./type_defs.md#listthingregistrationtaskreportsresponsetypedef) 


```python title="Usage example with kwargs"
kwargs: ListThingRegistrationTaskReportsRequestListThingRegistrationTaskReportsPaginateTypeDef = {  # (1)
    "taskId": ...,
    "reportType": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListThingRegistrationTaskReportsRequestListThingRegistrationTaskReportsPaginateTypeDef](./type_defs.md#listthingregistrationtaskreportsrequestlistthingregistrationtaskreportspaginatetypedef) 
## ListThingRegistrationTasksPaginator

Type annotations and code completion for `#!python session.create_client("iot").get_paginator("list_thing_registration_tasks")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot.html#IoT.Paginator.ListThingRegistrationTasks)

```python title="Usage example"
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
3. item: [:material-code-braces: ListThingRegistrationTasksResponseTypeDef](./type_defs.md#listthingregistrationtasksresponsetypedef) 


### paginate

Type annotations and code completion for `#!python ListThingRegistrationTasksPaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    status: StatusType = ...,  # (1)
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (2)
) -> AsyncIterator[ListThingRegistrationTasksResponseTypeDef]:  # (3)
    ...
```

1. See [:material-code-brackets: StatusType](./literals.md#statustype) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
3. See [:material-code-braces: ListThingRegistrationTasksResponseTypeDef](./type_defs.md#listthingregistrationtasksresponsetypedef) 


```python title="Usage example with kwargs"
kwargs: ListThingRegistrationTasksRequestListThingRegistrationTasksPaginateTypeDef = {  # (1)
    "status": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListThingRegistrationTasksRequestListThingRegistrationTasksPaginateTypeDef](./type_defs.md#listthingregistrationtasksrequestlistthingregistrationtaskspaginatetypedef) 
## ListThingTypesPaginator

Type annotations and code completion for `#!python session.create_client("iot").get_paginator("list_thing_types")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot.html#IoT.Paginator.ListThingTypes)

```python title="Usage example"
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
3. item: [:material-code-braces: ListThingTypesResponseTypeDef](./type_defs.md#listthingtypesresponsetypedef) 


### paginate

Type annotations and code completion for `#!python ListThingTypesPaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    thingTypeName: str = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AsyncIterator[ListThingTypesResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListThingTypesResponseTypeDef](./type_defs.md#listthingtypesresponsetypedef) 


```python title="Usage example with kwargs"
kwargs: ListThingTypesRequestListThingTypesPaginateTypeDef = {  # (1)
    "thingTypeName": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListThingTypesRequestListThingTypesPaginateTypeDef](./type_defs.md#listthingtypesrequestlistthingtypespaginatetypedef) 
## ListThingsPaginator

Type annotations and code completion for `#!python session.create_client("iot").get_paginator("list_things")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot.html#IoT.Paginator.ListThings)

```python title="Usage example"
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
3. item: [:material-code-braces: ListThingsResponseTypeDef](./type_defs.md#listthingsresponsetypedef) 


### paginate

Type annotations and code completion for `#!python ListThingsPaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    attributeName: str = ...,
    attributeValue: str = ...,
    thingTypeName: str = ...,
    usePrefixAttributeValue: bool = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AsyncIterator[ListThingsResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListThingsResponseTypeDef](./type_defs.md#listthingsresponsetypedef) 


```python title="Usage example with kwargs"
kwargs: ListThingsRequestListThingsPaginateTypeDef = {  # (1)
    "attributeName": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListThingsRequestListThingsPaginateTypeDef](./type_defs.md#listthingsrequestlistthingspaginatetypedef) 
## ListThingsInBillingGroupPaginator

Type annotations and code completion for `#!python session.create_client("iot").get_paginator("list_things_in_billing_group")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot.html#IoT.Paginator.ListThingsInBillingGroup)

```python title="Usage example"
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
3. item: [:material-code-braces: ListThingsInBillingGroupResponseTypeDef](./type_defs.md#listthingsinbillinggroupresponsetypedef) 


### paginate

Type annotations and code completion for `#!python ListThingsInBillingGroupPaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    billingGroupName: str,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AsyncIterator[ListThingsInBillingGroupResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListThingsInBillingGroupResponseTypeDef](./type_defs.md#listthingsinbillinggroupresponsetypedef) 


```python title="Usage example with kwargs"
kwargs: ListThingsInBillingGroupRequestListThingsInBillingGroupPaginateTypeDef = {  # (1)
    "billingGroupName": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListThingsInBillingGroupRequestListThingsInBillingGroupPaginateTypeDef](./type_defs.md#listthingsinbillinggrouprequestlistthingsinbillinggrouppaginatetypedef) 
## ListThingsInThingGroupPaginator

Type annotations and code completion for `#!python session.create_client("iot").get_paginator("list_things_in_thing_group")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot.html#IoT.Paginator.ListThingsInThingGroup)

```python title="Usage example"
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
3. item: [:material-code-braces: ListThingsInThingGroupResponseTypeDef](./type_defs.md#listthingsinthinggroupresponsetypedef) 


### paginate

Type annotations and code completion for `#!python ListThingsInThingGroupPaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    thingGroupName: str,
    recursive: bool = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AsyncIterator[ListThingsInThingGroupResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListThingsInThingGroupResponseTypeDef](./type_defs.md#listthingsinthinggroupresponsetypedef) 


```python title="Usage example with kwargs"
kwargs: ListThingsInThingGroupRequestListThingsInThingGroupPaginateTypeDef = {  # (1)
    "thingGroupName": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListThingsInThingGroupRequestListThingsInThingGroupPaginateTypeDef](./type_defs.md#listthingsinthinggrouprequestlistthingsinthinggrouppaginatetypedef) 
## ListTopicRuleDestinationsPaginator

Type annotations and code completion for `#!python session.create_client("iot").get_paginator("list_topic_rule_destinations")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot.html#IoT.Paginator.ListTopicRuleDestinations)

```python title="Usage example"
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
3. item: [:material-code-braces: ListTopicRuleDestinationsResponseTypeDef](./type_defs.md#listtopicruledestinationsresponsetypedef) 


### paginate

Type annotations and code completion for `#!python ListTopicRuleDestinationsPaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AsyncIterator[ListTopicRuleDestinationsResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListTopicRuleDestinationsResponseTypeDef](./type_defs.md#listtopicruledestinationsresponsetypedef) 


```python title="Usage example with kwargs"
kwargs: ListTopicRuleDestinationsRequestListTopicRuleDestinationsPaginateTypeDef = {  # (1)
    "PaginationConfig": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListTopicRuleDestinationsRequestListTopicRuleDestinationsPaginateTypeDef](./type_defs.md#listtopicruledestinationsrequestlisttopicruledestinationspaginatetypedef) 
## ListTopicRulesPaginator

Type annotations and code completion for `#!python session.create_client("iot").get_paginator("list_topic_rules")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot.html#IoT.Paginator.ListTopicRules)

```python title="Usage example"
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
3. item: [:material-code-braces: ListTopicRulesResponseTypeDef](./type_defs.md#listtopicrulesresponsetypedef) 


### paginate

Type annotations and code completion for `#!python ListTopicRulesPaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    topic: str = ...,
    ruleDisabled: bool = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AsyncIterator[ListTopicRulesResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListTopicRulesResponseTypeDef](./type_defs.md#listtopicrulesresponsetypedef) 


```python title="Usage example with kwargs"
kwargs: ListTopicRulesRequestListTopicRulesPaginateTypeDef = {  # (1)
    "topic": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListTopicRulesRequestListTopicRulesPaginateTypeDef](./type_defs.md#listtopicrulesrequestlisttopicrulespaginatetypedef) 
## ListV2LoggingLevelsPaginator

Type annotations and code completion for `#!python session.create_client("iot").get_paginator("list_v2_logging_levels")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot.html#IoT.Paginator.ListV2LoggingLevels)

```python title="Usage example"
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
3. item: [:material-code-braces: ListV2LoggingLevelsResponseTypeDef](./type_defs.md#listv2logginglevelsresponsetypedef) 


### paginate

Type annotations and code completion for `#!python ListV2LoggingLevelsPaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    targetType: LogTargetTypeType = ...,  # (1)
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (2)
) -> AsyncIterator[ListV2LoggingLevelsResponseTypeDef]:  # (3)
    ...
```

1. See [:material-code-brackets: LogTargetTypeType](./literals.md#logtargettypetype) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
3. See [:material-code-braces: ListV2LoggingLevelsResponseTypeDef](./type_defs.md#listv2logginglevelsresponsetypedef) 


```python title="Usage example with kwargs"
kwargs: ListV2LoggingLevelsRequestListV2LoggingLevelsPaginateTypeDef = {  # (1)
    "targetType": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListV2LoggingLevelsRequestListV2LoggingLevelsPaginateTypeDef](./type_defs.md#listv2logginglevelsrequestlistv2logginglevelspaginatetypedef) 
## ListViolationEventsPaginator

Type annotations and code completion for `#!python session.create_client("iot").get_paginator("list_violation_events")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot.html#IoT.Paginator.ListViolationEvents)

```python title="Usage example"
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
3. item: [:material-code-braces: ListViolationEventsResponseTypeDef](./type_defs.md#listviolationeventsresponsetypedef) 


### paginate

Type annotations and code completion for `#!python ListViolationEventsPaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    startTime: Union[datetime, str],
    endTime: Union[datetime, str],
    thingName: str = ...,
    securityProfileName: str = ...,
    behaviorCriteriaType: BehaviorCriteriaTypeType = ...,  # (1)
    listSuppressedAlerts: bool = ...,
    verificationState: VerificationStateType = ...,  # (2)
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (3)
) -> AsyncIterator[ListViolationEventsResponseTypeDef]:  # (4)
    ...
```

1. See [:material-code-brackets: BehaviorCriteriaTypeType](./literals.md#behaviorcriteriatypetype) 
2. See [:material-code-brackets: VerificationStateType](./literals.md#verificationstatetype) 
3. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
4. See [:material-code-braces: ListViolationEventsResponseTypeDef](./type_defs.md#listviolationeventsresponsetypedef) 


```python title="Usage example with kwargs"
kwargs: ListViolationEventsRequestListViolationEventsPaginateTypeDef = {  # (1)
    "startTime": ...,
    "endTime": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListViolationEventsRequestListViolationEventsPaginateTypeDef](./type_defs.md#listviolationeventsrequestlistviolationeventspaginatetypedef) 
