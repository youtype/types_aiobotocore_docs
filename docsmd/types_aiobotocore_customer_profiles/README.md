# CustomerProfiles module

> [Index](../README.md) > CustomerProfiles


!!! note ""

    Auto-generated documentation for [CustomerProfiles](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/customer-profiles.html#customerprofiles)
    type annotations stubs module [types-aiobotocore-customer-profiles](https://pypi.org/project/types-aiobotocore-customer-profiles/).

## How to install

### Generate locally (recommended)

You can generate type annotations for `aiobotocore` package locally with `mypy-boto3-builder`.
Use [uv](https://docs.astral.sh/uv/getting-started/installation/) for build isolation.

1. Run mypy-boto3-builder in your package root directory: `uvx --with 'aiobotocore==2.20.0' mypy-boto3-builder`
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

- [AddProfileKeyRequestTypeDef](./type_defs.md#addprofilekeyrequesttypedef)
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
- [BatchGetProfileRequestTypeDef](./type_defs.md#batchgetprofilerequesttypedef)
- [TimestampTypeDef](./type_defs.md#timestamptypedef)
- [RangeOverrideTypeDef](./type_defs.md#rangeoverridetypedef)
- [RangeTypeDef](./type_defs.md#rangetypedef)
- [ThresholdTypeDef](./type_defs.md#thresholdtypedef)
- [ConnectorOperatorTypeDef](./type_defs.md#connectoroperatortypedef)
- [ConsolidationTypeDef](./type_defs.md#consolidationtypedef)
- [CreateEventStreamRequestTypeDef](./type_defs.md#createeventstreamrequesttypedef)
- [CreateSegmentSnapshotRequestTypeDef](./type_defs.md#createsegmentsnapshotrequesttypedef)
- [DateDimensionOutputTypeDef](./type_defs.md#datedimensionoutputtypedef)
- [DateDimensionTypeDef](./type_defs.md#datedimensiontypedef)
- [DeleteCalculatedAttributeDefinitionRequestTypeDef](./type_defs.md#deletecalculatedattributedefinitionrequesttypedef)
- [DeleteDomainRequestTypeDef](./type_defs.md#deletedomainrequesttypedef)
- [DeleteEventStreamRequestTypeDef](./type_defs.md#deleteeventstreamrequesttypedef)
- [DeleteEventTriggerRequestTypeDef](./type_defs.md#deleteeventtriggerrequesttypedef)
- [DeleteIntegrationRequestTypeDef](./type_defs.md#deleteintegrationrequesttypedef)
- [DeleteProfileKeyRequestTypeDef](./type_defs.md#deleteprofilekeyrequesttypedef)
- [DeleteProfileObjectRequestTypeDef](./type_defs.md#deleteprofileobjectrequesttypedef)
- [DeleteProfileObjectTypeRequestTypeDef](./type_defs.md#deleteprofileobjecttyperequesttypedef)
- [DeleteProfileRequestTypeDef](./type_defs.md#deleteprofilerequesttypedef)
- [DeleteSegmentDefinitionRequestTypeDef](./type_defs.md#deletesegmentdefinitionrequesttypedef)
- [DeleteWorkflowRequestTypeDef](./type_defs.md#deleteworkflowrequesttypedef)
- [DestinationSummaryTypeDef](./type_defs.md#destinationsummarytypedef)
- [DetectProfileObjectTypeRequestTypeDef](./type_defs.md#detectprofileobjecttyperequesttypedef)
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
- [GetCalculatedAttributeDefinitionRequestTypeDef](./type_defs.md#getcalculatedattributedefinitionrequesttypedef)
- [GetCalculatedAttributeForProfileRequestTypeDef](./type_defs.md#getcalculatedattributeforprofilerequesttypedef)
- [GetDomainRequestTypeDef](./type_defs.md#getdomainrequesttypedef)
- [GetEventStreamRequestTypeDef](./type_defs.md#geteventstreamrequesttypedef)
- [GetEventTriggerRequestTypeDef](./type_defs.md#geteventtriggerrequesttypedef)
- [GetIdentityResolutionJobRequestTypeDef](./type_defs.md#getidentityresolutionjobrequesttypedef)
- [JobStatsTypeDef](./type_defs.md#jobstatstypedef)
- [GetIntegrationRequestTypeDef](./type_defs.md#getintegrationrequesttypedef)
- [GetMatchesRequestTypeDef](./type_defs.md#getmatchesrequesttypedef)
- [MatchItemTypeDef](./type_defs.md#matchitemtypedef)
- [GetProfileObjectTypeRequestTypeDef](./type_defs.md#getprofileobjecttyperequesttypedef)
- [GetProfileObjectTypeTemplateRequestTypeDef](./type_defs.md#getprofileobjecttypetemplaterequesttypedef)
- [GetSegmentDefinitionRequestTypeDef](./type_defs.md#getsegmentdefinitionrequesttypedef)
- [GetSegmentEstimateRequestTypeDef](./type_defs.md#getsegmentestimaterequesttypedef)
- [GetSegmentMembershipRequestTypeDef](./type_defs.md#getsegmentmembershiprequesttypedef)
- [ProfileQueryFailuresTypeDef](./type_defs.md#profilequeryfailurestypedef)
- [GetSegmentSnapshotRequestTypeDef](./type_defs.md#getsegmentsnapshotrequesttypedef)
- [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
- [GetSimilarProfilesRequestTypeDef](./type_defs.md#getsimilarprofilesrequesttypedef)
- [GetWorkflowRequestTypeDef](./type_defs.md#getworkflowrequesttypedef)
- [GetWorkflowStepsRequestTypeDef](./type_defs.md#getworkflowstepsrequesttypedef)
- [SourceSegmentTypeDef](./type_defs.md#sourcesegmenttypedef)
- [IncrementalPullConfigTypeDef](./type_defs.md#incrementalpullconfigtypedef)
- [JobScheduleTypeDef](./type_defs.md#jobscheduletypedef)
- [ListAccountIntegrationsRequestTypeDef](./type_defs.md#listaccountintegrationsrequesttypedef)
- [ListIntegrationItemTypeDef](./type_defs.md#listintegrationitemtypedef)
- [ListCalculatedAttributeDefinitionItemTypeDef](./type_defs.md#listcalculatedattributedefinitionitemtypedef)
- [ListCalculatedAttributeDefinitionsRequestTypeDef](./type_defs.md#listcalculatedattributedefinitionsrequesttypedef)
- [ListCalculatedAttributeForProfileItemTypeDef](./type_defs.md#listcalculatedattributeforprofileitemtypedef)
- [ListCalculatedAttributesForProfileRequestTypeDef](./type_defs.md#listcalculatedattributesforprofilerequesttypedef)
- [ListDomainItemTypeDef](./type_defs.md#listdomainitemtypedef)
- [ListDomainsRequestTypeDef](./type_defs.md#listdomainsrequesttypedef)
- [ListEventStreamsRequestTypeDef](./type_defs.md#listeventstreamsrequesttypedef)
- [ListEventTriggersRequestTypeDef](./type_defs.md#listeventtriggersrequesttypedef)
- [ListIdentityResolutionJobsRequestTypeDef](./type_defs.md#listidentityresolutionjobsrequesttypedef)
- [ListIntegrationsRequestTypeDef](./type_defs.md#listintegrationsrequesttypedef)
- [ListObjectTypeAttributeItemTypeDef](./type_defs.md#listobjecttypeattributeitemtypedef)
- [ListObjectTypeAttributesRequestTypeDef](./type_defs.md#listobjecttypeattributesrequesttypedef)
- [ListProfileObjectTypeItemTypeDef](./type_defs.md#listprofileobjecttypeitemtypedef)
- [ListProfileObjectTypeTemplateItemTypeDef](./type_defs.md#listprofileobjecttypetemplateitemtypedef)
- [ListProfileObjectTypeTemplatesRequestTypeDef](./type_defs.md#listprofileobjecttypetemplatesrequesttypedef)
- [ListProfileObjectTypesRequestTypeDef](./type_defs.md#listprofileobjecttypesrequesttypedef)
- [ListProfileObjectsItemTypeDef](./type_defs.md#listprofileobjectsitemtypedef)
- [ObjectFilterTypeDef](./type_defs.md#objectfiltertypedef)
- [ListRuleBasedMatchesRequestTypeDef](./type_defs.md#listrulebasedmatchesrequesttypedef)
- [ListSegmentDefinitionsRequestTypeDef](./type_defs.md#listsegmentdefinitionsrequesttypedef)
- [SegmentDefinitionItemTypeDef](./type_defs.md#segmentdefinitionitemtypedef)
- [ListTagsForResourceRequestTypeDef](./type_defs.md#listtagsforresourcerequesttypedef)
- [ListWorkflowsItemTypeDef](./type_defs.md#listworkflowsitemtypedef)
- [MarketoSourcePropertiesTypeDef](./type_defs.md#marketosourcepropertiestypedef)
- [MatchingRuleOutputTypeDef](./type_defs.md#matchingruleoutputtypedef)
- [MatchingRuleTypeDef](./type_defs.md#matchingruletypedef)
- [ObjectAttributeTypeDef](./type_defs.md#objectattributetypedef)
- [ObjectTypeKeyTypeDef](./type_defs.md#objecttypekeytypedef)
- [ProfileAttributeValuesRequestTypeDef](./type_defs.md#profileattributevaluesrequesttypedef)
- [ProfileDimensionTypeDef](./type_defs.md#profiledimensiontypedef)
- [PutProfileObjectRequestTypeDef](./type_defs.md#putprofileobjectrequesttypedef)
- [S3SourcePropertiesTypeDef](./type_defs.md#s3sourcepropertiestypedef)
- [SalesforceSourcePropertiesTypeDef](./type_defs.md#salesforcesourcepropertiestypedef)
- [ServiceNowSourcePropertiesTypeDef](./type_defs.md#servicenowsourcepropertiestypedef)
- [ZendeskSourcePropertiesTypeDef](./type_defs.md#zendesksourcepropertiestypedef)
- [TagResourceRequestTypeDef](./type_defs.md#tagresourcerequesttypedef)
- [UntagResourceRequestTypeDef](./type_defs.md#untagresourcerequesttypedef)
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
- [SearchProfilesRequestTypeDef](./type_defs.md#searchprofilesrequesttypedef)
- [AddressDimensionOutputTypeDef](./type_defs.md#addressdimensionoutputtypedef)
- [CreateProfileRequestTypeDef](./type_defs.md#createprofilerequesttypedef)
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
- [ListWorkflowsRequestTypeDef](./type_defs.md#listworkflowsrequesttypedef)
- [ScheduledTriggerPropertiesTypeDef](./type_defs.md#scheduledtriggerpropertiestypedef)
- [ConditionOverridesTypeDef](./type_defs.md#conditionoverridestypedef)
- [ConditionsTypeDef](./type_defs.md#conditionstypedef)
- [TaskTypeDef](./type_defs.md#tasktypedef)
- [ConsolidationUnionTypeDef](./type_defs.md#consolidationuniontypedef)
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
- [MergeProfilesRequestTypeDef](./type_defs.md#mergeprofilesrequesttypedef)
- [FilterDimensionOutputTypeDef](./type_defs.md#filterdimensionoutputtypedef)
- [FilterDimensionTypeDef](./type_defs.md#filterdimensiontypedef)
- [ProfileTypeDef](./type_defs.md#profiletypedef)
- [GetMatchesResponseTypeDef](./type_defs.md#getmatchesresponsetypedef)
- [GetSimilarProfilesRequestPaginateTypeDef](./type_defs.md#getsimilarprofilesrequestpaginatetypedef)
- [ListEventStreamsRequestPaginateTypeDef](./type_defs.md#listeventstreamsrequestpaginatetypedef)
- [ListEventTriggersRequestPaginateTypeDef](./type_defs.md#listeventtriggersrequestpaginatetypedef)
- [ListObjectTypeAttributesRequestPaginateTypeDef](./type_defs.md#listobjecttypeattributesrequestpaginatetypedef)
- [ListRuleBasedMatchesRequestPaginateTypeDef](./type_defs.md#listrulebasedmatchesrequestpaginatetypedef)
- [ListSegmentDefinitionsRequestPaginateTypeDef](./type_defs.md#listsegmentdefinitionsrequestpaginatetypedef)
- [ListAccountIntegrationsResponseTypeDef](./type_defs.md#listaccountintegrationsresponsetypedef)
- [ListIntegrationsResponseTypeDef](./type_defs.md#listintegrationsresponsetypedef)
- [ListCalculatedAttributeDefinitionsResponseTypeDef](./type_defs.md#listcalculatedattributedefinitionsresponsetypedef)
- [ListCalculatedAttributesForProfileResponseTypeDef](./type_defs.md#listcalculatedattributesforprofileresponsetypedef)
- [ListDomainsResponseTypeDef](./type_defs.md#listdomainsresponsetypedef)
- [ListObjectTypeAttributesResponseTypeDef](./type_defs.md#listobjecttypeattributesresponsetypedef)
- [ListProfileObjectTypesResponseTypeDef](./type_defs.md#listprofileobjecttypesresponsetypedef)
- [ListProfileObjectTypeTemplatesResponseTypeDef](./type_defs.md#listprofileobjecttypetemplatesresponsetypedef)
- [ListProfileObjectsResponseTypeDef](./type_defs.md#listprofileobjectsresponsetypedef)
- [ListProfileObjectsRequestTypeDef](./type_defs.md#listprofileobjectsrequesttypedef)
- [ListSegmentDefinitionsResponseTypeDef](./type_defs.md#listsegmentdefinitionsresponsetypedef)
- [ListWorkflowsResponseTypeDef](./type_defs.md#listworkflowsresponsetypedef)
- [MatchingRuleUnionTypeDef](./type_defs.md#matchingruleuniontypedef)
- [ObjectAttributeUnionTypeDef](./type_defs.md#objectattributeuniontypedef)
- [ObjectTypeKeyUnionTypeDef](./type_defs.md#objecttypekeyuniontypedef)
- [ProfileDimensionUnionTypeDef](./type_defs.md#profiledimensionuniontypedef)
- [SourceConnectorPropertiesTypeDef](./type_defs.md#sourceconnectorpropertiestypedef)
- [UpdateProfileRequestTypeDef](./type_defs.md#updateprofilerequesttypedef)
- [ProfileAttributesOutputTypeDef](./type_defs.md#profileattributesoutputtypedef)
- [GetWorkflowResponseTypeDef](./type_defs.md#getworkflowresponsetypedef)
- [GetWorkflowStepsResponseTypeDef](./type_defs.md#getworkflowstepsresponsetypedef)
- [AttributeDetailsUnionTypeDef](./type_defs.md#attributedetailsuniontypedef)
- [TriggerPropertiesTypeDef](./type_defs.md#triggerpropertiestypedef)
- [BatchGetCalculatedAttributeForProfileRequestTypeDef](./type_defs.md#batchgetcalculatedattributeforprofilerequesttypedef)
- [BatchGetCalculatedAttributeForProfileResponseTypeDef](./type_defs.md#batchgetcalculatedattributeforprofileresponsetypedef)
- [CalculatedAttributeDimensionOutputTypeDef](./type_defs.md#calculatedattributedimensionoutputtypedef)
- [CalculatedAttributeDimensionTypeDef](./type_defs.md#calculatedattributedimensiontypedef)
- [UpdateCalculatedAttributeDefinitionRequestTypeDef](./type_defs.md#updatecalculatedattributedefinitionrequesttypedef)
- [UpdateCalculatedAttributeDefinitionResponseTypeDef](./type_defs.md#updatecalculatedattributedefinitionresponsetypedef)
- [AutoMergingTypeDef](./type_defs.md#automergingtypedef)
- [GetAutoMergingPreviewRequestTypeDef](./type_defs.md#getautomergingpreviewrequesttypedef)
- [ListEventStreamsResponseTypeDef](./type_defs.md#listeventstreamsresponsetypedef)
- [DetectProfileObjectTypeResponseTypeDef](./type_defs.md#detectprofileobjecttyperesponsetypedef)
- [EventTriggerConditionOutputTypeDef](./type_defs.md#eventtriggerconditionoutputtypedef)
- [EventTriggerLimitsUnionTypeDef](./type_defs.md#eventtriggerlimitsuniontypedef)
- [MatchingResponseTypeDef](./type_defs.md#matchingresponsetypedef)
- [RuleBasedMatchingResponseTypeDef](./type_defs.md#rulebasedmatchingresponsetypedef)
- [GetIdentityResolutionJobResponseTypeDef](./type_defs.md#getidentityresolutionjobresponsetypedef)
- [IdentityResolutionJobTypeDef](./type_defs.md#identityresolutionjobtypedef)
- [FilterGroupOutputTypeDef](./type_defs.md#filtergroupoutputtypedef)
- [FilterGroupTypeDef](./type_defs.md#filtergrouptypedef)
- [BatchGetProfileResponseTypeDef](./type_defs.md#batchgetprofileresponsetypedef)
- [ProfileQueryResultTypeDef](./type_defs.md#profilequeryresulttypedef)
- [SearchProfilesResponseTypeDef](./type_defs.md#searchprofilesresponsetypedef)
- [RuleBasedMatchingRequestTypeDef](./type_defs.md#rulebasedmatchingrequesttypedef)
- [EventTriggerDimensionTypeDef](./type_defs.md#eventtriggerdimensiontypedef)
- [PutProfileObjectTypeRequestTypeDef](./type_defs.md#putprofileobjecttyperequesttypedef)
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
- [FilterTypeDef](./type_defs.md#filtertypedef)
- [GetSegmentMembershipResponseTypeDef](./type_defs.md#getsegmentmembershipresponsetypedef)
- [EventTriggerDimensionUnionTypeDef](./type_defs.md#eventtriggerdimensionuniontypedef)
- [AddressDimensionUnionTypeDef](./type_defs.md#addressdimensionuniontypedef)
- [FlowDefinitionTypeDef](./type_defs.md#flowdefinitiontypedef)
- [GroupOutputTypeDef](./type_defs.md#groupoutputtypedef)
- [MatchingRequestTypeDef](./type_defs.md#matchingrequesttypedef)
- [CreateCalculatedAttributeDefinitionResponseTypeDef](./type_defs.md#createcalculatedattributedefinitionresponsetypedef)
- [GetCalculatedAttributeDefinitionResponseTypeDef](./type_defs.md#getcalculatedattributedefinitionresponsetypedef)
- [FilterUnionTypeDef](./type_defs.md#filteruniontypedef)
- [EventTriggerConditionTypeDef](./type_defs.md#eventtriggerconditiontypedef)
- [ProfileAttributesTypeDef](./type_defs.md#profileattributestypedef)
- [AppflowIntegrationTypeDef](./type_defs.md#appflowintegrationtypedef)
- [PutIntegrationRequestTypeDef](./type_defs.md#putintegrationrequesttypedef)
- [SegmentGroupOutputTypeDef](./type_defs.md#segmentgroupoutputtypedef)
- [CreateDomainRequestTypeDef](./type_defs.md#createdomainrequesttypedef)
- [UpdateDomainRequestTypeDef](./type_defs.md#updatedomainrequesttypedef)
- [CreateCalculatedAttributeDefinitionRequestTypeDef](./type_defs.md#createcalculatedattributedefinitionrequesttypedef)
- [EventTriggerConditionUnionTypeDef](./type_defs.md#eventtriggerconditionuniontypedef)
- [ProfileAttributesUnionTypeDef](./type_defs.md#profileattributesuniontypedef)
- [IntegrationConfigTypeDef](./type_defs.md#integrationconfigtypedef)
- [GetSegmentDefinitionResponseTypeDef](./type_defs.md#getsegmentdefinitionresponsetypedef)
- [CreateEventTriggerRequestTypeDef](./type_defs.md#createeventtriggerrequesttypedef)
- [UpdateEventTriggerRequestTypeDef](./type_defs.md#updateeventtriggerrequesttypedef)
- [DimensionTypeDef](./type_defs.md#dimensiontypedef)
- [CreateIntegrationWorkflowRequestTypeDef](./type_defs.md#createintegrationworkflowrequesttypedef)
- [DimensionUnionTypeDef](./type_defs.md#dimensionuniontypedef)
- [GroupTypeDef](./type_defs.md#grouptypedef)
- [GroupUnionTypeDef](./type_defs.md#groupuniontypedef)
- [SegmentGroupTypeDef](./type_defs.md#segmentgrouptypedef)
- [SegmentGroupStructureTypeDef](./type_defs.md#segmentgroupstructuretypedef)
- [SegmentGroupUnionTypeDef](./type_defs.md#segmentgroupuniontypedef)
- [CreateSegmentEstimateRequestTypeDef](./type_defs.md#createsegmentestimaterequesttypedef)
- [CreateSegmentDefinitionRequestTypeDef](./type_defs.md#createsegmentdefinitionrequesttypedef)

