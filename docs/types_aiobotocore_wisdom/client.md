<a id="connectwisdomserviceclient-for-aiobotocore-connectwisdomservice-module"></a>

# ConnectWisdomServiceClient for aiobotocore ConnectWisdomService module

> [Index](../README.md) > [ConnectWisdomService](./README.md) >
> ConnectWisdomServiceClient

Auto-generated documentation for
[ConnectWisdomService](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/wisdom.html#ConnectWisdomService)
type annotations stubs module
[types-aiobotocore-wisdom](https://pypi.org/project/types-aiobotocore-wisdom/).

- [ConnectWisdomServiceClient for aiobotocore ConnectWisdomService module](#connectwisdomserviceclient-for-aiobotocore-connectwisdomservice-module)
  - [ConnectWisdomServiceClient](#connectwisdomserviceclient)
  - [Exceptions](#exceptions)
  - [Methods](#methods)
    - [exceptions](#exceptions)
    - [can_paginate](#can_paginate)
    - [create_assistant](#create_assistant)
    - [create_assistant_association](#create_assistant_association)
    - [create_content](#create_content)
    - [create_knowledge_base](#create_knowledge_base)
    - [create_session](#create_session)
    - [delete_assistant](#delete_assistant)
    - [delete_assistant_association](#delete_assistant_association)
    - [delete_content](#delete_content)
    - [delete_knowledge_base](#delete_knowledge_base)
    - [generate_presigned_url](#generate_presigned_url)
    - [get_assistant](#get_assistant)
    - [get_assistant_association](#get_assistant_association)
    - [get_content](#get_content)
    - [get_content_summary](#get_content_summary)
    - [get_knowledge_base](#get_knowledge_base)
    - [get_recommendations](#get_recommendations)
    - [get_session](#get_session)
    - [list_assistant_associations](#list_assistant_associations)
    - [list_assistants](#list_assistants)
    - [list_contents](#list_contents)
    - [list_knowledge_bases](#list_knowledge_bases)
    - [list_tags_for_resource](#list_tags_for_resource)
    - [notify_recommendations_received](#notify_recommendations_received)
    - [query_assistant](#query_assistant)
    - [remove_knowledge_base_template_uri](#remove_knowledge_base_template_uri)
    - [search_content](#search_content)
    - [search_sessions](#search_sessions)
    - [start_content_upload](#start_content_upload)
    - [tag_resource](#tag_resource)
    - [untag_resource](#untag_resource)
    - [update_content](#update_content)
    - [update_knowledge_base_template_uri](#update_knowledge_base_template_uri)
    - [\_\_aenter\_\_](#__aenter__)
    - [\_\_aexit\_\_](#__aexit__)
    - [get_paginator](#get_paginator)

<a id="connectwisdomserviceclient"></a>

## ConnectWisdomServiceClient

Type annotations for `session.create_client("wisdom")`

Can be used directly:

```python
from aiobotocore.session import get_session
from types_aiobotocore_wisdom.client import ConnectWisdomServiceClient

session = get_session()
async with session.create_client("wisdom") as client:
    client: ConnectWisdomServiceClient
```

Boto3 documentation:
[ConnectWisdomService.Client](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/wisdom.html#ConnectWisdomService.Client)

<a id="exceptions"></a>

## Exceptions

`boto3` client exceptions are generated in runtime. This class can be used for
static analysis directly:

```python
from types_aiobotocore_wisdom.client import Exceptions

def handle_error(exc: Exceptions.AccessDeniedException) -> None:
    ...
```

Exceptions:

- `Exceptions.AccessDeniedException`
- `Exceptions.ClientError`
- `Exceptions.ConflictException`
- `Exceptions.PreconditionFailedException`
- `Exceptions.ResourceNotFoundException`
- `Exceptions.ServiceQuotaExceededException`
- `Exceptions.TooManyTagsException`
- `Exceptions.ValidationException`

<a id="methods"></a>

## Methods

<a id="exceptions"></a>

### exceptions

ConnectWisdomServiceClient exceptions.

Type annotations for `session.create_client("wisdom").exceptions` method.

Boto3 documentation:
[ConnectWisdomService.Client.exceptions](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/wisdom.html#ConnectWisdomService.Client.exceptions)

Returns [Exceptions](#exceptions).

<a id="can\_paginate"></a>

### can_paginate

Check if an operation can be paginated.

Type annotations for `session.create_client("wisdom").can_paginate` method.

Boto3 documentation:
[ConnectWisdomService.Client.can_paginate](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/wisdom.html#ConnectWisdomService.Client.can_paginate)

Arguments:

- `operation_name`: `str` *(required)*

Returns `bool`.

<a id="create\_assistant"></a>

### create_assistant

Creates an Amazon Connect Wisdom assistant.

Type annotations for `session.create_client("wisdom").create_assistant` method.

Boto3 documentation:
[ConnectWisdomService.Client.create_assistant](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/wisdom.html#ConnectWisdomService.Client.create_assistant)

Asynchronous method. Use `await create_assistant(...)` for a synchronous call.

Arguments mapping described in
[CreateAssistantRequestRequestTypeDef](./type_defs.md#createassistantrequestrequesttypedef).

Keyword-only arguments:

- `name`: `str` *(required)*
- `type`: `Literal['AGENT']` (see
  [AssistantTypeType](./literals.md#assistanttypetype)) *(required)*
- `clientToken`: `str`
- `description`: `str`
- `serverSideEncryptionConfiguration`:
  [ServerSideEncryptionConfigurationTypeDef](./type_defs.md#serversideencryptionconfigurationtypedef)
- `tags`: `Mapping`\[`str`, `str`\]

Returns a `Coroutine` for
[CreateAssistantResponseTypeDef](./type_defs.md#createassistantresponsetypedef).

<a id="create\_assistant\_association"></a>

### create_assistant_association

Creates an association between an Amazon Connect Wisdom assistant and another
resource.

Type annotations for
`session.create_client("wisdom").create_assistant_association` method.

Boto3 documentation:
[ConnectWisdomService.Client.create_assistant_association](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/wisdom.html#ConnectWisdomService.Client.create_assistant_association)

Asynchronous method. Use `await create_assistant_association(...)` for a
synchronous call.

Arguments mapping described in
[CreateAssistantAssociationRequestRequestTypeDef](./type_defs.md#createassistantassociationrequestrequesttypedef).

Keyword-only arguments:

- `assistantId`: `str` *(required)*
- `association`:
  [AssistantAssociationInputDataTypeDef](./type_defs.md#assistantassociationinputdatatypedef)
  *(required)*
- `associationType`: `Literal['KNOWLEDGE_BASE']` (see
  [AssociationTypeType](./literals.md#associationtypetype)) *(required)*
- `clientToken`: `str`
- `tags`: `Mapping`\[`str`, `str`\]

Returns a `Coroutine` for
[CreateAssistantAssociationResponseTypeDef](./type_defs.md#createassistantassociationresponsetypedef).

<a id="create\_content"></a>

### create_content

Creates Wisdom content.

Type annotations for `session.create_client("wisdom").create_content` method.

Boto3 documentation:
[ConnectWisdomService.Client.create_content](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/wisdom.html#ConnectWisdomService.Client.create_content)

Asynchronous method. Use `await create_content(...)` for a synchronous call.

Arguments mapping described in
[CreateContentRequestRequestTypeDef](./type_defs.md#createcontentrequestrequesttypedef).

Keyword-only arguments:

- `knowledgeBaseId`: `str` *(required)*
- `name`: `str` *(required)*
- `uploadId`: `str` *(required)*
- `clientToken`: `str`
- `metadata`: `Mapping`\[`str`, `str`\]
- `overrideLinkOutUri`: `str`
- `tags`: `Mapping`\[`str`, `str`\]
- `title`: `str`

Returns a `Coroutine` for
[CreateContentResponseTypeDef](./type_defs.md#createcontentresponsetypedef).

<a id="create\_knowledge\_base"></a>

### create_knowledge_base

Creates a knowledge base.

Type annotations for `session.create_client("wisdom").create_knowledge_base`
method.

Boto3 documentation:
[ConnectWisdomService.Client.create_knowledge_base](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/wisdom.html#ConnectWisdomService.Client.create_knowledge_base)

Asynchronous method. Use `await create_knowledge_base(...)` for a synchronous
call.

Arguments mapping described in
[CreateKnowledgeBaseRequestRequestTypeDef](./type_defs.md#createknowledgebaserequestrequesttypedef).

Keyword-only arguments:

- `knowledgeBaseType`:
  [KnowledgeBaseTypeType](./literals.md#knowledgebasetypetype) *(required)*
- `name`: `str` *(required)*
- `clientToken`: `str`
- `description`: `str`
- `renderingConfiguration`:
  [RenderingConfigurationTypeDef](./type_defs.md#renderingconfigurationtypedef)
- `serverSideEncryptionConfiguration`:
  [ServerSideEncryptionConfigurationTypeDef](./type_defs.md#serversideencryptionconfigurationtypedef)
- `sourceConfiguration`:
  [SourceConfigurationTypeDef](./type_defs.md#sourceconfigurationtypedef)
- `tags`: `Mapping`\[`str`, `str`\]

Returns a `Coroutine` for
[CreateKnowledgeBaseResponseTypeDef](./type_defs.md#createknowledgebaseresponsetypedef).

<a id="create\_session"></a>

### create_session

Creates a session.

Type annotations for `session.create_client("wisdom").create_session` method.

Boto3 documentation:
[ConnectWisdomService.Client.create_session](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/wisdom.html#ConnectWisdomService.Client.create_session)

Asynchronous method. Use `await create_session(...)` for a synchronous call.

Arguments mapping described in
[CreateSessionRequestRequestTypeDef](./type_defs.md#createsessionrequestrequesttypedef).

Keyword-only arguments:

- `assistantId`: `str` *(required)*
- `name`: `str` *(required)*
- `clientToken`: `str`
- `description`: `str`
- `tags`: `Mapping`\[`str`, `str`\]

Returns a `Coroutine` for
[CreateSessionResponseTypeDef](./type_defs.md#createsessionresponsetypedef).

<a id="delete\_assistant"></a>

### delete_assistant

Deletes an assistant.

Type annotations for `session.create_client("wisdom").delete_assistant` method.

Boto3 documentation:
[ConnectWisdomService.Client.delete_assistant](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/wisdom.html#ConnectWisdomService.Client.delete_assistant)

Asynchronous method. Use `await delete_assistant(...)` for a synchronous call.

Arguments mapping described in
[DeleteAssistantRequestRequestTypeDef](./type_defs.md#deleteassistantrequestrequesttypedef).

Keyword-only arguments:

- `assistantId`: `str` *(required)*

Returns a `Coroutine` for `Dict`\[`str`, `Any`\].

<a id="delete\_assistant\_association"></a>

### delete_assistant_association

Deletes an assistant association.

Type annotations for
`session.create_client("wisdom").delete_assistant_association` method.

Boto3 documentation:
[ConnectWisdomService.Client.delete_assistant_association](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/wisdom.html#ConnectWisdomService.Client.delete_assistant_association)

Asynchronous method. Use `await delete_assistant_association(...)` for a
synchronous call.

Arguments mapping described in
[DeleteAssistantAssociationRequestRequestTypeDef](./type_defs.md#deleteassistantassociationrequestrequesttypedef).

Keyword-only arguments:

- `assistantAssociationId`: `str` *(required)*
- `assistantId`: `str` *(required)*

Returns a `Coroutine` for `Dict`\[`str`, `Any`\].

<a id="delete\_content"></a>

### delete_content

Deletes the content.

Type annotations for `session.create_client("wisdom").delete_content` method.

Boto3 documentation:
[ConnectWisdomService.Client.delete_content](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/wisdom.html#ConnectWisdomService.Client.delete_content)

Asynchronous method. Use `await delete_content(...)` for a synchronous call.

Arguments mapping described in
[DeleteContentRequestRequestTypeDef](./type_defs.md#deletecontentrequestrequesttypedef).

Keyword-only arguments:

- `contentId`: `str` *(required)*
- `knowledgeBaseId`: `str` *(required)*

Returns a `Coroutine` for `Dict`\[`str`, `Any`\].

<a id="delete\_knowledge\_base"></a>

### delete_knowledge_base

Deletes the knowledge base.

Type annotations for `session.create_client("wisdom").delete_knowledge_base`
method.

Boto3 documentation:
[ConnectWisdomService.Client.delete_knowledge_base](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/wisdom.html#ConnectWisdomService.Client.delete_knowledge_base)

Asynchronous method. Use `await delete_knowledge_base(...)` for a synchronous
call.

Arguments mapping described in
[DeleteKnowledgeBaseRequestRequestTypeDef](./type_defs.md#deleteknowledgebaserequestrequesttypedef).

Keyword-only arguments:

- `knowledgeBaseId`: `str` *(required)*

Returns a `Coroutine` for `Dict`\[`str`, `Any`\].

<a id="generate\_presigned\_url"></a>

### generate_presigned_url

Generate a presigned url given a client, its method, and arguments.

Type annotations for `session.create_client("wisdom").generate_presigned_url`
method.

Boto3 documentation:
[ConnectWisdomService.Client.generate_presigned_url](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/wisdom.html#ConnectWisdomService.Client.generate_presigned_url)

Asynchronous method. Use `await generate_presigned_url(...)` for a synchronous
call.

Arguments:

- `ClientMethod`: `str` *(required)*
- `Params`: `Mapping`\[`str`, `Any`\]
- `ExpiresIn`: `int`
- `HttpMethod`: `str`

Returns a `Coroutine` for `str`.

<a id="get\_assistant"></a>

### get_assistant

Retrieves information about an assistant.

Type annotations for `session.create_client("wisdom").get_assistant` method.

Boto3 documentation:
[ConnectWisdomService.Client.get_assistant](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/wisdom.html#ConnectWisdomService.Client.get_assistant)

Asynchronous method. Use `await get_assistant(...)` for a synchronous call.

Arguments mapping described in
[GetAssistantRequestRequestTypeDef](./type_defs.md#getassistantrequestrequesttypedef).

Keyword-only arguments:

- `assistantId`: `str` *(required)*

Returns a `Coroutine` for
[GetAssistantResponseTypeDef](./type_defs.md#getassistantresponsetypedef).

<a id="get\_assistant\_association"></a>

### get_assistant_association

Retrieves information about an assistant association.

Type annotations for
`session.create_client("wisdom").get_assistant_association` method.

Boto3 documentation:
[ConnectWisdomService.Client.get_assistant_association](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/wisdom.html#ConnectWisdomService.Client.get_assistant_association)

Asynchronous method. Use `await get_assistant_association(...)` for a
synchronous call.

Arguments mapping described in
[GetAssistantAssociationRequestRequestTypeDef](./type_defs.md#getassistantassociationrequestrequesttypedef).

Keyword-only arguments:

- `assistantAssociationId`: `str` *(required)*
- `assistantId`: `str` *(required)*

Returns a `Coroutine` for
[GetAssistantAssociationResponseTypeDef](./type_defs.md#getassistantassociationresponsetypedef).

<a id="get\_content"></a>

### get_content

Retrieves content, including a pre-signed URL to download the content.

Type annotations for `session.create_client("wisdom").get_content` method.

Boto3 documentation:
[ConnectWisdomService.Client.get_content](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/wisdom.html#ConnectWisdomService.Client.get_content)

Asynchronous method. Use `await get_content(...)` for a synchronous call.

Arguments mapping described in
[GetContentRequestRequestTypeDef](./type_defs.md#getcontentrequestrequesttypedef).

Keyword-only arguments:

- `contentId`: `str` *(required)*
- `knowledgeBaseId`: `str` *(required)*

Returns a `Coroutine` for
[GetContentResponseTypeDef](./type_defs.md#getcontentresponsetypedef).

<a id="get\_content\_summary"></a>

### get_content_summary

Retrieves summary information about the content.

Type annotations for `session.create_client("wisdom").get_content_summary`
method.

Boto3 documentation:
[ConnectWisdomService.Client.get_content_summary](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/wisdom.html#ConnectWisdomService.Client.get_content_summary)

Asynchronous method. Use `await get_content_summary(...)` for a synchronous
call.

Arguments mapping described in
[GetContentSummaryRequestRequestTypeDef](./type_defs.md#getcontentsummaryrequestrequesttypedef).

Keyword-only arguments:

- `contentId`: `str` *(required)*
- `knowledgeBaseId`: `str` *(required)*

Returns a `Coroutine` for
[GetContentSummaryResponseTypeDef](./type_defs.md#getcontentsummaryresponsetypedef).

<a id="get\_knowledge\_base"></a>

### get_knowledge_base

Retrieves information about the knowledge base.

Type annotations for `session.create_client("wisdom").get_knowledge_base`
method.

Boto3 documentation:
[ConnectWisdomService.Client.get_knowledge_base](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/wisdom.html#ConnectWisdomService.Client.get_knowledge_base)

Asynchronous method. Use `await get_knowledge_base(...)` for a synchronous
call.

Arguments mapping described in
[GetKnowledgeBaseRequestRequestTypeDef](./type_defs.md#getknowledgebaserequestrequesttypedef).

Keyword-only arguments:

- `knowledgeBaseId`: `str` *(required)*

Returns a `Coroutine` for
[GetKnowledgeBaseResponseTypeDef](./type_defs.md#getknowledgebaseresponsetypedef).

<a id="get\_recommendations"></a>

### get_recommendations

Retrieves recommendations for the specified session.

Type annotations for `session.create_client("wisdom").get_recommendations`
method.

Boto3 documentation:
[ConnectWisdomService.Client.get_recommendations](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/wisdom.html#ConnectWisdomService.Client.get_recommendations)

Asynchronous method. Use `await get_recommendations(...)` for a synchronous
call.

Arguments mapping described in
[GetRecommendationsRequestRequestTypeDef](./type_defs.md#getrecommendationsrequestrequesttypedef).

Keyword-only arguments:

- `assistantId`: `str` *(required)*
- `sessionId`: `str` *(required)*
- `maxResults`: `int`
- `waitTimeSeconds`: `int`

Returns a `Coroutine` for
[GetRecommendationsResponseTypeDef](./type_defs.md#getrecommendationsresponsetypedef).

<a id="get\_session"></a>

### get_session

Retrieves information for a specified session.

Type annotations for `session.create_client("wisdom").get_session` method.

Boto3 documentation:
[ConnectWisdomService.Client.get_session](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/wisdom.html#ConnectWisdomService.Client.get_session)

Asynchronous method. Use `await get_session(...)` for a synchronous call.

Arguments mapping described in
[GetSessionRequestRequestTypeDef](./type_defs.md#getsessionrequestrequesttypedef).

Keyword-only arguments:

- `assistantId`: `str` *(required)*
- `sessionId`: `str` *(required)*

Returns a `Coroutine` for
[GetSessionResponseTypeDef](./type_defs.md#getsessionresponsetypedef).

<a id="list\_assistant\_associations"></a>

### list_assistant_associations

Lists information about assistant associations.

Type annotations for
`session.create_client("wisdom").list_assistant_associations` method.

Boto3 documentation:
[ConnectWisdomService.Client.list_assistant_associations](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/wisdom.html#ConnectWisdomService.Client.list_assistant_associations)

Asynchronous method. Use `await list_assistant_associations(...)` for a
synchronous call.

Arguments mapping described in
[ListAssistantAssociationsRequestRequestTypeDef](./type_defs.md#listassistantassociationsrequestrequesttypedef).

Keyword-only arguments:

- `assistantId`: `str` *(required)*
- `maxResults`: `int`
- `nextToken`: `str`

Returns a `Coroutine` for
[ListAssistantAssociationsResponseTypeDef](./type_defs.md#listassistantassociationsresponsetypedef).

<a id="list\_assistants"></a>

### list_assistants

Lists information about assistants.

Type annotations for `session.create_client("wisdom").list_assistants` method.

Boto3 documentation:
[ConnectWisdomService.Client.list_assistants](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/wisdom.html#ConnectWisdomService.Client.list_assistants)

Asynchronous method. Use `await list_assistants(...)` for a synchronous call.

Arguments mapping described in
[ListAssistantsRequestRequestTypeDef](./type_defs.md#listassistantsrequestrequesttypedef).

Keyword-only arguments:

- `maxResults`: `int`
- `nextToken`: `str`

Returns a `Coroutine` for
[ListAssistantsResponseTypeDef](./type_defs.md#listassistantsresponsetypedef).

<a id="list\_contents"></a>

### list_contents

Lists the content.

Type annotations for `session.create_client("wisdom").list_contents` method.

Boto3 documentation:
[ConnectWisdomService.Client.list_contents](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/wisdom.html#ConnectWisdomService.Client.list_contents)

Asynchronous method. Use `await list_contents(...)` for a synchronous call.

Arguments mapping described in
[ListContentsRequestRequestTypeDef](./type_defs.md#listcontentsrequestrequesttypedef).

Keyword-only arguments:

- `knowledgeBaseId`: `str` *(required)*
- `maxResults`: `int`
- `nextToken`: `str`

Returns a `Coroutine` for
[ListContentsResponseTypeDef](./type_defs.md#listcontentsresponsetypedef).

<a id="list\_knowledge\_bases"></a>

### list_knowledge_bases

Lists the knowledge bases.

Type annotations for `session.create_client("wisdom").list_knowledge_bases`
method.

Boto3 documentation:
[ConnectWisdomService.Client.list_knowledge_bases](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/wisdom.html#ConnectWisdomService.Client.list_knowledge_bases)

Asynchronous method. Use `await list_knowledge_bases(...)` for a synchronous
call.

Arguments mapping described in
[ListKnowledgeBasesRequestRequestTypeDef](./type_defs.md#listknowledgebasesrequestrequesttypedef).

Keyword-only arguments:

- `maxResults`: `int`
- `nextToken`: `str`

Returns a `Coroutine` for
[ListKnowledgeBasesResponseTypeDef](./type_defs.md#listknowledgebasesresponsetypedef).

<a id="list\_tags\_for\_resource"></a>

### list_tags_for_resource

Lists the tags for the specified resource.

Type annotations for `session.create_client("wisdom").list_tags_for_resource`
method.

Boto3 documentation:
[ConnectWisdomService.Client.list_tags_for_resource](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/wisdom.html#ConnectWisdomService.Client.list_tags_for_resource)

Asynchronous method. Use `await list_tags_for_resource(...)` for a synchronous
call.

Arguments mapping described in
[ListTagsForResourceRequestRequestTypeDef](./type_defs.md#listtagsforresourcerequestrequesttypedef).

Keyword-only arguments:

- `resourceArn`: `str` *(required)*

Returns a `Coroutine` for
[ListTagsForResourceResponseTypeDef](./type_defs.md#listtagsforresourceresponsetypedef).

<a id="notify\_recommendations\_received"></a>

### notify_recommendations_received

Removes the specified recommendations from the specified assistant's queue of
newly available recommendations.

Type annotations for
`session.create_client("wisdom").notify_recommendations_received` method.

Boto3 documentation:
[ConnectWisdomService.Client.notify_recommendations_received](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/wisdom.html#ConnectWisdomService.Client.notify_recommendations_received)

Asynchronous method. Use `await notify_recommendations_received(...)` for a
synchronous call.

Arguments mapping described in
[NotifyRecommendationsReceivedRequestRequestTypeDef](./type_defs.md#notifyrecommendationsreceivedrequestrequesttypedef).

Keyword-only arguments:

- `assistantId`: `str` *(required)*
- `recommendationIds`: `Sequence`\[`str`\] *(required)*
- `sessionId`: `str` *(required)*

Returns a `Coroutine` for
[NotifyRecommendationsReceivedResponseTypeDef](./type_defs.md#notifyrecommendationsreceivedresponsetypedef).

<a id="query\_assistant"></a>

### query_assistant

Performs a manual search against the specified assistant.

Type annotations for `session.create_client("wisdom").query_assistant` method.

Boto3 documentation:
[ConnectWisdomService.Client.query_assistant](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/wisdom.html#ConnectWisdomService.Client.query_assistant)

Asynchronous method. Use `await query_assistant(...)` for a synchronous call.

Arguments mapping described in
[QueryAssistantRequestRequestTypeDef](./type_defs.md#queryassistantrequestrequesttypedef).

Keyword-only arguments:

- `assistantId`: `str` *(required)*
- `queryText`: `str` *(required)*
- `maxResults`: `int`
- `nextToken`: `str`

Returns a `Coroutine` for
[QueryAssistantResponseTypeDef](./type_defs.md#queryassistantresponsetypedef).

<a id="remove\_knowledge\_base\_template\_uri"></a>

### remove_knowledge_base_template_uri

Removes a URI template from a knowledge base.

Type annotations for
`session.create_client("wisdom").remove_knowledge_base_template_uri` method.

Boto3 documentation:
[ConnectWisdomService.Client.remove_knowledge_base_template_uri](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/wisdom.html#ConnectWisdomService.Client.remove_knowledge_base_template_uri)

Asynchronous method. Use `await remove_knowledge_base_template_uri(...)` for a
synchronous call.

Arguments mapping described in
[RemoveKnowledgeBaseTemplateUriRequestRequestTypeDef](./type_defs.md#removeknowledgebasetemplateurirequestrequesttypedef).

Keyword-only arguments:

- `knowledgeBaseId`: `str` *(required)*

Returns a `Coroutine` for `Dict`\[`str`, `Any`\].

<a id="search\_content"></a>

### search_content

Searches for content in a specified knowledge base.

Type annotations for `session.create_client("wisdom").search_content` method.

Boto3 documentation:
[ConnectWisdomService.Client.search_content](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/wisdom.html#ConnectWisdomService.Client.search_content)

Asynchronous method. Use `await search_content(...)` for a synchronous call.

Arguments mapping described in
[SearchContentRequestRequestTypeDef](./type_defs.md#searchcontentrequestrequesttypedef).

Keyword-only arguments:

- `knowledgeBaseId`: `str` *(required)*
- `searchExpression`:
  [SearchExpressionTypeDef](./type_defs.md#searchexpressiontypedef)
  *(required)*
- `maxResults`: `int`
- `nextToken`: `str`

Returns a `Coroutine` for
[SearchContentResponseTypeDef](./type_defs.md#searchcontentresponsetypedef).

<a id="search\_sessions"></a>

### search_sessions

Searches for sessions.

Type annotations for `session.create_client("wisdom").search_sessions` method.

Boto3 documentation:
[ConnectWisdomService.Client.search_sessions](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/wisdom.html#ConnectWisdomService.Client.search_sessions)

Asynchronous method. Use `await search_sessions(...)` for a synchronous call.

Arguments mapping described in
[SearchSessionsRequestRequestTypeDef](./type_defs.md#searchsessionsrequestrequesttypedef).

Keyword-only arguments:

- `assistantId`: `str` *(required)*
- `searchExpression`:
  [SearchExpressionTypeDef](./type_defs.md#searchexpressiontypedef)
  *(required)*
- `maxResults`: `int`
- `nextToken`: `str`

Returns a `Coroutine` for
[SearchSessionsResponseTypeDef](./type_defs.md#searchsessionsresponsetypedef).

<a id="start\_content\_upload"></a>

### start_content_upload

Get a URL to upload content to a knowledge base.

Type annotations for `session.create_client("wisdom").start_content_upload`
method.

Boto3 documentation:
[ConnectWisdomService.Client.start_content_upload](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/wisdom.html#ConnectWisdomService.Client.start_content_upload)

Asynchronous method. Use `await start_content_upload(...)` for a synchronous
call.

Arguments mapping described in
[StartContentUploadRequestRequestTypeDef](./type_defs.md#startcontentuploadrequestrequesttypedef).

Keyword-only arguments:

- `contentType`: `str` *(required)*
- `knowledgeBaseId`: `str` *(required)*

Returns a `Coroutine` for
[StartContentUploadResponseTypeDef](./type_defs.md#startcontentuploadresponsetypedef).

<a id="tag\_resource"></a>

### tag_resource

Adds the specified tags to the specified resource.

Type annotations for `session.create_client("wisdom").tag_resource` method.

Boto3 documentation:
[ConnectWisdomService.Client.tag_resource](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/wisdom.html#ConnectWisdomService.Client.tag_resource)

Asynchronous method. Use `await tag_resource(...)` for a synchronous call.

Arguments mapping described in
[TagResourceRequestRequestTypeDef](./type_defs.md#tagresourcerequestrequesttypedef).

Keyword-only arguments:

- `resourceArn`: `str` *(required)*
- `tags`: `Mapping`\[`str`, `str`\] *(required)*

Returns a `Coroutine` for `Dict`\[`str`, `Any`\].

<a id="untag\_resource"></a>

### untag_resource

Removes the specified tags from the specified resource.

Type annotations for `session.create_client("wisdom").untag_resource` method.

Boto3 documentation:
[ConnectWisdomService.Client.untag_resource](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/wisdom.html#ConnectWisdomService.Client.untag_resource)

Asynchronous method. Use `await untag_resource(...)` for a synchronous call.

Arguments mapping described in
[UntagResourceRequestRequestTypeDef](./type_defs.md#untagresourcerequestrequesttypedef).

Keyword-only arguments:

- `resourceArn`: `str` *(required)*
- `tagKeys`: `Sequence`\[`str`\] *(required)*

Returns a `Coroutine` for `Dict`\[`str`, `Any`\].

<a id="update\_content"></a>

### update_content

Updates information about the content.

Type annotations for `session.create_client("wisdom").update_content` method.

Boto3 documentation:
[ConnectWisdomService.Client.update_content](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/wisdom.html#ConnectWisdomService.Client.update_content)

Asynchronous method. Use `await update_content(...)` for a synchronous call.

Arguments mapping described in
[UpdateContentRequestRequestTypeDef](./type_defs.md#updatecontentrequestrequesttypedef).

Keyword-only arguments:

- `contentId`: `str` *(required)*
- `knowledgeBaseId`: `str` *(required)*
- `metadata`: `Mapping`\[`str`, `str`\]
- `overrideLinkOutUri`: `str`
- `removeOverrideLinkOutUri`: `bool`
- `revisionId`: `str`
- `title`: `str`
- `uploadId`: `str`

Returns a `Coroutine` for
[UpdateContentResponseTypeDef](./type_defs.md#updatecontentresponsetypedef).

<a id="update\_knowledge\_base\_template\_uri"></a>

### update_knowledge_base_template_uri

Updates the template URI of a knowledge base.

Type annotations for
`session.create_client("wisdom").update_knowledge_base_template_uri` method.

Boto3 documentation:
[ConnectWisdomService.Client.update_knowledge_base_template_uri](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/wisdom.html#ConnectWisdomService.Client.update_knowledge_base_template_uri)

Asynchronous method. Use `await update_knowledge_base_template_uri(...)` for a
synchronous call.

Arguments mapping described in
[UpdateKnowledgeBaseTemplateUriRequestRequestTypeDef](./type_defs.md#updateknowledgebasetemplateurirequestrequesttypedef).

Keyword-only arguments:

- `knowledgeBaseId`: `str` *(required)*
- `templateUri`: `str` *(required)*

Returns a `Coroutine` for
[UpdateKnowledgeBaseTemplateUriResponseTypeDef](./type_defs.md#updateknowledgebasetemplateuriresponsetypedef).

<a id="\_\_aenter\_\_"></a>

### \_\_aenter\_\_

Type annotations for `session.create_client("wisdom").__aenter__` method.

Boto3 documentation:
[ConnectWisdomService.Client.\_\_aenter\_\_](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/wisdom.html#ConnectWisdomService.Client.__aenter__)

Asynchronous method. Use `await __aenter__(...)` for a synchronous call.

Returns a `Coroutine` for
[ConnectWisdomServiceClient](#connectwisdomserviceclient).

<a id="\_\_aexit\_\_"></a>

### \_\_aexit\_\_

Type annotations for `session.create_client("wisdom").__aexit__` method.

Boto3 documentation:
[ConnectWisdomService.Client.\_\_aexit\_\_](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/wisdom.html#ConnectWisdomService.Client.__aexit__)

Asynchronous method. Use `await __aexit__(...)` for a synchronous call.

Arguments:

- `exc_type`: `Any` *(required)*
- `exc_val`: `Any` *(required)*
- `exc_tb`: `Any` *(required)*

Returns a `Coroutine` for `Any`.

<a id="get_paginator"></a>

### get_paginator

Type annotations for `session.create_client("wisdom").get_paginator` method
with overloads.

- `client.get_paginator("list_assistant_associations")` ->
  [ListAssistantAssociationsPaginator](./paginators.md#listassistantassociationspaginator)
- `client.get_paginator("list_assistants")` ->
  [ListAssistantsPaginator](./paginators.md#listassistantspaginator)
- `client.get_paginator("list_contents")` ->
  [ListContentsPaginator](./paginators.md#listcontentspaginator)
- `client.get_paginator("list_knowledge_bases")` ->
  [ListKnowledgeBasesPaginator](./paginators.md#listknowledgebasespaginator)
- `client.get_paginator("query_assistant")` ->
  [QueryAssistantPaginator](./paginators.md#queryassistantpaginator)
- `client.get_paginator("search_content")` ->
  [SearchContentPaginator](./paginators.md#searchcontentpaginator)
- `client.get_paginator("search_sessions")` ->
  [SearchSessionsPaginator](./paginators.md#searchsessionspaginator)
