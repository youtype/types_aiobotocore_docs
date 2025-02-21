# Paginators

> [Index](../README.md) > [Bedrock](./README.md) > Paginators

!!! note ""

    Auto-generated documentation for [Bedrock](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/bedrock.html#bedrock)
    type annotations stubs module [types-aiobotocore-bedrock](https://pypi.org/project/types-aiobotocore-bedrock/).

## ListCustomModelsPaginator

Type annotations and code completion for `#!python session.create_client("bedrock").get_paginator("list_custom_models")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/bedrock/paginator/ListCustomModels.html#Bedrock.Paginator.ListCustomModels)

```python
# ListCustomModelsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_bedrock.paginator import ListCustomModelsPaginator

session = get_session()
async with session.create_client("bedrock") as client:  # (1)
    paginator: ListCustomModelsPaginator = client.get_paginator("list_custom_models")  # (2)
    async for item in paginator.paginate(...):
        item: ListCustomModelsResponseTypeDef
        print(item)  # (3)
```

1. client: [BedrockClient](./client.md)
2. paginator: [ListCustomModelsPaginator](./paginators.md#listcustommodelspaginator)
3. item: [:material-code-braces: ListCustomModelsResponseTypeDef](./type_defs.md#listcustommodelsresponsetypedef) 


### paginate

Type annotations and code completion for `#!python ListCustomModelsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    creationTimeBefore: TimestampTypeDef = ...,
    creationTimeAfter: TimestampTypeDef = ...,
    nameContains: str = ...,
    baseModelArnEquals: str = ...,
    foundationModelArnEquals: str = ...,
    sortBy: SortModelsByType = ...,  # (1)
    sortOrder: SortOrderType = ...,  # (2)
    isOwned: bool = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (3)
) -> AioPageIterator[ListCustomModelsResponseTypeDef]:  # (4)
    ...
```

1. See [:material-code-brackets: SortModelsByType](./literals.md#sortmodelsbytype) 
2. See [:material-code-brackets: SortOrderType](./literals.md#sortordertype) 
3. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
4. See [:material-code-braces: ListCustomModelsResponseTypeDef](./type_defs.md#listcustommodelsresponsetypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: ListCustomModelsRequestPaginateTypeDef = {  # (1)
    "creationTimeBefore": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListCustomModelsRequestPaginateTypeDef](./type_defs.md#listcustommodelsrequestpaginatetypedef) 
## ListEvaluationJobsPaginator

Type annotations and code completion for `#!python session.create_client("bedrock").get_paginator("list_evaluation_jobs")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/bedrock/paginator/ListEvaluationJobs.html#Bedrock.Paginator.ListEvaluationJobs)

```python
# ListEvaluationJobsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_bedrock.paginator import ListEvaluationJobsPaginator

session = get_session()
async with session.create_client("bedrock") as client:  # (1)
    paginator: ListEvaluationJobsPaginator = client.get_paginator("list_evaluation_jobs")  # (2)
    async for item in paginator.paginate(...):
        item: ListEvaluationJobsResponseTypeDef
        print(item)  # (3)
```

1. client: [BedrockClient](./client.md)
2. paginator: [ListEvaluationJobsPaginator](./paginators.md#listevaluationjobspaginator)
3. item: [:material-code-braces: ListEvaluationJobsResponseTypeDef](./type_defs.md#listevaluationjobsresponsetypedef) 


### paginate

Type annotations and code completion for `#!python ListEvaluationJobsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    creationTimeAfter: TimestampTypeDef = ...,
    creationTimeBefore: TimestampTypeDef = ...,
    statusEquals: EvaluationJobStatusType = ...,  # (1)
    applicationTypeEquals: ApplicationTypeType = ...,  # (2)
    nameContains: str = ...,
    sortBy: SortJobsByType = ...,  # (3)
    sortOrder: SortOrderType = ...,  # (4)
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (5)
) -> AioPageIterator[ListEvaluationJobsResponseTypeDef]:  # (6)
    ...
```

1. See [:material-code-brackets: EvaluationJobStatusType](./literals.md#evaluationjobstatustype) 
2. See [:material-code-brackets: ApplicationTypeType](./literals.md#applicationtypetype) 
3. See [:material-code-brackets: SortJobsByType](./literals.md#sortjobsbytype) 
4. See [:material-code-brackets: SortOrderType](./literals.md#sortordertype) 
5. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
6. See [:material-code-braces: ListEvaluationJobsResponseTypeDef](./type_defs.md#listevaluationjobsresponsetypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: ListEvaluationJobsRequestPaginateTypeDef = {  # (1)
    "creationTimeAfter": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListEvaluationJobsRequestPaginateTypeDef](./type_defs.md#listevaluationjobsrequestpaginatetypedef) 
## ListGuardrailsPaginator

Type annotations and code completion for `#!python session.create_client("bedrock").get_paginator("list_guardrails")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/bedrock/paginator/ListGuardrails.html#Bedrock.Paginator.ListGuardrails)

```python
# ListGuardrailsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_bedrock.paginator import ListGuardrailsPaginator

session = get_session()
async with session.create_client("bedrock") as client:  # (1)
    paginator: ListGuardrailsPaginator = client.get_paginator("list_guardrails")  # (2)
    async for item in paginator.paginate(...):
        item: ListGuardrailsResponseTypeDef
        print(item)  # (3)
```

1. client: [BedrockClient](./client.md)
2. paginator: [ListGuardrailsPaginator](./paginators.md#listguardrailspaginator)
3. item: [:material-code-braces: ListGuardrailsResponseTypeDef](./type_defs.md#listguardrailsresponsetypedef) 


### paginate

Type annotations and code completion for `#!python ListGuardrailsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    guardrailIdentifier: str = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AioPageIterator[ListGuardrailsResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListGuardrailsResponseTypeDef](./type_defs.md#listguardrailsresponsetypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: ListGuardrailsRequestPaginateTypeDef = {  # (1)
    "guardrailIdentifier": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListGuardrailsRequestPaginateTypeDef](./type_defs.md#listguardrailsrequestpaginatetypedef) 
## ListImportedModelsPaginator

Type annotations and code completion for `#!python session.create_client("bedrock").get_paginator("list_imported_models")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/bedrock/paginator/ListImportedModels.html#Bedrock.Paginator.ListImportedModels)

```python
# ListImportedModelsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_bedrock.paginator import ListImportedModelsPaginator

session = get_session()
async with session.create_client("bedrock") as client:  # (1)
    paginator: ListImportedModelsPaginator = client.get_paginator("list_imported_models")  # (2)
    async for item in paginator.paginate(...):
        item: ListImportedModelsResponseTypeDef
        print(item)  # (3)
```

1. client: [BedrockClient](./client.md)
2. paginator: [ListImportedModelsPaginator](./paginators.md#listimportedmodelspaginator)
3. item: [:material-code-braces: ListImportedModelsResponseTypeDef](./type_defs.md#listimportedmodelsresponsetypedef) 


### paginate

Type annotations and code completion for `#!python ListImportedModelsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    creationTimeBefore: TimestampTypeDef = ...,
    creationTimeAfter: TimestampTypeDef = ...,
    nameContains: str = ...,
    sortBy: SortModelsByType = ...,  # (1)
    sortOrder: SortOrderType = ...,  # (2)
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (3)
) -> AioPageIterator[ListImportedModelsResponseTypeDef]:  # (4)
    ...
```

1. See [:material-code-brackets: SortModelsByType](./literals.md#sortmodelsbytype) 
2. See [:material-code-brackets: SortOrderType](./literals.md#sortordertype) 
3. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
4. See [:material-code-braces: ListImportedModelsResponseTypeDef](./type_defs.md#listimportedmodelsresponsetypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: ListImportedModelsRequestPaginateTypeDef = {  # (1)
    "creationTimeBefore": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListImportedModelsRequestPaginateTypeDef](./type_defs.md#listimportedmodelsrequestpaginatetypedef) 
## ListInferenceProfilesPaginator

Type annotations and code completion for `#!python session.create_client("bedrock").get_paginator("list_inference_profiles")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/bedrock/paginator/ListInferenceProfiles.html#Bedrock.Paginator.ListInferenceProfiles)

```python
# ListInferenceProfilesPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_bedrock.paginator import ListInferenceProfilesPaginator

session = get_session()
async with session.create_client("bedrock") as client:  # (1)
    paginator: ListInferenceProfilesPaginator = client.get_paginator("list_inference_profiles")  # (2)
    async for item in paginator.paginate(...):
        item: ListInferenceProfilesResponseTypeDef
        print(item)  # (3)
```

1. client: [BedrockClient](./client.md)
2. paginator: [ListInferenceProfilesPaginator](./paginators.md#listinferenceprofilespaginator)
3. item: [:material-code-braces: ListInferenceProfilesResponseTypeDef](./type_defs.md#listinferenceprofilesresponsetypedef) 


### paginate

Type annotations and code completion for `#!python ListInferenceProfilesPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    typeEquals: InferenceProfileTypeType = ...,  # (1)
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (2)
) -> AioPageIterator[ListInferenceProfilesResponseTypeDef]:  # (3)
    ...
```

1. See [:material-code-brackets: InferenceProfileTypeType](./literals.md#inferenceprofiletypetype) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
3. See [:material-code-braces: ListInferenceProfilesResponseTypeDef](./type_defs.md#listinferenceprofilesresponsetypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: ListInferenceProfilesRequestPaginateTypeDef = {  # (1)
    "typeEquals": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListInferenceProfilesRequestPaginateTypeDef](./type_defs.md#listinferenceprofilesrequestpaginatetypedef) 
## ListMarketplaceModelEndpointsPaginator

Type annotations and code completion for `#!python session.create_client("bedrock").get_paginator("list_marketplace_model_endpoints")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/bedrock/paginator/ListMarketplaceModelEndpoints.html#Bedrock.Paginator.ListMarketplaceModelEndpoints)

```python
# ListMarketplaceModelEndpointsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_bedrock.paginator import ListMarketplaceModelEndpointsPaginator

session = get_session()
async with session.create_client("bedrock") as client:  # (1)
    paginator: ListMarketplaceModelEndpointsPaginator = client.get_paginator("list_marketplace_model_endpoints")  # (2)
    async for item in paginator.paginate(...):
        item: ListMarketplaceModelEndpointsResponseTypeDef
        print(item)  # (3)
```

1. client: [BedrockClient](./client.md)
2. paginator: [ListMarketplaceModelEndpointsPaginator](./paginators.md#listmarketplacemodelendpointspaginator)
3. item: [:material-code-braces: ListMarketplaceModelEndpointsResponseTypeDef](./type_defs.md#listmarketplacemodelendpointsresponsetypedef) 


### paginate

Type annotations and code completion for `#!python ListMarketplaceModelEndpointsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    modelSourceEquals: str = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AioPageIterator[ListMarketplaceModelEndpointsResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListMarketplaceModelEndpointsResponseTypeDef](./type_defs.md#listmarketplacemodelendpointsresponsetypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: ListMarketplaceModelEndpointsRequestPaginateTypeDef = {  # (1)
    "modelSourceEquals": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListMarketplaceModelEndpointsRequestPaginateTypeDef](./type_defs.md#listmarketplacemodelendpointsrequestpaginatetypedef) 
## ListModelCopyJobsPaginator

Type annotations and code completion for `#!python session.create_client("bedrock").get_paginator("list_model_copy_jobs")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/bedrock/paginator/ListModelCopyJobs.html#Bedrock.Paginator.ListModelCopyJobs)

```python
# ListModelCopyJobsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_bedrock.paginator import ListModelCopyJobsPaginator

session = get_session()
async with session.create_client("bedrock") as client:  # (1)
    paginator: ListModelCopyJobsPaginator = client.get_paginator("list_model_copy_jobs")  # (2)
    async for item in paginator.paginate(...):
        item: ListModelCopyJobsResponseTypeDef
        print(item)  # (3)
```

1. client: [BedrockClient](./client.md)
2. paginator: [ListModelCopyJobsPaginator](./paginators.md#listmodelcopyjobspaginator)
3. item: [:material-code-braces: ListModelCopyJobsResponseTypeDef](./type_defs.md#listmodelcopyjobsresponsetypedef) 


### paginate

Type annotations and code completion for `#!python ListModelCopyJobsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    creationTimeAfter: TimestampTypeDef = ...,
    creationTimeBefore: TimestampTypeDef = ...,
    statusEquals: ModelCopyJobStatusType = ...,  # (1)
    sourceAccountEquals: str = ...,
    sourceModelArnEquals: str = ...,
    targetModelNameContains: str = ...,
    sortBy: SortJobsByType = ...,  # (2)
    sortOrder: SortOrderType = ...,  # (3)
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (4)
) -> AioPageIterator[ListModelCopyJobsResponseTypeDef]:  # (5)
    ...
```

1. See [:material-code-brackets: ModelCopyJobStatusType](./literals.md#modelcopyjobstatustype) 
2. See [:material-code-brackets: SortJobsByType](./literals.md#sortjobsbytype) 
3. See [:material-code-brackets: SortOrderType](./literals.md#sortordertype) 
4. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
5. See [:material-code-braces: ListModelCopyJobsResponseTypeDef](./type_defs.md#listmodelcopyjobsresponsetypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: ListModelCopyJobsRequestPaginateTypeDef = {  # (1)
    "creationTimeAfter": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListModelCopyJobsRequestPaginateTypeDef](./type_defs.md#listmodelcopyjobsrequestpaginatetypedef) 
## ListModelCustomizationJobsPaginator

Type annotations and code completion for `#!python session.create_client("bedrock").get_paginator("list_model_customization_jobs")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/bedrock/paginator/ListModelCustomizationJobs.html#Bedrock.Paginator.ListModelCustomizationJobs)

```python
# ListModelCustomizationJobsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_bedrock.paginator import ListModelCustomizationJobsPaginator

session = get_session()
async with session.create_client("bedrock") as client:  # (1)
    paginator: ListModelCustomizationJobsPaginator = client.get_paginator("list_model_customization_jobs")  # (2)
    async for item in paginator.paginate(...):
        item: ListModelCustomizationJobsResponseTypeDef
        print(item)  # (3)
```

1. client: [BedrockClient](./client.md)
2. paginator: [ListModelCustomizationJobsPaginator](./paginators.md#listmodelcustomizationjobspaginator)
3. item: [:material-code-braces: ListModelCustomizationJobsResponseTypeDef](./type_defs.md#listmodelcustomizationjobsresponsetypedef) 


### paginate

Type annotations and code completion for `#!python ListModelCustomizationJobsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    creationTimeAfter: TimestampTypeDef = ...,
    creationTimeBefore: TimestampTypeDef = ...,
    statusEquals: FineTuningJobStatusType = ...,  # (1)
    nameContains: str = ...,
    sortBy: SortJobsByType = ...,  # (2)
    sortOrder: SortOrderType = ...,  # (3)
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (4)
) -> AioPageIterator[ListModelCustomizationJobsResponseTypeDef]:  # (5)
    ...
```

1. See [:material-code-brackets: FineTuningJobStatusType](./literals.md#finetuningjobstatustype) 
2. See [:material-code-brackets: SortJobsByType](./literals.md#sortjobsbytype) 
3. See [:material-code-brackets: SortOrderType](./literals.md#sortordertype) 
4. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
5. See [:material-code-braces: ListModelCustomizationJobsResponseTypeDef](./type_defs.md#listmodelcustomizationjobsresponsetypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: ListModelCustomizationJobsRequestPaginateTypeDef = {  # (1)
    "creationTimeAfter": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListModelCustomizationJobsRequestPaginateTypeDef](./type_defs.md#listmodelcustomizationjobsrequestpaginatetypedef) 
## ListModelImportJobsPaginator

Type annotations and code completion for `#!python session.create_client("bedrock").get_paginator("list_model_import_jobs")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/bedrock/paginator/ListModelImportJobs.html#Bedrock.Paginator.ListModelImportJobs)

```python
# ListModelImportJobsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_bedrock.paginator import ListModelImportJobsPaginator

session = get_session()
async with session.create_client("bedrock") as client:  # (1)
    paginator: ListModelImportJobsPaginator = client.get_paginator("list_model_import_jobs")  # (2)
    async for item in paginator.paginate(...):
        item: ListModelImportJobsResponseTypeDef
        print(item)  # (3)
```

1. client: [BedrockClient](./client.md)
2. paginator: [ListModelImportJobsPaginator](./paginators.md#listmodelimportjobspaginator)
3. item: [:material-code-braces: ListModelImportJobsResponseTypeDef](./type_defs.md#listmodelimportjobsresponsetypedef) 


### paginate

Type annotations and code completion for `#!python ListModelImportJobsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    creationTimeAfter: TimestampTypeDef = ...,
    creationTimeBefore: TimestampTypeDef = ...,
    statusEquals: ModelImportJobStatusType = ...,  # (1)
    nameContains: str = ...,
    sortBy: SortJobsByType = ...,  # (2)
    sortOrder: SortOrderType = ...,  # (3)
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (4)
) -> AioPageIterator[ListModelImportJobsResponseTypeDef]:  # (5)
    ...
```

1. See [:material-code-brackets: ModelImportJobStatusType](./literals.md#modelimportjobstatustype) 
2. See [:material-code-brackets: SortJobsByType](./literals.md#sortjobsbytype) 
3. See [:material-code-brackets: SortOrderType](./literals.md#sortordertype) 
4. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
5. See [:material-code-braces: ListModelImportJobsResponseTypeDef](./type_defs.md#listmodelimportjobsresponsetypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: ListModelImportJobsRequestPaginateTypeDef = {  # (1)
    "creationTimeAfter": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListModelImportJobsRequestPaginateTypeDef](./type_defs.md#listmodelimportjobsrequestpaginatetypedef) 
## ListModelInvocationJobsPaginator

Type annotations and code completion for `#!python session.create_client("bedrock").get_paginator("list_model_invocation_jobs")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/bedrock/paginator/ListModelInvocationJobs.html#Bedrock.Paginator.ListModelInvocationJobs)

```python
# ListModelInvocationJobsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_bedrock.paginator import ListModelInvocationJobsPaginator

session = get_session()
async with session.create_client("bedrock") as client:  # (1)
    paginator: ListModelInvocationJobsPaginator = client.get_paginator("list_model_invocation_jobs")  # (2)
    async for item in paginator.paginate(...):
        item: ListModelInvocationJobsResponseTypeDef
        print(item)  # (3)
```

1. client: [BedrockClient](./client.md)
2. paginator: [ListModelInvocationJobsPaginator](./paginators.md#listmodelinvocationjobspaginator)
3. item: [:material-code-braces: ListModelInvocationJobsResponseTypeDef](./type_defs.md#listmodelinvocationjobsresponsetypedef) 


### paginate

Type annotations and code completion for `#!python ListModelInvocationJobsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    submitTimeAfter: TimestampTypeDef = ...,
    submitTimeBefore: TimestampTypeDef = ...,
    statusEquals: ModelInvocationJobStatusType = ...,  # (1)
    nameContains: str = ...,
    sortBy: SortJobsByType = ...,  # (2)
    sortOrder: SortOrderType = ...,  # (3)
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (4)
) -> AioPageIterator[ListModelInvocationJobsResponseTypeDef]:  # (5)
    ...
```

1. See [:material-code-brackets: ModelInvocationJobStatusType](./literals.md#modelinvocationjobstatustype) 
2. See [:material-code-brackets: SortJobsByType](./literals.md#sortjobsbytype) 
3. See [:material-code-brackets: SortOrderType](./literals.md#sortordertype) 
4. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
5. See [:material-code-braces: ListModelInvocationJobsResponseTypeDef](./type_defs.md#listmodelinvocationjobsresponsetypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: ListModelInvocationJobsRequestPaginateTypeDef = {  # (1)
    "submitTimeAfter": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListModelInvocationJobsRequestPaginateTypeDef](./type_defs.md#listmodelinvocationjobsrequestpaginatetypedef) 
## ListPromptRoutersPaginator

Type annotations and code completion for `#!python session.create_client("bedrock").get_paginator("list_prompt_routers")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/bedrock/paginator/ListPromptRouters.html#Bedrock.Paginator.ListPromptRouters)

```python
# ListPromptRoutersPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_bedrock.paginator import ListPromptRoutersPaginator

session = get_session()
async with session.create_client("bedrock") as client:  # (1)
    paginator: ListPromptRoutersPaginator = client.get_paginator("list_prompt_routers")  # (2)
    async for item in paginator.paginate(...):
        item: ListPromptRoutersResponseTypeDef
        print(item)  # (3)
```

1. client: [BedrockClient](./client.md)
2. paginator: [ListPromptRoutersPaginator](./paginators.md#listpromptrouterspaginator)
3. item: [:material-code-braces: ListPromptRoutersResponseTypeDef](./type_defs.md#listpromptroutersresponsetypedef) 


### paginate

Type annotations and code completion for `#!python ListPromptRoutersPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AioPageIterator[ListPromptRoutersResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListPromptRoutersResponseTypeDef](./type_defs.md#listpromptroutersresponsetypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: ListPromptRoutersRequestPaginateTypeDef = {  # (1)
    "PaginationConfig": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListPromptRoutersRequestPaginateTypeDef](./type_defs.md#listpromptroutersrequestpaginatetypedef) 
## ListProvisionedModelThroughputsPaginator

Type annotations and code completion for `#!python session.create_client("bedrock").get_paginator("list_provisioned_model_throughputs")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/bedrock/paginator/ListProvisionedModelThroughputs.html#Bedrock.Paginator.ListProvisionedModelThroughputs)

```python
# ListProvisionedModelThroughputsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_bedrock.paginator import ListProvisionedModelThroughputsPaginator

session = get_session()
async with session.create_client("bedrock") as client:  # (1)
    paginator: ListProvisionedModelThroughputsPaginator = client.get_paginator("list_provisioned_model_throughputs")  # (2)
    async for item in paginator.paginate(...):
        item: ListProvisionedModelThroughputsResponseTypeDef
        print(item)  # (3)
```

1. client: [BedrockClient](./client.md)
2. paginator: [ListProvisionedModelThroughputsPaginator](./paginators.md#listprovisionedmodelthroughputspaginator)
3. item: [:material-code-braces: ListProvisionedModelThroughputsResponseTypeDef](./type_defs.md#listprovisionedmodelthroughputsresponsetypedef) 


### paginate

Type annotations and code completion for `#!python ListProvisionedModelThroughputsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    creationTimeAfter: TimestampTypeDef = ...,
    creationTimeBefore: TimestampTypeDef = ...,
    statusEquals: ProvisionedModelStatusType = ...,  # (1)
    modelArnEquals: str = ...,
    nameContains: str = ...,
    sortBy: SortByProvisionedModelsType = ...,  # (2)
    sortOrder: SortOrderType = ...,  # (3)
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (4)
) -> AioPageIterator[ListProvisionedModelThroughputsResponseTypeDef]:  # (5)
    ...
```

1. See [:material-code-brackets: ProvisionedModelStatusType](./literals.md#provisionedmodelstatustype) 
2. See [:material-code-brackets: SortByProvisionedModelsType](./literals.md#sortbyprovisionedmodelstype) 
3. See [:material-code-brackets: SortOrderType](./literals.md#sortordertype) 
4. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
5. See [:material-code-braces: ListProvisionedModelThroughputsResponseTypeDef](./type_defs.md#listprovisionedmodelthroughputsresponsetypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: ListProvisionedModelThroughputsRequestPaginateTypeDef = {  # (1)
    "creationTimeAfter": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListProvisionedModelThroughputsRequestPaginateTypeDef](./type_defs.md#listprovisionedmodelthroughputsrequestpaginatetypedef) 
