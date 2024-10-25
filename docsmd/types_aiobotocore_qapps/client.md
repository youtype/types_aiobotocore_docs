# QAppsClient

> [Index](../README.md) > [QApps](./README.md) > QAppsClient

!!! note ""

    Auto-generated documentation for [QApps](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/qapps.html#QApps)
    type annotations stubs module [types-aiobotocore-qapps](https://pypi.org/project/types-aiobotocore-qapps/).

## QAppsClient

Type annotations and code completion for `#!python session.create_client("qapps")`
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/qapps.html#QApps.Client)

```python
# QAppsClient usage example

from aiobotocore.session import get_session
from types_aiobotocore_qapps.client import QAppsClient

session = get_session()
async with session.create_client("qapps") as client:
    client: QAppsClient
```

## Exceptions


`aiobotocore` client exceptions are generated in runtime.
This class provides code completion for `#!python session.create_client("qapps").exceptions` structure.

```python
# QAppsClient.exceptions usage example

async with session.create_client("qapps") as client:
    try:
        do_something(client)
    except (
            client.AccessDeniedException,
        client.ClientError,
        client.ConflictException,
        client.ContentTooLargeException,
        client.InternalServerException,
        client.ResourceNotFoundException,
        client.ServiceQuotaExceededException,
        client.ThrottlingException,
        client.UnauthorizedException,
        client.ValidationException,
    ) as e:
        print(e)
```

```python
# QAppsClient usage type checking example

from types_aiobotocore_qapps.client import Exceptions

def handle_error(exc: Exceptions.AccessDeniedException) -> None:
    ...
```


## Methods


### associate\_library\_item\_review

Associates a rating or review for a library item with the user submitting the
request.

Type annotations and code completion for `#!python session.create_client("qapps").associate_library_item_review` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/qapps.html#QApps.Client.associate_library_item_review)

```python
# associate_library_item_review method definition

await def associate_library_item_review(
    self,
    *,
    instanceId: str,
    libraryItemId: str,
) -> EmptyResponseMetadataTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef) 


```python
# associate_library_item_review method usage example with argument unpacking

kwargs: AssociateLibraryItemReviewInputRequestTypeDef = {  # (1)
    "instanceId": ...,
    "libraryItemId": ...,
}

parent.associate_library_item_review(**kwargs)
```

1. See [:material-code-braces: AssociateLibraryItemReviewInputRequestTypeDef](./type_defs.md#associatelibraryitemreviewinputrequesttypedef) 

### associate\_q\_app\_with\_user

This operation creates a link between the user's identity calling the operation
and a specific Q
App.

Type annotations and code completion for `#!python session.create_client("qapps").associate_q_app_with_user` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/qapps.html#QApps.Client.associate_q_app_with_user)

```python
# associate_q_app_with_user method definition

await def associate_q_app_with_user(
    self,
    *,
    instanceId: str,
    appId: str,
) -> EmptyResponseMetadataTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef) 


```python
# associate_q_app_with_user method usage example with argument unpacking

kwargs: AssociateQAppWithUserInputRequestTypeDef = {  # (1)
    "instanceId": ...,
    "appId": ...,
}

parent.associate_q_app_with_user(**kwargs)
```

1. See [:material-code-braces: AssociateQAppWithUserInputRequestTypeDef](./type_defs.md#associateqappwithuserinputrequesttypedef) 

### can\_paginate

Check if an operation can be paginated.

Type annotations and code completion for `#!python session.create_client("qapps").can_paginate` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/qapps.html#QApps.Client.can_paginate)

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

Type annotations and code completion for `#!python session.create_client("qapps").close` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/qapps.html#QApps.Client.close)

```python
# close method definition

await def close(
    self,
) -> None:
    ...
```


### create\_library\_item

Creates a new library item for an Amazon Q App, allowing it to be discovered
and used by other allowed
users.

Type annotations and code completion for `#!python session.create_client("qapps").create_library_item` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/qapps.html#QApps.Client.create_library_item)

```python
# create_library_item method definition

await def create_library_item(
    self,
    *,
    instanceId: str,
    appId: str,
    appVersion: int,
    categories: Sequence[str],
) -> CreateLibraryItemOutputTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: CreateLibraryItemOutputTypeDef](./type_defs.md#createlibraryitemoutputtypedef) 


```python
# create_library_item method usage example with argument unpacking

kwargs: CreateLibraryItemInputRequestTypeDef = {  # (1)
    "instanceId": ...,
    "appId": ...,
    "appVersion": ...,
    "categories": ...,
}

parent.create_library_item(**kwargs)
```

1. See [:material-code-braces: CreateLibraryItemInputRequestTypeDef](./type_defs.md#createlibraryiteminputrequesttypedef) 

### create\_q\_app

Creates a new Amazon Q App based on the provided definition.

Type annotations and code completion for `#!python session.create_client("qapps").create_q_app` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/qapps.html#QApps.Client.create_q_app)

```python
# create_q_app method definition

await def create_q_app(
    self,
    *,
    instanceId: str,
    title: str,
    appDefinition: AppDefinitionInputTypeDef,  # (1)
    description: str = ...,
    tags: Mapping[str, str] = ...,
) -> CreateQAppOutputTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: AppDefinitionInputTypeDef](./type_defs.md#appdefinitioninputtypedef) 
2. See [:material-code-braces: CreateQAppOutputTypeDef](./type_defs.md#createqappoutputtypedef) 


```python
# create_q_app method usage example with argument unpacking

kwargs: CreateQAppInputRequestTypeDef = {  # (1)
    "instanceId": ...,
    "title": ...,
    "appDefinition": ...,
}

parent.create_q_app(**kwargs)
```

1. See [:material-code-braces: CreateQAppInputRequestTypeDef](./type_defs.md#createqappinputrequesttypedef) 

### delete\_library\_item

Deletes a library item for an Amazon Q App, removing it from the library so it
can no longer be discovered or used by other
users.

Type annotations and code completion for `#!python session.create_client("qapps").delete_library_item` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/qapps.html#QApps.Client.delete_library_item)

```python
# delete_library_item method definition

await def delete_library_item(
    self,
    *,
    instanceId: str,
    libraryItemId: str,
) -> EmptyResponseMetadataTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef) 


```python
# delete_library_item method usage example with argument unpacking

kwargs: DeleteLibraryItemInputRequestTypeDef = {  # (1)
    "instanceId": ...,
    "libraryItemId": ...,
}

parent.delete_library_item(**kwargs)
```

1. See [:material-code-braces: DeleteLibraryItemInputRequestTypeDef](./type_defs.md#deletelibraryiteminputrequesttypedef) 

### delete\_q\_app

Deletes an Amazon Q App owned by the user.

Type annotations and code completion for `#!python session.create_client("qapps").delete_q_app` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/qapps.html#QApps.Client.delete_q_app)

```python
# delete_q_app method definition

await def delete_q_app(
    self,
    *,
    instanceId: str,
    appId: str,
) -> EmptyResponseMetadataTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef) 


```python
# delete_q_app method usage example with argument unpacking

kwargs: DeleteQAppInputRequestTypeDef = {  # (1)
    "instanceId": ...,
    "appId": ...,
}

parent.delete_q_app(**kwargs)
```

1. See [:material-code-braces: DeleteQAppInputRequestTypeDef](./type_defs.md#deleteqappinputrequesttypedef) 

### disassociate\_library\_item\_review

Removes a rating or review previously submitted by the user for a library item.

Type annotations and code completion for `#!python session.create_client("qapps").disassociate_library_item_review` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/qapps.html#QApps.Client.disassociate_library_item_review)

```python
# disassociate_library_item_review method definition

await def disassociate_library_item_review(
    self,
    *,
    instanceId: str,
    libraryItemId: str,
) -> EmptyResponseMetadataTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef) 


```python
# disassociate_library_item_review method usage example with argument unpacking

kwargs: DisassociateLibraryItemReviewInputRequestTypeDef = {  # (1)
    "instanceId": ...,
    "libraryItemId": ...,
}

parent.disassociate_library_item_review(**kwargs)
```

1. See [:material-code-braces: DisassociateLibraryItemReviewInputRequestTypeDef](./type_defs.md#disassociatelibraryitemreviewinputrequesttypedef) 

### disassociate\_q\_app\_from\_user

Disassociates a Q App from a user removing the user's access to run the Q App.

Type annotations and code completion for `#!python session.create_client("qapps").disassociate_q_app_from_user` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/qapps.html#QApps.Client.disassociate_q_app_from_user)

```python
# disassociate_q_app_from_user method definition

await def disassociate_q_app_from_user(
    self,
    *,
    instanceId: str,
    appId: str,
) -> EmptyResponseMetadataTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef) 


```python
# disassociate_q_app_from_user method usage example with argument unpacking

kwargs: DisassociateQAppFromUserInputRequestTypeDef = {  # (1)
    "instanceId": ...,
    "appId": ...,
}

parent.disassociate_q_app_from_user(**kwargs)
```

1. See [:material-code-braces: DisassociateQAppFromUserInputRequestTypeDef](./type_defs.md#disassociateqappfromuserinputrequesttypedef) 

### generate\_presigned\_url

Generate a presigned url given a client, its method, and arguments.

Type annotations and code completion for `#!python session.create_client("qapps").generate_presigned_url` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/qapps.html#QApps.Client.generate_presigned_url)

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


### get\_library\_item

Retrieves details about a library item for an Amazon Q App, including its
metadata, categories, ratings, and usage
statistics.

Type annotations and code completion for `#!python session.create_client("qapps").get_library_item` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/qapps.html#QApps.Client.get_library_item)

```python
# get_library_item method definition

await def get_library_item(
    self,
    *,
    instanceId: str,
    libraryItemId: str,
    appId: str = ...,
) -> GetLibraryItemOutputTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetLibraryItemOutputTypeDef](./type_defs.md#getlibraryitemoutputtypedef) 


```python
# get_library_item method usage example with argument unpacking

kwargs: GetLibraryItemInputRequestTypeDef = {  # (1)
    "instanceId": ...,
    "libraryItemId": ...,
}

parent.get_library_item(**kwargs)
```

1. See [:material-code-braces: GetLibraryItemInputRequestTypeDef](./type_defs.md#getlibraryiteminputrequesttypedef) 

### get\_q\_app

Retrieves the full details of an Q App, including its definition specifying the
cards and
flow.

Type annotations and code completion for `#!python session.create_client("qapps").get_q_app` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/qapps.html#QApps.Client.get_q_app)

```python
# get_q_app method definition

await def get_q_app(
    self,
    *,
    instanceId: str,
    appId: str,
) -> GetQAppOutputTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetQAppOutputTypeDef](./type_defs.md#getqappoutputtypedef) 


```python
# get_q_app method usage example with argument unpacking

kwargs: GetQAppInputRequestTypeDef = {  # (1)
    "instanceId": ...,
    "appId": ...,
}

parent.get_q_app(**kwargs)
```

1. See [:material-code-braces: GetQAppInputRequestTypeDef](./type_defs.md#getqappinputrequesttypedef) 

### get\_q\_app\_session

Retrieves the current state and results for an active session of an Amazon Q
App.

Type annotations and code completion for `#!python session.create_client("qapps").get_q_app_session` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/qapps.html#QApps.Client.get_q_app_session)

```python
# get_q_app_session method definition

await def get_q_app_session(
    self,
    *,
    instanceId: str,
    sessionId: str,
) -> GetQAppSessionOutputTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetQAppSessionOutputTypeDef](./type_defs.md#getqappsessionoutputtypedef) 


```python
# get_q_app_session method usage example with argument unpacking

kwargs: GetQAppSessionInputRequestTypeDef = {  # (1)
    "instanceId": ...,
    "sessionId": ...,
}

parent.get_q_app_session(**kwargs)
```

1. See [:material-code-braces: GetQAppSessionInputRequestTypeDef](./type_defs.md#getqappsessioninputrequesttypedef) 

### import\_document

Uploads a file that can then be used either as a default in a `FileUploadCard`
from Q App definition or as a file that is used inside a single Q App
run.

Type annotations and code completion for `#!python session.create_client("qapps").import_document` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/qapps.html#QApps.Client.import_document)

```python
# import_document method definition

await def import_document(
    self,
    *,
    instanceId: str,
    cardId: str,
    appId: str,
    fileContentsBase64: str,
    fileName: str,
    scope: DocumentScopeType,  # (1)
    sessionId: str = ...,
) -> ImportDocumentOutputTypeDef:  # (2)
    ...
```

1. See [:material-code-brackets: DocumentScopeType](./literals.md#documentscopetype) 
2. See [:material-code-braces: ImportDocumentOutputTypeDef](./type_defs.md#importdocumentoutputtypedef) 


```python
# import_document method usage example with argument unpacking

kwargs: ImportDocumentInputRequestTypeDef = {  # (1)
    "instanceId": ...,
    "cardId": ...,
    "appId": ...,
    "fileContentsBase64": ...,
    "fileName": ...,
    "scope": ...,
}

parent.import_document(**kwargs)
```

1. See [:material-code-braces: ImportDocumentInputRequestTypeDef](./type_defs.md#importdocumentinputrequesttypedef) 

### list\_library\_items

Lists the library items for Amazon Q Apps that are published and available for
users in your Amazon Web Services
account.

Type annotations and code completion for `#!python session.create_client("qapps").list_library_items` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/qapps.html#QApps.Client.list_library_items)

```python
# list_library_items method definition

await def list_library_items(
    self,
    *,
    instanceId: str,
    limit: int = ...,
    nextToken: str = ...,
    categoryId: str = ...,
) -> ListLibraryItemsOutputTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListLibraryItemsOutputTypeDef](./type_defs.md#listlibraryitemsoutputtypedef) 


```python
# list_library_items method usage example with argument unpacking

kwargs: ListLibraryItemsInputRequestTypeDef = {  # (1)
    "instanceId": ...,
}

parent.list_library_items(**kwargs)
```

1. See [:material-code-braces: ListLibraryItemsInputRequestTypeDef](./type_defs.md#listlibraryitemsinputrequesttypedef) 

### list\_q\_apps

Lists the Amazon Q Apps owned by or associated with the user either because
they created it or because they used it from the library in the
past.

Type annotations and code completion for `#!python session.create_client("qapps").list_q_apps` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/qapps.html#QApps.Client.list_q_apps)

```python
# list_q_apps method definition

await def list_q_apps(
    self,
    *,
    instanceId: str,
    limit: int = ...,
    nextToken: str = ...,
) -> ListQAppsOutputTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListQAppsOutputTypeDef](./type_defs.md#listqappsoutputtypedef) 


```python
# list_q_apps method usage example with argument unpacking

kwargs: ListQAppsInputRequestTypeDef = {  # (1)
    "instanceId": ...,
}

parent.list_q_apps(**kwargs)
```

1. See [:material-code-braces: ListQAppsInputRequestTypeDef](./type_defs.md#listqappsinputrequesttypedef) 

### list\_tags\_for\_resource

Lists the tags associated with an Amazon Q Apps resource.

Type annotations and code completion for `#!python session.create_client("qapps").list_tags_for_resource` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/qapps.html#QApps.Client.list_tags_for_resource)

```python
# list_tags_for_resource method definition

await def list_tags_for_resource(
    self,
    *,
    resourceARN: str,
) -> ListTagsForResourceResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListTagsForResourceResponseTypeDef](./type_defs.md#listtagsforresourceresponsetypedef) 


```python
# list_tags_for_resource method usage example with argument unpacking

kwargs: ListTagsForResourceRequestRequestTypeDef = {  # (1)
    "resourceARN": ...,
}

parent.list_tags_for_resource(**kwargs)
```

1. See [:material-code-braces: ListTagsForResourceRequestRequestTypeDef](./type_defs.md#listtagsforresourcerequestrequesttypedef) 

### predict\_q\_app

Generates an Amazon Q App definition based on either a conversation or a
problem statement provided as input.The resulting app definition can be used to
call
`CreateQApp`.

Type annotations and code completion for `#!python session.create_client("qapps").predict_q_app` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/qapps.html#QApps.Client.predict_q_app)

```python
# predict_q_app method definition

await def predict_q_app(
    self,
    *,
    instanceId: str,
    options: PredictQAppInputOptionsTypeDef = ...,  # (1)
) -> PredictQAppOutputTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: PredictQAppInputOptionsTypeDef](./type_defs.md#predictqappinputoptionstypedef) 
2. See [:material-code-braces: PredictQAppOutputTypeDef](./type_defs.md#predictqappoutputtypedef) 


```python
# predict_q_app method usage example with argument unpacking

kwargs: PredictQAppInputRequestTypeDef = {  # (1)
    "instanceId": ...,
}

parent.predict_q_app(**kwargs)
```

1. See [:material-code-braces: PredictQAppInputRequestTypeDef](./type_defs.md#predictqappinputrequesttypedef) 

### start\_q\_app\_session

Starts a new session for an Amazon Q App, allowing inputs to be provided and
the app to be
run.

Type annotations and code completion for `#!python session.create_client("qapps").start_q_app_session` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/qapps.html#QApps.Client.start_q_app_session)

```python
# start_q_app_session method definition

await def start_q_app_session(
    self,
    *,
    instanceId: str,
    appId: str,
    appVersion: int,
    initialValues: Sequence[CardValueTypeDef] = ...,  # (1)
    tags: Mapping[str, str] = ...,
) -> StartQAppSessionOutputTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: CardValueTypeDef](./type_defs.md#cardvaluetypedef) 
2. See [:material-code-braces: StartQAppSessionOutputTypeDef](./type_defs.md#startqappsessionoutputtypedef) 


```python
# start_q_app_session method usage example with argument unpacking

kwargs: StartQAppSessionInputRequestTypeDef = {  # (1)
    "instanceId": ...,
    "appId": ...,
    "appVersion": ...,
}

parent.start_q_app_session(**kwargs)
```

1. See [:material-code-braces: StartQAppSessionInputRequestTypeDef](./type_defs.md#startqappsessioninputrequesttypedef) 

### stop\_q\_app\_session

Stops an active session for an Amazon Q App.This deletes all data related to
the session and makes it invalid for future
uses.

Type annotations and code completion for `#!python session.create_client("qapps").stop_q_app_session` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/qapps.html#QApps.Client.stop_q_app_session)

```python
# stop_q_app_session method definition

await def stop_q_app_session(
    self,
    *,
    instanceId: str,
    sessionId: str,
) -> EmptyResponseMetadataTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef) 


```python
# stop_q_app_session method usage example with argument unpacking

kwargs: StopQAppSessionInputRequestTypeDef = {  # (1)
    "instanceId": ...,
    "sessionId": ...,
}

parent.stop_q_app_session(**kwargs)
```

1. See [:material-code-braces: StopQAppSessionInputRequestTypeDef](./type_defs.md#stopqappsessioninputrequesttypedef) 

### tag\_resource

Associates tags with an Amazon Q Apps resource.

Type annotations and code completion for `#!python session.create_client("qapps").tag_resource` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/qapps.html#QApps.Client.tag_resource)

```python
# tag_resource method definition

await def tag_resource(
    self,
    *,
    resourceARN: str,
    tags: Mapping[str, str],
) -> Dict[str, Any]:
    ...
```



```python
# tag_resource method usage example with argument unpacking

kwargs: TagResourceRequestRequestTypeDef = {  # (1)
    "resourceARN": ...,
    "tags": ...,
}

parent.tag_resource(**kwargs)
```

1. See [:material-code-braces: TagResourceRequestRequestTypeDef](./type_defs.md#tagresourcerequestrequesttypedef) 

### untag\_resource

Disassociates tags from an Amazon Q Apps resource.

Type annotations and code completion for `#!python session.create_client("qapps").untag_resource` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/qapps.html#QApps.Client.untag_resource)

```python
# untag_resource method definition

await def untag_resource(
    self,
    *,
    resourceARN: str,
    tagKeys: Sequence[str],
) -> Dict[str, Any]:
    ...
```



```python
# untag_resource method usage example with argument unpacking

kwargs: UntagResourceRequestRequestTypeDef = {  # (1)
    "resourceARN": ...,
    "tagKeys": ...,
}

parent.untag_resource(**kwargs)
```

1. See [:material-code-braces: UntagResourceRequestRequestTypeDef](./type_defs.md#untagresourcerequestrequesttypedef) 

### update\_library\_item

Updates the library item for an Amazon Q App.

Type annotations and code completion for `#!python session.create_client("qapps").update_library_item` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/qapps.html#QApps.Client.update_library_item)

```python
# update_library_item method definition

await def update_library_item(
    self,
    *,
    instanceId: str,
    libraryItemId: str,
    status: LibraryItemStatusType = ...,  # (1)
    categories: Sequence[str] = ...,
) -> UpdateLibraryItemOutputTypeDef:  # (2)
    ...
```

1. See [:material-code-brackets: LibraryItemStatusType](./literals.md#libraryitemstatustype) 
2. See [:material-code-braces: UpdateLibraryItemOutputTypeDef](./type_defs.md#updatelibraryitemoutputtypedef) 


```python
# update_library_item method usage example with argument unpacking

kwargs: UpdateLibraryItemInputRequestTypeDef = {  # (1)
    "instanceId": ...,
    "libraryItemId": ...,
}

parent.update_library_item(**kwargs)
```

1. See [:material-code-braces: UpdateLibraryItemInputRequestTypeDef](./type_defs.md#updatelibraryiteminputrequesttypedef) 

### update\_library\_item\_metadata

Updates the verification status of a library item for an Amazon Q App.

Type annotations and code completion for `#!python session.create_client("qapps").update_library_item_metadata` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/qapps.html#QApps.Client.update_library_item_metadata)

```python
# update_library_item_metadata method definition

await def update_library_item_metadata(
    self,
    *,
    instanceId: str,
    libraryItemId: str,
    isVerified: bool = ...,
) -> EmptyResponseMetadataTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef) 


```python
# update_library_item_metadata method usage example with argument unpacking

kwargs: UpdateLibraryItemMetadataInputRequestTypeDef = {  # (1)
    "instanceId": ...,
    "libraryItemId": ...,
}

parent.update_library_item_metadata(**kwargs)
```

1. See [:material-code-braces: UpdateLibraryItemMetadataInputRequestTypeDef](./type_defs.md#updatelibraryitemmetadatainputrequesttypedef) 

### update\_q\_app

Updates an existing Amazon Q App, allowing modifications to its title,
description, and
definition.

Type annotations and code completion for `#!python session.create_client("qapps").update_q_app` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/qapps.html#QApps.Client.update_q_app)

```python
# update_q_app method definition

await def update_q_app(
    self,
    *,
    instanceId: str,
    appId: str,
    title: str = ...,
    description: str = ...,
    appDefinition: AppDefinitionInputTypeDef = ...,  # (1)
) -> UpdateQAppOutputTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: AppDefinitionInputTypeDef](./type_defs.md#appdefinitioninputtypedef) 
2. See [:material-code-braces: UpdateQAppOutputTypeDef](./type_defs.md#updateqappoutputtypedef) 


```python
# update_q_app method usage example with argument unpacking

kwargs: UpdateQAppInputRequestTypeDef = {  # (1)
    "instanceId": ...,
    "appId": ...,
}

parent.update_q_app(**kwargs)
```

1. See [:material-code-braces: UpdateQAppInputRequestTypeDef](./type_defs.md#updateqappinputrequesttypedef) 

### update\_q\_app\_session

Updates the session for a given Q App `sessionId`.

Type annotations and code completion for `#!python session.create_client("qapps").update_q_app_session` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/qapps.html#QApps.Client.update_q_app_session)

```python
# update_q_app_session method definition

await def update_q_app_session(
    self,
    *,
    instanceId: str,
    sessionId: str,
    values: Sequence[CardValueTypeDef] = ...,  # (1)
) -> UpdateQAppSessionOutputTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: CardValueTypeDef](./type_defs.md#cardvaluetypedef) 
2. See [:material-code-braces: UpdateQAppSessionOutputTypeDef](./type_defs.md#updateqappsessionoutputtypedef) 


```python
# update_q_app_session method usage example with argument unpacking

kwargs: UpdateQAppSessionInputRequestTypeDef = {  # (1)
    "instanceId": ...,
    "sessionId": ...,
}

parent.update_q_app_session(**kwargs)
```

1. See [:material-code-braces: UpdateQAppSessionInputRequestTypeDef](./type_defs.md#updateqappsessioninputrequesttypedef) 

### \_\_aenter\_\_



Type annotations and code completion for `#!python session.create_client("qapps").__aenter__` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/qapps.html#QApps.Client.__aenter__)

```python
# __aenter__ method definition

await def __aenter__(
    self,
) -> "QAppsClient":
    ...
```


### \_\_aexit\_\_



Type annotations and code completion for `#!python session.create_client("qapps").__aexit__` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/qapps.html#QApps.Client.__aexit__)

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

Type annotations and code completion for `#!python session.create_client("qapps").get_paginator` method with overloads.

- `client.get_paginator("list_library_items")` -> [ListLibraryItemsPaginator](./paginators.md#listlibraryitemspaginator)
- `client.get_paginator("list_q_apps")` -> [ListQAppsPaginator](./paginators.md#listqappspaginator)



