# OpenSearchServiceServerless module

> [Index](../README.md) > OpenSearchServiceServerless


!!! note ""

    Auto-generated documentation for [OpenSearchServiceServerless](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/opensearchserverless.html#opensearchserviceserverless)
    type annotations stubs module [types-aiobotocore-opensearchserverless](https://pypi.org/project/types-aiobotocore-opensearchserverless/).

## How to install

### Generate locally (recommended)

You can generate type annotations for `aiobotocore` package locally with `mypy_boto3_builder`.
Use [uv](https://docs.astral.sh/uv/getting-started/installation/) for build isolation.

1. Run mypy-boto3-builder in your package root directory: `uvx --with 'aiobotocore==2.19.0' mypy_boto3_builder`
1. Select `aiobotocore` AWS SDK.
1. Add `OpenSearchServiceServerless` service.
1. Use provided commands to install generated packages.



### From PyPI with pip

Install `types-aiobotocore` for `OpenSearchServiceServerless` service.

```bash
# install with aiobotocore type annotations
python -m pip install 'types-aiobotocore[opensearchserverless]'

# Lite version does not provide session.client/resource overloads
# it is more RAM-friendly, but requires explicit type annotations
python -m pip install 'types-aiobotocore-lite[opensearchserverless]'

# standalone installation
python -m pip install types-aiobotocore-opensearchserverless
```



## How to uninstall

```bash
python -m pip uninstall -y types-aiobotocore-opensearchserverless
```

## Usage

Code samples can be found in [Examples](./usage.md).

## OpenSearchServiceServerlessClient

Type annotations and code completion for  `#!python session.create_client("opensearchserverless")` as [OpenSearchServiceServerlessClient](./client.md)
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/opensearchserverless.html#OpenSearchServiceServerless.Client)

```python
# OpenSearchServiceServerlessClient usage example

from aiobotocore.session import get_session

from types_aiobotocore_opensearchserverless.client import OpenSearchServiceServerlessClient


session = get_session()
async with session.create_client("opensearchserverless") as client:
    client: OpenSearchServiceServerlessClient
```








## Literals

Type annotations for [literals](./literals.md) used in methods and schema.

```python
# AccessPolicyTypeType usage example

from types_aiobotocore_opensearchserverless.literals import AccessPolicyTypeType

def get_value() -> AccessPolicyTypeType:
    return "data"
```

- [AccessPolicyTypeType](./literals.md#accesspolicytypetype)
- [CollectionStatusType](./literals.md#collectionstatustype)
- [CollectionTypeType](./literals.md#collectiontypetype)
- [IamIdentityCenterGroupAttributeType](./literals.md#iamidentitycentergroupattributetype)
- [IamIdentityCenterUserAttributeType](./literals.md#iamidentitycenteruserattributetype)
- [LifecyclePolicyTypeType](./literals.md#lifecyclepolicytypetype)
- [ResourceTypeType](./literals.md#resourcetypetype)
- [SecurityConfigTypeType](./literals.md#securityconfigtypetype)
- [SecurityPolicyTypeType](./literals.md#securitypolicytypetype)
- [StandbyReplicasType](./literals.md#standbyreplicastype)
- [VpcEndpointStatusType](./literals.md#vpcendpointstatustype)
- [OpenSearchServiceServerlessServiceName](./literals.md#opensearchserviceserverlessservicename)
- [ServiceName](./literals.md#servicename)
- [ResourceServiceName](./literals.md#resourceservicename)
- [RegionName](./literals.md#regionname)




## Type definitions

Type annotations for [type definitions](./type_defs.md) used in methods and schema.

- [AccessPolicyDetailTypeDef](./type_defs.md#accesspolicydetailtypedef)
- [AccessPolicyStatsTypeDef](./type_defs.md#accesspolicystatstypedef)
- [AccessPolicySummaryTypeDef](./type_defs.md#accesspolicysummarytypedef)
- [CapacityLimitsTypeDef](./type_defs.md#capacitylimitstypedef)
- [BatchGetCollectionRequestRequestTypeDef](./type_defs.md#batchgetcollectionrequestrequesttypedef)
- [CollectionDetailTypeDef](./type_defs.md#collectiondetailtypedef)
- [CollectionErrorDetailTypeDef](./type_defs.md#collectionerrordetailtypedef)
- [ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef)
- [LifecyclePolicyResourceIdentifierTypeDef](./type_defs.md#lifecyclepolicyresourceidentifiertypedef)
- [EffectiveLifecyclePolicyDetailTypeDef](./type_defs.md#effectivelifecyclepolicydetailtypedef)
- [EffectiveLifecyclePolicyErrorDetailTypeDef](./type_defs.md#effectivelifecyclepolicyerrordetailtypedef)
- [LifecyclePolicyIdentifierTypeDef](./type_defs.md#lifecyclepolicyidentifiertypedef)
- [LifecyclePolicyDetailTypeDef](./type_defs.md#lifecyclepolicydetailtypedef)
- [LifecyclePolicyErrorDetailTypeDef](./type_defs.md#lifecyclepolicyerrordetailtypedef)
- [BatchGetVpcEndpointRequestRequestTypeDef](./type_defs.md#batchgetvpcendpointrequestrequesttypedef)
- [VpcEndpointDetailTypeDef](./type_defs.md#vpcendpointdetailtypedef)
- [VpcEndpointErrorDetailTypeDef](./type_defs.md#vpcendpointerrordetailtypedef)
- [CollectionFiltersTypeDef](./type_defs.md#collectionfilterstypedef)
- [CollectionSummaryTypeDef](./type_defs.md#collectionsummarytypedef)
- [CreateAccessPolicyRequestRequestTypeDef](./type_defs.md#createaccesspolicyrequestrequesttypedef)
- [CreateCollectionDetailTypeDef](./type_defs.md#createcollectiondetailtypedef)
- [TagTypeDef](./type_defs.md#tagtypedef)
- [CreateIamIdentityCenterConfigOptionsTypeDef](./type_defs.md#createiamidentitycenterconfigoptionstypedef)
- [CreateLifecyclePolicyRequestRequestTypeDef](./type_defs.md#createlifecyclepolicyrequestrequesttypedef)
- [SamlConfigOptionsTypeDef](./type_defs.md#samlconfigoptionstypedef)
- [CreateSecurityPolicyRequestRequestTypeDef](./type_defs.md#createsecuritypolicyrequestrequesttypedef)
- [SecurityPolicyDetailTypeDef](./type_defs.md#securitypolicydetailtypedef)
- [CreateVpcEndpointDetailTypeDef](./type_defs.md#createvpcendpointdetailtypedef)
- [CreateVpcEndpointRequestRequestTypeDef](./type_defs.md#createvpcendpointrequestrequesttypedef)
- [DeleteAccessPolicyRequestRequestTypeDef](./type_defs.md#deleteaccesspolicyrequestrequesttypedef)
- [DeleteCollectionDetailTypeDef](./type_defs.md#deletecollectiondetailtypedef)
- [DeleteCollectionRequestRequestTypeDef](./type_defs.md#deletecollectionrequestrequesttypedef)
- [DeleteLifecyclePolicyRequestRequestTypeDef](./type_defs.md#deletelifecyclepolicyrequestrequesttypedef)
- [DeleteSecurityConfigRequestRequestTypeDef](./type_defs.md#deletesecurityconfigrequestrequesttypedef)
- [DeleteSecurityPolicyRequestRequestTypeDef](./type_defs.md#deletesecuritypolicyrequestrequesttypedef)
- [DeleteVpcEndpointDetailTypeDef](./type_defs.md#deletevpcendpointdetailtypedef)
- [DeleteVpcEndpointRequestRequestTypeDef](./type_defs.md#deletevpcendpointrequestrequesttypedef)
- [GetAccessPolicyRequestRequestTypeDef](./type_defs.md#getaccesspolicyrequestrequesttypedef)
- [LifecyclePolicyStatsTypeDef](./type_defs.md#lifecyclepolicystatstypedef)
- [SecurityConfigStatsTypeDef](./type_defs.md#securityconfigstatstypedef)
- [SecurityPolicyStatsTypeDef](./type_defs.md#securitypolicystatstypedef)
- [GetSecurityConfigRequestRequestTypeDef](./type_defs.md#getsecurityconfigrequestrequesttypedef)
- [GetSecurityPolicyRequestRequestTypeDef](./type_defs.md#getsecuritypolicyrequestrequesttypedef)
- [IamIdentityCenterConfigOptionsTypeDef](./type_defs.md#iamidentitycenterconfigoptionstypedef)
- [LifecyclePolicySummaryTypeDef](./type_defs.md#lifecyclepolicysummarytypedef)
- [ListAccessPoliciesRequestRequestTypeDef](./type_defs.md#listaccesspoliciesrequestrequesttypedef)
- [ListLifecyclePoliciesRequestRequestTypeDef](./type_defs.md#listlifecyclepoliciesrequestrequesttypedef)
- [ListSecurityConfigsRequestRequestTypeDef](./type_defs.md#listsecurityconfigsrequestrequesttypedef)
- [SecurityConfigSummaryTypeDef](./type_defs.md#securityconfigsummarytypedef)
- [ListSecurityPoliciesRequestRequestTypeDef](./type_defs.md#listsecuritypoliciesrequestrequesttypedef)
- [SecurityPolicySummaryTypeDef](./type_defs.md#securitypolicysummarytypedef)
- [ListTagsForResourceRequestRequestTypeDef](./type_defs.md#listtagsforresourcerequestrequesttypedef)
- [VpcEndpointFiltersTypeDef](./type_defs.md#vpcendpointfilterstypedef)
- [VpcEndpointSummaryTypeDef](./type_defs.md#vpcendpointsummarytypedef)
- [UntagResourceRequestRequestTypeDef](./type_defs.md#untagresourcerequestrequesttypedef)
- [UpdateAccessPolicyRequestRequestTypeDef](./type_defs.md#updateaccesspolicyrequestrequesttypedef)
- [UpdateCollectionDetailTypeDef](./type_defs.md#updatecollectiondetailtypedef)
- [UpdateCollectionRequestRequestTypeDef](./type_defs.md#updatecollectionrequestrequesttypedef)
- [UpdateIamIdentityCenterConfigOptionsTypeDef](./type_defs.md#updateiamidentitycenterconfigoptionstypedef)
- [UpdateLifecyclePolicyRequestRequestTypeDef](./type_defs.md#updatelifecyclepolicyrequestrequesttypedef)
- [UpdateSecurityPolicyRequestRequestTypeDef](./type_defs.md#updatesecuritypolicyrequestrequesttypedef)
- [UpdateVpcEndpointDetailTypeDef](./type_defs.md#updatevpcendpointdetailtypedef)
- [UpdateVpcEndpointRequestRequestTypeDef](./type_defs.md#updatevpcendpointrequestrequesttypedef)
- [AccountSettingsDetailTypeDef](./type_defs.md#accountsettingsdetailtypedef)
- [UpdateAccountSettingsRequestRequestTypeDef](./type_defs.md#updateaccountsettingsrequestrequesttypedef)
- [BatchGetCollectionResponseTypeDef](./type_defs.md#batchgetcollectionresponsetypedef)
- [CreateAccessPolicyResponseTypeDef](./type_defs.md#createaccesspolicyresponsetypedef)
- [GetAccessPolicyResponseTypeDef](./type_defs.md#getaccesspolicyresponsetypedef)
- [ListAccessPoliciesResponseTypeDef](./type_defs.md#listaccesspoliciesresponsetypedef)
- [UpdateAccessPolicyResponseTypeDef](./type_defs.md#updateaccesspolicyresponsetypedef)
- [BatchGetEffectiveLifecyclePolicyRequestRequestTypeDef](./type_defs.md#batchgeteffectivelifecyclepolicyrequestrequesttypedef)
- [BatchGetEffectiveLifecyclePolicyResponseTypeDef](./type_defs.md#batchgeteffectivelifecyclepolicyresponsetypedef)
- [BatchGetLifecyclePolicyRequestRequestTypeDef](./type_defs.md#batchgetlifecyclepolicyrequestrequesttypedef)
- [CreateLifecyclePolicyResponseTypeDef](./type_defs.md#createlifecyclepolicyresponsetypedef)
- [UpdateLifecyclePolicyResponseTypeDef](./type_defs.md#updatelifecyclepolicyresponsetypedef)
- [BatchGetLifecyclePolicyResponseTypeDef](./type_defs.md#batchgetlifecyclepolicyresponsetypedef)
- [BatchGetVpcEndpointResponseTypeDef](./type_defs.md#batchgetvpcendpointresponsetypedef)
- [ListCollectionsRequestRequestTypeDef](./type_defs.md#listcollectionsrequestrequesttypedef)
- [ListCollectionsResponseTypeDef](./type_defs.md#listcollectionsresponsetypedef)
- [CreateCollectionResponseTypeDef](./type_defs.md#createcollectionresponsetypedef)
- [CreateCollectionRequestRequestTypeDef](./type_defs.md#createcollectionrequestrequesttypedef)
- [ListTagsForResourceResponseTypeDef](./type_defs.md#listtagsforresourceresponsetypedef)
- [TagResourceRequestRequestTypeDef](./type_defs.md#tagresourcerequestrequesttypedef)
- [CreateSecurityConfigRequestRequestTypeDef](./type_defs.md#createsecurityconfigrequestrequesttypedef)
- [CreateSecurityPolicyResponseTypeDef](./type_defs.md#createsecuritypolicyresponsetypedef)
- [GetSecurityPolicyResponseTypeDef](./type_defs.md#getsecuritypolicyresponsetypedef)
- [UpdateSecurityPolicyResponseTypeDef](./type_defs.md#updatesecuritypolicyresponsetypedef)
- [CreateVpcEndpointResponseTypeDef](./type_defs.md#createvpcendpointresponsetypedef)
- [DeleteCollectionResponseTypeDef](./type_defs.md#deletecollectionresponsetypedef)
- [DeleteVpcEndpointResponseTypeDef](./type_defs.md#deletevpcendpointresponsetypedef)
- [GetPoliciesStatsResponseTypeDef](./type_defs.md#getpoliciesstatsresponsetypedef)
- [SecurityConfigDetailTypeDef](./type_defs.md#securityconfigdetailtypedef)
- [ListLifecyclePoliciesResponseTypeDef](./type_defs.md#listlifecyclepoliciesresponsetypedef)
- [ListSecurityConfigsResponseTypeDef](./type_defs.md#listsecurityconfigsresponsetypedef)
- [ListSecurityPoliciesResponseTypeDef](./type_defs.md#listsecuritypoliciesresponsetypedef)
- [ListVpcEndpointsRequestRequestTypeDef](./type_defs.md#listvpcendpointsrequestrequesttypedef)
- [ListVpcEndpointsResponseTypeDef](./type_defs.md#listvpcendpointsresponsetypedef)
- [UpdateCollectionResponseTypeDef](./type_defs.md#updatecollectionresponsetypedef)
- [UpdateSecurityConfigRequestRequestTypeDef](./type_defs.md#updatesecurityconfigrequestrequesttypedef)
- [UpdateVpcEndpointResponseTypeDef](./type_defs.md#updatevpcendpointresponsetypedef)
- [GetAccountSettingsResponseTypeDef](./type_defs.md#getaccountsettingsresponsetypedef)
- [UpdateAccountSettingsResponseTypeDef](./type_defs.md#updateaccountsettingsresponsetypedef)
- [CreateSecurityConfigResponseTypeDef](./type_defs.md#createsecurityconfigresponsetypedef)
- [GetSecurityConfigResponseTypeDef](./type_defs.md#getsecurityconfigresponsetypedef)
- [UpdateSecurityConfigResponseTypeDef](./type_defs.md#updatesecurityconfigresponsetypedef)

