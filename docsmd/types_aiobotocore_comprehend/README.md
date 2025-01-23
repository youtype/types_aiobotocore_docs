# Comprehend module

> [Index](../README.md) > Comprehend


!!! note ""

    Auto-generated documentation for [Comprehend](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/comprehend.html#comprehend)
    type annotations stubs module [types-aiobotocore-comprehend](https://pypi.org/project/types-aiobotocore-comprehend/).

## How to install

### Generate locally (recommended)

You can generate type annotations for `aiobotocore` package locally with `mypy_boto3_builder`.
Use [uv](https://docs.astral.sh/uv/getting-started/installation/) for build isolation.

1. Run mypy-boto3-builder in your package root directory: `uvx --with 'aiobotocore==2.19.0' mypy_boto3_builder`
1. Select `aiobotocore` AWS SDK.
1. Add `Comprehend` service.
1. Use provided commands to install generated packages.



### From PyPI with pip

Install `types-aiobotocore` for `Comprehend` service.

```bash
# install with aiobotocore type annotations
python -m pip install 'types-aiobotocore[comprehend]'

# Lite version does not provide session.client/resource overloads
# it is more RAM-friendly, but requires explicit type annotations
python -m pip install 'types-aiobotocore-lite[comprehend]'

# standalone installation
python -m pip install types-aiobotocore-comprehend
```



## How to uninstall

```bash
python -m pip uninstall -y types-aiobotocore-comprehend
```

## Usage

Code samples can be found in [Examples](./usage.md).

## ComprehendClient

Type annotations and code completion for  `#!python session.create_client("comprehend")` as [ComprehendClient](./client.md)
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/comprehend.html#Comprehend.Client)

```python
# ComprehendClient usage example

from aiobotocore.session import get_session

from types_aiobotocore_comprehend.client import ComprehendClient


session = get_session()
async with session.create_client("comprehend") as client:
    client: ComprehendClient
```


## Paginators

Type annotations and code completion for
[paginators](./paginators.md)
from `#!python session.create_client("comprehend").get_paginator("...")`.

```python
# ListDocumentClassificationJobsPaginator usage example

from types_aiobotocore_comprehend.paginator import ListDocumentClassificationJobsPaginator

def get_list_document_classification_jobs_paginator() -> ListDocumentClassificationJobsPaginator:
    return client.get_paginator("list_document_classification_jobs"))
```

- [ListDocumentClassificationJobsPaginator](./paginators.md#listdocumentclassificationjobspaginator)
- [ListDocumentClassifiersPaginator](./paginators.md#listdocumentclassifierspaginator)
- [ListDominantLanguageDetectionJobsPaginator](./paginators.md#listdominantlanguagedetectionjobspaginator)
- [ListEndpointsPaginator](./paginators.md#listendpointspaginator)
- [ListEntitiesDetectionJobsPaginator](./paginators.md#listentitiesdetectionjobspaginator)
- [ListEntityRecognizersPaginator](./paginators.md#listentityrecognizerspaginator)
- [ListKeyPhrasesDetectionJobsPaginator](./paginators.md#listkeyphrasesdetectionjobspaginator)
- [ListPiiEntitiesDetectionJobsPaginator](./paginators.md#listpiientitiesdetectionjobspaginator)
- [ListSentimentDetectionJobsPaginator](./paginators.md#listsentimentdetectionjobspaginator)
- [ListTopicsDetectionJobsPaginator](./paginators.md#listtopicsdetectionjobspaginator)








## Literals

Type annotations for [literals](./literals.md) used in methods and schema.

```python
# AugmentedManifestsDocumentTypeFormatType usage example

from types_aiobotocore_comprehend.literals import AugmentedManifestsDocumentTypeFormatType

def get_value() -> AugmentedManifestsDocumentTypeFormatType:
    return "PLAIN_TEXT_DOCUMENT"
```

- [AugmentedManifestsDocumentTypeFormatType](./literals.md#augmentedmanifestsdocumenttypeformattype)
- [BlockTypeType](./literals.md#blocktypetype)
- [DatasetDataFormatType](./literals.md#datasetdataformattype)
- [DatasetStatusType](./literals.md#datasetstatustype)
- [DatasetTypeType](./literals.md#datasettypetype)
- [DocumentClassifierDataFormatType](./literals.md#documentclassifierdataformattype)
- [DocumentClassifierDocumentTypeFormatType](./literals.md#documentclassifierdocumenttypeformattype)
- [DocumentClassifierModeType](./literals.md#documentclassifiermodetype)
- [DocumentReadActionType](./literals.md#documentreadactiontype)
- [DocumentReadFeatureTypesType](./literals.md#documentreadfeaturetypestype)
- [DocumentReadModeType](./literals.md#documentreadmodetype)
- [DocumentTypeType](./literals.md#documenttypetype)
- [EndpointStatusType](./literals.md#endpointstatustype)
- [EntityRecognizerDataFormatType](./literals.md#entityrecognizerdataformattype)
- [EntityTypeType](./literals.md#entitytypetype)
- [FlywheelIterationStatusType](./literals.md#flywheeliterationstatustype)
- [FlywheelStatusType](./literals.md#flywheelstatustype)
- [InputFormatType](./literals.md#inputformattype)
- [JobStatusType](./literals.md#jobstatustype)
- [LanguageCodeType](./literals.md#languagecodetype)
- [ListDocumentClassificationJobsPaginatorName](./literals.md#listdocumentclassificationjobspaginatorname)
- [ListDocumentClassifiersPaginatorName](./literals.md#listdocumentclassifierspaginatorname)
- [ListDominantLanguageDetectionJobsPaginatorName](./literals.md#listdominantlanguagedetectionjobspaginatorname)
- [ListEndpointsPaginatorName](./literals.md#listendpointspaginatorname)
- [ListEntitiesDetectionJobsPaginatorName](./literals.md#listentitiesdetectionjobspaginatorname)
- [ListEntityRecognizersPaginatorName](./literals.md#listentityrecognizerspaginatorname)
- [ListKeyPhrasesDetectionJobsPaginatorName](./literals.md#listkeyphrasesdetectionjobspaginatorname)
- [ListPiiEntitiesDetectionJobsPaginatorName](./literals.md#listpiientitiesdetectionjobspaginatorname)
- [ListSentimentDetectionJobsPaginatorName](./literals.md#listsentimentdetectionjobspaginatorname)
- [ListTopicsDetectionJobsPaginatorName](./literals.md#listtopicsdetectionjobspaginatorname)
- [ModelStatusType](./literals.md#modelstatustype)
- [ModelTypeType](./literals.md#modeltypetype)
- [PageBasedErrorCodeType](./literals.md#pagebasederrorcodetype)
- [PageBasedWarningCodeType](./literals.md#pagebasedwarningcodetype)
- [PartOfSpeechTagTypeType](./literals.md#partofspeechtagtypetype)
- [PiiEntitiesDetectionMaskModeType](./literals.md#piientitiesdetectionmaskmodetype)
- [PiiEntitiesDetectionModeType](./literals.md#piientitiesdetectionmodetype)
- [PiiEntityTypeType](./literals.md#piientitytypetype)
- [RelationshipTypeType](./literals.md#relationshiptypetype)
- [SentimentTypeType](./literals.md#sentimenttypetype)
- [SplitType](./literals.md#splittype)
- [SyntaxLanguageCodeType](./literals.md#syntaxlanguagecodetype)
- [TargetedSentimentEntityTypeType](./literals.md#targetedsentimententitytypetype)
- [ToxicContentTypeType](./literals.md#toxiccontenttypetype)
- [ComprehendServiceName](./literals.md#comprehendservicename)
- [ServiceName](./literals.md#servicename)
- [ResourceServiceName](./literals.md#resourceservicename)
- [PaginatorName](./literals.md#paginatorname)
- [RegionName](./literals.md#regionname)




## Type definitions

Type annotations for [type definitions](./type_defs.md) used in methods and schema.

- [AugmentedManifestsListItemOutputTypeDef](./type_defs.md#augmentedmanifestslistitemoutputtypedef)
- [AugmentedManifestsListItemTypeDef](./type_defs.md#augmentedmanifestslistitemtypedef)
- [DominantLanguageTypeDef](./type_defs.md#dominantlanguagetypedef)
- [BatchDetectDominantLanguageRequestRequestTypeDef](./type_defs.md#batchdetectdominantlanguagerequestrequesttypedef)
- [BatchItemErrorTypeDef](./type_defs.md#batchitemerrortypedef)
- [ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef)
- [BatchDetectEntitiesRequestRequestTypeDef](./type_defs.md#batchdetectentitiesrequestrequesttypedef)
- [KeyPhraseTypeDef](./type_defs.md#keyphrasetypedef)
- [BatchDetectKeyPhrasesRequestRequestTypeDef](./type_defs.md#batchdetectkeyphrasesrequestrequesttypedef)
- [SentimentScoreTypeDef](./type_defs.md#sentimentscoretypedef)
- [BatchDetectSentimentRequestRequestTypeDef](./type_defs.md#batchdetectsentimentrequestrequesttypedef)
- [BatchDetectSyntaxRequestRequestTypeDef](./type_defs.md#batchdetectsyntaxrequestrequesttypedef)
- [BatchDetectTargetedSentimentRequestRequestTypeDef](./type_defs.md#batchdetecttargetedsentimentrequestrequesttypedef)
- [BlobTypeDef](./type_defs.md#blobtypedef)
- [ChildBlockTypeDef](./type_defs.md#childblocktypedef)
- [RelationshipsListItemTypeDef](./type_defs.md#relationshipslistitemtypedef)
- [BoundingBoxTypeDef](./type_defs.md#boundingboxtypedef)
- [ClassifierEvaluationMetricsTypeDef](./type_defs.md#classifierevaluationmetricstypedef)
- [DocumentReaderConfigTypeDef](./type_defs.md#documentreaderconfigtypedef)
- [DocumentClassTypeDef](./type_defs.md#documentclasstypedef)
- [DocumentLabelTypeDef](./type_defs.md#documentlabeltypedef)
- [DocumentTypeListItemTypeDef](./type_defs.md#documenttypelistitemtypedef)
- [ErrorsListItemTypeDef](./type_defs.md#errorslistitemtypedef)
- [WarningsListItemTypeDef](./type_defs.md#warningslistitemtypedef)
- [ContainsPiiEntitiesRequestRequestTypeDef](./type_defs.md#containspiientitiesrequestrequesttypedef)
- [EntityLabelTypeDef](./type_defs.md#entitylabeltypedef)
- [TagTypeDef](./type_defs.md#tagtypedef)
- [DocumentClassifierOutputDataConfigTypeDef](./type_defs.md#documentclassifieroutputdataconfigtypedef)
- [VpcConfigTypeDef](./type_defs.md#vpcconfigtypedef)
- [VpcConfigOutputTypeDef](./type_defs.md#vpcconfigoutputtypedef)
- [DatasetAugmentedManifestsListItemTypeDef](./type_defs.md#datasetaugmentedmanifestslistitemtypedef)
- [DatasetDocumentClassifierInputDataConfigTypeDef](./type_defs.md#datasetdocumentclassifierinputdataconfigtypedef)
- [DatasetEntityRecognizerAnnotationsTypeDef](./type_defs.md#datasetentityrecognizerannotationstypedef)
- [DatasetEntityRecognizerDocumentsTypeDef](./type_defs.md#datasetentityrecognizerdocumentstypedef)
- [DatasetEntityRecognizerEntityListTypeDef](./type_defs.md#datasetentityrecognizerentitylisttypedef)
- [TimestampTypeDef](./type_defs.md#timestamptypedef)
- [DatasetPropertiesTypeDef](./type_defs.md#datasetpropertiestypedef)
- [DeleteDocumentClassifierRequestRequestTypeDef](./type_defs.md#deletedocumentclassifierrequestrequesttypedef)
- [DeleteEndpointRequestRequestTypeDef](./type_defs.md#deleteendpointrequestrequesttypedef)
- [DeleteEntityRecognizerRequestRequestTypeDef](./type_defs.md#deleteentityrecognizerrequestrequesttypedef)
- [DeleteFlywheelRequestRequestTypeDef](./type_defs.md#deleteflywheelrequestrequesttypedef)
- [DeleteResourcePolicyRequestRequestTypeDef](./type_defs.md#deleteresourcepolicyrequestrequesttypedef)
- [DescribeDatasetRequestRequestTypeDef](./type_defs.md#describedatasetrequestrequesttypedef)
- [DescribeDocumentClassificationJobRequestRequestTypeDef](./type_defs.md#describedocumentclassificationjobrequestrequesttypedef)
- [DescribeDocumentClassifierRequestRequestTypeDef](./type_defs.md#describedocumentclassifierrequestrequesttypedef)
- [DescribeDominantLanguageDetectionJobRequestRequestTypeDef](./type_defs.md#describedominantlanguagedetectionjobrequestrequesttypedef)
- [DescribeEndpointRequestRequestTypeDef](./type_defs.md#describeendpointrequestrequesttypedef)
- [EndpointPropertiesTypeDef](./type_defs.md#endpointpropertiestypedef)
- [DescribeEntitiesDetectionJobRequestRequestTypeDef](./type_defs.md#describeentitiesdetectionjobrequestrequesttypedef)
- [DescribeEntityRecognizerRequestRequestTypeDef](./type_defs.md#describeentityrecognizerrequestrequesttypedef)
- [DescribeEventsDetectionJobRequestRequestTypeDef](./type_defs.md#describeeventsdetectionjobrequestrequesttypedef)
- [DescribeFlywheelIterationRequestRequestTypeDef](./type_defs.md#describeflywheeliterationrequestrequesttypedef)
- [DescribeFlywheelRequestRequestTypeDef](./type_defs.md#describeflywheelrequestrequesttypedef)
- [DescribeKeyPhrasesDetectionJobRequestRequestTypeDef](./type_defs.md#describekeyphrasesdetectionjobrequestrequesttypedef)
- [DescribePiiEntitiesDetectionJobRequestRequestTypeDef](./type_defs.md#describepiientitiesdetectionjobrequestrequesttypedef)
- [DescribeResourcePolicyRequestRequestTypeDef](./type_defs.md#describeresourcepolicyrequestrequesttypedef)
- [DescribeSentimentDetectionJobRequestRequestTypeDef](./type_defs.md#describesentimentdetectionjobrequestrequesttypedef)
- [DescribeTargetedSentimentDetectionJobRequestRequestTypeDef](./type_defs.md#describetargetedsentimentdetectionjobrequestrequesttypedef)
- [DescribeTopicsDetectionJobRequestRequestTypeDef](./type_defs.md#describetopicsdetectionjobrequestrequesttypedef)
- [DetectDominantLanguageRequestRequestTypeDef](./type_defs.md#detectdominantlanguagerequestrequesttypedef)
- [DetectKeyPhrasesRequestRequestTypeDef](./type_defs.md#detectkeyphrasesrequestrequesttypedef)
- [DetectPiiEntitiesRequestRequestTypeDef](./type_defs.md#detectpiientitiesrequestrequesttypedef)
- [PiiEntityTypeDef](./type_defs.md#piientitytypedef)
- [DetectSentimentRequestRequestTypeDef](./type_defs.md#detectsentimentrequestrequesttypedef)
- [DetectSyntaxRequestRequestTypeDef](./type_defs.md#detectsyntaxrequestrequesttypedef)
- [DetectTargetedSentimentRequestRequestTypeDef](./type_defs.md#detecttargetedsentimentrequestrequesttypedef)
- [TextSegmentTypeDef](./type_defs.md#textsegmenttypedef)
- [DocumentClassificationConfigOutputTypeDef](./type_defs.md#documentclassificationconfigoutputtypedef)
- [DocumentClassificationConfigTypeDef](./type_defs.md#documentclassificationconfigtypedef)
- [OutputDataConfigTypeDef](./type_defs.md#outputdataconfigtypedef)
- [DocumentClassifierDocumentsTypeDef](./type_defs.md#documentclassifierdocumentstypedef)
- [DocumentReaderConfigOutputTypeDef](./type_defs.md#documentreaderconfigoutputtypedef)
- [DocumentClassifierSummaryTypeDef](./type_defs.md#documentclassifiersummarytypedef)
- [ExtractedCharactersListItemTypeDef](./type_defs.md#extractedcharacterslistitemtypedef)
- [EntityTypesListItemTypeDef](./type_defs.md#entitytypeslistitemtypedef)
- [EntityRecognizerAnnotationsTypeDef](./type_defs.md#entityrecognizerannotationstypedef)
- [EntityRecognizerDocumentsTypeDef](./type_defs.md#entityrecognizerdocumentstypedef)
- [EntityRecognizerEntityListTypeDef](./type_defs.md#entityrecognizerentitylisttypedef)
- [EntityRecognizerEvaluationMetricsTypeDef](./type_defs.md#entityrecognizerevaluationmetricstypedef)
- [EntityTypesEvaluationMetricsTypeDef](./type_defs.md#entitytypesevaluationmetricstypedef)
- [EntityRecognizerOutputDataConfigTypeDef](./type_defs.md#entityrecognizeroutputdataconfigtypedef)
- [EntityRecognizerSummaryTypeDef](./type_defs.md#entityrecognizersummarytypedef)
- [FlywheelModelEvaluationMetricsTypeDef](./type_defs.md#flywheelmodelevaluationmetricstypedef)
- [FlywheelSummaryTypeDef](./type_defs.md#flywheelsummarytypedef)
- [PointTypeDef](./type_defs.md#pointtypedef)
- [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
- [ListDocumentClassifierSummariesRequestRequestTypeDef](./type_defs.md#listdocumentclassifiersummariesrequestrequesttypedef)
- [ListEntityRecognizerSummariesRequestRequestTypeDef](./type_defs.md#listentityrecognizersummariesrequestrequesttypedef)
- [ListTagsForResourceRequestRequestTypeDef](./type_defs.md#listtagsforresourcerequestrequesttypedef)
- [PartOfSpeechTagTypeDef](./type_defs.md#partofspeechtagtypedef)
- [PiiOutputDataConfigTypeDef](./type_defs.md#piioutputdataconfigtypedef)
- [RedactionConfigOutputTypeDef](./type_defs.md#redactionconfigoutputtypedef)
- [PutResourcePolicyRequestRequestTypeDef](./type_defs.md#putresourcepolicyrequestrequesttypedef)
- [RedactionConfigTypeDef](./type_defs.md#redactionconfigtypedef)
- [StartFlywheelIterationRequestRequestTypeDef](./type_defs.md#startflywheeliterationrequestrequesttypedef)
- [StopDominantLanguageDetectionJobRequestRequestTypeDef](./type_defs.md#stopdominantlanguagedetectionjobrequestrequesttypedef)
- [StopEntitiesDetectionJobRequestRequestTypeDef](./type_defs.md#stopentitiesdetectionjobrequestrequesttypedef)
- [StopEventsDetectionJobRequestRequestTypeDef](./type_defs.md#stopeventsdetectionjobrequestrequesttypedef)
- [StopKeyPhrasesDetectionJobRequestRequestTypeDef](./type_defs.md#stopkeyphrasesdetectionjobrequestrequesttypedef)
- [StopPiiEntitiesDetectionJobRequestRequestTypeDef](./type_defs.md#stoppiientitiesdetectionjobrequestrequesttypedef)
- [StopSentimentDetectionJobRequestRequestTypeDef](./type_defs.md#stopsentimentdetectionjobrequestrequesttypedef)
- [StopTargetedSentimentDetectionJobRequestRequestTypeDef](./type_defs.md#stoptargetedsentimentdetectionjobrequestrequesttypedef)
- [StopTrainingDocumentClassifierRequestRequestTypeDef](./type_defs.md#stoptrainingdocumentclassifierrequestrequesttypedef)
- [StopTrainingEntityRecognizerRequestRequestTypeDef](./type_defs.md#stoptrainingentityrecognizerrequestrequesttypedef)
- [ToxicContentTypeDef](./type_defs.md#toxiccontenttypedef)
- [UntagResourceRequestRequestTypeDef](./type_defs.md#untagresourcerequestrequesttypedef)
- [UpdateEndpointRequestRequestTypeDef](./type_defs.md#updateendpointrequestrequesttypedef)
- [AugmentedManifestsListItemUnionTypeDef](./type_defs.md#augmentedmanifestslistitemuniontypedef)
- [BatchDetectDominantLanguageItemResultTypeDef](./type_defs.md#batchdetectdominantlanguageitemresulttypedef)
- [CreateDatasetResponseTypeDef](./type_defs.md#createdatasetresponsetypedef)
- [CreateDocumentClassifierResponseTypeDef](./type_defs.md#createdocumentclassifierresponsetypedef)
- [CreateEndpointResponseTypeDef](./type_defs.md#createendpointresponsetypedef)
- [CreateEntityRecognizerResponseTypeDef](./type_defs.md#createentityrecognizerresponsetypedef)
- [CreateFlywheelResponseTypeDef](./type_defs.md#createflywheelresponsetypedef)
- [DescribeResourcePolicyResponseTypeDef](./type_defs.md#describeresourcepolicyresponsetypedef)
- [DetectDominantLanguageResponseTypeDef](./type_defs.md#detectdominantlanguageresponsetypedef)
- [ImportModelResponseTypeDef](./type_defs.md#importmodelresponsetypedef)
- [PutResourcePolicyResponseTypeDef](./type_defs.md#putresourcepolicyresponsetypedef)
- [StartDocumentClassificationJobResponseTypeDef](./type_defs.md#startdocumentclassificationjobresponsetypedef)
- [StartDominantLanguageDetectionJobResponseTypeDef](./type_defs.md#startdominantlanguagedetectionjobresponsetypedef)
- [StartEntitiesDetectionJobResponseTypeDef](./type_defs.md#startentitiesdetectionjobresponsetypedef)
- [StartEventsDetectionJobResponseTypeDef](./type_defs.md#starteventsdetectionjobresponsetypedef)
- [StartFlywheelIterationResponseTypeDef](./type_defs.md#startflywheeliterationresponsetypedef)
- [StartKeyPhrasesDetectionJobResponseTypeDef](./type_defs.md#startkeyphrasesdetectionjobresponsetypedef)
- [StartPiiEntitiesDetectionJobResponseTypeDef](./type_defs.md#startpiientitiesdetectionjobresponsetypedef)
- [StartSentimentDetectionJobResponseTypeDef](./type_defs.md#startsentimentdetectionjobresponsetypedef)
- [StartTargetedSentimentDetectionJobResponseTypeDef](./type_defs.md#starttargetedsentimentdetectionjobresponsetypedef)
- [StartTopicsDetectionJobResponseTypeDef](./type_defs.md#starttopicsdetectionjobresponsetypedef)
- [StopDominantLanguageDetectionJobResponseTypeDef](./type_defs.md#stopdominantlanguagedetectionjobresponsetypedef)
- [StopEntitiesDetectionJobResponseTypeDef](./type_defs.md#stopentitiesdetectionjobresponsetypedef)
- [StopEventsDetectionJobResponseTypeDef](./type_defs.md#stopeventsdetectionjobresponsetypedef)
- [StopKeyPhrasesDetectionJobResponseTypeDef](./type_defs.md#stopkeyphrasesdetectionjobresponsetypedef)
- [StopPiiEntitiesDetectionJobResponseTypeDef](./type_defs.md#stoppiientitiesdetectionjobresponsetypedef)
- [StopSentimentDetectionJobResponseTypeDef](./type_defs.md#stopsentimentdetectionjobresponsetypedef)
- [StopTargetedSentimentDetectionJobResponseTypeDef](./type_defs.md#stoptargetedsentimentdetectionjobresponsetypedef)
- [UpdateEndpointResponseTypeDef](./type_defs.md#updateendpointresponsetypedef)
- [BatchDetectKeyPhrasesItemResultTypeDef](./type_defs.md#batchdetectkeyphrasesitemresulttypedef)
- [DetectKeyPhrasesResponseTypeDef](./type_defs.md#detectkeyphrasesresponsetypedef)
- [BatchDetectSentimentItemResultTypeDef](./type_defs.md#batchdetectsentimentitemresulttypedef)
- [DetectSentimentResponseTypeDef](./type_defs.md#detectsentimentresponsetypedef)
- [MentionSentimentTypeDef](./type_defs.md#mentionsentimenttypedef)
- [BlockReferenceTypeDef](./type_defs.md#blockreferencetypedef)
- [ClassifierMetadataTypeDef](./type_defs.md#classifiermetadatatypedef)
- [ClassifyDocumentRequestRequestTypeDef](./type_defs.md#classifydocumentrequestrequesttypedef)
- [DetectEntitiesRequestRequestTypeDef](./type_defs.md#detectentitiesrequestrequesttypedef)
- [ContainsPiiEntitiesResponseTypeDef](./type_defs.md#containspiientitiesresponsetypedef)
- [CreateEndpointRequestRequestTypeDef](./type_defs.md#createendpointrequestrequesttypedef)
- [ImportModelRequestRequestTypeDef](./type_defs.md#importmodelrequestrequesttypedef)
- [ListTagsForResourceResponseTypeDef](./type_defs.md#listtagsforresourceresponsetypedef)
- [TagResourceRequestRequestTypeDef](./type_defs.md#tagresourcerequestrequesttypedef)
- [DataSecurityConfigOutputTypeDef](./type_defs.md#datasecurityconfigoutputtypedef)
- [VpcConfigUnionTypeDef](./type_defs.md#vpcconfiguniontypedef)
- [DatasetEntityRecognizerInputDataConfigTypeDef](./type_defs.md#datasetentityrecognizerinputdataconfigtypedef)
- [DatasetFilterTypeDef](./type_defs.md#datasetfiltertypedef)
- [DocumentClassificationJobFilterTypeDef](./type_defs.md#documentclassificationjobfiltertypedef)
- [DocumentClassifierFilterTypeDef](./type_defs.md#documentclassifierfiltertypedef)
- [DominantLanguageDetectionJobFilterTypeDef](./type_defs.md#dominantlanguagedetectionjobfiltertypedef)
- [EndpointFilterTypeDef](./type_defs.md#endpointfiltertypedef)
- [EntitiesDetectionJobFilterTypeDef](./type_defs.md#entitiesdetectionjobfiltertypedef)
- [EntityRecognizerFilterTypeDef](./type_defs.md#entityrecognizerfiltertypedef)
- [EventsDetectionJobFilterTypeDef](./type_defs.md#eventsdetectionjobfiltertypedef)
- [FlywheelFilterTypeDef](./type_defs.md#flywheelfiltertypedef)
- [FlywheelIterationFilterTypeDef](./type_defs.md#flywheeliterationfiltertypedef)
- [KeyPhrasesDetectionJobFilterTypeDef](./type_defs.md#keyphrasesdetectionjobfiltertypedef)
- [PiiEntitiesDetectionJobFilterTypeDef](./type_defs.md#piientitiesdetectionjobfiltertypedef)
- [SentimentDetectionJobFilterTypeDef](./type_defs.md#sentimentdetectionjobfiltertypedef)
- [TargetedSentimentDetectionJobFilterTypeDef](./type_defs.md#targetedsentimentdetectionjobfiltertypedef)
- [TopicsDetectionJobFilterTypeDef](./type_defs.md#topicsdetectionjobfiltertypedef)
- [DescribeDatasetResponseTypeDef](./type_defs.md#describedatasetresponsetypedef)
- [ListDatasetsResponseTypeDef](./type_defs.md#listdatasetsresponsetypedef)
- [DescribeEndpointResponseTypeDef](./type_defs.md#describeendpointresponsetypedef)
- [ListEndpointsResponseTypeDef](./type_defs.md#listendpointsresponsetypedef)
- [DetectPiiEntitiesResponseTypeDef](./type_defs.md#detectpiientitiesresponsetypedef)
- [DetectToxicContentRequestRequestTypeDef](./type_defs.md#detecttoxiccontentrequestrequesttypedef)
- [DocumentClassificationConfigUnionTypeDef](./type_defs.md#documentclassificationconfiguniontypedef)
- [DocumentClassifierInputDataConfigOutputTypeDef](./type_defs.md#documentclassifierinputdataconfigoutputtypedef)
- [DocumentReaderConfigUnionTypeDef](./type_defs.md#documentreaderconfiguniontypedef)
- [InputDataConfigOutputTypeDef](./type_defs.md#inputdataconfigoutputtypedef)
- [ListDocumentClassifierSummariesResponseTypeDef](./type_defs.md#listdocumentclassifiersummariesresponsetypedef)
- [DocumentMetadataTypeDef](./type_defs.md#documentmetadatatypedef)
- [EntityRecognitionConfigOutputTypeDef](./type_defs.md#entityrecognitionconfigoutputtypedef)
- [EntityRecognitionConfigTypeDef](./type_defs.md#entityrecognitionconfigtypedef)
- [EntityRecognizerInputDataConfigOutputTypeDef](./type_defs.md#entityrecognizerinputdataconfigoutputtypedef)
- [EntityRecognizerMetadataEntityTypesListItemTypeDef](./type_defs.md#entityrecognizermetadataentitytypeslistitemtypedef)
- [ListEntityRecognizerSummariesResponseTypeDef](./type_defs.md#listentityrecognizersummariesresponsetypedef)
- [FlywheelIterationPropertiesTypeDef](./type_defs.md#flywheeliterationpropertiestypedef)
- [ListFlywheelsResponseTypeDef](./type_defs.md#listflywheelsresponsetypedef)
- [GeometryTypeDef](./type_defs.md#geometrytypedef)
- [SyntaxTokenTypeDef](./type_defs.md#syntaxtokentypedef)
- [ToxicLabelsTypeDef](./type_defs.md#toxiclabelstypedef)
- [EntityRecognizerInputDataConfigTypeDef](./type_defs.md#entityrecognizerinputdataconfigtypedef)
- [BatchDetectDominantLanguageResponseTypeDef](./type_defs.md#batchdetectdominantlanguageresponsetypedef)
- [BatchDetectKeyPhrasesResponseTypeDef](./type_defs.md#batchdetectkeyphrasesresponsetypedef)
- [BatchDetectSentimentResponseTypeDef](./type_defs.md#batchdetectsentimentresponsetypedef)
- [TargetedSentimentMentionTypeDef](./type_defs.md#targetedsentimentmentiontypedef)
- [EntityTypeDef](./type_defs.md#entitytypedef)
- [DataSecurityConfigTypeDef](./type_defs.md#datasecurityconfigtypedef)
- [UpdateDataSecurityConfigTypeDef](./type_defs.md#updatedatasecurityconfigtypedef)
- [DatasetInputDataConfigTypeDef](./type_defs.md#datasetinputdataconfigtypedef)
- [ListDatasetsRequestRequestTypeDef](./type_defs.md#listdatasetsrequestrequesttypedef)
- [ListDocumentClassificationJobsRequestPaginateTypeDef](./type_defs.md#listdocumentclassificationjobsrequestpaginatetypedef)
- [ListDocumentClassificationJobsRequestRequestTypeDef](./type_defs.md#listdocumentclassificationjobsrequestrequesttypedef)
- [ListDocumentClassifiersRequestPaginateTypeDef](./type_defs.md#listdocumentclassifiersrequestpaginatetypedef)
- [ListDocumentClassifiersRequestRequestTypeDef](./type_defs.md#listdocumentclassifiersrequestrequesttypedef)
- [ListDominantLanguageDetectionJobsRequestPaginateTypeDef](./type_defs.md#listdominantlanguagedetectionjobsrequestpaginatetypedef)
- [ListDominantLanguageDetectionJobsRequestRequestTypeDef](./type_defs.md#listdominantlanguagedetectionjobsrequestrequesttypedef)
- [ListEndpointsRequestPaginateTypeDef](./type_defs.md#listendpointsrequestpaginatetypedef)
- [ListEndpointsRequestRequestTypeDef](./type_defs.md#listendpointsrequestrequesttypedef)
- [ListEntitiesDetectionJobsRequestPaginateTypeDef](./type_defs.md#listentitiesdetectionjobsrequestpaginatetypedef)
- [ListEntitiesDetectionJobsRequestRequestTypeDef](./type_defs.md#listentitiesdetectionjobsrequestrequesttypedef)
- [ListEntityRecognizersRequestPaginateTypeDef](./type_defs.md#listentityrecognizersrequestpaginatetypedef)
- [ListEntityRecognizersRequestRequestTypeDef](./type_defs.md#listentityrecognizersrequestrequesttypedef)
- [ListEventsDetectionJobsRequestRequestTypeDef](./type_defs.md#listeventsdetectionjobsrequestrequesttypedef)
- [ListFlywheelsRequestRequestTypeDef](./type_defs.md#listflywheelsrequestrequesttypedef)
- [ListFlywheelIterationHistoryRequestRequestTypeDef](./type_defs.md#listflywheeliterationhistoryrequestrequesttypedef)
- [ListKeyPhrasesDetectionJobsRequestPaginateTypeDef](./type_defs.md#listkeyphrasesdetectionjobsrequestpaginatetypedef)
- [ListKeyPhrasesDetectionJobsRequestRequestTypeDef](./type_defs.md#listkeyphrasesdetectionjobsrequestrequesttypedef)
- [ListPiiEntitiesDetectionJobsRequestPaginateTypeDef](./type_defs.md#listpiientitiesdetectionjobsrequestpaginatetypedef)
- [ListPiiEntitiesDetectionJobsRequestRequestTypeDef](./type_defs.md#listpiientitiesdetectionjobsrequestrequesttypedef)
- [ListSentimentDetectionJobsRequestPaginateTypeDef](./type_defs.md#listsentimentdetectionjobsrequestpaginatetypedef)
- [ListSentimentDetectionJobsRequestRequestTypeDef](./type_defs.md#listsentimentdetectionjobsrequestrequesttypedef)
- [ListTargetedSentimentDetectionJobsRequestRequestTypeDef](./type_defs.md#listtargetedsentimentdetectionjobsrequestrequesttypedef)
- [ListTopicsDetectionJobsRequestPaginateTypeDef](./type_defs.md#listtopicsdetectionjobsrequestpaginatetypedef)
- [ListTopicsDetectionJobsRequestRequestTypeDef](./type_defs.md#listtopicsdetectionjobsrequestrequesttypedef)
- [DocumentClassifierPropertiesTypeDef](./type_defs.md#documentclassifierpropertiestypedef)
- [DocumentClassifierInputDataConfigTypeDef](./type_defs.md#documentclassifierinputdataconfigtypedef)
- [InputDataConfigTypeDef](./type_defs.md#inputdataconfigtypedef)
- [DocumentClassificationJobPropertiesTypeDef](./type_defs.md#documentclassificationjobpropertiestypedef)
- [DominantLanguageDetectionJobPropertiesTypeDef](./type_defs.md#dominantlanguagedetectionjobpropertiestypedef)
- [EntitiesDetectionJobPropertiesTypeDef](./type_defs.md#entitiesdetectionjobpropertiestypedef)
- [EventsDetectionJobPropertiesTypeDef](./type_defs.md#eventsdetectionjobpropertiestypedef)
- [KeyPhrasesDetectionJobPropertiesTypeDef](./type_defs.md#keyphrasesdetectionjobpropertiestypedef)
- [PiiEntitiesDetectionJobPropertiesTypeDef](./type_defs.md#piientitiesdetectionjobpropertiestypedef)
- [SentimentDetectionJobPropertiesTypeDef](./type_defs.md#sentimentdetectionjobpropertiestypedef)
- [TargetedSentimentDetectionJobPropertiesTypeDef](./type_defs.md#targetedsentimentdetectionjobpropertiestypedef)
- [TopicsDetectionJobPropertiesTypeDef](./type_defs.md#topicsdetectionjobpropertiestypedef)
- [ClassifyDocumentResponseTypeDef](./type_defs.md#classifydocumentresponsetypedef)
- [TaskConfigOutputTypeDef](./type_defs.md#taskconfigoutputtypedef)
- [EntityRecognitionConfigUnionTypeDef](./type_defs.md#entityrecognitionconfiguniontypedef)
- [EntityRecognizerMetadataTypeDef](./type_defs.md#entityrecognizermetadatatypedef)
- [DescribeFlywheelIterationResponseTypeDef](./type_defs.md#describeflywheeliterationresponsetypedef)
- [ListFlywheelIterationHistoryResponseTypeDef](./type_defs.md#listflywheeliterationhistoryresponsetypedef)
- [BlockTypeDef](./type_defs.md#blocktypedef)
- [BatchDetectSyntaxItemResultTypeDef](./type_defs.md#batchdetectsyntaxitemresulttypedef)
- [DetectSyntaxResponseTypeDef](./type_defs.md#detectsyntaxresponsetypedef)
- [DetectToxicContentResponseTypeDef](./type_defs.md#detecttoxiccontentresponsetypedef)
- [CreateEntityRecognizerRequestRequestTypeDef](./type_defs.md#createentityrecognizerrequestrequesttypedef)
- [TargetedSentimentEntityTypeDef](./type_defs.md#targetedsentimententitytypedef)
- [BatchDetectEntitiesItemResultTypeDef](./type_defs.md#batchdetectentitiesitemresulttypedef)
- [UpdateFlywheelRequestRequestTypeDef](./type_defs.md#updateflywheelrequestrequesttypedef)
- [CreateDatasetRequestRequestTypeDef](./type_defs.md#createdatasetrequestrequesttypedef)
- [DescribeDocumentClassifierResponseTypeDef](./type_defs.md#describedocumentclassifierresponsetypedef)
- [ListDocumentClassifiersResponseTypeDef](./type_defs.md#listdocumentclassifiersresponsetypedef)
- [CreateDocumentClassifierRequestRequestTypeDef](./type_defs.md#createdocumentclassifierrequestrequesttypedef)
- [StartDocumentClassificationJobRequestRequestTypeDef](./type_defs.md#startdocumentclassificationjobrequestrequesttypedef)
- [StartDominantLanguageDetectionJobRequestRequestTypeDef](./type_defs.md#startdominantlanguagedetectionjobrequestrequesttypedef)
- [StartEntitiesDetectionJobRequestRequestTypeDef](./type_defs.md#startentitiesdetectionjobrequestrequesttypedef)
- [StartEventsDetectionJobRequestRequestTypeDef](./type_defs.md#starteventsdetectionjobrequestrequesttypedef)
- [StartKeyPhrasesDetectionJobRequestRequestTypeDef](./type_defs.md#startkeyphrasesdetectionjobrequestrequesttypedef)
- [StartPiiEntitiesDetectionJobRequestRequestTypeDef](./type_defs.md#startpiientitiesdetectionjobrequestrequesttypedef)
- [StartSentimentDetectionJobRequestRequestTypeDef](./type_defs.md#startsentimentdetectionjobrequestrequesttypedef)
- [StartTargetedSentimentDetectionJobRequestRequestTypeDef](./type_defs.md#starttargetedsentimentdetectionjobrequestrequesttypedef)
- [StartTopicsDetectionJobRequestRequestTypeDef](./type_defs.md#starttopicsdetectionjobrequestrequesttypedef)
- [DescribeDocumentClassificationJobResponseTypeDef](./type_defs.md#describedocumentclassificationjobresponsetypedef)
- [ListDocumentClassificationJobsResponseTypeDef](./type_defs.md#listdocumentclassificationjobsresponsetypedef)
- [DescribeDominantLanguageDetectionJobResponseTypeDef](./type_defs.md#describedominantlanguagedetectionjobresponsetypedef)
- [ListDominantLanguageDetectionJobsResponseTypeDef](./type_defs.md#listdominantlanguagedetectionjobsresponsetypedef)
- [DescribeEntitiesDetectionJobResponseTypeDef](./type_defs.md#describeentitiesdetectionjobresponsetypedef)
- [ListEntitiesDetectionJobsResponseTypeDef](./type_defs.md#listentitiesdetectionjobsresponsetypedef)
- [DescribeEventsDetectionJobResponseTypeDef](./type_defs.md#describeeventsdetectionjobresponsetypedef)
- [ListEventsDetectionJobsResponseTypeDef](./type_defs.md#listeventsdetectionjobsresponsetypedef)
- [DescribeKeyPhrasesDetectionJobResponseTypeDef](./type_defs.md#describekeyphrasesdetectionjobresponsetypedef)
- [ListKeyPhrasesDetectionJobsResponseTypeDef](./type_defs.md#listkeyphrasesdetectionjobsresponsetypedef)
- [DescribePiiEntitiesDetectionJobResponseTypeDef](./type_defs.md#describepiientitiesdetectionjobresponsetypedef)
- [ListPiiEntitiesDetectionJobsResponseTypeDef](./type_defs.md#listpiientitiesdetectionjobsresponsetypedef)
- [DescribeSentimentDetectionJobResponseTypeDef](./type_defs.md#describesentimentdetectionjobresponsetypedef)
- [ListSentimentDetectionJobsResponseTypeDef](./type_defs.md#listsentimentdetectionjobsresponsetypedef)
- [DescribeTargetedSentimentDetectionJobResponseTypeDef](./type_defs.md#describetargetedsentimentdetectionjobresponsetypedef)
- [ListTargetedSentimentDetectionJobsResponseTypeDef](./type_defs.md#listtargetedsentimentdetectionjobsresponsetypedef)
- [DescribeTopicsDetectionJobResponseTypeDef](./type_defs.md#describetopicsdetectionjobresponsetypedef)
- [ListTopicsDetectionJobsResponseTypeDef](./type_defs.md#listtopicsdetectionjobsresponsetypedef)
- [FlywheelPropertiesTypeDef](./type_defs.md#flywheelpropertiestypedef)
- [TaskConfigTypeDef](./type_defs.md#taskconfigtypedef)
- [EntityRecognizerPropertiesTypeDef](./type_defs.md#entityrecognizerpropertiestypedef)
- [DetectEntitiesResponseTypeDef](./type_defs.md#detectentitiesresponsetypedef)
- [BatchDetectSyntaxResponseTypeDef](./type_defs.md#batchdetectsyntaxresponsetypedef)
- [BatchDetectTargetedSentimentItemResultTypeDef](./type_defs.md#batchdetecttargetedsentimentitemresulttypedef)
- [DetectTargetedSentimentResponseTypeDef](./type_defs.md#detecttargetedsentimentresponsetypedef)
- [BatchDetectEntitiesResponseTypeDef](./type_defs.md#batchdetectentitiesresponsetypedef)
- [DescribeFlywheelResponseTypeDef](./type_defs.md#describeflywheelresponsetypedef)
- [UpdateFlywheelResponseTypeDef](./type_defs.md#updateflywheelresponsetypedef)
- [CreateFlywheelRequestRequestTypeDef](./type_defs.md#createflywheelrequestrequesttypedef)
- [DescribeEntityRecognizerResponseTypeDef](./type_defs.md#describeentityrecognizerresponsetypedef)
- [ListEntityRecognizersResponseTypeDef](./type_defs.md#listentityrecognizersresponsetypedef)
- [BatchDetectTargetedSentimentResponseTypeDef](./type_defs.md#batchdetecttargetedsentimentresponsetypedef)

