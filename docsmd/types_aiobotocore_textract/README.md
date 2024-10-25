# Textract module

> [Index](../README.md) > Textract


!!! note ""

    Auto-generated documentation for [Textract](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/textract.html#Textract)
    type annotations stubs module [types-aiobotocore-textract](https://pypi.org/project/types-aiobotocore-textract/).

## How to install



### From PyPI with pip

Install `types-aiobotocore` for `Textract` service.

```bash
# install with aiobotocore type annotations
python -m pip install 'types-aiobotocore[textract]'


# Lite version does not provide session.client/resource overloads
# it is more RAM-friendly, but requires explicit type annotations
python -m pip install 'types-aiobotocore-lite[textract]'


# standalone installation
python -m pip install types-aiobotocore-textract
```



## How to uninstall

```bash
python -m pip uninstall -y types-aiobotocore-textract
```

## Usage

Code samples can be found in [Examples](./usage.md).

## TextractClient

Type annotations and code completion for  `#!python session.create_client("textract")` as [TextractClient](./client.md)
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/textract.html#Textract.Client)

```python
# TextractClient usage example

from aiobotocore.session import get_session

from types_aiobotocore_textract.client import TextractClient


session = get_session()
async with session.create_client("textract") as client:
    client: TextractClient
```


## Paginators

Type annotations and code completion for
[paginators](./paginators.md)
from `#!python session.create_client("textract").get_paginator("...")`.

```python
# ListAdapterVersionsPaginator usage example

from types_aiobotocore_textract.paginator import ListAdapterVersionsPaginator

def get_list_adapter_versions_paginator() -> ListAdapterVersionsPaginator:
    return client.get_paginator("list_adapter_versions"))
```

- [ListAdapterVersionsPaginator](./paginators.md#listadapterversionspaginator)
- [ListAdaptersPaginator](./paginators.md#listadapterspaginator)








## Literals

Type annotations for [literals](./literals.md) used in methods and schema.

```python
# AdapterVersionStatusType usage example

from types_aiobotocore_textract.literals import AdapterVersionStatusType

def get_value() -> AdapterVersionStatusType:
    return "ACTIVE"
```

- [AdapterVersionStatusType](./literals.md#adapterversionstatustype)
- [AutoUpdateType](./literals.md#autoupdatetype)
- [BlockTypeType](./literals.md#blocktypetype)
- [ContentClassifierType](./literals.md#contentclassifiertype)
- [EntityTypeType](./literals.md#entitytypetype)
- [FeatureTypeType](./literals.md#featuretypetype)
- [JobStatusType](./literals.md#jobstatustype)
- [ListAdapterVersionsPaginatorName](./literals.md#listadapterversionspaginatorname)
- [ListAdaptersPaginatorName](./literals.md#listadapterspaginatorname)
- [RelationshipTypeType](./literals.md#relationshiptypetype)
- [SelectionStatusType](./literals.md#selectionstatustype)
- [TextTypeType](./literals.md#texttypetype)
- [ValueTypeType](./literals.md#valuetypetype)
- [TextractServiceName](./literals.md#textractservicename)
- [ServiceName](./literals.md#servicename)
- [ResourceServiceName](./literals.md#resourceservicename)
- [PaginatorName](./literals.md#paginatorname)
- [RegionName](./literals.md#regionname)




## Type definitions

Type annotations for [type definitions](./type_defs.md) used in methods and schema.

- [AdapterOverviewTypeDef](./type_defs.md#adapteroverviewtypedef)
- [AdapterTypeDef](./type_defs.md#adaptertypedef)
- [S3ObjectTypeDef](./type_defs.md#s3objecttypedef)
- [EvaluationMetricTypeDef](./type_defs.md#evaluationmetrictypedef)
- [AdapterVersionOverviewTypeDef](./type_defs.md#adapterversionoverviewtypedef)
- [DocumentMetadataTypeDef](./type_defs.md#documentmetadatatypedef)
- [HumanLoopActivationOutputTypeDef](./type_defs.md#humanloopactivationoutputtypedef)
- [ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef)
- [NormalizedValueTypeDef](./type_defs.md#normalizedvaluetypedef)
- [BlobTypeDef](./type_defs.md#blobtypedef)
- [QueryOutputTypeDef](./type_defs.md#queryoutputtypedef)
- [RelationshipTypeDef](./type_defs.md#relationshiptypedef)
- [BoundingBoxTypeDef](./type_defs.md#boundingboxtypedef)
- [CreateAdapterRequestRequestTypeDef](./type_defs.md#createadapterrequestrequesttypedef)
- [OutputConfigTypeDef](./type_defs.md#outputconfigtypedef)
- [DeleteAdapterRequestRequestTypeDef](./type_defs.md#deleteadapterrequestrequesttypedef)
- [DeleteAdapterVersionRequestRequestTypeDef](./type_defs.md#deleteadapterversionrequestrequesttypedef)
- [DetectedSignatureTypeDef](./type_defs.md#detectedsignaturetypedef)
- [SplitDocumentTypeDef](./type_defs.md#splitdocumenttypedef)
- [UndetectedSignatureTypeDef](./type_defs.md#undetectedsignaturetypedef)
- [ExpenseCurrencyTypeDef](./type_defs.md#expensecurrencytypedef)
- [ExpenseGroupPropertyTypeDef](./type_defs.md#expensegrouppropertytypedef)
- [ExpenseTypeTypeDef](./type_defs.md#expensetypetypedef)
- [PointTypeDef](./type_defs.md#pointtypedef)
- [GetAdapterRequestRequestTypeDef](./type_defs.md#getadapterrequestrequesttypedef)
- [GetAdapterVersionRequestRequestTypeDef](./type_defs.md#getadapterversionrequestrequesttypedef)
- [GetDocumentAnalysisRequestRequestTypeDef](./type_defs.md#getdocumentanalysisrequestrequesttypedef)
- [WarningTypeDef](./type_defs.md#warningtypedef)
- [GetDocumentTextDetectionRequestRequestTypeDef](./type_defs.md#getdocumenttextdetectionrequestrequesttypedef)
- [GetExpenseAnalysisRequestRequestTypeDef](./type_defs.md#getexpenseanalysisrequestrequesttypedef)
- [GetLendingAnalysisRequestRequestTypeDef](./type_defs.md#getlendinganalysisrequestrequesttypedef)
- [GetLendingAnalysisSummaryRequestRequestTypeDef](./type_defs.md#getlendinganalysissummaryrequestrequesttypedef)
- [HumanLoopDataAttributesTypeDef](./type_defs.md#humanloopdataattributestypedef)
- [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
- [TimestampTypeDef](./type_defs.md#timestamptypedef)
- [ListTagsForResourceRequestRequestTypeDef](./type_defs.md#listtagsforresourcerequestrequesttypedef)
- [NotificationChannelTypeDef](./type_defs.md#notificationchanneltypedef)
- [PredictionTypeDef](./type_defs.md#predictiontypedef)
- [QueryTypeDef](./type_defs.md#querytypedef)
- [TagResourceRequestRequestTypeDef](./type_defs.md#tagresourcerequestrequesttypedef)
- [UntagResourceRequestRequestTypeDef](./type_defs.md#untagresourcerequestrequesttypedef)
- [UpdateAdapterRequestRequestTypeDef](./type_defs.md#updateadapterrequestrequesttypedef)
- [AdaptersConfigTypeDef](./type_defs.md#adaptersconfigtypedef)
- [AdapterVersionDatasetConfigTypeDef](./type_defs.md#adapterversiondatasetconfigtypedef)
- [DocumentLocationTypeDef](./type_defs.md#documentlocationtypedef)
- [AdapterVersionEvaluationMetricTypeDef](./type_defs.md#adapterversionevaluationmetrictypedef)
- [CreateAdapterResponseTypeDef](./type_defs.md#createadapterresponsetypedef)
- [CreateAdapterVersionResponseTypeDef](./type_defs.md#createadapterversionresponsetypedef)
- [GetAdapterResponseTypeDef](./type_defs.md#getadapterresponsetypedef)
- [ListAdapterVersionsResponseTypeDef](./type_defs.md#listadapterversionsresponsetypedef)
- [ListAdaptersResponseTypeDef](./type_defs.md#listadaptersresponsetypedef)
- [ListTagsForResourceResponseTypeDef](./type_defs.md#listtagsforresourceresponsetypedef)
- [StartDocumentAnalysisResponseTypeDef](./type_defs.md#startdocumentanalysisresponsetypedef)
- [StartDocumentTextDetectionResponseTypeDef](./type_defs.md#startdocumenttextdetectionresponsetypedef)
- [StartExpenseAnalysisResponseTypeDef](./type_defs.md#startexpenseanalysisresponsetypedef)
- [StartLendingAnalysisResponseTypeDef](./type_defs.md#startlendinganalysisresponsetypedef)
- [UpdateAdapterResponseTypeDef](./type_defs.md#updateadapterresponsetypedef)
- [AnalyzeIDDetectionsTypeDef](./type_defs.md#analyzeiddetectionstypedef)
- [DocumentTypeDef](./type_defs.md#documenttypedef)
- [DocumentGroupTypeDef](./type_defs.md#documentgrouptypedef)
- [GeometryTypeDef](./type_defs.md#geometrytypedef)
- [HumanLoopConfigTypeDef](./type_defs.md#humanloopconfigtypedef)
- [ListAdapterVersionsRequestListAdapterVersionsPaginateTypeDef](./type_defs.md#listadapterversionsrequestlistadapterversionspaginatetypedef)
- [ListAdapterVersionsRequestRequestTypeDef](./type_defs.md#listadapterversionsrequestrequesttypedef)
- [ListAdaptersRequestListAdaptersPaginateTypeDef](./type_defs.md#listadaptersrequestlistadapterspaginatetypedef)
- [ListAdaptersRequestRequestTypeDef](./type_defs.md#listadaptersrequestrequesttypedef)
- [PageClassificationTypeDef](./type_defs.md#pageclassificationtypedef)
- [QueryUnionTypeDef](./type_defs.md#queryuniontypedef)
- [CreateAdapterVersionRequestRequestTypeDef](./type_defs.md#createadapterversionrequestrequesttypedef)
- [StartDocumentTextDetectionRequestRequestTypeDef](./type_defs.md#startdocumenttextdetectionrequestrequesttypedef)
- [StartExpenseAnalysisRequestRequestTypeDef](./type_defs.md#startexpenseanalysisrequestrequesttypedef)
- [StartLendingAnalysisRequestRequestTypeDef](./type_defs.md#startlendinganalysisrequestrequesttypedef)
- [GetAdapterVersionResponseTypeDef](./type_defs.md#getadapterversionresponsetypedef)
- [IdentityDocumentFieldTypeDef](./type_defs.md#identitydocumentfieldtypedef)
- [AnalyzeExpenseRequestRequestTypeDef](./type_defs.md#analyzeexpenserequestrequesttypedef)
- [AnalyzeIDRequestRequestTypeDef](./type_defs.md#analyzeidrequestrequesttypedef)
- [DetectDocumentTextRequestRequestTypeDef](./type_defs.md#detectdocumenttextrequestrequesttypedef)
- [LendingSummaryTypeDef](./type_defs.md#lendingsummarytypedef)
- [BlockTypeDef](./type_defs.md#blocktypedef)
- [ExpenseDetectionTypeDef](./type_defs.md#expensedetectiontypedef)
- [LendingDetectionTypeDef](./type_defs.md#lendingdetectiontypedef)
- [SignatureDetectionTypeDef](./type_defs.md#signaturedetectiontypedef)
- [QueriesConfigTypeDef](./type_defs.md#queriesconfigtypedef)
- [GetLendingAnalysisSummaryResponseTypeDef](./type_defs.md#getlendinganalysissummaryresponsetypedef)
- [AnalyzeDocumentResponseTypeDef](./type_defs.md#analyzedocumentresponsetypedef)
- [DetectDocumentTextResponseTypeDef](./type_defs.md#detectdocumenttextresponsetypedef)
- [GetDocumentAnalysisResponseTypeDef](./type_defs.md#getdocumentanalysisresponsetypedef)
- [GetDocumentTextDetectionResponseTypeDef](./type_defs.md#getdocumenttextdetectionresponsetypedef)
- [IdentityDocumentTypeDef](./type_defs.md#identitydocumenttypedef)
- [ExpenseFieldTypeDef](./type_defs.md#expensefieldtypedef)
- [LendingFieldTypeDef](./type_defs.md#lendingfieldtypedef)
- [AnalyzeDocumentRequestRequestTypeDef](./type_defs.md#analyzedocumentrequestrequesttypedef)
- [StartDocumentAnalysisRequestRequestTypeDef](./type_defs.md#startdocumentanalysisrequestrequesttypedef)
- [AnalyzeIDResponseTypeDef](./type_defs.md#analyzeidresponsetypedef)
- [LineItemFieldsTypeDef](./type_defs.md#lineitemfieldstypedef)
- [LendingDocumentTypeDef](./type_defs.md#lendingdocumenttypedef)
- [LineItemGroupTypeDef](./type_defs.md#lineitemgrouptypedef)
- [ExpenseDocumentTypeDef](./type_defs.md#expensedocumenttypedef)
- [AnalyzeExpenseResponseTypeDef](./type_defs.md#analyzeexpenseresponsetypedef)
- [ExtractionTypeDef](./type_defs.md#extractiontypedef)
- [GetExpenseAnalysisResponseTypeDef](./type_defs.md#getexpenseanalysisresponsetypedef)
- [LendingResultTypeDef](./type_defs.md#lendingresulttypedef)
- [GetLendingAnalysisResponseTypeDef](./type_defs.md#getlendinganalysisresponsetypedef)

