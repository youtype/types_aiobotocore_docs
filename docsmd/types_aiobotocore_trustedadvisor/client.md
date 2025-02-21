# TrustedAdvisorPublicAPIClient

> [Index](../README.md) > [TrustedAdvisorPublicAPI](./README.md) > TrustedAdvisorPublicAPIClient

!!! note ""

    Auto-generated documentation for [TrustedAdvisorPublicAPI](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/trustedadvisor.html#trustedadvisorpublicapi)
    type annotations stubs module [types-aiobotocore-trustedadvisor](https://pypi.org/project/types-aiobotocore-trustedadvisor/).

## TrustedAdvisorPublicAPIClient

Type annotations and code completion for `#!python session.create_client("trustedadvisor")`
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/trustedadvisor.html#TrustedAdvisorPublicAPI.Client)

```python
# TrustedAdvisorPublicAPIClient usage example

from aiobotocore.session import get_session
from types_aiobotocore_trustedadvisor.client import TrustedAdvisorPublicAPIClient

session = get_session()
async with session.create_client("trustedadvisor") as client:
    client: TrustedAdvisorPublicAPIClient
```

## Exceptions


`aiobotocore` client exceptions are generated in runtime.
This class provides code completion for `#!python session.create_client("trustedadvisor").exceptions` structure.

```python
# TrustedAdvisorPublicAPIClient.exceptions usage example

async with session.create_client("trustedadvisor") as client:
    try:
        do_something(client)
    except (
            client.AccessDeniedException,
        client.ClientError,
        client.ConflictException,
        client.InternalServerException,
        client.ResourceNotFoundException,
        client.ThrottlingException,
        client.ValidationException,
    ) as e:
        print(e)
```

```python
# TrustedAdvisorPublicAPIClient usage type checking example

from types_aiobotocore_trustedadvisor.client import Exceptions

def handle_error(exc: Exceptions.AccessDeniedException) -> None:
    ...
```


## Methods


### can\_paginate



Type annotations and code completion for `#!python session.create_client("trustedadvisor").can_paginate` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/trustedadvisor/client/can_paginate.html)

```python
# can_paginate method definition

def can_paginate(
    self,
    operation_name: str,
) -> bool:
    ...
```


### generate\_presigned\_url



Type annotations and code completion for `#!python session.create_client("trustedadvisor").generate_presigned_url` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/trustedadvisor/client/generate_presigned_url.html)

```python
# generate_presigned_url method definition

await def generate_presigned_url(
    self,
    ClientMethod: str,
    Params: Mapping[str, Any] = ...,
    ExpiresIn: int = 3600,
    HttpMethod: str = ...,
) -> str:
    ...
```


### batch\_update\_recommendation\_resource\_exclusion

Update one or more exclusion status for a list of recommendation resources.

Type annotations and code completion for `#!python session.create_client("trustedadvisor").batch_update_recommendation_resource_exclusion` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/trustedadvisor/client/batch_update_recommendation_resource_exclusion.html)

```python
# batch_update_recommendation_resource_exclusion method definition

await def batch_update_recommendation_resource_exclusion(
    self,
    *,
    recommendationResourceExclusions: Sequence[RecommendationResourceExclusionTypeDef],  # (1)
) -> BatchUpdateRecommendationResourceExclusionResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: RecommendationResourceExclusionTypeDef](./type_defs.md#recommendationresourceexclusiontypedef) 
2. See [:material-code-braces: BatchUpdateRecommendationResourceExclusionResponseTypeDef](./type_defs.md#batchupdaterecommendationresourceexclusionresponsetypedef) 


```python
# batch_update_recommendation_resource_exclusion method usage example with argument unpacking

kwargs: BatchUpdateRecommendationResourceExclusionRequestTypeDef = {  # (1)
    "recommendationResourceExclusions": ...,
}

parent.batch_update_recommendation_resource_exclusion(**kwargs)
```

1. See [:material-code-braces: BatchUpdateRecommendationResourceExclusionRequestTypeDef](./type_defs.md#batchupdaterecommendationresourceexclusionrequesttypedef) 

### get\_organization\_recommendation

Get a specific recommendation within an AWS Organizations organization.

Type annotations and code completion for `#!python session.create_client("trustedadvisor").get_organization_recommendation` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/trustedadvisor/client/get_organization_recommendation.html)

```python
# get_organization_recommendation method definition

await def get_organization_recommendation(
    self,
    *,
    organizationRecommendationIdentifier: str,
) -> GetOrganizationRecommendationResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetOrganizationRecommendationResponseTypeDef](./type_defs.md#getorganizationrecommendationresponsetypedef) 


```python
# get_organization_recommendation method usage example with argument unpacking

kwargs: GetOrganizationRecommendationRequestTypeDef = {  # (1)
    "organizationRecommendationIdentifier": ...,
}

parent.get_organization_recommendation(**kwargs)
```

1. See [:material-code-braces: GetOrganizationRecommendationRequestTypeDef](./type_defs.md#getorganizationrecommendationrequesttypedef) 

### get\_recommendation

Get a specific Recommendation.

Type annotations and code completion for `#!python session.create_client("trustedadvisor").get_recommendation` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/trustedadvisor/client/get_recommendation.html)

```python
# get_recommendation method definition

await def get_recommendation(
    self,
    *,
    recommendationIdentifier: str,
) -> GetRecommendationResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetRecommendationResponseTypeDef](./type_defs.md#getrecommendationresponsetypedef) 


```python
# get_recommendation method usage example with argument unpacking

kwargs: GetRecommendationRequestTypeDef = {  # (1)
    "recommendationIdentifier": ...,
}

parent.get_recommendation(**kwargs)
```

1. See [:material-code-braces: GetRecommendationRequestTypeDef](./type_defs.md#getrecommendationrequesttypedef) 

### list\_checks

List a filterable set of Checks.

Type annotations and code completion for `#!python session.create_client("trustedadvisor").list_checks` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/trustedadvisor/client/list_checks.html)

```python
# list_checks method definition

await def list_checks(
    self,
    *,
    awsService: str = ...,
    language: RecommendationLanguageType = ...,  # (1)
    maxResults: int = ...,
    nextToken: str = ...,
    pillar: RecommendationPillarType = ...,  # (2)
    source: RecommendationSourceType = ...,  # (3)
) -> ListChecksResponseTypeDef:  # (4)
    ...
```

1. See [:material-code-brackets: RecommendationLanguageType](./literals.md#recommendationlanguagetype) 
2. See [:material-code-brackets: RecommendationPillarType](./literals.md#recommendationpillartype) 
3. See [:material-code-brackets: RecommendationSourceType](./literals.md#recommendationsourcetype) 
4. See [:material-code-braces: ListChecksResponseTypeDef](./type_defs.md#listchecksresponsetypedef) 


```python
# list_checks method usage example with argument unpacking

kwargs: ListChecksRequestTypeDef = {  # (1)
    "awsService": ...,
}

parent.list_checks(**kwargs)
```

1. See [:material-code-braces: ListChecksRequestTypeDef](./type_defs.md#listchecksrequesttypedef) 

### list\_organization\_recommendation\_accounts

Lists the accounts that own the resources for an organization aggregate
recommendation.

Type annotations and code completion for `#!python session.create_client("trustedadvisor").list_organization_recommendation_accounts` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/trustedadvisor/client/list_organization_recommendation_accounts.html)

```python
# list_organization_recommendation_accounts method definition

await def list_organization_recommendation_accounts(
    self,
    *,
    organizationRecommendationIdentifier: str,
    affectedAccountId: str = ...,
    maxResults: int = ...,
    nextToken: str = ...,
) -> ListOrganizationRecommendationAccountsResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListOrganizationRecommendationAccountsResponseTypeDef](./type_defs.md#listorganizationrecommendationaccountsresponsetypedef) 


```python
# list_organization_recommendation_accounts method usage example with argument unpacking

kwargs: ListOrganizationRecommendationAccountsRequestTypeDef = {  # (1)
    "organizationRecommendationIdentifier": ...,
}

parent.list_organization_recommendation_accounts(**kwargs)
```

1. See [:material-code-braces: ListOrganizationRecommendationAccountsRequestTypeDef](./type_defs.md#listorganizationrecommendationaccountsrequesttypedef) 

### list\_organization\_recommendation\_resources

List Resources of a Recommendation within an Organization.

Type annotations and code completion for `#!python session.create_client("trustedadvisor").list_organization_recommendation_resources` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/trustedadvisor/client/list_organization_recommendation_resources.html)

```python
# list_organization_recommendation_resources method definition

await def list_organization_recommendation_resources(
    self,
    *,
    organizationRecommendationIdentifier: str,
    affectedAccountId: str = ...,
    exclusionStatus: ExclusionStatusType = ...,  # (1)
    maxResults: int = ...,
    nextToken: str = ...,
    regionCode: str = ...,
    status: ResourceStatusType = ...,  # (2)
) -> ListOrganizationRecommendationResourcesResponseTypeDef:  # (3)
    ...
```

1. See [:material-code-brackets: ExclusionStatusType](./literals.md#exclusionstatustype) 
2. See [:material-code-brackets: ResourceStatusType](./literals.md#resourcestatustype) 
3. See [:material-code-braces: ListOrganizationRecommendationResourcesResponseTypeDef](./type_defs.md#listorganizationrecommendationresourcesresponsetypedef) 


```python
# list_organization_recommendation_resources method usage example with argument unpacking

kwargs: ListOrganizationRecommendationResourcesRequestTypeDef = {  # (1)
    "organizationRecommendationIdentifier": ...,
}

parent.list_organization_recommendation_resources(**kwargs)
```

1. See [:material-code-braces: ListOrganizationRecommendationResourcesRequestTypeDef](./type_defs.md#listorganizationrecommendationresourcesrequesttypedef) 

### list\_organization\_recommendations

List a filterable set of Recommendations within an Organization.

Type annotations and code completion for `#!python session.create_client("trustedadvisor").list_organization_recommendations` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/trustedadvisor/client/list_organization_recommendations.html)

```python
# list_organization_recommendations method definition

await def list_organization_recommendations(
    self,
    *,
    afterLastUpdatedAt: TimestampTypeDef = ...,
    awsService: str = ...,
    beforeLastUpdatedAt: TimestampTypeDef = ...,
    checkIdentifier: str = ...,
    maxResults: int = ...,
    nextToken: str = ...,
    pillar: RecommendationPillarType = ...,  # (1)
    source: RecommendationSourceType = ...,  # (2)
    status: RecommendationStatusType = ...,  # (3)
    type: RecommendationTypeType = ...,  # (4)
) -> ListOrganizationRecommendationsResponseTypeDef:  # (5)
    ...
```

1. See [:material-code-brackets: RecommendationPillarType](./literals.md#recommendationpillartype) 
2. See [:material-code-brackets: RecommendationSourceType](./literals.md#recommendationsourcetype) 
3. See [:material-code-brackets: RecommendationStatusType](./literals.md#recommendationstatustype) 
4. See [:material-code-brackets: RecommendationTypeType](./literals.md#recommendationtypetype) 
5. See [:material-code-braces: ListOrganizationRecommendationsResponseTypeDef](./type_defs.md#listorganizationrecommendationsresponsetypedef) 


```python
# list_organization_recommendations method usage example with argument unpacking

kwargs: ListOrganizationRecommendationsRequestTypeDef = {  # (1)
    "afterLastUpdatedAt": ...,
}

parent.list_organization_recommendations(**kwargs)
```

1. See [:material-code-braces: ListOrganizationRecommendationsRequestTypeDef](./type_defs.md#listorganizationrecommendationsrequesttypedef) 

### list\_recommendation\_resources

List Resources of a Recommendation.

Type annotations and code completion for `#!python session.create_client("trustedadvisor").list_recommendation_resources` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/trustedadvisor/client/list_recommendation_resources.html)

```python
# list_recommendation_resources method definition

await def list_recommendation_resources(
    self,
    *,
    recommendationIdentifier: str,
    exclusionStatus: ExclusionStatusType = ...,  # (1)
    maxResults: int = ...,
    nextToken: str = ...,
    regionCode: str = ...,
    status: ResourceStatusType = ...,  # (2)
) -> ListRecommendationResourcesResponseTypeDef:  # (3)
    ...
```

1. See [:material-code-brackets: ExclusionStatusType](./literals.md#exclusionstatustype) 
2. See [:material-code-brackets: ResourceStatusType](./literals.md#resourcestatustype) 
3. See [:material-code-braces: ListRecommendationResourcesResponseTypeDef](./type_defs.md#listrecommendationresourcesresponsetypedef) 


```python
# list_recommendation_resources method usage example with argument unpacking

kwargs: ListRecommendationResourcesRequestTypeDef = {  # (1)
    "recommendationIdentifier": ...,
}

parent.list_recommendation_resources(**kwargs)
```

1. See [:material-code-braces: ListRecommendationResourcesRequestTypeDef](./type_defs.md#listrecommendationresourcesrequesttypedef) 

### list\_recommendations

List a filterable set of Recommendations.

Type annotations and code completion for `#!python session.create_client("trustedadvisor").list_recommendations` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/trustedadvisor/client/list_recommendations.html)

```python
# list_recommendations method definition

await def list_recommendations(
    self,
    *,
    afterLastUpdatedAt: TimestampTypeDef = ...,
    awsService: str = ...,
    beforeLastUpdatedAt: TimestampTypeDef = ...,
    checkIdentifier: str = ...,
    maxResults: int = ...,
    nextToken: str = ...,
    pillar: RecommendationPillarType = ...,  # (1)
    source: RecommendationSourceType = ...,  # (2)
    status: RecommendationStatusType = ...,  # (3)
    type: RecommendationTypeType = ...,  # (4)
) -> ListRecommendationsResponseTypeDef:  # (5)
    ...
```

1. See [:material-code-brackets: RecommendationPillarType](./literals.md#recommendationpillartype) 
2. See [:material-code-brackets: RecommendationSourceType](./literals.md#recommendationsourcetype) 
3. See [:material-code-brackets: RecommendationStatusType](./literals.md#recommendationstatustype) 
4. See [:material-code-brackets: RecommendationTypeType](./literals.md#recommendationtypetype) 
5. See [:material-code-braces: ListRecommendationsResponseTypeDef](./type_defs.md#listrecommendationsresponsetypedef) 


```python
# list_recommendations method usage example with argument unpacking

kwargs: ListRecommendationsRequestTypeDef = {  # (1)
    "afterLastUpdatedAt": ...,
}

parent.list_recommendations(**kwargs)
```

1. See [:material-code-braces: ListRecommendationsRequestTypeDef](./type_defs.md#listrecommendationsrequesttypedef) 

### update\_organization\_recommendation\_lifecycle

Update the lifecycle of a Recommendation within an Organization.

Type annotations and code completion for `#!python session.create_client("trustedadvisor").update_organization_recommendation_lifecycle` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/trustedadvisor/client/update_organization_recommendation_lifecycle.html)

```python
# update_organization_recommendation_lifecycle method definition

await def update_organization_recommendation_lifecycle(
    self,
    *,
    lifecycleStage: UpdateRecommendationLifecycleStageType,  # (1)
    organizationRecommendationIdentifier: str,
    updateReason: str = ...,
    updateReasonCode: UpdateRecommendationLifecycleStageReasonCodeType = ...,  # (2)
) -> EmptyResponseMetadataTypeDef:  # (3)
    ...
```

1. See [:material-code-brackets: UpdateRecommendationLifecycleStageType](./literals.md#updaterecommendationlifecyclestagetype) 
2. See [:material-code-brackets: UpdateRecommendationLifecycleStageReasonCodeType](./literals.md#updaterecommendationlifecyclestagereasoncodetype) 
3. See [:material-code-braces: EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef) 


```python
# update_organization_recommendation_lifecycle method usage example with argument unpacking

kwargs: UpdateOrganizationRecommendationLifecycleRequestTypeDef = {  # (1)
    "lifecycleStage": ...,
    "organizationRecommendationIdentifier": ...,
}

parent.update_organization_recommendation_lifecycle(**kwargs)
```

1. See [:material-code-braces: UpdateOrganizationRecommendationLifecycleRequestTypeDef](./type_defs.md#updateorganizationrecommendationlifecyclerequesttypedef) 

### update\_recommendation\_lifecycle

Update the lifecyle of a Recommendation.

Type annotations and code completion for `#!python session.create_client("trustedadvisor").update_recommendation_lifecycle` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/trustedadvisor/client/update_recommendation_lifecycle.html)

```python
# update_recommendation_lifecycle method definition

await def update_recommendation_lifecycle(
    self,
    *,
    lifecycleStage: UpdateRecommendationLifecycleStageType,  # (1)
    recommendationIdentifier: str,
    updateReason: str = ...,
    updateReasonCode: UpdateRecommendationLifecycleStageReasonCodeType = ...,  # (2)
) -> EmptyResponseMetadataTypeDef:  # (3)
    ...
```

1. See [:material-code-brackets: UpdateRecommendationLifecycleStageType](./literals.md#updaterecommendationlifecyclestagetype) 
2. See [:material-code-brackets: UpdateRecommendationLifecycleStageReasonCodeType](./literals.md#updaterecommendationlifecyclestagereasoncodetype) 
3. See [:material-code-braces: EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef) 


```python
# update_recommendation_lifecycle method usage example with argument unpacking

kwargs: UpdateRecommendationLifecycleRequestTypeDef = {  # (1)
    "lifecycleStage": ...,
    "recommendationIdentifier": ...,
}

parent.update_recommendation_lifecycle(**kwargs)
```

1. See [:material-code-braces: UpdateRecommendationLifecycleRequestTypeDef](./type_defs.md#updaterecommendationlifecyclerequesttypedef) 

### \_\_aenter\_\_



Type annotations and code completion for `#!python session.create_client("trustedadvisor").__aenter__` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/trustedadvisor.html#TrustedAdvisorPublicAPI.Client)

```python
# __aenter__ method definition

await def __aenter__(
    self,
) -> Self:
    ...
```


### \_\_aexit\_\_



Type annotations and code completion for `#!python session.create_client("trustedadvisor").__aexit__` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/trustedadvisor.html#TrustedAdvisorPublicAPI.Client)

```python
# __aexit__ method definition

await def __aexit__(
    self,
    exc_type: Union[Type[BaseException], None],
    exc_val: Union[BaseException, None],
    exc_tb: Union[TracebackType, None],
) -> None:
    ...
```




### get_paginator

Type annotations and code completion for `#!python session.create_client("trustedadvisor").get_paginator` method with overloads.

- `client.get_paginator("list_checks")` -> [ListChecksPaginator](./paginators.md#listcheckspaginator)
- `client.get_paginator("list_organization_recommendation_accounts")` -> [ListOrganizationRecommendationAccountsPaginator](./paginators.md#listorganizationrecommendationaccountspaginator)
- `client.get_paginator("list_organization_recommendation_resources")` -> [ListOrganizationRecommendationResourcesPaginator](./paginators.md#listorganizationrecommendationresourcespaginator)
- `client.get_paginator("list_organization_recommendations")` -> [ListOrganizationRecommendationsPaginator](./paginators.md#listorganizationrecommendationspaginator)
- `client.get_paginator("list_recommendation_resources")` -> [ListRecommendationResourcesPaginator](./paginators.md#listrecommendationresourcespaginator)
- `client.get_paginator("list_recommendations")` -> [ListRecommendationsPaginator](./paginators.md#listrecommendationspaginator)



