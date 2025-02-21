# Paginators

> [Index](../README.md) > [ComputeOptimizer](./README.md) > Paginators

!!! note ""

    Auto-generated documentation for [ComputeOptimizer](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/compute-optimizer.html#computeoptimizer)
    type annotations stubs module [types-aiobotocore-compute-optimizer](https://pypi.org/project/types-aiobotocore-compute-optimizer/).

## DescribeRecommendationExportJobsPaginator

Type annotations and code completion for `#!python session.create_client("compute-optimizer").get_paginator("describe_recommendation_export_jobs")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/compute-optimizer/paginator/DescribeRecommendationExportJobs.html#ComputeOptimizer.Paginator.DescribeRecommendationExportJobs)

```python
# DescribeRecommendationExportJobsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_compute_optimizer.paginator import DescribeRecommendationExportJobsPaginator

session = get_session()
async with session.create_client("compute-optimizer") as client:  # (1)
    paginator: DescribeRecommendationExportJobsPaginator = client.get_paginator("describe_recommendation_export_jobs")  # (2)
    async for item in paginator.paginate(...):
        item: DescribeRecommendationExportJobsResponseTypeDef
        print(item)  # (3)
```

1. client: [ComputeOptimizerClient](./client.md)
2. paginator: [DescribeRecommendationExportJobsPaginator](./paginators.md#describerecommendationexportjobspaginator)
3. item: [:material-code-braces: DescribeRecommendationExportJobsResponseTypeDef](./type_defs.md#describerecommendationexportjobsresponsetypedef) 


### paginate

Type annotations and code completion for `#!python DescribeRecommendationExportJobsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    jobIds: Sequence[str] = ...,
    filters: Sequence[JobFilterTypeDef] = ...,  # (1)
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (2)
) -> AioPageIterator[DescribeRecommendationExportJobsResponseTypeDef]:  # (3)
    ...
```

1. See [:material-code-braces: JobFilterTypeDef](./type_defs.md#jobfiltertypedef) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
3. See [:material-code-braces: DescribeRecommendationExportJobsResponseTypeDef](./type_defs.md#describerecommendationexportjobsresponsetypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: DescribeRecommendationExportJobsRequestPaginateTypeDef = {  # (1)
    "jobIds": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: DescribeRecommendationExportJobsRequestPaginateTypeDef](./type_defs.md#describerecommendationexportjobsrequestpaginatetypedef) 
## GetEnrollmentStatusesForOrganizationPaginator

Type annotations and code completion for `#!python session.create_client("compute-optimizer").get_paginator("get_enrollment_statuses_for_organization")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/compute-optimizer/paginator/GetEnrollmentStatusesForOrganization.html#ComputeOptimizer.Paginator.GetEnrollmentStatusesForOrganization)

```python
# GetEnrollmentStatusesForOrganizationPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_compute_optimizer.paginator import GetEnrollmentStatusesForOrganizationPaginator

session = get_session()
async with session.create_client("compute-optimizer") as client:  # (1)
    paginator: GetEnrollmentStatusesForOrganizationPaginator = client.get_paginator("get_enrollment_statuses_for_organization")  # (2)
    async for item in paginator.paginate(...):
        item: GetEnrollmentStatusesForOrganizationResponseTypeDef
        print(item)  # (3)
```

1. client: [ComputeOptimizerClient](./client.md)
2. paginator: [GetEnrollmentStatusesForOrganizationPaginator](./paginators.md#getenrollmentstatusesfororganizationpaginator)
3. item: [:material-code-braces: GetEnrollmentStatusesForOrganizationResponseTypeDef](./type_defs.md#getenrollmentstatusesfororganizationresponsetypedef) 


### paginate

Type annotations and code completion for `#!python GetEnrollmentStatusesForOrganizationPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    filters: Sequence[EnrollmentFilterTypeDef] = ...,  # (1)
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (2)
) -> AioPageIterator[GetEnrollmentStatusesForOrganizationResponseTypeDef]:  # (3)
    ...
```

1. See [:material-code-braces: EnrollmentFilterTypeDef](./type_defs.md#enrollmentfiltertypedef) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
3. See [:material-code-braces: GetEnrollmentStatusesForOrganizationResponseTypeDef](./type_defs.md#getenrollmentstatusesfororganizationresponsetypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: GetEnrollmentStatusesForOrganizationRequestPaginateTypeDef = {  # (1)
    "filters": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: GetEnrollmentStatusesForOrganizationRequestPaginateTypeDef](./type_defs.md#getenrollmentstatusesfororganizationrequestpaginatetypedef) 
## GetLambdaFunctionRecommendationsPaginator

Type annotations and code completion for `#!python session.create_client("compute-optimizer").get_paginator("get_lambda_function_recommendations")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/compute-optimizer/paginator/GetLambdaFunctionRecommendations.html#ComputeOptimizer.Paginator.GetLambdaFunctionRecommendations)

```python
# GetLambdaFunctionRecommendationsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_compute_optimizer.paginator import GetLambdaFunctionRecommendationsPaginator

session = get_session()
async with session.create_client("compute-optimizer") as client:  # (1)
    paginator: GetLambdaFunctionRecommendationsPaginator = client.get_paginator("get_lambda_function_recommendations")  # (2)
    async for item in paginator.paginate(...):
        item: GetLambdaFunctionRecommendationsResponseTypeDef
        print(item)  # (3)
```

1. client: [ComputeOptimizerClient](./client.md)
2. paginator: [GetLambdaFunctionRecommendationsPaginator](./paginators.md#getlambdafunctionrecommendationspaginator)
3. item: [:material-code-braces: GetLambdaFunctionRecommendationsResponseTypeDef](./type_defs.md#getlambdafunctionrecommendationsresponsetypedef) 


### paginate

Type annotations and code completion for `#!python GetLambdaFunctionRecommendationsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    functionArns: Sequence[str] = ...,
    accountIds: Sequence[str] = ...,
    filters: Sequence[LambdaFunctionRecommendationFilterTypeDef] = ...,  # (1)
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (2)
) -> AioPageIterator[GetLambdaFunctionRecommendationsResponseTypeDef]:  # (3)
    ...
```

1. See [:material-code-braces: LambdaFunctionRecommendationFilterTypeDef](./type_defs.md#lambdafunctionrecommendationfiltertypedef) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
3. See [:material-code-braces: GetLambdaFunctionRecommendationsResponseTypeDef](./type_defs.md#getlambdafunctionrecommendationsresponsetypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: GetLambdaFunctionRecommendationsRequestPaginateTypeDef = {  # (1)
    "functionArns": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: GetLambdaFunctionRecommendationsRequestPaginateTypeDef](./type_defs.md#getlambdafunctionrecommendationsrequestpaginatetypedef) 
## GetRecommendationPreferencesPaginator

Type annotations and code completion for `#!python session.create_client("compute-optimizer").get_paginator("get_recommendation_preferences")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/compute-optimizer/paginator/GetRecommendationPreferences.html#ComputeOptimizer.Paginator.GetRecommendationPreferences)

```python
# GetRecommendationPreferencesPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_compute_optimizer.paginator import GetRecommendationPreferencesPaginator

session = get_session()
async with session.create_client("compute-optimizer") as client:  # (1)
    paginator: GetRecommendationPreferencesPaginator = client.get_paginator("get_recommendation_preferences")  # (2)
    async for item in paginator.paginate(...):
        item: GetRecommendationPreferencesResponseTypeDef
        print(item)  # (3)
```

1. client: [ComputeOptimizerClient](./client.md)
2. paginator: [GetRecommendationPreferencesPaginator](./paginators.md#getrecommendationpreferencespaginator)
3. item: [:material-code-braces: GetRecommendationPreferencesResponseTypeDef](./type_defs.md#getrecommendationpreferencesresponsetypedef) 


### paginate

Type annotations and code completion for `#!python GetRecommendationPreferencesPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    resourceType: ResourceTypeType,  # (1)
    scope: ScopeTypeDef = ...,  # (2)
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (3)
) -> AioPageIterator[GetRecommendationPreferencesResponseTypeDef]:  # (4)
    ...
```

1. See [:material-code-brackets: ResourceTypeType](./literals.md#resourcetypetype) 
2. See [:material-code-braces: ScopeTypeDef](./type_defs.md#scopetypedef) 
3. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
4. See [:material-code-braces: GetRecommendationPreferencesResponseTypeDef](./type_defs.md#getrecommendationpreferencesresponsetypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: GetRecommendationPreferencesRequestPaginateTypeDef = {  # (1)
    "resourceType": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: GetRecommendationPreferencesRequestPaginateTypeDef](./type_defs.md#getrecommendationpreferencesrequestpaginatetypedef) 
## GetRecommendationSummariesPaginator

Type annotations and code completion for `#!python session.create_client("compute-optimizer").get_paginator("get_recommendation_summaries")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/compute-optimizer/paginator/GetRecommendationSummaries.html#ComputeOptimizer.Paginator.GetRecommendationSummaries)

```python
# GetRecommendationSummariesPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_compute_optimizer.paginator import GetRecommendationSummariesPaginator

session = get_session()
async with session.create_client("compute-optimizer") as client:  # (1)
    paginator: GetRecommendationSummariesPaginator = client.get_paginator("get_recommendation_summaries")  # (2)
    async for item in paginator.paginate(...):
        item: GetRecommendationSummariesResponseTypeDef
        print(item)  # (3)
```

1. client: [ComputeOptimizerClient](./client.md)
2. paginator: [GetRecommendationSummariesPaginator](./paginators.md#getrecommendationsummariespaginator)
3. item: [:material-code-braces: GetRecommendationSummariesResponseTypeDef](./type_defs.md#getrecommendationsummariesresponsetypedef) 


### paginate

Type annotations and code completion for `#!python GetRecommendationSummariesPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    accountIds: Sequence[str] = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AioPageIterator[GetRecommendationSummariesResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: GetRecommendationSummariesResponseTypeDef](./type_defs.md#getrecommendationsummariesresponsetypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: GetRecommendationSummariesRequestPaginateTypeDef = {  # (1)
    "accountIds": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: GetRecommendationSummariesRequestPaginateTypeDef](./type_defs.md#getrecommendationsummariesrequestpaginatetypedef) 
