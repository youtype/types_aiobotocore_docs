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

```python title="Usage example"
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

```python title="Usage example"
from types_aiobotocore_amplifyuibuilder.paginator import ExportComponentsPaginator

def get_export_components_paginator() -> ExportComponentsPaginator:
    return client.get_paginator("export_components"))
```

- [ExportComponentsPaginator](./paginators.md#exportcomponentspaginator)
- [ExportThemesPaginator](./paginators.md#exportthemespaginator)
- [ListComponentsPaginator](./paginators.md#listcomponentspaginator)
- [ListThemesPaginator](./paginators.md#listthemespaginator)








## Literals

Type annotations for [literals](./literals.md) used in methods and schema.

```python title="Usage example"
from types_aiobotocore_amplifyuibuilder.literals import ExportComponentsPaginatorName

def get_value() -> ExportComponentsPaginatorName:
    return "export_components"
```

- [ExportComponentsPaginatorName](./literals.md#exportcomponentspaginatorname)
- [ExportThemesPaginatorName](./literals.md#exportthemespaginatorname)
- [ListComponentsPaginatorName](./literals.md#listcomponentspaginatorname)
- [ListThemesPaginatorName](./literals.md#listthemespaginatorname)
- [SortDirectionType](./literals.md#sortdirectiontype)
- [TokenProvidersType](./literals.md#tokenproviderstype)
- [AmplifyUIBuilderServiceName](./literals.md#amplifyuibuilderservicename)
- [ServiceName](./literals.md#servicename)
- [ResourceServiceName](./literals.md#resourceservicename)
- [PaginatorName](./literals.md#paginatorname)
- [RegionName](./literals.md#regionname)




## Typed dictionaries

Type annotations for [typed dictionaries](./type_defs.md) used in methods and schema.

```python title="Usage example"
from types_aiobotocore_amplifyuibuilder.type_defs import MutationActionSetStateParameterTypeDef

def get_value() -> MutationActionSetStateParameterTypeDef:
    return {
        "componentName": ...,
        "property": ...,
        "set": ...,
    }
```

- [MutationActionSetStateParameterTypeDef](./type_defs.md#mutationactionsetstateparametertypedef)
- [ComponentBindingPropertiesValuePropertiesTypeDef](./type_defs.md#componentbindingpropertiesvaluepropertiestypedef)
- [ComponentConditionPropertyTypeDef](./type_defs.md#componentconditionpropertytypedef)
- [SortPropertyTypeDef](./type_defs.md#sortpropertytypedef)
- [ComponentPropertyBindingPropertiesTypeDef](./type_defs.md#componentpropertybindingpropertiestypedef)
- [FormBindingElementTypeDef](./type_defs.md#formbindingelementtypedef)
- [ComponentSummaryTypeDef](./type_defs.md#componentsummarytypedef)
- [ComponentVariantTypeDef](./type_defs.md#componentvarianttypedef)
- [ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef)
- [CreateThemeDataTypeDef](./type_defs.md#createthemedatatypedef)
- [ThemeTypeDef](./type_defs.md#themetypedef)
- [DeleteComponentRequestRequestTypeDef](./type_defs.md#deletecomponentrequestrequesttypedef)
- [DeleteThemeRequestRequestTypeDef](./type_defs.md#deletethemerequestrequesttypedef)
- [ExchangeCodeForTokenRequestBodyTypeDef](./type_defs.md#exchangecodefortokenrequestbodytypedef)
- [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
- [ExportComponentsRequestRequestTypeDef](./type_defs.md#exportcomponentsrequestrequesttypedef)
- [ExportThemesRequestRequestTypeDef](./type_defs.md#exportthemesrequestrequesttypedef)
- [GetComponentRequestRequestTypeDef](./type_defs.md#getcomponentrequestrequesttypedef)
- [GetThemeRequestRequestTypeDef](./type_defs.md#getthemerequestrequesttypedef)
- [ListComponentsRequestRequestTypeDef](./type_defs.md#listcomponentsrequestrequesttypedef)
- [ListThemesRequestRequestTypeDef](./type_defs.md#listthemesrequestrequesttypedef)
- [ThemeSummaryTypeDef](./type_defs.md#themesummarytypedef)
- [PredicateTypeDef](./type_defs.md#predicatetypedef)
- [RefreshTokenRequestBodyTypeDef](./type_defs.md#refreshtokenrequestbodytypedef)
- [ThemeValueTypeDef](./type_defs.md#themevaluetypedef)
- [ThemeValuesTypeDef](./type_defs.md#themevaluestypedef)
- [UpdateThemeDataTypeDef](./type_defs.md#updatethemedatatypedef)
- [ActionParametersTypeDef](./type_defs.md#actionparameterstypedef)
- [ComponentBindingPropertiesValueTypeDef](./type_defs.md#componentbindingpropertiesvaluetypedef)
- [ComponentDataConfigurationTypeDef](./type_defs.md#componentdataconfigurationtypedef)
- [ComponentPropertyTypeDef](./type_defs.md#componentpropertytypedef)
- [EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef)
- [ExchangeCodeForTokenResponseTypeDef](./type_defs.md#exchangecodefortokenresponsetypedef)
- [ListComponentsResponseTypeDef](./type_defs.md#listcomponentsresponsetypedef)
- [RefreshTokenResponseTypeDef](./type_defs.md#refreshtokenresponsetypedef)
- [CreateThemeRequestRequestTypeDef](./type_defs.md#createthemerequestrequesttypedef)
- [CreateThemeResponseTypeDef](./type_defs.md#createthemeresponsetypedef)
- [ExportThemesResponseTypeDef](./type_defs.md#exportthemesresponsetypedef)
- [GetThemeResponseTypeDef](./type_defs.md#getthemeresponsetypedef)
- [UpdateThemeResponseTypeDef](./type_defs.md#updatethemeresponsetypedef)
- [ExchangeCodeForTokenRequestRequestTypeDef](./type_defs.md#exchangecodefortokenrequestrequesttypedef)
- [ExportComponentsRequestExportComponentsPaginateTypeDef](./type_defs.md#exportcomponentsrequestexportcomponentspaginatetypedef)
- [ExportThemesRequestExportThemesPaginateTypeDef](./type_defs.md#exportthemesrequestexportthemespaginatetypedef)
- [ListComponentsRequestListComponentsPaginateTypeDef](./type_defs.md#listcomponentsrequestlistcomponentspaginatetypedef)
- [ListThemesRequestListThemesPaginateTypeDef](./type_defs.md#listthemesrequestlistthemespaginatetypedef)
- [ListThemesResponseTypeDef](./type_defs.md#listthemesresponsetypedef)
- [RefreshTokenRequestRequestTypeDef](./type_defs.md#refreshtokenrequestrequesttypedef)
- [UpdateThemeRequestRequestTypeDef](./type_defs.md#updatethemerequestrequesttypedef)
- [ComponentEventTypeDef](./type_defs.md#componenteventtypedef)
- [ComponentChildTypeDef](./type_defs.md#componentchildtypedef)
- [ComponentTypeDef](./type_defs.md#componenttypedef)
- [CreateComponentDataTypeDef](./type_defs.md#createcomponentdatatypedef)
- [UpdateComponentDataTypeDef](./type_defs.md#updatecomponentdatatypedef)
- [CreateComponentResponseTypeDef](./type_defs.md#createcomponentresponsetypedef)
- [ExportComponentsResponseTypeDef](./type_defs.md#exportcomponentsresponsetypedef)
- [GetComponentResponseTypeDef](./type_defs.md#getcomponentresponsetypedef)
- [UpdateComponentResponseTypeDef](./type_defs.md#updatecomponentresponsetypedef)
- [CreateComponentRequestRequestTypeDef](./type_defs.md#createcomponentrequestrequesttypedef)
- [UpdateComponentRequestRequestTypeDef](./type_defs.md#updatecomponentrequestrequesttypedef)

