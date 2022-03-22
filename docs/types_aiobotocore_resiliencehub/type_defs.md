<a id="typed-dictionaries-for-aiobotocore-resiliencehub-module"></a>

# Typed dictionaries for aiobotocore ResilienceHub module

> [Index](../README.md) > [ResilienceHub](./README.md) > Typed dictionaries

Auto-generated documentation for
[ResilienceHub](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/resiliencehub.html#ResilienceHub)
type annotations stubs module
[types-aiobotocore-resiliencehub](https://pypi.org/project/types-aiobotocore-resiliencehub/).

- [Typed dictionaries for aiobotocore ResilienceHub module](#typed-dictionaries-for-aiobotocore-resiliencehub-module)
  - [AddDraftAppVersionResourceMappingsRequestRequestTypeDef](#adddraftappversionresourcemappingsrequestrequesttypedef)
  - [AddDraftAppVersionResourceMappingsResponseTypeDef](#adddraftappversionresourcemappingsresponsetypedef)
  - [AlarmRecommendationTypeDef](#alarmrecommendationtypedef)
  - [AppAssessmentSummaryTypeDef](#appassessmentsummarytypedef)
  - [AppAssessmentTypeDef](#appassessmenttypedef)
  - [AppComponentComplianceTypeDef](#appcomponentcompliancetypedef)
  - [AppComponentTypeDef](#appcomponenttypedef)
  - [AppSummaryTypeDef](#appsummarytypedef)
  - [AppTypeDef](#apptypedef)
  - [AppVersionSummaryTypeDef](#appversionsummarytypedef)
  - [ComponentRecommendationTypeDef](#componentrecommendationtypedef)
  - [ConfigRecommendationTypeDef](#configrecommendationtypedef)
  - [CostTypeDef](#costtypedef)
  - [CreateAppRequestRequestTypeDef](#createapprequestrequesttypedef)
  - [CreateAppResponseTypeDef](#createappresponsetypedef)
  - [CreateRecommendationTemplateRequestRequestTypeDef](#createrecommendationtemplaterequestrequesttypedef)
  - [CreateRecommendationTemplateResponseTypeDef](#createrecommendationtemplateresponsetypedef)
  - [CreateResiliencyPolicyRequestRequestTypeDef](#createresiliencypolicyrequestrequesttypedef)
  - [CreateResiliencyPolicyResponseTypeDef](#createresiliencypolicyresponsetypedef)
  - [DeleteAppAssessmentRequestRequestTypeDef](#deleteappassessmentrequestrequesttypedef)
  - [DeleteAppAssessmentResponseTypeDef](#deleteappassessmentresponsetypedef)
  - [DeleteAppRequestRequestTypeDef](#deleteapprequestrequesttypedef)
  - [DeleteAppResponseTypeDef](#deleteappresponsetypedef)
  - [DeleteRecommendationTemplateRequestRequestTypeDef](#deleterecommendationtemplaterequestrequesttypedef)
  - [DeleteRecommendationTemplateResponseTypeDef](#deleterecommendationtemplateresponsetypedef)
  - [DeleteResiliencyPolicyRequestRequestTypeDef](#deleteresiliencypolicyrequestrequesttypedef)
  - [DeleteResiliencyPolicyResponseTypeDef](#deleteresiliencypolicyresponsetypedef)
  - [DescribeAppAssessmentRequestRequestTypeDef](#describeappassessmentrequestrequesttypedef)
  - [DescribeAppAssessmentResponseTypeDef](#describeappassessmentresponsetypedef)
  - [DescribeAppRequestRequestTypeDef](#describeapprequestrequesttypedef)
  - [DescribeAppResponseTypeDef](#describeappresponsetypedef)
  - [DescribeAppVersionResourcesResolutionStatusRequestRequestTypeDef](#describeappversionresourcesresolutionstatusrequestrequesttypedef)
  - [DescribeAppVersionResourcesResolutionStatusResponseTypeDef](#describeappversionresourcesresolutionstatusresponsetypedef)
  - [DescribeAppVersionTemplateRequestRequestTypeDef](#describeappversiontemplaterequestrequesttypedef)
  - [DescribeAppVersionTemplateResponseTypeDef](#describeappversiontemplateresponsetypedef)
  - [DescribeDraftAppVersionResourcesImportStatusRequestRequestTypeDef](#describedraftappversionresourcesimportstatusrequestrequesttypedef)
  - [DescribeDraftAppVersionResourcesImportStatusResponseTypeDef](#describedraftappversionresourcesimportstatusresponsetypedef)
  - [DescribeResiliencyPolicyRequestRequestTypeDef](#describeresiliencypolicyrequestrequesttypedef)
  - [DescribeResiliencyPolicyResponseTypeDef](#describeresiliencypolicyresponsetypedef)
  - [DisruptionComplianceTypeDef](#disruptioncompliancetypedef)
  - [FailurePolicyTypeDef](#failurepolicytypedef)
  - [ImportResourcesToDraftAppVersionRequestRequestTypeDef](#importresourcestodraftappversionrequestrequesttypedef)
  - [ImportResourcesToDraftAppVersionResponseTypeDef](#importresourcestodraftappversionresponsetypedef)
  - [ListAlarmRecommendationsRequestRequestTypeDef](#listalarmrecommendationsrequestrequesttypedef)
  - [ListAlarmRecommendationsResponseTypeDef](#listalarmrecommendationsresponsetypedef)
  - [ListAppAssessmentsRequestRequestTypeDef](#listappassessmentsrequestrequesttypedef)
  - [ListAppAssessmentsResponseTypeDef](#listappassessmentsresponsetypedef)
  - [ListAppComponentCompliancesRequestRequestTypeDef](#listappcomponentcompliancesrequestrequesttypedef)
  - [ListAppComponentCompliancesResponseTypeDef](#listappcomponentcompliancesresponsetypedef)
  - [ListAppComponentRecommendationsRequestRequestTypeDef](#listappcomponentrecommendationsrequestrequesttypedef)
  - [ListAppComponentRecommendationsResponseTypeDef](#listappcomponentrecommendationsresponsetypedef)
  - [ListAppVersionResourceMappingsRequestRequestTypeDef](#listappversionresourcemappingsrequestrequesttypedef)
  - [ListAppVersionResourceMappingsResponseTypeDef](#listappversionresourcemappingsresponsetypedef)
  - [ListAppVersionResourcesRequestRequestTypeDef](#listappversionresourcesrequestrequesttypedef)
  - [ListAppVersionResourcesResponseTypeDef](#listappversionresourcesresponsetypedef)
  - [ListAppVersionsRequestRequestTypeDef](#listappversionsrequestrequesttypedef)
  - [ListAppVersionsResponseTypeDef](#listappversionsresponsetypedef)
  - [ListAppsRequestRequestTypeDef](#listappsrequestrequesttypedef)
  - [ListAppsResponseTypeDef](#listappsresponsetypedef)
  - [ListRecommendationTemplatesRequestRequestTypeDef](#listrecommendationtemplatesrequestrequesttypedef)
  - [ListRecommendationTemplatesResponseTypeDef](#listrecommendationtemplatesresponsetypedef)
  - [ListResiliencyPoliciesRequestRequestTypeDef](#listresiliencypoliciesrequestrequesttypedef)
  - [ListResiliencyPoliciesResponseTypeDef](#listresiliencypoliciesresponsetypedef)
  - [ListSopRecommendationsRequestRequestTypeDef](#listsoprecommendationsrequestrequesttypedef)
  - [ListSopRecommendationsResponseTypeDef](#listsoprecommendationsresponsetypedef)
  - [ListSuggestedResiliencyPoliciesRequestRequestTypeDef](#listsuggestedresiliencypoliciesrequestrequesttypedef)
  - [ListSuggestedResiliencyPoliciesResponseTypeDef](#listsuggestedresiliencypoliciesresponsetypedef)
  - [ListTagsForResourceRequestRequestTypeDef](#listtagsforresourcerequestrequesttypedef)
  - [ListTagsForResourceResponseTypeDef](#listtagsforresourceresponsetypedef)
  - [ListTestRecommendationsRequestRequestTypeDef](#listtestrecommendationsrequestrequesttypedef)
  - [ListTestRecommendationsResponseTypeDef](#listtestrecommendationsresponsetypedef)
  - [ListUnsupportedAppVersionResourcesRequestRequestTypeDef](#listunsupportedappversionresourcesrequestrequesttypedef)
  - [ListUnsupportedAppVersionResourcesResponseTypeDef](#listunsupportedappversionresourcesresponsetypedef)
  - [LogicalResourceIdTypeDef](#logicalresourceidtypedef)
  - [PhysicalResourceIdTypeDef](#physicalresourceidtypedef)
  - [PhysicalResourceTypeDef](#physicalresourcetypedef)
  - [PublishAppVersionRequestRequestTypeDef](#publishappversionrequestrequesttypedef)
  - [PublishAppVersionResponseTypeDef](#publishappversionresponsetypedef)
  - [PutDraftAppVersionTemplateRequestRequestTypeDef](#putdraftappversiontemplaterequestrequesttypedef)
  - [PutDraftAppVersionTemplateResponseTypeDef](#putdraftappversiontemplateresponsetypedef)
  - [RecommendationDisruptionComplianceTypeDef](#recommendationdisruptioncompliancetypedef)
  - [RecommendationItemTypeDef](#recommendationitemtypedef)
  - [RecommendationTemplateTypeDef](#recommendationtemplatetypedef)
  - [RemoveDraftAppVersionResourceMappingsRequestRequestTypeDef](#removedraftappversionresourcemappingsrequestrequesttypedef)
  - [RemoveDraftAppVersionResourceMappingsResponseTypeDef](#removedraftappversionresourcemappingsresponsetypedef)
  - [ResiliencyPolicyTypeDef](#resiliencypolicytypedef)
  - [ResiliencyScoreTypeDef](#resiliencyscoretypedef)
  - [ResolveAppVersionResourcesRequestRequestTypeDef](#resolveappversionresourcesrequestrequesttypedef)
  - [ResolveAppVersionResourcesResponseTypeDef](#resolveappversionresourcesresponsetypedef)
  - [ResourceMappingTypeDef](#resourcemappingtypedef)
  - [ResponseMetadataTypeDef](#responsemetadatatypedef)
  - [S3LocationTypeDef](#s3locationtypedef)
  - [SopRecommendationTypeDef](#soprecommendationtypedef)
  - [StartAppAssessmentRequestRequestTypeDef](#startappassessmentrequestrequesttypedef)
  - [StartAppAssessmentResponseTypeDef](#startappassessmentresponsetypedef)
  - [TagResourceRequestRequestTypeDef](#tagresourcerequestrequesttypedef)
  - [TestRecommendationTypeDef](#testrecommendationtypedef)
  - [UnsupportedResourceTypeDef](#unsupportedresourcetypedef)
  - [UntagResourceRequestRequestTypeDef](#untagresourcerequestrequesttypedef)
  - [UpdateAppRequestRequestTypeDef](#updateapprequestrequesttypedef)
  - [UpdateAppResponseTypeDef](#updateappresponsetypedef)
  - [UpdateResiliencyPolicyRequestRequestTypeDef](#updateresiliencypolicyrequestrequesttypedef)
  - [UpdateResiliencyPolicyResponseTypeDef](#updateresiliencypolicyresponsetypedef)

<a id="adddraftappversionresourcemappingsrequestrequesttypedef"></a>

## AddDraftAppVersionResourceMappingsRequestRequestTypeDef

```python
from types_aiobotocore_resiliencehub.type_defs import AddDraftAppVersionResourceMappingsRequestRequestTypeDef
```

Required fields:

- `appArn`: `str`
- `resourceMappings`:
  `Sequence`\[[ResourceMappingTypeDef](./type_defs.md#resourcemappingtypedef)\]

<a id="adddraftappversionresourcemappingsresponsetypedef"></a>

## AddDraftAppVersionResourceMappingsResponseTypeDef

```python
from types_aiobotocore_resiliencehub.type_defs import AddDraftAppVersionResourceMappingsResponseTypeDef
```

Required fields:

- `appArn`: `str`
- `appVersion`: `str`
- `resourceMappings`:
  `List`\[[ResourceMappingTypeDef](./type_defs.md#resourcemappingtypedef)\]
- `ResponseMetadata`:
  [ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef)

<a id="alarmrecommendationtypedef"></a>

## AlarmRecommendationTypeDef

```python
from types_aiobotocore_resiliencehub.type_defs import AlarmRecommendationTypeDef
```

Required fields:

- `name`: `str`
- `recommendationId`: `str`
- `referenceId`: `str`
- `type`: [AlarmTypeType](./literals.md#alarmtypetype)

Optional fields:

- `appComponentName`: `str`
- `description`: `str`
- `items`:
  `List`\[[RecommendationItemTypeDef](./type_defs.md#recommendationitemtypedef)\]
- `prerequisite`: `str`

<a id="appassessmentsummarytypedef"></a>

## AppAssessmentSummaryTypeDef

```python
from types_aiobotocore_resiliencehub.type_defs import AppAssessmentSummaryTypeDef
```

Required fields:

- `assessmentArn`: `str`
- `assessmentStatus`:
  [AssessmentStatusType](./literals.md#assessmentstatustype)

Optional fields:

- `appArn`: `str`
- `appVersion`: `str`
- `assessmentName`: `str`
- `complianceStatus`:
  [ComplianceStatusType](./literals.md#compliancestatustype)
- `cost`: [CostTypeDef](./type_defs.md#costtypedef)
- `endTime`: `datetime`
- `invoker`: [AssessmentInvokerType](./literals.md#assessmentinvokertype)
- `message`: `str`
- `resiliencyScore`: `float`
- `startTime`: `datetime`

<a id="appassessmenttypedef"></a>

## AppAssessmentTypeDef

```python
from types_aiobotocore_resiliencehub.type_defs import AppAssessmentTypeDef
```

Required fields:

- `assessmentArn`: `str`
- `assessmentStatus`:
  [AssessmentStatusType](./literals.md#assessmentstatustype)
- `invoker`: [AssessmentInvokerType](./literals.md#assessmentinvokertype)

Optional fields:

- `appArn`: `str`
- `appVersion`: `str`
- `assessmentName`: `str`
- `compliance`: `Dict`\[[DisruptionTypeType](./literals.md#disruptiontypetype),
  [DisruptionComplianceTypeDef](./type_defs.md#disruptioncompliancetypedef)\]
- `complianceStatus`:
  [ComplianceStatusType](./literals.md#compliancestatustype)
- `cost`: [CostTypeDef](./type_defs.md#costtypedef)
- `endTime`: `datetime`
- `message`: `str`
- `policy`: [ResiliencyPolicyTypeDef](./type_defs.md#resiliencypolicytypedef)
- `resiliencyScore`:
  [ResiliencyScoreTypeDef](./type_defs.md#resiliencyscoretypedef)
- `startTime`: `datetime`
- `tags`: `Dict`\[`str`, `str`\]

<a id="appcomponentcompliancetypedef"></a>

## AppComponentComplianceTypeDef

```python
from types_aiobotocore_resiliencehub.type_defs import AppComponentComplianceTypeDef
```

Optional fields:

- `appComponentName`: `str`
- `compliance`: `Dict`\[[DisruptionTypeType](./literals.md#disruptiontypetype),
  [DisruptionComplianceTypeDef](./type_defs.md#disruptioncompliancetypedef)\]
- `cost`: [CostTypeDef](./type_defs.md#costtypedef)
- `message`: `str`
- `resiliencyScore`:
  [ResiliencyScoreTypeDef](./type_defs.md#resiliencyscoretypedef)
- `status`: [ComplianceStatusType](./literals.md#compliancestatustype)

<a id="appcomponenttypedef"></a>

## AppComponentTypeDef

```python
from types_aiobotocore_resiliencehub.type_defs import AppComponentTypeDef
```

Required fields:

- `name`: `str`
- `type`: `str`

<a id="appsummarytypedef"></a>

## AppSummaryTypeDef

```python
from types_aiobotocore_resiliencehub.type_defs import AppSummaryTypeDef
```

Required fields:

- `appArn`: `str`
- `creationTime`: `datetime`
- `name`: `str`

Optional fields:

- `complianceStatus`:
  [AppComplianceStatusTypeType](./literals.md#appcompliancestatustypetype)
- `description`: `str`
- `resiliencyScore`: `float`

<a id="apptypedef"></a>

## AppTypeDef

```python
from types_aiobotocore_resiliencehub.type_defs import AppTypeDef
```

Required fields:

- `appArn`: `str`
- `creationTime`: `datetime`
- `name`: `str`

Optional fields:

- `complianceStatus`:
  [AppComplianceStatusTypeType](./literals.md#appcompliancestatustypetype)
- `description`: `str`
- `lastAppComplianceEvaluationTime`: `datetime`
- `lastResiliencyScoreEvaluationTime`: `datetime`
- `policyArn`: `str`
- `resiliencyScore`: `float`
- `status`: [AppStatusTypeType](./literals.md#appstatustypetype)
- `tags`: `Dict`\[`str`, `str`\]

<a id="appversionsummarytypedef"></a>

## AppVersionSummaryTypeDef

```python
from types_aiobotocore_resiliencehub.type_defs import AppVersionSummaryTypeDef
```

Required fields:

- `appVersion`: `str`

<a id="componentrecommendationtypedef"></a>

## ComponentRecommendationTypeDef

```python
from types_aiobotocore_resiliencehub.type_defs import ComponentRecommendationTypeDef
```

Required fields:

- `appComponentName`: `str`
- `configRecommendations`:
  `List`\[[ConfigRecommendationTypeDef](./type_defs.md#configrecommendationtypedef)\]
- `recommendationStatus`:
  [RecommendationComplianceStatusType](./literals.md#recommendationcompliancestatustype)

<a id="configrecommendationtypedef"></a>

## ConfigRecommendationTypeDef

```python
from types_aiobotocore_resiliencehub.type_defs import ConfigRecommendationTypeDef
```

Required fields:

- `name`: `str`
- `optimizationType`:
  [ConfigRecommendationOptimizationTypeType](./literals.md#configrecommendationoptimizationtypetype)
- `referenceId`: `str`

Optional fields:

- `appComponentName`: `str`
- `compliance`: `Dict`\[[DisruptionTypeType](./literals.md#disruptiontypetype),
  [DisruptionComplianceTypeDef](./type_defs.md#disruptioncompliancetypedef)\]
- `cost`: [CostTypeDef](./type_defs.md#costtypedef)
- `description`: `str`
- `haArchitecture`: [HaArchitectureType](./literals.md#haarchitecturetype)
- `recommendationCompliance`:
  `Dict`\[[DisruptionTypeType](./literals.md#disruptiontypetype),
  [RecommendationDisruptionComplianceTypeDef](./type_defs.md#recommendationdisruptioncompliancetypedef)\]
- `suggestedChanges`: `List`\[`str`\]

<a id="costtypedef"></a>

## CostTypeDef

```python
from types_aiobotocore_resiliencehub.type_defs import CostTypeDef
```

Required fields:

- `amount`: `float`
- `currency`: `str`
- `frequency`: [CostFrequencyType](./literals.md#costfrequencytype)

<a id="createapprequestrequesttypedef"></a>

## CreateAppRequestRequestTypeDef

```python
from types_aiobotocore_resiliencehub.type_defs import CreateAppRequestRequestTypeDef
```

Required fields:

- `name`: `str`

Optional fields:

- `clientToken`: `str`
- `description`: `str`
- `policyArn`: `str`
- `tags`: `Mapping`\[`str`, `str`\]

<a id="createappresponsetypedef"></a>

## CreateAppResponseTypeDef

```python
from types_aiobotocore_resiliencehub.type_defs import CreateAppResponseTypeDef
```

Required fields:

- `app`: [AppTypeDef](./type_defs.md#apptypedef)
- `ResponseMetadata`:
  [ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef)

<a id="createrecommendationtemplaterequestrequesttypedef"></a>

## CreateRecommendationTemplateRequestRequestTypeDef

```python
from types_aiobotocore_resiliencehub.type_defs import CreateRecommendationTemplateRequestRequestTypeDef
```

Required fields:

- `assessmentArn`: `str`
- `name`: `str`

Optional fields:

- `bucketName`: `str`
- `clientToken`: `str`
- `format`: [TemplateFormatType](./literals.md#templateformattype)
- `recommendationIds`: `Sequence`\[`str`\]
- `recommendationTypes`:
  `Sequence`\[[RenderRecommendationTypeType](./literals.md#renderrecommendationtypetype)\]
- `tags`: `Mapping`\[`str`, `str`\]

<a id="createrecommendationtemplateresponsetypedef"></a>

## CreateRecommendationTemplateResponseTypeDef

```python
from types_aiobotocore_resiliencehub.type_defs import CreateRecommendationTemplateResponseTypeDef
```

Required fields:

- `recommendationTemplate`:
  [RecommendationTemplateTypeDef](./type_defs.md#recommendationtemplatetypedef)
- `ResponseMetadata`:
  [ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef)

<a id="createresiliencypolicyrequestrequesttypedef"></a>

## CreateResiliencyPolicyRequestRequestTypeDef

```python
from types_aiobotocore_resiliencehub.type_defs import CreateResiliencyPolicyRequestRequestTypeDef
```

Required fields:

- `policy`: `Mapping`\[[DisruptionTypeType](./literals.md#disruptiontypetype),
  [FailurePolicyTypeDef](./type_defs.md#failurepolicytypedef)\]
- `policyName`: `str`
- `tier`: [ResiliencyPolicyTierType](./literals.md#resiliencypolicytiertype)

Optional fields:

- `clientToken`: `str`
- `dataLocationConstraint`:
  [DataLocationConstraintType](./literals.md#datalocationconstrainttype)
- `policyDescription`: `str`
- `tags`: `Mapping`\[`str`, `str`\]

<a id="createresiliencypolicyresponsetypedef"></a>

## CreateResiliencyPolicyResponseTypeDef

```python
from types_aiobotocore_resiliencehub.type_defs import CreateResiliencyPolicyResponseTypeDef
```

Required fields:

- `policy`: [ResiliencyPolicyTypeDef](./type_defs.md#resiliencypolicytypedef)
- `ResponseMetadata`:
  [ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef)

<a id="deleteappassessmentrequestrequesttypedef"></a>

## DeleteAppAssessmentRequestRequestTypeDef

```python
from types_aiobotocore_resiliencehub.type_defs import DeleteAppAssessmentRequestRequestTypeDef
```

Required fields:

- `assessmentArn`: `str`

Optional fields:

- `clientToken`: `str`

<a id="deleteappassessmentresponsetypedef"></a>

## DeleteAppAssessmentResponseTypeDef

```python
from types_aiobotocore_resiliencehub.type_defs import DeleteAppAssessmentResponseTypeDef
```

Required fields:

- `assessmentArn`: `str`
- `assessmentStatus`:
  [AssessmentStatusType](./literals.md#assessmentstatustype)
- `ResponseMetadata`:
  [ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef)

<a id="deleteapprequestrequesttypedef"></a>

## DeleteAppRequestRequestTypeDef

```python
from types_aiobotocore_resiliencehub.type_defs import DeleteAppRequestRequestTypeDef
```

Required fields:

- `appArn`: `str`

Optional fields:

- `clientToken`: `str`
- `forceDelete`: `bool`

<a id="deleteappresponsetypedef"></a>

## DeleteAppResponseTypeDef

```python
from types_aiobotocore_resiliencehub.type_defs import DeleteAppResponseTypeDef
```

Required fields:

- `appArn`: `str`
- `ResponseMetadata`:
  [ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef)

<a id="deleterecommendationtemplaterequestrequesttypedef"></a>

## DeleteRecommendationTemplateRequestRequestTypeDef

```python
from types_aiobotocore_resiliencehub.type_defs import DeleteRecommendationTemplateRequestRequestTypeDef
```

Required fields:

- `recommendationTemplateArn`: `str`

Optional fields:

- `clientToken`: `str`

<a id="deleterecommendationtemplateresponsetypedef"></a>

## DeleteRecommendationTemplateResponseTypeDef

```python
from types_aiobotocore_resiliencehub.type_defs import DeleteRecommendationTemplateResponseTypeDef
```

Required fields:

- `recommendationTemplateArn`: `str`
- `status`:
  [RecommendationTemplateStatusType](./literals.md#recommendationtemplatestatustype)
- `ResponseMetadata`:
  [ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef)

<a id="deleteresiliencypolicyrequestrequesttypedef"></a>

## DeleteResiliencyPolicyRequestRequestTypeDef

```python
from types_aiobotocore_resiliencehub.type_defs import DeleteResiliencyPolicyRequestRequestTypeDef
```

Required fields:

- `policyArn`: `str`

Optional fields:

- `clientToken`: `str`

<a id="deleteresiliencypolicyresponsetypedef"></a>

## DeleteResiliencyPolicyResponseTypeDef

```python
from types_aiobotocore_resiliencehub.type_defs import DeleteResiliencyPolicyResponseTypeDef
```

Required fields:

- `policyArn`: `str`
- `ResponseMetadata`:
  [ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef)

<a id="describeappassessmentrequestrequesttypedef"></a>

## DescribeAppAssessmentRequestRequestTypeDef

```python
from types_aiobotocore_resiliencehub.type_defs import DescribeAppAssessmentRequestRequestTypeDef
```

Required fields:

- `assessmentArn`: `str`

<a id="describeappassessmentresponsetypedef"></a>

## DescribeAppAssessmentResponseTypeDef

```python
from types_aiobotocore_resiliencehub.type_defs import DescribeAppAssessmentResponseTypeDef
```

Required fields:

- `assessment`: [AppAssessmentTypeDef](./type_defs.md#appassessmenttypedef)
- `ResponseMetadata`:
  [ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef)

<a id="describeapprequestrequesttypedef"></a>

## DescribeAppRequestRequestTypeDef

```python
from types_aiobotocore_resiliencehub.type_defs import DescribeAppRequestRequestTypeDef
```

Required fields:

- `appArn`: `str`

<a id="describeappresponsetypedef"></a>

## DescribeAppResponseTypeDef

```python
from types_aiobotocore_resiliencehub.type_defs import DescribeAppResponseTypeDef
```

Required fields:

- `app`: [AppTypeDef](./type_defs.md#apptypedef)
- `ResponseMetadata`:
  [ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef)

<a id="describeappversionresourcesresolutionstatusrequestrequesttypedef"></a>

## DescribeAppVersionResourcesResolutionStatusRequestRequestTypeDef

```python
from types_aiobotocore_resiliencehub.type_defs import DescribeAppVersionResourcesResolutionStatusRequestRequestTypeDef
```

Required fields:

- `appArn`: `str`
- `appVersion`: `str`

Optional fields:

- `resolutionId`: `str`

<a id="describeappversionresourcesresolutionstatusresponsetypedef"></a>

## DescribeAppVersionResourcesResolutionStatusResponseTypeDef

```python
from types_aiobotocore_resiliencehub.type_defs import DescribeAppVersionResourcesResolutionStatusResponseTypeDef
```

Required fields:

- `appArn`: `str`
- `appVersion`: `str`
- `errorMessage`: `str`
- `resolutionId`: `str`
- `status`:
  [ResourceResolutionStatusTypeType](./literals.md#resourceresolutionstatustypetype)
- `ResponseMetadata`:
  [ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef)

<a id="describeappversiontemplaterequestrequesttypedef"></a>

## DescribeAppVersionTemplateRequestRequestTypeDef

```python
from types_aiobotocore_resiliencehub.type_defs import DescribeAppVersionTemplateRequestRequestTypeDef
```

Required fields:

- `appArn`: `str`
- `appVersion`: `str`

<a id="describeappversiontemplateresponsetypedef"></a>

## DescribeAppVersionTemplateResponseTypeDef

```python
from types_aiobotocore_resiliencehub.type_defs import DescribeAppVersionTemplateResponseTypeDef
```

Required fields:

- `appArn`: `str`
- `appTemplateBody`: `str`
- `appVersion`: `str`
- `ResponseMetadata`:
  [ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef)

<a id="describedraftappversionresourcesimportstatusrequestrequesttypedef"></a>

## DescribeDraftAppVersionResourcesImportStatusRequestRequestTypeDef

```python
from types_aiobotocore_resiliencehub.type_defs import DescribeDraftAppVersionResourcesImportStatusRequestRequestTypeDef
```

Required fields:

- `appArn`: `str`

<a id="describedraftappversionresourcesimportstatusresponsetypedef"></a>

## DescribeDraftAppVersionResourcesImportStatusResponseTypeDef

```python
from types_aiobotocore_resiliencehub.type_defs import DescribeDraftAppVersionResourcesImportStatusResponseTypeDef
```

Required fields:

- `appArn`: `str`
- `appVersion`: `str`
- `errorMessage`: `str`
- `status`:
  [ResourceImportStatusTypeType](./literals.md#resourceimportstatustypetype)
- `statusChangeTime`: `datetime`
- `ResponseMetadata`:
  [ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef)

<a id="describeresiliencypolicyrequestrequesttypedef"></a>

## DescribeResiliencyPolicyRequestRequestTypeDef

```python
from types_aiobotocore_resiliencehub.type_defs import DescribeResiliencyPolicyRequestRequestTypeDef
```

Required fields:

- `policyArn`: `str`

<a id="describeresiliencypolicyresponsetypedef"></a>

## DescribeResiliencyPolicyResponseTypeDef

```python
from types_aiobotocore_resiliencehub.type_defs import DescribeResiliencyPolicyResponseTypeDef
```

Required fields:

- `policy`: [ResiliencyPolicyTypeDef](./type_defs.md#resiliencypolicytypedef)
- `ResponseMetadata`:
  [ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef)

<a id="disruptioncompliancetypedef"></a>

## DisruptionComplianceTypeDef

```python
from types_aiobotocore_resiliencehub.type_defs import DisruptionComplianceTypeDef
```

Required fields:

- `complianceStatus`:
  [ComplianceStatusType](./literals.md#compliancestatustype)

Optional fields:

- `achievableRpoInSecs`: `int`
- `achievableRtoInSecs`: `int`
- `currentRpoInSecs`: `int`
- `currentRtoInSecs`: `int`
- `message`: `str`
- `rpoDescription`: `str`
- `rpoReferenceId`: `str`
- `rtoDescription`: `str`
- `rtoReferenceId`: `str`

<a id="failurepolicytypedef"></a>

## FailurePolicyTypeDef

```python
from types_aiobotocore_resiliencehub.type_defs import FailurePolicyTypeDef
```

Required fields:

- `rpoInSecs`: `int`
- `rtoInSecs`: `int`

<a id="importresourcestodraftappversionrequestrequesttypedef"></a>

## ImportResourcesToDraftAppVersionRequestRequestTypeDef

```python
from types_aiobotocore_resiliencehub.type_defs import ImportResourcesToDraftAppVersionRequestRequestTypeDef
```

Required fields:

- `appArn`: `str`
- `sourceArns`: `Sequence`\[`str`\]

<a id="importresourcestodraftappversionresponsetypedef"></a>

## ImportResourcesToDraftAppVersionResponseTypeDef

```python
from types_aiobotocore_resiliencehub.type_defs import ImportResourcesToDraftAppVersionResponseTypeDef
```

Required fields:

- `appArn`: `str`
- `appVersion`: `str`
- `sourceArns`: `List`\[`str`\]
- `status`:
  [ResourceImportStatusTypeType](./literals.md#resourceimportstatustypetype)
- `ResponseMetadata`:
  [ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef)

<a id="listalarmrecommendationsrequestrequesttypedef"></a>

## ListAlarmRecommendationsRequestRequestTypeDef

```python
from types_aiobotocore_resiliencehub.type_defs import ListAlarmRecommendationsRequestRequestTypeDef
```

Required fields:

- `assessmentArn`: `str`

Optional fields:

- `maxResults`: `int`
- `nextToken`: `str`

<a id="listalarmrecommendationsresponsetypedef"></a>

## ListAlarmRecommendationsResponseTypeDef

```python
from types_aiobotocore_resiliencehub.type_defs import ListAlarmRecommendationsResponseTypeDef
```

Required fields:

- `alarmRecommendations`:
  `List`\[[AlarmRecommendationTypeDef](./type_defs.md#alarmrecommendationtypedef)\]
- `nextToken`: `str`
- `ResponseMetadata`:
  [ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef)

<a id="listappassessmentsrequestrequesttypedef"></a>

## ListAppAssessmentsRequestRequestTypeDef

```python
from types_aiobotocore_resiliencehub.type_defs import ListAppAssessmentsRequestRequestTypeDef
```

Optional fields:

- `appArn`: `str`
- `assessmentName`: `str`
- `assessmentStatus`:
  `Sequence`\[[AssessmentStatusType](./literals.md#assessmentstatustype)\]
- `complianceStatus`:
  [ComplianceStatusType](./literals.md#compliancestatustype)
- `invoker`: [AssessmentInvokerType](./literals.md#assessmentinvokertype)
- `maxResults`: `int`
- `nextToken`: `str`
- `reverseOrder`: `bool`

<a id="listappassessmentsresponsetypedef"></a>

## ListAppAssessmentsResponseTypeDef

```python
from types_aiobotocore_resiliencehub.type_defs import ListAppAssessmentsResponseTypeDef
```

Required fields:

- `assessmentSummaries`:
  `List`\[[AppAssessmentSummaryTypeDef](./type_defs.md#appassessmentsummarytypedef)\]
- `nextToken`: `str`
- `ResponseMetadata`:
  [ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef)

<a id="listappcomponentcompliancesrequestrequesttypedef"></a>

## ListAppComponentCompliancesRequestRequestTypeDef

```python
from types_aiobotocore_resiliencehub.type_defs import ListAppComponentCompliancesRequestRequestTypeDef
```

Required fields:

- `assessmentArn`: `str`

Optional fields:

- `maxResults`: `int`
- `nextToken`: `str`

<a id="listappcomponentcompliancesresponsetypedef"></a>

## ListAppComponentCompliancesResponseTypeDef

```python
from types_aiobotocore_resiliencehub.type_defs import ListAppComponentCompliancesResponseTypeDef
```

Required fields:

- `componentCompliances`:
  `List`\[[AppComponentComplianceTypeDef](./type_defs.md#appcomponentcompliancetypedef)\]
- `nextToken`: `str`
- `ResponseMetadata`:
  [ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef)

<a id="listappcomponentrecommendationsrequestrequesttypedef"></a>

## ListAppComponentRecommendationsRequestRequestTypeDef

```python
from types_aiobotocore_resiliencehub.type_defs import ListAppComponentRecommendationsRequestRequestTypeDef
```

Required fields:

- `assessmentArn`: `str`

Optional fields:

- `maxResults`: `int`
- `nextToken`: `str`

<a id="listappcomponentrecommendationsresponsetypedef"></a>

## ListAppComponentRecommendationsResponseTypeDef

```python
from types_aiobotocore_resiliencehub.type_defs import ListAppComponentRecommendationsResponseTypeDef
```

Required fields:

- `componentRecommendations`:
  `List`\[[ComponentRecommendationTypeDef](./type_defs.md#componentrecommendationtypedef)\]
- `nextToken`: `str`
- `ResponseMetadata`:
  [ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef)

<a id="listappversionresourcemappingsrequestrequesttypedef"></a>

## ListAppVersionResourceMappingsRequestRequestTypeDef

```python
from types_aiobotocore_resiliencehub.type_defs import ListAppVersionResourceMappingsRequestRequestTypeDef
```

Required fields:

- `appArn`: `str`
- `appVersion`: `str`

Optional fields:

- `maxResults`: `int`
- `nextToken`: `str`

<a id="listappversionresourcemappingsresponsetypedef"></a>

## ListAppVersionResourceMappingsResponseTypeDef

```python
from types_aiobotocore_resiliencehub.type_defs import ListAppVersionResourceMappingsResponseTypeDef
```

Required fields:

- `nextToken`: `str`
- `resourceMappings`:
  `List`\[[ResourceMappingTypeDef](./type_defs.md#resourcemappingtypedef)\]
- `ResponseMetadata`:
  [ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef)

<a id="listappversionresourcesrequestrequesttypedef"></a>

## ListAppVersionResourcesRequestRequestTypeDef

```python
from types_aiobotocore_resiliencehub.type_defs import ListAppVersionResourcesRequestRequestTypeDef
```

Required fields:

- `appArn`: `str`
- `appVersion`: `str`

Optional fields:

- `maxResults`: `int`
- `nextToken`: `str`
- `resolutionId`: `str`

<a id="listappversionresourcesresponsetypedef"></a>

## ListAppVersionResourcesResponseTypeDef

```python
from types_aiobotocore_resiliencehub.type_defs import ListAppVersionResourcesResponseTypeDef
```

Required fields:

- `nextToken`: `str`
- `physicalResources`:
  `List`\[[PhysicalResourceTypeDef](./type_defs.md#physicalresourcetypedef)\]
- `resolutionId`: `str`
- `ResponseMetadata`:
  [ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef)

<a id="listappversionsrequestrequesttypedef"></a>

## ListAppVersionsRequestRequestTypeDef

```python
from types_aiobotocore_resiliencehub.type_defs import ListAppVersionsRequestRequestTypeDef
```

Required fields:

- `appArn`: `str`

Optional fields:

- `maxResults`: `int`
- `nextToken`: `str`

<a id="listappversionsresponsetypedef"></a>

## ListAppVersionsResponseTypeDef

```python
from types_aiobotocore_resiliencehub.type_defs import ListAppVersionsResponseTypeDef
```

Required fields:

- `appVersions`:
  `List`\[[AppVersionSummaryTypeDef](./type_defs.md#appversionsummarytypedef)\]
- `nextToken`: `str`
- `ResponseMetadata`:
  [ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef)

<a id="listappsrequestrequesttypedef"></a>

## ListAppsRequestRequestTypeDef

```python
from types_aiobotocore_resiliencehub.type_defs import ListAppsRequestRequestTypeDef
```

Optional fields:

- `appArn`: `str`
- `maxResults`: `int`
- `name`: `str`
- `nextToken`: `str`

<a id="listappsresponsetypedef"></a>

## ListAppsResponseTypeDef

```python
from types_aiobotocore_resiliencehub.type_defs import ListAppsResponseTypeDef
```

Required fields:

- `appSummaries`:
  `List`\[[AppSummaryTypeDef](./type_defs.md#appsummarytypedef)\]
- `nextToken`: `str`
- `ResponseMetadata`:
  [ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef)

<a id="listrecommendationtemplatesrequestrequesttypedef"></a>

## ListRecommendationTemplatesRequestRequestTypeDef

```python
from types_aiobotocore_resiliencehub.type_defs import ListRecommendationTemplatesRequestRequestTypeDef
```

Required fields:

- `assessmentArn`: `str`

Optional fields:

- `maxResults`: `int`
- `name`: `str`
- `nextToken`: `str`
- `recommendationTemplateArn`: `str`
- `reverseOrder`: `bool`
- `status`:
  `Sequence`\[[RecommendationTemplateStatusType](./literals.md#recommendationtemplatestatustype)\]

<a id="listrecommendationtemplatesresponsetypedef"></a>

## ListRecommendationTemplatesResponseTypeDef

```python
from types_aiobotocore_resiliencehub.type_defs import ListRecommendationTemplatesResponseTypeDef
```

Required fields:

- `nextToken`: `str`
- `recommendationTemplates`:
  `List`\[[RecommendationTemplateTypeDef](./type_defs.md#recommendationtemplatetypedef)\]
- `ResponseMetadata`:
  [ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef)

<a id="listresiliencypoliciesrequestrequesttypedef"></a>

## ListResiliencyPoliciesRequestRequestTypeDef

```python
from types_aiobotocore_resiliencehub.type_defs import ListResiliencyPoliciesRequestRequestTypeDef
```

Optional fields:

- `maxResults`: `int`
- `nextToken`: `str`
- `policyName`: `str`

<a id="listresiliencypoliciesresponsetypedef"></a>

## ListResiliencyPoliciesResponseTypeDef

```python
from types_aiobotocore_resiliencehub.type_defs import ListResiliencyPoliciesResponseTypeDef
```

Required fields:

- `nextToken`: `str`
- `resiliencyPolicies`:
  `List`\[[ResiliencyPolicyTypeDef](./type_defs.md#resiliencypolicytypedef)\]
- `ResponseMetadata`:
  [ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef)

<a id="listsoprecommendationsrequestrequesttypedef"></a>

## ListSopRecommendationsRequestRequestTypeDef

```python
from types_aiobotocore_resiliencehub.type_defs import ListSopRecommendationsRequestRequestTypeDef
```

Required fields:

- `assessmentArn`: `str`

Optional fields:

- `maxResults`: `int`
- `nextToken`: `str`

<a id="listsoprecommendationsresponsetypedef"></a>

## ListSopRecommendationsResponseTypeDef

```python
from types_aiobotocore_resiliencehub.type_defs import ListSopRecommendationsResponseTypeDef
```

Required fields:

- `nextToken`: `str`
- `sopRecommendations`:
  `List`\[[SopRecommendationTypeDef](./type_defs.md#soprecommendationtypedef)\]
- `ResponseMetadata`:
  [ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef)

<a id="listsuggestedresiliencypoliciesrequestrequesttypedef"></a>

## ListSuggestedResiliencyPoliciesRequestRequestTypeDef

```python
from types_aiobotocore_resiliencehub.type_defs import ListSuggestedResiliencyPoliciesRequestRequestTypeDef
```

Optional fields:

- `maxResults`: `int`
- `nextToken`: `str`

<a id="listsuggestedresiliencypoliciesresponsetypedef"></a>

## ListSuggestedResiliencyPoliciesResponseTypeDef

```python
from types_aiobotocore_resiliencehub.type_defs import ListSuggestedResiliencyPoliciesResponseTypeDef
```

Required fields:

- `nextToken`: `str`
- `resiliencyPolicies`:
  `List`\[[ResiliencyPolicyTypeDef](./type_defs.md#resiliencypolicytypedef)\]
- `ResponseMetadata`:
  [ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef)

<a id="listtagsforresourcerequestrequesttypedef"></a>

## ListTagsForResourceRequestRequestTypeDef

```python
from types_aiobotocore_resiliencehub.type_defs import ListTagsForResourceRequestRequestTypeDef
```

Required fields:

- `resourceArn`: `str`

<a id="listtagsforresourceresponsetypedef"></a>

## ListTagsForResourceResponseTypeDef

```python
from types_aiobotocore_resiliencehub.type_defs import ListTagsForResourceResponseTypeDef
```

Required fields:

- `tags`: `Dict`\[`str`, `str`\]
- `ResponseMetadata`:
  [ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef)

<a id="listtestrecommendationsrequestrequesttypedef"></a>

## ListTestRecommendationsRequestRequestTypeDef

```python
from types_aiobotocore_resiliencehub.type_defs import ListTestRecommendationsRequestRequestTypeDef
```

Required fields:

- `assessmentArn`: `str`

Optional fields:

- `maxResults`: `int`
- `nextToken`: `str`

<a id="listtestrecommendationsresponsetypedef"></a>

## ListTestRecommendationsResponseTypeDef

```python
from types_aiobotocore_resiliencehub.type_defs import ListTestRecommendationsResponseTypeDef
```

Required fields:

- `nextToken`: `str`
- `testRecommendations`:
  `List`\[[TestRecommendationTypeDef](./type_defs.md#testrecommendationtypedef)\]
- `ResponseMetadata`:
  [ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef)

<a id="listunsupportedappversionresourcesrequestrequesttypedef"></a>

## ListUnsupportedAppVersionResourcesRequestRequestTypeDef

```python
from types_aiobotocore_resiliencehub.type_defs import ListUnsupportedAppVersionResourcesRequestRequestTypeDef
```

Required fields:

- `appArn`: `str`
- `appVersion`: `str`

Optional fields:

- `maxResults`: `int`
- `nextToken`: `str`
- `resolutionId`: `str`

<a id="listunsupportedappversionresourcesresponsetypedef"></a>

## ListUnsupportedAppVersionResourcesResponseTypeDef

```python
from types_aiobotocore_resiliencehub.type_defs import ListUnsupportedAppVersionResourcesResponseTypeDef
```

Required fields:

- `nextToken`: `str`
- `resolutionId`: `str`
- `unsupportedResources`:
  `List`\[[UnsupportedResourceTypeDef](./type_defs.md#unsupportedresourcetypedef)\]
- `ResponseMetadata`:
  [ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef)

<a id="logicalresourceidtypedef"></a>

## LogicalResourceIdTypeDef

```python
from types_aiobotocore_resiliencehub.type_defs import LogicalResourceIdTypeDef
```

Required fields:

- `identifier`: `str`

Optional fields:

- `logicalStackName`: `str`
- `resourceGroupName`: `str`

<a id="physicalresourceidtypedef"></a>

## PhysicalResourceIdTypeDef

```python
from types_aiobotocore_resiliencehub.type_defs import PhysicalResourceIdTypeDef
```

Required fields:

- `identifier`: `str`
- `type`:
  [PhysicalIdentifierTypeType](./literals.md#physicalidentifiertypetype)

Optional fields:

- `awsAccountId`: `str`
- `awsRegion`: `str`

<a id="physicalresourcetypedef"></a>

## PhysicalResourceTypeDef

```python
from types_aiobotocore_resiliencehub.type_defs import PhysicalResourceTypeDef
```

Required fields:

- `logicalResourceId`:
  [LogicalResourceIdTypeDef](./type_defs.md#logicalresourceidtypedef)
- `physicalResourceId`:
  [PhysicalResourceIdTypeDef](./type_defs.md#physicalresourceidtypedef)
- `resourceType`: `str`

Optional fields:

- `appComponents`:
  `List`\[[AppComponentTypeDef](./type_defs.md#appcomponenttypedef)\]
- `resourceName`: `str`

<a id="publishappversionrequestrequesttypedef"></a>

## PublishAppVersionRequestRequestTypeDef

```python
from types_aiobotocore_resiliencehub.type_defs import PublishAppVersionRequestRequestTypeDef
```

Required fields:

- `appArn`: `str`

<a id="publishappversionresponsetypedef"></a>

## PublishAppVersionResponseTypeDef

```python
from types_aiobotocore_resiliencehub.type_defs import PublishAppVersionResponseTypeDef
```

Required fields:

- `appArn`: `str`
- `appVersion`: `str`
- `ResponseMetadata`:
  [ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef)

<a id="putdraftappversiontemplaterequestrequesttypedef"></a>

## PutDraftAppVersionTemplateRequestRequestTypeDef

```python
from types_aiobotocore_resiliencehub.type_defs import PutDraftAppVersionTemplateRequestRequestTypeDef
```

Required fields:

- `appArn`: `str`
- `appTemplateBody`: `str`

<a id="putdraftappversiontemplateresponsetypedef"></a>

## PutDraftAppVersionTemplateResponseTypeDef

```python
from types_aiobotocore_resiliencehub.type_defs import PutDraftAppVersionTemplateResponseTypeDef
```

Required fields:

- `appArn`: `str`
- `appVersion`: `str`
- `ResponseMetadata`:
  [ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef)

<a id="recommendationdisruptioncompliancetypedef"></a>

## RecommendationDisruptionComplianceTypeDef

```python
from types_aiobotocore_resiliencehub.type_defs import RecommendationDisruptionComplianceTypeDef
```

Required fields:

- `expectedComplianceStatus`:
  [ComplianceStatusType](./literals.md#compliancestatustype)

Optional fields:

- `expectedRpoDescription`: `str`
- `expectedRpoInSecs`: `int`
- `expectedRtoDescription`: `str`
- `expectedRtoInSecs`: `int`

<a id="recommendationitemtypedef"></a>

## RecommendationItemTypeDef

```python
from types_aiobotocore_resiliencehub.type_defs import RecommendationItemTypeDef
```

Optional fields:

- `alreadyImplemented`: `bool`
- `resourceId`: `str`
- `targetAccountId`: `str`
- `targetRegion`: `str`

<a id="recommendationtemplatetypedef"></a>

## RecommendationTemplateTypeDef

```python
from types_aiobotocore_resiliencehub.type_defs import RecommendationTemplateTypeDef
```

Required fields:

- `assessmentArn`: `str`
- `format`: [TemplateFormatType](./literals.md#templateformattype)
- `name`: `str`
- `recommendationTemplateArn`: `str`
- `recommendationTypes`:
  `List`\[[RenderRecommendationTypeType](./literals.md#renderrecommendationtypetype)\]
- `status`:
  [RecommendationTemplateStatusType](./literals.md#recommendationtemplatestatustype)

Optional fields:

- `appArn`: `str`
- `endTime`: `datetime`
- `message`: `str`
- `needsReplacements`: `bool`
- `recommendationIds`: `List`\[`str`\]
- `startTime`: `datetime`
- `tags`: `Dict`\[`str`, `str`\]
- `templatesLocation`: [S3LocationTypeDef](./type_defs.md#s3locationtypedef)

<a id="removedraftappversionresourcemappingsrequestrequesttypedef"></a>

## RemoveDraftAppVersionResourceMappingsRequestRequestTypeDef

```python
from types_aiobotocore_resiliencehub.type_defs import RemoveDraftAppVersionResourceMappingsRequestRequestTypeDef
```

Required fields:

- `appArn`: `str`

Optional fields:

- `appRegistryAppNames`: `Sequence`\[`str`\]
- `logicalStackNames`: `Sequence`\[`str`\]
- `resourceGroupNames`: `Sequence`\[`str`\]
- `resourceNames`: `Sequence`\[`str`\]

<a id="removedraftappversionresourcemappingsresponsetypedef"></a>

## RemoveDraftAppVersionResourceMappingsResponseTypeDef

```python
from types_aiobotocore_resiliencehub.type_defs import RemoveDraftAppVersionResourceMappingsResponseTypeDef
```

Required fields:

- `appArn`: `str`
- `appVersion`: `str`
- `ResponseMetadata`:
  [ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef)

<a id="resiliencypolicytypedef"></a>

## ResiliencyPolicyTypeDef

```python
from types_aiobotocore_resiliencehub.type_defs import ResiliencyPolicyTypeDef
```

Optional fields:

- `creationTime`: `datetime`
- `dataLocationConstraint`:
  [DataLocationConstraintType](./literals.md#datalocationconstrainttype)
- `estimatedCostTier`:
  [EstimatedCostTierType](./literals.md#estimatedcosttiertype)
- `policy`: `Dict`\[[DisruptionTypeType](./literals.md#disruptiontypetype),
  [FailurePolicyTypeDef](./type_defs.md#failurepolicytypedef)\]
- `policyArn`: `str`
- `policyDescription`: `str`
- `policyName`: `str`
- `tags`: `Dict`\[`str`, `str`\]
- `tier`: [ResiliencyPolicyTierType](./literals.md#resiliencypolicytiertype)

<a id="resiliencyscoretypedef"></a>

## ResiliencyScoreTypeDef

```python
from types_aiobotocore_resiliencehub.type_defs import ResiliencyScoreTypeDef
```

Required fields:

- `disruptionScore`:
  `Dict`\[[DisruptionTypeType](./literals.md#disruptiontypetype), `float`\]
- `score`: `float`

<a id="resolveappversionresourcesrequestrequesttypedef"></a>

## ResolveAppVersionResourcesRequestRequestTypeDef

```python
from types_aiobotocore_resiliencehub.type_defs import ResolveAppVersionResourcesRequestRequestTypeDef
```

Required fields:

- `appArn`: `str`
- `appVersion`: `str`

<a id="resolveappversionresourcesresponsetypedef"></a>

## ResolveAppVersionResourcesResponseTypeDef

```python
from types_aiobotocore_resiliencehub.type_defs import ResolveAppVersionResourcesResponseTypeDef
```

Required fields:

- `appArn`: `str`
- `appVersion`: `str`
- `resolutionId`: `str`
- `status`:
  [ResourceResolutionStatusTypeType](./literals.md#resourceresolutionstatustypetype)
- `ResponseMetadata`:
  [ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef)

<a id="resourcemappingtypedef"></a>

## ResourceMappingTypeDef

```python
from types_aiobotocore_resiliencehub.type_defs import ResourceMappingTypeDef
```

Required fields:

- `mappingType`:
  [ResourceMappingTypeType](./literals.md#resourcemappingtypetype)
- `physicalResourceId`:
  [PhysicalResourceIdTypeDef](./type_defs.md#physicalresourceidtypedef)

Optional fields:

- `appRegistryAppName`: `str`
- `logicalStackName`: `str`
- `resourceGroupName`: `str`
- `resourceName`: `str`

<a id="responsemetadatatypedef"></a>

## ResponseMetadataTypeDef

```python
from types_aiobotocore_resiliencehub.type_defs import ResponseMetadataTypeDef
```

Required fields:

- `RequestId`: `str`
- `HostId`: `str`
- `HTTPStatusCode`: `int`
- `HTTPHeaders`: `Dict`\[`str`, `str`\]
- `RetryAttempts`: `int`

<a id="s3locationtypedef"></a>

## S3LocationTypeDef

```python
from types_aiobotocore_resiliencehub.type_defs import S3LocationTypeDef
```

Optional fields:

- `bucket`: `str`
- `prefix`: `str`

<a id="soprecommendationtypedef"></a>

## SopRecommendationTypeDef

```python
from types_aiobotocore_resiliencehub.type_defs import SopRecommendationTypeDef
```

Required fields:

- `recommendationId`: `str`
- `referenceId`: `str`
- `serviceType`: `Literal['SSM']` (see
  [SopServiceTypeType](./literals.md#sopservicetypetype))

Optional fields:

- `appComponentName`: `str`
- `description`: `str`
- `items`:
  `List`\[[RecommendationItemTypeDef](./type_defs.md#recommendationitemtypedef)\]
- `name`: `str`
- `prerequisite`: `str`

<a id="startappassessmentrequestrequesttypedef"></a>

## StartAppAssessmentRequestRequestTypeDef

```python
from types_aiobotocore_resiliencehub.type_defs import StartAppAssessmentRequestRequestTypeDef
```

Required fields:

- `appArn`: `str`
- `appVersion`: `str`
- `assessmentName`: `str`

Optional fields:

- `clientToken`: `str`
- `tags`: `Mapping`\[`str`, `str`\]

<a id="startappassessmentresponsetypedef"></a>

## StartAppAssessmentResponseTypeDef

```python
from types_aiobotocore_resiliencehub.type_defs import StartAppAssessmentResponseTypeDef
```

Required fields:

- `assessment`: [AppAssessmentTypeDef](./type_defs.md#appassessmenttypedef)
- `ResponseMetadata`:
  [ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef)

<a id="tagresourcerequestrequesttypedef"></a>

## TagResourceRequestRequestTypeDef

```python
from types_aiobotocore_resiliencehub.type_defs import TagResourceRequestRequestTypeDef
```

Required fields:

- `resourceArn`: `str`
- `tags`: `Mapping`\[`str`, `str`\]

<a id="testrecommendationtypedef"></a>

## TestRecommendationTypeDef

```python
from types_aiobotocore_resiliencehub.type_defs import TestRecommendationTypeDef
```

Required fields:

- `referenceId`: `str`

Optional fields:

- `appComponentName`: `str`
- `description`: `str`
- `intent`: `str`
- `items`:
  `List`\[[RecommendationItemTypeDef](./type_defs.md#recommendationitemtypedef)\]
- `name`: `str`
- `prerequisite`: `str`
- `recommendationId`: `str`
- `risk`: [TestRiskType](./literals.md#testrisktype)
- `type`: [TestTypeType](./literals.md#testtypetype)

<a id="unsupportedresourcetypedef"></a>

## UnsupportedResourceTypeDef

```python
from types_aiobotocore_resiliencehub.type_defs import UnsupportedResourceTypeDef
```

Required fields:

- `logicalResourceId`:
  [LogicalResourceIdTypeDef](./type_defs.md#logicalresourceidtypedef)
- `physicalResourceId`:
  [PhysicalResourceIdTypeDef](./type_defs.md#physicalresourceidtypedef)
- `resourceType`: `str`

<a id="untagresourcerequestrequesttypedef"></a>

## UntagResourceRequestRequestTypeDef

```python
from types_aiobotocore_resiliencehub.type_defs import UntagResourceRequestRequestTypeDef
```

Required fields:

- `resourceArn`: `str`
- `tagKeys`: `Sequence`\[`str`\]

<a id="updateapprequestrequesttypedef"></a>

## UpdateAppRequestRequestTypeDef

```python
from types_aiobotocore_resiliencehub.type_defs import UpdateAppRequestRequestTypeDef
```

Required fields:

- `appArn`: `str`

Optional fields:

- `clearResiliencyPolicyArn`: `bool`
- `description`: `str`
- `policyArn`: `str`

<a id="updateappresponsetypedef"></a>

## UpdateAppResponseTypeDef

```python
from types_aiobotocore_resiliencehub.type_defs import UpdateAppResponseTypeDef
```

Required fields:

- `app`: [AppTypeDef](./type_defs.md#apptypedef)
- `ResponseMetadata`:
  [ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef)

<a id="updateresiliencypolicyrequestrequesttypedef"></a>

## UpdateResiliencyPolicyRequestRequestTypeDef

```python
from types_aiobotocore_resiliencehub.type_defs import UpdateResiliencyPolicyRequestRequestTypeDef
```

Required fields:

- `policyArn`: `str`

Optional fields:

- `dataLocationConstraint`:
  [DataLocationConstraintType](./literals.md#datalocationconstrainttype)
- `policy`: `Mapping`\[[DisruptionTypeType](./literals.md#disruptiontypetype),
  [FailurePolicyTypeDef](./type_defs.md#failurepolicytypedef)\]
- `policyDescription`: `str`
- `policyName`: `str`
- `tier`: [ResiliencyPolicyTierType](./literals.md#resiliencypolicytiertype)

<a id="updateresiliencypolicyresponsetypedef"></a>

## UpdateResiliencyPolicyResponseTypeDef

```python
from types_aiobotocore_resiliencehub.type_defs import UpdateResiliencyPolicyResponseTypeDef
```

Required fields:

- `policy`: [ResiliencyPolicyTypeDef](./type_defs.md#resiliencypolicytypedef)
- `ResponseMetadata`:
  [ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef)
