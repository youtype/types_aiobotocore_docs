# Type definitions

> [Index](../README.md) > [ComprehendMedical](./README.md) > Type definitions

!!! note ""

    Auto-generated documentation for [ComprehendMedical](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/comprehendmedical.html#ComprehendMedical)
    type annotations stubs module [types-aiobotocore-comprehendmedical](https://pypi.org/project/types-aiobotocore-comprehendmedical/).

## TimestampTypeDef

```python
# TimestampTypeDef definition

TimestampTypeDef = Union[
    datetime,
    str,
]
```




## TraitTypeDef

```python
# TraitTypeDef definition

class TraitTypeDef(TypedDict):
    Name: NotRequired[AttributeNameType],  # (1)
    Score: NotRequired[float],
```

1. See [:material-code-brackets: AttributeNameType](./literals.md#attributenametype) 
## CharactersTypeDef

```python
# CharactersTypeDef definition

class CharactersTypeDef(TypedDict):
    OriginalTextCharacters: NotRequired[int],
```

## InputDataConfigTypeDef

```python
# InputDataConfigTypeDef definition

class InputDataConfigTypeDef(TypedDict):
    S3Bucket: str,
    S3Key: NotRequired[str],
```

## OutputDataConfigTypeDef

```python
# OutputDataConfigTypeDef definition

class OutputDataConfigTypeDef(TypedDict):
    S3Bucket: str,
    S3Key: NotRequired[str],
```

## DescribeEntitiesDetectionV2JobRequestRequestTypeDef

```python
# DescribeEntitiesDetectionV2JobRequestRequestTypeDef definition

class DescribeEntitiesDetectionV2JobRequestRequestTypeDef(TypedDict):
    JobId: str,
```

## ResponseMetadataTypeDef

```python
# ResponseMetadataTypeDef definition

class ResponseMetadataTypeDef(TypedDict):
    RequestId: str,
    HTTPStatusCode: int,
    HTTPHeaders: Dict[str, str],
    RetryAttempts: int,
    HostId: NotRequired[str],
```

## DescribeICD10CMInferenceJobRequestRequestTypeDef

```python
# DescribeICD10CMInferenceJobRequestRequestTypeDef definition

class DescribeICD10CMInferenceJobRequestRequestTypeDef(TypedDict):
    JobId: str,
```

## DescribePHIDetectionJobRequestRequestTypeDef

```python
# DescribePHIDetectionJobRequestRequestTypeDef definition

class DescribePHIDetectionJobRequestRequestTypeDef(TypedDict):
    JobId: str,
```

## DescribeRxNormInferenceJobRequestRequestTypeDef

```python
# DescribeRxNormInferenceJobRequestRequestTypeDef definition

class DescribeRxNormInferenceJobRequestRequestTypeDef(TypedDict):
    JobId: str,
```

## DescribeSNOMEDCTInferenceJobRequestRequestTypeDef

```python
# DescribeSNOMEDCTInferenceJobRequestRequestTypeDef definition

class DescribeSNOMEDCTInferenceJobRequestRequestTypeDef(TypedDict):
    JobId: str,
```

## DetectEntitiesRequestRequestTypeDef

```python
# DetectEntitiesRequestRequestTypeDef definition

class DetectEntitiesRequestRequestTypeDef(TypedDict):
    Text: str,
```

## DetectEntitiesV2RequestRequestTypeDef

```python
# DetectEntitiesV2RequestRequestTypeDef definition

class DetectEntitiesV2RequestRequestTypeDef(TypedDict):
    Text: str,
```

## DetectPHIRequestRequestTypeDef

```python
# DetectPHIRequestRequestTypeDef definition

class DetectPHIRequestRequestTypeDef(TypedDict):
    Text: str,
```

## ICD10CMTraitTypeDef

```python
# ICD10CMTraitTypeDef definition

class ICD10CMTraitTypeDef(TypedDict):
    Name: NotRequired[ICD10CMTraitNameType],  # (1)
    Score: NotRequired[float],
```

1. See [:material-code-brackets: ICD10CMTraitNameType](./literals.md#icd10cmtraitnametype) 
## ICD10CMConceptTypeDef

```python
# ICD10CMConceptTypeDef definition

class ICD10CMConceptTypeDef(TypedDict):
    Description: NotRequired[str],
    Code: NotRequired[str],
    Score: NotRequired[float],
```

## InferICD10CMRequestRequestTypeDef

```python
# InferICD10CMRequestRequestTypeDef definition

class InferICD10CMRequestRequestTypeDef(TypedDict):
    Text: str,
```

## InferRxNormRequestRequestTypeDef

```python
# InferRxNormRequestRequestTypeDef definition

class InferRxNormRequestRequestTypeDef(TypedDict):
    Text: str,
```

## InferSNOMEDCTRequestRequestTypeDef

```python
# InferSNOMEDCTRequestRequestTypeDef definition

class InferSNOMEDCTRequestRequestTypeDef(TypedDict):
    Text: str,
```

## SNOMEDCTDetailsTypeDef

```python
# SNOMEDCTDetailsTypeDef definition

class SNOMEDCTDetailsTypeDef(TypedDict):
    Edition: NotRequired[str],
    Language: NotRequired[str],
    VersionDate: NotRequired[str],
```

## RxNormTraitTypeDef

```python
# RxNormTraitTypeDef definition

class RxNormTraitTypeDef(TypedDict):
    Name: NotRequired[RxNormTraitNameType],  # (1)
    Score: NotRequired[float],
```

1. See [:material-code-brackets: RxNormTraitNameType](./literals.md#rxnormtraitnametype) 
## RxNormConceptTypeDef

```python
# RxNormConceptTypeDef definition

class RxNormConceptTypeDef(TypedDict):
    Description: NotRequired[str],
    Code: NotRequired[str],
    Score: NotRequired[float],
```

## SNOMEDCTConceptTypeDef

```python
# SNOMEDCTConceptTypeDef definition

class SNOMEDCTConceptTypeDef(TypedDict):
    Description: NotRequired[str],
    Code: NotRequired[str],
    Score: NotRequired[float],
```

## SNOMEDCTTraitTypeDef

```python
# SNOMEDCTTraitTypeDef definition

class SNOMEDCTTraitTypeDef(TypedDict):
    Name: NotRequired[SNOMEDCTTraitNameType],  # (1)
    Score: NotRequired[float],
```

1. See [:material-code-brackets: SNOMEDCTTraitNameType](./literals.md#snomedcttraitnametype) 
## StopEntitiesDetectionV2JobRequestRequestTypeDef

```python
# StopEntitiesDetectionV2JobRequestRequestTypeDef definition

class StopEntitiesDetectionV2JobRequestRequestTypeDef(TypedDict):
    JobId: str,
```

## StopICD10CMInferenceJobRequestRequestTypeDef

```python
# StopICD10CMInferenceJobRequestRequestTypeDef definition

class StopICD10CMInferenceJobRequestRequestTypeDef(TypedDict):
    JobId: str,
```

## StopPHIDetectionJobRequestRequestTypeDef

```python
# StopPHIDetectionJobRequestRequestTypeDef definition

class StopPHIDetectionJobRequestRequestTypeDef(TypedDict):
    JobId: str,
```

## StopRxNormInferenceJobRequestRequestTypeDef

```python
# StopRxNormInferenceJobRequestRequestTypeDef definition

class StopRxNormInferenceJobRequestRequestTypeDef(TypedDict):
    JobId: str,
```

## StopSNOMEDCTInferenceJobRequestRequestTypeDef

```python
# StopSNOMEDCTInferenceJobRequestRequestTypeDef definition

class StopSNOMEDCTInferenceJobRequestRequestTypeDef(TypedDict):
    JobId: str,
```

## AttributeTypeDef

```python
# AttributeTypeDef definition

class AttributeTypeDef(TypedDict):
    Type: NotRequired[EntitySubTypeType],  # (1)
    Score: NotRequired[float],
    RelationshipScore: NotRequired[float],
    RelationshipType: NotRequired[RelationshipTypeType],  # (2)
    Id: NotRequired[int],
    BeginOffset: NotRequired[int],
    EndOffset: NotRequired[int],
    Text: NotRequired[str],
    Category: NotRequired[EntityTypeType],  # (3)
    Traits: NotRequired[List[TraitTypeDef]],  # (4)
```

1. See [:material-code-brackets: EntitySubTypeType](./literals.md#entitysubtypetype) 
2. See [:material-code-brackets: RelationshipTypeType](./literals.md#relationshiptypetype) 
3. See [:material-code-brackets: EntityTypeType](./literals.md#entitytypetype) 
4. See [:material-code-braces: TraitTypeDef](./type_defs.md#traittypedef) 
## ComprehendMedicalAsyncJobFilterTypeDef

```python
# ComprehendMedicalAsyncJobFilterTypeDef definition

class ComprehendMedicalAsyncJobFilterTypeDef(TypedDict):
    JobName: NotRequired[str],
    JobStatus: NotRequired[JobStatusType],  # (1)
    SubmitTimeBefore: NotRequired[TimestampTypeDef],
    SubmitTimeAfter: NotRequired[TimestampTypeDef],
```

1. See [:material-code-brackets: JobStatusType](./literals.md#jobstatustype) 
## ComprehendMedicalAsyncJobPropertiesTypeDef

```python
# ComprehendMedicalAsyncJobPropertiesTypeDef definition

class ComprehendMedicalAsyncJobPropertiesTypeDef(TypedDict):
    JobId: NotRequired[str],
    JobName: NotRequired[str],
    JobStatus: NotRequired[JobStatusType],  # (1)
    Message: NotRequired[str],
    SubmitTime: NotRequired[datetime],
    EndTime: NotRequired[datetime],
    ExpirationTime: NotRequired[datetime],
    InputDataConfig: NotRequired[InputDataConfigTypeDef],  # (2)
    OutputDataConfig: NotRequired[OutputDataConfigTypeDef],  # (3)
    LanguageCode: NotRequired[LanguageCodeType],  # (4)
    DataAccessRoleArn: NotRequired[str],
    ManifestFilePath: NotRequired[str],
    KMSKey: NotRequired[str],
    ModelVersion: NotRequired[str],
```

1. See [:material-code-brackets: JobStatusType](./literals.md#jobstatustype) 
2. See [:material-code-braces: InputDataConfigTypeDef](./type_defs.md#inputdataconfigtypedef) 
3. See [:material-code-braces: OutputDataConfigTypeDef](./type_defs.md#outputdataconfigtypedef) 
4. See [:material-code-brackets: LanguageCodeType](./literals.md#languagecodetype) 
## StartEntitiesDetectionV2JobRequestRequestTypeDef

```python
# StartEntitiesDetectionV2JobRequestRequestTypeDef definition

class StartEntitiesDetectionV2JobRequestRequestTypeDef(TypedDict):
    InputDataConfig: InputDataConfigTypeDef,  # (1)
    OutputDataConfig: OutputDataConfigTypeDef,  # (2)
    DataAccessRoleArn: str,
    LanguageCode: LanguageCodeType,  # (3)
    JobName: NotRequired[str],
    ClientRequestToken: NotRequired[str],
    KMSKey: NotRequired[str],
```

1. See [:material-code-braces: InputDataConfigTypeDef](./type_defs.md#inputdataconfigtypedef) 
2. See [:material-code-braces: OutputDataConfigTypeDef](./type_defs.md#outputdataconfigtypedef) 
3. See [:material-code-brackets: LanguageCodeType](./literals.md#languagecodetype) 
## StartICD10CMInferenceJobRequestRequestTypeDef

```python
# StartICD10CMInferenceJobRequestRequestTypeDef definition

class StartICD10CMInferenceJobRequestRequestTypeDef(TypedDict):
    InputDataConfig: InputDataConfigTypeDef,  # (1)
    OutputDataConfig: OutputDataConfigTypeDef,  # (2)
    DataAccessRoleArn: str,
    LanguageCode: LanguageCodeType,  # (3)
    JobName: NotRequired[str],
    ClientRequestToken: NotRequired[str],
    KMSKey: NotRequired[str],
```

1. See [:material-code-braces: InputDataConfigTypeDef](./type_defs.md#inputdataconfigtypedef) 
2. See [:material-code-braces: OutputDataConfigTypeDef](./type_defs.md#outputdataconfigtypedef) 
3. See [:material-code-brackets: LanguageCodeType](./literals.md#languagecodetype) 
## StartPHIDetectionJobRequestRequestTypeDef

```python
# StartPHIDetectionJobRequestRequestTypeDef definition

class StartPHIDetectionJobRequestRequestTypeDef(TypedDict):
    InputDataConfig: InputDataConfigTypeDef,  # (1)
    OutputDataConfig: OutputDataConfigTypeDef,  # (2)
    DataAccessRoleArn: str,
    LanguageCode: LanguageCodeType,  # (3)
    JobName: NotRequired[str],
    ClientRequestToken: NotRequired[str],
    KMSKey: NotRequired[str],
```

1. See [:material-code-braces: InputDataConfigTypeDef](./type_defs.md#inputdataconfigtypedef) 
2. See [:material-code-braces: OutputDataConfigTypeDef](./type_defs.md#outputdataconfigtypedef) 
3. See [:material-code-brackets: LanguageCodeType](./literals.md#languagecodetype) 
## StartRxNormInferenceJobRequestRequestTypeDef

```python
# StartRxNormInferenceJobRequestRequestTypeDef definition

class StartRxNormInferenceJobRequestRequestTypeDef(TypedDict):
    InputDataConfig: InputDataConfigTypeDef,  # (1)
    OutputDataConfig: OutputDataConfigTypeDef,  # (2)
    DataAccessRoleArn: str,
    LanguageCode: LanguageCodeType,  # (3)
    JobName: NotRequired[str],
    ClientRequestToken: NotRequired[str],
    KMSKey: NotRequired[str],
```

1. See [:material-code-braces: InputDataConfigTypeDef](./type_defs.md#inputdataconfigtypedef) 
2. See [:material-code-braces: OutputDataConfigTypeDef](./type_defs.md#outputdataconfigtypedef) 
3. See [:material-code-brackets: LanguageCodeType](./literals.md#languagecodetype) 
## StartSNOMEDCTInferenceJobRequestRequestTypeDef

```python
# StartSNOMEDCTInferenceJobRequestRequestTypeDef definition

class StartSNOMEDCTInferenceJobRequestRequestTypeDef(TypedDict):
    InputDataConfig: InputDataConfigTypeDef,  # (1)
    OutputDataConfig: OutputDataConfigTypeDef,  # (2)
    DataAccessRoleArn: str,
    LanguageCode: LanguageCodeType,  # (3)
    JobName: NotRequired[str],
    ClientRequestToken: NotRequired[str],
    KMSKey: NotRequired[str],
```

1. See [:material-code-braces: InputDataConfigTypeDef](./type_defs.md#inputdataconfigtypedef) 
2. See [:material-code-braces: OutputDataConfigTypeDef](./type_defs.md#outputdataconfigtypedef) 
3. See [:material-code-brackets: LanguageCodeType](./literals.md#languagecodetype) 
## StartEntitiesDetectionV2JobResponseTypeDef

```python
# StartEntitiesDetectionV2JobResponseTypeDef definition

class StartEntitiesDetectionV2JobResponseTypeDef(TypedDict):
    JobId: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## StartICD10CMInferenceJobResponseTypeDef

```python
# StartICD10CMInferenceJobResponseTypeDef definition

class StartICD10CMInferenceJobResponseTypeDef(TypedDict):
    JobId: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## StartPHIDetectionJobResponseTypeDef

```python
# StartPHIDetectionJobResponseTypeDef definition

class StartPHIDetectionJobResponseTypeDef(TypedDict):
    JobId: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## StartRxNormInferenceJobResponseTypeDef

```python
# StartRxNormInferenceJobResponseTypeDef definition

class StartRxNormInferenceJobResponseTypeDef(TypedDict):
    JobId: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## StartSNOMEDCTInferenceJobResponseTypeDef

```python
# StartSNOMEDCTInferenceJobResponseTypeDef definition

class StartSNOMEDCTInferenceJobResponseTypeDef(TypedDict):
    JobId: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## StopEntitiesDetectionV2JobResponseTypeDef

```python
# StopEntitiesDetectionV2JobResponseTypeDef definition

class StopEntitiesDetectionV2JobResponseTypeDef(TypedDict):
    JobId: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## StopICD10CMInferenceJobResponseTypeDef

```python
# StopICD10CMInferenceJobResponseTypeDef definition

class StopICD10CMInferenceJobResponseTypeDef(TypedDict):
    JobId: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## StopPHIDetectionJobResponseTypeDef

```python
# StopPHIDetectionJobResponseTypeDef definition

class StopPHIDetectionJobResponseTypeDef(TypedDict):
    JobId: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## StopRxNormInferenceJobResponseTypeDef

```python
# StopRxNormInferenceJobResponseTypeDef definition

class StopRxNormInferenceJobResponseTypeDef(TypedDict):
    JobId: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## StopSNOMEDCTInferenceJobResponseTypeDef

```python
# StopSNOMEDCTInferenceJobResponseTypeDef definition

class StopSNOMEDCTInferenceJobResponseTypeDef(TypedDict):
    JobId: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ICD10CMAttributeTypeDef

```python
# ICD10CMAttributeTypeDef definition

class ICD10CMAttributeTypeDef(TypedDict):
    Type: NotRequired[ICD10CMAttributeTypeType],  # (1)
    Score: NotRequired[float],
    RelationshipScore: NotRequired[float],
    Id: NotRequired[int],
    BeginOffset: NotRequired[int],
    EndOffset: NotRequired[int],
    Text: NotRequired[str],
    Traits: NotRequired[List[ICD10CMTraitTypeDef]],  # (2)
    Category: NotRequired[ICD10CMEntityTypeType],  # (3)
    RelationshipType: NotRequired[ICD10CMRelationshipTypeType],  # (4)
```

1. See [:material-code-brackets: ICD10CMAttributeTypeType](./literals.md#icd10cmattributetypetype) 
2. See [:material-code-braces: ICD10CMTraitTypeDef](./type_defs.md#icd10cmtraittypedef) 
3. See [:material-code-brackets: ICD10CMEntityTypeType](./literals.md#icd10cmentitytypetype) 
4. See [:material-code-brackets: ICD10CMRelationshipTypeType](./literals.md#icd10cmrelationshiptypetype) 
## RxNormAttributeTypeDef

```python
# RxNormAttributeTypeDef definition

class RxNormAttributeTypeDef(TypedDict):
    Type: NotRequired[RxNormAttributeTypeType],  # (1)
    Score: NotRequired[float],
    RelationshipScore: NotRequired[float],
    Id: NotRequired[int],
    BeginOffset: NotRequired[int],
    EndOffset: NotRequired[int],
    Text: NotRequired[str],
    Traits: NotRequired[List[RxNormTraitTypeDef]],  # (2)
```

1. See [:material-code-brackets: RxNormAttributeTypeType](./literals.md#rxnormattributetypetype) 
2. See [:material-code-braces: RxNormTraitTypeDef](./type_defs.md#rxnormtraittypedef) 
## SNOMEDCTAttributeTypeDef

```python
# SNOMEDCTAttributeTypeDef definition

class SNOMEDCTAttributeTypeDef(TypedDict):
    Category: NotRequired[SNOMEDCTEntityCategoryType],  # (1)
    Type: NotRequired[SNOMEDCTAttributeTypeType],  # (2)
    Score: NotRequired[float],
    RelationshipScore: NotRequired[float],
    RelationshipType: NotRequired[SNOMEDCTRelationshipTypeType],  # (3)
    Id: NotRequired[int],
    BeginOffset: NotRequired[int],
    EndOffset: NotRequired[int],
    Text: NotRequired[str],
    Traits: NotRequired[List[SNOMEDCTTraitTypeDef]],  # (4)
    SNOMEDCTConcepts: NotRequired[List[SNOMEDCTConceptTypeDef]],  # (5)
```

1. See [:material-code-brackets: SNOMEDCTEntityCategoryType](./literals.md#snomedctentitycategorytype) 
2. See [:material-code-brackets: SNOMEDCTAttributeTypeType](./literals.md#snomedctattributetypetype) 
3. See [:material-code-brackets: SNOMEDCTRelationshipTypeType](./literals.md#snomedctrelationshiptypetype) 
4. See [:material-code-braces: SNOMEDCTTraitTypeDef](./type_defs.md#snomedcttraittypedef) 
5. See [:material-code-braces: SNOMEDCTConceptTypeDef](./type_defs.md#snomedctconcepttypedef) 
## EntityTypeDef

```python
# EntityTypeDef definition

class EntityTypeDef(TypedDict):
    Id: NotRequired[int],
    BeginOffset: NotRequired[int],
    EndOffset: NotRequired[int],
    Score: NotRequired[float],
    Text: NotRequired[str],
    Category: NotRequired[EntityTypeType],  # (1)
    Type: NotRequired[EntitySubTypeType],  # (2)
    Traits: NotRequired[List[TraitTypeDef]],  # (3)
    Attributes: NotRequired[List[AttributeTypeDef]],  # (4)
```

1. See [:material-code-brackets: EntityTypeType](./literals.md#entitytypetype) 
2. See [:material-code-brackets: EntitySubTypeType](./literals.md#entitysubtypetype) 
3. See [:material-code-braces: TraitTypeDef](./type_defs.md#traittypedef) 
4. See [:material-code-braces: AttributeTypeDef](./type_defs.md#attributetypedef) 
## UnmappedAttributeTypeDef

```python
# UnmappedAttributeTypeDef definition

class UnmappedAttributeTypeDef(TypedDict):
    Type: NotRequired[EntityTypeType],  # (1)
    Attribute: NotRequired[AttributeTypeDef],  # (2)
```

1. See [:material-code-brackets: EntityTypeType](./literals.md#entitytypetype) 
2. See [:material-code-braces: AttributeTypeDef](./type_defs.md#attributetypedef) 
## ListEntitiesDetectionV2JobsRequestRequestTypeDef

```python
# ListEntitiesDetectionV2JobsRequestRequestTypeDef definition

class ListEntitiesDetectionV2JobsRequestRequestTypeDef(TypedDict):
    Filter: NotRequired[ComprehendMedicalAsyncJobFilterTypeDef],  # (1)
    NextToken: NotRequired[str],
    MaxResults: NotRequired[int],
```

1. See [:material-code-braces: ComprehendMedicalAsyncJobFilterTypeDef](./type_defs.md#comprehendmedicalasyncjobfiltertypedef) 
## ListICD10CMInferenceJobsRequestRequestTypeDef

```python
# ListICD10CMInferenceJobsRequestRequestTypeDef definition

class ListICD10CMInferenceJobsRequestRequestTypeDef(TypedDict):
    Filter: NotRequired[ComprehendMedicalAsyncJobFilterTypeDef],  # (1)
    NextToken: NotRequired[str],
    MaxResults: NotRequired[int],
```

1. See [:material-code-braces: ComprehendMedicalAsyncJobFilterTypeDef](./type_defs.md#comprehendmedicalasyncjobfiltertypedef) 
## ListPHIDetectionJobsRequestRequestTypeDef

```python
# ListPHIDetectionJobsRequestRequestTypeDef definition

class ListPHIDetectionJobsRequestRequestTypeDef(TypedDict):
    Filter: NotRequired[ComprehendMedicalAsyncJobFilterTypeDef],  # (1)
    NextToken: NotRequired[str],
    MaxResults: NotRequired[int],
```

1. See [:material-code-braces: ComprehendMedicalAsyncJobFilterTypeDef](./type_defs.md#comprehendmedicalasyncjobfiltertypedef) 
## ListRxNormInferenceJobsRequestRequestTypeDef

```python
# ListRxNormInferenceJobsRequestRequestTypeDef definition

class ListRxNormInferenceJobsRequestRequestTypeDef(TypedDict):
    Filter: NotRequired[ComprehendMedicalAsyncJobFilterTypeDef],  # (1)
    NextToken: NotRequired[str],
    MaxResults: NotRequired[int],
```

1. See [:material-code-braces: ComprehendMedicalAsyncJobFilterTypeDef](./type_defs.md#comprehendmedicalasyncjobfiltertypedef) 
## ListSNOMEDCTInferenceJobsRequestRequestTypeDef

```python
# ListSNOMEDCTInferenceJobsRequestRequestTypeDef definition

class ListSNOMEDCTInferenceJobsRequestRequestTypeDef(TypedDict):
    Filter: NotRequired[ComprehendMedicalAsyncJobFilterTypeDef],  # (1)
    NextToken: NotRequired[str],
    MaxResults: NotRequired[int],
```

1. See [:material-code-braces: ComprehendMedicalAsyncJobFilterTypeDef](./type_defs.md#comprehendmedicalasyncjobfiltertypedef) 
## DescribeEntitiesDetectionV2JobResponseTypeDef

```python
# DescribeEntitiesDetectionV2JobResponseTypeDef definition

class DescribeEntitiesDetectionV2JobResponseTypeDef(TypedDict):
    ComprehendMedicalAsyncJobProperties: ComprehendMedicalAsyncJobPropertiesTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ComprehendMedicalAsyncJobPropertiesTypeDef](./type_defs.md#comprehendmedicalasyncjobpropertiestypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DescribeICD10CMInferenceJobResponseTypeDef

```python
# DescribeICD10CMInferenceJobResponseTypeDef definition

class DescribeICD10CMInferenceJobResponseTypeDef(TypedDict):
    ComprehendMedicalAsyncJobProperties: ComprehendMedicalAsyncJobPropertiesTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ComprehendMedicalAsyncJobPropertiesTypeDef](./type_defs.md#comprehendmedicalasyncjobpropertiestypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DescribePHIDetectionJobResponseTypeDef

```python
# DescribePHIDetectionJobResponseTypeDef definition

class DescribePHIDetectionJobResponseTypeDef(TypedDict):
    ComprehendMedicalAsyncJobProperties: ComprehendMedicalAsyncJobPropertiesTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ComprehendMedicalAsyncJobPropertiesTypeDef](./type_defs.md#comprehendmedicalasyncjobpropertiestypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DescribeRxNormInferenceJobResponseTypeDef

```python
# DescribeRxNormInferenceJobResponseTypeDef definition

class DescribeRxNormInferenceJobResponseTypeDef(TypedDict):
    ComprehendMedicalAsyncJobProperties: ComprehendMedicalAsyncJobPropertiesTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ComprehendMedicalAsyncJobPropertiesTypeDef](./type_defs.md#comprehendmedicalasyncjobpropertiestypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DescribeSNOMEDCTInferenceJobResponseTypeDef

```python
# DescribeSNOMEDCTInferenceJobResponseTypeDef definition

class DescribeSNOMEDCTInferenceJobResponseTypeDef(TypedDict):
    ComprehendMedicalAsyncJobProperties: ComprehendMedicalAsyncJobPropertiesTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ComprehendMedicalAsyncJobPropertiesTypeDef](./type_defs.md#comprehendmedicalasyncjobpropertiestypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListEntitiesDetectionV2JobsResponseTypeDef

```python
# ListEntitiesDetectionV2JobsResponseTypeDef definition

class ListEntitiesDetectionV2JobsResponseTypeDef(TypedDict):
    ComprehendMedicalAsyncJobPropertiesList: List[ComprehendMedicalAsyncJobPropertiesTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: ComprehendMedicalAsyncJobPropertiesTypeDef](./type_defs.md#comprehendmedicalasyncjobpropertiestypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListICD10CMInferenceJobsResponseTypeDef

```python
# ListICD10CMInferenceJobsResponseTypeDef definition

class ListICD10CMInferenceJobsResponseTypeDef(TypedDict):
    ComprehendMedicalAsyncJobPropertiesList: List[ComprehendMedicalAsyncJobPropertiesTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: ComprehendMedicalAsyncJobPropertiesTypeDef](./type_defs.md#comprehendmedicalasyncjobpropertiestypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListPHIDetectionJobsResponseTypeDef

```python
# ListPHIDetectionJobsResponseTypeDef definition

class ListPHIDetectionJobsResponseTypeDef(TypedDict):
    ComprehendMedicalAsyncJobPropertiesList: List[ComprehendMedicalAsyncJobPropertiesTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: ComprehendMedicalAsyncJobPropertiesTypeDef](./type_defs.md#comprehendmedicalasyncjobpropertiestypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListRxNormInferenceJobsResponseTypeDef

```python
# ListRxNormInferenceJobsResponseTypeDef definition

class ListRxNormInferenceJobsResponseTypeDef(TypedDict):
    ComprehendMedicalAsyncJobPropertiesList: List[ComprehendMedicalAsyncJobPropertiesTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: ComprehendMedicalAsyncJobPropertiesTypeDef](./type_defs.md#comprehendmedicalasyncjobpropertiestypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListSNOMEDCTInferenceJobsResponseTypeDef

```python
# ListSNOMEDCTInferenceJobsResponseTypeDef definition

class ListSNOMEDCTInferenceJobsResponseTypeDef(TypedDict):
    ComprehendMedicalAsyncJobPropertiesList: List[ComprehendMedicalAsyncJobPropertiesTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: ComprehendMedicalAsyncJobPropertiesTypeDef](./type_defs.md#comprehendmedicalasyncjobpropertiestypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ICD10CMEntityTypeDef

```python
# ICD10CMEntityTypeDef definition

class ICD10CMEntityTypeDef(TypedDict):
    Id: NotRequired[int],
    Text: NotRequired[str],
    Category: NotRequired[ICD10CMEntityCategoryType],  # (1)
    Type: NotRequired[ICD10CMEntityTypeType],  # (2)
    Score: NotRequired[float],
    BeginOffset: NotRequired[int],
    EndOffset: NotRequired[int],
    Attributes: NotRequired[List[ICD10CMAttributeTypeDef]],  # (3)
    Traits: NotRequired[List[ICD10CMTraitTypeDef]],  # (4)
    ICD10CMConcepts: NotRequired[List[ICD10CMConceptTypeDef]],  # (5)
```

1. See [:material-code-brackets: ICD10CMEntityCategoryType](./literals.md#icd10cmentitycategorytype) 
2. See [:material-code-brackets: ICD10CMEntityTypeType](./literals.md#icd10cmentitytypetype) 
3. See [:material-code-braces: ICD10CMAttributeTypeDef](./type_defs.md#icd10cmattributetypedef) 
4. See [:material-code-braces: ICD10CMTraitTypeDef](./type_defs.md#icd10cmtraittypedef) 
5. See [:material-code-braces: ICD10CMConceptTypeDef](./type_defs.md#icd10cmconcepttypedef) 
## RxNormEntityTypeDef

```python
# RxNormEntityTypeDef definition

class RxNormEntityTypeDef(TypedDict):
    Id: NotRequired[int],
    Text: NotRequired[str],
    Category: NotRequired[RxNormEntityCategoryType],  # (1)
    Type: NotRequired[RxNormEntityTypeType],  # (2)
    Score: NotRequired[float],
    BeginOffset: NotRequired[int],
    EndOffset: NotRequired[int],
    Attributes: NotRequired[List[RxNormAttributeTypeDef]],  # (3)
    Traits: NotRequired[List[RxNormTraitTypeDef]],  # (4)
    RxNormConcepts: NotRequired[List[RxNormConceptTypeDef]],  # (5)
```

1. See [:material-code-brackets: RxNormEntityCategoryType](./literals.md#rxnormentitycategorytype) 
2. See [:material-code-brackets: RxNormEntityTypeType](./literals.md#rxnormentitytypetype) 
3. See [:material-code-braces: RxNormAttributeTypeDef](./type_defs.md#rxnormattributetypedef) 
4. See [:material-code-braces: RxNormTraitTypeDef](./type_defs.md#rxnormtraittypedef) 
5. See [:material-code-braces: RxNormConceptTypeDef](./type_defs.md#rxnormconcepttypedef) 
## SNOMEDCTEntityTypeDef

```python
# SNOMEDCTEntityTypeDef definition

class SNOMEDCTEntityTypeDef(TypedDict):
    Id: NotRequired[int],
    Text: NotRequired[str],
    Category: NotRequired[SNOMEDCTEntityCategoryType],  # (1)
    Type: NotRequired[SNOMEDCTEntityTypeType],  # (2)
    Score: NotRequired[float],
    BeginOffset: NotRequired[int],
    EndOffset: NotRequired[int],
    Attributes: NotRequired[List[SNOMEDCTAttributeTypeDef]],  # (3)
    Traits: NotRequired[List[SNOMEDCTTraitTypeDef]],  # (4)
    SNOMEDCTConcepts: NotRequired[List[SNOMEDCTConceptTypeDef]],  # (5)
```

1. See [:material-code-brackets: SNOMEDCTEntityCategoryType](./literals.md#snomedctentitycategorytype) 
2. See [:material-code-brackets: SNOMEDCTEntityTypeType](./literals.md#snomedctentitytypetype) 
3. See [:material-code-braces: SNOMEDCTAttributeTypeDef](./type_defs.md#snomedctattributetypedef) 
4. See [:material-code-braces: SNOMEDCTTraitTypeDef](./type_defs.md#snomedcttraittypedef) 
5. See [:material-code-braces: SNOMEDCTConceptTypeDef](./type_defs.md#snomedctconcepttypedef) 
## DetectPHIResponseTypeDef

```python
# DetectPHIResponseTypeDef definition

class DetectPHIResponseTypeDef(TypedDict):
    Entities: List[EntityTypeDef],  # (1)
    PaginationToken: str,
    ModelVersion: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: EntityTypeDef](./type_defs.md#entitytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DetectEntitiesResponseTypeDef

```python
# DetectEntitiesResponseTypeDef definition

class DetectEntitiesResponseTypeDef(TypedDict):
    Entities: List[EntityTypeDef],  # (1)
    UnmappedAttributes: List[UnmappedAttributeTypeDef],  # (2)
    PaginationToken: str,
    ModelVersion: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (3)
```

1. See [:material-code-braces: EntityTypeDef](./type_defs.md#entitytypedef) 
2. See [:material-code-braces: UnmappedAttributeTypeDef](./type_defs.md#unmappedattributetypedef) 
3. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DetectEntitiesV2ResponseTypeDef

```python
# DetectEntitiesV2ResponseTypeDef definition

class DetectEntitiesV2ResponseTypeDef(TypedDict):
    Entities: List[EntityTypeDef],  # (1)
    UnmappedAttributes: List[UnmappedAttributeTypeDef],  # (2)
    PaginationToken: str,
    ModelVersion: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (3)
```

1. See [:material-code-braces: EntityTypeDef](./type_defs.md#entitytypedef) 
2. See [:material-code-braces: UnmappedAttributeTypeDef](./type_defs.md#unmappedattributetypedef) 
3. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## InferICD10CMResponseTypeDef

```python
# InferICD10CMResponseTypeDef definition

class InferICD10CMResponseTypeDef(TypedDict):
    Entities: List[ICD10CMEntityTypeDef],  # (1)
    PaginationToken: str,
    ModelVersion: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ICD10CMEntityTypeDef](./type_defs.md#icd10cmentitytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## InferRxNormResponseTypeDef

```python
# InferRxNormResponseTypeDef definition

class InferRxNormResponseTypeDef(TypedDict):
    Entities: List[RxNormEntityTypeDef],  # (1)
    PaginationToken: str,
    ModelVersion: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: RxNormEntityTypeDef](./type_defs.md#rxnormentitytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## InferSNOMEDCTResponseTypeDef

```python
# InferSNOMEDCTResponseTypeDef definition

class InferSNOMEDCTResponseTypeDef(TypedDict):
    Entities: List[SNOMEDCTEntityTypeDef],  # (1)
    PaginationToken: str,
    ModelVersion: str,
    SNOMEDCTDetails: SNOMEDCTDetailsTypeDef,  # (2)
    Characters: CharactersTypeDef,  # (3)
    ResponseMetadata: ResponseMetadataTypeDef,  # (4)
```

1. See [:material-code-braces: SNOMEDCTEntityTypeDef](./type_defs.md#snomedctentitytypedef) 
2. See [:material-code-braces: SNOMEDCTDetailsTypeDef](./type_defs.md#snomedctdetailstypedef) 
3. See [:material-code-braces: CharactersTypeDef](./type_defs.md#characterstypedef) 
4. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
