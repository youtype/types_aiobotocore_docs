# CleanRoomsService module

> [Index](../README.md) > CleanRoomsService


!!! note ""

    Auto-generated documentation for [CleanRoomsService](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cleanrooms.html#CleanRoomsService)
    type annotations stubs module [types-aiobotocore-cleanrooms](https://pypi.org/project/types-aiobotocore-cleanrooms/).

## How to install



### From PyPI with pip

Install `types-aiobotocore` for `CleanRoomsService` service.

```bash
# install with aiobotocore type annotations
python -m pip install 'types-aiobotocore[cleanrooms]'


# Lite version does not provide session.client/resource overloads
# it is more RAM-friendly, but requires explicit type annotations
python -m pip install 'types-aiobotocore-lite[cleanrooms]'


# standalone installation
python -m pip install types-aiobotocore-cleanrooms
```



## How to uninstall

```bash
python -m pip uninstall -y types-aiobotocore-cleanrooms
```

## Usage

Code samples can be found in [Examples](./usage.md).

## CleanRoomsServiceClient

Type annotations and code completion for  `#!python session.create_client("cleanrooms")` as [CleanRoomsServiceClient](./client.md)
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cleanrooms.html#CleanRoomsService.Client)

```python
# CleanRoomsServiceClient usage example

from aiobotocore.session import get_session

from types_aiobotocore_cleanrooms.client import CleanRoomsServiceClient


session = get_session()
async with session.create_client("cleanrooms") as client:
    client: CleanRoomsServiceClient
```


## Paginators

Type annotations and code completion for
[paginators](./paginators.md)
from `#!python session.create_client("cleanrooms").get_paginator("...")`.

```python
# ListAnalysisTemplatesPaginator usage example

from types_aiobotocore_cleanrooms.paginator import ListAnalysisTemplatesPaginator

def get_list_analysis_templates_paginator() -> ListAnalysisTemplatesPaginator:
    return client.get_paginator("list_analysis_templates"))
```

- [ListAnalysisTemplatesPaginator](./paginators.md#listanalysistemplatespaginator)
- [ListCollaborationAnalysisTemplatesPaginator](./paginators.md#listcollaborationanalysistemplatespaginator)
- [ListCollaborationConfiguredAudienceModelAssociationsPaginator](./paginators.md#listcollaborationconfiguredaudiencemodelassociationspaginator)
- [ListCollaborationIdNamespaceAssociationsPaginator](./paginators.md#listcollaborationidnamespaceassociationspaginator)
- [ListCollaborationPrivacyBudgetTemplatesPaginator](./paginators.md#listcollaborationprivacybudgettemplatespaginator)
- [ListCollaborationPrivacyBudgetsPaginator](./paginators.md#listcollaborationprivacybudgetspaginator)
- [ListCollaborationsPaginator](./paginators.md#listcollaborationspaginator)
- [ListConfiguredAudienceModelAssociationsPaginator](./paginators.md#listconfiguredaudiencemodelassociationspaginator)
- [ListConfiguredTableAssociationsPaginator](./paginators.md#listconfiguredtableassociationspaginator)
- [ListConfiguredTablesPaginator](./paginators.md#listconfiguredtablespaginator)
- [ListIdMappingTablesPaginator](./paginators.md#listidmappingtablespaginator)
- [ListIdNamespaceAssociationsPaginator](./paginators.md#listidnamespaceassociationspaginator)
- [ListMembersPaginator](./paginators.md#listmemberspaginator)
- [ListMembershipsPaginator](./paginators.md#listmembershipspaginator)
- [ListPrivacyBudgetTemplatesPaginator](./paginators.md#listprivacybudgettemplatespaginator)
- [ListPrivacyBudgetsPaginator](./paginators.md#listprivacybudgetspaginator)
- [ListProtectedQueriesPaginator](./paginators.md#listprotectedqueriespaginator)
- [ListSchemasPaginator](./paginators.md#listschemaspaginator)








## Literals

Type annotations for [literals](./literals.md) used in methods and schema.

```python
# AdditionalAnalysesType usage example

from types_aiobotocore_cleanrooms.literals import AdditionalAnalysesType

def get_value() -> AdditionalAnalysesType:
    return "ALLOWED"
```

- [AdditionalAnalysesType](./literals.md#additionalanalysestype)
- [AggregateFunctionNameType](./literals.md#aggregatefunctionnametype)
- [AggregationTypeType](./literals.md#aggregationtypetype)
- [AnalysisFormatType](./literals.md#analysisformattype)
- [AnalysisMethodType](./literals.md#analysismethodtype)
- [AnalysisRuleTypeType](./literals.md#analysisruletypetype)
- [AnalysisTemplateValidationStatusType](./literals.md#analysistemplatevalidationstatustype)
- [AnalysisTemplateValidationTypeType](./literals.md#analysistemplatevalidationtypetype)
- [AnalysisTypeType](./literals.md#analysistypetype)
- [CollaborationQueryLogStatusType](./literals.md#collaborationquerylogstatustype)
- [ConfiguredTableAnalysisRuleTypeType](./literals.md#configuredtableanalysisruletypetype)
- [ConfiguredTableAssociationAnalysisRuleTypeType](./literals.md#configuredtableassociationanalysisruletypetype)
- [DifferentialPrivacyAggregationTypeType](./literals.md#differentialprivacyaggregationtypetype)
- [FilterableMemberStatusType](./literals.md#filterablememberstatustype)
- [IdNamespaceTypeType](./literals.md#idnamespacetypetype)
- [JoinOperatorType](./literals.md#joinoperatortype)
- [JoinRequiredOptionType](./literals.md#joinrequiredoptiontype)
- [ListAnalysisTemplatesPaginatorName](./literals.md#listanalysistemplatespaginatorname)
- [ListCollaborationAnalysisTemplatesPaginatorName](./literals.md#listcollaborationanalysistemplatespaginatorname)
- [ListCollaborationConfiguredAudienceModelAssociationsPaginatorName](./literals.md#listcollaborationconfiguredaudiencemodelassociationspaginatorname)
- [ListCollaborationIdNamespaceAssociationsPaginatorName](./literals.md#listcollaborationidnamespaceassociationspaginatorname)
- [ListCollaborationPrivacyBudgetTemplatesPaginatorName](./literals.md#listcollaborationprivacybudgettemplatespaginatorname)
- [ListCollaborationPrivacyBudgetsPaginatorName](./literals.md#listcollaborationprivacybudgetspaginatorname)
- [ListCollaborationsPaginatorName](./literals.md#listcollaborationspaginatorname)
- [ListConfiguredAudienceModelAssociationsPaginatorName](./literals.md#listconfiguredaudiencemodelassociationspaginatorname)
- [ListConfiguredTableAssociationsPaginatorName](./literals.md#listconfiguredtableassociationspaginatorname)
- [ListConfiguredTablesPaginatorName](./literals.md#listconfiguredtablespaginatorname)
- [ListIdMappingTablesPaginatorName](./literals.md#listidmappingtablespaginatorname)
- [ListIdNamespaceAssociationsPaginatorName](./literals.md#listidnamespaceassociationspaginatorname)
- [ListMembersPaginatorName](./literals.md#listmemberspaginatorname)
- [ListMembershipsPaginatorName](./literals.md#listmembershipspaginatorname)
- [ListPrivacyBudgetTemplatesPaginatorName](./literals.md#listprivacybudgettemplatespaginatorname)
- [ListPrivacyBudgetsPaginatorName](./literals.md#listprivacybudgetspaginatorname)
- [ListProtectedQueriesPaginatorName](./literals.md#listprotectedqueriespaginatorname)
- [ListSchemasPaginatorName](./literals.md#listschemaspaginatorname)
- [MemberAbilityType](./literals.md#memberabilitytype)
- [MemberStatusType](./literals.md#memberstatustype)
- [MembershipQueryLogStatusType](./literals.md#membershipquerylogstatustype)
- [MembershipStatusType](./literals.md#membershipstatustype)
- [ParameterTypeType](./literals.md#parametertypetype)
- [PrivacyBudgetTemplateAutoRefreshType](./literals.md#privacybudgettemplateautorefreshtype)
- [PrivacyBudgetTypeType](./literals.md#privacybudgettypetype)
- [ProtectedQueryStatusType](./literals.md#protectedquerystatustype)
- [ProtectedQueryTypeType](./literals.md#protectedquerytypetype)
- [ResultFormatType](./literals.md#resultformattype)
- [ScalarFunctionsType](./literals.md#scalarfunctionstype)
- [SchemaConfigurationType](./literals.md#schemaconfigurationtype)
- [SchemaStatusReasonCodeType](./literals.md#schemastatusreasoncodetype)
- [SchemaStatusType](./literals.md#schemastatustype)
- [SchemaTypeType](./literals.md#schematypetype)
- [TargetProtectedQueryStatusType](./literals.md#targetprotectedquerystatustype)
- [CleanRoomsServiceServiceName](./literals.md#cleanroomsserviceservicename)
- [ServiceName](./literals.md#servicename)
- [ResourceServiceName](./literals.md#resourceservicename)
- [PaginatorName](./literals.md#paginatorname)
- [RegionName](./literals.md#regionname)




## Type definitions

Type annotations for [type definitions](./type_defs.md) used in methods and schema.

- [AggregateColumnOutputTypeDef](./type_defs.md#aggregatecolumnoutputtypedef)
- [AggregateColumnTypeDef](./type_defs.md#aggregatecolumntypedef)
- [AggregationConstraintTypeDef](./type_defs.md#aggregationconstrainttypedef)
- [AnalysisParameterTypeDef](./type_defs.md#analysisparametertypedef)
- [AnalysisRuleListOutputTypeDef](./type_defs.md#analysisrulelistoutputtypedef)
- [AnalysisRuleListTypeDef](./type_defs.md#analysisrulelisttypedef)
- [AnalysisSchemaTypeDef](./type_defs.md#analysisschematypedef)
- [AnalysisSourceTypeDef](./type_defs.md#analysissourcetypedef)
- [AnalysisTemplateSummaryTypeDef](./type_defs.md#analysistemplatesummarytypedef)
- [AnalysisTemplateValidationStatusReasonTypeDef](./type_defs.md#analysistemplatevalidationstatusreasontypedef)
- [BatchGetCollaborationAnalysisTemplateErrorTypeDef](./type_defs.md#batchgetcollaborationanalysistemplateerrortypedef)
- [BatchGetCollaborationAnalysisTemplateInputRequestTypeDef](./type_defs.md#batchgetcollaborationanalysistemplateinputrequesttypedef)
- [ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef)
- [BatchGetSchemaAnalysisRuleErrorTypeDef](./type_defs.md#batchgetschemaanalysisruleerrortypedef)
- [SchemaAnalysisRuleRequestTypeDef](./type_defs.md#schemaanalysisrulerequesttypedef)
- [BatchGetSchemaErrorTypeDef](./type_defs.md#batchgetschemaerrortypedef)
- [BatchGetSchemaInputRequestTypeDef](./type_defs.md#batchgetschemainputrequesttypedef)
- [CollaborationAnalysisTemplateSummaryTypeDef](./type_defs.md#collaborationanalysistemplatesummarytypedef)
- [CollaborationConfiguredAudienceModelAssociationSummaryTypeDef](./type_defs.md#collaborationconfiguredaudiencemodelassociationsummarytypedef)
- [CollaborationConfiguredAudienceModelAssociationTypeDef](./type_defs.md#collaborationconfiguredaudiencemodelassociationtypedef)
- [IdNamespaceAssociationInputReferenceConfigTypeDef](./type_defs.md#idnamespaceassociationinputreferenceconfigtypedef)
- [IdNamespaceAssociationInputReferencePropertiesSummaryTypeDef](./type_defs.md#idnamespaceassociationinputreferencepropertiessummarytypedef)
- [IdMappingConfigTypeDef](./type_defs.md#idmappingconfigtypedef)
- [IdNamespaceAssociationInputReferencePropertiesTypeDef](./type_defs.md#idnamespaceassociationinputreferencepropertiestypedef)
- [CollaborationPrivacyBudgetTemplateSummaryTypeDef](./type_defs.md#collaborationprivacybudgettemplatesummarytypedef)
- [CollaborationSummaryTypeDef](./type_defs.md#collaborationsummarytypedef)
- [DataEncryptionMetadataTypeDef](./type_defs.md#dataencryptionmetadatatypedef)
- [ColumnTypeDef](./type_defs.md#columntypedef)
- [DirectAnalysisConfigurationDetailsTypeDef](./type_defs.md#directanalysisconfigurationdetailstypedef)
- [ConfiguredAudienceModelAssociationSummaryTypeDef](./type_defs.md#configuredaudiencemodelassociationsummarytypedef)
- [ConfiguredAudienceModelAssociationTypeDef](./type_defs.md#configuredaudiencemodelassociationtypedef)
- [ConfiguredTableAssociationAnalysisRuleAggregationOutputTypeDef](./type_defs.md#configuredtableassociationanalysisruleaggregationoutputtypedef)
- [ConfiguredTableAssociationAnalysisRuleAggregationTypeDef](./type_defs.md#configuredtableassociationanalysisruleaggregationtypedef)
- [ConfiguredTableAssociationAnalysisRuleCustomOutputTypeDef](./type_defs.md#configuredtableassociationanalysisrulecustomoutputtypedef)
- [ConfiguredTableAssociationAnalysisRuleCustomTypeDef](./type_defs.md#configuredtableassociationanalysisrulecustomtypedef)
- [ConfiguredTableAssociationAnalysisRuleListOutputTypeDef](./type_defs.md#configuredtableassociationanalysisrulelistoutputtypedef)
- [ConfiguredTableAssociationAnalysisRuleListTypeDef](./type_defs.md#configuredtableassociationanalysisrulelisttypedef)
- [ConfiguredTableAssociationSummaryTypeDef](./type_defs.md#configuredtableassociationsummarytypedef)
- [ConfiguredTableAssociationTypeDef](./type_defs.md#configuredtableassociationtypedef)
- [ConfiguredTableSummaryTypeDef](./type_defs.md#configuredtablesummarytypedef)
- [CreateConfiguredAudienceModelAssociationInputRequestTypeDef](./type_defs.md#createconfiguredaudiencemodelassociationinputrequesttypedef)
- [CreateConfiguredTableAssociationInputRequestTypeDef](./type_defs.md#createconfiguredtableassociationinputrequesttypedef)
- [IdMappingTableInputReferenceConfigTypeDef](./type_defs.md#idmappingtableinputreferenceconfigtypedef)
- [DeleteAnalysisTemplateInputRequestTypeDef](./type_defs.md#deleteanalysistemplateinputrequesttypedef)
- [DeleteCollaborationInputRequestTypeDef](./type_defs.md#deletecollaborationinputrequesttypedef)
- [DeleteConfiguredAudienceModelAssociationInputRequestTypeDef](./type_defs.md#deleteconfiguredaudiencemodelassociationinputrequesttypedef)
- [DeleteConfiguredTableAnalysisRuleInputRequestTypeDef](./type_defs.md#deleteconfiguredtableanalysisruleinputrequesttypedef)
- [DeleteConfiguredTableAssociationAnalysisRuleInputRequestTypeDef](./type_defs.md#deleteconfiguredtableassociationanalysisruleinputrequesttypedef)
- [DeleteConfiguredTableAssociationInputRequestTypeDef](./type_defs.md#deleteconfiguredtableassociationinputrequesttypedef)
- [DeleteConfiguredTableInputRequestTypeDef](./type_defs.md#deleteconfiguredtableinputrequesttypedef)
- [DeleteIdMappingTableInputRequestTypeDef](./type_defs.md#deleteidmappingtableinputrequesttypedef)
- [DeleteIdNamespaceAssociationInputRequestTypeDef](./type_defs.md#deleteidnamespaceassociationinputrequesttypedef)
- [DeleteMemberInputRequestTypeDef](./type_defs.md#deletememberinputrequesttypedef)
- [DeleteMembershipInputRequestTypeDef](./type_defs.md#deletemembershipinputrequesttypedef)
- [DeletePrivacyBudgetTemplateInputRequestTypeDef](./type_defs.md#deleteprivacybudgettemplateinputrequesttypedef)
- [DifferentialPrivacyColumnTypeDef](./type_defs.md#differentialprivacycolumntypedef)
- [DifferentialPrivacySensitivityParametersTypeDef](./type_defs.md#differentialprivacysensitivityparameterstypedef)
- [DifferentialPrivacyPreviewAggregationTypeDef](./type_defs.md#differentialprivacypreviewaggregationtypedef)
- [DifferentialPrivacyPreviewParametersInputTypeDef](./type_defs.md#differentialprivacypreviewparametersinputtypedef)
- [DifferentialPrivacyPrivacyBudgetAggregationTypeDef](./type_defs.md#differentialprivacyprivacybudgetaggregationtypedef)
- [DifferentialPrivacyTemplateParametersInputTypeDef](./type_defs.md#differentialprivacytemplateparametersinputtypedef)
- [DifferentialPrivacyTemplateParametersOutputTypeDef](./type_defs.md#differentialprivacytemplateparametersoutputtypedef)
- [DifferentialPrivacyTemplateUpdateParametersTypeDef](./type_defs.md#differentialprivacytemplateupdateparameterstypedef)
- [GetAnalysisTemplateInputRequestTypeDef](./type_defs.md#getanalysistemplateinputrequesttypedef)
- [GetCollaborationAnalysisTemplateInputRequestTypeDef](./type_defs.md#getcollaborationanalysistemplateinputrequesttypedef)
- [GetCollaborationConfiguredAudienceModelAssociationInputRequestTypeDef](./type_defs.md#getcollaborationconfiguredaudiencemodelassociationinputrequesttypedef)
- [GetCollaborationIdNamespaceAssociationInputRequestTypeDef](./type_defs.md#getcollaborationidnamespaceassociationinputrequesttypedef)
- [GetCollaborationInputRequestTypeDef](./type_defs.md#getcollaborationinputrequesttypedef)
- [GetCollaborationPrivacyBudgetTemplateInputRequestTypeDef](./type_defs.md#getcollaborationprivacybudgettemplateinputrequesttypedef)
- [GetConfiguredAudienceModelAssociationInputRequestTypeDef](./type_defs.md#getconfiguredaudiencemodelassociationinputrequesttypedef)
- [GetConfiguredTableAnalysisRuleInputRequestTypeDef](./type_defs.md#getconfiguredtableanalysisruleinputrequesttypedef)
- [GetConfiguredTableAssociationAnalysisRuleInputRequestTypeDef](./type_defs.md#getconfiguredtableassociationanalysisruleinputrequesttypedef)
- [GetConfiguredTableAssociationInputRequestTypeDef](./type_defs.md#getconfiguredtableassociationinputrequesttypedef)
- [GetConfiguredTableInputRequestTypeDef](./type_defs.md#getconfiguredtableinputrequesttypedef)
- [GetIdMappingTableInputRequestTypeDef](./type_defs.md#getidmappingtableinputrequesttypedef)
- [GetIdNamespaceAssociationInputRequestTypeDef](./type_defs.md#getidnamespaceassociationinputrequesttypedef)
- [GetMembershipInputRequestTypeDef](./type_defs.md#getmembershipinputrequesttypedef)
- [GetPrivacyBudgetTemplateInputRequestTypeDef](./type_defs.md#getprivacybudgettemplateinputrequesttypedef)
- [GetProtectedQueryInputRequestTypeDef](./type_defs.md#getprotectedqueryinputrequesttypedef)
- [GetSchemaAnalysisRuleInputRequestTypeDef](./type_defs.md#getschemaanalysisruleinputrequesttypedef)
- [GetSchemaInputRequestTypeDef](./type_defs.md#getschemainputrequesttypedef)
- [GlueTableReferenceTypeDef](./type_defs.md#gluetablereferencetypedef)
- [IdMappingTableInputSourceTypeDef](./type_defs.md#idmappingtableinputsourcetypedef)
- [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
- [ListAnalysisTemplatesInputRequestTypeDef](./type_defs.md#listanalysistemplatesinputrequesttypedef)
- [ListCollaborationAnalysisTemplatesInputRequestTypeDef](./type_defs.md#listcollaborationanalysistemplatesinputrequesttypedef)
- [ListCollaborationConfiguredAudienceModelAssociationsInputRequestTypeDef](./type_defs.md#listcollaborationconfiguredaudiencemodelassociationsinputrequesttypedef)
- [ListCollaborationIdNamespaceAssociationsInputRequestTypeDef](./type_defs.md#listcollaborationidnamespaceassociationsinputrequesttypedef)
- [ListCollaborationPrivacyBudgetTemplatesInputRequestTypeDef](./type_defs.md#listcollaborationprivacybudgettemplatesinputrequesttypedef)
- [ListCollaborationPrivacyBudgetsInputRequestTypeDef](./type_defs.md#listcollaborationprivacybudgetsinputrequesttypedef)
- [ListCollaborationsInputRequestTypeDef](./type_defs.md#listcollaborationsinputrequesttypedef)
- [ListConfiguredAudienceModelAssociationsInputRequestTypeDef](./type_defs.md#listconfiguredaudiencemodelassociationsinputrequesttypedef)
- [ListConfiguredTableAssociationsInputRequestTypeDef](./type_defs.md#listconfiguredtableassociationsinputrequesttypedef)
- [ListConfiguredTablesInputRequestTypeDef](./type_defs.md#listconfiguredtablesinputrequesttypedef)
- [ListIdMappingTablesInputRequestTypeDef](./type_defs.md#listidmappingtablesinputrequesttypedef)
- [ListIdNamespaceAssociationsInputRequestTypeDef](./type_defs.md#listidnamespaceassociationsinputrequesttypedef)
- [ListMembersInputRequestTypeDef](./type_defs.md#listmembersinputrequesttypedef)
- [ListMembershipsInputRequestTypeDef](./type_defs.md#listmembershipsinputrequesttypedef)
- [ListPrivacyBudgetTemplatesInputRequestTypeDef](./type_defs.md#listprivacybudgettemplatesinputrequesttypedef)
- [PrivacyBudgetTemplateSummaryTypeDef](./type_defs.md#privacybudgettemplatesummarytypedef)
- [ListPrivacyBudgetsInputRequestTypeDef](./type_defs.md#listprivacybudgetsinputrequesttypedef)
- [ListProtectedQueriesInputRequestTypeDef](./type_defs.md#listprotectedqueriesinputrequesttypedef)
- [ListSchemasInputRequestTypeDef](./type_defs.md#listschemasinputrequesttypedef)
- [SchemaSummaryTypeDef](./type_defs.md#schemasummarytypedef)
- [ListTagsForResourceInputRequestTypeDef](./type_defs.md#listtagsforresourceinputrequesttypedef)
- [MembershipQueryComputePaymentConfigTypeDef](./type_defs.md#membershipquerycomputepaymentconfigtypedef)
- [ProtectedQueryS3OutputConfigurationTypeDef](./type_defs.md#protectedquerys3outputconfigurationtypedef)
- [QueryComputePaymentConfigTypeDef](./type_defs.md#querycomputepaymentconfigtypedef)
- [PopulateIdMappingTableInputRequestTypeDef](./type_defs.md#populateidmappingtableinputrequesttypedef)
- [ProtectedQueryErrorTypeDef](./type_defs.md#protectedqueryerrortypedef)
- [ProtectedQueryMemberOutputConfigurationTypeDef](./type_defs.md#protectedquerymemberoutputconfigurationtypedef)
- [ProtectedQueryS3OutputTypeDef](./type_defs.md#protectedquerys3outputtypedef)
- [ProtectedQuerySingleMemberOutputTypeDef](./type_defs.md#protectedquerysinglememberoutputtypedef)
- [ProtectedQuerySQLParametersOutputTypeDef](./type_defs.md#protectedquerysqlparametersoutputtypedef)
- [ProtectedQuerySQLParametersTypeDef](./type_defs.md#protectedquerysqlparameterstypedef)
- [ProtectedQueryStatisticsTypeDef](./type_defs.md#protectedquerystatisticstypedef)
- [QueryConstraintRequireOverlapTypeDef](./type_defs.md#queryconstraintrequireoverlaptypedef)
- [SchemaStatusReasonTypeDef](./type_defs.md#schemastatusreasontypedef)
- [TagResourceInputRequestTypeDef](./type_defs.md#tagresourceinputrequesttypedef)
- [UntagResourceInputRequestTypeDef](./type_defs.md#untagresourceinputrequesttypedef)
- [UpdateAnalysisTemplateInputRequestTypeDef](./type_defs.md#updateanalysistemplateinputrequesttypedef)
- [UpdateCollaborationInputRequestTypeDef](./type_defs.md#updatecollaborationinputrequesttypedef)
- [UpdateConfiguredAudienceModelAssociationInputRequestTypeDef](./type_defs.md#updateconfiguredaudiencemodelassociationinputrequesttypedef)
- [UpdateConfiguredTableAssociationInputRequestTypeDef](./type_defs.md#updateconfiguredtableassociationinputrequesttypedef)
- [UpdateConfiguredTableInputRequestTypeDef](./type_defs.md#updateconfiguredtableinputrequesttypedef)
- [UpdateIdMappingTableInputRequestTypeDef](./type_defs.md#updateidmappingtableinputrequesttypedef)
- [UpdateProtectedQueryInputRequestTypeDef](./type_defs.md#updateprotectedqueryinputrequesttypedef)
- [AggregateColumnUnionTypeDef](./type_defs.md#aggregatecolumnuniontypedef)
- [AnalysisRuleAggregationOutputTypeDef](./type_defs.md#analysisruleaggregationoutputtypedef)
- [AnalysisRuleListUnionTypeDef](./type_defs.md#analysisrulelistuniontypedef)
- [CreateAnalysisTemplateInputRequestTypeDef](./type_defs.md#createanalysistemplateinputrequesttypedef)
- [AnalysisTemplateValidationStatusDetailTypeDef](./type_defs.md#analysistemplatevalidationstatusdetailtypedef)
- [ListAnalysisTemplatesOutputTypeDef](./type_defs.md#listanalysistemplatesoutputtypedef)
- [ListTagsForResourceOutputTypeDef](./type_defs.md#listtagsforresourceoutputtypedef)
- [PopulateIdMappingTableOutputTypeDef](./type_defs.md#populateidmappingtableoutputtypedef)
- [BatchGetSchemaAnalysisRuleInputRequestTypeDef](./type_defs.md#batchgetschemaanalysisruleinputrequesttypedef)
- [ListCollaborationAnalysisTemplatesOutputTypeDef](./type_defs.md#listcollaborationanalysistemplatesoutputtypedef)
- [ListCollaborationConfiguredAudienceModelAssociationsOutputTypeDef](./type_defs.md#listcollaborationconfiguredaudiencemodelassociationsoutputtypedef)
- [GetCollaborationConfiguredAudienceModelAssociationOutputTypeDef](./type_defs.md#getcollaborationconfiguredaudiencemodelassociationoutputtypedef)
- [CollaborationIdNamespaceAssociationSummaryTypeDef](./type_defs.md#collaborationidnamespaceassociationsummarytypedef)
- [IdNamespaceAssociationSummaryTypeDef](./type_defs.md#idnamespaceassociationsummarytypedef)
- [CreateIdNamespaceAssociationInputRequestTypeDef](./type_defs.md#createidnamespaceassociationinputrequesttypedef)
- [UpdateIdNamespaceAssociationInputRequestTypeDef](./type_defs.md#updateidnamespaceassociationinputrequesttypedef)
- [CollaborationIdNamespaceAssociationTypeDef](./type_defs.md#collaborationidnamespaceassociationtypedef)
- [IdNamespaceAssociationTypeDef](./type_defs.md#idnamespaceassociationtypedef)
- [ListCollaborationPrivacyBudgetTemplatesOutputTypeDef](./type_defs.md#listcollaborationprivacybudgettemplatesoutputtypedef)
- [ListCollaborationsOutputTypeDef](./type_defs.md#listcollaborationsoutputtypedef)
- [CollaborationTypeDef](./type_defs.md#collaborationtypedef)
- [ConfigurationDetailsTypeDef](./type_defs.md#configurationdetailstypedef)
- [ListConfiguredAudienceModelAssociationsOutputTypeDef](./type_defs.md#listconfiguredaudiencemodelassociationsoutputtypedef)
- [CreateConfiguredAudienceModelAssociationOutputTypeDef](./type_defs.md#createconfiguredaudiencemodelassociationoutputtypedef)
- [GetConfiguredAudienceModelAssociationOutputTypeDef](./type_defs.md#getconfiguredaudiencemodelassociationoutputtypedef)
- [UpdateConfiguredAudienceModelAssociationOutputTypeDef](./type_defs.md#updateconfiguredaudiencemodelassociationoutputtypedef)
- [ConfiguredTableAssociationAnalysisRuleAggregationUnionTypeDef](./type_defs.md#configuredtableassociationanalysisruleaggregationuniontypedef)
- [ConfiguredTableAssociationAnalysisRuleCustomUnionTypeDef](./type_defs.md#configuredtableassociationanalysisrulecustomuniontypedef)
- [ConfiguredTableAssociationAnalysisRulePolicyV1OutputTypeDef](./type_defs.md#configuredtableassociationanalysisrulepolicyv1outputtypedef)
- [ConfiguredTableAssociationAnalysisRuleListUnionTypeDef](./type_defs.md#configuredtableassociationanalysisrulelistuniontypedef)
- [ListConfiguredTableAssociationsOutputTypeDef](./type_defs.md#listconfiguredtableassociationsoutputtypedef)
- [CreateConfiguredTableAssociationOutputTypeDef](./type_defs.md#createconfiguredtableassociationoutputtypedef)
- [GetConfiguredTableAssociationOutputTypeDef](./type_defs.md#getconfiguredtableassociationoutputtypedef)
- [UpdateConfiguredTableAssociationOutputTypeDef](./type_defs.md#updateconfiguredtableassociationoutputtypedef)
- [ListConfiguredTablesOutputTypeDef](./type_defs.md#listconfiguredtablesoutputtypedef)
- [CreateIdMappingTableInputRequestTypeDef](./type_defs.md#createidmappingtableinputrequesttypedef)
- [IdMappingTableSummaryTypeDef](./type_defs.md#idmappingtablesummarytypedef)
- [DifferentialPrivacyConfigurationOutputTypeDef](./type_defs.md#differentialprivacyconfigurationoutputtypedef)
- [DifferentialPrivacyConfigurationTypeDef](./type_defs.md#differentialprivacyconfigurationtypedef)
- [DifferentialPrivacyParametersTypeDef](./type_defs.md#differentialprivacyparameterstypedef)
- [DifferentialPrivacyPrivacyImpactTypeDef](./type_defs.md#differentialprivacyprivacyimpacttypedef)
- [PreviewPrivacyImpactParametersInputTypeDef](./type_defs.md#previewprivacyimpactparametersinputtypedef)
- [DifferentialPrivacyPrivacyBudgetTypeDef](./type_defs.md#differentialprivacyprivacybudgettypedef)
- [PrivacyBudgetTemplateParametersInputTypeDef](./type_defs.md#privacybudgettemplateparametersinputtypedef)
- [PrivacyBudgetTemplateParametersOutputTypeDef](./type_defs.md#privacybudgettemplateparametersoutputtypedef)
- [PrivacyBudgetTemplateUpdateParametersTypeDef](./type_defs.md#privacybudgettemplateupdateparameterstypedef)
- [TableReferenceTypeDef](./type_defs.md#tablereferencetypedef)
- [IdMappingTableInputReferencePropertiesTypeDef](./type_defs.md#idmappingtableinputreferencepropertiestypedef)
- [IdMappingTableSchemaTypePropertiesTypeDef](./type_defs.md#idmappingtableschematypepropertiestypedef)
- [ListAnalysisTemplatesInputListAnalysisTemplatesPaginateTypeDef](./type_defs.md#listanalysistemplatesinputlistanalysistemplatespaginatetypedef)
- [ListCollaborationAnalysisTemplatesInputListCollaborationAnalysisTemplatesPaginateTypeDef](./type_defs.md#listcollaborationanalysistemplatesinputlistcollaborationanalysistemplatespaginatetypedef)
- [ListCollaborationConfiguredAudienceModelAssociationsInputListCollaborationConfiguredAudienceModelAssociationsPaginateTypeDef](./type_defs.md#listcollaborationconfiguredaudiencemodelassociationsinputlistcollaborationconfiguredaudiencemodelassociationspaginatetypedef)
- [ListCollaborationIdNamespaceAssociationsInputListCollaborationIdNamespaceAssociationsPaginateTypeDef](./type_defs.md#listcollaborationidnamespaceassociationsinputlistcollaborationidnamespaceassociationspaginatetypedef)
- [ListCollaborationPrivacyBudgetTemplatesInputListCollaborationPrivacyBudgetTemplatesPaginateTypeDef](./type_defs.md#listcollaborationprivacybudgettemplatesinputlistcollaborationprivacybudgettemplatespaginatetypedef)
- [ListCollaborationPrivacyBudgetsInputListCollaborationPrivacyBudgetsPaginateTypeDef](./type_defs.md#listcollaborationprivacybudgetsinputlistcollaborationprivacybudgetspaginatetypedef)
- [ListCollaborationsInputListCollaborationsPaginateTypeDef](./type_defs.md#listcollaborationsinputlistcollaborationspaginatetypedef)
- [ListConfiguredAudienceModelAssociationsInputListConfiguredAudienceModelAssociationsPaginateTypeDef](./type_defs.md#listconfiguredaudiencemodelassociationsinputlistconfiguredaudiencemodelassociationspaginatetypedef)
- [ListConfiguredTableAssociationsInputListConfiguredTableAssociationsPaginateTypeDef](./type_defs.md#listconfiguredtableassociationsinputlistconfiguredtableassociationspaginatetypedef)
- [ListConfiguredTablesInputListConfiguredTablesPaginateTypeDef](./type_defs.md#listconfiguredtablesinputlistconfiguredtablespaginatetypedef)
- [ListIdMappingTablesInputListIdMappingTablesPaginateTypeDef](./type_defs.md#listidmappingtablesinputlistidmappingtablespaginatetypedef)
- [ListIdNamespaceAssociationsInputListIdNamespaceAssociationsPaginateTypeDef](./type_defs.md#listidnamespaceassociationsinputlistidnamespaceassociationspaginatetypedef)
- [ListMembersInputListMembersPaginateTypeDef](./type_defs.md#listmembersinputlistmemberspaginatetypedef)
- [ListMembershipsInputListMembershipsPaginateTypeDef](./type_defs.md#listmembershipsinputlistmembershipspaginatetypedef)
- [ListPrivacyBudgetTemplatesInputListPrivacyBudgetTemplatesPaginateTypeDef](./type_defs.md#listprivacybudgettemplatesinputlistprivacybudgettemplatespaginatetypedef)
- [ListPrivacyBudgetsInputListPrivacyBudgetsPaginateTypeDef](./type_defs.md#listprivacybudgetsinputlistprivacybudgetspaginatetypedef)
- [ListProtectedQueriesInputListProtectedQueriesPaginateTypeDef](./type_defs.md#listprotectedqueriesinputlistprotectedqueriespaginatetypedef)
- [ListSchemasInputListSchemasPaginateTypeDef](./type_defs.md#listschemasinputlistschemaspaginatetypedef)
- [ListPrivacyBudgetTemplatesOutputTypeDef](./type_defs.md#listprivacybudgettemplatesoutputtypedef)
- [ListSchemasOutputTypeDef](./type_defs.md#listschemasoutputtypedef)
- [MembershipPaymentConfigurationTypeDef](./type_defs.md#membershippaymentconfigurationtypedef)
- [MembershipProtectedQueryOutputConfigurationTypeDef](./type_defs.md#membershipprotectedqueryoutputconfigurationtypedef)
- [PaymentConfigurationTypeDef](./type_defs.md#paymentconfigurationtypedef)
- [ProtectedQueryOutputConfigurationTypeDef](./type_defs.md#protectedqueryoutputconfigurationtypedef)
- [ProtectedQueryOutputTypeDef](./type_defs.md#protectedqueryoutputtypedef)
- [QueryConstraintTypeDef](./type_defs.md#queryconstrainttypedef)
- [SchemaStatusDetailTypeDef](./type_defs.md#schemastatusdetailtypedef)
- [AnalysisRuleAggregationTypeDef](./type_defs.md#analysisruleaggregationtypedef)
- [AnalysisTemplateTypeDef](./type_defs.md#analysistemplatetypedef)
- [CollaborationAnalysisTemplateTypeDef](./type_defs.md#collaborationanalysistemplatetypedef)
- [ListCollaborationIdNamespaceAssociationsOutputTypeDef](./type_defs.md#listcollaborationidnamespaceassociationsoutputtypedef)
- [ListIdNamespaceAssociationsOutputTypeDef](./type_defs.md#listidnamespaceassociationsoutputtypedef)
- [GetCollaborationIdNamespaceAssociationOutputTypeDef](./type_defs.md#getcollaborationidnamespaceassociationoutputtypedef)
- [CreateIdNamespaceAssociationOutputTypeDef](./type_defs.md#createidnamespaceassociationoutputtypedef)
- [GetIdNamespaceAssociationOutputTypeDef](./type_defs.md#getidnamespaceassociationoutputtypedef)
- [UpdateIdNamespaceAssociationOutputTypeDef](./type_defs.md#updateidnamespaceassociationoutputtypedef)
- [CreateCollaborationOutputTypeDef](./type_defs.md#createcollaborationoutputtypedef)
- [GetCollaborationOutputTypeDef](./type_defs.md#getcollaborationoutputtypedef)
- [UpdateCollaborationOutputTypeDef](./type_defs.md#updatecollaborationoutputtypedef)
- [ReceiverConfigurationTypeDef](./type_defs.md#receiverconfigurationtypedef)
- [ConfiguredTableAssociationAnalysisRulePolicyOutputTypeDef](./type_defs.md#configuredtableassociationanalysisrulepolicyoutputtypedef)
- [ConfiguredTableAssociationAnalysisRulePolicyV1TypeDef](./type_defs.md#configuredtableassociationanalysisrulepolicyv1typedef)
- [ListIdMappingTablesOutputTypeDef](./type_defs.md#listidmappingtablesoutputtypedef)
- [AnalysisRuleCustomOutputTypeDef](./type_defs.md#analysisrulecustomoutputtypedef)
- [DifferentialPrivacyConfigurationUnionTypeDef](./type_defs.md#differentialprivacyconfigurationuniontypedef)
- [PrivacyImpactTypeDef](./type_defs.md#privacyimpacttypedef)
- [PreviewPrivacyImpactInputRequestTypeDef](./type_defs.md#previewprivacyimpactinputrequesttypedef)
- [PrivacyBudgetTypeDef](./type_defs.md#privacybudgettypedef)
- [CreatePrivacyBudgetTemplateInputRequestTypeDef](./type_defs.md#createprivacybudgettemplateinputrequesttypedef)
- [CollaborationPrivacyBudgetTemplateTypeDef](./type_defs.md#collaborationprivacybudgettemplatetypedef)
- [PrivacyBudgetTemplateTypeDef](./type_defs.md#privacybudgettemplatetypedef)
- [UpdatePrivacyBudgetTemplateInputRequestTypeDef](./type_defs.md#updateprivacybudgettemplateinputrequesttypedef)
- [ConfiguredTableTypeDef](./type_defs.md#configuredtabletypedef)
- [CreateConfiguredTableInputRequestTypeDef](./type_defs.md#createconfiguredtableinputrequesttypedef)
- [IdMappingTableTypeDef](./type_defs.md#idmappingtabletypedef)
- [SchemaTypePropertiesTypeDef](./type_defs.md#schematypepropertiestypedef)
- [MembershipSummaryTypeDef](./type_defs.md#membershipsummarytypedef)
- [MembershipProtectedQueryResultConfigurationTypeDef](./type_defs.md#membershipprotectedqueryresultconfigurationtypedef)
- [MemberSpecificationTypeDef](./type_defs.md#memberspecificationtypedef)
- [MemberSummaryTypeDef](./type_defs.md#membersummarytypedef)
- [ProtectedQueryResultConfigurationTypeDef](./type_defs.md#protectedqueryresultconfigurationtypedef)
- [ProtectedQueryResultTypeDef](./type_defs.md#protectedqueryresulttypedef)
- [AnalysisRuleIdMappingTableTypeDef](./type_defs.md#analysisruleidmappingtabletypedef)
- [AnalysisRuleAggregationUnionTypeDef](./type_defs.md#analysisruleaggregationuniontypedef)
- [CreateAnalysisTemplateOutputTypeDef](./type_defs.md#createanalysistemplateoutputtypedef)
- [GetAnalysisTemplateOutputTypeDef](./type_defs.md#getanalysistemplateoutputtypedef)
- [UpdateAnalysisTemplateOutputTypeDef](./type_defs.md#updateanalysistemplateoutputtypedef)
- [BatchGetCollaborationAnalysisTemplateOutputTypeDef](./type_defs.md#batchgetcollaborationanalysistemplateoutputtypedef)
- [GetCollaborationAnalysisTemplateOutputTypeDef](./type_defs.md#getcollaborationanalysistemplateoutputtypedef)
- [ProtectedQuerySummaryTypeDef](./type_defs.md#protectedquerysummarytypedef)
- [ConfiguredTableAssociationAnalysisRuleTypeDef](./type_defs.md#configuredtableassociationanalysisruletypedef)
- [ConfiguredTableAssociationAnalysisRulePolicyV1UnionTypeDef](./type_defs.md#configuredtableassociationanalysisrulepolicyv1uniontypedef)
- [ConfiguredTableAnalysisRulePolicyV1OutputTypeDef](./type_defs.md#configuredtableanalysisrulepolicyv1outputtypedef)
- [AnalysisRuleCustomTypeDef](./type_defs.md#analysisrulecustomtypedef)
- [PreviewPrivacyImpactOutputTypeDef](./type_defs.md#previewprivacyimpactoutputtypedef)
- [CollaborationPrivacyBudgetSummaryTypeDef](./type_defs.md#collaborationprivacybudgetsummarytypedef)
- [PrivacyBudgetSummaryTypeDef](./type_defs.md#privacybudgetsummarytypedef)
- [GetCollaborationPrivacyBudgetTemplateOutputTypeDef](./type_defs.md#getcollaborationprivacybudgettemplateoutputtypedef)
- [CreatePrivacyBudgetTemplateOutputTypeDef](./type_defs.md#createprivacybudgettemplateoutputtypedef)
- [GetPrivacyBudgetTemplateOutputTypeDef](./type_defs.md#getprivacybudgettemplateoutputtypedef)
- [UpdatePrivacyBudgetTemplateOutputTypeDef](./type_defs.md#updateprivacybudgettemplateoutputtypedef)
- [CreateConfiguredTableOutputTypeDef](./type_defs.md#createconfiguredtableoutputtypedef)
- [GetConfiguredTableOutputTypeDef](./type_defs.md#getconfiguredtableoutputtypedef)
- [UpdateConfiguredTableOutputTypeDef](./type_defs.md#updateconfiguredtableoutputtypedef)
- [CreateIdMappingTableOutputTypeDef](./type_defs.md#createidmappingtableoutputtypedef)
- [GetIdMappingTableOutputTypeDef](./type_defs.md#getidmappingtableoutputtypedef)
- [UpdateIdMappingTableOutputTypeDef](./type_defs.md#updateidmappingtableoutputtypedef)
- [SchemaTypeDef](./type_defs.md#schematypedef)
- [ListMembershipsOutputTypeDef](./type_defs.md#listmembershipsoutputtypedef)
- [CreateMembershipInputRequestTypeDef](./type_defs.md#createmembershipinputrequesttypedef)
- [MembershipTypeDef](./type_defs.md#membershiptypedef)
- [UpdateMembershipInputRequestTypeDef](./type_defs.md#updatemembershipinputrequesttypedef)
- [CreateCollaborationInputRequestTypeDef](./type_defs.md#createcollaborationinputrequesttypedef)
- [ListMembersOutputTypeDef](./type_defs.md#listmembersoutputtypedef)
- [StartProtectedQueryInputRequestTypeDef](./type_defs.md#startprotectedqueryinputrequesttypedef)
- [ProtectedQueryTypeDef](./type_defs.md#protectedquerytypedef)
- [AnalysisRulePolicyV1TypeDef](./type_defs.md#analysisrulepolicyv1typedef)
- [ListProtectedQueriesOutputTypeDef](./type_defs.md#listprotectedqueriesoutputtypedef)
- [CreateConfiguredTableAssociationAnalysisRuleOutputTypeDef](./type_defs.md#createconfiguredtableassociationanalysisruleoutputtypedef)
- [GetConfiguredTableAssociationAnalysisRuleOutputTypeDef](./type_defs.md#getconfiguredtableassociationanalysisruleoutputtypedef)
- [UpdateConfiguredTableAssociationAnalysisRuleOutputTypeDef](./type_defs.md#updateconfiguredtableassociationanalysisruleoutputtypedef)
- [ConfiguredTableAssociationAnalysisRulePolicyTypeDef](./type_defs.md#configuredtableassociationanalysisrulepolicytypedef)
- [ConfiguredTableAnalysisRulePolicyOutputTypeDef](./type_defs.md#configuredtableanalysisrulepolicyoutputtypedef)
- [AnalysisRuleCustomUnionTypeDef](./type_defs.md#analysisrulecustomuniontypedef)
- [ListCollaborationPrivacyBudgetsOutputTypeDef](./type_defs.md#listcollaborationprivacybudgetsoutputtypedef)
- [ListPrivacyBudgetsOutputTypeDef](./type_defs.md#listprivacybudgetsoutputtypedef)
- [BatchGetSchemaOutputTypeDef](./type_defs.md#batchgetschemaoutputtypedef)
- [GetSchemaOutputTypeDef](./type_defs.md#getschemaoutputtypedef)
- [CreateMembershipOutputTypeDef](./type_defs.md#createmembershipoutputtypedef)
- [GetMembershipOutputTypeDef](./type_defs.md#getmembershipoutputtypedef)
- [UpdateMembershipOutputTypeDef](./type_defs.md#updatemembershipoutputtypedef)
- [GetProtectedQueryOutputTypeDef](./type_defs.md#getprotectedqueryoutputtypedef)
- [StartProtectedQueryOutputTypeDef](./type_defs.md#startprotectedqueryoutputtypedef)
- [UpdateProtectedQueryOutputTypeDef](./type_defs.md#updateprotectedqueryoutputtypedef)
- [AnalysisRulePolicyTypeDef](./type_defs.md#analysisrulepolicytypedef)
- [CreateConfiguredTableAssociationAnalysisRuleInputRequestTypeDef](./type_defs.md#createconfiguredtableassociationanalysisruleinputrequesttypedef)
- [UpdateConfiguredTableAssociationAnalysisRuleInputRequestTypeDef](./type_defs.md#updateconfiguredtableassociationanalysisruleinputrequesttypedef)
- [ConfiguredTableAnalysisRuleTypeDef](./type_defs.md#configuredtableanalysisruletypedef)
- [ConfiguredTableAnalysisRulePolicyV1TypeDef](./type_defs.md#configuredtableanalysisrulepolicyv1typedef)
- [AnalysisRuleTypeDef](./type_defs.md#analysisruletypedef)
- [CreateConfiguredTableAnalysisRuleOutputTypeDef](./type_defs.md#createconfiguredtableanalysisruleoutputtypedef)
- [GetConfiguredTableAnalysisRuleOutputTypeDef](./type_defs.md#getconfiguredtableanalysisruleoutputtypedef)
- [UpdateConfiguredTableAnalysisRuleOutputTypeDef](./type_defs.md#updateconfiguredtableanalysisruleoutputtypedef)
- [ConfiguredTableAnalysisRulePolicyV1UnionTypeDef](./type_defs.md#configuredtableanalysisrulepolicyv1uniontypedef)
- [BatchGetSchemaAnalysisRuleOutputTypeDef](./type_defs.md#batchgetschemaanalysisruleoutputtypedef)
- [GetSchemaAnalysisRuleOutputTypeDef](./type_defs.md#getschemaanalysisruleoutputtypedef)
- [ConfiguredTableAnalysisRulePolicyTypeDef](./type_defs.md#configuredtableanalysisrulepolicytypedef)
- [CreateConfiguredTableAnalysisRuleInputRequestTypeDef](./type_defs.md#createconfiguredtableanalysisruleinputrequesttypedef)
- [UpdateConfiguredTableAnalysisRuleInputRequestTypeDef](./type_defs.md#updateconfiguredtableanalysisruleinputrequesttypedef)

