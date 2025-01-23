# QAppsClient

> [Index](../README.md) > [QApps](./README.md) > QAppsClient

!!! note ""

    Auto-generated documentation for [QApps](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/qapps.html#qapps)
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


### can\_paginate



Type annotations and code completion for `#!python session.create_client("qapps").can_paginate` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/qapps/client/can_paginate.html)

```python
# can_paginate method definition

def can_paginate(
    self,
    operation_name: str,
) -> bool:
    ...
```


### generate\_presigned\_url



Type annotations and code completion for `#!python session.create_client("qapps").generate_presigned_url` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/qapps/client/generate_presigned_url.html)

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


### associate\_library\_item\_review

Associates a rating or review for a library item with the user submitting the
request.

Type annotations and code completion for `#!python session.create_client("qapps").associate_library_item_review` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/qapps/client/associate_library_item_review.html)

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
and a specific Q App.

Type annotations and code completion for `#!python session.create_client("qapps").associate_q_app_with_user` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/qapps/client/associate_q_app_with_user.html)

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

### batch\_create\_category

Creates Categories for the Amazon Q Business application environment instance.

Type annotations and code completion for `#!python session.create_client("qapps").batch_create_category` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/qapps/client/batch_create_category.html)

```python
# batch_create_category method definition

await def batch_create_category(
    self,
    *,
    instanceId: str,
    categories: Sequence[BatchCreateCategoryInputCategoryTypeDef],  # (1)
) -> EmptyResponseMetadataTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: BatchCreateCategoryInputCategoryTypeDef](./type_defs.md#batchcreatecategoryinputcategorytypedef) 
2. See [:material-code-braces: EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef) 


```python
# batch_create_category method usage example with argument unpacking

kwargs: BatchCreateCategoryInputRequestTypeDef = {  # (1)
    "instanceId": ...,
    "categories": ...,
}

parent.batch_create_category(**kwargs)
```

1. See [:material-code-braces: BatchCreateCategoryInputRequestTypeDef](./type_defs.md#batchcreatecategoryinputrequesttypedef) 

### batch\_delete\_category

Deletes Categories for the Amazon Q Business application environment instance.

Type annotations and code completion for `#!python session.create_client("qapps").batch_delete_category` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/qapps/client/batch_delete_category.html)

```python
# batch_delete_category method definition

await def batch_delete_category(
    self,
    *,
    instanceId: str,
    categories: Sequence[str],
) -> EmptyResponseMetadataTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef) 


```python
# batch_delete_category method usage example with argument unpacking

kwargs: BatchDeleteCategoryInputRequestTypeDef = {  # (1)
    "instanceId": ...,
    "categories": ...,
}

parent.batch_delete_category(**kwargs)
```

1. See [:material-code-braces: BatchDeleteCategoryInputRequestTypeDef](./type_defs.md#batchdeletecategoryinputrequesttypedef) 

### batch\_update\_category

Updates Categories for the Amazon Q Business application environment instance.

Type annotations and code completion for `#!python session.create_client("qapps").batch_update_category` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/qapps/client/batch_update_category.html)

```python
# batch_update_category method definition

await def batch_update_category(
    self,
    *,
    instanceId: str,
    categories: Sequence[CategoryInputTypeDef],  # (1)
) -> EmptyResponseMetadataTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: CategoryInputTypeDef](./type_defs.md#categoryinputtypedef) 
2. See [:material-code-braces: EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef) 


```python
# batch_update_category method usage example with argument unpacking

kwargs: BatchUpdateCategoryInputRequestTypeDef = {  # (1)
    "instanceId": ...,
    "categories": ...,
}

parent.batch_update_category(**kwargs)
```

1. See [:material-code-braces: BatchUpdateCategoryInputRequestTypeDef](./type_defs.md#batchupdatecategoryinputrequesttypedef) 

### create\_library\_item

Creates a new library item for an Amazon Q App, allowing it to be discovered
and used by other allowed users.

Type annotations and code completion for `#!python session.create_client("qapps").create_library_item` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/qapps/client/create_library_item.html)

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

### create\_presigned\_url

Creates a presigned URL for an S3 POST operation to upload a file.

Type annotations and code completion for `#!python session.create_client("qapps").create_presigned_url` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/qapps/client/create_presigned_url.html)

```python
# create_presigned_url method definition

await def create_presigned_url(
    self,
    *,
    instanceId: str,
    cardId: str,
    appId: str,
    fileContentsSha256: str,
    fileName: str,
    scope: DocumentScopeType,  # (1)
    sessionId: str = ...,
) -> CreatePresignedUrlOutputTypeDef:  # (2)
    ...
```

1. See [:material-code-brackets: DocumentScopeType](./literals.md#documentscopetype) 
2. See [:material-code-braces: CreatePresignedUrlOutputTypeDef](./type_defs.md#createpresignedurloutputtypedef) 


```python
# create_presigned_url method usage example with argument unpacking

kwargs: CreatePresignedUrlInputRequestTypeDef = {  # (1)
    "instanceId": ...,
    "cardId": ...,
    "appId": ...,
    "fileContentsSha256": ...,
    "fileName": ...,
    "scope": ...,
}

parent.create_presigned_url(**kwargs)
```

1. See [:material-code-braces: CreatePresignedUrlInputRequestTypeDef](./type_defs.md#createpresignedurlinputrequesttypedef) 

### create\_q\_app

Creates a new Amazon Q App based on the provided definition.

Type annotations and code completion for `#!python session.create_client("qapps").create_q_app` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/qapps/client/create_q_app.html)

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
can no longer be discovered or used by other users.

Type annotations and code completion for `#!python session.create_client("qapps").delete_library_item` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/qapps/client/delete_library_item.html)

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
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/qapps/client/delete_q_app.html)

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

### describe\_q\_app\_permissions

Describes read permissions for a Amazon Q App in Amazon Q Business application
environment instance.

Type annotations and code completion for `#!python session.create_client("qapps").describe_q_app_permissions` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/qapps/client/describe_q_app_permissions.html)

```python
# describe_q_app_permissions method definition

await def describe_q_app_permissions(
    self,
    *,
    instanceId: str,
    appId: str,
) -> DescribeQAppPermissionsOutputTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DescribeQAppPermissionsOutputTypeDef](./type_defs.md#describeqapppermissionsoutputtypedef) 


```python
# describe_q_app_permissions method usage example with argument unpacking

kwargs: DescribeQAppPermissionsInputRequestTypeDef = {  # (1)
    "instanceId": ...,
    "appId": ...,
}

parent.describe_q_app_permissions(**kwargs)
```

1. See [:material-code-braces: DescribeQAppPermissionsInputRequestTypeDef](./type_defs.md#describeqapppermissionsinputrequesttypedef) 

### disassociate\_library\_item\_review

Removes a rating or review previously submitted by the user for a library item.

Type annotations and code completion for `#!python session.create_client("qapps").disassociate_library_item_review` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/qapps/client/disassociate_library_item_review.html)

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
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/qapps/client/disassociate_q_app_from_user.html)

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

### export\_q\_app\_session\_data

Exports the collected data of a Q App data collection session.

Type annotations and code completion for `#!python session.create_client("qapps").export_q_app_session_data` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/qapps/client/export_q_app_session_data.html)

```python
# export_q_app_session_data method definition

await def export_q_app_session_data(
    self,
    *,
    instanceId: str,
    sessionId: str,
) -> ExportQAppSessionDataOutputTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ExportQAppSessionDataOutputTypeDef](./type_defs.md#exportqappsessiondataoutputtypedef) 


```python
# export_q_app_session_data method usage example with argument unpacking

kwargs: ExportQAppSessionDataInputRequestTypeDef = {  # (1)
    "instanceId": ...,
    "sessionId": ...,
}

parent.export_q_app_session_data(**kwargs)
```

1. See [:material-code-braces: ExportQAppSessionDataInputRequestTypeDef](./type_defs.md#exportqappsessiondatainputrequesttypedef) 

### get\_library\_item

Retrieves details about a library item for an Amazon Q App, including its
metadata, categories, ratings, and usage statistics.

Type annotations and code completion for `#!python session.create_client("qapps").get_library_item` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/qapps/client/get_library_item.html)

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
cards and flow.

Type annotations and code completion for `#!python session.create_client("qapps").get_q_app` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/qapps/client/get_q_app.html)

```python
# get_q_app method definition

await def get_q_app(
    self,
    *,
    instanceId: str,
    appId: str,
    appVersion: int = ...,
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
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/qapps/client/get_q_app_session.html)

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

### get\_q\_app\_session\_metadata

Retrieves the current configuration of a Q App session.

Type annotations and code completion for `#!python session.create_client("qapps").get_q_app_session_metadata` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/qapps/client/get_q_app_session_metadata.html)

```python
# get_q_app_session_metadata method definition

await def get_q_app_session_metadata(
    self,
    *,
    instanceId: str,
    sessionId: str,
) -> GetQAppSessionMetadataOutputTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetQAppSessionMetadataOutputTypeDef](./type_defs.md#getqappsessionmetadataoutputtypedef) 


```python
# get_q_app_session_metadata method usage example with argument unpacking

kwargs: GetQAppSessionMetadataInputRequestTypeDef = {  # (1)
    "instanceId": ...,
    "sessionId": ...,
}

parent.get_q_app_session_metadata(**kwargs)
```

1. See [:material-code-braces: GetQAppSessionMetadataInputRequestTypeDef](./type_defs.md#getqappsessionmetadatainputrequesttypedef) 

### import\_document

Uploads a file that can then be used either as a default in a
<code>FileUploadCard</code> from Q App definition or as a file that is used
inside a single Q App run.

Type annotations and code completion for `#!python session.create_client("qapps").import_document` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/qapps/client/import_document.html)

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

### list\_categories

Lists the categories of a Amazon Q Business application environment instance.

Type annotations and code completion for `#!python session.create_client("qapps").list_categories` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/qapps/client/list_categories.html)

```python
# list_categories method definition

await def list_categories(
    self,
    *,
    instanceId: str,
) -> ListCategoriesOutputTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListCategoriesOutputTypeDef](./type_defs.md#listcategoriesoutputtypedef) 


```python
# list_categories method usage example with argument unpacking

kwargs: ListCategoriesInputRequestTypeDef = {  # (1)
    "instanceId": ...,
}

parent.list_categories(**kwargs)
```

1. See [:material-code-braces: ListCategoriesInputRequestTypeDef](./type_defs.md#listcategoriesinputrequesttypedef) 

### list\_library\_items

Lists the library items for Amazon Q Apps that are published and available for
users in your Amazon Web Services account.

Type annotations and code completion for `#!python session.create_client("qapps").list_library_items` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/qapps/client/list_library_items.html)

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

### list\_q\_app\_session\_data

Lists the collected data of a Q App data collection session.

Type annotations and code completion for `#!python session.create_client("qapps").list_q_app_session_data` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/qapps/client/list_q_app_session_data.html)

```python
# list_q_app_session_data method definition

await def list_q_app_session_data(
    self,
    *,
    instanceId: str,
    sessionId: str,
) -> ListQAppSessionDataOutputTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListQAppSessionDataOutputTypeDef](./type_defs.md#listqappsessiondataoutputtypedef) 


```python
# list_q_app_session_data method usage example with argument unpacking

kwargs: ListQAppSessionDataInputRequestTypeDef = {  # (1)
    "instanceId": ...,
    "sessionId": ...,
}

parent.list_q_app_session_data(**kwargs)
```

1. See [:material-code-braces: ListQAppSessionDataInputRequestTypeDef](./type_defs.md#listqappsessiondatainputrequesttypedef) 

### list\_q\_apps

Lists the Amazon Q Apps owned by or associated with the user either because
they created it or because they used it from the library in the past.

Type annotations and code completion for `#!python session.create_client("qapps").list_q_apps` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/qapps/client/list_q_apps.html)

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
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/qapps/client/list_tags_for_resource.html)

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
call <code>CreateQApp</code>.

Type annotations and code completion for `#!python session.create_client("qapps").predict_q_app` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/qapps/client/predict_q_app.html)

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
the app to be run.

Type annotations and code completion for `#!python session.create_client("qapps").start_q_app_session` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/qapps/client/start_q_app_session.html)

```python
# start_q_app_session method definition

await def start_q_app_session(
    self,
    *,
    instanceId: str,
    appId: str,
    appVersion: int,
    initialValues: Sequence[CardValueTypeDef] = ...,  # (1)
    sessionId: str = ...,
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
the session and makes it invalid for future uses.

Type annotations and code completion for `#!python session.create_client("qapps").stop_q_app_session` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/qapps/client/stop_q_app_session.html)

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
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/qapps/client/tag_resource.html)

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
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/qapps/client/untag_resource.html)

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
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/qapps/client/update_library_item.html)

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
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/qapps/client/update_library_item_metadata.html)

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
description, and definition.

Type annotations and code completion for `#!python session.create_client("qapps").update_q_app` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/qapps/client/update_q_app.html)

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

### update\_q\_app\_permissions

Updates read permissions for a Amazon Q App in Amazon Q Business application
environment instance.

Type annotations and code completion for `#!python session.create_client("qapps").update_q_app_permissions` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/qapps/client/update_q_app_permissions.html)

```python
# update_q_app_permissions method definition

await def update_q_app_permissions(
    self,
    *,
    instanceId: str,
    appId: str,
    grantPermissions: Sequence[PermissionInputTypeDef] = ...,  # (1)
    revokePermissions: Sequence[PermissionInputTypeDef] = ...,  # (1)
) -> UpdateQAppPermissionsOutputTypeDef:  # (3)
    ...
```

1. See [:material-code-braces: PermissionInputTypeDef](./type_defs.md#permissioninputtypedef) 
2. See [:material-code-braces: PermissionInputTypeDef](./type_defs.md#permissioninputtypedef) 
3. See [:material-code-braces: UpdateQAppPermissionsOutputTypeDef](./type_defs.md#updateqapppermissionsoutputtypedef) 


```python
# update_q_app_permissions method usage example with argument unpacking

kwargs: UpdateQAppPermissionsInputRequestTypeDef = {  # (1)
    "instanceId": ...,
    "appId": ...,
}

parent.update_q_app_permissions(**kwargs)
```

1. See [:material-code-braces: UpdateQAppPermissionsInputRequestTypeDef](./type_defs.md#updateqapppermissionsinputrequesttypedef) 

### update\_q\_app\_session

Updates the session for a given Q App <code>sessionId</code>.

Type annotations and code completion for `#!python session.create_client("qapps").update_q_app_session` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/qapps/client/update_q_app_session.html)

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

### update\_q\_app\_session\_metadata

Updates the configuration metadata of a session for a given Q App
<code>sessionId</code>.

Type annotations and code completion for `#!python session.create_client("qapps").update_q_app_session_metadata` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/qapps/client/update_q_app_session_metadata.html)

```python
# update_q_app_session_metadata method definition

await def update_q_app_session_metadata(
    self,
    *,
    instanceId: str,
    sessionId: str,
    sharingConfiguration: SessionSharingConfigurationTypeDef,  # (1)
    sessionName: str = ...,
) -> UpdateQAppSessionMetadataOutputTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: SessionSharingConfigurationTypeDef](./type_defs.md#sessionsharingconfigurationtypedef) 
2. See [:material-code-braces: UpdateQAppSessionMetadataOutputTypeDef](./type_defs.md#updateqappsessionmetadataoutputtypedef) 


```python
# update_q_app_session_metadata method usage example with argument unpacking

kwargs: UpdateQAppSessionMetadataInputRequestTypeDef = {  # (1)
    "instanceId": ...,
    "sessionId": ...,
    "sharingConfiguration": ...,
}

parent.update_q_app_session_metadata(**kwargs)
```

1. See [:material-code-braces: UpdateQAppSessionMetadataInputRequestTypeDef](./type_defs.md#updateqappsessionmetadatainputrequesttypedef) 

### \_\_aenter\_\_



Type annotations and code completion for `#!python session.create_client("qapps").__aenter__` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/qapps.html#QApps.Client)

```python
# __aenter__ method definition

await def __aenter__(
    self,
) -> Self:
    ...
```


### \_\_aexit\_\_



Type annotations and code completion for `#!python session.create_client("qapps").__aexit__` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/qapps.html#QApps.Client)

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

Type annotations and code completion for `#!python session.create_client("qapps").get_paginator` method with overloads.

- `client.get_paginator("list_library_items")` -> [ListLibraryItemsPaginator](./paginators.md#listlibraryitemspaginator)
- `client.get_paginator("list_q_apps")` -> [ListQAppsPaginator](./paginators.md#listqappspaginator)



