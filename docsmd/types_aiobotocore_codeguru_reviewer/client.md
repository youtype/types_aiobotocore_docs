# CodeGuruReviewerClient

> [Index](../README.md) > [CodeGuruReviewer](./README.md) > CodeGuruReviewerClient

!!! note ""

    Auto-generated documentation for [CodeGuruReviewer](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codeguru-reviewer.html#CodeGuruReviewer)
    type annotations stubs module [types-aiobotocore-codeguru-reviewer](https://pypi.org/project/types-aiobotocore-codeguru-reviewer/).

## CodeGuruReviewerClient

Type annotations and code completion for `#!python session.create_client("codeguru-reviewer")`
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codeguru-reviewer.html#CodeGuruReviewer.Client)

```python
# CodeGuruReviewerClient usage example

from aiobotocore.session import get_session
from types_aiobotocore_codeguru_reviewer.client import CodeGuruReviewerClient

session = get_session()
async with session.create_client("codeguru-reviewer") as client:
    client: CodeGuruReviewerClient
```

## Exceptions


`aiobotocore` client exceptions are generated in runtime.
This class provides code completion for `#!python session.create_client("codeguru-reviewer").exceptions` structure.

```python
# CodeGuruReviewerClient.exceptions usage example

async with session.create_client("codeguru-reviewer") as client:
    try:
        do_something(client)
    except (
            client.AccessDeniedException,
        client.ClientError,
        client.ConflictException,
        client.InternalServerException,
        client.NotFoundException,
        client.ResourceNotFoundException,
        client.ThrottlingException,
        client.ValidationException,
    ) as e:
        print(e)
```

```python
# CodeGuruReviewerClient usage type checking example

from types_aiobotocore_codeguru_reviewer.client import Exceptions

def handle_error(exc: Exceptions.AccessDeniedException) -> None:
    ...
```


## Methods


### associate\_repository

Use to associate an Amazon Web Services CodeCommit repository or a repository
managed by Amazon Web Services CodeStar Connections with Amazon CodeGuru
Reviewer.

Type annotations and code completion for `#!python session.create_client("codeguru-reviewer").associate_repository` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codeguru-reviewer.html#CodeGuruReviewer.Client.associate_repository)

```python
# associate_repository method definition

await def associate_repository(
    self,
    *,
    Repository: RepositoryTypeDef,  # (1)
    ClientRequestToken: str = ...,
    Tags: Mapping[str, str] = ...,
    KMSKeyDetails: KMSKeyDetailsTypeDef = ...,  # (2)
) -> AssociateRepositoryResponseTypeDef:  # (3)
    ...
```

1. See [:material-code-braces: RepositoryTypeDef](./type_defs.md#repositorytypedef) 
2. See [:material-code-braces: KMSKeyDetailsTypeDef](./type_defs.md#kmskeydetailstypedef) 
3. See [:material-code-braces: AssociateRepositoryResponseTypeDef](./type_defs.md#associaterepositoryresponsetypedef) 


```python
# associate_repository method usage example with argument unpacking

kwargs: AssociateRepositoryRequestRequestTypeDef = {  # (1)
    "Repository": ...,
}

parent.associate_repository(**kwargs)
```

1. See [:material-code-braces: AssociateRepositoryRequestRequestTypeDef](./type_defs.md#associaterepositoryrequestrequesttypedef) 

### can\_paginate

Check if an operation can be paginated.

Type annotations and code completion for `#!python session.create_client("codeguru-reviewer").can_paginate` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codeguru-reviewer.html#CodeGuruReviewer.Client.can_paginate)

```python
# can_paginate method definition

def can_paginate(
    self,
    operation_name: str,
) -> bool:
    ...
```


### close

Closes underlying endpoint connections.

Type annotations and code completion for `#!python session.create_client("codeguru-reviewer").close` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codeguru-reviewer.html#CodeGuruReviewer.Client.close)

```python
# close method definition

await def close(
    self,
) -> None:
    ...
```


### create\_code\_review

Use to create a code review with a
[CodeReviewType](https://docs.aws.amazon.com/codeguru/latest/reviewer-api/API_CodeReviewType.html)
of
`RepositoryAnalysis`.

Type annotations and code completion for `#!python session.create_client("codeguru-reviewer").create_code_review` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codeguru-reviewer.html#CodeGuruReviewer.Client.create_code_review)

```python
# create_code_review method definition

await def create_code_review(
    self,
    *,
    Name: str,
    RepositoryAssociationArn: str,
    Type: CodeReviewTypeTypeDef,  # (1)
    ClientRequestToken: str = ...,
) -> CreateCodeReviewResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: CodeReviewTypeTypeDef](./type_defs.md#codereviewtypetypedef) 
2. See [:material-code-braces: CreateCodeReviewResponseTypeDef](./type_defs.md#createcodereviewresponsetypedef) 


```python
# create_code_review method usage example with argument unpacking

kwargs: CreateCodeReviewRequestRequestTypeDef = {  # (1)
    "Name": ...,
    "RepositoryAssociationArn": ...,
    "Type": ...,
}

parent.create_code_review(**kwargs)
```

1. See [:material-code-braces: CreateCodeReviewRequestRequestTypeDef](./type_defs.md#createcodereviewrequestrequesttypedef) 

### describe\_code\_review

Returns the metadata associated with the code review along with its status.

Type annotations and code completion for `#!python session.create_client("codeguru-reviewer").describe_code_review` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codeguru-reviewer.html#CodeGuruReviewer.Client.describe_code_review)

```python
# describe_code_review method definition

await def describe_code_review(
    self,
    *,
    CodeReviewArn: str,
) -> DescribeCodeReviewResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DescribeCodeReviewResponseTypeDef](./type_defs.md#describecodereviewresponsetypedef) 


```python
# describe_code_review method usage example with argument unpacking

kwargs: DescribeCodeReviewRequestRequestTypeDef = {  # (1)
    "CodeReviewArn": ...,
}

parent.describe_code_review(**kwargs)
```

1. See [:material-code-braces: DescribeCodeReviewRequestRequestTypeDef](./type_defs.md#describecodereviewrequestrequesttypedef) 

### describe\_recommendation\_feedback

Describes the customer feedback for a CodeGuru Reviewer recommendation.

Type annotations and code completion for `#!python session.create_client("codeguru-reviewer").describe_recommendation_feedback` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codeguru-reviewer.html#CodeGuruReviewer.Client.describe_recommendation_feedback)

```python
# describe_recommendation_feedback method definition

await def describe_recommendation_feedback(
    self,
    *,
    CodeReviewArn: str,
    RecommendationId: str,
    UserId: str = ...,
) -> DescribeRecommendationFeedbackResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DescribeRecommendationFeedbackResponseTypeDef](./type_defs.md#describerecommendationfeedbackresponsetypedef) 


```python
# describe_recommendation_feedback method usage example with argument unpacking

kwargs: DescribeRecommendationFeedbackRequestRequestTypeDef = {  # (1)
    "CodeReviewArn": ...,
    "RecommendationId": ...,
}

parent.describe_recommendation_feedback(**kwargs)
```

1. See [:material-code-braces: DescribeRecommendationFeedbackRequestRequestTypeDef](./type_defs.md#describerecommendationfeedbackrequestrequesttypedef) 

### describe\_repository\_association

Returns a
[RepositoryAssociation](https://docs.aws.amazon.com/codeguru/latest/reviewer-api/API_RepositoryAssociation.html)
object that contains information about the requested repository
association.

Type annotations and code completion for `#!python session.create_client("codeguru-reviewer").describe_repository_association` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codeguru-reviewer.html#CodeGuruReviewer.Client.describe_repository_association)

```python
# describe_repository_association method definition

await def describe_repository_association(
    self,
    *,
    AssociationArn: str,
) -> DescribeRepositoryAssociationResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DescribeRepositoryAssociationResponseTypeDef](./type_defs.md#describerepositoryassociationresponsetypedef) 


```python
# describe_repository_association method usage example with argument unpacking

kwargs: DescribeRepositoryAssociationRequestRequestTypeDef = {  # (1)
    "AssociationArn": ...,
}

parent.describe_repository_association(**kwargs)
```

1. See [:material-code-braces: DescribeRepositoryAssociationRequestRequestTypeDef](./type_defs.md#describerepositoryassociationrequestrequesttypedef) 

### disassociate\_repository

Removes the association between Amazon CodeGuru Reviewer and a repository.

Type annotations and code completion for `#!python session.create_client("codeguru-reviewer").disassociate_repository` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codeguru-reviewer.html#CodeGuruReviewer.Client.disassociate_repository)

```python
# disassociate_repository method definition

await def disassociate_repository(
    self,
    *,
    AssociationArn: str,
) -> DisassociateRepositoryResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DisassociateRepositoryResponseTypeDef](./type_defs.md#disassociaterepositoryresponsetypedef) 


```python
# disassociate_repository method usage example with argument unpacking

kwargs: DisassociateRepositoryRequestRequestTypeDef = {  # (1)
    "AssociationArn": ...,
}

parent.disassociate_repository(**kwargs)
```

1. See [:material-code-braces: DisassociateRepositoryRequestRequestTypeDef](./type_defs.md#disassociaterepositoryrequestrequesttypedef) 

### generate\_presigned\_url

Generate a presigned url given a client, its method, and arguments.

Type annotations and code completion for `#!python session.create_client("codeguru-reviewer").generate_presigned_url` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codeguru-reviewer.html#CodeGuruReviewer.Client.generate_presigned_url)

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


### list\_code\_reviews

Lists all the code reviews that the customer has created in the past 90 days.

Type annotations and code completion for `#!python session.create_client("codeguru-reviewer").list_code_reviews` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codeguru-reviewer.html#CodeGuruReviewer.Client.list_code_reviews)

```python
# list_code_reviews method definition

await def list_code_reviews(
    self,
    *,
    Type: TypeType,  # (1)
    ProviderTypes: Sequence[ProviderTypeType] = ...,  # (2)
    States: Sequence[JobStateType] = ...,  # (3)
    RepositoryNames: Sequence[str] = ...,
    MaxResults: int = ...,
    NextToken: str = ...,
) -> ListCodeReviewsResponseTypeDef:  # (4)
    ...
```

1. See [:material-code-brackets: TypeType](./literals.md#typetype) 
2. See [:material-code-brackets: ProviderTypeType](./literals.md#providertypetype) 
3. See [:material-code-brackets: JobStateType](./literals.md#jobstatetype) 
4. See [:material-code-braces: ListCodeReviewsResponseTypeDef](./type_defs.md#listcodereviewsresponsetypedef) 


```python
# list_code_reviews method usage example with argument unpacking

kwargs: ListCodeReviewsRequestRequestTypeDef = {  # (1)
    "Type": ...,
}

parent.list_code_reviews(**kwargs)
```

1. See [:material-code-braces: ListCodeReviewsRequestRequestTypeDef](./type_defs.md#listcodereviewsrequestrequesttypedef) 

### list\_recommendation\_feedback

Returns a list of
[RecommendationFeedbackSummary](https://docs.aws.amazon.com/codeguru/latest/reviewer-api/API_RecommendationFeedbackSummary.html)
objects that contain customer recommendation feedback for all CodeGuru Reviewer
users.

Type annotations and code completion for `#!python session.create_client("codeguru-reviewer").list_recommendation_feedback` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codeguru-reviewer.html#CodeGuruReviewer.Client.list_recommendation_feedback)

```python
# list_recommendation_feedback method definition

await def list_recommendation_feedback(
    self,
    *,
    CodeReviewArn: str,
    NextToken: str = ...,
    MaxResults: int = ...,
    UserIds: Sequence[str] = ...,
    RecommendationIds: Sequence[str] = ...,
) -> ListRecommendationFeedbackResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListRecommendationFeedbackResponseTypeDef](./type_defs.md#listrecommendationfeedbackresponsetypedef) 


```python
# list_recommendation_feedback method usage example with argument unpacking

kwargs: ListRecommendationFeedbackRequestRequestTypeDef = {  # (1)
    "CodeReviewArn": ...,
}

parent.list_recommendation_feedback(**kwargs)
```

1. See [:material-code-braces: ListRecommendationFeedbackRequestRequestTypeDef](./type_defs.md#listrecommendationfeedbackrequestrequesttypedef) 

### list\_recommendations

Returns the list of all recommendations for a completed code review.

Type annotations and code completion for `#!python session.create_client("codeguru-reviewer").list_recommendations` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codeguru-reviewer.html#CodeGuruReviewer.Client.list_recommendations)

```python
# list_recommendations method definition

await def list_recommendations(
    self,
    *,
    CodeReviewArn: str,
    NextToken: str = ...,
    MaxResults: int = ...,
) -> ListRecommendationsResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListRecommendationsResponseTypeDef](./type_defs.md#listrecommendationsresponsetypedef) 


```python
# list_recommendations method usage example with argument unpacking

kwargs: ListRecommendationsRequestRequestTypeDef = {  # (1)
    "CodeReviewArn": ...,
}

parent.list_recommendations(**kwargs)
```

1. See [:material-code-braces: ListRecommendationsRequestRequestTypeDef](./type_defs.md#listrecommendationsrequestrequesttypedef) 

### list\_repository\_associations

Returns a list of
[RepositoryAssociationSummary](https://docs.aws.amazon.com/codeguru/latest/reviewer-api/API_RepositoryAssociationSummary.html)
objects that contain summary information about a repository
association.

Type annotations and code completion for `#!python session.create_client("codeguru-reviewer").list_repository_associations` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codeguru-reviewer.html#CodeGuruReviewer.Client.list_repository_associations)

```python
# list_repository_associations method definition

await def list_repository_associations(
    self,
    *,
    ProviderTypes: Sequence[ProviderTypeType] = ...,  # (1)
    States: Sequence[RepositoryAssociationStateType] = ...,  # (2)
    Names: Sequence[str] = ...,
    Owners: Sequence[str] = ...,
    MaxResults: int = ...,
    NextToken: str = ...,
) -> ListRepositoryAssociationsResponseTypeDef:  # (3)
    ...
```

1. See [:material-code-brackets: ProviderTypeType](./literals.md#providertypetype) 
2. See [:material-code-brackets: RepositoryAssociationStateType](./literals.md#repositoryassociationstatetype) 
3. See [:material-code-braces: ListRepositoryAssociationsResponseTypeDef](./type_defs.md#listrepositoryassociationsresponsetypedef) 


```python
# list_repository_associations method usage example with argument unpacking

kwargs: ListRepositoryAssociationsRequestRequestTypeDef = {  # (1)
    "ProviderTypes": ...,
}

parent.list_repository_associations(**kwargs)
```

1. See [:material-code-braces: ListRepositoryAssociationsRequestRequestTypeDef](./type_defs.md#listrepositoryassociationsrequestrequesttypedef) 

### list\_tags\_for\_resource

Returns the list of tags associated with an associated repository resource.

Type annotations and code completion for `#!python session.create_client("codeguru-reviewer").list_tags_for_resource` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codeguru-reviewer.html#CodeGuruReviewer.Client.list_tags_for_resource)

```python
# list_tags_for_resource method definition

await def list_tags_for_resource(
    self,
    *,
    resourceArn: str,
) -> ListTagsForResourceResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListTagsForResourceResponseTypeDef](./type_defs.md#listtagsforresourceresponsetypedef) 


```python
# list_tags_for_resource method usage example with argument unpacking

kwargs: ListTagsForResourceRequestRequestTypeDef = {  # (1)
    "resourceArn": ...,
}

parent.list_tags_for_resource(**kwargs)
```

1. See [:material-code-braces: ListTagsForResourceRequestRequestTypeDef](./type_defs.md#listtagsforresourcerequestrequesttypedef) 

### put\_recommendation\_feedback

Stores customer feedback for a CodeGuru Reviewer recommendation.

Type annotations and code completion for `#!python session.create_client("codeguru-reviewer").put_recommendation_feedback` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codeguru-reviewer.html#CodeGuruReviewer.Client.put_recommendation_feedback)

```python
# put_recommendation_feedback method definition

await def put_recommendation_feedback(
    self,
    *,
    CodeReviewArn: str,
    RecommendationId: str,
    Reactions: Sequence[ReactionType],  # (1)
) -> Dict[str, Any]:
    ...
```

1. See [:material-code-brackets: ReactionType](./literals.md#reactiontype) 


```python
# put_recommendation_feedback method usage example with argument unpacking

kwargs: PutRecommendationFeedbackRequestRequestTypeDef = {  # (1)
    "CodeReviewArn": ...,
    "RecommendationId": ...,
    "Reactions": ...,
}

parent.put_recommendation_feedback(**kwargs)
```

1. See [:material-code-braces: PutRecommendationFeedbackRequestRequestTypeDef](./type_defs.md#putrecommendationfeedbackrequestrequesttypedef) 

### tag\_resource

Adds one or more tags to an associated repository.

Type annotations and code completion for `#!python session.create_client("codeguru-reviewer").tag_resource` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codeguru-reviewer.html#CodeGuruReviewer.Client.tag_resource)

```python
# tag_resource method definition

await def tag_resource(
    self,
    *,
    resourceArn: str,
    Tags: Mapping[str, str],
) -> Dict[str, Any]:
    ...
```



```python
# tag_resource method usage example with argument unpacking

kwargs: TagResourceRequestRequestTypeDef = {  # (1)
    "resourceArn": ...,
    "Tags": ...,
}

parent.tag_resource(**kwargs)
```

1. See [:material-code-braces: TagResourceRequestRequestTypeDef](./type_defs.md#tagresourcerequestrequesttypedef) 

### untag\_resource

Removes a tag from an associated repository.

Type annotations and code completion for `#!python session.create_client("codeguru-reviewer").untag_resource` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codeguru-reviewer.html#CodeGuruReviewer.Client.untag_resource)

```python
# untag_resource method definition

await def untag_resource(
    self,
    *,
    resourceArn: str,
    TagKeys: Sequence[str],
) -> Dict[str, Any]:
    ...
```



```python
# untag_resource method usage example with argument unpacking

kwargs: UntagResourceRequestRequestTypeDef = {  # (1)
    "resourceArn": ...,
    "TagKeys": ...,
}

parent.untag_resource(**kwargs)
```

1. See [:material-code-braces: UntagResourceRequestRequestTypeDef](./type_defs.md#untagresourcerequestrequesttypedef) 

### \_\_aenter\_\_



Type annotations and code completion for `#!python session.create_client("codeguru-reviewer").__aenter__` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codeguru-reviewer.html#CodeGuruReviewer.Client.__aenter__)

```python
# __aenter__ method definition

await def __aenter__(
    self,
) -> "CodeGuruReviewerClient":
    ...
```


### \_\_aexit\_\_



Type annotations and code completion for `#!python session.create_client("codeguru-reviewer").__aexit__` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codeguru-reviewer.html#CodeGuruReviewer.Client.__aexit__)

```python
# __aexit__ method definition

await def __aexit__(
    self,
    exc_type: Any,
    exc_val: Any,
    exc_tb: Any,
) -> Any:
    ...
```




### get_paginator

Type annotations and code completion for `#!python session.create_client("codeguru-reviewer").get_paginator` method with overloads.

- `client.get_paginator("list_repository_associations")` -> [ListRepositoryAssociationsPaginator](./paginators.md#listrepositoryassociationspaginator)




### get_waiter

Type annotations and code completion for `#!python session.create_client("codeguru-reviewer").get_waiter` method with overloads.

- `client.get_waiter("code_review_completed")` -> [CodeReviewCompletedWaiter](./waiters.md#codereviewcompletedwaiter)
- `client.get_waiter("repository_association_succeeded")` -> [RepositoryAssociationSucceededWaiter](./waiters.md#repositoryassociationsucceededwaiter)

