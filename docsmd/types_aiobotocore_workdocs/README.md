# WorkDocs module

> [Index](../README.md) > WorkDocs


!!! note ""

    Auto-generated documentation for [WorkDocs](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workdocs.html#workdocs)
    type annotations stubs module [types-aiobotocore-workdocs](https://pypi.org/project/types-aiobotocore-workdocs/).

## How to install

### Generate locally (recommended)

You can generate type annotations for `aiobotocore` package locally with `mypy_boto3_builder`.
Use [uv](https://docs.astral.sh/uv/getting-started/installation/) for build isolation.

1. Run mypy-boto3-builder in your package root directory: `uvx --with 'aiobotocore==2.19.0' mypy_boto3_builder`
1. Select `aiobotocore` AWS SDK.
1. Add `WorkDocs` service.
1. Use provided commands to install generated packages.



### From PyPI with pip

Install `types-aiobotocore` for `WorkDocs` service.

```bash
# install with aiobotocore type annotations
python -m pip install 'types-aiobotocore[workdocs]'

# Lite version does not provide session.client/resource overloads
# it is more RAM-friendly, but requires explicit type annotations
python -m pip install 'types-aiobotocore-lite[workdocs]'

# standalone installation
python -m pip install types-aiobotocore-workdocs
```



## How to uninstall

```bash
python -m pip uninstall -y types-aiobotocore-workdocs
```

## Usage

Code samples can be found in [Examples](./usage.md).

## WorkDocsClient

Type annotations and code completion for  `#!python session.create_client("workdocs")` as [WorkDocsClient](./client.md)
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workdocs.html#WorkDocs.Client)

```python
# WorkDocsClient usage example

from aiobotocore.session import get_session

from types_aiobotocore_workdocs.client import WorkDocsClient


session = get_session()
async with session.create_client("workdocs") as client:
    client: WorkDocsClient
```


## Paginators

Type annotations and code completion for
[paginators](./paginators.md)
from `#!python session.create_client("workdocs").get_paginator("...")`.

```python
# DescribeActivitiesPaginator usage example

from types_aiobotocore_workdocs.paginator import DescribeActivitiesPaginator

def get_describe_activities_paginator() -> DescribeActivitiesPaginator:
    return client.get_paginator("describe_activities"))
```

- [DescribeActivitiesPaginator](./paginators.md#describeactivitiespaginator)
- [DescribeCommentsPaginator](./paginators.md#describecommentspaginator)
- [DescribeDocumentVersionsPaginator](./paginators.md#describedocumentversionspaginator)
- [DescribeFolderContentsPaginator](./paginators.md#describefoldercontentspaginator)
- [DescribeGroupsPaginator](./paginators.md#describegroupspaginator)
- [DescribeNotificationSubscriptionsPaginator](./paginators.md#describenotificationsubscriptionspaginator)
- [DescribeResourcePermissionsPaginator](./paginators.md#describeresourcepermissionspaginator)
- [DescribeRootFoldersPaginator](./paginators.md#describerootfolderspaginator)
- [DescribeUsersPaginator](./paginators.md#describeuserspaginator)
- [SearchResourcesPaginator](./paginators.md#searchresourcespaginator)








## Literals

Type annotations for [literals](./literals.md) used in methods and schema.

```python
# ActivityTypeType usage example

from types_aiobotocore_workdocs.literals import ActivityTypeType

def get_value() -> ActivityTypeType:
    return "DOCUMENT_ANNOTATION_ADDED"
```

- [ActivityTypeType](./literals.md#activitytypetype)
- [AdditionalResponseFieldTypeType](./literals.md#additionalresponsefieldtypetype)
- [BooleanEnumTypeType](./literals.md#booleanenumtypetype)
- [CommentStatusTypeType](./literals.md#commentstatustypetype)
- [CommentVisibilityTypeType](./literals.md#commentvisibilitytypetype)
- [ContentCategoryTypeType](./literals.md#contentcategorytypetype)
- [DescribeActivitiesPaginatorName](./literals.md#describeactivitiespaginatorname)
- [DescribeCommentsPaginatorName](./literals.md#describecommentspaginatorname)
- [DescribeDocumentVersionsPaginatorName](./literals.md#describedocumentversionspaginatorname)
- [DescribeFolderContentsPaginatorName](./literals.md#describefoldercontentspaginatorname)
- [DescribeGroupsPaginatorName](./literals.md#describegroupspaginatorname)
- [DescribeNotificationSubscriptionsPaginatorName](./literals.md#describenotificationsubscriptionspaginatorname)
- [DescribeResourcePermissionsPaginatorName](./literals.md#describeresourcepermissionspaginatorname)
- [DescribeRootFoldersPaginatorName](./literals.md#describerootfolderspaginatorname)
- [DescribeUsersPaginatorName](./literals.md#describeuserspaginatorname)
- [DocumentSourceTypeType](./literals.md#documentsourcetypetype)
- [DocumentStatusTypeType](./literals.md#documentstatustypetype)
- [DocumentThumbnailTypeType](./literals.md#documentthumbnailtypetype)
- [DocumentVersionStatusType](./literals.md#documentversionstatustype)
- [FolderContentTypeType](./literals.md#foldercontenttypetype)
- [LanguageCodeTypeType](./literals.md#languagecodetypetype)
- [LocaleTypeType](./literals.md#localetypetype)
- [OrderByFieldTypeType](./literals.md#orderbyfieldtypetype)
- [OrderTypeType](./literals.md#ordertypetype)
- [PrincipalRoleTypeType](./literals.md#principalroletypetype)
- [PrincipalTypeType](./literals.md#principaltypetype)
- [ResourceCollectionTypeType](./literals.md#resourcecollectiontypetype)
- [ResourceSortTypeType](./literals.md#resourcesorttypetype)
- [ResourceStateTypeType](./literals.md#resourcestatetypetype)
- [ResourceTypeType](./literals.md#resourcetypetype)
- [ResponseItemTypeType](./literals.md#responseitemtypetype)
- [RolePermissionTypeType](./literals.md#rolepermissiontypetype)
- [RoleTypeType](./literals.md#roletypetype)
- [SearchCollectionTypeType](./literals.md#searchcollectiontypetype)
- [SearchQueryScopeTypeType](./literals.md#searchqueryscopetypetype)
- [SearchResourceTypeType](./literals.md#searchresourcetypetype)
- [SearchResourcesPaginatorName](./literals.md#searchresourcespaginatorname)
- [ShareStatusTypeType](./literals.md#sharestatustypetype)
- [SortOrderType](./literals.md#sortordertype)
- [StorageTypeType](./literals.md#storagetypetype)
- [SubscriptionProtocolTypeType](./literals.md#subscriptionprotocoltypetype)
- [SubscriptionTypeType](./literals.md#subscriptiontypetype)
- [UserFilterTypeType](./literals.md#userfiltertypetype)
- [UserSortTypeType](./literals.md#usersorttypetype)
- [UserStatusTypeType](./literals.md#userstatustypetype)
- [UserTypeType](./literals.md#usertypetype)
- [WorkDocsServiceName](./literals.md#workdocsservicename)
- [ServiceName](./literals.md#servicename)
- [ResourceServiceName](./literals.md#resourceservicename)
- [PaginatorName](./literals.md#paginatorname)
- [RegionName](./literals.md#regionname)




## Type definitions

Type annotations for [type definitions](./type_defs.md) used in methods and schema.

- [AbortDocumentVersionUploadRequestRequestTypeDef](./type_defs.md#abortdocumentversionuploadrequestrequesttypedef)
- [ActivateUserRequestRequestTypeDef](./type_defs.md#activateuserrequestrequesttypedef)
- [ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef)
- [UserMetadataTypeDef](./type_defs.md#usermetadatatypedef)
- [NotificationOptionsTypeDef](./type_defs.md#notificationoptionstypedef)
- [SharePrincipalTypeDef](./type_defs.md#shareprincipaltypedef)
- [ShareResultTypeDef](./type_defs.md#shareresulttypedef)
- [CreateCommentRequestRequestTypeDef](./type_defs.md#createcommentrequestrequesttypedef)
- [CreateCustomMetadataRequestRequestTypeDef](./type_defs.md#createcustommetadatarequestrequesttypedef)
- [CreateFolderRequestRequestTypeDef](./type_defs.md#createfolderrequestrequesttypedef)
- [FolderMetadataTypeDef](./type_defs.md#foldermetadatatypedef)
- [CreateLabelsRequestRequestTypeDef](./type_defs.md#createlabelsrequestrequesttypedef)
- [CreateNotificationSubscriptionRequestRequestTypeDef](./type_defs.md#createnotificationsubscriptionrequestrequesttypedef)
- [SubscriptionTypeDef](./type_defs.md#subscriptiontypedef)
- [StorageRuleTypeTypeDef](./type_defs.md#storageruletypetypedef)
- [TimestampTypeDef](./type_defs.md#timestamptypedef)
- [DeactivateUserRequestRequestTypeDef](./type_defs.md#deactivateuserrequestrequesttypedef)
- [DeleteCommentRequestRequestTypeDef](./type_defs.md#deletecommentrequestrequesttypedef)
- [DeleteCustomMetadataRequestRequestTypeDef](./type_defs.md#deletecustommetadatarequestrequesttypedef)
- [DeleteDocumentRequestRequestTypeDef](./type_defs.md#deletedocumentrequestrequesttypedef)
- [DeleteDocumentVersionRequestRequestTypeDef](./type_defs.md#deletedocumentversionrequestrequesttypedef)
- [DeleteFolderContentsRequestRequestTypeDef](./type_defs.md#deletefoldercontentsrequestrequesttypedef)
- [DeleteFolderRequestRequestTypeDef](./type_defs.md#deletefolderrequestrequesttypedef)
- [DeleteLabelsRequestRequestTypeDef](./type_defs.md#deletelabelsrequestrequesttypedef)
- [DeleteNotificationSubscriptionRequestRequestTypeDef](./type_defs.md#deletenotificationsubscriptionrequestrequesttypedef)
- [DeleteUserRequestRequestTypeDef](./type_defs.md#deleteuserrequestrequesttypedef)
- [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
- [DescribeCommentsRequestRequestTypeDef](./type_defs.md#describecommentsrequestrequesttypedef)
- [DescribeDocumentVersionsRequestRequestTypeDef](./type_defs.md#describedocumentversionsrequestrequesttypedef)
- [DocumentVersionMetadataTypeDef](./type_defs.md#documentversionmetadatatypedef)
- [DescribeFolderContentsRequestRequestTypeDef](./type_defs.md#describefoldercontentsrequestrequesttypedef)
- [DescribeGroupsRequestRequestTypeDef](./type_defs.md#describegroupsrequestrequesttypedef)
- [GroupMetadataTypeDef](./type_defs.md#groupmetadatatypedef)
- [DescribeNotificationSubscriptionsRequestRequestTypeDef](./type_defs.md#describenotificationsubscriptionsrequestrequesttypedef)
- [DescribeResourcePermissionsRequestRequestTypeDef](./type_defs.md#describeresourcepermissionsrequestrequesttypedef)
- [DescribeRootFoldersRequestRequestTypeDef](./type_defs.md#describerootfoldersrequestrequesttypedef)
- [DescribeUsersRequestRequestTypeDef](./type_defs.md#describeusersrequestrequesttypedef)
- [LongRangeTypeTypeDef](./type_defs.md#longrangetypetypedef)
- [SearchPrincipalTypeTypeDef](./type_defs.md#searchprincipaltypetypedef)
- [GetCurrentUserRequestRequestTypeDef](./type_defs.md#getcurrentuserrequestrequesttypedef)
- [GetDocumentPathRequestRequestTypeDef](./type_defs.md#getdocumentpathrequestrequesttypedef)
- [GetDocumentRequestRequestTypeDef](./type_defs.md#getdocumentrequestrequesttypedef)
- [GetDocumentVersionRequestRequestTypeDef](./type_defs.md#getdocumentversionrequestrequesttypedef)
- [GetFolderPathRequestRequestTypeDef](./type_defs.md#getfolderpathrequestrequesttypedef)
- [GetFolderRequestRequestTypeDef](./type_defs.md#getfolderrequestrequesttypedef)
- [GetResourcesRequestRequestTypeDef](./type_defs.md#getresourcesrequestrequesttypedef)
- [UploadMetadataTypeDef](./type_defs.md#uploadmetadatatypedef)
- [PermissionInfoTypeDef](./type_defs.md#permissioninfotypedef)
- [RemoveAllResourcePermissionsRequestRequestTypeDef](./type_defs.md#removeallresourcepermissionsrequestrequesttypedef)
- [RemoveResourcePermissionRequestRequestTypeDef](./type_defs.md#removeresourcepermissionrequestrequesttypedef)
- [ResourcePathComponentTypeDef](./type_defs.md#resourcepathcomponenttypedef)
- [RestoreDocumentVersionsRequestRequestTypeDef](./type_defs.md#restoredocumentversionsrequestrequesttypedef)
- [SearchSortResultTypeDef](./type_defs.md#searchsortresulttypedef)
- [UpdateDocumentRequestRequestTypeDef](./type_defs.md#updatedocumentrequestrequesttypedef)
- [UpdateDocumentVersionRequestRequestTypeDef](./type_defs.md#updatedocumentversionrequestrequesttypedef)
- [UpdateFolderRequestRequestTypeDef](./type_defs.md#updatefolderrequestrequesttypedef)
- [EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef)
- [ResourceMetadataTypeDef](./type_defs.md#resourcemetadatatypedef)
- [AddResourcePermissionsRequestRequestTypeDef](./type_defs.md#addresourcepermissionsrequestrequesttypedef)
- [AddResourcePermissionsResponseTypeDef](./type_defs.md#addresourcepermissionsresponsetypedef)
- [CreateFolderResponseTypeDef](./type_defs.md#createfolderresponsetypedef)
- [DescribeRootFoldersResponseTypeDef](./type_defs.md#describerootfoldersresponsetypedef)
- [GetFolderResponseTypeDef](./type_defs.md#getfolderresponsetypedef)
- [CreateNotificationSubscriptionResponseTypeDef](./type_defs.md#createnotificationsubscriptionresponsetypedef)
- [DescribeNotificationSubscriptionsResponseTypeDef](./type_defs.md#describenotificationsubscriptionsresponsetypedef)
- [CreateUserRequestRequestTypeDef](./type_defs.md#createuserrequestrequesttypedef)
- [UpdateUserRequestRequestTypeDef](./type_defs.md#updateuserrequestrequesttypedef)
- [UserStorageMetadataTypeDef](./type_defs.md#userstoragemetadatatypedef)
- [DateRangeTypeTypeDef](./type_defs.md#daterangetypetypedef)
- [DescribeActivitiesRequestRequestTypeDef](./type_defs.md#describeactivitiesrequestrequesttypedef)
- [InitiateDocumentVersionUploadRequestRequestTypeDef](./type_defs.md#initiatedocumentversionuploadrequestrequesttypedef)
- [DescribeActivitiesRequestPaginateTypeDef](./type_defs.md#describeactivitiesrequestpaginatetypedef)
- [DescribeCommentsRequestPaginateTypeDef](./type_defs.md#describecommentsrequestpaginatetypedef)
- [DescribeDocumentVersionsRequestPaginateTypeDef](./type_defs.md#describedocumentversionsrequestpaginatetypedef)
- [DescribeFolderContentsRequestPaginateTypeDef](./type_defs.md#describefoldercontentsrequestpaginatetypedef)
- [DescribeGroupsRequestPaginateTypeDef](./type_defs.md#describegroupsrequestpaginatetypedef)
- [DescribeNotificationSubscriptionsRequestPaginateTypeDef](./type_defs.md#describenotificationsubscriptionsrequestpaginatetypedef)
- [DescribeResourcePermissionsRequestPaginateTypeDef](./type_defs.md#describeresourcepermissionsrequestpaginatetypedef)
- [DescribeRootFoldersRequestPaginateTypeDef](./type_defs.md#describerootfoldersrequestpaginatetypedef)
- [DescribeUsersRequestPaginateTypeDef](./type_defs.md#describeusersrequestpaginatetypedef)
- [DescribeDocumentVersionsResponseTypeDef](./type_defs.md#describedocumentversionsresponsetypedef)
- [DocumentMetadataTypeDef](./type_defs.md#documentmetadatatypedef)
- [GetDocumentVersionResponseTypeDef](./type_defs.md#getdocumentversionresponsetypedef)
- [DescribeGroupsResponseTypeDef](./type_defs.md#describegroupsresponsetypedef)
- [ParticipantsTypeDef](./type_defs.md#participantstypedef)
- [PrincipalTypeDef](./type_defs.md#principaltypedef)
- [ResourcePathTypeDef](./type_defs.md#resourcepathtypedef)
- [UserTypeDef](./type_defs.md#usertypedef)
- [FiltersTypeDef](./type_defs.md#filterstypedef)
- [DescribeFolderContentsResponseTypeDef](./type_defs.md#describefoldercontentsresponsetypedef)
- [GetDocumentResponseTypeDef](./type_defs.md#getdocumentresponsetypedef)
- [GetResourcesResponseTypeDef](./type_defs.md#getresourcesresponsetypedef)
- [InitiateDocumentVersionUploadResponseTypeDef](./type_defs.md#initiatedocumentversionuploadresponsetypedef)
- [DescribeResourcePermissionsResponseTypeDef](./type_defs.md#describeresourcepermissionsresponsetypedef)
- [GetDocumentPathResponseTypeDef](./type_defs.md#getdocumentpathresponsetypedef)
- [GetFolderPathResponseTypeDef](./type_defs.md#getfolderpathresponsetypedef)
- [ActivateUserResponseTypeDef](./type_defs.md#activateuserresponsetypedef)
- [CommentMetadataTypeDef](./type_defs.md#commentmetadatatypedef)
- [CommentTypeDef](./type_defs.md#commenttypedef)
- [CreateUserResponseTypeDef](./type_defs.md#createuserresponsetypedef)
- [DescribeUsersResponseTypeDef](./type_defs.md#describeusersresponsetypedef)
- [GetCurrentUserResponseTypeDef](./type_defs.md#getcurrentuserresponsetypedef)
- [UpdateUserResponseTypeDef](./type_defs.md#updateuserresponsetypedef)
- [SearchResourcesRequestPaginateTypeDef](./type_defs.md#searchresourcesrequestpaginatetypedef)
- [SearchResourcesRequestRequestTypeDef](./type_defs.md#searchresourcesrequestrequesttypedef)
- [ActivityTypeDef](./type_defs.md#activitytypedef)
- [ResponseItemTypeDef](./type_defs.md#responseitemtypedef)
- [CreateCommentResponseTypeDef](./type_defs.md#createcommentresponsetypedef)
- [DescribeCommentsResponseTypeDef](./type_defs.md#describecommentsresponsetypedef)
- [DescribeActivitiesResponseTypeDef](./type_defs.md#describeactivitiesresponsetypedef)
- [SearchResourcesResponseTypeDef](./type_defs.md#searchresourcesresponsetypedef)

