# Type definitions

> [Index](../README.md) > [B2BI](./README.md) > Type definitions

!!! note ""

    Auto-generated documentation for [B2BI](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/b2bi.html#b2bi)
    type annotations stubs module [types-aiobotocore-b2bi](https://pypi.org/project/types-aiobotocore-b2bi/).



## CapabilitySummaryTypeDef

```python
# CapabilitySummaryTypeDef definition

class CapabilitySummaryTypeDef(TypedDict):
    capabilityId: str,
    name: str,
    type: CapabilityTypeType,  # (1)
    createdAt: datetime,
    modifiedAt: NotRequired[datetime],
```

1. See [:material-code-brackets: CapabilityTypeType](./literals.md#capabilitytypetype) 
## InputFileSourceTypeDef

```python
# InputFileSourceTypeDef definition

class InputFileSourceTypeDef(TypedDict):
    fileContent: NotRequired[str],
```

## X12DetailsTypeDef

```python
# X12DetailsTypeDef definition

class X12DetailsTypeDef(TypedDict):
    transactionSet: NotRequired[X12TransactionSetType],  # (1)
    version: NotRequired[X12VersionType],  # (2)
```

1. See [:material-code-brackets: X12TransactionSetType](./literals.md#x12transactionsettype) 
2. See [:material-code-brackets: X12VersionType](./literals.md#x12versiontype) 
## S3LocationTypeDef

```python
# S3LocationTypeDef definition

class S3LocationTypeDef(TypedDict):
    bucketName: NotRequired[str],
    key: NotRequired[str],
```

## TagTypeDef

```python
# TagTypeDef definition

class TagTypeDef(TypedDict):
    Key: str,
    Value: str,
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

## MappingTypeDef

```python
# MappingTypeDef definition

class MappingTypeDef(TypedDict):
    templateLanguage: MappingTemplateLanguageType,  # (1)
    template: NotRequired[str],
```

1. See [:material-code-brackets: MappingTemplateLanguageType](./literals.md#mappingtemplatelanguagetype) 
## DeleteCapabilityRequestRequestTypeDef

```python
# DeleteCapabilityRequestRequestTypeDef definition

class DeleteCapabilityRequestRequestTypeDef(TypedDict):
    capabilityId: str,
```

## DeletePartnershipRequestRequestTypeDef

```python
# DeletePartnershipRequestRequestTypeDef definition

class DeletePartnershipRequestRequestTypeDef(TypedDict):
    partnershipId: str,
```

## DeleteProfileRequestRequestTypeDef

```python
# DeleteProfileRequestRequestTypeDef definition

class DeleteProfileRequestRequestTypeDef(TypedDict):
    profileId: str,
```

## DeleteTransformerRequestRequestTypeDef

```python
# DeleteTransformerRequestRequestTypeDef definition

class DeleteTransformerRequestRequestTypeDef(TypedDict):
    transformerId: str,
```

## GenerateMappingRequestRequestTypeDef

```python
# GenerateMappingRequestRequestTypeDef definition

class GenerateMappingRequestRequestTypeDef(TypedDict):
    inputFileContent: str,
    outputFileContent: str,
    mappingType: MappingTypeType,  # (1)
```

1. See [:material-code-brackets: MappingTypeType](./literals.md#mappingtypetype) 
## GetCapabilityRequestRequestTypeDef

```python
# GetCapabilityRequestRequestTypeDef definition

class GetCapabilityRequestRequestTypeDef(TypedDict):
    capabilityId: str,
```

## GetPartnershipRequestRequestTypeDef

```python
# GetPartnershipRequestRequestTypeDef definition

class GetPartnershipRequestRequestTypeDef(TypedDict):
    partnershipId: str,
```

## GetProfileRequestRequestTypeDef

```python
# GetProfileRequestRequestTypeDef definition

class GetProfileRequestRequestTypeDef(TypedDict):
    profileId: str,
```

## GetTransformerJobRequestRequestTypeDef

```python
# GetTransformerJobRequestRequestTypeDef definition

class GetTransformerJobRequestRequestTypeDef(TypedDict):
    transformerJobId: str,
    transformerId: str,
```

## GetTransformerRequestRequestTypeDef

```python
# GetTransformerRequestRequestTypeDef definition

class GetTransformerRequestRequestTypeDef(TypedDict):
    transformerId: str,
```

## PaginatorConfigTypeDef

```python
# PaginatorConfigTypeDef definition

class PaginatorConfigTypeDef(TypedDict):
    MaxItems: NotRequired[int],
    PageSize: NotRequired[int],
    StartingToken: NotRequired[str],
```

## ListCapabilitiesRequestRequestTypeDef

```python
# ListCapabilitiesRequestRequestTypeDef definition

class ListCapabilitiesRequestRequestTypeDef(TypedDict):
    nextToken: NotRequired[str],
    maxResults: NotRequired[int],
```

## ListPartnershipsRequestRequestTypeDef

```python
# ListPartnershipsRequestRequestTypeDef definition

class ListPartnershipsRequestRequestTypeDef(TypedDict):
    profileId: NotRequired[str],
    nextToken: NotRequired[str],
    maxResults: NotRequired[int],
```

## ListProfilesRequestRequestTypeDef

```python
# ListProfilesRequestRequestTypeDef definition

class ListProfilesRequestRequestTypeDef(TypedDict):
    nextToken: NotRequired[str],
    maxResults: NotRequired[int],
```

## ProfileSummaryTypeDef

```python
# ProfileSummaryTypeDef definition

class ProfileSummaryTypeDef(TypedDict):
    profileId: str,
    name: str,
    businessName: str,
    createdAt: datetime,
    logging: NotRequired[LoggingType],  # (1)
    logGroupName: NotRequired[str],
    modifiedAt: NotRequired[datetime],
```

1. See [:material-code-brackets: LoggingType](./literals.md#loggingtype) 
## ListTagsForResourceRequestRequestTypeDef

```python
# ListTagsForResourceRequestRequestTypeDef definition

class ListTagsForResourceRequestRequestTypeDef(TypedDict):
    ResourceARN: str,
```

## ListTransformersRequestRequestTypeDef

```python
# ListTransformersRequestRequestTypeDef definition

class ListTransformersRequestRequestTypeDef(TypedDict):
    nextToken: NotRequired[str],
    maxResults: NotRequired[int],
```

## SampleDocumentKeysTypeDef

```python
# SampleDocumentKeysTypeDef definition

class SampleDocumentKeysTypeDef(TypedDict):
    input: NotRequired[str],
    output: NotRequired[str],
```

## TestMappingRequestRequestTypeDef

```python
# TestMappingRequestRequestTypeDef definition

class TestMappingRequestRequestTypeDef(TypedDict):
    inputFileContent: str,
    mappingTemplate: str,
    fileFormat: FileFormatType,  # (1)
```

1. See [:material-code-brackets: FileFormatType](./literals.md#fileformattype) 
## UntagResourceRequestRequestTypeDef

```python
# UntagResourceRequestRequestTypeDef definition

class UntagResourceRequestRequestTypeDef(TypedDict):
    ResourceARN: str,
    TagKeys: Sequence[str],
```

## UpdateProfileRequestRequestTypeDef

```python
# UpdateProfileRequestRequestTypeDef definition

class UpdateProfileRequestRequestTypeDef(TypedDict):
    profileId: str,
    name: NotRequired[str],
    email: NotRequired[str],
    phone: NotRequired[str],
    businessName: NotRequired[str],
```

## X12DelimitersTypeDef

```python
# X12DelimitersTypeDef definition

class X12DelimitersTypeDef(TypedDict):
    componentSeparator: NotRequired[str],
    dataElementSeparator: NotRequired[str],
    segmentTerminator: NotRequired[str],
```

## X12FunctionalGroupHeadersTypeDef

```python
# X12FunctionalGroupHeadersTypeDef definition

class X12FunctionalGroupHeadersTypeDef(TypedDict):
    applicationSenderCode: NotRequired[str],
    applicationReceiverCode: NotRequired[str],
    responsibleAgencyCode: NotRequired[str],
```

## X12InterchangeControlHeadersTypeDef

```python
# X12InterchangeControlHeadersTypeDef definition

class X12InterchangeControlHeadersTypeDef(TypedDict):
    senderIdQualifier: NotRequired[str],
    senderId: NotRequired[str],
    receiverIdQualifier: NotRequired[str],
    receiverId: NotRequired[str],
    repetitionSeparator: NotRequired[str],
    acknowledgmentRequestedCode: NotRequired[str],
    usageIndicatorCode: NotRequired[str],
```

## ConversionSourceTypeDef

```python
# ConversionSourceTypeDef definition

class ConversionSourceTypeDef(TypedDict):
    fileFormat: ConversionSourceFormatType,  # (1)
    inputFile: InputFileSourceTypeDef,  # (2)
```

1. See [:material-code-brackets: ConversionSourceFormatType](./literals.md#conversionsourceformattype) 
2. See [:material-code-braces: InputFileSourceTypeDef](./type_defs.md#inputfilesourcetypedef) 
## ConversionTargetFormatDetailsTypeDef

```python
# ConversionTargetFormatDetailsTypeDef definition

class ConversionTargetFormatDetailsTypeDef(TypedDict):
    x12: NotRequired[X12DetailsTypeDef],  # (1)
```

1. See [:material-code-braces: X12DetailsTypeDef](./type_defs.md#x12detailstypedef) 
## EdiTypeTypeDef

```python
# EdiTypeTypeDef definition

class EdiTypeTypeDef(TypedDict):
    x12Details: NotRequired[X12DetailsTypeDef],  # (1)
```

1. See [:material-code-braces: X12DetailsTypeDef](./type_defs.md#x12detailstypedef) 
## FormatOptionsTypeDef

```python
# FormatOptionsTypeDef definition

class FormatOptionsTypeDef(TypedDict):
    x12: NotRequired[X12DetailsTypeDef],  # (1)
```

1. See [:material-code-braces: X12DetailsTypeDef](./type_defs.md#x12detailstypedef) 
## TemplateDetailsTypeDef

```python
# TemplateDetailsTypeDef definition

class TemplateDetailsTypeDef(TypedDict):
    x12: NotRequired[X12DetailsTypeDef],  # (1)
```

1. See [:material-code-braces: X12DetailsTypeDef](./type_defs.md#x12detailstypedef) 
## OutputSampleFileSourceTypeDef

```python
# OutputSampleFileSourceTypeDef definition

class OutputSampleFileSourceTypeDef(TypedDict):
    fileLocation: NotRequired[S3LocationTypeDef],  # (1)
```

1. See [:material-code-braces: S3LocationTypeDef](./type_defs.md#s3locationtypedef) 
## StartTransformerJobRequestRequestTypeDef

```python
# StartTransformerJobRequestRequestTypeDef definition

class StartTransformerJobRequestRequestTypeDef(TypedDict):
    inputFile: S3LocationTypeDef,  # (1)
    outputLocation: S3LocationTypeDef,  # (1)
    transformerId: str,
    clientToken: NotRequired[str],
```

1. See [:material-code-braces: S3LocationTypeDef](./type_defs.md#s3locationtypedef) 
2. See [:material-code-braces: S3LocationTypeDef](./type_defs.md#s3locationtypedef) 
## CreateProfileRequestRequestTypeDef

```python
# CreateProfileRequestRequestTypeDef definition

class CreateProfileRequestRequestTypeDef(TypedDict):
    name: str,
    phone: str,
    businessName: str,
    logging: LoggingType,  # (1)
    email: NotRequired[str],
    clientToken: NotRequired[str],
    tags: NotRequired[Sequence[TagTypeDef]],  # (2)
```

1. See [:material-code-brackets: LoggingType](./literals.md#loggingtype) 
2. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
## TagResourceRequestRequestTypeDef

```python
# TagResourceRequestRequestTypeDef definition

class TagResourceRequestRequestTypeDef(TypedDict):
    ResourceARN: str,
    Tags: Sequence[TagTypeDef],  # (1)
```

1. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
## CreateProfileResponseTypeDef

```python
# CreateProfileResponseTypeDef definition

class CreateProfileResponseTypeDef(TypedDict):
    profileId: str,
    profileArn: str,
    name: str,
    businessName: str,
    phone: str,
    email: str,
    logging: LoggingType,  # (1)
    logGroupName: str,
    createdAt: datetime,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-brackets: LoggingType](./literals.md#loggingtype) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateStarterMappingTemplateResponseTypeDef

```python
# CreateStarterMappingTemplateResponseTypeDef definition

class CreateStarterMappingTemplateResponseTypeDef(TypedDict):
    mappingTemplate: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## EmptyResponseMetadataTypeDef

```python
# EmptyResponseMetadataTypeDef definition

class EmptyResponseMetadataTypeDef(TypedDict):
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GenerateMappingResponseTypeDef

```python
# GenerateMappingResponseTypeDef definition

class GenerateMappingResponseTypeDef(TypedDict):
    mappingTemplate: str,
    mappingAccuracy: float,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetProfileResponseTypeDef

```python
# GetProfileResponseTypeDef definition

class GetProfileResponseTypeDef(TypedDict):
    profileId: str,
    profileArn: str,
    name: str,
    email: str,
    phone: str,
    businessName: str,
    logging: LoggingType,  # (1)
    logGroupName: str,
    createdAt: datetime,
    modifiedAt: datetime,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-brackets: LoggingType](./literals.md#loggingtype) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetTransformerJobResponseTypeDef

```python
# GetTransformerJobResponseTypeDef definition

class GetTransformerJobResponseTypeDef(TypedDict):
    status: TransformerJobStatusType,  # (1)
    outputFiles: List[S3LocationTypeDef],  # (2)
    message: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (3)
```

1. See [:material-code-brackets: TransformerJobStatusType](./literals.md#transformerjobstatustype) 
2. See [:material-code-braces: S3LocationTypeDef](./type_defs.md#s3locationtypedef) 
3. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListCapabilitiesResponseTypeDef

```python
# ListCapabilitiesResponseTypeDef definition

class ListCapabilitiesResponseTypeDef(TypedDict):
    capabilities: List[CapabilitySummaryTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    nextToken: NotRequired[str],
```

1. See [:material-code-braces: CapabilitySummaryTypeDef](./type_defs.md#capabilitysummarytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListTagsForResourceResponseTypeDef

```python
# ListTagsForResourceResponseTypeDef definition

class ListTagsForResourceResponseTypeDef(TypedDict):
    Tags: List[TagTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## StartTransformerJobResponseTypeDef

```python
# StartTransformerJobResponseTypeDef definition

class StartTransformerJobResponseTypeDef(TypedDict):
    transformerJobId: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## TestConversionResponseTypeDef

```python
# TestConversionResponseTypeDef definition

class TestConversionResponseTypeDef(TypedDict):
    convertedFileContent: str,
    validationMessages: List[str],
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## TestMappingResponseTypeDef

```python
# TestMappingResponseTypeDef definition

class TestMappingResponseTypeDef(TypedDict):
    mappedFileContent: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## TestParsingResponseTypeDef

```python
# TestParsingResponseTypeDef definition

class TestParsingResponseTypeDef(TypedDict):
    parsedFileContent: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdateProfileResponseTypeDef

```python
# UpdateProfileResponseTypeDef definition

class UpdateProfileResponseTypeDef(TypedDict):
    profileId: str,
    profileArn: str,
    name: str,
    email: str,
    phone: str,
    businessName: str,
    logging: LoggingType,  # (1)
    logGroupName: str,
    createdAt: datetime,
    modifiedAt: datetime,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-brackets: LoggingType](./literals.md#loggingtype) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListCapabilitiesRequestPaginateTypeDef

```python
# ListCapabilitiesRequestPaginateTypeDef definition

class ListCapabilitiesRequestPaginateTypeDef(TypedDict):
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListPartnershipsRequestPaginateTypeDef

```python
# ListPartnershipsRequestPaginateTypeDef definition

class ListPartnershipsRequestPaginateTypeDef(TypedDict):
    profileId: NotRequired[str],
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListProfilesRequestPaginateTypeDef

```python
# ListProfilesRequestPaginateTypeDef definition

class ListProfilesRequestPaginateTypeDef(TypedDict):
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListTransformersRequestPaginateTypeDef

```python
# ListTransformersRequestPaginateTypeDef definition

class ListTransformersRequestPaginateTypeDef(TypedDict):
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListProfilesResponseTypeDef

```python
# ListProfilesResponseTypeDef definition

class ListProfilesResponseTypeDef(TypedDict):
    profiles: List[ProfileSummaryTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    nextToken: NotRequired[str],
```

1. See [:material-code-braces: ProfileSummaryTypeDef](./type_defs.md#profilesummarytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## SampleDocumentsOutputTypeDef

```python
# SampleDocumentsOutputTypeDef definition

class SampleDocumentsOutputTypeDef(TypedDict):
    bucketName: str,
    keys: List[SampleDocumentKeysTypeDef],  # (1)
```

1. See [:material-code-braces: SampleDocumentKeysTypeDef](./type_defs.md#sampledocumentkeystypedef) 
## SampleDocumentsTypeDef

```python
# SampleDocumentsTypeDef definition

class SampleDocumentsTypeDef(TypedDict):
    bucketName: str,
    keys: Sequence[SampleDocumentKeysTypeDef],  # (1)
```

1. See [:material-code-braces: SampleDocumentKeysTypeDef](./type_defs.md#sampledocumentkeystypedef) 
## X12OutboundEdiHeadersTypeDef

```python
# X12OutboundEdiHeadersTypeDef definition

class X12OutboundEdiHeadersTypeDef(TypedDict):
    interchangeControlHeaders: NotRequired[X12InterchangeControlHeadersTypeDef],  # (1)
    functionalGroupHeaders: NotRequired[X12FunctionalGroupHeadersTypeDef],  # (2)
    delimiters: NotRequired[X12DelimitersTypeDef],  # (3)
    validateEdi: NotRequired[bool],
```

1. See [:material-code-braces: X12InterchangeControlHeadersTypeDef](./type_defs.md#x12interchangecontrolheaderstypedef) 
2. See [:material-code-braces: X12FunctionalGroupHeadersTypeDef](./type_defs.md#x12functionalgroupheaderstypedef) 
3. See [:material-code-braces: X12DelimitersTypeDef](./type_defs.md#x12delimiterstypedef) 
## EdiConfigurationTypeDef

```python
# EdiConfigurationTypeDef definition

class EdiConfigurationTypeDef(TypedDict):
    type: EdiTypeTypeDef,  # (2)
    inputLocation: S3LocationTypeDef,  # (3)
    outputLocation: S3LocationTypeDef,  # (3)
    transformerId: str,
    capabilityDirection: NotRequired[CapabilityDirectionType],  # (1)
```

1. See [:material-code-brackets: CapabilityDirectionType](./literals.md#capabilitydirectiontype) 
2. See [:material-code-braces: EdiTypeTypeDef](./type_defs.md#editypetypedef) 
3. See [:material-code-braces: S3LocationTypeDef](./type_defs.md#s3locationtypedef) 
4. See [:material-code-braces: S3LocationTypeDef](./type_defs.md#s3locationtypedef) 
## TestParsingRequestRequestTypeDef

```python
# TestParsingRequestRequestTypeDef definition

class TestParsingRequestRequestTypeDef(TypedDict):
    inputFile: S3LocationTypeDef,  # (1)
    fileFormat: FileFormatType,  # (2)
    ediType: EdiTypeTypeDef,  # (3)
```

1. See [:material-code-braces: S3LocationTypeDef](./type_defs.md#s3locationtypedef) 
2. See [:material-code-brackets: FileFormatType](./literals.md#fileformattype) 
3. See [:material-code-braces: EdiTypeTypeDef](./type_defs.md#editypetypedef) 
## InputConversionTypeDef

```python
# InputConversionTypeDef definition

class InputConversionTypeDef(TypedDict):
    fromFormat: FromFormatType,  # (1)
    formatOptions: NotRequired[FormatOptionsTypeDef],  # (2)
```

1. See [:material-code-brackets: FromFormatType](./literals.md#fromformattype) 
2. See [:material-code-braces: FormatOptionsTypeDef](./type_defs.md#formatoptionstypedef) 
## OutputConversionTypeDef

```python
# OutputConversionTypeDef definition

class OutputConversionTypeDef(TypedDict):
    toFormat: ToFormatType,  # (1)
    formatOptions: NotRequired[FormatOptionsTypeDef],  # (2)
```

1. See [:material-code-brackets: ToFormatType](./literals.md#toformattype) 
2. See [:material-code-braces: FormatOptionsTypeDef](./type_defs.md#formatoptionstypedef) 
## CreateStarterMappingTemplateRequestRequestTypeDef

```python
# CreateStarterMappingTemplateRequestRequestTypeDef definition

class CreateStarterMappingTemplateRequestRequestTypeDef(TypedDict):
    mappingType: MappingTypeType,  # (1)
    templateDetails: TemplateDetailsTypeDef,  # (2)
    outputSampleLocation: NotRequired[S3LocationTypeDef],  # (3)
```

1. See [:material-code-brackets: MappingTypeType](./literals.md#mappingtypetype) 
2. See [:material-code-braces: TemplateDetailsTypeDef](./type_defs.md#templatedetailstypedef) 
3. See [:material-code-braces: S3LocationTypeDef](./type_defs.md#s3locationtypedef) 
## ConversionTargetTypeDef

```python
# ConversionTargetTypeDef definition

class ConversionTargetTypeDef(TypedDict):
    fileFormat: ConversionTargetFormatType,  # (1)
    formatDetails: NotRequired[ConversionTargetFormatDetailsTypeDef],  # (2)
    outputSampleFile: NotRequired[OutputSampleFileSourceTypeDef],  # (3)
```

1. See [:material-code-brackets: ConversionTargetFormatType](./literals.md#conversiontargetformattype) 
2. See [:material-code-braces: ConversionTargetFormatDetailsTypeDef](./type_defs.md#conversiontargetformatdetailstypedef) 
3. See [:material-code-braces: OutputSampleFileSourceTypeDef](./type_defs.md#outputsamplefilesourcetypedef) 
## X12EnvelopeTypeDef

```python
# X12EnvelopeTypeDef definition

class X12EnvelopeTypeDef(TypedDict):
    common: NotRequired[X12OutboundEdiHeadersTypeDef],  # (1)
```

1. See [:material-code-braces: X12OutboundEdiHeadersTypeDef](./type_defs.md#x12outboundediheaderstypedef) 
## CapabilityConfigurationTypeDef

```python
# CapabilityConfigurationTypeDef definition

class CapabilityConfigurationTypeDef(TypedDict):
    edi: NotRequired[EdiConfigurationTypeDef],  # (1)
```

1. See [:material-code-braces: EdiConfigurationTypeDef](./type_defs.md#ediconfigurationtypedef) 
## CreateTransformerRequestRequestTypeDef

```python
# CreateTransformerRequestRequestTypeDef definition

class CreateTransformerRequestRequestTypeDef(TypedDict):
    name: str,
    clientToken: NotRequired[str],
    tags: NotRequired[Sequence[TagTypeDef]],  # (1)
    fileFormat: NotRequired[FileFormatType],  # (2)
    mappingTemplate: NotRequired[str],
    ediType: NotRequired[EdiTypeTypeDef],  # (3)
    sampleDocument: NotRequired[str],
    inputConversion: NotRequired[InputConversionTypeDef],  # (4)
    mapping: NotRequired[MappingTypeDef],  # (5)
    outputConversion: NotRequired[OutputConversionTypeDef],  # (6)
    sampleDocuments: NotRequired[SampleDocumentsTypeDef],  # (7)
```

1. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
2. See [:material-code-brackets: FileFormatType](./literals.md#fileformattype) 
3. See [:material-code-braces: EdiTypeTypeDef](./type_defs.md#editypetypedef) 
4. See [:material-code-braces: InputConversionTypeDef](./type_defs.md#inputconversiontypedef) 
5. See [:material-code-braces: MappingTypeDef](./type_defs.md#mappingtypedef) 
6. See [:material-code-braces: OutputConversionTypeDef](./type_defs.md#outputconversiontypedef) 
7. See [:material-code-braces: SampleDocumentsTypeDef](./type_defs.md#sampledocumentstypedef) 
## CreateTransformerResponseTypeDef

```python
# CreateTransformerResponseTypeDef definition

class CreateTransformerResponseTypeDef(TypedDict):
    transformerId: str,
    transformerArn: str,
    name: str,
    status: TransformerStatusType,  # (1)
    createdAt: datetime,
    fileFormat: FileFormatType,  # (2)
    mappingTemplate: str,
    ediType: EdiTypeTypeDef,  # (3)
    sampleDocument: str,
    inputConversion: InputConversionTypeDef,  # (4)
    mapping: MappingTypeDef,  # (5)
    outputConversion: OutputConversionTypeDef,  # (6)
    sampleDocuments: SampleDocumentsOutputTypeDef,  # (7)
    ResponseMetadata: ResponseMetadataTypeDef,  # (8)
```

1. See [:material-code-brackets: TransformerStatusType](./literals.md#transformerstatustype) 
2. See [:material-code-brackets: FileFormatType](./literals.md#fileformattype) 
3. See [:material-code-braces: EdiTypeTypeDef](./type_defs.md#editypetypedef) 
4. See [:material-code-braces: InputConversionTypeDef](./type_defs.md#inputconversiontypedef) 
5. See [:material-code-braces: MappingTypeDef](./type_defs.md#mappingtypedef) 
6. See [:material-code-braces: OutputConversionTypeDef](./type_defs.md#outputconversiontypedef) 
7. See [:material-code-braces: SampleDocumentsOutputTypeDef](./type_defs.md#sampledocumentsoutputtypedef) 
8. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetTransformerResponseTypeDef

```python
# GetTransformerResponseTypeDef definition

class GetTransformerResponseTypeDef(TypedDict):
    transformerId: str,
    transformerArn: str,
    name: str,
    status: TransformerStatusType,  # (1)
    createdAt: datetime,
    modifiedAt: datetime,
    fileFormat: FileFormatType,  # (2)
    mappingTemplate: str,
    ediType: EdiTypeTypeDef,  # (3)
    sampleDocument: str,
    inputConversion: InputConversionTypeDef,  # (4)
    mapping: MappingTypeDef,  # (5)
    outputConversion: OutputConversionTypeDef,  # (6)
    sampleDocuments: SampleDocumentsOutputTypeDef,  # (7)
    ResponseMetadata: ResponseMetadataTypeDef,  # (8)
```

1. See [:material-code-brackets: TransformerStatusType](./literals.md#transformerstatustype) 
2. See [:material-code-brackets: FileFormatType](./literals.md#fileformattype) 
3. See [:material-code-braces: EdiTypeTypeDef](./type_defs.md#editypetypedef) 
4. See [:material-code-braces: InputConversionTypeDef](./type_defs.md#inputconversiontypedef) 
5. See [:material-code-braces: MappingTypeDef](./type_defs.md#mappingtypedef) 
6. See [:material-code-braces: OutputConversionTypeDef](./type_defs.md#outputconversiontypedef) 
7. See [:material-code-braces: SampleDocumentsOutputTypeDef](./type_defs.md#sampledocumentsoutputtypedef) 
8. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## TransformerSummaryTypeDef

```python
# TransformerSummaryTypeDef definition

class TransformerSummaryTypeDef(TypedDict):
    transformerId: str,
    name: str,
    status: TransformerStatusType,  # (1)
    createdAt: datetime,
    modifiedAt: NotRequired[datetime],
    fileFormat: NotRequired[FileFormatType],  # (2)
    mappingTemplate: NotRequired[str],
    ediType: NotRequired[EdiTypeTypeDef],  # (3)
    sampleDocument: NotRequired[str],
    inputConversion: NotRequired[InputConversionTypeDef],  # (4)
    mapping: NotRequired[MappingTypeDef],  # (5)
    outputConversion: NotRequired[OutputConversionTypeDef],  # (6)
    sampleDocuments: NotRequired[SampleDocumentsOutputTypeDef],  # (7)
```

1. See [:material-code-brackets: TransformerStatusType](./literals.md#transformerstatustype) 
2. See [:material-code-brackets: FileFormatType](./literals.md#fileformattype) 
3. See [:material-code-braces: EdiTypeTypeDef](./type_defs.md#editypetypedef) 
4. See [:material-code-braces: InputConversionTypeDef](./type_defs.md#inputconversiontypedef) 
5. See [:material-code-braces: MappingTypeDef](./type_defs.md#mappingtypedef) 
6. See [:material-code-braces: OutputConversionTypeDef](./type_defs.md#outputconversiontypedef) 
7. See [:material-code-braces: SampleDocumentsOutputTypeDef](./type_defs.md#sampledocumentsoutputtypedef) 
## UpdateTransformerRequestRequestTypeDef

```python
# UpdateTransformerRequestRequestTypeDef definition

class UpdateTransformerRequestRequestTypeDef(TypedDict):
    transformerId: str,
    name: NotRequired[str],
    status: NotRequired[TransformerStatusType],  # (1)
    fileFormat: NotRequired[FileFormatType],  # (2)
    mappingTemplate: NotRequired[str],
    ediType: NotRequired[EdiTypeTypeDef],  # (3)
    sampleDocument: NotRequired[str],
    inputConversion: NotRequired[InputConversionTypeDef],  # (4)
    mapping: NotRequired[MappingTypeDef],  # (5)
    outputConversion: NotRequired[OutputConversionTypeDef],  # (6)
    sampleDocuments: NotRequired[SampleDocumentsTypeDef],  # (7)
```

1. See [:material-code-brackets: TransformerStatusType](./literals.md#transformerstatustype) 
2. See [:material-code-brackets: FileFormatType](./literals.md#fileformattype) 
3. See [:material-code-braces: EdiTypeTypeDef](./type_defs.md#editypetypedef) 
4. See [:material-code-braces: InputConversionTypeDef](./type_defs.md#inputconversiontypedef) 
5. See [:material-code-braces: MappingTypeDef](./type_defs.md#mappingtypedef) 
6. See [:material-code-braces: OutputConversionTypeDef](./type_defs.md#outputconversiontypedef) 
7. See [:material-code-braces: SampleDocumentsTypeDef](./type_defs.md#sampledocumentstypedef) 
## UpdateTransformerResponseTypeDef

```python
# UpdateTransformerResponseTypeDef definition

class UpdateTransformerResponseTypeDef(TypedDict):
    transformerId: str,
    transformerArn: str,
    name: str,
    status: TransformerStatusType,  # (1)
    createdAt: datetime,
    modifiedAt: datetime,
    fileFormat: FileFormatType,  # (2)
    mappingTemplate: str,
    ediType: EdiTypeTypeDef,  # (3)
    sampleDocument: str,
    inputConversion: InputConversionTypeDef,  # (4)
    mapping: MappingTypeDef,  # (5)
    outputConversion: OutputConversionTypeDef,  # (6)
    sampleDocuments: SampleDocumentsOutputTypeDef,  # (7)
    ResponseMetadata: ResponseMetadataTypeDef,  # (8)
```

1. See [:material-code-brackets: TransformerStatusType](./literals.md#transformerstatustype) 
2. See [:material-code-brackets: FileFormatType](./literals.md#fileformattype) 
3. See [:material-code-braces: EdiTypeTypeDef](./type_defs.md#editypetypedef) 
4. See [:material-code-braces: InputConversionTypeDef](./type_defs.md#inputconversiontypedef) 
5. See [:material-code-braces: MappingTypeDef](./type_defs.md#mappingtypedef) 
6. See [:material-code-braces: OutputConversionTypeDef](./type_defs.md#outputconversiontypedef) 
7. See [:material-code-braces: SampleDocumentsOutputTypeDef](./type_defs.md#sampledocumentsoutputtypedef) 
8. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## TestConversionRequestRequestTypeDef

```python
# TestConversionRequestRequestTypeDef definition

class TestConversionRequestRequestTypeDef(TypedDict):
    source: ConversionSourceTypeDef,  # (1)
    target: ConversionTargetTypeDef,  # (2)
```

1. See [:material-code-braces: ConversionSourceTypeDef](./type_defs.md#conversionsourcetypedef) 
2. See [:material-code-braces: ConversionTargetTypeDef](./type_defs.md#conversiontargettypedef) 
## OutboundEdiOptionsTypeDef

```python
# OutboundEdiOptionsTypeDef definition

class OutboundEdiOptionsTypeDef(TypedDict):
    x12: NotRequired[X12EnvelopeTypeDef],  # (1)
```

1. See [:material-code-braces: X12EnvelopeTypeDef](./type_defs.md#x12envelopetypedef) 
## CreateCapabilityRequestRequestTypeDef

```python
# CreateCapabilityRequestRequestTypeDef definition

class CreateCapabilityRequestRequestTypeDef(TypedDict):
    name: str,
    type: CapabilityTypeType,  # (1)
    configuration: CapabilityConfigurationTypeDef,  # (2)
    instructionsDocuments: NotRequired[Sequence[S3LocationTypeDef]],  # (3)
    clientToken: NotRequired[str],
    tags: NotRequired[Sequence[TagTypeDef]],  # (4)
```

1. See [:material-code-brackets: CapabilityTypeType](./literals.md#capabilitytypetype) 
2. See [:material-code-braces: CapabilityConfigurationTypeDef](./type_defs.md#capabilityconfigurationtypedef) 
3. See [:material-code-braces: S3LocationTypeDef](./type_defs.md#s3locationtypedef) 
4. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
## CreateCapabilityResponseTypeDef

```python
# CreateCapabilityResponseTypeDef definition

class CreateCapabilityResponseTypeDef(TypedDict):
    capabilityId: str,
    capabilityArn: str,
    name: str,
    type: CapabilityTypeType,  # (1)
    configuration: CapabilityConfigurationTypeDef,  # (2)
    instructionsDocuments: List[S3LocationTypeDef],  # (3)
    createdAt: datetime,
    ResponseMetadata: ResponseMetadataTypeDef,  # (4)
```

1. See [:material-code-brackets: CapabilityTypeType](./literals.md#capabilitytypetype) 
2. See [:material-code-braces: CapabilityConfigurationTypeDef](./type_defs.md#capabilityconfigurationtypedef) 
3. See [:material-code-braces: S3LocationTypeDef](./type_defs.md#s3locationtypedef) 
4. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetCapabilityResponseTypeDef

```python
# GetCapabilityResponseTypeDef definition

class GetCapabilityResponseTypeDef(TypedDict):
    capabilityId: str,
    capabilityArn: str,
    name: str,
    type: CapabilityTypeType,  # (1)
    configuration: CapabilityConfigurationTypeDef,  # (2)
    instructionsDocuments: List[S3LocationTypeDef],  # (3)
    createdAt: datetime,
    modifiedAt: datetime,
    ResponseMetadata: ResponseMetadataTypeDef,  # (4)
```

1. See [:material-code-brackets: CapabilityTypeType](./literals.md#capabilitytypetype) 
2. See [:material-code-braces: CapabilityConfigurationTypeDef](./type_defs.md#capabilityconfigurationtypedef) 
3. See [:material-code-braces: S3LocationTypeDef](./type_defs.md#s3locationtypedef) 
4. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdateCapabilityRequestRequestTypeDef

```python
# UpdateCapabilityRequestRequestTypeDef definition

class UpdateCapabilityRequestRequestTypeDef(TypedDict):
    capabilityId: str,
    name: NotRequired[str],
    configuration: NotRequired[CapabilityConfigurationTypeDef],  # (1)
    instructionsDocuments: NotRequired[Sequence[S3LocationTypeDef]],  # (2)
```

1. See [:material-code-braces: CapabilityConfigurationTypeDef](./type_defs.md#capabilityconfigurationtypedef) 
2. See [:material-code-braces: S3LocationTypeDef](./type_defs.md#s3locationtypedef) 
## UpdateCapabilityResponseTypeDef

```python
# UpdateCapabilityResponseTypeDef definition

class UpdateCapabilityResponseTypeDef(TypedDict):
    capabilityId: str,
    capabilityArn: str,
    name: str,
    type: CapabilityTypeType,  # (1)
    configuration: CapabilityConfigurationTypeDef,  # (2)
    instructionsDocuments: List[S3LocationTypeDef],  # (3)
    createdAt: datetime,
    modifiedAt: datetime,
    ResponseMetadata: ResponseMetadataTypeDef,  # (4)
```

1. See [:material-code-brackets: CapabilityTypeType](./literals.md#capabilitytypetype) 
2. See [:material-code-braces: CapabilityConfigurationTypeDef](./type_defs.md#capabilityconfigurationtypedef) 
3. See [:material-code-braces: S3LocationTypeDef](./type_defs.md#s3locationtypedef) 
4. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListTransformersResponseTypeDef

```python
# ListTransformersResponseTypeDef definition

class ListTransformersResponseTypeDef(TypedDict):
    transformers: List[TransformerSummaryTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    nextToken: NotRequired[str],
```

1. See [:material-code-braces: TransformerSummaryTypeDef](./type_defs.md#transformersummarytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CapabilityOptionsTypeDef

```python
# CapabilityOptionsTypeDef definition

class CapabilityOptionsTypeDef(TypedDict):
    outboundEdi: NotRequired[OutboundEdiOptionsTypeDef],  # (1)
```

1. See [:material-code-braces: OutboundEdiOptionsTypeDef](./type_defs.md#outboundedioptionstypedef) 
## CreatePartnershipRequestRequestTypeDef

```python
# CreatePartnershipRequestRequestTypeDef definition

class CreatePartnershipRequestRequestTypeDef(TypedDict):
    profileId: str,
    name: str,
    email: str,
    capabilities: Sequence[str],
    phone: NotRequired[str],
    capabilityOptions: NotRequired[CapabilityOptionsTypeDef],  # (1)
    clientToken: NotRequired[str],
    tags: NotRequired[Sequence[TagTypeDef]],  # (2)
```

1. See [:material-code-braces: CapabilityOptionsTypeDef](./type_defs.md#capabilityoptionstypedef) 
2. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
## CreatePartnershipResponseTypeDef

```python
# CreatePartnershipResponseTypeDef definition

class CreatePartnershipResponseTypeDef(TypedDict):
    profileId: str,
    partnershipId: str,
    partnershipArn: str,
    name: str,
    email: str,
    phone: str,
    capabilities: List[str],
    capabilityOptions: CapabilityOptionsTypeDef,  # (1)
    tradingPartnerId: str,
    createdAt: datetime,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: CapabilityOptionsTypeDef](./type_defs.md#capabilityoptionstypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetPartnershipResponseTypeDef

```python
# GetPartnershipResponseTypeDef definition

class GetPartnershipResponseTypeDef(TypedDict):
    profileId: str,
    partnershipId: str,
    partnershipArn: str,
    name: str,
    email: str,
    phone: str,
    capabilities: List[str],
    capabilityOptions: CapabilityOptionsTypeDef,  # (1)
    tradingPartnerId: str,
    createdAt: datetime,
    modifiedAt: datetime,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: CapabilityOptionsTypeDef](./type_defs.md#capabilityoptionstypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## PartnershipSummaryTypeDef

```python
# PartnershipSummaryTypeDef definition

class PartnershipSummaryTypeDef(TypedDict):
    profileId: str,
    partnershipId: str,
    createdAt: datetime,
    name: NotRequired[str],
    capabilities: NotRequired[List[str]],
    capabilityOptions: NotRequired[CapabilityOptionsTypeDef],  # (1)
    tradingPartnerId: NotRequired[str],
    modifiedAt: NotRequired[datetime],
```

1. See [:material-code-braces: CapabilityOptionsTypeDef](./type_defs.md#capabilityoptionstypedef) 
## UpdatePartnershipRequestRequestTypeDef

```python
# UpdatePartnershipRequestRequestTypeDef definition

class UpdatePartnershipRequestRequestTypeDef(TypedDict):
    partnershipId: str,
    name: NotRequired[str],
    capabilities: NotRequired[Sequence[str]],
    capabilityOptions: NotRequired[CapabilityOptionsTypeDef],  # (1)
```

1. See [:material-code-braces: CapabilityOptionsTypeDef](./type_defs.md#capabilityoptionstypedef) 
## UpdatePartnershipResponseTypeDef

```python
# UpdatePartnershipResponseTypeDef definition

class UpdatePartnershipResponseTypeDef(TypedDict):
    profileId: str,
    partnershipId: str,
    partnershipArn: str,
    name: str,
    email: str,
    phone: str,
    capabilities: List[str],
    capabilityOptions: CapabilityOptionsTypeDef,  # (1)
    tradingPartnerId: str,
    createdAt: datetime,
    modifiedAt: datetime,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: CapabilityOptionsTypeDef](./type_defs.md#capabilityoptionstypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListPartnershipsResponseTypeDef

```python
# ListPartnershipsResponseTypeDef definition

class ListPartnershipsResponseTypeDef(TypedDict):
    partnerships: List[PartnershipSummaryTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    nextToken: NotRequired[str],
```

1. See [:material-code-braces: PartnershipSummaryTypeDef](./type_defs.md#partnershipsummarytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
