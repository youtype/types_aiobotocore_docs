# CustomerProfiles module

> [Index](../README.md) > CustomerProfiles


!!! note ""

    Auto-generated documentation for [CustomerProfiles](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/customer-profiles.html#CustomerProfiles)
    type annotations stubs module [types-aiobotocore-customer-profiles](https://pypi.org/project/types-aiobotocore-customer-profiles/).

## How to install



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
# ListEventStreamsPaginator usage example

from types_aiobotocore_customer_profiles.paginator import ListEventStreamsPaginator

def get_list_event_streams_paginator() -> ListEventStreamsPaginator:
    return client.get_paginator("list_event_streams"))
```

- [ListEventStreamsPaginator](./paginators.md#listeventstreamspaginator)








## Literals

Type annotations for [literals](./literals.md) used in methods and schema.

```python
# AttributeMatchingModelType usage example

from types_aiobotocore_customer_profiles.literals import AttributeMatchingModelType

def get_value() -> AttributeMatchingModelType:
    return "MANY_TO_MANY"
```

- [AttributeMatchingModelType](./literals.md#attributematchingmodeltype)
- [ConflictResolvingModelType](./literals.md#conflictresolvingmodeltype)
- [DataPullModeType](./literals.md#datapullmodetype)
- [EventStreamDestinationStatusType](./literals.md#eventstreamdestinationstatustype)
- [EventStreamStateType](./literals.md#eventstreamstatetype)
- [FieldContentTypeType](./literals.md#fieldcontenttypetype)
- [GenderType](./literals.md#gendertype)
- [IdentityResolutionJobStatusType](./literals.md#identityresolutionjobstatustype)
- [JobScheduleDayOfTheWeekType](./literals.md#jobscheduledayoftheweektype)
- [ListEventStreamsPaginatorName](./literals.md#listeventstreamspaginatorname)
- [LogicalOperatorType](./literals.md#logicaloperatortype)
- [MarketoConnectorOperatorType](./literals.md#marketoconnectoroperatortype)
- [MatchTypeType](./literals.md#matchtypetype)
- [OperatorPropertiesKeysType](./literals.md#operatorpropertieskeystype)
- [OperatorType](./literals.md#operatortype)
- [PartyTypeType](./literals.md#partytypetype)
- [RuleBasedMatchingStatusType](./literals.md#rulebasedmatchingstatustype)
- [S3ConnectorOperatorType](./literals.md#s3connectoroperatortype)
- [SalesforceConnectorOperatorType](./literals.md#salesforceconnectoroperatortype)
- [ServiceNowConnectorOperatorType](./literals.md#servicenowconnectoroperatortype)
- [SourceConnectorTypeType](./literals.md#sourceconnectortypetype)
- [StandardIdentifierType](./literals.md#standardidentifiertype)
- [StatisticType](./literals.md#statistictype)
- [StatusType](./literals.md#statustype)
- [TaskTypeType](./literals.md#tasktypetype)
- [TriggerTypeType](./literals.md#triggertypetype)
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
- [AddressTypeDef](./type_defs.md#addresstypedef)
- [AppflowIntegrationWorkflowAttributesTypeDef](./type_defs.md#appflowintegrationworkflowattributestypedef)
- [AppflowIntegrationWorkflowMetricsTypeDef](./type_defs.md#appflowintegrationworkflowmetricstypedef)
- [AppflowIntegrationWorkflowStepTypeDef](./type_defs.md#appflowintegrationworkflowsteptypedef)
- [AttributeItemTypeDef](./type_defs.md#attributeitemtypedef)
- [AttributeTypesSelectorOutputTypeDef](./type_defs.md#attributetypesselectoroutputtypedef)
- [AttributeTypesSelectorTypeDef](./type_defs.md#attributetypesselectortypedef)
- [ConflictResolutionTypeDef](./type_defs.md#conflictresolutiontypedef)
- [ConsolidationOutputTypeDef](./type_defs.md#consolidationoutputtypedef)
- [TimestampTypeDef](./type_defs.md#timestamptypedef)
- [RangeTypeDef](./type_defs.md#rangetypedef)
- [ThresholdTypeDef](./type_defs.md#thresholdtypedef)
- [ConnectorOperatorTypeDef](./type_defs.md#connectoroperatortypedef)
- [ConsolidationTypeDef](./type_defs.md#consolidationtypedef)
- [CreateEventStreamRequestRequestTypeDef](./type_defs.md#createeventstreamrequestrequesttypedef)
- [DeleteCalculatedAttributeDefinitionRequestRequestTypeDef](./type_defs.md#deletecalculatedattributedefinitionrequestrequesttypedef)
- [DeleteDomainRequestRequestTypeDef](./type_defs.md#deletedomainrequestrequesttypedef)
- [DeleteEventStreamRequestRequestTypeDef](./type_defs.md#deleteeventstreamrequestrequesttypedef)
- [DeleteIntegrationRequestRequestTypeDef](./type_defs.md#deleteintegrationrequestrequesttypedef)
- [DeleteProfileKeyRequestRequestTypeDef](./type_defs.md#deleteprofilekeyrequestrequesttypedef)
- [DeleteProfileObjectRequestRequestTypeDef](./type_defs.md#deleteprofileobjectrequestrequesttypedef)
- [DeleteProfileObjectTypeRequestRequestTypeDef](./type_defs.md#deleteprofileobjecttyperequestrequesttypedef)
- [DeleteProfileRequestRequestTypeDef](./type_defs.md#deleteprofilerequestrequesttypedef)
- [DeleteWorkflowRequestRequestTypeDef](./type_defs.md#deleteworkflowrequestrequesttypedef)
- [DestinationSummaryTypeDef](./type_defs.md#destinationsummarytypedef)
- [DetectProfileObjectTypeRequestRequestTypeDef](./type_defs.md#detectprofileobjecttyperequestrequesttypedef)
- [ObjectTypeFieldTypeDef](./type_defs.md#objecttypefieldtypedef)
- [ObjectTypeKeyOutputTypeDef](./type_defs.md#objecttypekeyoutputtypedef)
- [DomainStatsTypeDef](./type_defs.md#domainstatstypedef)
- [EventStreamDestinationDetailsTypeDef](./type_defs.md#eventstreamdestinationdetailstypedef)
- [S3ExportingConfigTypeDef](./type_defs.md#s3exportingconfigtypedef)
- [S3ExportingLocationTypeDef](./type_defs.md#s3exportinglocationtypedef)
- [FieldSourceProfileIdsTypeDef](./type_defs.md#fieldsourceprofileidstypedef)
- [FoundByKeyValueTypeDef](./type_defs.md#foundbykeyvaluetypedef)
- [GetCalculatedAttributeDefinitionRequestRequestTypeDef](./type_defs.md#getcalculatedattributedefinitionrequestrequesttypedef)
- [GetCalculatedAttributeForProfileRequestRequestTypeDef](./type_defs.md#getcalculatedattributeforprofilerequestrequesttypedef)
- [GetDomainRequestRequestTypeDef](./type_defs.md#getdomainrequestrequesttypedef)
- [GetEventStreamRequestRequestTypeDef](./type_defs.md#geteventstreamrequestrequesttypedef)
- [GetIdentityResolutionJobRequestRequestTypeDef](./type_defs.md#getidentityresolutionjobrequestrequesttypedef)
- [JobStatsTypeDef](./type_defs.md#jobstatstypedef)
- [GetIntegrationRequestRequestTypeDef](./type_defs.md#getintegrationrequestrequesttypedef)
- [GetMatchesRequestRequestTypeDef](./type_defs.md#getmatchesrequestrequesttypedef)
- [MatchItemTypeDef](./type_defs.md#matchitemtypedef)
- [GetProfileObjectTypeRequestRequestTypeDef](./type_defs.md#getprofileobjecttyperequestrequesttypedef)
- [GetProfileObjectTypeTemplateRequestRequestTypeDef](./type_defs.md#getprofileobjecttypetemplaterequestrequesttypedef)
- [GetSimilarProfilesRequestRequestTypeDef](./type_defs.md#getsimilarprofilesrequestrequesttypedef)
- [GetWorkflowRequestRequestTypeDef](./type_defs.md#getworkflowrequestrequesttypedef)
- [GetWorkflowStepsRequestRequestTypeDef](./type_defs.md#getworkflowstepsrequestrequesttypedef)
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
- [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
- [ListEventStreamsRequestRequestTypeDef](./type_defs.md#listeventstreamsrequestrequesttypedef)
- [ListIdentityResolutionJobsRequestRequestTypeDef](./type_defs.md#listidentityresolutionjobsrequestrequesttypedef)
- [ListIntegrationsRequestRequestTypeDef](./type_defs.md#listintegrationsrequestrequesttypedef)
- [ListProfileObjectTypeItemTypeDef](./type_defs.md#listprofileobjecttypeitemtypedef)
- [ListProfileObjectTypeTemplateItemTypeDef](./type_defs.md#listprofileobjecttypetemplateitemtypedef)
- [ListProfileObjectTypeTemplatesRequestRequestTypeDef](./type_defs.md#listprofileobjecttypetemplatesrequestrequesttypedef)
- [ListProfileObjectTypesRequestRequestTypeDef](./type_defs.md#listprofileobjecttypesrequestrequesttypedef)
- [ListProfileObjectsItemTypeDef](./type_defs.md#listprofileobjectsitemtypedef)
- [ObjectFilterTypeDef](./type_defs.md#objectfiltertypedef)
- [ListRuleBasedMatchesRequestRequestTypeDef](./type_defs.md#listrulebasedmatchesrequestrequesttypedef)
- [ListTagsForResourceRequestRequestTypeDef](./type_defs.md#listtagsforresourcerequestrequesttypedef)
- [ListWorkflowsItemTypeDef](./type_defs.md#listworkflowsitemtypedef)
- [MarketoSourcePropertiesTypeDef](./type_defs.md#marketosourcepropertiestypedef)
- [MatchingRuleOutputTypeDef](./type_defs.md#matchingruleoutputtypedef)
- [MatchingRuleTypeDef](./type_defs.md#matchingruletypedef)
- [ObjectTypeKeyTypeDef](./type_defs.md#objecttypekeytypedef)
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
- [DeleteDomainResponseTypeDef](./type_defs.md#deletedomainresponsetypedef)
- [DeleteIntegrationResponseTypeDef](./type_defs.md#deleteintegrationresponsetypedef)
- [DeleteProfileKeyResponseTypeDef](./type_defs.md#deleteprofilekeyresponsetypedef)
- [DeleteProfileObjectResponseTypeDef](./type_defs.md#deleteprofileobjectresponsetypedef)
- [DeleteProfileObjectTypeResponseTypeDef](./type_defs.md#deleteprofileobjecttyperesponsetypedef)
- [DeleteProfileResponseTypeDef](./type_defs.md#deleteprofileresponsetypedef)
- [GetAutoMergingPreviewResponseTypeDef](./type_defs.md#getautomergingpreviewresponsetypedef)
- [GetCalculatedAttributeForProfileResponseTypeDef](./type_defs.md#getcalculatedattributeforprofileresponsetypedef)
- [GetIntegrationResponseTypeDef](./type_defs.md#getintegrationresponsetypedef)
- [GetSimilarProfilesResponseTypeDef](./type_defs.md#getsimilarprofilesresponsetypedef)
- [ListRuleBasedMatchesResponseTypeDef](./type_defs.md#listrulebasedmatchesresponsetypedef)
- [ListTagsForResourceResponseTypeDef](./type_defs.md#listtagsforresourceresponsetypedef)
- [MergeProfilesResponseTypeDef](./type_defs.md#mergeprofilesresponsetypedef)
- [PutIntegrationResponseTypeDef](./type_defs.md#putintegrationresponsetypedef)
- [PutProfileObjectResponseTypeDef](./type_defs.md#putprofileobjectresponsetypedef)
- [UpdateProfileResponseTypeDef](./type_defs.md#updateprofileresponsetypedef)
- [SearchProfilesRequestRequestTypeDef](./type_defs.md#searchprofilesrequestrequesttypedef)
- [CreateProfileRequestRequestTypeDef](./type_defs.md#createprofilerequestrequesttypedef)
- [WorkflowAttributesTypeDef](./type_defs.md#workflowattributestypedef)
- [WorkflowMetricsTypeDef](./type_defs.md#workflowmetricstypedef)
- [WorkflowStepItemTypeDef](./type_defs.md#workflowstepitemtypedef)
- [AttributeDetailsOutputTypeDef](./type_defs.md#attributedetailsoutputtypedef)
- [AttributeDetailsTypeDef](./type_defs.md#attributedetailstypedef)
- [AttributeTypesSelectorUnionTypeDef](./type_defs.md#attributetypesselectoruniontypedef)
- [AutoMergingOutputTypeDef](./type_defs.md#automergingoutputtypedef)
- [BatchTypeDef](./type_defs.md#batchtypedef)
- [ListWorkflowsRequestRequestTypeDef](./type_defs.md#listworkflowsrequestrequesttypedef)
- [ScheduledTriggerPropertiesTypeDef](./type_defs.md#scheduledtriggerpropertiestypedef)
- [ConditionsTypeDef](./type_defs.md#conditionstypedef)
- [TaskTypeDef](./type_defs.md#tasktypedef)
- [ConsolidationUnionTypeDef](./type_defs.md#consolidationuniontypedef)
- [GetAutoMergingPreviewRequestRequestTypeDef](./type_defs.md#getautomergingpreviewrequestrequesttypedef)
- [EventStreamSummaryTypeDef](./type_defs.md#eventstreamsummarytypedef)
- [DetectedProfileObjectTypeTypeDef](./type_defs.md#detectedprofileobjecttypetypedef)
- [GetProfileObjectTypeResponseTypeDef](./type_defs.md#getprofileobjecttyperesponsetypedef)
- [GetProfileObjectTypeTemplateResponseTypeDef](./type_defs.md#getprofileobjecttypetemplateresponsetypedef)
- [PutProfileObjectTypeResponseTypeDef](./type_defs.md#putprofileobjecttyperesponsetypedef)
- [GetEventStreamResponseTypeDef](./type_defs.md#geteventstreamresponsetypedef)
- [ExportingConfigTypeDef](./type_defs.md#exportingconfigtypedef)
- [ExportingLocationTypeDef](./type_defs.md#exportinglocationtypedef)
- [MergeProfilesRequestRequestTypeDef](./type_defs.md#mergeprofilesrequestrequesttypedef)
- [ProfileTypeDef](./type_defs.md#profiletypedef)
- [GetMatchesResponseTypeDef](./type_defs.md#getmatchesresponsetypedef)
- [ListAccountIntegrationsResponseTypeDef](./type_defs.md#listaccountintegrationsresponsetypedef)
- [ListIntegrationsResponseTypeDef](./type_defs.md#listintegrationsresponsetypedef)
- [ListCalculatedAttributeDefinitionsResponseTypeDef](./type_defs.md#listcalculatedattributedefinitionsresponsetypedef)
- [ListCalculatedAttributesForProfileResponseTypeDef](./type_defs.md#listcalculatedattributesforprofileresponsetypedef)
- [ListDomainsResponseTypeDef](./type_defs.md#listdomainsresponsetypedef)
- [ListEventStreamsRequestListEventStreamsPaginateTypeDef](./type_defs.md#listeventstreamsrequestlisteventstreamspaginatetypedef)
- [ListProfileObjectTypesResponseTypeDef](./type_defs.md#listprofileobjecttypesresponsetypedef)
- [ListProfileObjectTypeTemplatesResponseTypeDef](./type_defs.md#listprofileobjecttypetemplatesresponsetypedef)
- [ListProfileObjectsResponseTypeDef](./type_defs.md#listprofileobjectsresponsetypedef)
- [ListProfileObjectsRequestRequestTypeDef](./type_defs.md#listprofileobjectsrequestrequesttypedef)
- [ListWorkflowsResponseTypeDef](./type_defs.md#listworkflowsresponsetypedef)
- [MatchingRuleUnionTypeDef](./type_defs.md#matchingruleuniontypedef)
- [ObjectTypeKeyUnionTypeDef](./type_defs.md#objecttypekeyuniontypedef)
- [SourceConnectorPropertiesTypeDef](./type_defs.md#sourceconnectorpropertiestypedef)
- [UpdateProfileRequestRequestTypeDef](./type_defs.md#updateprofilerequestrequesttypedef)
- [GetWorkflowResponseTypeDef](./type_defs.md#getworkflowresponsetypedef)
- [GetWorkflowStepsResponseTypeDef](./type_defs.md#getworkflowstepsresponsetypedef)
- [TriggerPropertiesTypeDef](./type_defs.md#triggerpropertiestypedef)
- [CreateCalculatedAttributeDefinitionRequestRequestTypeDef](./type_defs.md#createcalculatedattributedefinitionrequestrequesttypedef)
- [CreateCalculatedAttributeDefinitionResponseTypeDef](./type_defs.md#createcalculatedattributedefinitionresponsetypedef)
- [GetCalculatedAttributeDefinitionResponseTypeDef](./type_defs.md#getcalculatedattributedefinitionresponsetypedef)
- [UpdateCalculatedAttributeDefinitionRequestRequestTypeDef](./type_defs.md#updatecalculatedattributedefinitionrequestrequesttypedef)
- [UpdateCalculatedAttributeDefinitionResponseTypeDef](./type_defs.md#updatecalculatedattributedefinitionresponsetypedef)
- [AutoMergingTypeDef](./type_defs.md#automergingtypedef)
- [ListEventStreamsResponseTypeDef](./type_defs.md#listeventstreamsresponsetypedef)
- [DetectProfileObjectTypeResponseTypeDef](./type_defs.md#detectprofileobjecttyperesponsetypedef)
- [MatchingResponseTypeDef](./type_defs.md#matchingresponsetypedef)
- [RuleBasedMatchingResponseTypeDef](./type_defs.md#rulebasedmatchingresponsetypedef)
- [GetIdentityResolutionJobResponseTypeDef](./type_defs.md#getidentityresolutionjobresponsetypedef)
- [IdentityResolutionJobTypeDef](./type_defs.md#identityresolutionjobtypedef)
- [SearchProfilesResponseTypeDef](./type_defs.md#searchprofilesresponsetypedef)
- [RuleBasedMatchingRequestTypeDef](./type_defs.md#rulebasedmatchingrequesttypedef)
- [PutProfileObjectTypeRequestRequestTypeDef](./type_defs.md#putprofileobjecttyperequestrequesttypedef)
- [SourceFlowConfigTypeDef](./type_defs.md#sourceflowconfigtypedef)
- [TriggerConfigTypeDef](./type_defs.md#triggerconfigtypedef)
- [AutoMergingUnionTypeDef](./type_defs.md#automerginguniontypedef)
- [CreateDomainResponseTypeDef](./type_defs.md#createdomainresponsetypedef)
- [GetDomainResponseTypeDef](./type_defs.md#getdomainresponsetypedef)
- [UpdateDomainResponseTypeDef](./type_defs.md#updatedomainresponsetypedef)
- [ListIdentityResolutionJobsResponseTypeDef](./type_defs.md#listidentityresolutionjobsresponsetypedef)
- [FlowDefinitionTypeDef](./type_defs.md#flowdefinitiontypedef)
- [MatchingRequestTypeDef](./type_defs.md#matchingrequesttypedef)
- [AppflowIntegrationTypeDef](./type_defs.md#appflowintegrationtypedef)
- [PutIntegrationRequestRequestTypeDef](./type_defs.md#putintegrationrequestrequesttypedef)
- [CreateDomainRequestRequestTypeDef](./type_defs.md#createdomainrequestrequesttypedef)
- [UpdateDomainRequestRequestTypeDef](./type_defs.md#updatedomainrequestrequesttypedef)
- [IntegrationConfigTypeDef](./type_defs.md#integrationconfigtypedef)
- [CreateIntegrationWorkflowRequestRequestTypeDef](./type_defs.md#createintegrationworkflowrequestrequesttypedef)

