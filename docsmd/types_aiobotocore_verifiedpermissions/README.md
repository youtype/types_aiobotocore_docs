# VerifiedPermissions module

> [Index](../README.md) > VerifiedPermissions


!!! note ""

    Auto-generated documentation for [VerifiedPermissions](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/verifiedpermissions.html#VerifiedPermissions)
    type annotations stubs module [types-aiobotocore-verifiedpermissions](https://pypi.org/project/types-aiobotocore-verifiedpermissions/).

## How to install



### From PyPI with pip

Install `types-aiobotocore` for `VerifiedPermissions` service.

```bash
# install with aiobotocore type annotations
python -m pip install 'types-aiobotocore[verifiedpermissions]'


# Lite version does not provide session.client/resource overloads
# it is more RAM-friendly, but requires explicit type annotations
python -m pip install 'types-aiobotocore-lite[verifiedpermissions]'


# standalone installation
python -m pip install types-aiobotocore-verifiedpermissions
```



## How to uninstall

```bash
python -m pip uninstall -y types-aiobotocore-verifiedpermissions
```

## Usage

Code samples can be found in [Examples](./usage.md).

## VerifiedPermissionsClient

Type annotations and code completion for  `#!python session.create_client("verifiedpermissions")` as [VerifiedPermissionsClient](./client.md)
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/verifiedpermissions.html#VerifiedPermissions.Client)

```python
# VerifiedPermissionsClient usage example

from aiobotocore.session import get_session

from types_aiobotocore_verifiedpermissions.client import VerifiedPermissionsClient


session = get_session()
async with session.create_client("verifiedpermissions") as client:
    client: VerifiedPermissionsClient
```


## Paginators

Type annotations and code completion for
[paginators](./paginators.md)
from `#!python session.create_client("verifiedpermissions").get_paginator("...")`.

```python
# ListIdentitySourcesPaginator usage example

from types_aiobotocore_verifiedpermissions.paginator import ListIdentitySourcesPaginator

def get_list_identity_sources_paginator() -> ListIdentitySourcesPaginator:
    return client.get_paginator("list_identity_sources"))
```

- [ListIdentitySourcesPaginator](./paginators.md#listidentitysourcespaginator)
- [ListPoliciesPaginator](./paginators.md#listpoliciespaginator)
- [ListPolicyStoresPaginator](./paginators.md#listpolicystorespaginator)
- [ListPolicyTemplatesPaginator](./paginators.md#listpolicytemplatespaginator)








## Literals

Type annotations for [literals](./literals.md) used in methods and schema.

```python
# DecisionType usage example

from types_aiobotocore_verifiedpermissions.literals import DecisionType

def get_value() -> DecisionType:
    return "ALLOW"
```

- [DecisionType](./literals.md#decisiontype)
- [ListIdentitySourcesPaginatorName](./literals.md#listidentitysourcespaginatorname)
- [ListPoliciesPaginatorName](./literals.md#listpoliciespaginatorname)
- [ListPolicyStoresPaginatorName](./literals.md#listpolicystorespaginatorname)
- [ListPolicyTemplatesPaginatorName](./literals.md#listpolicytemplatespaginatorname)
- [OpenIdIssuerType](./literals.md#openidissuertype)
- [PolicyTypeType](./literals.md#policytypetype)
- [ValidationModeType](./literals.md#validationmodetype)
- [VerifiedPermissionsServiceName](./literals.md#verifiedpermissionsservicename)
- [ServiceName](./literals.md#servicename)
- [ResourceServiceName](./literals.md#resourceservicename)
- [PaginatorName](./literals.md#paginatorname)
- [RegionName](./literals.md#regionname)




## Type definitions

Type annotations for [type definitions](./type_defs.md) used in methods and schema.

- [ActionIdentifierTypeDef](./type_defs.md#actionidentifiertypedef)
- [EntityIdentifierTypeDef](./type_defs.md#entityidentifiertypedef)
- [CognitoUserPoolConfigurationTypeDef](./type_defs.md#cognitouserpoolconfigurationtypedef)
- [ContextDefinitionTypeDef](./type_defs.md#contextdefinitiontypedef)
- [ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef)
- [ValidationSettingsTypeDef](./type_defs.md#validationsettingstypedef)
- [CreatePolicyTemplateInputRequestTypeDef](./type_defs.md#createpolicytemplateinputrequesttypedef)
- [DeleteIdentitySourceInputRequestTypeDef](./type_defs.md#deleteidentitysourceinputrequesttypedef)
- [DeletePolicyInputRequestTypeDef](./type_defs.md#deletepolicyinputrequesttypedef)
- [DeletePolicyStoreInputRequestTypeDef](./type_defs.md#deletepolicystoreinputrequesttypedef)
- [DeletePolicyTemplateInputRequestTypeDef](./type_defs.md#deletepolicytemplateinputrequesttypedef)
- [DeterminingPolicyItemTypeDef](./type_defs.md#determiningpolicyitemtypedef)
- [EvaluationErrorItemTypeDef](./type_defs.md#evaluationerroritemtypedef)
- [GetIdentitySourceInputRequestTypeDef](./type_defs.md#getidentitysourceinputrequesttypedef)
- [IdentitySourceDetailsTypeDef](./type_defs.md#identitysourcedetailstypedef)
- [GetPolicyInputRequestTypeDef](./type_defs.md#getpolicyinputrequesttypedef)
- [GetPolicyStoreInputRequestTypeDef](./type_defs.md#getpolicystoreinputrequesttypedef)
- [GetPolicyTemplateInputRequestTypeDef](./type_defs.md#getpolicytemplateinputrequesttypedef)
- [GetSchemaInputRequestTypeDef](./type_defs.md#getschemainputrequesttypedef)
- [IdentitySourceFilterTypeDef](./type_defs.md#identitysourcefiltertypedef)
- [IdentitySourceItemDetailsTypeDef](./type_defs.md#identitysourceitemdetailstypedef)
- [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
- [ListPolicyStoresInputRequestTypeDef](./type_defs.md#listpolicystoresinputrequesttypedef)
- [PolicyStoreItemTypeDef](./type_defs.md#policystoreitemtypedef)
- [ListPolicyTemplatesInputRequestTypeDef](./type_defs.md#listpolicytemplatesinputrequesttypedef)
- [PolicyTemplateItemTypeDef](./type_defs.md#policytemplateitemtypedef)
- [StaticPolicyDefinitionDetailTypeDef](./type_defs.md#staticpolicydefinitiondetailtypedef)
- [StaticPolicyDefinitionItemTypeDef](./type_defs.md#staticpolicydefinitionitemtypedef)
- [StaticPolicyDefinitionTypeDef](./type_defs.md#staticpolicydefinitiontypedef)
- [SchemaDefinitionTypeDef](./type_defs.md#schemadefinitiontypedef)
- [UpdateCognitoUserPoolConfigurationTypeDef](./type_defs.md#updatecognitouserpoolconfigurationtypedef)
- [UpdateStaticPolicyDefinitionTypeDef](./type_defs.md#updatestaticpolicydefinitiontypedef)
- [UpdatePolicyTemplateInputRequestTypeDef](./type_defs.md#updatepolicytemplateinputrequesttypedef)
- [AttributeValueTypeDef](./type_defs.md#attributevaluetypedef)
- [EntityItemTypeDef](./type_defs.md#entityitemtypedef)
- [EntityReferenceTypeDef](./type_defs.md#entityreferencetypedef)
- [TemplateLinkedPolicyDefinitionDetailTypeDef](./type_defs.md#templatelinkedpolicydefinitiondetailtypedef)
- [TemplateLinkedPolicyDefinitionItemTypeDef](./type_defs.md#templatelinkedpolicydefinitionitemtypedef)
- [TemplateLinkedPolicyDefinitionTypeDef](./type_defs.md#templatelinkedpolicydefinitiontypedef)
- [ConfigurationTypeDef](./type_defs.md#configurationtypedef)
- [CreateIdentitySourceOutputTypeDef](./type_defs.md#createidentitysourceoutputtypedef)
- [CreatePolicyOutputTypeDef](./type_defs.md#createpolicyoutputtypedef)
- [CreatePolicyStoreOutputTypeDef](./type_defs.md#createpolicystoreoutputtypedef)
- [CreatePolicyTemplateOutputTypeDef](./type_defs.md#createpolicytemplateoutputtypedef)
- [GetPolicyTemplateOutputTypeDef](./type_defs.md#getpolicytemplateoutputtypedef)
- [GetSchemaOutputTypeDef](./type_defs.md#getschemaoutputtypedef)
- [PutSchemaOutputTypeDef](./type_defs.md#putschemaoutputtypedef)
- [UpdateIdentitySourceOutputTypeDef](./type_defs.md#updateidentitysourceoutputtypedef)
- [UpdatePolicyOutputTypeDef](./type_defs.md#updatepolicyoutputtypedef)
- [UpdatePolicyStoreOutputTypeDef](./type_defs.md#updatepolicystoreoutputtypedef)
- [UpdatePolicyTemplateOutputTypeDef](./type_defs.md#updatepolicytemplateoutputtypedef)
- [CreatePolicyStoreInputRequestTypeDef](./type_defs.md#createpolicystoreinputrequesttypedef)
- [GetPolicyStoreOutputTypeDef](./type_defs.md#getpolicystoreoutputtypedef)
- [UpdatePolicyStoreInputRequestTypeDef](./type_defs.md#updatepolicystoreinputrequesttypedef)
- [IsAuthorizedOutputTypeDef](./type_defs.md#isauthorizedoutputtypedef)
- [IsAuthorizedWithTokenOutputTypeDef](./type_defs.md#isauthorizedwithtokenoutputtypedef)
- [GetIdentitySourceOutputTypeDef](./type_defs.md#getidentitysourceoutputtypedef)
- [ListIdentitySourcesInputRequestTypeDef](./type_defs.md#listidentitysourcesinputrequesttypedef)
- [IdentitySourceItemTypeDef](./type_defs.md#identitysourceitemtypedef)
- [ListIdentitySourcesInputListIdentitySourcesPaginateTypeDef](./type_defs.md#listidentitysourcesinputlistidentitysourcespaginatetypedef)
- [ListPolicyStoresInputListPolicyStoresPaginateTypeDef](./type_defs.md#listpolicystoresinputlistpolicystorespaginatetypedef)
- [ListPolicyTemplatesInputListPolicyTemplatesPaginateTypeDef](./type_defs.md#listpolicytemplatesinputlistpolicytemplatespaginatetypedef)
- [ListPolicyStoresOutputTypeDef](./type_defs.md#listpolicystoresoutputtypedef)
- [ListPolicyTemplatesOutputTypeDef](./type_defs.md#listpolicytemplatesoutputtypedef)
- [PutSchemaInputRequestTypeDef](./type_defs.md#putschemainputrequesttypedef)
- [UpdateConfigurationTypeDef](./type_defs.md#updateconfigurationtypedef)
- [UpdatePolicyDefinitionTypeDef](./type_defs.md#updatepolicydefinitiontypedef)
- [EntitiesDefinitionTypeDef](./type_defs.md#entitiesdefinitiontypedef)
- [PolicyFilterTypeDef](./type_defs.md#policyfiltertypedef)
- [PolicyDefinitionDetailTypeDef](./type_defs.md#policydefinitiondetailtypedef)
- [PolicyDefinitionItemTypeDef](./type_defs.md#policydefinitionitemtypedef)
- [PolicyDefinitionTypeDef](./type_defs.md#policydefinitiontypedef)
- [CreateIdentitySourceInputRequestTypeDef](./type_defs.md#createidentitysourceinputrequesttypedef)
- [ListIdentitySourcesOutputTypeDef](./type_defs.md#listidentitysourcesoutputtypedef)
- [UpdateIdentitySourceInputRequestTypeDef](./type_defs.md#updateidentitysourceinputrequesttypedef)
- [UpdatePolicyInputRequestTypeDef](./type_defs.md#updatepolicyinputrequesttypedef)
- [IsAuthorizedInputRequestTypeDef](./type_defs.md#isauthorizedinputrequesttypedef)
- [IsAuthorizedWithTokenInputRequestTypeDef](./type_defs.md#isauthorizedwithtokeninputrequesttypedef)
- [ListPoliciesInputListPoliciesPaginateTypeDef](./type_defs.md#listpoliciesinputlistpoliciespaginatetypedef)
- [ListPoliciesInputRequestTypeDef](./type_defs.md#listpoliciesinputrequesttypedef)
- [GetPolicyOutputTypeDef](./type_defs.md#getpolicyoutputtypedef)
- [PolicyItemTypeDef](./type_defs.md#policyitemtypedef)
- [CreatePolicyInputRequestTypeDef](./type_defs.md#createpolicyinputrequesttypedef)
- [ListPoliciesOutputTypeDef](./type_defs.md#listpoliciesoutputtypedef)

