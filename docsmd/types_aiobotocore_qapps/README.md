# QApps module

> [Index](../README.md) > QApps


!!! note ""

    Auto-generated documentation for [QApps](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/qapps.html#qapps)
    type annotations stubs module [types-aiobotocore-qapps](https://pypi.org/project/types-aiobotocore-qapps/).

## How to install

### Generate locally (recommended)

You can generate type annotations for `aiobotocore` package locally with `mypy_boto3_builder`.
Use [uv](https://docs.astral.sh/uv/getting-started/installation/) for build isolation.

1. Run mypy-boto3-builder in your package root directory: `uvx --with 'aiobotocore==2.19.0' mypy_boto3_builder`
1. Select `aiobotocore` AWS SDK.
1. Add `QApps` service.
1. Use provided commands to install generated packages.



### From PyPI with pip

Install `types-aiobotocore` for `QApps` service.

```bash
# install with aiobotocore type annotations
python -m pip install 'types-aiobotocore[qapps]'

# Lite version does not provide session.client/resource overloads
# it is more RAM-friendly, but requires explicit type annotations
python -m pip install 'types-aiobotocore-lite[qapps]'

# standalone installation
python -m pip install types-aiobotocore-qapps
```



## How to uninstall

```bash
python -m pip uninstall -y types-aiobotocore-qapps
```

## Usage

Code samples can be found in [Examples](./usage.md).

## QAppsClient

Type annotations and code completion for  `#!python session.create_client("qapps")` as [QAppsClient](./client.md)
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/qapps.html#QApps.Client)

```python
# QAppsClient usage example

from aiobotocore.session import get_session

from types_aiobotocore_qapps.client import QAppsClient


session = get_session()
async with session.create_client("qapps") as client:
    client: QAppsClient
```


## Paginators

Type annotations and code completion for
[paginators](./paginators.md)
from `#!python session.create_client("qapps").get_paginator("...")`.

```python
# ListLibraryItemsPaginator usage example

from types_aiobotocore_qapps.paginator import ListLibraryItemsPaginator

def get_list_library_items_paginator() -> ListLibraryItemsPaginator:
    return client.get_paginator("list_library_items"))
```

- [ListLibraryItemsPaginator](./paginators.md#listlibraryitemspaginator)
- [ListQAppsPaginator](./paginators.md#listqappspaginator)








## Literals

Type annotations for [literals](./literals.md) used in methods and schema.

```python
# AppRequiredCapabilityType usage example

from types_aiobotocore_qapps.literals import AppRequiredCapabilityType

def get_value() -> AppRequiredCapabilityType:
    return "CreatorMode"
```

- [AppRequiredCapabilityType](./literals.md#apprequiredcapabilitytype)
- [AppStatusType](./literals.md#appstatustype)
- [CardOutputSourceType](./literals.md#cardoutputsourcetype)
- [CardTypeType](./literals.md#cardtypetype)
- [DocumentScopeType](./literals.md#documentscopetype)
- [ExecutionStatusType](./literals.md#executionstatustype)
- [InputCardComputeModeType](./literals.md#inputcardcomputemodetype)
- [LibraryItemStatusType](./literals.md#libraryitemstatustype)
- [ListLibraryItemsPaginatorName](./literals.md#listlibraryitemspaginatorname)
- [ListQAppsPaginatorName](./literals.md#listqappspaginatorname)
- [PermissionInputActionEnumType](./literals.md#permissioninputactionenumtype)
- [PermissionOutputActionEnumType](./literals.md#permissionoutputactionenumtype)
- [PluginTypeType](./literals.md#plugintypetype)
- [PrincipalOutputUserTypeEnumType](./literals.md#principaloutputusertypeenumtype)
- [SenderType](./literals.md#sendertype)
- [SubmissionMutationKindType](./literals.md#submissionmutationkindtype)
- [QAppsServiceName](./literals.md#qappsservicename)
- [ServiceName](./literals.md#servicename)
- [ResourceServiceName](./literals.md#resourceservicename)
- [PaginatorName](./literals.md#paginatorname)




## Type definitions

Type annotations for [type definitions](./type_defs.md) used in methods and schema.

- [AssociateLibraryItemReviewInputRequestTypeDef](./type_defs.md#associatelibraryitemreviewinputrequesttypedef)
- [AssociateQAppWithUserInputRequestTypeDef](./type_defs.md#associateqappwithuserinputrequesttypedef)
- [BatchCreateCategoryInputCategoryTypeDef](./type_defs.md#batchcreatecategoryinputcategorytypedef)
- [BatchDeleteCategoryInputRequestTypeDef](./type_defs.md#batchdeletecategoryinputrequesttypedef)
- [CategoryInputTypeDef](./type_defs.md#categoryinputtypedef)
- [FileUploadCardInputTypeDef](./type_defs.md#fileuploadcardinputtypedef)
- [QPluginCardInputTypeDef](./type_defs.md#qplugincardinputtypedef)
- [TextInputCardInputTypeDef](./type_defs.md#textinputcardinputtypedef)
- [SubmissionTypeDef](./type_defs.md#submissiontypedef)
- [FileUploadCardTypeDef](./type_defs.md#fileuploadcardtypedef)
- [QPluginCardTypeDef](./type_defs.md#qplugincardtypedef)
- [TextInputCardTypeDef](./type_defs.md#textinputcardtypedef)
- [SubmissionMutationTypeDef](./type_defs.md#submissionmutationtypedef)
- [CategoryTypeDef](./type_defs.md#categorytypedef)
- [ConversationMessageTypeDef](./type_defs.md#conversationmessagetypedef)
- [CreateLibraryItemInputRequestTypeDef](./type_defs.md#createlibraryiteminputrequesttypedef)
- [ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef)
- [CreatePresignedUrlInputRequestTypeDef](./type_defs.md#createpresignedurlinputrequesttypedef)
- [DeleteLibraryItemInputRequestTypeDef](./type_defs.md#deletelibraryiteminputrequesttypedef)
- [DeleteQAppInputRequestTypeDef](./type_defs.md#deleteqappinputrequesttypedef)
- [DescribeQAppPermissionsInputRequestTypeDef](./type_defs.md#describeqapppermissionsinputrequesttypedef)
- [DisassociateLibraryItemReviewInputRequestTypeDef](./type_defs.md#disassociatelibraryitemreviewinputrequesttypedef)
- [DisassociateQAppFromUserInputRequestTypeDef](./type_defs.md#disassociateqappfromuserinputrequesttypedef)
- [DocumentAttributeValueOutputTypeDef](./type_defs.md#documentattributevalueoutputtypedef)
- [TimestampTypeDef](./type_defs.md#timestamptypedef)
- [ExportQAppSessionDataInputRequestTypeDef](./type_defs.md#exportqappsessiondatainputrequesttypedef)
- [FormInputCardMetadataOutputTypeDef](./type_defs.md#forminputcardmetadataoutputtypedef)
- [FormInputCardMetadataTypeDef](./type_defs.md#forminputcardmetadatatypedef)
- [GetLibraryItemInputRequestTypeDef](./type_defs.md#getlibraryiteminputrequesttypedef)
- [GetQAppInputRequestTypeDef](./type_defs.md#getqappinputrequesttypedef)
- [GetQAppSessionInputRequestTypeDef](./type_defs.md#getqappsessioninputrequesttypedef)
- [GetQAppSessionMetadataInputRequestTypeDef](./type_defs.md#getqappsessionmetadatainputrequesttypedef)
- [SessionSharingConfigurationTypeDef](./type_defs.md#sessionsharingconfigurationtypedef)
- [ImportDocumentInputRequestTypeDef](./type_defs.md#importdocumentinputrequesttypedef)
- [ListCategoriesInputRequestTypeDef](./type_defs.md#listcategoriesinputrequesttypedef)
- [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
- [ListLibraryItemsInputRequestTypeDef](./type_defs.md#listlibraryitemsinputrequesttypedef)
- [ListQAppSessionDataInputRequestTypeDef](./type_defs.md#listqappsessiondatainputrequesttypedef)
- [ListQAppsInputRequestTypeDef](./type_defs.md#listqappsinputrequesttypedef)
- [UserAppItemTypeDef](./type_defs.md#userappitemtypedef)
- [ListTagsForResourceRequestRequestTypeDef](./type_defs.md#listtagsforresourcerequestrequesttypedef)
- [PermissionInputTypeDef](./type_defs.md#permissioninputtypedef)
- [PrincipalOutputTypeDef](./type_defs.md#principaloutputtypedef)
- [UserTypeDef](./type_defs.md#usertypedef)
- [StopQAppSessionInputRequestTypeDef](./type_defs.md#stopqappsessioninputrequesttypedef)
- [TagResourceRequestRequestTypeDef](./type_defs.md#tagresourcerequestrequesttypedef)
- [UntagResourceRequestRequestTypeDef](./type_defs.md#untagresourcerequestrequesttypedef)
- [UpdateLibraryItemInputRequestTypeDef](./type_defs.md#updatelibraryiteminputrequesttypedef)
- [UpdateLibraryItemMetadataInputRequestTypeDef](./type_defs.md#updatelibraryitemmetadatainputrequesttypedef)
- [BatchCreateCategoryInputRequestTypeDef](./type_defs.md#batchcreatecategoryinputrequesttypedef)
- [BatchUpdateCategoryInputRequestTypeDef](./type_defs.md#batchupdatecategoryinputrequesttypedef)
- [CardStatusTypeDef](./type_defs.md#cardstatustypedef)
- [CardValueTypeDef](./type_defs.md#cardvaluetypedef)
- [LibraryItemMemberTypeDef](./type_defs.md#libraryitemmembertypedef)
- [PredictQAppInputOptionsTypeDef](./type_defs.md#predictqappinputoptionstypedef)
- [CreateLibraryItemOutputTypeDef](./type_defs.md#createlibraryitemoutputtypedef)
- [CreatePresignedUrlOutputTypeDef](./type_defs.md#createpresignedurloutputtypedef)
- [CreateQAppOutputTypeDef](./type_defs.md#createqappoutputtypedef)
- [EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef)
- [ExportQAppSessionDataOutputTypeDef](./type_defs.md#exportqappsessiondataoutputtypedef)
- [GetLibraryItemOutputTypeDef](./type_defs.md#getlibraryitemoutputtypedef)
- [ImportDocumentOutputTypeDef](./type_defs.md#importdocumentoutputtypedef)
- [ListCategoriesOutputTypeDef](./type_defs.md#listcategoriesoutputtypedef)
- [ListTagsForResourceResponseTypeDef](./type_defs.md#listtagsforresourceresponsetypedef)
- [StartQAppSessionOutputTypeDef](./type_defs.md#startqappsessionoutputtypedef)
- [UpdateLibraryItemOutputTypeDef](./type_defs.md#updatelibraryitemoutputtypedef)
- [UpdateQAppOutputTypeDef](./type_defs.md#updateqappoutputtypedef)
- [UpdateQAppSessionOutputTypeDef](./type_defs.md#updateqappsessionoutputtypedef)
- [DocumentAttributeOutputTypeDef](./type_defs.md#documentattributeoutputtypedef)
- [DocumentAttributeValueTypeDef](./type_defs.md#documentattributevaluetypedef)
- [FormInputCardInputOutputTypeDef](./type_defs.md#forminputcardinputoutputtypedef)
- [FormInputCardTypeDef](./type_defs.md#forminputcardtypedef)
- [FormInputCardMetadataUnionTypeDef](./type_defs.md#forminputcardmetadatauniontypedef)
- [GetQAppSessionMetadataOutputTypeDef](./type_defs.md#getqappsessionmetadataoutputtypedef)
- [UpdateQAppSessionMetadataInputRequestTypeDef](./type_defs.md#updateqappsessionmetadatainputrequesttypedef)
- [UpdateQAppSessionMetadataOutputTypeDef](./type_defs.md#updateqappsessionmetadataoutputtypedef)
- [ListLibraryItemsInputPaginateTypeDef](./type_defs.md#listlibraryitemsinputpaginatetypedef)
- [ListQAppsInputPaginateTypeDef](./type_defs.md#listqappsinputpaginatetypedef)
- [ListQAppsOutputTypeDef](./type_defs.md#listqappsoutputtypedef)
- [UpdateQAppPermissionsInputRequestTypeDef](./type_defs.md#updateqapppermissionsinputrequesttypedef)
- [PermissionOutputTypeDef](./type_defs.md#permissionoutputtypedef)
- [QAppSessionDataTypeDef](./type_defs.md#qappsessiondatatypedef)
- [GetQAppSessionOutputTypeDef](./type_defs.md#getqappsessionoutputtypedef)
- [StartQAppSessionInputRequestTypeDef](./type_defs.md#startqappsessioninputrequesttypedef)
- [UpdateQAppSessionInputRequestTypeDef](./type_defs.md#updateqappsessioninputrequesttypedef)
- [ListLibraryItemsOutputTypeDef](./type_defs.md#listlibraryitemsoutputtypedef)
- [PredictQAppInputRequestTypeDef](./type_defs.md#predictqappinputrequesttypedef)
- [AttributeFilterOutputTypeDef](./type_defs.md#attributefilteroutputtypedef)
- [DocumentAttributeValueUnionTypeDef](./type_defs.md#documentattributevalueuniontypedef)
- [FormInputCardInputTypeDef](./type_defs.md#forminputcardinputtypedef)
- [DescribeQAppPermissionsOutputTypeDef](./type_defs.md#describeqapppermissionsoutputtypedef)
- [UpdateQAppPermissionsOutputTypeDef](./type_defs.md#updateqapppermissionsoutputtypedef)
- [ListQAppSessionDataOutputTypeDef](./type_defs.md#listqappsessiondataoutputtypedef)
- [QQueryCardInputOutputTypeDef](./type_defs.md#qquerycardinputoutputtypedef)
- [QQueryCardTypeDef](./type_defs.md#qquerycardtypedef)
- [DocumentAttributeTypeDef](./type_defs.md#documentattributetypedef)
- [FormInputCardInputUnionTypeDef](./type_defs.md#forminputcardinputuniontypedef)
- [CardInputOutputTypeDef](./type_defs.md#cardinputoutputtypedef)
- [CardTypeDef](./type_defs.md#cardtypedef)
- [DocumentAttributeUnionTypeDef](./type_defs.md#documentattributeuniontypedef)
- [AppDefinitionInputOutputTypeDef](./type_defs.md#appdefinitioninputoutputtypedef)
- [AppDefinitionTypeDef](./type_defs.md#appdefinitiontypedef)
- [AttributeFilterTypeDef](./type_defs.md#attributefiltertypedef)
- [PredictAppDefinitionTypeDef](./type_defs.md#predictappdefinitiontypedef)
- [GetQAppOutputTypeDef](./type_defs.md#getqappoutputtypedef)
- [AttributeFilterUnionTypeDef](./type_defs.md#attributefilteruniontypedef)
- [PredictQAppOutputTypeDef](./type_defs.md#predictqappoutputtypedef)
- [QQueryCardInputTypeDef](./type_defs.md#qquerycardinputtypedef)
- [QQueryCardInputUnionTypeDef](./type_defs.md#qquerycardinputuniontypedef)
- [CardInputTypeDef](./type_defs.md#cardinputtypedef)
- [CardInputUnionTypeDef](./type_defs.md#cardinputuniontypedef)
- [AppDefinitionInputTypeDef](./type_defs.md#appdefinitioninputtypedef)
- [CreateQAppInputRequestTypeDef](./type_defs.md#createqappinputrequesttypedef)
- [UpdateQAppInputRequestTypeDef](./type_defs.md#updateqappinputrequesttypedef)

