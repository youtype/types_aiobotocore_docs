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
- [ListCollaborationsPaginator](./paginators.md#listcollaborationspaginator)
- [ListConfiguredTableAssociationsPaginator](./paginators.md#listconfiguredtableassociationspaginator)
- [ListConfiguredTablesPaginator](./paginators.md#listconfiguredtablespaginator)
- [ListMembersPaginator](./paginators.md#listmemberspaginator)
- [ListMembershipsPaginator](./paginators.md#listmembershipspaginator)
- [ListProtectedQueriesPaginator](./paginators.md#listprotectedqueriespaginator)
- [ListSchemasPaginator](./paginators.md#listschemaspaginator)








## Literals

Type annotations for [literals](./literals.md) used in methods and schema.

```python
# AggregateFunctionNameType usage example

from types_aiobotocore_cleanrooms.literals import AggregateFunctionNameType

def get_value() -> AggregateFunctionNameType:
    return "AVG"
```

- [AggregateFunctionNameType](./literals.md#aggregatefunctionnametype)
- [AggregationTypeType](./literals.md#aggregationtypetype)
- [AnalysisFormatType](./literals.md#analysisformattype)
- [AnalysisMethodType](./literals.md#analysismethodtype)
- [AnalysisRuleTypeType](./literals.md#analysisruletypetype)
- [CollaborationQueryLogStatusType](./literals.md#collaborationquerylogstatustype)
- [ConfiguredTableAnalysisRuleTypeType](./literals.md#configuredtableanalysisruletypetype)
- [FilterableMemberStatusType](./literals.md#filterablememberstatustype)
- [JoinOperatorType](./literals.md#joinoperatortype)
- [JoinRequiredOptionType](./literals.md#joinrequiredoptiontype)
- [ListAnalysisTemplatesPaginatorName](./literals.md#listanalysistemplatespaginatorname)
- [ListCollaborationAnalysisTemplatesPaginatorName](./literals.md#listcollaborationanalysistemplatespaginatorname)
- [ListCollaborationsPaginatorName](./literals.md#listcollaborationspaginatorname)
- [ListConfiguredTableAssociationsPaginatorName](./literals.md#listconfiguredtableassociationspaginatorname)
- [ListConfiguredTablesPaginatorName](./literals.md#listconfiguredtablespaginatorname)
- [ListMembersPaginatorName](./literals.md#listmemberspaginatorname)
- [ListMembershipsPaginatorName](./literals.md#listmembershipspaginatorname)
- [ListProtectedQueriesPaginatorName](./literals.md#listprotectedqueriespaginatorname)
- [ListSchemasPaginatorName](./literals.md#listschemaspaginatorname)
- [MemberAbilityType](./literals.md#memberabilitytype)
- [MemberStatusType](./literals.md#memberstatustype)
- [MembershipQueryLogStatusType](./literals.md#membershipquerylogstatustype)
- [MembershipStatusType](./literals.md#membershipstatustype)
- [ParameterTypeType](./literals.md#parametertypetype)
- [ProtectedQueryStatusType](./literals.md#protectedquerystatustype)
- [ProtectedQueryTypeType](./literals.md#protectedquerytypetype)
- [ResultFormatType](./literals.md#resultformattype)
- [ScalarFunctionsType](./literals.md#scalarfunctionstype)
- [SchemaTypeType](./literals.md#schematypetype)
- [TargetProtectedQueryStatusType](./literals.md#targetprotectedquerystatustype)
- [CleanRoomsServiceServiceName](./literals.md#cleanroomsserviceservicename)
- [ServiceName](./literals.md#servicename)
- [ResourceServiceName](./literals.md#resourceservicename)
- [PaginatorName](./literals.md#paginatorname)
- [RegionName](./literals.md#regionname)




## Type definitions

Type annotations for [type definitions](./type_defs.md) used in methods and schema.

- [AggregateColumnTypeDef](./type_defs.md#aggregatecolumntypedef)
- [AggregationConstraintTypeDef](./type_defs.md#aggregationconstrainttypedef)
- [AnalysisParameterTypeDef](./type_defs.md#analysisparametertypedef)
- [AnalysisRuleCustomTypeDef](./type_defs.md#analysisrulecustomtypedef)
- [AnalysisRuleListTypeDef](./type_defs.md#analysisrulelisttypedef)
- [AnalysisSchemaTypeDef](./type_defs.md#analysisschematypedef)
- [AnalysisSourceTypeDef](./type_defs.md#analysissourcetypedef)
- [AnalysisTemplateSummaryTypeDef](./type_defs.md#analysistemplatesummarytypedef)
- [BatchGetCollaborationAnalysisTemplateErrorTypeDef](./type_defs.md#batchgetcollaborationanalysistemplateerrortypedef)
- [BatchGetCollaborationAnalysisTemplateInputRequestTypeDef](./type_defs.md#batchgetcollaborationanalysistemplateinputrequesttypedef)
- [ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef)
- [BatchGetSchemaErrorTypeDef](./type_defs.md#batchgetschemaerrortypedef)
- [BatchGetSchemaInputRequestTypeDef](./type_defs.md#batchgetschemainputrequesttypedef)
- [CollaborationAnalysisTemplateSummaryTypeDef](./type_defs.md#collaborationanalysistemplatesummarytypedef)
- [CollaborationSummaryTypeDef](./type_defs.md#collaborationsummarytypedef)
- [DataEncryptionMetadataTypeDef](./type_defs.md#dataencryptionmetadatatypedef)
- [ColumnTypeDef](./type_defs.md#columntypedef)
- [ConfiguredTableAssociationSummaryTypeDef](./type_defs.md#configuredtableassociationsummarytypedef)
- [ConfiguredTableAssociationTypeDef](./type_defs.md#configuredtableassociationtypedef)
- [ConfiguredTableSummaryTypeDef](./type_defs.md#configuredtablesummarytypedef)
- [MemberSpecificationTypeDef](./type_defs.md#memberspecificationtypedef)
- [CreateConfiguredTableAssociationInputRequestTypeDef](./type_defs.md#createconfiguredtableassociationinputrequesttypedef)
- [CreateMembershipInputRequestTypeDef](./type_defs.md#createmembershipinputrequesttypedef)
- [MembershipTypeDef](./type_defs.md#membershiptypedef)
- [DeleteAnalysisTemplateInputRequestTypeDef](./type_defs.md#deleteanalysistemplateinputrequesttypedef)
- [DeleteCollaborationInputRequestTypeDef](./type_defs.md#deletecollaborationinputrequesttypedef)
- [DeleteConfiguredTableAnalysisRuleInputRequestTypeDef](./type_defs.md#deleteconfiguredtableanalysisruleinputrequesttypedef)
- [DeleteConfiguredTableAssociationInputRequestTypeDef](./type_defs.md#deleteconfiguredtableassociationinputrequesttypedef)
- [DeleteConfiguredTableInputRequestTypeDef](./type_defs.md#deleteconfiguredtableinputrequesttypedef)
- [DeleteMemberInputRequestTypeDef](./type_defs.md#deletememberinputrequesttypedef)
- [DeleteMembershipInputRequestTypeDef](./type_defs.md#deletemembershipinputrequesttypedef)
- [GetAnalysisTemplateInputRequestTypeDef](./type_defs.md#getanalysistemplateinputrequesttypedef)
- [GetCollaborationAnalysisTemplateInputRequestTypeDef](./type_defs.md#getcollaborationanalysistemplateinputrequesttypedef)
- [GetCollaborationInputRequestTypeDef](./type_defs.md#getcollaborationinputrequesttypedef)
- [GetConfiguredTableAnalysisRuleInputRequestTypeDef](./type_defs.md#getconfiguredtableanalysisruleinputrequesttypedef)
- [GetConfiguredTableAssociationInputRequestTypeDef](./type_defs.md#getconfiguredtableassociationinputrequesttypedef)
- [GetConfiguredTableInputRequestTypeDef](./type_defs.md#getconfiguredtableinputrequesttypedef)
- [GetMembershipInputRequestTypeDef](./type_defs.md#getmembershipinputrequesttypedef)
- [GetProtectedQueryInputRequestTypeDef](./type_defs.md#getprotectedqueryinputrequesttypedef)
- [GetSchemaAnalysisRuleInputRequestTypeDef](./type_defs.md#getschemaanalysisruleinputrequesttypedef)
- [GetSchemaInputRequestTypeDef](./type_defs.md#getschemainputrequesttypedef)
- [GlueTableReferenceTypeDef](./type_defs.md#gluetablereferencetypedef)
- [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
- [ListAnalysisTemplatesInputRequestTypeDef](./type_defs.md#listanalysistemplatesinputrequesttypedef)
- [ListCollaborationAnalysisTemplatesInputRequestTypeDef](./type_defs.md#listcollaborationanalysistemplatesinputrequesttypedef)
- [ListCollaborationsInputRequestTypeDef](./type_defs.md#listcollaborationsinputrequesttypedef)
- [ListConfiguredTableAssociationsInputRequestTypeDef](./type_defs.md#listconfiguredtableassociationsinputrequesttypedef)
- [ListConfiguredTablesInputRequestTypeDef](./type_defs.md#listconfiguredtablesinputrequesttypedef)
- [ListMembersInputRequestTypeDef](./type_defs.md#listmembersinputrequesttypedef)
- [MemberSummaryTypeDef](./type_defs.md#membersummarytypedef)
- [ListMembershipsInputRequestTypeDef](./type_defs.md#listmembershipsinputrequesttypedef)
- [MembershipSummaryTypeDef](./type_defs.md#membershipsummarytypedef)
- [ListProtectedQueriesInputRequestTypeDef](./type_defs.md#listprotectedqueriesinputrequesttypedef)
- [ProtectedQuerySummaryTypeDef](./type_defs.md#protectedquerysummarytypedef)
- [ListSchemasInputRequestTypeDef](./type_defs.md#listschemasinputrequesttypedef)
- [SchemaSummaryTypeDef](./type_defs.md#schemasummarytypedef)
- [ListTagsForResourceInputRequestTypeDef](./type_defs.md#listtagsforresourceinputrequesttypedef)
- [ProtectedQueryErrorTypeDef](./type_defs.md#protectedqueryerrortypedef)
- [ProtectedQueryS3OutputConfigurationTypeDef](./type_defs.md#protectedquerys3outputconfigurationtypedef)
- [ProtectedQueryS3OutputTypeDef](./type_defs.md#protectedquerys3outputtypedef)
- [ProtectedQuerySQLParametersTypeDef](./type_defs.md#protectedquerysqlparameterstypedef)
- [ProtectedQueryStatisticsTypeDef](./type_defs.md#protectedquerystatisticstypedef)
- [TagResourceInputRequestTypeDef](./type_defs.md#tagresourceinputrequesttypedef)
- [UntagResourceInputRequestTypeDef](./type_defs.md#untagresourceinputrequesttypedef)
- [UpdateAnalysisTemplateInputRequestTypeDef](./type_defs.md#updateanalysistemplateinputrequesttypedef)
- [UpdateCollaborationInputRequestTypeDef](./type_defs.md#updatecollaborationinputrequesttypedef)
- [UpdateConfiguredTableAssociationInputRequestTypeDef](./type_defs.md#updateconfiguredtableassociationinputrequesttypedef)
- [UpdateConfiguredTableInputRequestTypeDef](./type_defs.md#updateconfiguredtableinputrequesttypedef)
- [UpdateMembershipInputRequestTypeDef](./type_defs.md#updatemembershipinputrequesttypedef)
- [UpdateProtectedQueryInputRequestTypeDef](./type_defs.md#updateprotectedqueryinputrequesttypedef)
- [AnalysisRuleAggregationTypeDef](./type_defs.md#analysisruleaggregationtypedef)
- [AnalysisTemplateTypeDef](./type_defs.md#analysistemplatetypedef)
- [CollaborationAnalysisTemplateTypeDef](./type_defs.md#collaborationanalysistemplatetypedef)
- [CreateAnalysisTemplateInputRequestTypeDef](./type_defs.md#createanalysistemplateinputrequesttypedef)
- [ListAnalysisTemplatesOutputTypeDef](./type_defs.md#listanalysistemplatesoutputtypedef)
- [ListTagsForResourceOutputTypeDef](./type_defs.md#listtagsforresourceoutputtypedef)
- [ListCollaborationAnalysisTemplatesOutputTypeDef](./type_defs.md#listcollaborationanalysistemplatesoutputtypedef)
- [ListCollaborationsOutputTypeDef](./type_defs.md#listcollaborationsoutputtypedef)
- [CollaborationTypeDef](./type_defs.md#collaborationtypedef)
- [SchemaTypeDef](./type_defs.md#schematypedef)
- [ListConfiguredTableAssociationsOutputTypeDef](./type_defs.md#listconfiguredtableassociationsoutputtypedef)
- [CreateConfiguredTableAssociationOutputTypeDef](./type_defs.md#createconfiguredtableassociationoutputtypedef)
- [GetConfiguredTableAssociationOutputTypeDef](./type_defs.md#getconfiguredtableassociationoutputtypedef)
- [UpdateConfiguredTableAssociationOutputTypeDef](./type_defs.md#updateconfiguredtableassociationoutputtypedef)
- [ListConfiguredTablesOutputTypeDef](./type_defs.md#listconfiguredtablesoutputtypedef)
- [CreateCollaborationInputRequestTypeDef](./type_defs.md#createcollaborationinputrequesttypedef)
- [CreateMembershipOutputTypeDef](./type_defs.md#createmembershipoutputtypedef)
- [GetMembershipOutputTypeDef](./type_defs.md#getmembershipoutputtypedef)
- [UpdateMembershipOutputTypeDef](./type_defs.md#updatemembershipoutputtypedef)
- [TableReferenceTypeDef](./type_defs.md#tablereferencetypedef)
- [ListAnalysisTemplatesInputListAnalysisTemplatesPaginateTypeDef](./type_defs.md#listanalysistemplatesinputlistanalysistemplatespaginatetypedef)
- [ListCollaborationAnalysisTemplatesInputListCollaborationAnalysisTemplatesPaginateTypeDef](./type_defs.md#listcollaborationanalysistemplatesinputlistcollaborationanalysistemplatespaginatetypedef)
- [ListCollaborationsInputListCollaborationsPaginateTypeDef](./type_defs.md#listcollaborationsinputlistcollaborationspaginatetypedef)
- [ListConfiguredTableAssociationsInputListConfiguredTableAssociationsPaginateTypeDef](./type_defs.md#listconfiguredtableassociationsinputlistconfiguredtableassociationspaginatetypedef)
- [ListConfiguredTablesInputListConfiguredTablesPaginateTypeDef](./type_defs.md#listconfiguredtablesinputlistconfiguredtablespaginatetypedef)
- [ListMembersInputListMembersPaginateTypeDef](./type_defs.md#listmembersinputlistmemberspaginatetypedef)
- [ListMembershipsInputListMembershipsPaginateTypeDef](./type_defs.md#listmembershipsinputlistmembershipspaginatetypedef)
- [ListProtectedQueriesInputListProtectedQueriesPaginateTypeDef](./type_defs.md#listprotectedqueriesinputlistprotectedqueriespaginatetypedef)
- [ListSchemasInputListSchemasPaginateTypeDef](./type_defs.md#listschemasinputlistschemaspaginatetypedef)
- [ListMembersOutputTypeDef](./type_defs.md#listmembersoutputtypedef)
- [ListMembershipsOutputTypeDef](./type_defs.md#listmembershipsoutputtypedef)
- [ListProtectedQueriesOutputTypeDef](./type_defs.md#listprotectedqueriesoutputtypedef)
- [ListSchemasOutputTypeDef](./type_defs.md#listschemasoutputtypedef)
- [ProtectedQueryOutputConfigurationTypeDef](./type_defs.md#protectedqueryoutputconfigurationtypedef)
- [ProtectedQueryOutputTypeDef](./type_defs.md#protectedqueryoutputtypedef)
- [AnalysisRulePolicyV1TypeDef](./type_defs.md#analysisrulepolicyv1typedef)
- [ConfiguredTableAnalysisRulePolicyV1TypeDef](./type_defs.md#configuredtableanalysisrulepolicyv1typedef)
- [CreateAnalysisTemplateOutputTypeDef](./type_defs.md#createanalysistemplateoutputtypedef)
- [GetAnalysisTemplateOutputTypeDef](./type_defs.md#getanalysistemplateoutputtypedef)
- [UpdateAnalysisTemplateOutputTypeDef](./type_defs.md#updateanalysistemplateoutputtypedef)
- [BatchGetCollaborationAnalysisTemplateOutputTypeDef](./type_defs.md#batchgetcollaborationanalysistemplateoutputtypedef)
- [GetCollaborationAnalysisTemplateOutputTypeDef](./type_defs.md#getcollaborationanalysistemplateoutputtypedef)
- [CreateCollaborationOutputTypeDef](./type_defs.md#createcollaborationoutputtypedef)
- [GetCollaborationOutputTypeDef](./type_defs.md#getcollaborationoutputtypedef)
- [UpdateCollaborationOutputTypeDef](./type_defs.md#updatecollaborationoutputtypedef)
- [BatchGetSchemaOutputTypeDef](./type_defs.md#batchgetschemaoutputtypedef)
- [GetSchemaOutputTypeDef](./type_defs.md#getschemaoutputtypedef)
- [ConfiguredTableTypeDef](./type_defs.md#configuredtabletypedef)
- [CreateConfiguredTableInputRequestTypeDef](./type_defs.md#createconfiguredtableinputrequesttypedef)
- [ProtectedQueryResultConfigurationTypeDef](./type_defs.md#protectedqueryresultconfigurationtypedef)
- [ProtectedQueryResultTypeDef](./type_defs.md#protectedqueryresulttypedef)
- [AnalysisRulePolicyTypeDef](./type_defs.md#analysisrulepolicytypedef)
- [ConfiguredTableAnalysisRulePolicyTypeDef](./type_defs.md#configuredtableanalysisrulepolicytypedef)
- [CreateConfiguredTableOutputTypeDef](./type_defs.md#createconfiguredtableoutputtypedef)
- [GetConfiguredTableOutputTypeDef](./type_defs.md#getconfiguredtableoutputtypedef)
- [UpdateConfiguredTableOutputTypeDef](./type_defs.md#updateconfiguredtableoutputtypedef)
- [StartProtectedQueryInputRequestTypeDef](./type_defs.md#startprotectedqueryinputrequesttypedef)
- [ProtectedQueryTypeDef](./type_defs.md#protectedquerytypedef)
- [AnalysisRuleTypeDef](./type_defs.md#analysisruletypedef)
- [ConfiguredTableAnalysisRuleTypeDef](./type_defs.md#configuredtableanalysisruletypedef)
- [CreateConfiguredTableAnalysisRuleInputRequestTypeDef](./type_defs.md#createconfiguredtableanalysisruleinputrequesttypedef)
- [UpdateConfiguredTableAnalysisRuleInputRequestTypeDef](./type_defs.md#updateconfiguredtableanalysisruleinputrequesttypedef)
- [GetProtectedQueryOutputTypeDef](./type_defs.md#getprotectedqueryoutputtypedef)
- [StartProtectedQueryOutputTypeDef](./type_defs.md#startprotectedqueryoutputtypedef)
- [UpdateProtectedQueryOutputTypeDef](./type_defs.md#updateprotectedqueryoutputtypedef)
- [GetSchemaAnalysisRuleOutputTypeDef](./type_defs.md#getschemaanalysisruleoutputtypedef)
- [CreateConfiguredTableAnalysisRuleOutputTypeDef](./type_defs.md#createconfiguredtableanalysisruleoutputtypedef)
- [GetConfiguredTableAnalysisRuleOutputTypeDef](./type_defs.md#getconfiguredtableanalysisruleoutputtypedef)
- [UpdateConfiguredTableAnalysisRuleOutputTypeDef](./type_defs.md#updateconfiguredtableanalysisruleoutputtypedef)

