# Paginators

> [Index](../README.md) > [SecurityHub](./README.md) > Paginators

!!! note ""

    Auto-generated documentation for [SecurityHub](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/securityhub.html#securityhub)
    type annotations stubs module [types-aiobotocore-securityhub](https://pypi.org/project/types-aiobotocore-securityhub/).

## DescribeActionTargetsPaginator

Type annotations and code completion for `#!python session.create_client("securityhub").get_paginator("describe_action_targets")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/securityhub/paginator/DescribeActionTargets.html#SecurityHub.Paginator.DescribeActionTargets)

```python
# DescribeActionTargetsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_securityhub.paginator import DescribeActionTargetsPaginator

session = get_session()
async with session.create_client("securityhub") as client:  # (1)
    paginator: DescribeActionTargetsPaginator = client.get_paginator("describe_action_targets")  # (2)
    async for item in paginator.paginate(...):
        item: DescribeActionTargetsResponseTypeDef
        print(item)  # (3)
```

1. client: [SecurityHubClient](./client.md)
2. paginator: [DescribeActionTargetsPaginator](./paginators.md#describeactiontargetspaginator)
3. item: [:material-code-braces: DescribeActionTargetsResponseTypeDef](./type_defs.md#describeactiontargetsresponsetypedef) 


### paginate

Type annotations and code completion for `#!python DescribeActionTargetsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    ActionTargetArns: Sequence[str] = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AioPageIterator[DescribeActionTargetsResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: DescribeActionTargetsResponseTypeDef](./type_defs.md#describeactiontargetsresponsetypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: DescribeActionTargetsRequestPaginateTypeDef = {  # (1)
    "ActionTargetArns": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: DescribeActionTargetsRequestPaginateTypeDef](./type_defs.md#describeactiontargetsrequestpaginatetypedef) 
## DescribeProductsPaginator

Type annotations and code completion for `#!python session.create_client("securityhub").get_paginator("describe_products")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/securityhub/paginator/DescribeProducts.html#SecurityHub.Paginator.DescribeProducts)

```python
# DescribeProductsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_securityhub.paginator import DescribeProductsPaginator

session = get_session()
async with session.create_client("securityhub") as client:  # (1)
    paginator: DescribeProductsPaginator = client.get_paginator("describe_products")  # (2)
    async for item in paginator.paginate(...):
        item: DescribeProductsResponseTypeDef
        print(item)  # (3)
```

1. client: [SecurityHubClient](./client.md)
2. paginator: [DescribeProductsPaginator](./paginators.md#describeproductspaginator)
3. item: [:material-code-braces: DescribeProductsResponseTypeDef](./type_defs.md#describeproductsresponsetypedef) 


### paginate

Type annotations and code completion for `#!python DescribeProductsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    ProductArn: str = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AioPageIterator[DescribeProductsResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: DescribeProductsResponseTypeDef](./type_defs.md#describeproductsresponsetypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: DescribeProductsRequestPaginateTypeDef = {  # (1)
    "ProductArn": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: DescribeProductsRequestPaginateTypeDef](./type_defs.md#describeproductsrequestpaginatetypedef) 
## DescribeStandardsControlsPaginator

Type annotations and code completion for `#!python session.create_client("securityhub").get_paginator("describe_standards_controls")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/securityhub/paginator/DescribeStandardsControls.html#SecurityHub.Paginator.DescribeStandardsControls)

```python
# DescribeStandardsControlsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_securityhub.paginator import DescribeStandardsControlsPaginator

session = get_session()
async with session.create_client("securityhub") as client:  # (1)
    paginator: DescribeStandardsControlsPaginator = client.get_paginator("describe_standards_controls")  # (2)
    async for item in paginator.paginate(...):
        item: DescribeStandardsControlsResponseTypeDef
        print(item)  # (3)
```

1. client: [SecurityHubClient](./client.md)
2. paginator: [DescribeStandardsControlsPaginator](./paginators.md#describestandardscontrolspaginator)
3. item: [:material-code-braces: DescribeStandardsControlsResponseTypeDef](./type_defs.md#describestandardscontrolsresponsetypedef) 


### paginate

Type annotations and code completion for `#!python DescribeStandardsControlsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    StandardsSubscriptionArn: str,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AioPageIterator[DescribeStandardsControlsResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: DescribeStandardsControlsResponseTypeDef](./type_defs.md#describestandardscontrolsresponsetypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: DescribeStandardsControlsRequestPaginateTypeDef = {  # (1)
    "StandardsSubscriptionArn": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: DescribeStandardsControlsRequestPaginateTypeDef](./type_defs.md#describestandardscontrolsrequestpaginatetypedef) 
## DescribeStandardsPaginator

Type annotations and code completion for `#!python session.create_client("securityhub").get_paginator("describe_standards")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/securityhub/paginator/DescribeStandards.html#SecurityHub.Paginator.DescribeStandards)

```python
# DescribeStandardsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_securityhub.paginator import DescribeStandardsPaginator

session = get_session()
async with session.create_client("securityhub") as client:  # (1)
    paginator: DescribeStandardsPaginator = client.get_paginator("describe_standards")  # (2)
    async for item in paginator.paginate(...):
        item: DescribeStandardsResponseTypeDef
        print(item)  # (3)
```

1. client: [SecurityHubClient](./client.md)
2. paginator: [DescribeStandardsPaginator](./paginators.md#describestandardspaginator)
3. item: [:material-code-braces: DescribeStandardsResponseTypeDef](./type_defs.md#describestandardsresponsetypedef) 


### paginate

Type annotations and code completion for `#!python DescribeStandardsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AioPageIterator[DescribeStandardsResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: DescribeStandardsResponseTypeDef](./type_defs.md#describestandardsresponsetypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: DescribeStandardsRequestPaginateTypeDef = {  # (1)
    "PaginationConfig": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: DescribeStandardsRequestPaginateTypeDef](./type_defs.md#describestandardsrequestpaginatetypedef) 
## GetEnabledStandardsPaginator

Type annotations and code completion for `#!python session.create_client("securityhub").get_paginator("get_enabled_standards")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/securityhub/paginator/GetEnabledStandards.html#SecurityHub.Paginator.GetEnabledStandards)

```python
# GetEnabledStandardsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_securityhub.paginator import GetEnabledStandardsPaginator

session = get_session()
async with session.create_client("securityhub") as client:  # (1)
    paginator: GetEnabledStandardsPaginator = client.get_paginator("get_enabled_standards")  # (2)
    async for item in paginator.paginate(...):
        item: GetEnabledStandardsResponseTypeDef
        print(item)  # (3)
```

1. client: [SecurityHubClient](./client.md)
2. paginator: [GetEnabledStandardsPaginator](./paginators.md#getenabledstandardspaginator)
3. item: [:material-code-braces: GetEnabledStandardsResponseTypeDef](./type_defs.md#getenabledstandardsresponsetypedef) 


### paginate

Type annotations and code completion for `#!python GetEnabledStandardsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    StandardsSubscriptionArns: Sequence[str] = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AioPageIterator[GetEnabledStandardsResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: GetEnabledStandardsResponseTypeDef](./type_defs.md#getenabledstandardsresponsetypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: GetEnabledStandardsRequestPaginateTypeDef = {  # (1)
    "StandardsSubscriptionArns": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: GetEnabledStandardsRequestPaginateTypeDef](./type_defs.md#getenabledstandardsrequestpaginatetypedef) 
## GetFindingHistoryPaginator

Type annotations and code completion for `#!python session.create_client("securityhub").get_paginator("get_finding_history")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/securityhub/paginator/GetFindingHistory.html#SecurityHub.Paginator.GetFindingHistory)

```python
# GetFindingHistoryPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_securityhub.paginator import GetFindingHistoryPaginator

session = get_session()
async with session.create_client("securityhub") as client:  # (1)
    paginator: GetFindingHistoryPaginator = client.get_paginator("get_finding_history")  # (2)
    async for item in paginator.paginate(...):
        item: GetFindingHistoryResponseTypeDef
        print(item)  # (3)
```

1. client: [SecurityHubClient](./client.md)
2. paginator: [GetFindingHistoryPaginator](./paginators.md#getfindinghistorypaginator)
3. item: [:material-code-braces: GetFindingHistoryResponseTypeDef](./type_defs.md#getfindinghistoryresponsetypedef) 


### paginate

Type annotations and code completion for `#!python GetFindingHistoryPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    FindingIdentifier: AwsSecurityFindingIdentifierTypeDef,  # (1)
    StartTime: TimestampTypeDef = ...,
    EndTime: TimestampTypeDef = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (2)
) -> AioPageIterator[GetFindingHistoryResponseTypeDef]:  # (3)
    ...
```

1. See [:material-code-braces: AwsSecurityFindingIdentifierTypeDef](./type_defs.md#awssecurityfindingidentifiertypedef) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
3. See [:material-code-braces: GetFindingHistoryResponseTypeDef](./type_defs.md#getfindinghistoryresponsetypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: GetFindingHistoryRequestPaginateTypeDef = {  # (1)
    "FindingIdentifier": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: GetFindingHistoryRequestPaginateTypeDef](./type_defs.md#getfindinghistoryrequestpaginatetypedef) 
## GetFindingsPaginator

Type annotations and code completion for `#!python session.create_client("securityhub").get_paginator("get_findings")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/securityhub/paginator/GetFindings.html#SecurityHub.Paginator.GetFindings)

```python
# GetFindingsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_securityhub.paginator import GetFindingsPaginator

session = get_session()
async with session.create_client("securityhub") as client:  # (1)
    paginator: GetFindingsPaginator = client.get_paginator("get_findings")  # (2)
    async for item in paginator.paginate(...):
        item: GetFindingsResponseTypeDef
        print(item)  # (3)
```

1. client: [SecurityHubClient](./client.md)
2. paginator: [GetFindingsPaginator](./paginators.md#getfindingspaginator)
3. item: [:material-code-braces: GetFindingsResponseTypeDef](./type_defs.md#getfindingsresponsetypedef) 


### paginate

Type annotations and code completion for `#!python GetFindingsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    Filters: AwsSecurityFindingFiltersUnionTypeDef = ...,  # (1)
    SortCriteria: Sequence[SortCriterionTypeDef] = ...,  # (2)
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (3)
) -> AioPageIterator[GetFindingsResponseTypeDef]:  # (4)
    ...
```

1. See [:material-code-braces: AwsSecurityFindingFiltersTypeDef](./type_defs.md#awssecurityfindingfilterstypedef) [:material-code-braces: AwsSecurityFindingFiltersOutputTypeDef](./type_defs.md#awssecurityfindingfiltersoutputtypedef) 
2. See [:material-code-braces: SortCriterionTypeDef](./type_defs.md#sortcriteriontypedef) 
3. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
4. See [:material-code-braces: GetFindingsResponseTypeDef](./type_defs.md#getfindingsresponsetypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: GetFindingsRequestPaginateTypeDef = {  # (1)
    "Filters": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: GetFindingsRequestPaginateTypeDef](./type_defs.md#getfindingsrequestpaginatetypedef) 
## GetInsightsPaginator

Type annotations and code completion for `#!python session.create_client("securityhub").get_paginator("get_insights")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/securityhub/paginator/GetInsights.html#SecurityHub.Paginator.GetInsights)

```python
# GetInsightsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_securityhub.paginator import GetInsightsPaginator

session = get_session()
async with session.create_client("securityhub") as client:  # (1)
    paginator: GetInsightsPaginator = client.get_paginator("get_insights")  # (2)
    async for item in paginator.paginate(...):
        item: GetInsightsResponseTypeDef
        print(item)  # (3)
```

1. client: [SecurityHubClient](./client.md)
2. paginator: [GetInsightsPaginator](./paginators.md#getinsightspaginator)
3. item: [:material-code-braces: GetInsightsResponseTypeDef](./type_defs.md#getinsightsresponsetypedef) 


### paginate

Type annotations and code completion for `#!python GetInsightsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    InsightArns: Sequence[str] = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AioPageIterator[GetInsightsResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: GetInsightsResponseTypeDef](./type_defs.md#getinsightsresponsetypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: GetInsightsRequestPaginateTypeDef = {  # (1)
    "InsightArns": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: GetInsightsRequestPaginateTypeDef](./type_defs.md#getinsightsrequestpaginatetypedef) 
## ListConfigurationPoliciesPaginator

Type annotations and code completion for `#!python session.create_client("securityhub").get_paginator("list_configuration_policies")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/securityhub/paginator/ListConfigurationPolicies.html#SecurityHub.Paginator.ListConfigurationPolicies)

```python
# ListConfigurationPoliciesPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_securityhub.paginator import ListConfigurationPoliciesPaginator

session = get_session()
async with session.create_client("securityhub") as client:  # (1)
    paginator: ListConfigurationPoliciesPaginator = client.get_paginator("list_configuration_policies")  # (2)
    async for item in paginator.paginate(...):
        item: ListConfigurationPoliciesResponseTypeDef
        print(item)  # (3)
```

1. client: [SecurityHubClient](./client.md)
2. paginator: [ListConfigurationPoliciesPaginator](./paginators.md#listconfigurationpoliciespaginator)
3. item: [:material-code-braces: ListConfigurationPoliciesResponseTypeDef](./type_defs.md#listconfigurationpoliciesresponsetypedef) 


### paginate

Type annotations and code completion for `#!python ListConfigurationPoliciesPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AioPageIterator[ListConfigurationPoliciesResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListConfigurationPoliciesResponseTypeDef](./type_defs.md#listconfigurationpoliciesresponsetypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: ListConfigurationPoliciesRequestPaginateTypeDef = {  # (1)
    "PaginationConfig": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListConfigurationPoliciesRequestPaginateTypeDef](./type_defs.md#listconfigurationpoliciesrequestpaginatetypedef) 
## ListConfigurationPolicyAssociationsPaginator

Type annotations and code completion for `#!python session.create_client("securityhub").get_paginator("list_configuration_policy_associations")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/securityhub/paginator/ListConfigurationPolicyAssociations.html#SecurityHub.Paginator.ListConfigurationPolicyAssociations)

```python
# ListConfigurationPolicyAssociationsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_securityhub.paginator import ListConfigurationPolicyAssociationsPaginator

session = get_session()
async with session.create_client("securityhub") as client:  # (1)
    paginator: ListConfigurationPolicyAssociationsPaginator = client.get_paginator("list_configuration_policy_associations")  # (2)
    async for item in paginator.paginate(...):
        item: ListConfigurationPolicyAssociationsResponseTypeDef
        print(item)  # (3)
```

1. client: [SecurityHubClient](./client.md)
2. paginator: [ListConfigurationPolicyAssociationsPaginator](./paginators.md#listconfigurationpolicyassociationspaginator)
3. item: [:material-code-braces: ListConfigurationPolicyAssociationsResponseTypeDef](./type_defs.md#listconfigurationpolicyassociationsresponsetypedef) 


### paginate

Type annotations and code completion for `#!python ListConfigurationPolicyAssociationsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    Filters: AssociationFiltersTypeDef = ...,  # (1)
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (2)
) -> AioPageIterator[ListConfigurationPolicyAssociationsResponseTypeDef]:  # (3)
    ...
```

1. See [:material-code-braces: AssociationFiltersTypeDef](./type_defs.md#associationfilterstypedef) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
3. See [:material-code-braces: ListConfigurationPolicyAssociationsResponseTypeDef](./type_defs.md#listconfigurationpolicyassociationsresponsetypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: ListConfigurationPolicyAssociationsRequestPaginateTypeDef = {  # (1)
    "Filters": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListConfigurationPolicyAssociationsRequestPaginateTypeDef](./type_defs.md#listconfigurationpolicyassociationsrequestpaginatetypedef) 
## ListEnabledProductsForImportPaginator

Type annotations and code completion for `#!python session.create_client("securityhub").get_paginator("list_enabled_products_for_import")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/securityhub/paginator/ListEnabledProductsForImport.html#SecurityHub.Paginator.ListEnabledProductsForImport)

```python
# ListEnabledProductsForImportPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_securityhub.paginator import ListEnabledProductsForImportPaginator

session = get_session()
async with session.create_client("securityhub") as client:  # (1)
    paginator: ListEnabledProductsForImportPaginator = client.get_paginator("list_enabled_products_for_import")  # (2)
    async for item in paginator.paginate(...):
        item: ListEnabledProductsForImportResponseTypeDef
        print(item)  # (3)
```

1. client: [SecurityHubClient](./client.md)
2. paginator: [ListEnabledProductsForImportPaginator](./paginators.md#listenabledproductsforimportpaginator)
3. item: [:material-code-braces: ListEnabledProductsForImportResponseTypeDef](./type_defs.md#listenabledproductsforimportresponsetypedef) 


### paginate

Type annotations and code completion for `#!python ListEnabledProductsForImportPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AioPageIterator[ListEnabledProductsForImportResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListEnabledProductsForImportResponseTypeDef](./type_defs.md#listenabledproductsforimportresponsetypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: ListEnabledProductsForImportRequestPaginateTypeDef = {  # (1)
    "PaginationConfig": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListEnabledProductsForImportRequestPaginateTypeDef](./type_defs.md#listenabledproductsforimportrequestpaginatetypedef) 
## ListFindingAggregatorsPaginator

Type annotations and code completion for `#!python session.create_client("securityhub").get_paginator("list_finding_aggregators")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/securityhub/paginator/ListFindingAggregators.html#SecurityHub.Paginator.ListFindingAggregators)

```python
# ListFindingAggregatorsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_securityhub.paginator import ListFindingAggregatorsPaginator

session = get_session()
async with session.create_client("securityhub") as client:  # (1)
    paginator: ListFindingAggregatorsPaginator = client.get_paginator("list_finding_aggregators")  # (2)
    async for item in paginator.paginate(...):
        item: ListFindingAggregatorsResponseTypeDef
        print(item)  # (3)
```

1. client: [SecurityHubClient](./client.md)
2. paginator: [ListFindingAggregatorsPaginator](./paginators.md#listfindingaggregatorspaginator)
3. item: [:material-code-braces: ListFindingAggregatorsResponseTypeDef](./type_defs.md#listfindingaggregatorsresponsetypedef) 


### paginate

Type annotations and code completion for `#!python ListFindingAggregatorsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AioPageIterator[ListFindingAggregatorsResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListFindingAggregatorsResponseTypeDef](./type_defs.md#listfindingaggregatorsresponsetypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: ListFindingAggregatorsRequestPaginateTypeDef = {  # (1)
    "PaginationConfig": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListFindingAggregatorsRequestPaginateTypeDef](./type_defs.md#listfindingaggregatorsrequestpaginatetypedef) 
## ListInvitationsPaginator

Type annotations and code completion for `#!python session.create_client("securityhub").get_paginator("list_invitations")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/securityhub/paginator/ListInvitations.html#SecurityHub.Paginator.ListInvitations)

```python
# ListInvitationsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_securityhub.paginator import ListInvitationsPaginator

session = get_session()
async with session.create_client("securityhub") as client:  # (1)
    paginator: ListInvitationsPaginator = client.get_paginator("list_invitations")  # (2)
    async for item in paginator.paginate(...):
        item: ListInvitationsResponseTypeDef
        print(item)  # (3)
```

1. client: [SecurityHubClient](./client.md)
2. paginator: [ListInvitationsPaginator](./paginators.md#listinvitationspaginator)
3. item: [:material-code-braces: ListInvitationsResponseTypeDef](./type_defs.md#listinvitationsresponsetypedef) 


### paginate

Type annotations and code completion for `#!python ListInvitationsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AioPageIterator[ListInvitationsResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListInvitationsResponseTypeDef](./type_defs.md#listinvitationsresponsetypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: ListInvitationsRequestPaginateTypeDef = {  # (1)
    "PaginationConfig": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListInvitationsRequestPaginateTypeDef](./type_defs.md#listinvitationsrequestpaginatetypedef) 
## ListMembersPaginator

Type annotations and code completion for `#!python session.create_client("securityhub").get_paginator("list_members")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/securityhub/paginator/ListMembers.html#SecurityHub.Paginator.ListMembers)

```python
# ListMembersPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_securityhub.paginator import ListMembersPaginator

session = get_session()
async with session.create_client("securityhub") as client:  # (1)
    paginator: ListMembersPaginator = client.get_paginator("list_members")  # (2)
    async for item in paginator.paginate(...):
        item: ListMembersResponseTypeDef
        print(item)  # (3)
```

1. client: [SecurityHubClient](./client.md)
2. paginator: [ListMembersPaginator](./paginators.md#listmemberspaginator)
3. item: [:material-code-braces: ListMembersResponseTypeDef](./type_defs.md#listmembersresponsetypedef) 


### paginate

Type annotations and code completion for `#!python ListMembersPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    OnlyAssociated: bool = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AioPageIterator[ListMembersResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListMembersResponseTypeDef](./type_defs.md#listmembersresponsetypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: ListMembersRequestPaginateTypeDef = {  # (1)
    "OnlyAssociated": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListMembersRequestPaginateTypeDef](./type_defs.md#listmembersrequestpaginatetypedef) 
## ListOrganizationAdminAccountsPaginator

Type annotations and code completion for `#!python session.create_client("securityhub").get_paginator("list_organization_admin_accounts")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/securityhub/paginator/ListOrganizationAdminAccounts.html#SecurityHub.Paginator.ListOrganizationAdminAccounts)

```python
# ListOrganizationAdminAccountsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_securityhub.paginator import ListOrganizationAdminAccountsPaginator

session = get_session()
async with session.create_client("securityhub") as client:  # (1)
    paginator: ListOrganizationAdminAccountsPaginator = client.get_paginator("list_organization_admin_accounts")  # (2)
    async for item in paginator.paginate(...):
        item: ListOrganizationAdminAccountsResponseTypeDef
        print(item)  # (3)
```

1. client: [SecurityHubClient](./client.md)
2. paginator: [ListOrganizationAdminAccountsPaginator](./paginators.md#listorganizationadminaccountspaginator)
3. item: [:material-code-braces: ListOrganizationAdminAccountsResponseTypeDef](./type_defs.md#listorganizationadminaccountsresponsetypedef) 


### paginate

Type annotations and code completion for `#!python ListOrganizationAdminAccountsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AioPageIterator[ListOrganizationAdminAccountsResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListOrganizationAdminAccountsResponseTypeDef](./type_defs.md#listorganizationadminaccountsresponsetypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: ListOrganizationAdminAccountsRequestPaginateTypeDef = {  # (1)
    "PaginationConfig": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListOrganizationAdminAccountsRequestPaginateTypeDef](./type_defs.md#listorganizationadminaccountsrequestpaginatetypedef) 
## ListSecurityControlDefinitionsPaginator

Type annotations and code completion for `#!python session.create_client("securityhub").get_paginator("list_security_control_definitions")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/securityhub/paginator/ListSecurityControlDefinitions.html#SecurityHub.Paginator.ListSecurityControlDefinitions)

```python
# ListSecurityControlDefinitionsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_securityhub.paginator import ListSecurityControlDefinitionsPaginator

session = get_session()
async with session.create_client("securityhub") as client:  # (1)
    paginator: ListSecurityControlDefinitionsPaginator = client.get_paginator("list_security_control_definitions")  # (2)
    async for item in paginator.paginate(...):
        item: ListSecurityControlDefinitionsResponseTypeDef
        print(item)  # (3)
```

1. client: [SecurityHubClient](./client.md)
2. paginator: [ListSecurityControlDefinitionsPaginator](./paginators.md#listsecuritycontroldefinitionspaginator)
3. item: [:material-code-braces: ListSecurityControlDefinitionsResponseTypeDef](./type_defs.md#listsecuritycontroldefinitionsresponsetypedef) 


### paginate

Type annotations and code completion for `#!python ListSecurityControlDefinitionsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    StandardsArn: str = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AioPageIterator[ListSecurityControlDefinitionsResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListSecurityControlDefinitionsResponseTypeDef](./type_defs.md#listsecuritycontroldefinitionsresponsetypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: ListSecurityControlDefinitionsRequestPaginateTypeDef = {  # (1)
    "StandardsArn": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListSecurityControlDefinitionsRequestPaginateTypeDef](./type_defs.md#listsecuritycontroldefinitionsrequestpaginatetypedef) 
## ListStandardsControlAssociationsPaginator

Type annotations and code completion for `#!python session.create_client("securityhub").get_paginator("list_standards_control_associations")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/securityhub/paginator/ListStandardsControlAssociations.html#SecurityHub.Paginator.ListStandardsControlAssociations)

```python
# ListStandardsControlAssociationsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_securityhub.paginator import ListStandardsControlAssociationsPaginator

session = get_session()
async with session.create_client("securityhub") as client:  # (1)
    paginator: ListStandardsControlAssociationsPaginator = client.get_paginator("list_standards_control_associations")  # (2)
    async for item in paginator.paginate(...):
        item: ListStandardsControlAssociationsResponseTypeDef
        print(item)  # (3)
```

1. client: [SecurityHubClient](./client.md)
2. paginator: [ListStandardsControlAssociationsPaginator](./paginators.md#liststandardscontrolassociationspaginator)
3. item: [:material-code-braces: ListStandardsControlAssociationsResponseTypeDef](./type_defs.md#liststandardscontrolassociationsresponsetypedef) 


### paginate

Type annotations and code completion for `#!python ListStandardsControlAssociationsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    SecurityControlId: str,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AioPageIterator[ListStandardsControlAssociationsResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListStandardsControlAssociationsResponseTypeDef](./type_defs.md#liststandardscontrolassociationsresponsetypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: ListStandardsControlAssociationsRequestPaginateTypeDef = {  # (1)
    "SecurityControlId": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListStandardsControlAssociationsRequestPaginateTypeDef](./type_defs.md#liststandardscontrolassociationsrequestpaginatetypedef) 
