# QApps module

> [Index](../README.md) > QApps


!!! note ""

    Auto-generated documentation for [QApps](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/qapps.html#QApps)
    type annotations stubs module [types-aiobotocore-qapps](https://pypi.org/project/types-aiobotocore-qapps/).

## How to install



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
- [LibraryItemStatusType](./literals.md#libraryitemstatustype)
- [ListLibraryItemsPaginatorName](./literals.md#listlibraryitemspaginatorname)
- [ListQAppsPaginatorName](./literals.md#listqappspaginatorname)
- [PluginTypeType](./literals.md#plugintypetype)
- [SenderType](./literals.md#sendertype)
- [QAppsServiceName](./literals.md#qappsservicename)
- [ServiceName](./literals.md#servicename)
- [ResourceServiceName](./literals.md#resourceservicename)
- [PaginatorName](./literals.md#paginatorname)




## Type definitions

Type annotations for [type definitions](./type_defs.md) used in methods and schema.

- [AssociateLibraryItemReviewInputRequestTypeDef](./type_defs.md#associatelibraryitemreviewinputrequesttypedef)
- [AssociateQAppWithUserInputRequestTypeDef](./type_defs.md#associateqappwithuserinputrequesttypedef)
- [FileUploadCardInputTypeDef](./type_defs.md#fileuploadcardinputtypedef)
- [QPluginCardInputTypeDef](./type_defs.md#qplugincardinputtypedef)
- [TextInputCardInputTypeDef](./type_defs.md#textinputcardinputtypedef)
- [CardStatusTypeDef](./type_defs.md#cardstatustypedef)
- [FileUploadCardTypeDef](./type_defs.md#fileuploadcardtypedef)
- [QPluginCardTypeDef](./type_defs.md#qplugincardtypedef)
- [TextInputCardTypeDef](./type_defs.md#textinputcardtypedef)
- [CardValueTypeDef](./type_defs.md#cardvaluetypedef)
- [CategoryTypeDef](./type_defs.md#categorytypedef)
- [ConversationMessageTypeDef](./type_defs.md#conversationmessagetypedef)
- [CreateLibraryItemInputRequestTypeDef](./type_defs.md#createlibraryiteminputrequesttypedef)
- [ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef)
- [DeleteLibraryItemInputRequestTypeDef](./type_defs.md#deletelibraryiteminputrequesttypedef)
- [DeleteQAppInputRequestTypeDef](./type_defs.md#deleteqappinputrequesttypedef)
- [DisassociateLibraryItemReviewInputRequestTypeDef](./type_defs.md#disassociatelibraryitemreviewinputrequesttypedef)
- [DisassociateQAppFromUserInputRequestTypeDef](./type_defs.md#disassociateqappfromuserinputrequesttypedef)
- [DocumentAttributeValueOutputTypeDef](./type_defs.md#documentattributevalueoutputtypedef)
- [TimestampTypeDef](./type_defs.md#timestamptypedef)
- [GetLibraryItemInputRequestTypeDef](./type_defs.md#getlibraryiteminputrequesttypedef)
- [GetQAppInputRequestTypeDef](./type_defs.md#getqappinputrequesttypedef)
- [GetQAppSessionInputRequestTypeDef](./type_defs.md#getqappsessioninputrequesttypedef)
- [ImportDocumentInputRequestTypeDef](./type_defs.md#importdocumentinputrequesttypedef)
- [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
- [ListLibraryItemsInputRequestTypeDef](./type_defs.md#listlibraryitemsinputrequesttypedef)
- [ListQAppsInputRequestTypeDef](./type_defs.md#listqappsinputrequesttypedef)
- [UserAppItemTypeDef](./type_defs.md#userappitemtypedef)
- [ListTagsForResourceRequestRequestTypeDef](./type_defs.md#listtagsforresourcerequestrequesttypedef)
- [StopQAppSessionInputRequestTypeDef](./type_defs.md#stopqappsessioninputrequesttypedef)
- [TagResourceRequestRequestTypeDef](./type_defs.md#tagresourcerequestrequesttypedef)
- [UntagResourceRequestRequestTypeDef](./type_defs.md#untagresourcerequestrequesttypedef)
- [UpdateLibraryItemInputRequestTypeDef](./type_defs.md#updatelibraryiteminputrequesttypedef)
- [UpdateLibraryItemMetadataInputRequestTypeDef](./type_defs.md#updatelibraryitemmetadatainputrequesttypedef)
- [StartQAppSessionInputRequestTypeDef](./type_defs.md#startqappsessioninputrequesttypedef)
- [UpdateQAppSessionInputRequestTypeDef](./type_defs.md#updateqappsessioninputrequesttypedef)
- [LibraryItemMemberTypeDef](./type_defs.md#libraryitemmembertypedef)
- [PredictQAppInputOptionsTypeDef](./type_defs.md#predictqappinputoptionstypedef)
- [CreateLibraryItemOutputTypeDef](./type_defs.md#createlibraryitemoutputtypedef)
- [CreateQAppOutputTypeDef](./type_defs.md#createqappoutputtypedef)
- [EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef)
- [GetLibraryItemOutputTypeDef](./type_defs.md#getlibraryitemoutputtypedef)
- [GetQAppSessionOutputTypeDef](./type_defs.md#getqappsessionoutputtypedef)
- [ImportDocumentOutputTypeDef](./type_defs.md#importdocumentoutputtypedef)
- [ListTagsForResourceResponseTypeDef](./type_defs.md#listtagsforresourceresponsetypedef)
- [StartQAppSessionOutputTypeDef](./type_defs.md#startqappsessionoutputtypedef)
- [UpdateLibraryItemOutputTypeDef](./type_defs.md#updatelibraryitemoutputtypedef)
- [UpdateQAppOutputTypeDef](./type_defs.md#updateqappoutputtypedef)
- [UpdateQAppSessionOutputTypeDef](./type_defs.md#updateqappsessionoutputtypedef)
- [DocumentAttributeOutputTypeDef](./type_defs.md#documentattributeoutputtypedef)
- [DocumentAttributeValueTypeDef](./type_defs.md#documentattributevaluetypedef)
- [ListLibraryItemsInputListLibraryItemsPaginateTypeDef](./type_defs.md#listlibraryitemsinputlistlibraryitemspaginatetypedef)
- [ListQAppsInputListQAppsPaginateTypeDef](./type_defs.md#listqappsinputlistqappspaginatetypedef)
- [ListQAppsOutputTypeDef](./type_defs.md#listqappsoutputtypedef)
- [ListLibraryItemsOutputTypeDef](./type_defs.md#listlibraryitemsoutputtypedef)
- [PredictQAppInputRequestTypeDef](./type_defs.md#predictqappinputrequesttypedef)
- [AttributeFilterOutputTypeDef](./type_defs.md#attributefilteroutputtypedef)
- [DocumentAttributeValueUnionTypeDef](./type_defs.md#documentattributevalueuniontypedef)
- [QQueryCardInputOutputTypeDef](./type_defs.md#qquerycardinputoutputtypedef)
- [QQueryCardTypeDef](./type_defs.md#qquerycardtypedef)
- [DocumentAttributeTypeDef](./type_defs.md#documentattributetypedef)
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

