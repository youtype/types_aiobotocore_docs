# Paginators

> [Index](../README.md) > [Inspector](./README.md) > Paginators

!!! note ""

    Auto-generated documentation for [Inspector](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/inspector.html#inspector)
    type annotations stubs module [types-aiobotocore-inspector](https://pypi.org/project/types-aiobotocore-inspector/).

## ListAssessmentRunAgentsPaginator

Type annotations and code completion for `#!python session.create_client("inspector").get_paginator("list_assessment_run_agents")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/inspector/paginator/ListAssessmentRunAgents.html#Inspector.Paginator.ListAssessmentRunAgents)

```python
# ListAssessmentRunAgentsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_inspector.paginator import ListAssessmentRunAgentsPaginator

session = get_session()
async with session.create_client("inspector") as client:  # (1)
    paginator: ListAssessmentRunAgentsPaginator = client.get_paginator("list_assessment_run_agents")  # (2)
    async for item in paginator.paginate(...):
        item: ListAssessmentRunAgentsResponseTypeDef
        print(item)  # (3)
```

1. client: [InspectorClient](./client.md)
2. paginator: [ListAssessmentRunAgentsPaginator](./paginators.md#listassessmentrunagentspaginator)
3. item: [:material-code-braces: ListAssessmentRunAgentsResponseTypeDef](./type_defs.md#listassessmentrunagentsresponsetypedef) 


### paginate

Type annotations and code completion for `#!python ListAssessmentRunAgentsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    assessmentRunArn: str,
    filter: AgentFilterTypeDef = ...,  # (1)
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (2)
) -> AioPageIterator[ListAssessmentRunAgentsResponseTypeDef]:  # (3)
    ...
```

1. See [:material-code-braces: AgentFilterTypeDef](./type_defs.md#agentfiltertypedef) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
3. See [:material-code-braces: ListAssessmentRunAgentsResponseTypeDef](./type_defs.md#listassessmentrunagentsresponsetypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: ListAssessmentRunAgentsRequestPaginateTypeDef = {  # (1)
    "assessmentRunArn": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListAssessmentRunAgentsRequestPaginateTypeDef](./type_defs.md#listassessmentrunagentsrequestpaginatetypedef) 
## ListAssessmentRunsPaginator

Type annotations and code completion for `#!python session.create_client("inspector").get_paginator("list_assessment_runs")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/inspector/paginator/ListAssessmentRuns.html#Inspector.Paginator.ListAssessmentRuns)

```python
# ListAssessmentRunsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_inspector.paginator import ListAssessmentRunsPaginator

session = get_session()
async with session.create_client("inspector") as client:  # (1)
    paginator: ListAssessmentRunsPaginator = client.get_paginator("list_assessment_runs")  # (2)
    async for item in paginator.paginate(...):
        item: ListAssessmentRunsResponseTypeDef
        print(item)  # (3)
```

1. client: [InspectorClient](./client.md)
2. paginator: [ListAssessmentRunsPaginator](./paginators.md#listassessmentrunspaginator)
3. item: [:material-code-braces: ListAssessmentRunsResponseTypeDef](./type_defs.md#listassessmentrunsresponsetypedef) 


### paginate

Type annotations and code completion for `#!python ListAssessmentRunsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    assessmentTemplateArns: Sequence[str] = ...,
    filter: AssessmentRunFilterTypeDef = ...,  # (1)
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (2)
) -> AioPageIterator[ListAssessmentRunsResponseTypeDef]:  # (3)
    ...
```

1. See [:material-code-braces: AssessmentRunFilterTypeDef](./type_defs.md#assessmentrunfiltertypedef) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
3. See [:material-code-braces: ListAssessmentRunsResponseTypeDef](./type_defs.md#listassessmentrunsresponsetypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: ListAssessmentRunsRequestPaginateTypeDef = {  # (1)
    "assessmentTemplateArns": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListAssessmentRunsRequestPaginateTypeDef](./type_defs.md#listassessmentrunsrequestpaginatetypedef) 
## ListAssessmentTargetsPaginator

Type annotations and code completion for `#!python session.create_client("inspector").get_paginator("list_assessment_targets")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/inspector/paginator/ListAssessmentTargets.html#Inspector.Paginator.ListAssessmentTargets)

```python
# ListAssessmentTargetsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_inspector.paginator import ListAssessmentTargetsPaginator

session = get_session()
async with session.create_client("inspector") as client:  # (1)
    paginator: ListAssessmentTargetsPaginator = client.get_paginator("list_assessment_targets")  # (2)
    async for item in paginator.paginate(...):
        item: ListAssessmentTargetsResponseTypeDef
        print(item)  # (3)
```

1. client: [InspectorClient](./client.md)
2. paginator: [ListAssessmentTargetsPaginator](./paginators.md#listassessmenttargetspaginator)
3. item: [:material-code-braces: ListAssessmentTargetsResponseTypeDef](./type_defs.md#listassessmenttargetsresponsetypedef) 


### paginate

Type annotations and code completion for `#!python ListAssessmentTargetsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    filter: AssessmentTargetFilterTypeDef = ...,  # (1)
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (2)
) -> AioPageIterator[ListAssessmentTargetsResponseTypeDef]:  # (3)
    ...
```

1. See [:material-code-braces: AssessmentTargetFilterTypeDef](./type_defs.md#assessmenttargetfiltertypedef) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
3. See [:material-code-braces: ListAssessmentTargetsResponseTypeDef](./type_defs.md#listassessmenttargetsresponsetypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: ListAssessmentTargetsRequestPaginateTypeDef = {  # (1)
    "filter": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListAssessmentTargetsRequestPaginateTypeDef](./type_defs.md#listassessmenttargetsrequestpaginatetypedef) 
## ListAssessmentTemplatesPaginator

Type annotations and code completion for `#!python session.create_client("inspector").get_paginator("list_assessment_templates")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/inspector/paginator/ListAssessmentTemplates.html#Inspector.Paginator.ListAssessmentTemplates)

```python
# ListAssessmentTemplatesPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_inspector.paginator import ListAssessmentTemplatesPaginator

session = get_session()
async with session.create_client("inspector") as client:  # (1)
    paginator: ListAssessmentTemplatesPaginator = client.get_paginator("list_assessment_templates")  # (2)
    async for item in paginator.paginate(...):
        item: ListAssessmentTemplatesResponseTypeDef
        print(item)  # (3)
```

1. client: [InspectorClient](./client.md)
2. paginator: [ListAssessmentTemplatesPaginator](./paginators.md#listassessmenttemplatespaginator)
3. item: [:material-code-braces: ListAssessmentTemplatesResponseTypeDef](./type_defs.md#listassessmenttemplatesresponsetypedef) 


### paginate

Type annotations and code completion for `#!python ListAssessmentTemplatesPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    assessmentTargetArns: Sequence[str] = ...,
    filter: AssessmentTemplateFilterTypeDef = ...,  # (1)
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (2)
) -> AioPageIterator[ListAssessmentTemplatesResponseTypeDef]:  # (3)
    ...
```

1. See [:material-code-braces: AssessmentTemplateFilterTypeDef](./type_defs.md#assessmenttemplatefiltertypedef) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
3. See [:material-code-braces: ListAssessmentTemplatesResponseTypeDef](./type_defs.md#listassessmenttemplatesresponsetypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: ListAssessmentTemplatesRequestPaginateTypeDef = {  # (1)
    "assessmentTargetArns": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListAssessmentTemplatesRequestPaginateTypeDef](./type_defs.md#listassessmenttemplatesrequestpaginatetypedef) 
## ListEventSubscriptionsPaginator

Type annotations and code completion for `#!python session.create_client("inspector").get_paginator("list_event_subscriptions")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/inspector/paginator/ListEventSubscriptions.html#Inspector.Paginator.ListEventSubscriptions)

```python
# ListEventSubscriptionsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_inspector.paginator import ListEventSubscriptionsPaginator

session = get_session()
async with session.create_client("inspector") as client:  # (1)
    paginator: ListEventSubscriptionsPaginator = client.get_paginator("list_event_subscriptions")  # (2)
    async for item in paginator.paginate(...):
        item: ListEventSubscriptionsResponseTypeDef
        print(item)  # (3)
```

1. client: [InspectorClient](./client.md)
2. paginator: [ListEventSubscriptionsPaginator](./paginators.md#listeventsubscriptionspaginator)
3. item: [:material-code-braces: ListEventSubscriptionsResponseTypeDef](./type_defs.md#listeventsubscriptionsresponsetypedef) 


### paginate

Type annotations and code completion for `#!python ListEventSubscriptionsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    resourceArn: str = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AioPageIterator[ListEventSubscriptionsResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListEventSubscriptionsResponseTypeDef](./type_defs.md#listeventsubscriptionsresponsetypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: ListEventSubscriptionsRequestPaginateTypeDef = {  # (1)
    "resourceArn": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListEventSubscriptionsRequestPaginateTypeDef](./type_defs.md#listeventsubscriptionsrequestpaginatetypedef) 
## ListExclusionsPaginator

Type annotations and code completion for `#!python session.create_client("inspector").get_paginator("list_exclusions")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/inspector/paginator/ListExclusions.html#Inspector.Paginator.ListExclusions)

```python
# ListExclusionsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_inspector.paginator import ListExclusionsPaginator

session = get_session()
async with session.create_client("inspector") as client:  # (1)
    paginator: ListExclusionsPaginator = client.get_paginator("list_exclusions")  # (2)
    async for item in paginator.paginate(...):
        item: ListExclusionsResponseTypeDef
        print(item)  # (3)
```

1. client: [InspectorClient](./client.md)
2. paginator: [ListExclusionsPaginator](./paginators.md#listexclusionspaginator)
3. item: [:material-code-braces: ListExclusionsResponseTypeDef](./type_defs.md#listexclusionsresponsetypedef) 


### paginate

Type annotations and code completion for `#!python ListExclusionsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    assessmentRunArn: str,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AioPageIterator[ListExclusionsResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListExclusionsResponseTypeDef](./type_defs.md#listexclusionsresponsetypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: ListExclusionsRequestPaginateTypeDef = {  # (1)
    "assessmentRunArn": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListExclusionsRequestPaginateTypeDef](./type_defs.md#listexclusionsrequestpaginatetypedef) 
## ListFindingsPaginator

Type annotations and code completion for `#!python session.create_client("inspector").get_paginator("list_findings")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/inspector/paginator/ListFindings.html#Inspector.Paginator.ListFindings)

```python
# ListFindingsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_inspector.paginator import ListFindingsPaginator

session = get_session()
async with session.create_client("inspector") as client:  # (1)
    paginator: ListFindingsPaginator = client.get_paginator("list_findings")  # (2)
    async for item in paginator.paginate(...):
        item: ListFindingsResponseTypeDef
        print(item)  # (3)
```

1. client: [InspectorClient](./client.md)
2. paginator: [ListFindingsPaginator](./paginators.md#listfindingspaginator)
3. item: [:material-code-braces: ListFindingsResponseTypeDef](./type_defs.md#listfindingsresponsetypedef) 


### paginate

Type annotations and code completion for `#!python ListFindingsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    assessmentRunArns: Sequence[str] = ...,
    filter: FindingFilterTypeDef = ...,  # (1)
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (2)
) -> AioPageIterator[ListFindingsResponseTypeDef]:  # (3)
    ...
```

1. See [:material-code-braces: FindingFilterTypeDef](./type_defs.md#findingfiltertypedef) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
3. See [:material-code-braces: ListFindingsResponseTypeDef](./type_defs.md#listfindingsresponsetypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: ListFindingsRequestPaginateTypeDef = {  # (1)
    "assessmentRunArns": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListFindingsRequestPaginateTypeDef](./type_defs.md#listfindingsrequestpaginatetypedef) 
## ListRulesPackagesPaginator

Type annotations and code completion for `#!python session.create_client("inspector").get_paginator("list_rules_packages")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/inspector/paginator/ListRulesPackages.html#Inspector.Paginator.ListRulesPackages)

```python
# ListRulesPackagesPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_inspector.paginator import ListRulesPackagesPaginator

session = get_session()
async with session.create_client("inspector") as client:  # (1)
    paginator: ListRulesPackagesPaginator = client.get_paginator("list_rules_packages")  # (2)
    async for item in paginator.paginate(...):
        item: ListRulesPackagesResponseTypeDef
        print(item)  # (3)
```

1. client: [InspectorClient](./client.md)
2. paginator: [ListRulesPackagesPaginator](./paginators.md#listrulespackagespaginator)
3. item: [:material-code-braces: ListRulesPackagesResponseTypeDef](./type_defs.md#listrulespackagesresponsetypedef) 


### paginate

Type annotations and code completion for `#!python ListRulesPackagesPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AioPageIterator[ListRulesPackagesResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListRulesPackagesResponseTypeDef](./type_defs.md#listrulespackagesresponsetypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: ListRulesPackagesRequestPaginateTypeDef = {  # (1)
    "PaginationConfig": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListRulesPackagesRequestPaginateTypeDef](./type_defs.md#listrulespackagesrequestpaginatetypedef) 
## PreviewAgentsPaginator

Type annotations and code completion for `#!python session.create_client("inspector").get_paginator("preview_agents")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/inspector/paginator/PreviewAgents.html#Inspector.Paginator.PreviewAgents)

```python
# PreviewAgentsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_inspector.paginator import PreviewAgentsPaginator

session = get_session()
async with session.create_client("inspector") as client:  # (1)
    paginator: PreviewAgentsPaginator = client.get_paginator("preview_agents")  # (2)
    async for item in paginator.paginate(...):
        item: PreviewAgentsResponseTypeDef
        print(item)  # (3)
```

1. client: [InspectorClient](./client.md)
2. paginator: [PreviewAgentsPaginator](./paginators.md#previewagentspaginator)
3. item: [:material-code-braces: PreviewAgentsResponseTypeDef](./type_defs.md#previewagentsresponsetypedef) 


### paginate

Type annotations and code completion for `#!python PreviewAgentsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    previewAgentsArn: str,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AioPageIterator[PreviewAgentsResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: PreviewAgentsResponseTypeDef](./type_defs.md#previewagentsresponsetypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: PreviewAgentsRequestPaginateTypeDef = {  # (1)
    "previewAgentsArn": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: PreviewAgentsRequestPaginateTypeDef](./type_defs.md#previewagentsrequestpaginatetypedef) 
