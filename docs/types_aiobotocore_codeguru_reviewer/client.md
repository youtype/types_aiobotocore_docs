<a id="codegurureviewerclient-for-aiobotocore-codegurureviewer-module"></a>

# CodeGuruReviewerClient for aiobotocore CodeGuruReviewer module

> [Index](../README.md) > [CodeGuruReviewer](./README.md) >
> CodeGuruReviewerClient

Auto-generated documentation for
[CodeGuruReviewer](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codeguru-reviewer.html#CodeGuruReviewer)
type annotations stubs module
[types-aiobotocore-codeguru-reviewer](https://pypi.org/project/types-aiobotocore-codeguru-reviewer/).

- [CodeGuruReviewerClient for aiobotocore CodeGuruReviewer module](#codegurureviewerclient-for-aiobotocore-codegurureviewer-module)
  - [CodeGuruReviewerClient](#codegurureviewerclient)
  - [Exceptions](#exceptions)
  - [Methods](#methods)
    - [exceptions](#exceptions)
    - [associate_repository](#associate_repository)
    - [can_paginate](#can_paginate)
    - [create_code_review](#create_code_review)
    - [describe_code_review](#describe_code_review)
    - [describe_recommendation_feedback](#describe_recommendation_feedback)
    - [describe_repository_association](#describe_repository_association)
    - [disassociate_repository](#disassociate_repository)
    - [generate_presigned_url](#generate_presigned_url)
    - [list_code_reviews](#list_code_reviews)
    - [list_recommendation_feedback](#list_recommendation_feedback)
    - [list_recommendations](#list_recommendations)
    - [list_repository_associations](#list_repository_associations)
    - [list_tags_for_resource](#list_tags_for_resource)
    - [put_recommendation_feedback](#put_recommendation_feedback)
    - [tag_resource](#tag_resource)
    - [untag_resource](#untag_resource)
    - [\_\_aenter\_\_](#__aenter__)
    - [\_\_aexit\_\_](#__aexit__)
    - [get_paginator](#get_paginator)
    - [get_waiter](#get_waiter)

<a id="codegurureviewerclient"></a>

## CodeGuruReviewerClient

Type annotations for `session.create_client("codeguru-reviewer")`

Can be used directly:

```python
from aiobotocore.session import get_session
from types_aiobotocore_codeguru_reviewer.client import CodeGuruReviewerClient

session = get_session()
async with session.create_client("codeguru-reviewer") as client:
    client: CodeGuruReviewerClient
```

Boto3 documentation:
[CodeGuruReviewer.Client](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codeguru-reviewer.html#CodeGuruReviewer.Client)

<a id="exceptions"></a>

## Exceptions

`boto3` client exceptions are generated in runtime. This class can be used for
static analysis directly:

```python
from types_aiobotocore_codeguru_reviewer.client import Exceptions

def handle_error(exc: Exceptions.AccessDeniedException) -> None:
    ...
```

Exceptions:

- `Exceptions.AccessDeniedException`
- `Exceptions.ClientError`
- `Exceptions.ConflictException`
- `Exceptions.InternalServerException`
- `Exceptions.NotFoundException`
- `Exceptions.ResourceNotFoundException`
- `Exceptions.ThrottlingException`
- `Exceptions.ValidationException`

<a id="methods"></a>

## Methods

<a id="exceptions"></a>

### exceptions

CodeGuruReviewerClient exceptions.

Type annotations for `session.create_client("codeguru-reviewer").exceptions`
method.

Boto3 documentation:
[CodeGuruReviewer.Client.exceptions](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codeguru-reviewer.html#CodeGuruReviewer.Client.exceptions)

Returns [Exceptions](#exceptions).

<a id="associate\_repository"></a>

### associate_repository

.

Type annotations for
`session.create_client("codeguru-reviewer").associate_repository` method.

Boto3 documentation:
[CodeGuruReviewer.Client.associate_repository](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codeguru-reviewer.html#CodeGuruReviewer.Client.associate_repository)

Asynchronous method. Use `await associate_repository(...)` for a synchronous
call.

Arguments mapping described in
[AssociateRepositoryRequestRequestTypeDef](./type_defs.md#associaterepositoryrequestrequesttypedef).

Keyword-only arguments:

- `Repository`: [RepositoryTypeDef](./type_defs.md#repositorytypedef)
  *(required)*
- `ClientRequestToken`: `str`
- `Tags`: `Mapping`\[`str`, `str`\]
- `KMSKeyDetails`: [KMSKeyDetailsTypeDef](./type_defs.md#kmskeydetailstypedef)

Returns a `Coroutine` for
[AssociateRepositoryResponseTypeDef](./type_defs.md#associaterepositoryresponsetypedef).

<a id="can\_paginate"></a>

### can_paginate

Check if an operation can be paginated.

Type annotations for `session.create_client("codeguru-reviewer").can_paginate`
method.

Boto3 documentation:
[CodeGuruReviewer.Client.can_paginate](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codeguru-reviewer.html#CodeGuruReviewer.Client.can_paginate)

Arguments:

- `operation_name`: `str` *(required)*

Returns `bool`.

<a id="create\_code\_review"></a>

### create_code_review

.

Type annotations for
`session.create_client("codeguru-reviewer").create_code_review` method.

Boto3 documentation:
[CodeGuruReviewer.Client.create_code_review](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codeguru-reviewer.html#CodeGuruReviewer.Client.create_code_review)

Asynchronous method. Use `await create_code_review(...)` for a synchronous
call.

Arguments mapping described in
[CreateCodeReviewRequestRequestTypeDef](./type_defs.md#createcodereviewrequestrequesttypedef).

Keyword-only arguments:

- `Name`: `str` *(required)*
- `RepositoryAssociationArn`: `str` *(required)*
- `Type`: [CodeReviewTypeTypeDef](./type_defs.md#codereviewtypetypedef)
  *(required)*
- `ClientRequestToken`: `str`

Returns a `Coroutine` for
[CreateCodeReviewResponseTypeDef](./type_defs.md#createcodereviewresponsetypedef).

<a id="describe\_code\_review"></a>

### describe_code_review

.

Type annotations for
`session.create_client("codeguru-reviewer").describe_code_review` method.

Boto3 documentation:
[CodeGuruReviewer.Client.describe_code_review](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codeguru-reviewer.html#CodeGuruReviewer.Client.describe_code_review)

Asynchronous method. Use `await describe_code_review(...)` for a synchronous
call.

Arguments mapping described in
[DescribeCodeReviewRequestRequestTypeDef](./type_defs.md#describecodereviewrequestrequesttypedef).

Keyword-only arguments:

- `CodeReviewArn`: `str` *(required)*

Returns a `Coroutine` for
[DescribeCodeReviewResponseTypeDef](./type_defs.md#describecodereviewresponsetypedef).

<a id="describe\_recommendation\_feedback"></a>

### describe_recommendation_feedback

.

Type annotations for
`session.create_client("codeguru-reviewer").describe_recommendation_feedback`
method.

Boto3 documentation:
[CodeGuruReviewer.Client.describe_recommendation_feedback](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codeguru-reviewer.html#CodeGuruReviewer.Client.describe_recommendation_feedback)

Asynchronous method. Use `await describe_recommendation_feedback(...)` for a
synchronous call.

Arguments mapping described in
[DescribeRecommendationFeedbackRequestRequestTypeDef](./type_defs.md#describerecommendationfeedbackrequestrequesttypedef).

Keyword-only arguments:

- `CodeReviewArn`: `str` *(required)*
- `RecommendationId`: `str` *(required)*
- `UserId`: `str`

Returns a `Coroutine` for
[DescribeRecommendationFeedbackResponseTypeDef](./type_defs.md#describerecommendationfeedbackresponsetypedef).

<a id="describe\_repository\_association"></a>

### describe_repository_association

.

Type annotations for
`session.create_client("codeguru-reviewer").describe_repository_association`
method.

Boto3 documentation:
[CodeGuruReviewer.Client.describe_repository_association](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codeguru-reviewer.html#CodeGuruReviewer.Client.describe_repository_association)

Asynchronous method. Use `await describe_repository_association(...)` for a
synchronous call.

Arguments mapping described in
[DescribeRepositoryAssociationRequestRequestTypeDef](./type_defs.md#describerepositoryassociationrequestrequesttypedef).

Keyword-only arguments:

- `AssociationArn`: `str` *(required)*

Returns a `Coroutine` for
[DescribeRepositoryAssociationResponseTypeDef](./type_defs.md#describerepositoryassociationresponsetypedef).

<a id="disassociate\_repository"></a>

### disassociate_repository

.

Type annotations for
`session.create_client("codeguru-reviewer").disassociate_repository` method.

Boto3 documentation:
[CodeGuruReviewer.Client.disassociate_repository](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codeguru-reviewer.html#CodeGuruReviewer.Client.disassociate_repository)

Asynchronous method. Use `await disassociate_repository(...)` for a synchronous
call.

Arguments mapping described in
[DisassociateRepositoryRequestRequestTypeDef](./type_defs.md#disassociaterepositoryrequestrequesttypedef).

Keyword-only arguments:

- `AssociationArn`: `str` *(required)*

Returns a `Coroutine` for
[DisassociateRepositoryResponseTypeDef](./type_defs.md#disassociaterepositoryresponsetypedef).

<a id="generate\_presigned\_url"></a>

### generate_presigned_url

Generate a presigned url given a client, its method, and arguments.

Type annotations for
`session.create_client("codeguru-reviewer").generate_presigned_url` method.

Boto3 documentation:
[CodeGuruReviewer.Client.generate_presigned_url](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codeguru-reviewer.html#CodeGuruReviewer.Client.generate_presigned_url)

Asynchronous method. Use `await generate_presigned_url(...)` for a synchronous
call.

Arguments:

- `ClientMethod`: `str` *(required)*
- `Params`: `Mapping`\[`str`, `Any`\]
- `ExpiresIn`: `int`
- `HttpMethod`: `str`

Returns a `Coroutine` for `str`.

<a id="list\_code\_reviews"></a>

### list_code_reviews

.

Type annotations for
`session.create_client("codeguru-reviewer").list_code_reviews` method.

Boto3 documentation:
[CodeGuruReviewer.Client.list_code_reviews](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codeguru-reviewer.html#CodeGuruReviewer.Client.list_code_reviews)

Asynchronous method. Use `await list_code_reviews(...)` for a synchronous call.

Arguments mapping described in
[ListCodeReviewsRequestRequestTypeDef](./type_defs.md#listcodereviewsrequestrequesttypedef).

Keyword-only arguments:

- `Type`: [TypeType](./literals.md#typetype) *(required)*
- `ProviderTypes`:
  `Sequence`\[[ProviderTypeType](./literals.md#providertypetype)\]
- `States`: `Sequence`\[[JobStateType](./literals.md#jobstatetype)\]
- `RepositoryNames`: `Sequence`\[`str`\]
- `MaxResults`: `int`
- `NextToken`: `str`

Returns a `Coroutine` for
[ListCodeReviewsResponseTypeDef](./type_defs.md#listcodereviewsresponsetypedef).

<a id="list\_recommendation\_feedback"></a>

### list_recommendation_feedback

.

Type annotations for
`session.create_client("codeguru-reviewer").list_recommendation_feedback`
method.

Boto3 documentation:
[CodeGuruReviewer.Client.list_recommendation_feedback](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codeguru-reviewer.html#CodeGuruReviewer.Client.list_recommendation_feedback)

Asynchronous method. Use `await list_recommendation_feedback(...)` for a
synchronous call.

Arguments mapping described in
[ListRecommendationFeedbackRequestRequestTypeDef](./type_defs.md#listrecommendationfeedbackrequestrequesttypedef).

Keyword-only arguments:

- `CodeReviewArn`: `str` *(required)*
- `NextToken`: `str`
- `MaxResults`: `int`
- `UserIds`: `Sequence`\[`str`\]
- `RecommendationIds`: `Sequence`\[`str`\]

Returns a `Coroutine` for
[ListRecommendationFeedbackResponseTypeDef](./type_defs.md#listrecommendationfeedbackresponsetypedef).

<a id="list\_recommendations"></a>

### list_recommendations

.

Type annotations for
`session.create_client("codeguru-reviewer").list_recommendations` method.

Boto3 documentation:
[CodeGuruReviewer.Client.list_recommendations](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codeguru-reviewer.html#CodeGuruReviewer.Client.list_recommendations)

Asynchronous method. Use `await list_recommendations(...)` for a synchronous
call.

Arguments mapping described in
[ListRecommendationsRequestRequestTypeDef](./type_defs.md#listrecommendationsrequestrequesttypedef).

Keyword-only arguments:

- `CodeReviewArn`: `str` *(required)*
- `NextToken`: `str`
- `MaxResults`: `int`

Returns a `Coroutine` for
[ListRecommendationsResponseTypeDef](./type_defs.md#listrecommendationsresponsetypedef).

<a id="list\_repository\_associations"></a>

### list_repository_associations

.

Type annotations for
`session.create_client("codeguru-reviewer").list_repository_associations`
method.

Boto3 documentation:
[CodeGuruReviewer.Client.list_repository_associations](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codeguru-reviewer.html#CodeGuruReviewer.Client.list_repository_associations)

Asynchronous method. Use `await list_repository_associations(...)` for a
synchronous call.

Arguments mapping described in
[ListRepositoryAssociationsRequestRequestTypeDef](./type_defs.md#listrepositoryassociationsrequestrequesttypedef).

Keyword-only arguments:

- `ProviderTypes`:
  `Sequence`\[[ProviderTypeType](./literals.md#providertypetype)\]
- `States`:
  `Sequence`\[[RepositoryAssociationStateType](./literals.md#repositoryassociationstatetype)\]
- `Names`: `Sequence`\[`str`\]
- `Owners`: `Sequence`\[`str`\]
- `MaxResults`: `int`
- `NextToken`: `str`

Returns a `Coroutine` for
[ListRepositoryAssociationsResponseTypeDef](./type_defs.md#listrepositoryassociationsresponsetypedef).

<a id="list\_tags\_for\_resource"></a>

### list_tags_for_resource

.

Type annotations for
`session.create_client("codeguru-reviewer").list_tags_for_resource` method.

Boto3 documentation:
[CodeGuruReviewer.Client.list_tags_for_resource](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codeguru-reviewer.html#CodeGuruReviewer.Client.list_tags_for_resource)

Asynchronous method. Use `await list_tags_for_resource(...)` for a synchronous
call.

Arguments mapping described in
[ListTagsForResourceRequestRequestTypeDef](./type_defs.md#listtagsforresourcerequestrequesttypedef).

Keyword-only arguments:

- `resourceArn`: `str` *(required)*

Returns a `Coroutine` for
[ListTagsForResourceResponseTypeDef](./type_defs.md#listtagsforresourceresponsetypedef).

<a id="put\_recommendation\_feedback"></a>

### put_recommendation_feedback

.

Type annotations for
`session.create_client("codeguru-reviewer").put_recommendation_feedback`
method.

Boto3 documentation:
[CodeGuruReviewer.Client.put_recommendation_feedback](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codeguru-reviewer.html#CodeGuruReviewer.Client.put_recommendation_feedback)

Asynchronous method. Use `await put_recommendation_feedback(...)` for a
synchronous call.

Arguments mapping described in
[PutRecommendationFeedbackRequestRequestTypeDef](./type_defs.md#putrecommendationfeedbackrequestrequesttypedef).

Keyword-only arguments:

- `CodeReviewArn`: `str` *(required)*
- `RecommendationId`: `str` *(required)*
- `Reactions`: `Sequence`\[[ReactionType](./literals.md#reactiontype)\]
  *(required)*

Returns a `Coroutine` for `Dict`\[`str`, `Any`\].

<a id="tag\_resource"></a>

### tag_resource

.

Type annotations for `session.create_client("codeguru-reviewer").tag_resource`
method.

Boto3 documentation:
[CodeGuruReviewer.Client.tag_resource](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codeguru-reviewer.html#CodeGuruReviewer.Client.tag_resource)

Asynchronous method. Use `await tag_resource(...)` for a synchronous call.

Arguments mapping described in
[TagResourceRequestRequestTypeDef](./type_defs.md#tagresourcerequestrequesttypedef).

Keyword-only arguments:

- `resourceArn`: `str` *(required)*
- `Tags`: `Mapping`\[`str`, `str`\] *(required)*

Returns a `Coroutine` for `Dict`\[`str`, `Any`\].

<a id="untag\_resource"></a>

### untag_resource

.

Type annotations for
`session.create_client("codeguru-reviewer").untag_resource` method.

Boto3 documentation:
[CodeGuruReviewer.Client.untag_resource](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codeguru-reviewer.html#CodeGuruReviewer.Client.untag_resource)

Asynchronous method. Use `await untag_resource(...)` for a synchronous call.

Arguments mapping described in
[UntagResourceRequestRequestTypeDef](./type_defs.md#untagresourcerequestrequesttypedef).

Keyword-only arguments:

- `resourceArn`: `str` *(required)*
- `TagKeys`: `Sequence`\[`str`\] *(required)*

Returns a `Coroutine` for `Dict`\[`str`, `Any`\].

<a id="\_\_aenter\_\_"></a>

### \_\_aenter\_\_

Type annotations for `session.create_client("codeguru-reviewer").__aenter__`
method.

Boto3 documentation:
[CodeGuruReviewer.Client.\_\_aenter\_\_](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codeguru-reviewer.html#CodeGuruReviewer.Client.__aenter__)

Asynchronous method. Use `await __aenter__(...)` for a synchronous call.

Returns a `Coroutine` for [CodeGuruReviewerClient](#codegurureviewerclient).

<a id="\_\_aexit\_\_"></a>

### \_\_aexit\_\_

Type annotations for `session.create_client("codeguru-reviewer").__aexit__`
method.

Boto3 documentation:
[CodeGuruReviewer.Client.\_\_aexit\_\_](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codeguru-reviewer.html#CodeGuruReviewer.Client.__aexit__)

Asynchronous method. Use `await __aexit__(...)` for a synchronous call.

Arguments:

- `exc_type`: `Any` *(required)*
- `exc_val`: `Any` *(required)*
- `exc_tb`: `Any` *(required)*

Returns a `Coroutine` for `Any`.

<a id="get_paginator"></a>

### get_paginator

Type annotations for `session.create_client("codeguru-reviewer").get_paginator`
method with overloads.

- `client.get_paginator("list_repository_associations")` ->
  [ListRepositoryAssociationsPaginator](./paginators.md#listrepositoryassociationspaginator)

<a id="get_waiter"></a>

### get_waiter

Type annotations for `session.create_client("codeguru-reviewer").get_waiter`
method with overloads.

- `client.get_waiter("code_review_completed")` ->
  [CodeReviewCompletedWaiter](./waiters.md#codereviewcompletedwaiter)
- `client.get_waiter("repository_association_succeeded")` ->
  [RepositoryAssociationSucceededWaiter](./waiters.md#repositoryassociationsucceededwaiter)