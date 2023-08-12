# AmplifyUIBuilder module

> [Index](../README.md) > AmplifyUIBuilder


!!! note ""

    Auto-generated documentation for [AmplifyUIBuilder](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/amplifyuibuilder.html#AmplifyUIBuilder)
    type annotations stubs module [types-aiobotocore-amplifyuibuilder](https://pypi.org/project/types-aiobotocore-amplifyuibuilder/).

## How to install



### From PyPI with pip

Install `types-aiobotocore` for `AmplifyUIBuilder` service.

```bash
# install with aiobotocore type annotations
python -m pip install 'types-aiobotocore[amplifyuibuilder]'


# Lite version does not provide session.client/resource overloads
# it is more RAM-friendly, but requires explicit type annotations
python -m pip install 'types-aiobotocore-lite[amplifyuibuilder]'


# standalone installation
python -m pip install types-aiobotocore-amplifyuibuilder
```



## How to uninstall

```bash
python -m pip uninstall -y types-aiobotocore-amplifyuibuilder
```

## Usage

Code samples can be found in [Examples](./usage.md).

## AmplifyUIBuilderClient

Type annotations and code completion for  `#!python session.create_client("amplifyuibuilder")` as [AmplifyUIBuilderClient](./client.md)
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/amplifyuibuilder.html#AmplifyUIBuilder.Client)

```python
# AmplifyUIBuilderClient usage example

from aiobotocore.session import get_session

from types_aiobotocore_amplifyuibuilder.client import AmplifyUIBuilderClient


session = get_session()
async with session.create_client("amplifyuibuilder") as client:
    client: AmplifyUIBuilderClient
```


## Paginators

Type annotations and code completion for
[paginators](./paginators.md)
from `#!python session.create_client("amplifyuibuilder").get_paginator("...")`.

```python
# ExportComponentsPaginator usage example

from types_aiobotocore_amplifyuibuilder.paginator import ExportComponentsPaginator

def get_export_components_paginator() -> ExportComponentsPaginator:
    return client.get_paginator("export_components"))
```

- [ExportComponentsPaginator](./paginators.md#exportcomponentspaginator)
- [ExportFormsPaginator](./paginators.md#exportformspaginator)
- [ExportThemesPaginator](./paginators.md#exportthemespaginator)
- [ListCodegenJobsPaginator](./paginators.md#listcodegenjobspaginator)
- [ListComponentsPaginator](./paginators.md#listcomponentspaginator)
- [ListFormsPaginator](./paginators.md#listformspaginator)
- [ListThemesPaginator](./paginators.md#listthemespaginator)








## Literals

Type annotations for [literals](./literals.md) used in methods and schema.

```python
# CodegenGenericDataFieldDataTypeType usage example

from types_aiobotocore_amplifyuibuilder.literals import CodegenGenericDataFieldDataTypeType

def get_value() -> CodegenGenericDataFieldDataTypeType:
    return "AWSDate"
```

- [CodegenGenericDataFieldDataTypeType](./literals.md#codegengenericdatafielddatatypetype)
- [CodegenJobGenericDataSourceTypeType](./literals.md#codegenjobgenericdatasourcetypetype)
- [CodegenJobStatusType](./literals.md#codegenjobstatustype)
- [ExportComponentsPaginatorName](./literals.md#exportcomponentspaginatorname)
- [ExportFormsPaginatorName](./literals.md#exportformspaginatorname)
- [ExportThemesPaginatorName](./literals.md#exportthemespaginatorname)
- [FixedPositionType](./literals.md#fixedpositiontype)
- [FormActionTypeType](./literals.md#formactiontypetype)
- [FormButtonsPositionType](./literals.md#formbuttonspositiontype)
- [FormDataSourceTypeType](./literals.md#formdatasourcetypetype)
- [GenericDataRelationshipTypeType](./literals.md#genericdatarelationshiptypetype)
- [JSModuleType](./literals.md#jsmoduletype)
- [JSScriptType](./literals.md#jsscripttype)
- [JSTargetType](./literals.md#jstargettype)
- [LabelDecoratorType](./literals.md#labeldecoratortype)
- [ListCodegenJobsPaginatorName](./literals.md#listcodegenjobspaginatorname)
- [ListComponentsPaginatorName](./literals.md#listcomponentspaginatorname)
- [ListFormsPaginatorName](./literals.md#listformspaginatorname)
- [ListThemesPaginatorName](./literals.md#listthemespaginatorname)
- [SortDirectionType](./literals.md#sortdirectiontype)
- [StorageAccessLevelType](./literals.md#storageaccessleveltype)
- [TokenProvidersType](./literals.md#tokenproviderstype)
- [AmplifyUIBuilderServiceName](./literals.md#amplifyuibuilderservicename)
- [ServiceName](./literals.md#servicename)
- [ResourceServiceName](./literals.md#resourceservicename)
- [PaginatorName](./literals.md#paginatorname)
- [RegionName](./literals.md#regionname)




## Type definitions

Type annotations for [type definitions](./type_defs.md) used in methods and schema.

- [MutationActionSetStateParameterTypeDef](./type_defs.md#mutationactionsetstateparametertypedef)
- [GraphQLRenderConfigTypeDef](./type_defs.md#graphqlrenderconfigtypedef)
- [CodegenFeatureFlagsTypeDef](./type_defs.md#codegenfeatureflagstypedef)
- [CodegenGenericDataEnumTypeDef](./type_defs.md#codegengenericdataenumtypedef)
- [CodegenGenericDataRelationshipTypeTypeDef](./type_defs.md#codegengenericdatarelationshiptypetypedef)
- [CodegenJobAssetTypeDef](./type_defs.md#codegenjobassettypedef)
- [CodegenJobSummaryTypeDef](./type_defs.md#codegenjobsummarytypedef)
- [ComponentBindingPropertiesValuePropertiesTypeDef](./type_defs.md#componentbindingpropertiesvaluepropertiestypedef)
- [ComponentConditionPropertyTypeDef](./type_defs.md#componentconditionpropertytypedef)
- [SortPropertyTypeDef](./type_defs.md#sortpropertytypedef)
- [ComponentPropertyBindingPropertiesTypeDef](./type_defs.md#componentpropertybindingpropertiestypedef)
- [FormBindingElementTypeDef](./type_defs.md#formbindingelementtypedef)
- [ComponentSummaryTypeDef](./type_defs.md#componentsummarytypedef)
- [ComponentVariantTypeDef](./type_defs.md#componentvarianttypedef)
- [ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef)
- [FormDataTypeConfigTypeDef](./type_defs.md#formdatatypeconfigtypedef)
- [CreateThemeDataTypeDef](./type_defs.md#createthemedatatypedef)
- [ThemeTypeDef](./type_defs.md#themetypedef)
- [DeleteComponentRequestRequestTypeDef](./type_defs.md#deletecomponentrequestrequesttypedef)
- [DeleteFormRequestRequestTypeDef](./type_defs.md#deleteformrequestrequesttypedef)
- [DeleteThemeRequestRequestTypeDef](./type_defs.md#deletethemerequestrequesttypedef)
- [ExchangeCodeForTokenRequestBodyTypeDef](./type_defs.md#exchangecodefortokenrequestbodytypedef)
- [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
- [ExportComponentsRequestRequestTypeDef](./type_defs.md#exportcomponentsrequestrequesttypedef)
- [ExportFormsRequestRequestTypeDef](./type_defs.md#exportformsrequestrequesttypedef)
- [ExportThemesRequestRequestTypeDef](./type_defs.md#exportthemesrequestrequesttypedef)
- [FieldPositionTypeDef](./type_defs.md#fieldpositiontypedef)
- [FieldValidationConfigurationTypeDef](./type_defs.md#fieldvalidationconfigurationtypedef)
- [FileUploaderFieldConfigTypeDef](./type_defs.md#fileuploaderfieldconfigtypedef)
- [FormInputBindingPropertiesValuePropertiesTypeDef](./type_defs.md#forminputbindingpropertiesvaluepropertiestypedef)
- [FormInputValuePropertyBindingPropertiesTypeDef](./type_defs.md#forminputvaluepropertybindingpropertiestypedef)
- [FormStyleConfigTypeDef](./type_defs.md#formstyleconfigtypedef)
- [GetCodegenJobRequestRequestTypeDef](./type_defs.md#getcodegenjobrequestrequesttypedef)
- [GetComponentRequestRequestTypeDef](./type_defs.md#getcomponentrequestrequesttypedef)
- [GetFormRequestRequestTypeDef](./type_defs.md#getformrequestrequesttypedef)
- [GetMetadataRequestRequestTypeDef](./type_defs.md#getmetadatarequestrequesttypedef)
- [GetThemeRequestRequestTypeDef](./type_defs.md#getthemerequestrequesttypedef)
- [ListCodegenJobsRequestRequestTypeDef](./type_defs.md#listcodegenjobsrequestrequesttypedef)
- [ListComponentsRequestRequestTypeDef](./type_defs.md#listcomponentsrequestrequesttypedef)
- [ListFormsRequestRequestTypeDef](./type_defs.md#listformsrequestrequesttypedef)
- [ListThemesRequestRequestTypeDef](./type_defs.md#listthemesrequestrequesttypedef)
- [ThemeSummaryTypeDef](./type_defs.md#themesummarytypedef)
- [PredicateTypeDef](./type_defs.md#predicatetypedef)
- [PutMetadataFlagBodyTypeDef](./type_defs.md#putmetadataflagbodytypedef)
- [RefreshTokenRequestBodyTypeDef](./type_defs.md#refreshtokenrequestbodytypedef)
- [ThemeValueTypeDef](./type_defs.md#themevaluetypedef)
- [ThemeValuesTypeDef](./type_defs.md#themevaluestypedef)
- [UpdateThemeDataTypeDef](./type_defs.md#updatethemedatatypedef)
- [ValueMappingTypeDef](./type_defs.md#valuemappingtypedef)
- [ActionParametersTypeDef](./type_defs.md#actionparameterstypedef)
- [ApiConfigurationTypeDef](./type_defs.md#apiconfigurationtypedef)
- [CodegenGenericDataFieldTypeDef](./type_defs.md#codegengenericdatafieldtypedef)
- [ComponentBindingPropertiesValueTypeDef](./type_defs.md#componentbindingpropertiesvaluetypedef)
- [ComponentDataConfigurationTypeDef](./type_defs.md#componentdataconfigurationtypedef)
- [ComponentPropertyTypeDef](./type_defs.md#componentpropertytypedef)
- [EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef)
- [ExchangeCodeForTokenResponseTypeDef](./type_defs.md#exchangecodefortokenresponsetypedef)
- [GetMetadataResponseTypeDef](./type_defs.md#getmetadataresponsetypedef)
- [ListCodegenJobsResponseTypeDef](./type_defs.md#listcodegenjobsresponsetypedef)
- [ListComponentsResponseTypeDef](./type_defs.md#listcomponentsresponsetypedef)
- [RefreshTokenResponseTypeDef](./type_defs.md#refreshtokenresponsetypedef)
- [FormSummaryTypeDef](./type_defs.md#formsummarytypedef)
- [CreateThemeRequestRequestTypeDef](./type_defs.md#createthemerequestrequesttypedef)
- [CreateThemeResponseTypeDef](./type_defs.md#createthemeresponsetypedef)
- [ExportThemesResponseTypeDef](./type_defs.md#exportthemesresponsetypedef)
- [GetThemeResponseTypeDef](./type_defs.md#getthemeresponsetypedef)
- [UpdateThemeResponseTypeDef](./type_defs.md#updatethemeresponsetypedef)
- [ExchangeCodeForTokenRequestRequestTypeDef](./type_defs.md#exchangecodefortokenrequestrequesttypedef)
- [ExportComponentsRequestExportComponentsPaginateTypeDef](./type_defs.md#exportcomponentsrequestexportcomponentspaginatetypedef)
- [ExportFormsRequestExportFormsPaginateTypeDef](./type_defs.md#exportformsrequestexportformspaginatetypedef)
- [ExportThemesRequestExportThemesPaginateTypeDef](./type_defs.md#exportthemesrequestexportthemespaginatetypedef)
- [ListCodegenJobsRequestListCodegenJobsPaginateTypeDef](./type_defs.md#listcodegenjobsrequestlistcodegenjobspaginatetypedef)
- [ListComponentsRequestListComponentsPaginateTypeDef](./type_defs.md#listcomponentsrequestlistcomponentspaginatetypedef)
- [ListFormsRequestListFormsPaginateTypeDef](./type_defs.md#listformsrequestlistformspaginatetypedef)
- [ListThemesRequestListThemesPaginateTypeDef](./type_defs.md#listthemesrequestlistthemespaginatetypedef)
- [FormButtonTypeDef](./type_defs.md#formbuttontypedef)
- [SectionalElementTypeDef](./type_defs.md#sectionalelementtypedef)
- [FormInputBindingPropertiesValueTypeDef](./type_defs.md#forminputbindingpropertiesvaluetypedef)
- [FormInputValuePropertyTypeDef](./type_defs.md#forminputvaluepropertytypedef)
- [FormStyleTypeDef](./type_defs.md#formstyletypedef)
- [ListThemesResponseTypeDef](./type_defs.md#listthemesresponsetypedef)
- [PutMetadataFlagRequestRequestTypeDef](./type_defs.md#putmetadataflagrequestrequesttypedef)
- [RefreshTokenRequestRequestTypeDef](./type_defs.md#refreshtokenrequestrequesttypedef)
- [UpdateThemeRequestRequestTypeDef](./type_defs.md#updatethemerequestrequesttypedef)
- [ComponentEventTypeDef](./type_defs.md#componenteventtypedef)
- [ReactStartCodegenJobDataTypeDef](./type_defs.md#reactstartcodegenjobdatatypedef)
- [CodegenGenericDataModelTypeDef](./type_defs.md#codegengenericdatamodeltypedef)
- [CodegenGenericDataNonModelTypeDef](./type_defs.md#codegengenericdatanonmodeltypedef)
- [ListFormsResponseTypeDef](./type_defs.md#listformsresponsetypedef)
- [FormCTATypeDef](./type_defs.md#formctatypedef)
- [ValueMappingsTypeDef](./type_defs.md#valuemappingstypedef)
- [ComponentChildTypeDef](./type_defs.md#componentchildtypedef)
- [ComponentTypeDef](./type_defs.md#componenttypedef)
- [CreateComponentDataTypeDef](./type_defs.md#createcomponentdatatypedef)
- [UpdateComponentDataTypeDef](./type_defs.md#updatecomponentdatatypedef)
- [CodegenJobRenderConfigTypeDef](./type_defs.md#codegenjobrenderconfigtypedef)
- [CodegenJobGenericDataSchemaTypeDef](./type_defs.md#codegenjobgenericdataschematypedef)
- [FieldInputConfigTypeDef](./type_defs.md#fieldinputconfigtypedef)
- [CreateComponentResponseTypeDef](./type_defs.md#createcomponentresponsetypedef)
- [ExportComponentsResponseTypeDef](./type_defs.md#exportcomponentsresponsetypedef)
- [GetComponentResponseTypeDef](./type_defs.md#getcomponentresponsetypedef)
- [UpdateComponentResponseTypeDef](./type_defs.md#updatecomponentresponsetypedef)
- [CreateComponentRequestRequestTypeDef](./type_defs.md#createcomponentrequestrequesttypedef)
- [UpdateComponentRequestRequestTypeDef](./type_defs.md#updatecomponentrequestrequesttypedef)
- [CodegenJobTypeDef](./type_defs.md#codegenjobtypedef)
- [StartCodegenJobDataTypeDef](./type_defs.md#startcodegenjobdatatypedef)
- [FieldConfigTypeDef](./type_defs.md#fieldconfigtypedef)
- [GetCodegenJobResponseTypeDef](./type_defs.md#getcodegenjobresponsetypedef)
- [StartCodegenJobResponseTypeDef](./type_defs.md#startcodegenjobresponsetypedef)
- [StartCodegenJobRequestRequestTypeDef](./type_defs.md#startcodegenjobrequestrequesttypedef)
- [CreateFormDataTypeDef](./type_defs.md#createformdatatypedef)
- [FormTypeDef](./type_defs.md#formtypedef)
- [UpdateFormDataTypeDef](./type_defs.md#updateformdatatypedef)
- [CreateFormRequestRequestTypeDef](./type_defs.md#createformrequestrequesttypedef)
- [CreateFormResponseTypeDef](./type_defs.md#createformresponsetypedef)
- [ExportFormsResponseTypeDef](./type_defs.md#exportformsresponsetypedef)
- [GetFormResponseTypeDef](./type_defs.md#getformresponsetypedef)
- [UpdateFormResponseTypeDef](./type_defs.md#updateformresponsetypedef)
- [UpdateFormRequestRequestTypeDef](./type_defs.md#updateformrequestrequesttypedef)

