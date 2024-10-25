# Type definitions

> [Index](../README.md) > [CustomerProfiles](./README.md) > Type definitions

!!! note ""

    Auto-generated documentation for [CustomerProfiles](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/customer-profiles.html#CustomerProfiles)
    type annotations stubs module [types-aiobotocore-customer-profiles](https://pypi.org/project/types-aiobotocore-customer-profiles/).

## TimestampTypeDef

```python
# TimestampTypeDef definition

TimestampTypeDef = Union[
    datetime,
    str,
]
```


## AttributeTypesSelectorUnionTypeDef

```python
# AttributeTypesSelectorUnionTypeDef definition

AttributeTypesSelectorUnionTypeDef = Union[
    AttributeTypesSelectorTypeDef,  # (1)
    AttributeTypesSelectorOutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: AttributeTypesSelectorTypeDef](./type_defs.md#attributetypesselectortypedef) 
2. See [:material-code-braces: AttributeTypesSelectorOutputTypeDef](./type_defs.md#attributetypesselectoroutputtypedef) 

## ConsolidationUnionTypeDef

```python
# ConsolidationUnionTypeDef definition

ConsolidationUnionTypeDef = Union[
    ConsolidationTypeDef,  # (1)
    ConsolidationOutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: ConsolidationTypeDef](./type_defs.md#consolidationtypedef) 
2. See [:material-code-braces: ConsolidationOutputTypeDef](./type_defs.md#consolidationoutputtypedef) 

## MatchingRuleUnionTypeDef

```python
# MatchingRuleUnionTypeDef definition

MatchingRuleUnionTypeDef = Union[
    MatchingRuleTypeDef,  # (1)
    MatchingRuleOutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: MatchingRuleTypeDef](./type_defs.md#matchingruletypedef) 
2. See [:material-code-braces: MatchingRuleOutputTypeDef](./type_defs.md#matchingruleoutputtypedef) 

## ObjectTypeKeyUnionTypeDef

```python
# ObjectTypeKeyUnionTypeDef definition

ObjectTypeKeyUnionTypeDef = Union[
    ObjectTypeKeyTypeDef,  # (1)
    ObjectTypeKeyOutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: ObjectTypeKeyTypeDef](./type_defs.md#objecttypekeytypedef) 
2. See [:material-code-braces: ObjectTypeKeyOutputTypeDef](./type_defs.md#objecttypekeyoutputtypedef) 

## AutoMergingUnionTypeDef

```python
# AutoMergingUnionTypeDef definition

AutoMergingUnionTypeDef = Union[
    AutoMergingTypeDef,  # (1)
    AutoMergingOutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: AutoMergingTypeDef](./type_defs.md#automergingtypedef) 
2. See [:material-code-braces: AutoMergingOutputTypeDef](./type_defs.md#automergingoutputtypedef) 



## AddProfileKeyRequestRequestTypeDef

```python
# AddProfileKeyRequestRequestTypeDef definition

class AddProfileKeyRequestRequestTypeDef(TypedDict):
    ProfileId: str,
    KeyName: str,
    Values: Sequence[str],
    DomainName: str,
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

## AdditionalSearchKeyTypeDef

```python
# AdditionalSearchKeyTypeDef definition

class AdditionalSearchKeyTypeDef(TypedDict):
    KeyName: str,
    Values: Sequence[str],
```

## AddressTypeDef

```python
# AddressTypeDef definition

class AddressTypeDef(TypedDict):
    Address1: NotRequired[str],
    Address2: NotRequired[str],
    Address3: NotRequired[str],
    Address4: NotRequired[str],
    City: NotRequired[str],
    County: NotRequired[str],
    State: NotRequired[str],
    Province: NotRequired[str],
    Country: NotRequired[str],
    PostalCode: NotRequired[str],
```

## AppflowIntegrationWorkflowAttributesTypeDef

```python
# AppflowIntegrationWorkflowAttributesTypeDef definition

class AppflowIntegrationWorkflowAttributesTypeDef(TypedDict):
    SourceConnectorType: SourceConnectorTypeType,  # (1)
    ConnectorProfileName: str,
    RoleArn: NotRequired[str],
```

1. See [:material-code-brackets: SourceConnectorTypeType](./literals.md#sourceconnectortypetype) 
## AppflowIntegrationWorkflowMetricsTypeDef

```python
# AppflowIntegrationWorkflowMetricsTypeDef definition

class AppflowIntegrationWorkflowMetricsTypeDef(TypedDict):
    RecordsProcessed: int,
    StepsCompleted: int,
    TotalSteps: int,
```

## AppflowIntegrationWorkflowStepTypeDef

```python
# AppflowIntegrationWorkflowStepTypeDef definition

class AppflowIntegrationWorkflowStepTypeDef(TypedDict):
    FlowName: str,
    Status: StatusType,  # (1)
    ExecutionMessage: str,
    RecordsProcessed: int,
    BatchRecordsStartTime: str,
    BatchRecordsEndTime: str,
    CreatedAt: datetime,
    LastUpdatedAt: datetime,
```

1. See [:material-code-brackets: StatusType](./literals.md#statustype) 
## AttributeItemTypeDef

```python
# AttributeItemTypeDef definition

class AttributeItemTypeDef(TypedDict):
    Name: str,
```

## AttributeTypesSelectorOutputTypeDef

```python
# AttributeTypesSelectorOutputTypeDef definition

class AttributeTypesSelectorOutputTypeDef(TypedDict):
    AttributeMatchingModel: AttributeMatchingModelType,  # (1)
    Address: NotRequired[List[str]],
    PhoneNumber: NotRequired[List[str]],
    EmailAddress: NotRequired[List[str]],
```

1. See [:material-code-brackets: AttributeMatchingModelType](./literals.md#attributematchingmodeltype) 
## AttributeTypesSelectorTypeDef

```python
# AttributeTypesSelectorTypeDef definition

class AttributeTypesSelectorTypeDef(TypedDict):
    AttributeMatchingModel: AttributeMatchingModelType,  # (1)
    Address: NotRequired[Sequence[str]],
    PhoneNumber: NotRequired[Sequence[str]],
    EmailAddress: NotRequired[Sequence[str]],
```

1. See [:material-code-brackets: AttributeMatchingModelType](./literals.md#attributematchingmodeltype) 
## ConflictResolutionTypeDef

```python
# ConflictResolutionTypeDef definition

class ConflictResolutionTypeDef(TypedDict):
    ConflictResolvingModel: ConflictResolvingModelType,  # (1)
    SourceName: NotRequired[str],
```

1. See [:material-code-brackets: ConflictResolvingModelType](./literals.md#conflictresolvingmodeltype) 
## ConsolidationOutputTypeDef

```python
# ConsolidationOutputTypeDef definition

class ConsolidationOutputTypeDef(TypedDict):
    MatchingAttributesList: List[List[str]],
```

## RangeTypeDef

```python
# RangeTypeDef definition

class RangeTypeDef(TypedDict):
    Value: int,
    Unit: UnitType,  # (1)
```

1. See [:material-code-brackets: UnitType](./literals.md#unittype) 
## ThresholdTypeDef

```python
# ThresholdTypeDef definition

class ThresholdTypeDef(TypedDict):
    Value: str,
    Operator: OperatorType,  # (1)
```

1. See [:material-code-brackets: OperatorType](./literals.md#operatortype) 
## ConnectorOperatorTypeDef

```python
# ConnectorOperatorTypeDef definition

class ConnectorOperatorTypeDef(TypedDict):
    Marketo: NotRequired[MarketoConnectorOperatorType],  # (1)
    S3: NotRequired[S3ConnectorOperatorType],  # (2)
    Salesforce: NotRequired[SalesforceConnectorOperatorType],  # (3)
    ServiceNow: NotRequired[ServiceNowConnectorOperatorType],  # (4)
    Zendesk: NotRequired[ZendeskConnectorOperatorType],  # (5)
```

1. See [:material-code-brackets: MarketoConnectorOperatorType](./literals.md#marketoconnectoroperatortype) 
2. See [:material-code-brackets: S3ConnectorOperatorType](./literals.md#s3connectoroperatortype) 
3. See [:material-code-brackets: SalesforceConnectorOperatorType](./literals.md#salesforceconnectoroperatortype) 
4. See [:material-code-brackets: ServiceNowConnectorOperatorType](./literals.md#servicenowconnectoroperatortype) 
5. See [:material-code-brackets: ZendeskConnectorOperatorType](./literals.md#zendeskconnectoroperatortype) 
## ConsolidationTypeDef

```python
# ConsolidationTypeDef definition

class ConsolidationTypeDef(TypedDict):
    MatchingAttributesList: Sequence[Sequence[str]],
```

## CreateEventStreamRequestRequestTypeDef

```python
# CreateEventStreamRequestRequestTypeDef definition

class CreateEventStreamRequestRequestTypeDef(TypedDict):
    DomainName: str,
    Uri: str,
    EventStreamName: str,
    Tags: NotRequired[Mapping[str, str]],
```

## DeleteCalculatedAttributeDefinitionRequestRequestTypeDef

```python
# DeleteCalculatedAttributeDefinitionRequestRequestTypeDef definition

class DeleteCalculatedAttributeDefinitionRequestRequestTypeDef(TypedDict):
    DomainName: str,
    CalculatedAttributeName: str,
```

## DeleteDomainRequestRequestTypeDef

```python
# DeleteDomainRequestRequestTypeDef definition

class DeleteDomainRequestRequestTypeDef(TypedDict):
    DomainName: str,
```

## DeleteEventStreamRequestRequestTypeDef

```python
# DeleteEventStreamRequestRequestTypeDef definition

class DeleteEventStreamRequestRequestTypeDef(TypedDict):
    DomainName: str,
    EventStreamName: str,
```

## DeleteIntegrationRequestRequestTypeDef

```python
# DeleteIntegrationRequestRequestTypeDef definition

class DeleteIntegrationRequestRequestTypeDef(TypedDict):
    DomainName: str,
    Uri: str,
```

## DeleteProfileKeyRequestRequestTypeDef

```python
# DeleteProfileKeyRequestRequestTypeDef definition

class DeleteProfileKeyRequestRequestTypeDef(TypedDict):
    ProfileId: str,
    KeyName: str,
    Values: Sequence[str],
    DomainName: str,
```

## DeleteProfileObjectRequestRequestTypeDef

```python
# DeleteProfileObjectRequestRequestTypeDef definition

class DeleteProfileObjectRequestRequestTypeDef(TypedDict):
    ProfileId: str,
    ProfileObjectUniqueKey: str,
    ObjectTypeName: str,
    DomainName: str,
```

## DeleteProfileObjectTypeRequestRequestTypeDef

```python
# DeleteProfileObjectTypeRequestRequestTypeDef definition

class DeleteProfileObjectTypeRequestRequestTypeDef(TypedDict):
    DomainName: str,
    ObjectTypeName: str,
```

## DeleteProfileRequestRequestTypeDef

```python
# DeleteProfileRequestRequestTypeDef definition

class DeleteProfileRequestRequestTypeDef(TypedDict):
    ProfileId: str,
    DomainName: str,
```

## DeleteWorkflowRequestRequestTypeDef

```python
# DeleteWorkflowRequestRequestTypeDef definition

class DeleteWorkflowRequestRequestTypeDef(TypedDict):
    DomainName: str,
    WorkflowId: str,
```

## DestinationSummaryTypeDef

```python
# DestinationSummaryTypeDef definition

class DestinationSummaryTypeDef(TypedDict):
    Uri: str,
    Status: EventStreamDestinationStatusType,  # (1)
    UnhealthySince: NotRequired[datetime],
```

1. See [:material-code-brackets: EventStreamDestinationStatusType](./literals.md#eventstreamdestinationstatustype) 
## DetectProfileObjectTypeRequestRequestTypeDef

```python
# DetectProfileObjectTypeRequestRequestTypeDef definition

class DetectProfileObjectTypeRequestRequestTypeDef(TypedDict):
    Objects: Sequence[str],
    DomainName: str,
```

## ObjectTypeFieldTypeDef

```python
# ObjectTypeFieldTypeDef definition

class ObjectTypeFieldTypeDef(TypedDict):
    Source: NotRequired[str],
    Target: NotRequired[str],
    ContentType: NotRequired[FieldContentTypeType],  # (1)
```

1. See [:material-code-brackets: FieldContentTypeType](./literals.md#fieldcontenttypetype) 
## ObjectTypeKeyOutputTypeDef

```python
# ObjectTypeKeyOutputTypeDef definition

class ObjectTypeKeyOutputTypeDef(TypedDict):
    StandardIdentifiers: NotRequired[List[StandardIdentifierType]],  # (1)
    FieldNames: NotRequired[List[str]],
```

1. See [:material-code-brackets: StandardIdentifierType](./literals.md#standardidentifiertype) 
## DomainStatsTypeDef

```python
# DomainStatsTypeDef definition

class DomainStatsTypeDef(TypedDict):
    ProfileCount: NotRequired[int],
    MeteringProfileCount: NotRequired[int],
    ObjectCount: NotRequired[int],
    TotalSize: NotRequired[int],
```

## EventStreamDestinationDetailsTypeDef

```python
# EventStreamDestinationDetailsTypeDef definition

class EventStreamDestinationDetailsTypeDef(TypedDict):
    Uri: str,
    Status: EventStreamDestinationStatusType,  # (1)
    UnhealthySince: NotRequired[datetime],
    Message: NotRequired[str],
```

1. See [:material-code-brackets: EventStreamDestinationStatusType](./literals.md#eventstreamdestinationstatustype) 
## S3ExportingConfigTypeDef

```python
# S3ExportingConfigTypeDef definition

class S3ExportingConfigTypeDef(TypedDict):
    S3BucketName: str,
    S3KeyName: NotRequired[str],
```

## S3ExportingLocationTypeDef

```python
# S3ExportingLocationTypeDef definition

class S3ExportingLocationTypeDef(TypedDict):
    S3BucketName: NotRequired[str],
    S3KeyName: NotRequired[str],
```

## FieldSourceProfileIdsTypeDef

```python
# FieldSourceProfileIdsTypeDef definition

class FieldSourceProfileIdsTypeDef(TypedDict):
    AccountNumber: NotRequired[str],
    AdditionalInformation: NotRequired[str],
    PartyType: NotRequired[str],
    BusinessName: NotRequired[str],
    FirstName: NotRequired[str],
    MiddleName: NotRequired[str],
    LastName: NotRequired[str],
    BirthDate: NotRequired[str],
    Gender: NotRequired[str],
    PhoneNumber: NotRequired[str],
    MobilePhoneNumber: NotRequired[str],
    HomePhoneNumber: NotRequired[str],
    BusinessPhoneNumber: NotRequired[str],
    EmailAddress: NotRequired[str],
    PersonalEmailAddress: NotRequired[str],
    BusinessEmailAddress: NotRequired[str],
    Address: NotRequired[str],
    ShippingAddress: NotRequired[str],
    MailingAddress: NotRequired[str],
    BillingAddress: NotRequired[str],
    Attributes: NotRequired[Mapping[str, str]],
```

## FoundByKeyValueTypeDef

```python
# FoundByKeyValueTypeDef definition

class FoundByKeyValueTypeDef(TypedDict):
    KeyName: NotRequired[str],
    Values: NotRequired[List[str]],
```

## GetCalculatedAttributeDefinitionRequestRequestTypeDef

```python
# GetCalculatedAttributeDefinitionRequestRequestTypeDef definition

class GetCalculatedAttributeDefinitionRequestRequestTypeDef(TypedDict):
    DomainName: str,
    CalculatedAttributeName: str,
```

## GetCalculatedAttributeForProfileRequestRequestTypeDef

```python
# GetCalculatedAttributeForProfileRequestRequestTypeDef definition

class GetCalculatedAttributeForProfileRequestRequestTypeDef(TypedDict):
    DomainName: str,
    ProfileId: str,
    CalculatedAttributeName: str,
```

## GetDomainRequestRequestTypeDef

```python
# GetDomainRequestRequestTypeDef definition

class GetDomainRequestRequestTypeDef(TypedDict):
    DomainName: str,
```

## GetEventStreamRequestRequestTypeDef

```python
# GetEventStreamRequestRequestTypeDef definition

class GetEventStreamRequestRequestTypeDef(TypedDict):
    DomainName: str,
    EventStreamName: str,
```

## GetIdentityResolutionJobRequestRequestTypeDef

```python
# GetIdentityResolutionJobRequestRequestTypeDef definition

class GetIdentityResolutionJobRequestRequestTypeDef(TypedDict):
    DomainName: str,
    JobId: str,
```

## JobStatsTypeDef

```python
# JobStatsTypeDef definition

class JobStatsTypeDef(TypedDict):
    NumberOfProfilesReviewed: NotRequired[int],
    NumberOfMatchesFound: NotRequired[int],
    NumberOfMergesDone: NotRequired[int],
```

## GetIntegrationRequestRequestTypeDef

```python
# GetIntegrationRequestRequestTypeDef definition

class GetIntegrationRequestRequestTypeDef(TypedDict):
    DomainName: str,
    Uri: str,
```

## GetMatchesRequestRequestTypeDef

```python
# GetMatchesRequestRequestTypeDef definition

class GetMatchesRequestRequestTypeDef(TypedDict):
    DomainName: str,
    NextToken: NotRequired[str],
    MaxResults: NotRequired[int],
```

## MatchItemTypeDef

```python
# MatchItemTypeDef definition

class MatchItemTypeDef(TypedDict):
    MatchId: NotRequired[str],
    ProfileIds: NotRequired[List[str]],
    ConfidenceScore: NotRequired[float],
```

## GetProfileObjectTypeRequestRequestTypeDef

```python
# GetProfileObjectTypeRequestRequestTypeDef definition

class GetProfileObjectTypeRequestRequestTypeDef(TypedDict):
    DomainName: str,
    ObjectTypeName: str,
```

## GetProfileObjectTypeTemplateRequestRequestTypeDef

```python
# GetProfileObjectTypeTemplateRequestRequestTypeDef definition

class GetProfileObjectTypeTemplateRequestRequestTypeDef(TypedDict):
    TemplateId: str,
```

## GetSimilarProfilesRequestRequestTypeDef

```python
# GetSimilarProfilesRequestRequestTypeDef definition

class GetSimilarProfilesRequestRequestTypeDef(TypedDict):
    DomainName: str,
    MatchType: MatchTypeType,  # (1)
    SearchKey: str,
    SearchValue: str,
    NextToken: NotRequired[str],
    MaxResults: NotRequired[int],
```

1. See [:material-code-brackets: MatchTypeType](./literals.md#matchtypetype) 
## GetWorkflowRequestRequestTypeDef

```python
# GetWorkflowRequestRequestTypeDef definition

class GetWorkflowRequestRequestTypeDef(TypedDict):
    DomainName: str,
    WorkflowId: str,
```

## GetWorkflowStepsRequestRequestTypeDef

```python
# GetWorkflowStepsRequestRequestTypeDef definition

class GetWorkflowStepsRequestRequestTypeDef(TypedDict):
    DomainName: str,
    WorkflowId: str,
    NextToken: NotRequired[str],
    MaxResults: NotRequired[int],
```

## IncrementalPullConfigTypeDef

```python
# IncrementalPullConfigTypeDef definition

class IncrementalPullConfigTypeDef(TypedDict):
    DatetimeTypeFieldName: NotRequired[str],
```

## JobScheduleTypeDef

```python
# JobScheduleTypeDef definition

class JobScheduleTypeDef(TypedDict):
    DayOfTheWeek: JobScheduleDayOfTheWeekType,  # (1)
    Time: str,
```

1. See [:material-code-brackets: JobScheduleDayOfTheWeekType](./literals.md#jobscheduledayoftheweektype) 
## ListAccountIntegrationsRequestRequestTypeDef

```python
# ListAccountIntegrationsRequestRequestTypeDef definition

class ListAccountIntegrationsRequestRequestTypeDef(TypedDict):
    Uri: str,
    NextToken: NotRequired[str],
    MaxResults: NotRequired[int],
    IncludeHidden: NotRequired[bool],
```

## ListIntegrationItemTypeDef

```python
# ListIntegrationItemTypeDef definition

class ListIntegrationItemTypeDef(TypedDict):
    DomainName: str,
    Uri: str,
    CreatedAt: datetime,
    LastUpdatedAt: datetime,
    ObjectTypeName: NotRequired[str],
    Tags: NotRequired[Dict[str, str]],
    ObjectTypeNames: NotRequired[Dict[str, str]],
    WorkflowId: NotRequired[str],
    IsUnstructured: NotRequired[bool],
    RoleArn: NotRequired[str],
```

## ListCalculatedAttributeDefinitionItemTypeDef

```python
# ListCalculatedAttributeDefinitionItemTypeDef definition

class ListCalculatedAttributeDefinitionItemTypeDef(TypedDict):
    CalculatedAttributeName: NotRequired[str],
    DisplayName: NotRequired[str],
    Description: NotRequired[str],
    CreatedAt: NotRequired[datetime],
    LastUpdatedAt: NotRequired[datetime],
    Tags: NotRequired[Dict[str, str]],
```

## ListCalculatedAttributeDefinitionsRequestRequestTypeDef

```python
# ListCalculatedAttributeDefinitionsRequestRequestTypeDef definition

class ListCalculatedAttributeDefinitionsRequestRequestTypeDef(TypedDict):
    DomainName: str,
    NextToken: NotRequired[str],
    MaxResults: NotRequired[int],
```

## ListCalculatedAttributeForProfileItemTypeDef

```python
# ListCalculatedAttributeForProfileItemTypeDef definition

class ListCalculatedAttributeForProfileItemTypeDef(TypedDict):
    CalculatedAttributeName: NotRequired[str],
    DisplayName: NotRequired[str],
    IsDataPartial: NotRequired[str],
    Value: NotRequired[str],
```

## ListCalculatedAttributesForProfileRequestRequestTypeDef

```python
# ListCalculatedAttributesForProfileRequestRequestTypeDef definition

class ListCalculatedAttributesForProfileRequestRequestTypeDef(TypedDict):
    DomainName: str,
    ProfileId: str,
    NextToken: NotRequired[str],
    MaxResults: NotRequired[int],
```

## ListDomainItemTypeDef

```python
# ListDomainItemTypeDef definition

class ListDomainItemTypeDef(TypedDict):
    DomainName: str,
    CreatedAt: datetime,
    LastUpdatedAt: datetime,
    Tags: NotRequired[Dict[str, str]],
```

## ListDomainsRequestRequestTypeDef

```python
# ListDomainsRequestRequestTypeDef definition

class ListDomainsRequestRequestTypeDef(TypedDict):
    NextToken: NotRequired[str],
    MaxResults: NotRequired[int],
```

## PaginatorConfigTypeDef

```python
# PaginatorConfigTypeDef definition

class PaginatorConfigTypeDef(TypedDict):
    MaxItems: NotRequired[int],
    PageSize: NotRequired[int],
    StartingToken: NotRequired[str],
```

## ListEventStreamsRequestRequestTypeDef

```python
# ListEventStreamsRequestRequestTypeDef definition

class ListEventStreamsRequestRequestTypeDef(TypedDict):
    DomainName: str,
    NextToken: NotRequired[str],
    MaxResults: NotRequired[int],
```

## ListIdentityResolutionJobsRequestRequestTypeDef

```python
# ListIdentityResolutionJobsRequestRequestTypeDef definition

class ListIdentityResolutionJobsRequestRequestTypeDef(TypedDict):
    DomainName: str,
    NextToken: NotRequired[str],
    MaxResults: NotRequired[int],
```

## ListIntegrationsRequestRequestTypeDef

```python
# ListIntegrationsRequestRequestTypeDef definition

class ListIntegrationsRequestRequestTypeDef(TypedDict):
    DomainName: str,
    NextToken: NotRequired[str],
    MaxResults: NotRequired[int],
    IncludeHidden: NotRequired[bool],
```

## ListProfileObjectTypeItemTypeDef

```python
# ListProfileObjectTypeItemTypeDef definition

class ListProfileObjectTypeItemTypeDef(TypedDict):
    ObjectTypeName: str,
    Description: str,
    CreatedAt: NotRequired[datetime],
    LastUpdatedAt: NotRequired[datetime],
    MaxProfileObjectCount: NotRequired[int],
    MaxAvailableProfileObjectCount: NotRequired[int],
    Tags: NotRequired[Dict[str, str]],
```

## ListProfileObjectTypeTemplateItemTypeDef

```python
# ListProfileObjectTypeTemplateItemTypeDef definition

class ListProfileObjectTypeTemplateItemTypeDef(TypedDict):
    TemplateId: NotRequired[str],
    SourceName: NotRequired[str],
    SourceObject: NotRequired[str],
```

## ListProfileObjectTypeTemplatesRequestRequestTypeDef

```python
# ListProfileObjectTypeTemplatesRequestRequestTypeDef definition

class ListProfileObjectTypeTemplatesRequestRequestTypeDef(TypedDict):
    NextToken: NotRequired[str],
    MaxResults: NotRequired[int],
```

## ListProfileObjectTypesRequestRequestTypeDef

```python
# ListProfileObjectTypesRequestRequestTypeDef definition

class ListProfileObjectTypesRequestRequestTypeDef(TypedDict):
    DomainName: str,
    NextToken: NotRequired[str],
    MaxResults: NotRequired[int],
```

## ListProfileObjectsItemTypeDef

```python
# ListProfileObjectsItemTypeDef definition

class ListProfileObjectsItemTypeDef(TypedDict):
    ObjectTypeName: NotRequired[str],
    ProfileObjectUniqueKey: NotRequired[str],
    Object: NotRequired[str],
```

## ObjectFilterTypeDef

```python
# ObjectFilterTypeDef definition

class ObjectFilterTypeDef(TypedDict):
    KeyName: str,
    Values: Sequence[str],
```

## ListRuleBasedMatchesRequestRequestTypeDef

```python
# ListRuleBasedMatchesRequestRequestTypeDef definition

class ListRuleBasedMatchesRequestRequestTypeDef(TypedDict):
    DomainName: str,
    NextToken: NotRequired[str],
    MaxResults: NotRequired[int],
```

## ListTagsForResourceRequestRequestTypeDef

```python
# ListTagsForResourceRequestRequestTypeDef definition

class ListTagsForResourceRequestRequestTypeDef(TypedDict):
    resourceArn: str,
```

## ListWorkflowsItemTypeDef

```python
# ListWorkflowsItemTypeDef definition

class ListWorkflowsItemTypeDef(TypedDict):
    WorkflowType: WorkflowTypeType,  # (1)
    WorkflowId: str,
    Status: StatusType,  # (2)
    StatusDescription: str,
    CreatedAt: datetime,
    LastUpdatedAt: datetime,
```

1. See [:material-code-brackets: WorkflowTypeType](./literals.md#workflowtypetype) 
2. See [:material-code-brackets: StatusType](./literals.md#statustype) 
## MarketoSourcePropertiesTypeDef

```python
# MarketoSourcePropertiesTypeDef definition

class MarketoSourcePropertiesTypeDef(TypedDict):
    Object: str,
```

## MatchingRuleOutputTypeDef

```python
# MatchingRuleOutputTypeDef definition

class MatchingRuleOutputTypeDef(TypedDict):
    Rule: List[str],
```

## MatchingRuleTypeDef

```python
# MatchingRuleTypeDef definition

class MatchingRuleTypeDef(TypedDict):
    Rule: Sequence[str],
```

## ObjectTypeKeyTypeDef

```python
# ObjectTypeKeyTypeDef definition

class ObjectTypeKeyTypeDef(TypedDict):
    StandardIdentifiers: NotRequired[Sequence[StandardIdentifierType]],  # (1)
    FieldNames: NotRequired[Sequence[str]],
```

1. See [:material-code-brackets: StandardIdentifierType](./literals.md#standardidentifiertype) 
## PutProfileObjectRequestRequestTypeDef

```python
# PutProfileObjectRequestRequestTypeDef definition

class PutProfileObjectRequestRequestTypeDef(TypedDict):
    ObjectTypeName: str,
    Object: str,
    DomainName: str,
```

## S3SourcePropertiesTypeDef

```python
# S3SourcePropertiesTypeDef definition

class S3SourcePropertiesTypeDef(TypedDict):
    BucketName: str,
    BucketPrefix: NotRequired[str],
```

## SalesforceSourcePropertiesTypeDef

```python
# SalesforceSourcePropertiesTypeDef definition

class SalesforceSourcePropertiesTypeDef(TypedDict):
    Object: str,
    EnableDynamicFieldUpdate: NotRequired[bool],
    IncludeDeletedRecords: NotRequired[bool],
```

## ServiceNowSourcePropertiesTypeDef

```python
# ServiceNowSourcePropertiesTypeDef definition

class ServiceNowSourcePropertiesTypeDef(TypedDict):
    Object: str,
```

## ZendeskSourcePropertiesTypeDef

```python
# ZendeskSourcePropertiesTypeDef definition

class ZendeskSourcePropertiesTypeDef(TypedDict):
    Object: str,
```

## TagResourceRequestRequestTypeDef

```python
# TagResourceRequestRequestTypeDef definition

class TagResourceRequestRequestTypeDef(TypedDict):
    resourceArn: str,
    tags: Mapping[str, str],
```

## UntagResourceRequestRequestTypeDef

```python
# UntagResourceRequestRequestTypeDef definition

class UntagResourceRequestRequestTypeDef(TypedDict):
    resourceArn: str,
    tagKeys: Sequence[str],
```

## UpdateAddressTypeDef

```python
# UpdateAddressTypeDef definition

class UpdateAddressTypeDef(TypedDict):
    Address1: NotRequired[str],
    Address2: NotRequired[str],
    Address3: NotRequired[str],
    Address4: NotRequired[str],
    City: NotRequired[str],
    County: NotRequired[str],
    State: NotRequired[str],
    Province: NotRequired[str],
    Country: NotRequired[str],
    PostalCode: NotRequired[str],
```

## AddProfileKeyResponseTypeDef

```python
# AddProfileKeyResponseTypeDef definition

class AddProfileKeyResponseTypeDef(TypedDict):
    KeyName: str,
    Values: List[str],
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateEventStreamResponseTypeDef

```python
# CreateEventStreamResponseTypeDef definition

class CreateEventStreamResponseTypeDef(TypedDict):
    EventStreamArn: str,
    Tags: Dict[str, str],
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateIntegrationWorkflowResponseTypeDef

```python
# CreateIntegrationWorkflowResponseTypeDef definition

class CreateIntegrationWorkflowResponseTypeDef(TypedDict):
    WorkflowId: str,
    Message: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateProfileResponseTypeDef

```python
# CreateProfileResponseTypeDef definition

class CreateProfileResponseTypeDef(TypedDict):
    ProfileId: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DeleteDomainResponseTypeDef

```python
# DeleteDomainResponseTypeDef definition

class DeleteDomainResponseTypeDef(TypedDict):
    Message: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DeleteIntegrationResponseTypeDef

```python
# DeleteIntegrationResponseTypeDef definition

class DeleteIntegrationResponseTypeDef(TypedDict):
    Message: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DeleteProfileKeyResponseTypeDef

```python
# DeleteProfileKeyResponseTypeDef definition

class DeleteProfileKeyResponseTypeDef(TypedDict):
    Message: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DeleteProfileObjectResponseTypeDef

```python
# DeleteProfileObjectResponseTypeDef definition

class DeleteProfileObjectResponseTypeDef(TypedDict):
    Message: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DeleteProfileObjectTypeResponseTypeDef

```python
# DeleteProfileObjectTypeResponseTypeDef definition

class DeleteProfileObjectTypeResponseTypeDef(TypedDict):
    Message: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DeleteProfileResponseTypeDef

```python
# DeleteProfileResponseTypeDef definition

class DeleteProfileResponseTypeDef(TypedDict):
    Message: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetAutoMergingPreviewResponseTypeDef

```python
# GetAutoMergingPreviewResponseTypeDef definition

class GetAutoMergingPreviewResponseTypeDef(TypedDict):
    DomainName: str,
    NumberOfMatchesInSample: int,
    NumberOfProfilesInSample: int,
    NumberOfProfilesWillBeMerged: int,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetCalculatedAttributeForProfileResponseTypeDef

```python
# GetCalculatedAttributeForProfileResponseTypeDef definition

class GetCalculatedAttributeForProfileResponseTypeDef(TypedDict):
    CalculatedAttributeName: str,
    DisplayName: str,
    IsDataPartial: str,
    Value: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetIntegrationResponseTypeDef

```python
# GetIntegrationResponseTypeDef definition

class GetIntegrationResponseTypeDef(TypedDict):
    DomainName: str,
    Uri: str,
    ObjectTypeName: str,
    CreatedAt: datetime,
    LastUpdatedAt: datetime,
    Tags: Dict[str, str],
    ObjectTypeNames: Dict[str, str],
    WorkflowId: str,
    IsUnstructured: bool,
    RoleArn: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetSimilarProfilesResponseTypeDef

```python
# GetSimilarProfilesResponseTypeDef definition

class GetSimilarProfilesResponseTypeDef(TypedDict):
    ProfileIds: List[str],
    MatchId: str,
    MatchType: MatchTypeType,  # (1)
    RuleLevel: int,
    ConfidenceScore: float,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See [:material-code-brackets: MatchTypeType](./literals.md#matchtypetype) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListRuleBasedMatchesResponseTypeDef

```python
# ListRuleBasedMatchesResponseTypeDef definition

class ListRuleBasedMatchesResponseTypeDef(TypedDict):
    MatchIds: List[str],
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListTagsForResourceResponseTypeDef

```python
# ListTagsForResourceResponseTypeDef definition

class ListTagsForResourceResponseTypeDef(TypedDict):
    tags: Dict[str, str],
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## MergeProfilesResponseTypeDef

```python
# MergeProfilesResponseTypeDef definition

class MergeProfilesResponseTypeDef(TypedDict):
    Message: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## PutIntegrationResponseTypeDef

```python
# PutIntegrationResponseTypeDef definition

class PutIntegrationResponseTypeDef(TypedDict):
    DomainName: str,
    Uri: str,
    ObjectTypeName: str,
    CreatedAt: datetime,
    LastUpdatedAt: datetime,
    Tags: Dict[str, str],
    ObjectTypeNames: Dict[str, str],
    WorkflowId: str,
    IsUnstructured: bool,
    RoleArn: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## PutProfileObjectResponseTypeDef

```python
# PutProfileObjectResponseTypeDef definition

class PutProfileObjectResponseTypeDef(TypedDict):
    ProfileObjectUniqueKey: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdateProfileResponseTypeDef

```python
# UpdateProfileResponseTypeDef definition

class UpdateProfileResponseTypeDef(TypedDict):
    ProfileId: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## SearchProfilesRequestRequestTypeDef

```python
# SearchProfilesRequestRequestTypeDef definition

class SearchProfilesRequestRequestTypeDef(TypedDict):
    DomainName: str,
    KeyName: str,
    Values: Sequence[str],
    NextToken: NotRequired[str],
    MaxResults: NotRequired[int],
    AdditionalSearchKeys: NotRequired[Sequence[AdditionalSearchKeyTypeDef]],  # (1)
    LogicalOperator: NotRequired[LogicalOperatorType],  # (2)
```

1. See [:material-code-braces: AdditionalSearchKeyTypeDef](./type_defs.md#additionalsearchkeytypedef) 
2. See [:material-code-brackets: LogicalOperatorType](./literals.md#logicaloperatortype) 
## CreateProfileRequestRequestTypeDef

```python
# CreateProfileRequestRequestTypeDef definition

class CreateProfileRequestRequestTypeDef(TypedDict):
    DomainName: str,
    AccountNumber: NotRequired[str],
    AdditionalInformation: NotRequired[str],
    PartyType: NotRequired[PartyTypeType],  # (1)
    BusinessName: NotRequired[str],
    FirstName: NotRequired[str],
    MiddleName: NotRequired[str],
    LastName: NotRequired[str],
    BirthDate: NotRequired[str],
    Gender: NotRequired[GenderType],  # (2)
    PhoneNumber: NotRequired[str],
    MobilePhoneNumber: NotRequired[str],
    HomePhoneNumber: NotRequired[str],
    BusinessPhoneNumber: NotRequired[str],
    EmailAddress: NotRequired[str],
    PersonalEmailAddress: NotRequired[str],
    BusinessEmailAddress: NotRequired[str],
    Address: NotRequired[AddressTypeDef],  # (3)
    ShippingAddress: NotRequired[AddressTypeDef],  # (3)
    MailingAddress: NotRequired[AddressTypeDef],  # (3)
    BillingAddress: NotRequired[AddressTypeDef],  # (3)
    Attributes: NotRequired[Mapping[str, str]],
    PartyTypeString: NotRequired[str],
    GenderString: NotRequired[str],
```

1. See [:material-code-brackets: PartyTypeType](./literals.md#partytypetype) 
2. See [:material-code-brackets: GenderType](./literals.md#gendertype) 
3. See [:material-code-braces: AddressTypeDef](./type_defs.md#addresstypedef) 
4. See [:material-code-braces: AddressTypeDef](./type_defs.md#addresstypedef) 
5. See [:material-code-braces: AddressTypeDef](./type_defs.md#addresstypedef) 
6. See [:material-code-braces: AddressTypeDef](./type_defs.md#addresstypedef) 
## WorkflowAttributesTypeDef

```python
# WorkflowAttributesTypeDef definition

class WorkflowAttributesTypeDef(TypedDict):
    AppflowIntegration: NotRequired[AppflowIntegrationWorkflowAttributesTypeDef],  # (1)
```

1. See [:material-code-braces: AppflowIntegrationWorkflowAttributesTypeDef](./type_defs.md#appflowintegrationworkflowattributestypedef) 
## WorkflowMetricsTypeDef

```python
# WorkflowMetricsTypeDef definition

class WorkflowMetricsTypeDef(TypedDict):
    AppflowIntegration: NotRequired[AppflowIntegrationWorkflowMetricsTypeDef],  # (1)
```

1. See [:material-code-braces: AppflowIntegrationWorkflowMetricsTypeDef](./type_defs.md#appflowintegrationworkflowmetricstypedef) 
## WorkflowStepItemTypeDef

```python
# WorkflowStepItemTypeDef definition

class WorkflowStepItemTypeDef(TypedDict):
    AppflowIntegration: NotRequired[AppflowIntegrationWorkflowStepTypeDef],  # (1)
```

1. See [:material-code-braces: AppflowIntegrationWorkflowStepTypeDef](./type_defs.md#appflowintegrationworkflowsteptypedef) 
## AttributeDetailsOutputTypeDef

```python
# AttributeDetailsOutputTypeDef definition

class AttributeDetailsOutputTypeDef(TypedDict):
    Attributes: List[AttributeItemTypeDef],  # (1)
    Expression: str,
```

1. See [:material-code-braces: AttributeItemTypeDef](./type_defs.md#attributeitemtypedef) 
## AttributeDetailsTypeDef

```python
# AttributeDetailsTypeDef definition

class AttributeDetailsTypeDef(TypedDict):
    Attributes: Sequence[AttributeItemTypeDef],  # (1)
    Expression: str,
```

1. See [:material-code-braces: AttributeItemTypeDef](./type_defs.md#attributeitemtypedef) 
## AutoMergingOutputTypeDef

```python
# AutoMergingOutputTypeDef definition

class AutoMergingOutputTypeDef(TypedDict):
    Enabled: bool,
    Consolidation: NotRequired[ConsolidationOutputTypeDef],  # (1)
    ConflictResolution: NotRequired[ConflictResolutionTypeDef],  # (2)
    MinAllowedConfidenceScoreForMerging: NotRequired[float],
```

1. See [:material-code-braces: ConsolidationOutputTypeDef](./type_defs.md#consolidationoutputtypedef) 
2. See [:material-code-braces: ConflictResolutionTypeDef](./type_defs.md#conflictresolutiontypedef) 
## BatchTypeDef

```python
# BatchTypeDef definition

class BatchTypeDef(TypedDict):
    StartTime: TimestampTypeDef,
    EndTime: TimestampTypeDef,
```

## ListWorkflowsRequestRequestTypeDef

```python
# ListWorkflowsRequestRequestTypeDef definition

class ListWorkflowsRequestRequestTypeDef(TypedDict):
    DomainName: str,
    WorkflowType: NotRequired[WorkflowTypeType],  # (1)
    Status: NotRequired[StatusType],  # (2)
    QueryStartDate: NotRequired[TimestampTypeDef],
    QueryEndDate: NotRequired[TimestampTypeDef],
    NextToken: NotRequired[str],
    MaxResults: NotRequired[int],
```

1. See [:material-code-brackets: WorkflowTypeType](./literals.md#workflowtypetype) 
2. See [:material-code-brackets: StatusType](./literals.md#statustype) 
## ScheduledTriggerPropertiesTypeDef

```python
# ScheduledTriggerPropertiesTypeDef definition

class ScheduledTriggerPropertiesTypeDef(TypedDict):
    ScheduleExpression: str,
    DataPullMode: NotRequired[DataPullModeType],  # (1)
    ScheduleStartTime: NotRequired[TimestampTypeDef],
    ScheduleEndTime: NotRequired[TimestampTypeDef],
    Timezone: NotRequired[str],
    ScheduleOffset: NotRequired[int],
    FirstExecutionFrom: NotRequired[TimestampTypeDef],
```

1. See [:material-code-brackets: DataPullModeType](./literals.md#datapullmodetype) 
## ConditionsTypeDef

```python
# ConditionsTypeDef definition

class ConditionsTypeDef(TypedDict):
    Range: NotRequired[RangeTypeDef],  # (1)
    ObjectCount: NotRequired[int],
    Threshold: NotRequired[ThresholdTypeDef],  # (2)
```

1. See [:material-code-braces: RangeTypeDef](./type_defs.md#rangetypedef) 
2. See [:material-code-braces: ThresholdTypeDef](./type_defs.md#thresholdtypedef) 
## TaskTypeDef

```python
# TaskTypeDef definition

class TaskTypeDef(TypedDict):
    SourceFields: Sequence[str],
    TaskType: TaskTypeType,  # (3)
    ConnectorOperator: NotRequired[ConnectorOperatorTypeDef],  # (1)
    DestinationField: NotRequired[str],
    TaskProperties: NotRequired[Mapping[OperatorPropertiesKeysType, str]],  # (2)
```

1. See [:material-code-braces: ConnectorOperatorTypeDef](./type_defs.md#connectoroperatortypedef) 
2. See [:material-code-brackets: OperatorPropertiesKeysType](./literals.md#operatorpropertieskeystype) 
3. See [:material-code-brackets: TaskTypeType](./literals.md#tasktypetype) 
## GetAutoMergingPreviewRequestRequestTypeDef

```python
# GetAutoMergingPreviewRequestRequestTypeDef definition

class GetAutoMergingPreviewRequestRequestTypeDef(TypedDict):
    DomainName: str,
    Consolidation: ConsolidationTypeDef,  # (1)
    ConflictResolution: ConflictResolutionTypeDef,  # (2)
    MinAllowedConfidenceScoreForMerging: NotRequired[float],
```

1. See [:material-code-braces: ConsolidationTypeDef](./type_defs.md#consolidationtypedef) 
2. See [:material-code-braces: ConflictResolutionTypeDef](./type_defs.md#conflictresolutiontypedef) 
## EventStreamSummaryTypeDef

```python
# EventStreamSummaryTypeDef definition

class EventStreamSummaryTypeDef(TypedDict):
    DomainName: str,
    EventStreamName: str,
    EventStreamArn: str,
    State: EventStreamStateType,  # (1)
    StoppedSince: NotRequired[datetime],
    DestinationSummary: NotRequired[DestinationSummaryTypeDef],  # (2)
    Tags: NotRequired[Dict[str, str]],
```

1. See [:material-code-brackets: EventStreamStateType](./literals.md#eventstreamstatetype) 
2. See [:material-code-braces: DestinationSummaryTypeDef](./type_defs.md#destinationsummarytypedef) 
## DetectedProfileObjectTypeTypeDef

```python
# DetectedProfileObjectTypeTypeDef definition

class DetectedProfileObjectTypeTypeDef(TypedDict):
    SourceLastUpdatedTimestampFormat: NotRequired[str],
    Fields: NotRequired[Dict[str, ObjectTypeFieldTypeDef]],  # (1)
    Keys: NotRequired[Dict[str, List[ObjectTypeKeyOutputTypeDef]]],  # (2)
```

1. See [:material-code-braces: ObjectTypeFieldTypeDef](./type_defs.md#objecttypefieldtypedef) 
2. See [:material-code-braces: ObjectTypeKeyOutputTypeDef](./type_defs.md#objecttypekeyoutputtypedef) 
## GetProfileObjectTypeResponseTypeDef

```python
# GetProfileObjectTypeResponseTypeDef definition

class GetProfileObjectTypeResponseTypeDef(TypedDict):
    ObjectTypeName: str,
    Description: str,
    TemplateId: str,
    ExpirationDays: int,
    EncryptionKey: str,
    AllowProfileCreation: bool,
    SourceLastUpdatedTimestampFormat: str,
    MaxAvailableProfileObjectCount: int,
    MaxProfileObjectCount: int,
    Fields: Dict[str, ObjectTypeFieldTypeDef],  # (1)
    Keys: Dict[str, List[ObjectTypeKeyOutputTypeDef]],  # (2)
    CreatedAt: datetime,
    LastUpdatedAt: datetime,
    Tags: Dict[str, str],
    ResponseMetadata: ResponseMetadataTypeDef,  # (3)
```

1. See [:material-code-braces: ObjectTypeFieldTypeDef](./type_defs.md#objecttypefieldtypedef) 
2. See [:material-code-braces: ObjectTypeKeyOutputTypeDef](./type_defs.md#objecttypekeyoutputtypedef) 
3. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetProfileObjectTypeTemplateResponseTypeDef

```python
# GetProfileObjectTypeTemplateResponseTypeDef definition

class GetProfileObjectTypeTemplateResponseTypeDef(TypedDict):
    TemplateId: str,
    SourceName: str,
    SourceObject: str,
    AllowProfileCreation: bool,
    SourceLastUpdatedTimestampFormat: str,
    Fields: Dict[str, ObjectTypeFieldTypeDef],  # (1)
    Keys: Dict[str, List[ObjectTypeKeyOutputTypeDef]],  # (2)
    ResponseMetadata: ResponseMetadataTypeDef,  # (3)
```

1. See [:material-code-braces: ObjectTypeFieldTypeDef](./type_defs.md#objecttypefieldtypedef) 
2. See [:material-code-braces: ObjectTypeKeyOutputTypeDef](./type_defs.md#objecttypekeyoutputtypedef) 
3. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## PutProfileObjectTypeResponseTypeDef

```python
# PutProfileObjectTypeResponseTypeDef definition

class PutProfileObjectTypeResponseTypeDef(TypedDict):
    ObjectTypeName: str,
    Description: str,
    TemplateId: str,
    ExpirationDays: int,
    EncryptionKey: str,
    AllowProfileCreation: bool,
    SourceLastUpdatedTimestampFormat: str,
    MaxProfileObjectCount: int,
    MaxAvailableProfileObjectCount: int,
    Fields: Dict[str, ObjectTypeFieldTypeDef],  # (1)
    Keys: Dict[str, List[ObjectTypeKeyOutputTypeDef]],  # (2)
    CreatedAt: datetime,
    LastUpdatedAt: datetime,
    Tags: Dict[str, str],
    ResponseMetadata: ResponseMetadataTypeDef,  # (3)
```

1. See [:material-code-braces: ObjectTypeFieldTypeDef](./type_defs.md#objecttypefieldtypedef) 
2. See [:material-code-braces: ObjectTypeKeyOutputTypeDef](./type_defs.md#objecttypekeyoutputtypedef) 
3. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetEventStreamResponseTypeDef

```python
# GetEventStreamResponseTypeDef definition

class GetEventStreamResponseTypeDef(TypedDict):
    DomainName: str,
    EventStreamArn: str,
    CreatedAt: datetime,
    State: EventStreamStateType,  # (1)
    StoppedSince: datetime,
    DestinationDetails: EventStreamDestinationDetailsTypeDef,  # (2)
    Tags: Dict[str, str],
    ResponseMetadata: ResponseMetadataTypeDef,  # (3)
```

1. See [:material-code-brackets: EventStreamStateType](./literals.md#eventstreamstatetype) 
2. See [:material-code-braces: EventStreamDestinationDetailsTypeDef](./type_defs.md#eventstreamdestinationdetailstypedef) 
3. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ExportingConfigTypeDef

```python
# ExportingConfigTypeDef definition

class ExportingConfigTypeDef(TypedDict):
    S3Exporting: NotRequired[S3ExportingConfigTypeDef],  # (1)
```

1. See [:material-code-braces: S3ExportingConfigTypeDef](./type_defs.md#s3exportingconfigtypedef) 
## ExportingLocationTypeDef

```python
# ExportingLocationTypeDef definition

class ExportingLocationTypeDef(TypedDict):
    S3Exporting: NotRequired[S3ExportingLocationTypeDef],  # (1)
```

1. See [:material-code-braces: S3ExportingLocationTypeDef](./type_defs.md#s3exportinglocationtypedef) 
## MergeProfilesRequestRequestTypeDef

```python
# MergeProfilesRequestRequestTypeDef definition

class MergeProfilesRequestRequestTypeDef(TypedDict):
    DomainName: str,
    MainProfileId: str,
    ProfileIdsToBeMerged: Sequence[str],
    FieldSourceProfileIds: NotRequired[FieldSourceProfileIdsTypeDef],  # (1)
```

1. See [:material-code-braces: FieldSourceProfileIdsTypeDef](./type_defs.md#fieldsourceprofileidstypedef) 
## ProfileTypeDef

```python
# ProfileTypeDef definition

class ProfileTypeDef(TypedDict):
    ProfileId: NotRequired[str],
    AccountNumber: NotRequired[str],
    AdditionalInformation: NotRequired[str],
    PartyType: NotRequired[PartyTypeType],  # (1)
    BusinessName: NotRequired[str],
    FirstName: NotRequired[str],
    MiddleName: NotRequired[str],
    LastName: NotRequired[str],
    BirthDate: NotRequired[str],
    Gender: NotRequired[GenderType],  # (2)
    PhoneNumber: NotRequired[str],
    MobilePhoneNumber: NotRequired[str],
    HomePhoneNumber: NotRequired[str],
    BusinessPhoneNumber: NotRequired[str],
    EmailAddress: NotRequired[str],
    PersonalEmailAddress: NotRequired[str],
    BusinessEmailAddress: NotRequired[str],
    Address: NotRequired[AddressTypeDef],  # (3)
    ShippingAddress: NotRequired[AddressTypeDef],  # (3)
    MailingAddress: NotRequired[AddressTypeDef],  # (3)
    BillingAddress: NotRequired[AddressTypeDef],  # (3)
    Attributes: NotRequired[Dict[str, str]],
    FoundByItems: NotRequired[List[FoundByKeyValueTypeDef]],  # (7)
    PartyTypeString: NotRequired[str],
    GenderString: NotRequired[str],
```

1. See [:material-code-brackets: PartyTypeType](./literals.md#partytypetype) 
2. See [:material-code-brackets: GenderType](./literals.md#gendertype) 
3. See [:material-code-braces: AddressTypeDef](./type_defs.md#addresstypedef) 
4. See [:material-code-braces: AddressTypeDef](./type_defs.md#addresstypedef) 
5. See [:material-code-braces: AddressTypeDef](./type_defs.md#addresstypedef) 
6. See [:material-code-braces: AddressTypeDef](./type_defs.md#addresstypedef) 
7. See [:material-code-braces: FoundByKeyValueTypeDef](./type_defs.md#foundbykeyvaluetypedef) 
## GetMatchesResponseTypeDef

```python
# GetMatchesResponseTypeDef definition

class GetMatchesResponseTypeDef(TypedDict):
    MatchGenerationDate: datetime,
    PotentialMatches: int,
    Matches: List[MatchItemTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: MatchItemTypeDef](./type_defs.md#matchitemtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListAccountIntegrationsResponseTypeDef

```python
# ListAccountIntegrationsResponseTypeDef definition

class ListAccountIntegrationsResponseTypeDef(TypedDict):
    Items: List[ListIntegrationItemTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: ListIntegrationItemTypeDef](./type_defs.md#listintegrationitemtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListIntegrationsResponseTypeDef

```python
# ListIntegrationsResponseTypeDef definition

class ListIntegrationsResponseTypeDef(TypedDict):
    Items: List[ListIntegrationItemTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: ListIntegrationItemTypeDef](./type_defs.md#listintegrationitemtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListCalculatedAttributeDefinitionsResponseTypeDef

```python
# ListCalculatedAttributeDefinitionsResponseTypeDef definition

class ListCalculatedAttributeDefinitionsResponseTypeDef(TypedDict):
    Items: List[ListCalculatedAttributeDefinitionItemTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: ListCalculatedAttributeDefinitionItemTypeDef](./type_defs.md#listcalculatedattributedefinitionitemtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListCalculatedAttributesForProfileResponseTypeDef

```python
# ListCalculatedAttributesForProfileResponseTypeDef definition

class ListCalculatedAttributesForProfileResponseTypeDef(TypedDict):
    Items: List[ListCalculatedAttributeForProfileItemTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: ListCalculatedAttributeForProfileItemTypeDef](./type_defs.md#listcalculatedattributeforprofileitemtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListDomainsResponseTypeDef

```python
# ListDomainsResponseTypeDef definition

class ListDomainsResponseTypeDef(TypedDict):
    Items: List[ListDomainItemTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: ListDomainItemTypeDef](./type_defs.md#listdomainitemtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListEventStreamsRequestListEventStreamsPaginateTypeDef

```python
# ListEventStreamsRequestListEventStreamsPaginateTypeDef definition

class ListEventStreamsRequestListEventStreamsPaginateTypeDef(TypedDict):
    DomainName: str,
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListProfileObjectTypesResponseTypeDef

```python
# ListProfileObjectTypesResponseTypeDef definition

class ListProfileObjectTypesResponseTypeDef(TypedDict):
    Items: List[ListProfileObjectTypeItemTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: ListProfileObjectTypeItemTypeDef](./type_defs.md#listprofileobjecttypeitemtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListProfileObjectTypeTemplatesResponseTypeDef

```python
# ListProfileObjectTypeTemplatesResponseTypeDef definition

class ListProfileObjectTypeTemplatesResponseTypeDef(TypedDict):
    Items: List[ListProfileObjectTypeTemplateItemTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: ListProfileObjectTypeTemplateItemTypeDef](./type_defs.md#listprofileobjecttypetemplateitemtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListProfileObjectsResponseTypeDef

```python
# ListProfileObjectsResponseTypeDef definition

class ListProfileObjectsResponseTypeDef(TypedDict):
    Items: List[ListProfileObjectsItemTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: ListProfileObjectsItemTypeDef](./type_defs.md#listprofileobjectsitemtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListProfileObjectsRequestRequestTypeDef

```python
# ListProfileObjectsRequestRequestTypeDef definition

class ListProfileObjectsRequestRequestTypeDef(TypedDict):
    DomainName: str,
    ObjectTypeName: str,
    ProfileId: str,
    NextToken: NotRequired[str],
    MaxResults: NotRequired[int],
    ObjectFilter: NotRequired[ObjectFilterTypeDef],  # (1)
```

1. See [:material-code-braces: ObjectFilterTypeDef](./type_defs.md#objectfiltertypedef) 
## ListWorkflowsResponseTypeDef

```python
# ListWorkflowsResponseTypeDef definition

class ListWorkflowsResponseTypeDef(TypedDict):
    Items: List[ListWorkflowsItemTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: ListWorkflowsItemTypeDef](./type_defs.md#listworkflowsitemtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## SourceConnectorPropertiesTypeDef

```python
# SourceConnectorPropertiesTypeDef definition

class SourceConnectorPropertiesTypeDef(TypedDict):
    Marketo: NotRequired[MarketoSourcePropertiesTypeDef],  # (1)
    S3: NotRequired[S3SourcePropertiesTypeDef],  # (2)
    Salesforce: NotRequired[SalesforceSourcePropertiesTypeDef],  # (3)
    ServiceNow: NotRequired[ServiceNowSourcePropertiesTypeDef],  # (4)
    Zendesk: NotRequired[ZendeskSourcePropertiesTypeDef],  # (5)
```

1. See [:material-code-braces: MarketoSourcePropertiesTypeDef](./type_defs.md#marketosourcepropertiestypedef) 
2. See [:material-code-braces: S3SourcePropertiesTypeDef](./type_defs.md#s3sourcepropertiestypedef) 
3. See [:material-code-braces: SalesforceSourcePropertiesTypeDef](./type_defs.md#salesforcesourcepropertiestypedef) 
4. See [:material-code-braces: ServiceNowSourcePropertiesTypeDef](./type_defs.md#servicenowsourcepropertiestypedef) 
5. See [:material-code-braces: ZendeskSourcePropertiesTypeDef](./type_defs.md#zendesksourcepropertiestypedef) 
## UpdateProfileRequestRequestTypeDef

```python
# UpdateProfileRequestRequestTypeDef definition

class UpdateProfileRequestRequestTypeDef(TypedDict):
    DomainName: str,
    ProfileId: str,
    AdditionalInformation: NotRequired[str],
    AccountNumber: NotRequired[str],
    PartyType: NotRequired[PartyTypeType],  # (1)
    BusinessName: NotRequired[str],
    FirstName: NotRequired[str],
    MiddleName: NotRequired[str],
    LastName: NotRequired[str],
    BirthDate: NotRequired[str],
    Gender: NotRequired[GenderType],  # (2)
    PhoneNumber: NotRequired[str],
    MobilePhoneNumber: NotRequired[str],
    HomePhoneNumber: NotRequired[str],
    BusinessPhoneNumber: NotRequired[str],
    EmailAddress: NotRequired[str],
    PersonalEmailAddress: NotRequired[str],
    BusinessEmailAddress: NotRequired[str],
    Address: NotRequired[UpdateAddressTypeDef],  # (3)
    ShippingAddress: NotRequired[UpdateAddressTypeDef],  # (3)
    MailingAddress: NotRequired[UpdateAddressTypeDef],  # (3)
    BillingAddress: NotRequired[UpdateAddressTypeDef],  # (3)
    Attributes: NotRequired[Mapping[str, str]],
    PartyTypeString: NotRequired[str],
    GenderString: NotRequired[str],
```

1. See [:material-code-brackets: PartyTypeType](./literals.md#partytypetype) 
2. See [:material-code-brackets: GenderType](./literals.md#gendertype) 
3. See [:material-code-braces: UpdateAddressTypeDef](./type_defs.md#updateaddresstypedef) 
4. See [:material-code-braces: UpdateAddressTypeDef](./type_defs.md#updateaddresstypedef) 
5. See [:material-code-braces: UpdateAddressTypeDef](./type_defs.md#updateaddresstypedef) 
6. See [:material-code-braces: UpdateAddressTypeDef](./type_defs.md#updateaddresstypedef) 
## GetWorkflowResponseTypeDef

```python
# GetWorkflowResponseTypeDef definition

class GetWorkflowResponseTypeDef(TypedDict):
    WorkflowId: str,
    WorkflowType: WorkflowTypeType,  # (1)
    Status: StatusType,  # (2)
    ErrorDescription: str,
    StartDate: datetime,
    LastUpdatedAt: datetime,
    Attributes: WorkflowAttributesTypeDef,  # (3)
    Metrics: WorkflowMetricsTypeDef,  # (4)
    ResponseMetadata: ResponseMetadataTypeDef,  # (5)
```

1. See [:material-code-brackets: WorkflowTypeType](./literals.md#workflowtypetype) 
2. See [:material-code-brackets: StatusType](./literals.md#statustype) 
3. See [:material-code-braces: WorkflowAttributesTypeDef](./type_defs.md#workflowattributestypedef) 
4. See [:material-code-braces: WorkflowMetricsTypeDef](./type_defs.md#workflowmetricstypedef) 
5. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetWorkflowStepsResponseTypeDef

```python
# GetWorkflowStepsResponseTypeDef definition

class GetWorkflowStepsResponseTypeDef(TypedDict):
    WorkflowId: str,
    WorkflowType: WorkflowTypeType,  # (1)
    Items: List[WorkflowStepItemTypeDef],  # (2)
    ResponseMetadata: ResponseMetadataTypeDef,  # (3)
    NextToken: NotRequired[str],
```

1. See [:material-code-brackets: WorkflowTypeType](./literals.md#workflowtypetype) 
2. See [:material-code-braces: WorkflowStepItemTypeDef](./type_defs.md#workflowstepitemtypedef) 
3. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## TriggerPropertiesTypeDef

```python
# TriggerPropertiesTypeDef definition

class TriggerPropertiesTypeDef(TypedDict):
    Scheduled: NotRequired[ScheduledTriggerPropertiesTypeDef],  # (1)
```

1. See [:material-code-braces: ScheduledTriggerPropertiesTypeDef](./type_defs.md#scheduledtriggerpropertiestypedef) 
## CreateCalculatedAttributeDefinitionRequestRequestTypeDef

```python
# CreateCalculatedAttributeDefinitionRequestRequestTypeDef definition

class CreateCalculatedAttributeDefinitionRequestRequestTypeDef(TypedDict):
    DomainName: str,
    CalculatedAttributeName: str,
    AttributeDetails: AttributeDetailsTypeDef,  # (1)
    Statistic: StatisticType,  # (2)
    DisplayName: NotRequired[str],
    Description: NotRequired[str],
    Conditions: NotRequired[ConditionsTypeDef],  # (3)
    Tags: NotRequired[Mapping[str, str]],
```

1. See [:material-code-braces: AttributeDetailsTypeDef](./type_defs.md#attributedetailstypedef) 
2. See [:material-code-brackets: StatisticType](./literals.md#statistictype) 
3. See [:material-code-braces: ConditionsTypeDef](./type_defs.md#conditionstypedef) 
## CreateCalculatedAttributeDefinitionResponseTypeDef

```python
# CreateCalculatedAttributeDefinitionResponseTypeDef definition

class CreateCalculatedAttributeDefinitionResponseTypeDef(TypedDict):
    CalculatedAttributeName: str,
    DisplayName: str,
    Description: str,
    AttributeDetails: AttributeDetailsOutputTypeDef,  # (1)
    Conditions: ConditionsTypeDef,  # (2)
    Statistic: StatisticType,  # (3)
    CreatedAt: datetime,
    LastUpdatedAt: datetime,
    Tags: Dict[str, str],
    ResponseMetadata: ResponseMetadataTypeDef,  # (4)
```

1. See [:material-code-braces: AttributeDetailsOutputTypeDef](./type_defs.md#attributedetailsoutputtypedef) 
2. See [:material-code-braces: ConditionsTypeDef](./type_defs.md#conditionstypedef) 
3. See [:material-code-brackets: StatisticType](./literals.md#statistictype) 
4. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetCalculatedAttributeDefinitionResponseTypeDef

```python
# GetCalculatedAttributeDefinitionResponseTypeDef definition

class GetCalculatedAttributeDefinitionResponseTypeDef(TypedDict):
    CalculatedAttributeName: str,
    DisplayName: str,
    Description: str,
    CreatedAt: datetime,
    LastUpdatedAt: datetime,
    Statistic: StatisticType,  # (1)
    Conditions: ConditionsTypeDef,  # (2)
    AttributeDetails: AttributeDetailsOutputTypeDef,  # (3)
    Tags: Dict[str, str],
    ResponseMetadata: ResponseMetadataTypeDef,  # (4)
```

1. See [:material-code-brackets: StatisticType](./literals.md#statistictype) 
2. See [:material-code-braces: ConditionsTypeDef](./type_defs.md#conditionstypedef) 
3. See [:material-code-braces: AttributeDetailsOutputTypeDef](./type_defs.md#attributedetailsoutputtypedef) 
4. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdateCalculatedAttributeDefinitionRequestRequestTypeDef

```python
# UpdateCalculatedAttributeDefinitionRequestRequestTypeDef definition

class UpdateCalculatedAttributeDefinitionRequestRequestTypeDef(TypedDict):
    DomainName: str,
    CalculatedAttributeName: str,
    DisplayName: NotRequired[str],
    Description: NotRequired[str],
    Conditions: NotRequired[ConditionsTypeDef],  # (1)
```

1. See [:material-code-braces: ConditionsTypeDef](./type_defs.md#conditionstypedef) 
## UpdateCalculatedAttributeDefinitionResponseTypeDef

```python
# UpdateCalculatedAttributeDefinitionResponseTypeDef definition

class UpdateCalculatedAttributeDefinitionResponseTypeDef(TypedDict):
    CalculatedAttributeName: str,
    DisplayName: str,
    Description: str,
    CreatedAt: datetime,
    LastUpdatedAt: datetime,
    Statistic: StatisticType,  # (1)
    Conditions: ConditionsTypeDef,  # (2)
    AttributeDetails: AttributeDetailsOutputTypeDef,  # (3)
    Tags: Dict[str, str],
    ResponseMetadata: ResponseMetadataTypeDef,  # (4)
```

1. See [:material-code-brackets: StatisticType](./literals.md#statistictype) 
2. See [:material-code-braces: ConditionsTypeDef](./type_defs.md#conditionstypedef) 
3. See [:material-code-braces: AttributeDetailsOutputTypeDef](./type_defs.md#attributedetailsoutputtypedef) 
4. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## AutoMergingTypeDef

```python
# AutoMergingTypeDef definition

class AutoMergingTypeDef(TypedDict):
    Enabled: bool,
    Consolidation: NotRequired[ConsolidationUnionTypeDef],  # (1)
    ConflictResolution: NotRequired[ConflictResolutionTypeDef],  # (2)
    MinAllowedConfidenceScoreForMerging: NotRequired[float],
```

1. See [:material-code-braces: ConsolidationTypeDef](./type_defs.md#consolidationtypedef) [:material-code-braces: ConsolidationOutputTypeDef](./type_defs.md#consolidationoutputtypedef) 
2. See [:material-code-braces: ConflictResolutionTypeDef](./type_defs.md#conflictresolutiontypedef) 
## ListEventStreamsResponseTypeDef

```python
# ListEventStreamsResponseTypeDef definition

class ListEventStreamsResponseTypeDef(TypedDict):
    Items: List[EventStreamSummaryTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: EventStreamSummaryTypeDef](./type_defs.md#eventstreamsummarytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DetectProfileObjectTypeResponseTypeDef

```python
# DetectProfileObjectTypeResponseTypeDef definition

class DetectProfileObjectTypeResponseTypeDef(TypedDict):
    DetectedProfileObjectTypes: List[DetectedProfileObjectTypeTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: DetectedProfileObjectTypeTypeDef](./type_defs.md#detectedprofileobjecttypetypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## MatchingResponseTypeDef

```python
# MatchingResponseTypeDef definition

class MatchingResponseTypeDef(TypedDict):
    Enabled: NotRequired[bool],
    JobSchedule: NotRequired[JobScheduleTypeDef],  # (1)
    AutoMerging: NotRequired[AutoMergingOutputTypeDef],  # (2)
    ExportingConfig: NotRequired[ExportingConfigTypeDef],  # (3)
```

1. See [:material-code-braces: JobScheduleTypeDef](./type_defs.md#jobscheduletypedef) 
2. See [:material-code-braces: AutoMergingOutputTypeDef](./type_defs.md#automergingoutputtypedef) 
3. See [:material-code-braces: ExportingConfigTypeDef](./type_defs.md#exportingconfigtypedef) 
## RuleBasedMatchingResponseTypeDef

```python
# RuleBasedMatchingResponseTypeDef definition

class RuleBasedMatchingResponseTypeDef(TypedDict):
    Enabled: NotRequired[bool],
    MatchingRules: NotRequired[List[MatchingRuleOutputTypeDef]],  # (1)
    Status: NotRequired[RuleBasedMatchingStatusType],  # (2)
    MaxAllowedRuleLevelForMerging: NotRequired[int],
    MaxAllowedRuleLevelForMatching: NotRequired[int],
    AttributeTypesSelector: NotRequired[AttributeTypesSelectorOutputTypeDef],  # (3)
    ConflictResolution: NotRequired[ConflictResolutionTypeDef],  # (4)
    ExportingConfig: NotRequired[ExportingConfigTypeDef],  # (5)
```

1. See [:material-code-braces: MatchingRuleOutputTypeDef](./type_defs.md#matchingruleoutputtypedef) 
2. See [:material-code-brackets: RuleBasedMatchingStatusType](./literals.md#rulebasedmatchingstatustype) 
3. See [:material-code-braces: AttributeTypesSelectorOutputTypeDef](./type_defs.md#attributetypesselectoroutputtypedef) 
4. See [:material-code-braces: ConflictResolutionTypeDef](./type_defs.md#conflictresolutiontypedef) 
5. See [:material-code-braces: ExportingConfigTypeDef](./type_defs.md#exportingconfigtypedef) 
## GetIdentityResolutionJobResponseTypeDef

```python
# GetIdentityResolutionJobResponseTypeDef definition

class GetIdentityResolutionJobResponseTypeDef(TypedDict):
    DomainName: str,
    JobId: str,
    Status: IdentityResolutionJobStatusType,  # (1)
    Message: str,
    JobStartTime: datetime,
    JobEndTime: datetime,
    LastUpdatedAt: datetime,
    JobExpirationTime: datetime,
    AutoMerging: AutoMergingOutputTypeDef,  # (2)
    ExportingLocation: ExportingLocationTypeDef,  # (3)
    JobStats: JobStatsTypeDef,  # (4)
    ResponseMetadata: ResponseMetadataTypeDef,  # (5)
```

1. See [:material-code-brackets: IdentityResolutionJobStatusType](./literals.md#identityresolutionjobstatustype) 
2. See [:material-code-braces: AutoMergingOutputTypeDef](./type_defs.md#automergingoutputtypedef) 
3. See [:material-code-braces: ExportingLocationTypeDef](./type_defs.md#exportinglocationtypedef) 
4. See [:material-code-braces: JobStatsTypeDef](./type_defs.md#jobstatstypedef) 
5. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## IdentityResolutionJobTypeDef

```python
# IdentityResolutionJobTypeDef definition

class IdentityResolutionJobTypeDef(TypedDict):
    DomainName: NotRequired[str],
    JobId: NotRequired[str],
    Status: NotRequired[IdentityResolutionJobStatusType],  # (1)
    JobStartTime: NotRequired[datetime],
    JobEndTime: NotRequired[datetime],
    JobStats: NotRequired[JobStatsTypeDef],  # (2)
    ExportingLocation: NotRequired[ExportingLocationTypeDef],  # (3)
    Message: NotRequired[str],
```

1. See [:material-code-brackets: IdentityResolutionJobStatusType](./literals.md#identityresolutionjobstatustype) 
2. See [:material-code-braces: JobStatsTypeDef](./type_defs.md#jobstatstypedef) 
3. See [:material-code-braces: ExportingLocationTypeDef](./type_defs.md#exportinglocationtypedef) 
## SearchProfilesResponseTypeDef

```python
# SearchProfilesResponseTypeDef definition

class SearchProfilesResponseTypeDef(TypedDict):
    Items: List[ProfileTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: ProfileTypeDef](./type_defs.md#profiletypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## RuleBasedMatchingRequestTypeDef

```python
# RuleBasedMatchingRequestTypeDef definition

class RuleBasedMatchingRequestTypeDef(TypedDict):
    Enabled: bool,
    MatchingRules: NotRequired[Sequence[MatchingRuleUnionTypeDef]],  # (1)
    MaxAllowedRuleLevelForMerging: NotRequired[int],
    MaxAllowedRuleLevelForMatching: NotRequired[int],
    AttributeTypesSelector: NotRequired[AttributeTypesSelectorUnionTypeDef],  # (2)
    ConflictResolution: NotRequired[ConflictResolutionTypeDef],  # (3)
    ExportingConfig: NotRequired[ExportingConfigTypeDef],  # (4)
```

1. See [:material-code-braces: MatchingRuleTypeDef](./type_defs.md#matchingruletypedef) [:material-code-braces: MatchingRuleOutputTypeDef](./type_defs.md#matchingruleoutputtypedef) 
2. See [:material-code-braces: AttributeTypesSelectorTypeDef](./type_defs.md#attributetypesselectortypedef) [:material-code-braces: AttributeTypesSelectorOutputTypeDef](./type_defs.md#attributetypesselectoroutputtypedef) 
3. See [:material-code-braces: ConflictResolutionTypeDef](./type_defs.md#conflictresolutiontypedef) 
4. See [:material-code-braces: ExportingConfigTypeDef](./type_defs.md#exportingconfigtypedef) 
## PutProfileObjectTypeRequestRequestTypeDef

```python
# PutProfileObjectTypeRequestRequestTypeDef definition

class PutProfileObjectTypeRequestRequestTypeDef(TypedDict):
    DomainName: str,
    ObjectTypeName: str,
    Description: str,
    TemplateId: NotRequired[str],
    ExpirationDays: NotRequired[int],
    EncryptionKey: NotRequired[str],
    AllowProfileCreation: NotRequired[bool],
    SourceLastUpdatedTimestampFormat: NotRequired[str],
    MaxProfileObjectCount: NotRequired[int],
    Fields: NotRequired[Mapping[str, ObjectTypeFieldTypeDef]],  # (1)
    Keys: NotRequired[Mapping[str, Sequence[ObjectTypeKeyUnionTypeDef]]],  # (2)
    Tags: NotRequired[Mapping[str, str]],
```

1. See [:material-code-braces: ObjectTypeFieldTypeDef](./type_defs.md#objecttypefieldtypedef) 
2. See [:material-code-braces: ObjectTypeKeyTypeDef](./type_defs.md#objecttypekeytypedef) [:material-code-braces: ObjectTypeKeyOutputTypeDef](./type_defs.md#objecttypekeyoutputtypedef) 
## SourceFlowConfigTypeDef

```python
# SourceFlowConfigTypeDef definition

class SourceFlowConfigTypeDef(TypedDict):
    ConnectorType: SourceConnectorTypeType,  # (1)
    SourceConnectorProperties: SourceConnectorPropertiesTypeDef,  # (3)
    ConnectorProfileName: NotRequired[str],
    IncrementalPullConfig: NotRequired[IncrementalPullConfigTypeDef],  # (2)
```

1. See [:material-code-brackets: SourceConnectorTypeType](./literals.md#sourceconnectortypetype) 
2. See [:material-code-braces: IncrementalPullConfigTypeDef](./type_defs.md#incrementalpullconfigtypedef) 
3. See [:material-code-braces: SourceConnectorPropertiesTypeDef](./type_defs.md#sourceconnectorpropertiestypedef) 
## TriggerConfigTypeDef

```python
# TriggerConfigTypeDef definition

class TriggerConfigTypeDef(TypedDict):
    TriggerType: TriggerTypeType,  # (1)
    TriggerProperties: NotRequired[TriggerPropertiesTypeDef],  # (2)
```

1. See [:material-code-brackets: TriggerTypeType](./literals.md#triggertypetype) 
2. See [:material-code-braces: TriggerPropertiesTypeDef](./type_defs.md#triggerpropertiestypedef) 
## CreateDomainResponseTypeDef

```python
# CreateDomainResponseTypeDef definition

class CreateDomainResponseTypeDef(TypedDict):
    DomainName: str,
    DefaultExpirationDays: int,
    DefaultEncryptionKey: str,
    DeadLetterQueueUrl: str,
    Matching: MatchingResponseTypeDef,  # (1)
    RuleBasedMatching: RuleBasedMatchingResponseTypeDef,  # (2)
    CreatedAt: datetime,
    LastUpdatedAt: datetime,
    Tags: Dict[str, str],
    ResponseMetadata: ResponseMetadataTypeDef,  # (3)
```

1. See [:material-code-braces: MatchingResponseTypeDef](./type_defs.md#matchingresponsetypedef) 
2. See [:material-code-braces: RuleBasedMatchingResponseTypeDef](./type_defs.md#rulebasedmatchingresponsetypedef) 
3. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetDomainResponseTypeDef

```python
# GetDomainResponseTypeDef definition

class GetDomainResponseTypeDef(TypedDict):
    DomainName: str,
    DefaultExpirationDays: int,
    DefaultEncryptionKey: str,
    DeadLetterQueueUrl: str,
    Stats: DomainStatsTypeDef,  # (1)
    Matching: MatchingResponseTypeDef,  # (2)
    RuleBasedMatching: RuleBasedMatchingResponseTypeDef,  # (3)
    CreatedAt: datetime,
    LastUpdatedAt: datetime,
    Tags: Dict[str, str],
    ResponseMetadata: ResponseMetadataTypeDef,  # (4)
```

1. See [:material-code-braces: DomainStatsTypeDef](./type_defs.md#domainstatstypedef) 
2. See [:material-code-braces: MatchingResponseTypeDef](./type_defs.md#matchingresponsetypedef) 
3. See [:material-code-braces: RuleBasedMatchingResponseTypeDef](./type_defs.md#rulebasedmatchingresponsetypedef) 
4. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdateDomainResponseTypeDef

```python
# UpdateDomainResponseTypeDef definition

class UpdateDomainResponseTypeDef(TypedDict):
    DomainName: str,
    DefaultExpirationDays: int,
    DefaultEncryptionKey: str,
    DeadLetterQueueUrl: str,
    Matching: MatchingResponseTypeDef,  # (1)
    RuleBasedMatching: RuleBasedMatchingResponseTypeDef,  # (2)
    CreatedAt: datetime,
    LastUpdatedAt: datetime,
    Tags: Dict[str, str],
    ResponseMetadata: ResponseMetadataTypeDef,  # (3)
```

1. See [:material-code-braces: MatchingResponseTypeDef](./type_defs.md#matchingresponsetypedef) 
2. See [:material-code-braces: RuleBasedMatchingResponseTypeDef](./type_defs.md#rulebasedmatchingresponsetypedef) 
3. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListIdentityResolutionJobsResponseTypeDef

```python
# ListIdentityResolutionJobsResponseTypeDef definition

class ListIdentityResolutionJobsResponseTypeDef(TypedDict):
    IdentityResolutionJobsList: List[IdentityResolutionJobTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: IdentityResolutionJobTypeDef](./type_defs.md#identityresolutionjobtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## FlowDefinitionTypeDef

```python
# FlowDefinitionTypeDef definition

class FlowDefinitionTypeDef(TypedDict):
    FlowName: str,
    KmsArn: str,
    SourceFlowConfig: SourceFlowConfigTypeDef,  # (1)
    Tasks: Sequence[TaskTypeDef],  # (2)
    TriggerConfig: TriggerConfigTypeDef,  # (3)
    Description: NotRequired[str],
```

1. See [:material-code-braces: SourceFlowConfigTypeDef](./type_defs.md#sourceflowconfigtypedef) 
2. See [:material-code-braces: TaskTypeDef](./type_defs.md#tasktypedef) 
3. See [:material-code-braces: TriggerConfigTypeDef](./type_defs.md#triggerconfigtypedef) 
## MatchingRequestTypeDef

```python
# MatchingRequestTypeDef definition

class MatchingRequestTypeDef(TypedDict):
    Enabled: bool,
    JobSchedule: NotRequired[JobScheduleTypeDef],  # (1)
    AutoMerging: NotRequired[AutoMergingUnionTypeDef],  # (2)
    ExportingConfig: NotRequired[ExportingConfigTypeDef],  # (3)
```

1. See [:material-code-braces: JobScheduleTypeDef](./type_defs.md#jobscheduletypedef) 
2. See [:material-code-braces: AutoMergingTypeDef](./type_defs.md#automergingtypedef) [:material-code-braces: AutoMergingOutputTypeDef](./type_defs.md#automergingoutputtypedef) 
3. See [:material-code-braces: ExportingConfigTypeDef](./type_defs.md#exportingconfigtypedef) 
## AppflowIntegrationTypeDef

```python
# AppflowIntegrationTypeDef definition

class AppflowIntegrationTypeDef(TypedDict):
    FlowDefinition: FlowDefinitionTypeDef,  # (1)
    Batches: NotRequired[Sequence[BatchTypeDef]],  # (2)
```

1. See [:material-code-braces: FlowDefinitionTypeDef](./type_defs.md#flowdefinitiontypedef) 
2. See [:material-code-braces: BatchTypeDef](./type_defs.md#batchtypedef) 
## PutIntegrationRequestRequestTypeDef

```python
# PutIntegrationRequestRequestTypeDef definition

class PutIntegrationRequestRequestTypeDef(TypedDict):
    DomainName: str,
    Uri: NotRequired[str],
    ObjectTypeName: NotRequired[str],
    Tags: NotRequired[Mapping[str, str]],
    FlowDefinition: NotRequired[FlowDefinitionTypeDef],  # (1)
    ObjectTypeNames: NotRequired[Mapping[str, str]],
    RoleArn: NotRequired[str],
```

1. See [:material-code-braces: FlowDefinitionTypeDef](./type_defs.md#flowdefinitiontypedef) 
## CreateDomainRequestRequestTypeDef

```python
# CreateDomainRequestRequestTypeDef definition

class CreateDomainRequestRequestTypeDef(TypedDict):
    DomainName: str,
    DefaultExpirationDays: int,
    DefaultEncryptionKey: NotRequired[str],
    DeadLetterQueueUrl: NotRequired[str],
    Matching: NotRequired[MatchingRequestTypeDef],  # (1)
    RuleBasedMatching: NotRequired[RuleBasedMatchingRequestTypeDef],  # (2)
    Tags: NotRequired[Mapping[str, str]],
```

1. See [:material-code-braces: MatchingRequestTypeDef](./type_defs.md#matchingrequesttypedef) 
2. See [:material-code-braces: RuleBasedMatchingRequestTypeDef](./type_defs.md#rulebasedmatchingrequesttypedef) 
## UpdateDomainRequestRequestTypeDef

```python
# UpdateDomainRequestRequestTypeDef definition

class UpdateDomainRequestRequestTypeDef(TypedDict):
    DomainName: str,
    DefaultExpirationDays: NotRequired[int],
    DefaultEncryptionKey: NotRequired[str],
    DeadLetterQueueUrl: NotRequired[str],
    Matching: NotRequired[MatchingRequestTypeDef],  # (1)
    RuleBasedMatching: NotRequired[RuleBasedMatchingRequestTypeDef],  # (2)
    Tags: NotRequired[Mapping[str, str]],
```

1. See [:material-code-braces: MatchingRequestTypeDef](./type_defs.md#matchingrequesttypedef) 
2. See [:material-code-braces: RuleBasedMatchingRequestTypeDef](./type_defs.md#rulebasedmatchingrequesttypedef) 
## IntegrationConfigTypeDef

```python
# IntegrationConfigTypeDef definition

class IntegrationConfigTypeDef(TypedDict):
    AppflowIntegration: NotRequired[AppflowIntegrationTypeDef],  # (1)
```

1. See [:material-code-braces: AppflowIntegrationTypeDef](./type_defs.md#appflowintegrationtypedef) 
## CreateIntegrationWorkflowRequestRequestTypeDef

```python
# CreateIntegrationWorkflowRequestRequestTypeDef definition

class CreateIntegrationWorkflowRequestRequestTypeDef(TypedDict):
    DomainName: str,
    WorkflowType: WorkflowTypeType,  # (1)
    IntegrationConfig: IntegrationConfigTypeDef,  # (2)
    ObjectTypeName: str,
    RoleArn: str,
    Tags: NotRequired[Mapping[str, str]],
```

1. See [:material-code-brackets: WorkflowTypeType](./literals.md#workflowtypetype) 
2. See [:material-code-braces: IntegrationConfigTypeDef](./type_defs.md#integrationconfigtypedef) 
