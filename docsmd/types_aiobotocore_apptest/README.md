# MainframeModernizationApplicationTesting module

> [Index](../README.md) > MainframeModernizationApplicationTesting


!!! note ""

    Auto-generated documentation for [MainframeModernizationApplicationTesting](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/apptest.html#mainframemodernizationapplicationtesting)
    type annotations stubs module [types-aiobotocore-apptest](https://pypi.org/project/types-aiobotocore-apptest/).

## How to install

### Generate locally (recommended)

You can generate type annotations for `aiobotocore` package locally with `mypy-boto3-builder`.
Use [uv](https://docs.astral.sh/uv/getting-started/installation/) for build isolation.

1. Run mypy-boto3-builder in your package root directory: `uvx --with 'aiobotocore==2.20.0' mypy-boto3-builder`
1. Select `aiobotocore` AWS SDK.
1. Add `MainframeModernizationApplicationTesting` service.
1. Use provided commands to install generated packages.



### From PyPI with pip

Install `types-aiobotocore` for `MainframeModernizationApplicationTesting` service.

```bash
# install with aiobotocore type annotations
python -m pip install 'types-aiobotocore[apptest]'

# Lite version does not provide session.client/resource overloads
# it is more RAM-friendly, but requires explicit type annotations
python -m pip install 'types-aiobotocore-lite[apptest]'

# standalone installation
python -m pip install types-aiobotocore-apptest
```



## How to uninstall

```bash
python -m pip uninstall -y types-aiobotocore-apptest
```

## Usage

Code samples can be found in [Examples](./usage.md).

## MainframeModernizationApplicationTestingClient

Type annotations and code completion for  `#!python session.create_client("apptest")` as [MainframeModernizationApplicationTestingClient](./client.md)
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/apptest.html#MainframeModernizationApplicationTesting.Client)

```python
# MainframeModernizationApplicationTestingClient usage example

from aiobotocore.session import get_session

from types_aiobotocore_apptest.client import MainframeModernizationApplicationTestingClient


session = get_session()
async with session.create_client("apptest") as client:
    client: MainframeModernizationApplicationTestingClient
```


## Paginators

Type annotations and code completion for
[paginators](./paginators.md)
from `#!python session.create_client("apptest").get_paginator("...")`.

```python
# ListTestCasesPaginator usage example

from types_aiobotocore_apptest.paginator import ListTestCasesPaginator

def get_list_test_cases_paginator() -> ListTestCasesPaginator:
    return client.get_paginator("list_test_cases"))
```

- [ListTestCasesPaginator](./paginators.md#listtestcasespaginator)
- [ListTestConfigurationsPaginator](./paginators.md#listtestconfigurationspaginator)
- [ListTestRunStepsPaginator](./paginators.md#listtestrunstepspaginator)
- [ListTestRunTestCasesPaginator](./paginators.md#listtestruntestcasespaginator)
- [ListTestRunsPaginator](./paginators.md#listtestrunspaginator)
- [ListTestSuitesPaginator](./paginators.md#listtestsuitespaginator)








## Literals

Type annotations for [literals](./literals.md) used in methods and schema.

```python
# CaptureToolType usage example

from types_aiobotocore_apptest.literals import CaptureToolType

def get_value() -> CaptureToolType:
    return "AWS DMS"
```

- [CaptureToolType](./literals.md#capturetooltype)
- [CloudFormationActionTypeType](./literals.md#cloudformationactiontypetype)
- [ComparisonStatusEnumType](./literals.md#comparisonstatusenumtype)
- [DataSetTypeType](./literals.md#datasettypetype)
- [FormatType](./literals.md#formattype)
- [ListTestCasesPaginatorName](./literals.md#listtestcasespaginatorname)
- [ListTestConfigurationsPaginatorName](./literals.md#listtestconfigurationspaginatorname)
- [ListTestRunStepsPaginatorName](./literals.md#listtestrunstepspaginatorname)
- [ListTestRunTestCasesPaginatorName](./literals.md#listtestruntestcasespaginatorname)
- [ListTestRunsPaginatorName](./literals.md#listtestrunspaginatorname)
- [ListTestSuitesPaginatorName](./literals.md#listtestsuitespaginatorname)
- [M2ManagedActionTypeType](./literals.md#m2managedactiontypetype)
- [M2ManagedRuntimeType](./literals.md#m2managedruntimetype)
- [M2NonManagedActionTypeType](./literals.md#m2nonmanagedactiontypetype)
- [M2NonManagedRuntimeType](./literals.md#m2nonmanagedruntimetype)
- [ScriptTypeType](./literals.md#scripttypetype)
- [SourceDatabaseType](./literals.md#sourcedatabasetype)
- [StepRunStatusType](./literals.md#steprunstatustype)
- [TargetDatabaseType](./literals.md#targetdatabasetype)
- [TestCaseLifecycleType](./literals.md#testcaselifecycletype)
- [TestCaseRunStatusType](./literals.md#testcaserunstatustype)
- [TestConfigurationLifecycleType](./literals.md#testconfigurationlifecycletype)
- [TestRunStatusType](./literals.md#testrunstatustype)
- [TestSuiteLifecycleType](./literals.md#testsuitelifecycletype)
- [MainframeModernizationApplicationTestingServiceName](./literals.md#mainframemodernizationapplicationtestingservicename)
- [ServiceName](./literals.md#servicename)
- [ResourceServiceName](./literals.md#resourceservicename)
- [PaginatorName](./literals.md#paginatorname)
- [RegionName](./literals.md#regionname)




## Type definitions

Type annotations for [type definitions](./type_defs.md) used in methods and schema.

- [BatchOutputTypeDef](./type_defs.md#batchoutputtypedef)
- [MainframeActionPropertiesTypeDef](./type_defs.md#mainframeactionpropertiestypedef)
- [DataSetTypeDef](./type_defs.md#datasettypedef)
- [BatchTypeDef](./type_defs.md#batchtypedef)
- [CloudFormationActionTypeDef](./type_defs.md#cloudformationactiontypedef)
- [CloudFormationOutputTypeDef](./type_defs.md#cloudformationoutputtypedef)
- [CloudFormationTypeDef](./type_defs.md#cloudformationtypedef)
- [CompareDataSetsStepOutputTypeDef](./type_defs.md#comparedatasetsstepoutputtypedef)
- [SourceDatabaseMetadataTypeDef](./type_defs.md#sourcedatabasemetadatatypedef)
- [TargetDatabaseMetadataTypeDef](./type_defs.md#targetdatabasemetadatatypedef)
- [CompareDatabaseCDCStepOutputTypeDef](./type_defs.md#comparedatabasecdcstepoutputtypedef)
- [CreateCloudFormationStepInputTypeDef](./type_defs.md#createcloudformationstepinputtypedef)
- [CreateCloudFormationStepOutputTypeDef](./type_defs.md#createcloudformationstepoutputtypedef)
- [ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef)
- [ServiceSettingsTypeDef](./type_defs.md#servicesettingstypedef)
- [DeleteCloudFormationStepInputTypeDef](./type_defs.md#deletecloudformationstepinputtypedef)
- [DeleteTestCaseRequestTypeDef](./type_defs.md#deletetestcaserequesttypedef)
- [DeleteTestConfigurationRequestTypeDef](./type_defs.md#deletetestconfigurationrequesttypedef)
- [DeleteTestRunRequestTypeDef](./type_defs.md#deletetestrunrequesttypedef)
- [DeleteTestSuiteRequestTypeDef](./type_defs.md#deletetestsuiterequesttypedef)
- [GetTestCaseRequestTypeDef](./type_defs.md#gettestcaserequesttypedef)
- [TestCaseLatestVersionTypeDef](./type_defs.md#testcaselatestversiontypedef)
- [GetTestConfigurationRequestTypeDef](./type_defs.md#gettestconfigurationrequesttypedef)
- [TestConfigurationLatestVersionTypeDef](./type_defs.md#testconfigurationlatestversiontypedef)
- [GetTestRunStepRequestTypeDef](./type_defs.md#gettestrunsteprequesttypedef)
- [GetTestSuiteRequestTypeDef](./type_defs.md#gettestsuiterequesttypedef)
- [TestCasesOutputTypeDef](./type_defs.md#testcasesoutputtypedef)
- [TestSuiteLatestVersionTypeDef](./type_defs.md#testsuitelatestversiontypedef)
- [ListTagsForResourceRequestTypeDef](./type_defs.md#listtagsforresourcerequesttypedef)
- [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
- [ListTestCasesRequestTypeDef](./type_defs.md#listtestcasesrequesttypedef)
- [TestCaseSummaryTypeDef](./type_defs.md#testcasesummarytypedef)
- [ListTestConfigurationsRequestTypeDef](./type_defs.md#listtestconfigurationsrequesttypedef)
- [TestConfigurationSummaryTypeDef](./type_defs.md#testconfigurationsummarytypedef)
- [ListTestRunStepsRequestTypeDef](./type_defs.md#listtestrunstepsrequesttypedef)
- [TestRunStepSummaryTypeDef](./type_defs.md#testrunstepsummarytypedef)
- [ListTestRunTestCasesRequestTypeDef](./type_defs.md#listtestruntestcasesrequesttypedef)
- [TestCaseRunSummaryTypeDef](./type_defs.md#testcaserunsummarytypedef)
- [ListTestRunsRequestTypeDef](./type_defs.md#listtestrunsrequesttypedef)
- [TestRunSummaryTypeDef](./type_defs.md#testrunsummarytypedef)
- [ListTestSuitesRequestTypeDef](./type_defs.md#listtestsuitesrequesttypedef)
- [TestSuiteSummaryTypeDef](./type_defs.md#testsuitesummarytypedef)
- [M2ManagedActionPropertiesTypeDef](./type_defs.md#m2managedactionpropertiestypedef)
- [M2ManagedApplicationStepOutputTypeDef](./type_defs.md#m2managedapplicationstepoutputtypedef)
- [M2ManagedApplicationSummaryTypeDef](./type_defs.md#m2managedapplicationsummarytypedef)
- [M2ManagedApplicationTypeDef](./type_defs.md#m2managedapplicationtypedef)
- [M2NonManagedApplicationActionTypeDef](./type_defs.md#m2nonmanagedapplicationactiontypedef)
- [M2NonManagedApplicationStepInputTypeDef](./type_defs.md#m2nonmanagedapplicationstepinputtypedef)
- [M2NonManagedApplicationSummaryTypeDef](./type_defs.md#m2nonmanagedapplicationsummarytypedef)
- [M2NonManagedApplicationTypeDef](./type_defs.md#m2nonmanagedapplicationtypedef)
- [OutputFileTypeDef](./type_defs.md#outputfiletypedef)
- [ScriptSummaryTypeDef](./type_defs.md#scriptsummarytypedef)
- [ScriptTypeDef](./type_defs.md#scripttypedef)
- [StartTestRunRequestTypeDef](./type_defs.md#starttestrunrequesttypedef)
- [TagResourceRequestTypeDef](./type_defs.md#tagresourcerequesttypedef)
- [TestCasesTypeDef](./type_defs.md#testcasestypedef)
- [UntagResourceRequestTypeDef](./type_defs.md#untagresourcerequesttypedef)
- [BatchStepOutputTypeDef](./type_defs.md#batchstepoutputtypedef)
- [CompareDataSetsStepInputTypeDef](./type_defs.md#comparedatasetsstepinputtypedef)
- [TN3270StepOutputTypeDef](./type_defs.md#tn3270stepoutputtypedef)
- [BatchUnionTypeDef](./type_defs.md#batchuniontypedef)
- [CloudFormationUnionTypeDef](./type_defs.md#cloudformationuniontypedef)
- [CompareDatabaseCDCStepInputTypeDef](./type_defs.md#comparedatabasecdcstepinputtypedef)
- [DatabaseCDCTypeDef](./type_defs.md#databasecdctypedef)
- [CreateCloudFormationSummaryTypeDef](./type_defs.md#createcloudformationsummarytypedef)
- [CreateTestCaseResponseTypeDef](./type_defs.md#createtestcaseresponsetypedef)
- [CreateTestConfigurationResponseTypeDef](./type_defs.md#createtestconfigurationresponsetypedef)
- [CreateTestSuiteResponseTypeDef](./type_defs.md#createtestsuiteresponsetypedef)
- [ListTagsForResourceResponseTypeDef](./type_defs.md#listtagsforresourceresponsetypedef)
- [StartTestRunResponseTypeDef](./type_defs.md#starttestrunresponsetypedef)
- [UpdateTestCaseResponseTypeDef](./type_defs.md#updatetestcaseresponsetypedef)
- [UpdateTestConfigurationResponseTypeDef](./type_defs.md#updatetestconfigurationresponsetypedef)
- [UpdateTestSuiteResponseTypeDef](./type_defs.md#updatetestsuiteresponsetypedef)
- [DeleteCloudFormationSummaryTypeDef](./type_defs.md#deletecloudformationsummarytypedef)
- [ListTestCasesRequestPaginateTypeDef](./type_defs.md#listtestcasesrequestpaginatetypedef)
- [ListTestConfigurationsRequestPaginateTypeDef](./type_defs.md#listtestconfigurationsrequestpaginatetypedef)
- [ListTestRunStepsRequestPaginateTypeDef](./type_defs.md#listtestrunstepsrequestpaginatetypedef)
- [ListTestRunTestCasesRequestPaginateTypeDef](./type_defs.md#listtestruntestcasesrequestpaginatetypedef)
- [ListTestRunsRequestPaginateTypeDef](./type_defs.md#listtestrunsrequestpaginatetypedef)
- [ListTestSuitesRequestPaginateTypeDef](./type_defs.md#listtestsuitesrequestpaginatetypedef)
- [ListTestCasesResponseTypeDef](./type_defs.md#listtestcasesresponsetypedef)
- [ListTestConfigurationsResponseTypeDef](./type_defs.md#listtestconfigurationsresponsetypedef)
- [ListTestRunStepsResponseTypeDef](./type_defs.md#listtestrunstepsresponsetypedef)
- [ListTestRunTestCasesResponseTypeDef](./type_defs.md#listtestruntestcasesresponsetypedef)
- [ListTestRunsResponseTypeDef](./type_defs.md#listtestrunsresponsetypedef)
- [ListTestSuitesResponseTypeDef](./type_defs.md#listtestsuitesresponsetypedef)
- [M2ManagedApplicationActionTypeDef](./type_defs.md#m2managedapplicationactiontypedef)
- [M2ManagedApplicationStepInputTypeDef](./type_defs.md#m2managedapplicationstepinputtypedef)
- [M2NonManagedApplicationStepSummaryTypeDef](./type_defs.md#m2nonmanagedapplicationstepsummarytypedef)
- [MainframeResourceSummaryTypeDef](./type_defs.md#mainframeresourcesummarytypedef)
- [ResourceTypeOutputTypeDef](./type_defs.md#resourcetypeoutputtypedef)
- [OutputTypeDef](./type_defs.md#outputtypedef)
- [TN3270OutputTypeDef](./type_defs.md#tn3270outputtypedef)
- [TN3270TypeDef](./type_defs.md#tn3270typedef)
- [TestCasesUnionTypeDef](./type_defs.md#testcasesuniontypedef)
- [CompareDataSetsSummaryTypeDef](./type_defs.md#comparedatasetssummarytypedef)
- [ResourceTypeTypeDef](./type_defs.md#resourcetypetypedef)
- [CompareDatabaseCDCSummaryTypeDef](./type_defs.md#comparedatabasecdcsummarytypedef)
- [FileMetadataOutputTypeDef](./type_defs.md#filemetadataoutputtypedef)
- [FileMetadataTypeDef](./type_defs.md#filemetadatatypedef)
- [CloudFormationStepSummaryTypeDef](./type_defs.md#cloudformationstepsummarytypedef)
- [ResourceActionTypeDef](./type_defs.md#resourceactiontypedef)
- [M2ManagedApplicationStepSummaryTypeDef](./type_defs.md#m2managedapplicationstepsummarytypedef)
- [BatchStepInputTypeDef](./type_defs.md#batchstepinputtypedef)
- [TN3270StepInputTypeDef](./type_defs.md#tn3270stepinputtypedef)
- [ResourceOutputTypeDef](./type_defs.md#resourceoutputtypedef)
- [MainframeActionTypeOutputTypeDef](./type_defs.md#mainframeactiontypeoutputtypedef)
- [TN3270UnionTypeDef](./type_defs.md#tn3270uniontypedef)
- [ResourceTypeUnionTypeDef](./type_defs.md#resourcetypeuniontypedef)
- [CompareFileTypeTypeDef](./type_defs.md#comparefiletypetypedef)
- [InputFileOutputTypeDef](./type_defs.md#inputfileoutputtypedef)
- [FileMetadataUnionTypeDef](./type_defs.md#filemetadatauniontypedef)
- [ResourceActionSummaryTypeDef](./type_defs.md#resourceactionsummarytypedef)
- [BatchSummaryTypeDef](./type_defs.md#batchsummarytypedef)
- [TN3270SummaryTypeDef](./type_defs.md#tn3270summarytypedef)
- [GetTestConfigurationResponseTypeDef](./type_defs.md#gettestconfigurationresponsetypedef)
- [MainframeActionOutputTypeDef](./type_defs.md#mainframeactionoutputtypedef)
- [MainframeActionTypeTypeDef](./type_defs.md#mainframeactiontypetypedef)
- [ResourceTypeDef](./type_defs.md#resourcetypedef)
- [FileTypeDef](./type_defs.md#filetypedef)
- [InputOutputTypeDef](./type_defs.md#inputoutputtypedef)
- [InputFileTypeDef](./type_defs.md#inputfiletypedef)
- [MainframeActionSummaryTypeDef](./type_defs.md#mainframeactionsummarytypedef)
- [MainframeActionTypeUnionTypeDef](./type_defs.md#mainframeactiontypeuniontypedef)
- [ResourceUnionTypeDef](./type_defs.md#resourceuniontypedef)
- [CompareActionSummaryTypeDef](./type_defs.md#compareactionsummarytypedef)
- [CompareActionOutputTypeDef](./type_defs.md#compareactionoutputtypedef)
- [InputFileUnionTypeDef](./type_defs.md#inputfileuniontypedef)
- [MainframeActionTypeDef](./type_defs.md#mainframeactiontypedef)
- [CreateTestConfigurationRequestTypeDef](./type_defs.md#createtestconfigurationrequesttypedef)
- [UpdateTestConfigurationRequestTypeDef](./type_defs.md#updatetestconfigurationrequesttypedef)
- [StepRunSummaryTypeDef](./type_defs.md#steprunsummarytypedef)
- [StepActionOutputTypeDef](./type_defs.md#stepactionoutputtypedef)
- [InputTypeDef](./type_defs.md#inputtypedef)
- [MainframeActionUnionTypeDef](./type_defs.md#mainframeactionuniontypedef)
- [GetTestRunStepResponseTypeDef](./type_defs.md#gettestrunstepresponsetypedef)
- [StepOutputTypeDef](./type_defs.md#stepoutputtypedef)
- [InputUnionTypeDef](./type_defs.md#inputuniontypedef)
- [GetTestCaseResponseTypeDef](./type_defs.md#gettestcaseresponsetypedef)
- [GetTestSuiteResponseTypeDef](./type_defs.md#gettestsuiteresponsetypedef)
- [CompareActionTypeDef](./type_defs.md#compareactiontypedef)
- [CompareActionUnionTypeDef](./type_defs.md#compareactionuniontypedef)
- [StepActionTypeDef](./type_defs.md#stepactiontypedef)
- [StepActionUnionTypeDef](./type_defs.md#stepactionuniontypedef)
- [StepTypeDef](./type_defs.md#steptypedef)
- [StepUnionTypeDef](./type_defs.md#stepuniontypedef)
- [CreateTestCaseRequestTypeDef](./type_defs.md#createtestcaserequesttypedef)
- [CreateTestSuiteRequestTypeDef](./type_defs.md#createtestsuiterequesttypedef)
- [UpdateTestCaseRequestTypeDef](./type_defs.md#updatetestcaserequesttypedef)
- [UpdateTestSuiteRequestTypeDef](./type_defs.md#updatetestsuiterequesttypedef)

