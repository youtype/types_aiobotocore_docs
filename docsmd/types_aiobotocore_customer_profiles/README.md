# CustomerProfiles module

> [Index](../README.md) > CustomerProfiles


!!! note ""

    Auto-generated documentation for [CustomerProfiles](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/customer-profiles.html#customerprofiles)
    type annotations stubs module [types-aiobotocore-customer-profiles](https://pypi.org/project/types-aiobotocore-customer-profiles/).

## How to install

### Generate locally (recommended)

You can generate type annotations for `aiobotocore` package locally with `mypy_boto3_builder`.
Use [uv](https://docs.astral.sh/uv/getting-started/installation/) for build isolation.

1. Run mypy-boto3-builder in your package root directory: `uvx --with 'aiobotocore==2.16.0' mypy_boto3_builder`
1. Select `aiobotocore` AWS SDK.
1. Add `CustomerProfiles` service.
1. Use provided commands to install generated packages.



### From PyPI with pip

Install `types-aiobotocore` for `CustomerProfiles` service.

```bash
# install with aiobotocore type annotations
python -m pip install 'types-aiobotocore[customer-profiles]'

# Lite version does not provide session.client/resource overloads
# it is more RAM-friendly, but requires explicit type annotations
python -m pip install 'types-aiobotocore-lite[customer-profiles]'

# standalone installation
python -m pip install types-aiobotocore-customer-profiles
```



## How to uninstall

```bash
python -m pip uninstall -y types-aiobotocore-customer-profiles
```

## Usage

Code samples can be found in [Examples](./usage.md).

## CustomerProfilesClient

Type annotations and code completion for  `#!python session.create_client("customer-profiles")` as [CustomerProfilesClient](./client.md)
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/customer-profiles.html#CustomerProfiles.Client)

```python
# CustomerProfilesClient usage example

from aiobotocore.session import get_session

from types_aiobotocore_customer_profiles.client import CustomerProfilesClient


session = get_session()
async with session.create_client("customer-profiles") as client:
    client: CustomerProfilesClient
```


## Paginators

Type annotations and code completion for
[paginators](./paginators.md)
from `#!python session.create_client("customer-profiles").get_paginator("...")`.

```python
# GetSimilarProfilesPaginator usage example

from types_aiobotocore_customer_profiles.paginator import GetSimilarProfilesPaginator

def get_get_similar_profiles_paginator() -> GetSimilarProfilesPaginator:
    return client.get_paginator("get_similar_profiles"))
```

- [GetSimilarProfilesPaginator](./paginators.md#getsimilarprofilespaginator)
- [ListEventStreamsPaginator](./paginators.md#listeventstreamspaginator)
- [ListEventTriggersPaginator](./paginators.md#listeventtriggerspaginator)
- [ListObjectTypeAttributesPaginator](./paginators.md#listobjecttypeattributespaginator)
- [ListRuleBasedMatchesPaginator](./paginators.md#listrulebasedmatchespaginator)
- [ListSegmentDefinitionsPaginator](./paginators.md#listsegmentdefinitionspaginator)








## Literals

Type annotations for [literals](./literals.md) used in methods and schema.

```python
# AttributeDimensionTypeType usage example

from types_aiobotocore_customer_profiles.literals import AttributeDimensionTypeType

def get_value() -> AttributeDimensionTypeType:
    return "AFTER"
```

- [AttributeDimensionTypeType](./literals.md#attributedimensiontypetype)
- [AttributeMatchingModelType](./literals.md#attributematchingmodeltype)
- [ComparisonOperatorType](./literals.md#comparisonoperatortype)
- [ConflictResolvingModelType](./literals.md#conflictresolvingmodeltype)
- [DataFormatType](./literals.md#dataformattype)
- [DataPullModeType](./literals.md#datapullmodetype)
- [DateDimensionTypeType](./literals.md#datedimensiontypetype)
- [EstimateStatusType](./literals.md#estimatestatustype)
- [EventStreamDestinationStatusType](./literals.md#eventstreamdestinationstatustype)
- [EventStreamStateType](./literals.md#eventstreamstatetype)
- [EventTriggerLogicalOperatorType](./literals.md#eventtriggerlogicaloperatortype)
- [FieldContentTypeType](./literals.md#fieldcontenttypetype)
- [FilterDimensionTypeType](./literals.md#filterdimensiontypetype)
- [GenderType](./literals.md#gendertype)
- [GetSimilarProfilesPaginatorName](./literals.md#getsimilarprofilespaginatorname)
- [IdentityResolutionJobStatusType](./literals.md#identityresolutionjobstatustype)
- [IncludeOptionsType](./literals.md#includeoptionstype)
- [IncludeType](./literals.md#includetype)
- [JobScheduleDayOfTheWeekType](./literals.md#jobscheduledayoftheweektype)
- [ListEventStreamsPaginatorName](./literals.md#listeventstreamspaginatorname)
- [ListEventTriggersPaginatorName](./literals.md#listeventtriggerspaginatorname)
- [ListObjectTypeAttributesPaginatorName](./literals.md#listobjecttypeattributespaginatorname)
- [ListRuleBasedMatchesPaginatorName](./literals.md#listrulebasedmatchespaginatorname)
- [ListSegmentDefinitionsPaginatorName](./literals.md#listsegmentdefinitionspaginatorname)
- [LogicalOperatorType](./literals.md#logicaloperatortype)
- [MarketoConnectorOperatorType](./literals.md#marketoconnectoroperatortype)
- [MatchTypeType](./literals.md#matchtypetype)
- [OperatorPropertiesKeysType](./literals.md#operatorpropertieskeystype)
- [OperatorType](./literals.md#operatortype)
- [PartyTypeType](./literals.md#partytypetype)
- [PeriodUnitType](./literals.md#periodunittype)
- [QueryResultType](./literals.md#queryresulttype)
- [RangeUnitType](./literals.md#rangeunittype)
- [RuleBasedMatchingStatusType](./literals.md#rulebasedmatchingstatustype)
- [S3ConnectorOperatorType](./literals.md#s3connectoroperatortype)
- [SalesforceConnectorOperatorType](./literals.md#salesforceconnectoroperatortype)
- [SegmentSnapshotStatusType](./literals.md#segmentsnapshotstatustype)
- [ServiceNowConnectorOperatorType](./literals.md#servicenowconnectoroperatortype)
- [SourceConnectorTypeType](./literals.md#sourceconnectortypetype)
- [StandardIdentifierType](./literals.md#standardidentifiertype)
- [StatisticType](./literals.md#statistictype)
- [StatusType](./literals.md#statustype)
- [StringDimensionTypeType](./literals.md#stringdimensiontypetype)
- [TaskTypeType](./literals.md#tasktypetype)
- [TriggerTypeType](./literals.md#triggertypetype)
- [TypeType](./literals.md#typetype)
- [UnitType](./literals.md#unittype)
- [WorkflowTypeType](./literals.md#workflowtypetype)
- [ZendeskConnectorOperatorType](./literals.md#zendeskconnectoroperatortype)
- [CustomerProfilesServiceName](./literals.md#customerprofilesservicename)
- [ServiceName](./literals.md#servicename)
- [ResourceServiceName](./literals.md#resourceservicename)
- [PaginatorName](./literals.md#paginatorname)
- [RegionName](./literals.md#regionname)




## Type definitions

Type annotations for [type definitions](./type_defs.md) used in methods and schema.

- [AddProfileKeyRequestRequestTypeDef](./type_defs.md#addprofilekeyrequestrequesttypedef)
- [ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef)
- [AdditionalSearchKeyTypeDef](./type_defs.md#additionalsearchkeytypedef)
- [ProfileDimensionOutputTypeDef](./type_defs.md#profiledimensionoutputtypedef)
- [AddressTypeDef](./type_defs.md#addresstypedef)
- [AppflowIntegrationWorkflowAttributesTypeDef](./type_defs.md#appflowintegrationworkflowattributestypedef)
- [AppflowIntegrationWorkflowMetricsTypeDef](./type_defs.md#appflowintegrationworkflowmetricstypedef)
- [AppflowIntegrationWorkflowStepTypeDef](./type_defs.md#appflowintegrationworkflowsteptypedef)
- [AttributeItemTypeDef](./type_defs.md#attributeitemtypedef)
- [AttributeDimensionOutputTypeDef](./type_defs.md#attributedimensionoutputtypedef)
- [AttributeDimensionTypeDef](./type_defs.md#attributedimensiontypedef)
- [AttributeTypesSelectorOutputTypeDef](./type_defs.md#attributetypesselectoroutputtypedef)
- [AttributeTypesSelectorTypeDef](./type_defs.md#attributetypesselectortypedef)
- [AttributeValueItemTypeDef](./type_defs.md#attributevalueitemtypedef)
- [ConflictResolutionTypeDef](./type_defs.md#conflictresolutiontypedef)
- [ConsolidationOutputTypeDef](./type_defs.md#consolidationoutputtypedef)
- [BatchGetCalculatedAttributeForProfileErrorTypeDef](./type_defs.md#batchgetcalculatedattributeforprofileerrortypedef)
- [CalculatedAttributeValueTypeDef](./type_defs.md#calculatedattributevaluetypedef)
- [BatchGetProfileErrorTypeDef](./type_defs.md#batchgetprofileerrortypedef)
- [BatchGetProfileRequestRequestTypeDef](./type_defs.md#batchgetprofilerequestrequesttypedef)
- [TimestampTypeDef](./type_defs.md#timestamptypedef)
- [RangeOverrideTypeDef](./type_defs.md#rangeoverridetypedef)
- [RangeTypeDef](./type_defs.md#rangetypedef)
- [ThresholdTypeDef](./type_defs.md#thresholdtypedef)
- [ConnectorOperatorTypeDef](./type_defs.md#connectoroperatortypedef)
- [ConsolidationTypeDef](./type_defs.md#consolidationtypedef)
- [CreateEventStreamRequestRequestTypeDef](./type_defs.md#createeventstreamrequestrequesttypedef)
- [CreateSegmentSnapshotRequestRequestTypeDef](./type_defs.md#createsegmentsnapshotrequestrequesttypedef)
- [DateDimensionOutputTypeDef](./type_defs.md#datedimensionoutputtypedef)
- [DateDimensionTypeDef](./type_defs.md#datedimensiontypedef)
- [DeleteCalculatedAttributeDefinitionRequestRequestTypeDef](./type_defs.md#deletecalculatedattributedefinitionrequestrequesttypedef)
- [DeleteDomainRequestRequestTypeDef](./type_defs.md#deletedomainrequestrequesttypedef)
- [DeleteEventStreamRequestRequestTypeDef](./type_defs.md#deleteeventstreamrequestrequesttypedef)
- [DeleteEventTriggerRequestRequestTypeDef](./type_defs.md#deleteeventtriggerrequestrequesttypedef)
- [DeleteIntegrationRequestRequestTypeDef](./type_defs.md#deleteintegrationrequestrequesttypedef)
- [DeleteProfileKeyRequestRequestTypeDef](./type_defs.md#deleteprofilekeyrequestrequesttypedef)
- [DeleteProfileObjectRequestRequestTypeDef](./type_defs.md#deleteprofileobjectrequestrequesttypedef)
- [DeleteProfileObjectTypeRequestRequestTypeDef](./type_defs.md#deleteprofileobjecttyperequestrequesttypedef)
- [DeleteProfileRequestRequestTypeDef](./type_defs.md#deleteprofilerequestrequesttypedef)
- [DeleteSegmentDefinitionRequestRequestTypeDef](./type_defs.md#deletesegmentdefinitionrequestrequesttypedef)
- [DeleteWorkflowRequestRequestTypeDef](./type_defs.md#deleteworkflowrequestrequesttypedef)
- [DestinationSummaryTypeDef](./type_defs.md#destinationsummarytypedef)
- [DetectProfileObjectTypeRequestRequestTypeDef](./type_defs.md#detectprofileobjecttyperequestrequesttypedef)
- [ObjectTypeFieldTypeDef](./type_defs.md#objecttypefieldtypedef)
- [ObjectTypeKeyOutputTypeDef](./type_defs.md#objecttypekeyoutputtypedef)
- [DomainStatsTypeDef](./type_defs.md#domainstatstypedef)
- [EventStreamDestinationDetailsTypeDef](./type_defs.md#eventstreamdestinationdetailstypedef)
- [ObjectAttributeOutputTypeDef](./type_defs.md#objectattributeoutputtypedef)
- [PeriodTypeDef](./type_defs.md#periodtypedef)
- [EventTriggerSummaryItemTypeDef](./type_defs.md#eventtriggersummaryitemtypedef)
- [S3ExportingConfigTypeDef](./type_defs.md#s3exportingconfigtypedef)
- [S3ExportingLocationTypeDef](./type_defs.md#s3exportinglocationtypedef)
- [ExtraLengthValueProfileDimensionOutputTypeDef](./type_defs.md#extralengthvalueprofiledimensionoutputtypedef)
- [ExtraLengthValueProfileDimensionTypeDef](./type_defs.md#extralengthvalueprofiledimensiontypedef)
- [FieldSourceProfileIdsTypeDef](./type_defs.md#fieldsourceprofileidstypedef)
- [FilterAttributeDimensionOutputTypeDef](./type_defs.md#filterattributedimensionoutputtypedef)
- [FilterAttributeDimensionTypeDef](./type_defs.md#filterattributedimensiontypedef)
- [FoundByKeyValueTypeDef](./type_defs.md#foundbykeyvaluetypedef)
- [GetCalculatedAttributeDefinitionRequestRequestTypeDef](./type_defs.md#getcalculatedattributedefinitionrequestrequesttypedef)
- [GetCalculatedAttributeForProfileRequestRequestTypeDef](./type_defs.md#getcalculatedattributeforprofilerequestrequesttypedef)
- [GetDomainRequestRequestTypeDef](./type_defs.md#getdomainrequestrequesttypedef)
- [GetEventStreamRequestRequestTypeDef](./type_defs.md#geteventstreamrequestrequesttypedef)
- [GetEventTriggerRequestRequestTypeDef](./type_defs.md#geteventtriggerrequestrequesttypedef)
- [GetIdentityResolutionJobRequestRequestTypeDef](./type_defs.md#getidentityresolutionjobrequestrequesttypedef)
- [JobStatsTypeDef](./type_defs.md#jobstatstypedef)
- [GetIntegrationRequestRequestTypeDef](./type_defs.md#getintegrationrequestrequesttypedef)
- [GetMatchesRequestRequestTypeDef](./type_defs.md#getmatchesrequestrequesttypedef)
- [MatchItemTypeDef](./type_defs.md#matchitemtypedef)
- [GetProfileObjectTypeRequestRequestTypeDef](./type_defs.md#getprofileobjecttyperequestrequesttypedef)
- [GetProfileObjectTypeTemplateRequestRequestTypeDef](./type_defs.md#getprofileobjecttypetemplaterequestrequesttypedef)
- [GetSegmentDefinitionRequestRequestTypeDef](./type_defs.md#getsegmentdefinitionrequestrequesttypedef)
- [GetSegmentEstimateRequestRequestTypeDef](./type_defs.md#getsegmentestimaterequestrequesttypedef)
- [GetSegmentMembershipRequestRequestTypeDef](./type_defs.md#getsegmentmembershiprequestrequesttypedef)
- [ProfileQueryFailuresTypeDef](./type_defs.md#profilequeryfailurestypedef)
- [GetSegmentSnapshotRequestRequestTypeDef](./type_defs.md#getsegmentsnapshotrequestrequesttypedef)
- [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
- [GetSimilarProfilesRequestRequestTypeDef](./type_defs.md#getsimilarprofilesrequestrequesttypedef)
- [GetWorkflowRequestRequestTypeDef](./type_defs.md#getworkflowrequestrequesttypedef)
- [GetWorkflowStepsRequestRequestTypeDef](./type_defs.md#getworkflowstepsrequestrequesttypedef)
- [SourceSegmentTypeDef](./type_defs.md#sourcesegmenttypedef)
- [IncrementalPullConfigTypeDef](./type_defs.md#incrementalpullconfigtypedef)
- [JobScheduleTypeDef](./type_defs.md#jobscheduletypedef)
- [ListAccountIntegrationsRequestRequestTypeDef](./type_defs.md#listaccountintegrationsrequestrequesttypedef)
- [ListIntegrationItemTypeDef](./type_defs.md#listintegrationitemtypedef)
- [ListCalculatedAttributeDefinitionItemTypeDef](./type_defs.md#listcalculatedattributedefinitionitemtypedef)
- [ListCalculatedAttributeDefinitionsRequestRequestTypeDef](./type_defs.md#listcalculatedattributedefinitionsrequestrequesttypedef)
- [ListCalculatedAttributeForProfileItemTypeDef](./type_defs.md#listcalculatedattributeforprofileitemtypedef)
- [ListCalculatedAttributesForProfileRequestRequestTypeDef](./type_defs.md#listcalculatedattributesforprofilerequestrequesttypedef)
- [ListDomainItemTypeDef](./type_defs.md#listdomainitemtypedef)
- [ListDomainsRequestRequestTypeDef](./type_defs.md#listdomainsrequestrequesttypedef)
- [ListEventStreamsRequestRequestTypeDef](./type_defs.md#listeventstreamsrequestrequesttypedef)
- [ListEventTriggersRequestRequestTypeDef](./type_defs.md#listeventtriggersrequestrequesttypedef)
- [ListIdentityResolutionJobsRequestRequestTypeDef](./type_defs.md#listidentityresolutionjobsrequestrequesttypedef)
- [ListIntegrationsRequestRequestTypeDef](./type_defs.md#listintegrationsrequestrequesttypedef)
- [ListObjectTypeAttributeItemTypeDef](./type_defs.md#listobjecttypeattributeitemtypedef)
- [ListObjectTypeAttributesRequestRequestTypeDef](./type_defs.md#listobjecttypeattributesrequestrequesttypedef)
- [ListProfileObjectTypeItemTypeDef](./type_defs.md#listprofileobjecttypeitemtypedef)
- [ListProfileObjectTypeTemplateItemTypeDef](./type_defs.md#listprofileobjecttypetemplateitemtypedef)
- [ListProfileObjectTypeTemplatesRequestRequestTypeDef](./type_defs.md#listprofileobjecttypetemplatesrequestrequesttypedef)
- [ListProfileObjectTypesRequestRequestTypeDef](./type_defs.md#listprofileobjecttypesrequestrequesttypedef)
- [ListProfileObjectsItemTypeDef](./type_defs.md#listprofileobjectsitemtypedef)
- [ObjectFilterTypeDef](./type_defs.md#objectfiltertypedef)
- [ListRuleBasedMatchesRequestRequestTypeDef](./type_defs.md#listrulebasedmatchesrequestrequesttypedef)
- [ListSegmentDefinitionsRequestRequestTypeDef](./type_defs.md#listsegmentdefinitionsrequestrequesttypedef)
- [SegmentDefinitionItemTypeDef](./type_defs.md#segmentdefinitionitemtypedef)
- [ListTagsForResourceRequestRequestTypeDef](./type_defs.md#listtagsforresourcerequestrequesttypedef)
- [ListWorkflowsItemTypeDef](./type_defs.md#listworkflowsitemtypedef)
- [MarketoSourcePropertiesTypeDef](./type_defs.md#marketosourcepropertiestypedef)
- [MatchingRuleOutputTypeDef](./type_defs.md#matchingruleoutputtypedef)
- [MatchingRuleTypeDef](./type_defs.md#matchingruletypedef)
- [ObjectAttributeTypeDef](./type_defs.md#objectattributetypedef)
- [ObjectTypeKeyTypeDef](./type_defs.md#objecttypekeytypedef)
- [ProfileAttributeValuesRequestRequestTypeDef](./type_defs.md#profileattributevaluesrequestrequesttypedef)
- [ProfileDimensionTypeDef](./type_defs.md#profiledimensiontypedef)
- [PutProfileObjectRequestRequestTypeDef](./type_defs.md#putprofileobjectrequestrequesttypedef)
- [S3SourcePropertiesTypeDef](./type_defs.md#s3sourcepropertiestypedef)
- [SalesforceSourcePropertiesTypeDef](./type_defs.md#salesforcesourcepropertiestypedef)
- [ServiceNowSourcePropertiesTypeDef](./type_defs.md#servicenowsourcepropertiestypedef)
- [ZendeskSourcePropertiesTypeDef](./type_defs.md#zendesksourcepropertiestypedef)
- [TagResourceRequestRequestTypeDef](./type_defs.md#tagresourcerequestrequesttypedef)
- [UntagResourceRequestRequestTypeDef](./type_defs.md#untagresourcerequestrequesttypedef)
- [UpdateAddressTypeDef](./type_defs.md#updateaddresstypedef)
- [AddProfileKeyResponseTypeDef](./type_defs.md#addprofilekeyresponsetypedef)
- [CreateEventStreamResponseTypeDef](./type_defs.md#createeventstreamresponsetypedef)
- [CreateIntegrationWorkflowResponseTypeDef](./type_defs.md#createintegrationworkflowresponsetypedef)
- [CreateProfileResponseTypeDef](./type_defs.md#createprofileresponsetypedef)
- [CreateSegmentDefinitionResponseTypeDef](./type_defs.md#createsegmentdefinitionresponsetypedef)
- [CreateSegmentEstimateResponseTypeDef](./type_defs.md#createsegmentestimateresponsetypedef)
- [CreateSegmentSnapshotResponseTypeDef](./type_defs.md#createsegmentsnapshotresponsetypedef)
- [DeleteDomainResponseTypeDef](./type_defs.md#deletedomainresponsetypedef)
- [DeleteEventTriggerResponseTypeDef](./type_defs.md#deleteeventtriggerresponsetypedef)
- [DeleteIntegrationResponseTypeDef](./type_defs.md#deleteintegrationresponsetypedef)
- [DeleteProfileKeyResponseTypeDef](./type_defs.md#deleteprofilekeyresponsetypedef)
- [DeleteProfileObjectResponseTypeDef](./type_defs.md#deleteprofileobjectresponsetypedef)
- [DeleteProfileObjectTypeResponseTypeDef](./type_defs.md#deleteprofileobjecttyperesponsetypedef)
- [DeleteProfileResponseTypeDef](./type_defs.md#deleteprofileresponsetypedef)
- [DeleteSegmentDefinitionResponseTypeDef](./type_defs.md#deletesegmentdefinitionresponsetypedef)
- [GetAutoMergingPreviewResponseTypeDef](./type_defs.md#getautomergingpreviewresponsetypedef)
- [GetCalculatedAttributeForProfileResponseTypeDef](./type_defs.md#getcalculatedattributeforprofileresponsetypedef)
- [GetIntegrationResponseTypeDef](./type_defs.md#getintegrationresponsetypedef)
- [GetSegmentEstimateResponseTypeDef](./type_defs.md#getsegmentestimateresponsetypedef)
- [GetSegmentSnapshotResponseTypeDef](./type_defs.md#getsegmentsnapshotresponsetypedef)
- [GetSimilarProfilesResponseTypeDef](./type_defs.md#getsimilarprofilesresponsetypedef)
- [ListRuleBasedMatchesResponseTypeDef](./type_defs.md#listrulebasedmatchesresponsetypedef)
- [ListTagsForResourceResponseTypeDef](./type_defs.md#listtagsforresourceresponsetypedef)
- [MergeProfilesResponseTypeDef](./type_defs.md#mergeprofilesresponsetypedef)
- [PutIntegrationResponseTypeDef](./type_defs.md#putintegrationresponsetypedef)
- [PutProfileObjectResponseTypeDef](./type_defs.md#putprofileobjectresponsetypedef)
- [UpdateProfileResponseTypeDef](./type_defs.md#updateprofileresponsetypedef)
- [SearchProfilesRequestRequestTypeDef](./type_defs.md#searchprofilesrequestrequesttypedef)
- [AddressDimensionOutputTypeDef](./type_defs.md#addressdimensionoutputtypedef)
- [CreateProfileRequestRequestTypeDef](./type_defs.md#createprofilerequestrequesttypedef)
- [WorkflowAttributesTypeDef](./type_defs.md#workflowattributestypedef)
- [WorkflowMetricsTypeDef](./type_defs.md#workflowmetricstypedef)
- [WorkflowStepItemTypeDef](./type_defs.md#workflowstepitemtypedef)
- [AttributeDetailsOutputTypeDef](./type_defs.md#attributedetailsoutputtypedef)
- [AttributeDetailsTypeDef](./type_defs.md#attributedetailstypedef)
- [AttributeDimensionUnionTypeDef](./type_defs.md#attributedimensionuniontypedef)
- [AttributeTypesSelectorUnionTypeDef](./type_defs.md#attributetypesselectoruniontypedef)
- [ProfileAttributeValuesResponseTypeDef](./type_defs.md#profileattributevaluesresponsetypedef)
- [AutoMergingOutputTypeDef](./type_defs.md#automergingoutputtypedef)
- [BatchTypeDef](./type_defs.md#batchtypedef)
- [ListWorkflowsRequestRequestTypeDef](./type_defs.md#listworkflowsrequestrequesttypedef)
- [ScheduledTriggerPropertiesTypeDef](./type_defs.md#scheduledtriggerpropertiestypedef)
- [ConditionOverridesTypeDef](./type_defs.md#conditionoverridestypedef)
- [ConditionsTypeDef](./type_defs.md#conditionstypedef)
- [TaskTypeDef](./type_defs.md#tasktypedef)
- [ConsolidationUnionTypeDef](./type_defs.md#consolidationuniontypedef)
- [GetAutoMergingPreviewRequestRequestTypeDef](./type_defs.md#getautomergingpreviewrequestrequesttypedef)
- [DateDimensionUnionTypeDef](./type_defs.md#datedimensionuniontypedef)
- [EventStreamSummaryTypeDef](./type_defs.md#eventstreamsummarytypedef)
- [DetectedProfileObjectTypeTypeDef](./type_defs.md#detectedprofileobjecttypetypedef)
- [GetProfileObjectTypeResponseTypeDef](./type_defs.md#getprofileobjecttyperesponsetypedef)
- [GetProfileObjectTypeTemplateResponseTypeDef](./type_defs.md#getprofileobjecttypetemplateresponsetypedef)
- [PutProfileObjectTypeResponseTypeDef](./type_defs.md#putprofileobjecttyperesponsetypedef)
- [GetEventStreamResponseTypeDef](./type_defs.md#geteventstreamresponsetypedef)
- [EventTriggerDimensionOutputTypeDef](./type_defs.md#eventtriggerdimensionoutputtypedef)
- [EventTriggerLimitsOutputTypeDef](./type_defs.md#eventtriggerlimitsoutputtypedef)
- [EventTriggerLimitsTypeDef](./type_defs.md#eventtriggerlimitstypedef)
- [ListEventTriggersResponseTypeDef](./type_defs.md#listeventtriggersresponsetypedef)
- [ExportingConfigTypeDef](./type_defs.md#exportingconfigtypedef)
- [ExportingLocationTypeDef](./type_defs.md#exportinglocationtypedef)
- [ExtraLengthValueProfileDimensionUnionTypeDef](./type_defs.md#extralengthvalueprofiledimensionuniontypedef)
- [MergeProfilesRequestRequestTypeDef](./type_defs.md#mergeprofilesrequestrequesttypedef)
- [FilterDimensionOutputTypeDef](./type_defs.md#filterdimensionoutputtypedef)
- [FilterAttributeDimensionUnionTypeDef](./type_defs.md#filterattributedimensionuniontypedef)
- [ProfileTypeDef](./type_defs.md#profiletypedef)
- [GetMatchesResponseTypeDef](./type_defs.md#getmatchesresponsetypedef)
- [GetSimilarProfilesRequestGetSimilarProfilesPaginateTypeDef](./type_defs.md#getsimilarprofilesrequestgetsimilarprofilespaginatetypedef)
- [ListEventStreamsRequestListEventStreamsPaginateTypeDef](./type_defs.md#listeventstreamsrequestlisteventstreamspaginatetypedef)
- [ListEventTriggersRequestListEventTriggersPaginateTypeDef](./type_defs.md#listeventtriggersrequestlisteventtriggerspaginatetypedef)
- [ListObjectTypeAttributesRequestListObjectTypeAttributesPaginateTypeDef](./type_defs.md#listobjecttypeattributesrequestlistobjecttypeattributespaginatetypedef)
- [ListRuleBasedMatchesRequestListRuleBasedMatchesPaginateTypeDef](./type_defs.md#listrulebasedmatchesrequestlistrulebasedmatchespaginatetypedef)
- [ListSegmentDefinitionsRequestListSegmentDefinitionsPaginateTypeDef](./type_defs.md#listsegmentdefinitionsrequestlistsegmentdefinitionspaginatetypedef)
- [ListAccountIntegrationsResponseTypeDef](./type_defs.md#listaccountintegrationsresponsetypedef)
- [ListIntegrationsResponseTypeDef](./type_defs.md#listintegrationsresponsetypedef)
- [ListCalculatedAttributeDefinitionsResponseTypeDef](./type_defs.md#listcalculatedattributedefinitionsresponsetypedef)
- [ListCalculatedAttributesForProfileResponseTypeDef](./type_defs.md#listcalculatedattributesforprofileresponsetypedef)
- [ListDomainsResponseTypeDef](./type_defs.md#listdomainsresponsetypedef)
- [ListObjectTypeAttributesResponseTypeDef](./type_defs.md#listobjecttypeattributesresponsetypedef)
- [ListProfileObjectTypesResponseTypeDef](./type_defs.md#listprofileobjecttypesresponsetypedef)
- [ListProfileObjectTypeTemplatesResponseTypeDef](./type_defs.md#listprofileobjecttypetemplatesresponsetypedef)
- [ListProfileObjectsResponseTypeDef](./type_defs.md#listprofileobjectsresponsetypedef)
- [ListProfileObjectsRequestRequestTypeDef](./type_defs.md#listprofileobjectsrequestrequesttypedef)
- [ListSegmentDefinitionsResponseTypeDef](./type_defs.md#listsegmentdefinitionsresponsetypedef)
- [ListWorkflowsResponseTypeDef](./type_defs.md#listworkflowsresponsetypedef)
- [MatchingRuleUnionTypeDef](./type_defs.md#matchingruleuniontypedef)
- [ObjectAttributeUnionTypeDef](./type_defs.md#objectattributeuniontypedef)
- [ObjectTypeKeyUnionTypeDef](./type_defs.md#objecttypekeyuniontypedef)
- [ProfileDimensionUnionTypeDef](./type_defs.md#profiledimensionuniontypedef)
- [SourceConnectorPropertiesTypeDef](./type_defs.md#sourceconnectorpropertiestypedef)
- [UpdateProfileRequestRequestTypeDef](./type_defs.md#updateprofilerequestrequesttypedef)
- [ProfileAttributesOutputTypeDef](./type_defs.md#profileattributesoutputtypedef)
- [GetWorkflowResponseTypeDef](./type_defs.md#getworkflowresponsetypedef)
- [GetWorkflowStepsResponseTypeDef](./type_defs.md#getworkflowstepsresponsetypedef)
- [TriggerPropertiesTypeDef](./type_defs.md#triggerpropertiestypedef)
- [BatchGetCalculatedAttributeForProfileRequestRequestTypeDef](./type_defs.md#batchgetcalculatedattributeforprofilerequestrequesttypedef)
- [BatchGetCalculatedAttributeForProfileResponseTypeDef](./type_defs.md#batchgetcalculatedattributeforprofileresponsetypedef)
- [CalculatedAttributeDimensionOutputTypeDef](./type_defs.md#calculatedattributedimensionoutputtypedef)
- [CalculatedAttributeDimensionTypeDef](./type_defs.md#calculatedattributedimensiontypedef)
- [UpdateCalculatedAttributeDefinitionRequestRequestTypeDef](./type_defs.md#updatecalculatedattributedefinitionrequestrequesttypedef)
- [UpdateCalculatedAttributeDefinitionResponseTypeDef](./type_defs.md#updatecalculatedattributedefinitionresponsetypedef)
- [AutoMergingTypeDef](./type_defs.md#automergingtypedef)
- [ListEventStreamsResponseTypeDef](./type_defs.md#listeventstreamsresponsetypedef)
- [DetectProfileObjectTypeResponseTypeDef](./type_defs.md#detectprofileobjecttyperesponsetypedef)
- [EventTriggerConditionOutputTypeDef](./type_defs.md#eventtriggerconditionoutputtypedef)
- [MatchingResponseTypeDef](./type_defs.md#matchingresponsetypedef)
- [RuleBasedMatchingResponseTypeDef](./type_defs.md#rulebasedmatchingresponsetypedef)
- [GetIdentityResolutionJobResponseTypeDef](./type_defs.md#getidentityresolutionjobresponsetypedef)
- [IdentityResolutionJobTypeDef](./type_defs.md#identityresolutionjobtypedef)
- [FilterGroupOutputTypeDef](./type_defs.md#filtergroupoutputtypedef)
- [FilterDimensionTypeDef](./type_defs.md#filterdimensiontypedef)
- [BatchGetProfileResponseTypeDef](./type_defs.md#batchgetprofileresponsetypedef)
- [ProfileQueryResultTypeDef](./type_defs.md#profilequeryresulttypedef)
- [SearchProfilesResponseTypeDef](./type_defs.md#searchprofilesresponsetypedef)
- [RuleBasedMatchingRequestTypeDef](./type_defs.md#rulebasedmatchingrequesttypedef)
- [EventTriggerDimensionTypeDef](./type_defs.md#eventtriggerdimensiontypedef)
- [PutProfileObjectTypeRequestRequestTypeDef](./type_defs.md#putprofileobjecttyperequestrequesttypedef)
- [AddressDimensionTypeDef](./type_defs.md#addressdimensiontypedef)
- [SourceFlowConfigTypeDef](./type_defs.md#sourceflowconfigtypedef)
- [TriggerConfigTypeDef](./type_defs.md#triggerconfigtypedef)
- [DimensionOutputTypeDef](./type_defs.md#dimensionoutputtypedef)
- [CalculatedAttributeDimensionUnionTypeDef](./type_defs.md#calculatedattributedimensionuniontypedef)
- [AutoMergingUnionTypeDef](./type_defs.md#automerginguniontypedef)
- [CreateEventTriggerResponseTypeDef](./type_defs.md#createeventtriggerresponsetypedef)
- [GetEventTriggerResponseTypeDef](./type_defs.md#geteventtriggerresponsetypedef)
- [UpdateEventTriggerResponseTypeDef](./type_defs.md#updateeventtriggerresponsetypedef)
- [CreateDomainResponseTypeDef](./type_defs.md#createdomainresponsetypedef)
- [GetDomainResponseTypeDef](./type_defs.md#getdomainresponsetypedef)
- [UpdateDomainResponseTypeDef](./type_defs.md#updatedomainresponsetypedef)
- [ListIdentityResolutionJobsResponseTypeDef](./type_defs.md#listidentityresolutionjobsresponsetypedef)
- [FilterOutputTypeDef](./type_defs.md#filteroutputtypedef)
- [FilterDimensionUnionTypeDef](./type_defs.md#filterdimensionuniontypedef)
- [GetSegmentMembershipResponseTypeDef](./type_defs.md#getsegmentmembershipresponsetypedef)
- [EventTriggerDimensionUnionTypeDef](./type_defs.md#eventtriggerdimensionuniontypedef)
- [AddressDimensionUnionTypeDef](./type_defs.md#addressdimensionuniontypedef)
- [FlowDefinitionTypeDef](./type_defs.md#flowdefinitiontypedef)
- [GroupOutputTypeDef](./type_defs.md#groupoutputtypedef)
- [MatchingRequestTypeDef](./type_defs.md#matchingrequesttypedef)
- [CreateCalculatedAttributeDefinitionResponseTypeDef](./type_defs.md#createcalculatedattributedefinitionresponsetypedef)
- [GetCalculatedAttributeDefinitionResponseTypeDef](./type_defs.md#getcalculatedattributedefinitionresponsetypedef)
- [FilterGroupTypeDef](./type_defs.md#filtergrouptypedef)
- [EventTriggerConditionTypeDef](./type_defs.md#eventtriggerconditiontypedef)
- [ProfileAttributesTypeDef](./type_defs.md#profileattributestypedef)
- [AppflowIntegrationTypeDef](./type_defs.md#appflowintegrationtypedef)
- [PutIntegrationRequestRequestTypeDef](./type_defs.md#putintegrationrequestrequesttypedef)
- [SegmentGroupOutputTypeDef](./type_defs.md#segmentgroupoutputtypedef)
- [CreateDomainRequestRequestTypeDef](./type_defs.md#createdomainrequestrequesttypedef)
- [UpdateDomainRequestRequestTypeDef](./type_defs.md#updatedomainrequestrequesttypedef)
- [FilterGroupUnionTypeDef](./type_defs.md#filtergroupuniontypedef)
- [EventTriggerConditionUnionTypeDef](./type_defs.md#eventtriggerconditionuniontypedef)
- [UpdateEventTriggerRequestRequestTypeDef](./type_defs.md#updateeventtriggerrequestrequesttypedef)
- [ProfileAttributesUnionTypeDef](./type_defs.md#profileattributesuniontypedef)
- [IntegrationConfigTypeDef](./type_defs.md#integrationconfigtypedef)
- [GetSegmentDefinitionResponseTypeDef](./type_defs.md#getsegmentdefinitionresponsetypedef)
- [FilterTypeDef](./type_defs.md#filtertypedef)
- [CreateEventTriggerRequestRequestTypeDef](./type_defs.md#createeventtriggerrequestrequesttypedef)
- [DimensionTypeDef](./type_defs.md#dimensiontypedef)
- [CreateIntegrationWorkflowRequestRequestTypeDef](./type_defs.md#createintegrationworkflowrequestrequesttypedef)
- [CreateCalculatedAttributeDefinitionRequestRequestTypeDef](./type_defs.md#createcalculatedattributedefinitionrequestrequesttypedef)
- [DimensionUnionTypeDef](./type_defs.md#dimensionuniontypedef)
- [GroupTypeDef](./type_defs.md#grouptypedef)
- [GroupUnionTypeDef](./type_defs.md#groupuniontypedef)
- [SegmentGroupStructureTypeDef](./type_defs.md#segmentgroupstructuretypedef)
- [SegmentGroupTypeDef](./type_defs.md#segmentgrouptypedef)
- [CreateSegmentEstimateRequestRequestTypeDef](./type_defs.md#createsegmentestimaterequestrequesttypedef)
- [CreateSegmentDefinitionRequestRequestTypeDef](./type_defs.md#createsegmentdefinitionrequestrequesttypedef)

