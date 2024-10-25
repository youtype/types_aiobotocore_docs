# Paginators

> [Index](../README.md) > [EKS](./README.md) > Paginators

!!! note ""

    Auto-generated documentation for [EKS](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/eks.html#EKS)
    type annotations stubs module [types-aiobotocore-eks](https://pypi.org/project/types-aiobotocore-eks/).

## DescribeAddonVersionsPaginator

Type annotations and code completion for `#!python session.create_client("eks").get_paginator("describe_addon_versions")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/eks.html#EKS.Paginator.DescribeAddonVersions)

```python
# DescribeAddonVersionsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_eks.paginator import DescribeAddonVersionsPaginator

session = get_session()
async with session.create_client("eks") as client:  # (1)
    paginator: DescribeAddonVersionsPaginator = client.get_paginator("describe_addon_versions")  # (2)
    async for item in paginator.paginate(...):
        item: DescribeAddonVersionsResponseTypeDef
        print(item)  # (3)
```

1. client: [EKSClient](./client.md)
2. paginator: [DescribeAddonVersionsPaginator](./paginators.md#describeaddonversionspaginator)
3. item: [:material-code-braces: DescribeAddonVersionsResponseTypeDef](./type_defs.md#describeaddonversionsresponsetypedef) 


### paginate

Type annotations and code completion for `#!python DescribeAddonVersionsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    kubernetesVersion: str = ...,
    addonName: str = ...,
    types: Sequence[str] = ...,
    publishers: Sequence[str] = ...,
    owners: Sequence[str] = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AsyncIterator[DescribeAddonVersionsResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: DescribeAddonVersionsResponseTypeDef](./type_defs.md#describeaddonversionsresponsetypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: DescribeAddonVersionsRequestDescribeAddonVersionsPaginateTypeDef = {  # (1)
    "kubernetesVersion": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: DescribeAddonVersionsRequestDescribeAddonVersionsPaginateTypeDef](./type_defs.md#describeaddonversionsrequestdescribeaddonversionspaginatetypedef) 
## ListAccessEntriesPaginator

Type annotations and code completion for `#!python session.create_client("eks").get_paginator("list_access_entries")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/eks.html#EKS.Paginator.ListAccessEntries)

```python
# ListAccessEntriesPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_eks.paginator import ListAccessEntriesPaginator

session = get_session()
async with session.create_client("eks") as client:  # (1)
    paginator: ListAccessEntriesPaginator = client.get_paginator("list_access_entries")  # (2)
    async for item in paginator.paginate(...):
        item: ListAccessEntriesResponseTypeDef
        print(item)  # (3)
```

1. client: [EKSClient](./client.md)
2. paginator: [ListAccessEntriesPaginator](./paginators.md#listaccessentriespaginator)
3. item: [:material-code-braces: ListAccessEntriesResponseTypeDef](./type_defs.md#listaccessentriesresponsetypedef) 


### paginate

Type annotations and code completion for `#!python ListAccessEntriesPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    clusterName: str,
    associatedPolicyArn: str = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AsyncIterator[ListAccessEntriesResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListAccessEntriesResponseTypeDef](./type_defs.md#listaccessentriesresponsetypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: ListAccessEntriesRequestListAccessEntriesPaginateTypeDef = {  # (1)
    "clusterName": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListAccessEntriesRequestListAccessEntriesPaginateTypeDef](./type_defs.md#listaccessentriesrequestlistaccessentriespaginatetypedef) 
## ListAccessPoliciesPaginator

Type annotations and code completion for `#!python session.create_client("eks").get_paginator("list_access_policies")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/eks.html#EKS.Paginator.ListAccessPolicies)

```python
# ListAccessPoliciesPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_eks.paginator import ListAccessPoliciesPaginator

session = get_session()
async with session.create_client("eks") as client:  # (1)
    paginator: ListAccessPoliciesPaginator = client.get_paginator("list_access_policies")  # (2)
    async for item in paginator.paginate(...):
        item: ListAccessPoliciesResponseTypeDef
        print(item)  # (3)
```

1. client: [EKSClient](./client.md)
2. paginator: [ListAccessPoliciesPaginator](./paginators.md#listaccesspoliciespaginator)
3. item: [:material-code-braces: ListAccessPoliciesResponseTypeDef](./type_defs.md#listaccesspoliciesresponsetypedef) 


### paginate

Type annotations and code completion for `#!python ListAccessPoliciesPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AsyncIterator[ListAccessPoliciesResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListAccessPoliciesResponseTypeDef](./type_defs.md#listaccesspoliciesresponsetypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: ListAccessPoliciesRequestListAccessPoliciesPaginateTypeDef = {  # (1)
    "PaginationConfig": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListAccessPoliciesRequestListAccessPoliciesPaginateTypeDef](./type_defs.md#listaccesspoliciesrequestlistaccesspoliciespaginatetypedef) 
## ListAddonsPaginator

Type annotations and code completion for `#!python session.create_client("eks").get_paginator("list_addons")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/eks.html#EKS.Paginator.ListAddons)

```python
# ListAddonsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_eks.paginator import ListAddonsPaginator

session = get_session()
async with session.create_client("eks") as client:  # (1)
    paginator: ListAddonsPaginator = client.get_paginator("list_addons")  # (2)
    async for item in paginator.paginate(...):
        item: ListAddonsResponseTypeDef
        print(item)  # (3)
```

1. client: [EKSClient](./client.md)
2. paginator: [ListAddonsPaginator](./paginators.md#listaddonspaginator)
3. item: [:material-code-braces: ListAddonsResponseTypeDef](./type_defs.md#listaddonsresponsetypedef) 


### paginate

Type annotations and code completion for `#!python ListAddonsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    clusterName: str,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AsyncIterator[ListAddonsResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListAddonsResponseTypeDef](./type_defs.md#listaddonsresponsetypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: ListAddonsRequestListAddonsPaginateTypeDef = {  # (1)
    "clusterName": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListAddonsRequestListAddonsPaginateTypeDef](./type_defs.md#listaddonsrequestlistaddonspaginatetypedef) 
## ListAssociatedAccessPoliciesPaginator

Type annotations and code completion for `#!python session.create_client("eks").get_paginator("list_associated_access_policies")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/eks.html#EKS.Paginator.ListAssociatedAccessPolicies)

```python
# ListAssociatedAccessPoliciesPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_eks.paginator import ListAssociatedAccessPoliciesPaginator

session = get_session()
async with session.create_client("eks") as client:  # (1)
    paginator: ListAssociatedAccessPoliciesPaginator = client.get_paginator("list_associated_access_policies")  # (2)
    async for item in paginator.paginate(...):
        item: ListAssociatedAccessPoliciesResponseTypeDef
        print(item)  # (3)
```

1. client: [EKSClient](./client.md)
2. paginator: [ListAssociatedAccessPoliciesPaginator](./paginators.md#listassociatedaccesspoliciespaginator)
3. item: [:material-code-braces: ListAssociatedAccessPoliciesResponseTypeDef](./type_defs.md#listassociatedaccesspoliciesresponsetypedef) 


### paginate

Type annotations and code completion for `#!python ListAssociatedAccessPoliciesPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    clusterName: str,
    principalArn: str,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AsyncIterator[ListAssociatedAccessPoliciesResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListAssociatedAccessPoliciesResponseTypeDef](./type_defs.md#listassociatedaccesspoliciesresponsetypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: ListAssociatedAccessPoliciesRequestListAssociatedAccessPoliciesPaginateTypeDef = {  # (1)
    "clusterName": ...,
    "principalArn": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListAssociatedAccessPoliciesRequestListAssociatedAccessPoliciesPaginateTypeDef](./type_defs.md#listassociatedaccesspoliciesrequestlistassociatedaccesspoliciespaginatetypedef) 
## ListClustersPaginator

Type annotations and code completion for `#!python session.create_client("eks").get_paginator("list_clusters")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/eks.html#EKS.Paginator.ListClusters)

```python
# ListClustersPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_eks.paginator import ListClustersPaginator

session = get_session()
async with session.create_client("eks") as client:  # (1)
    paginator: ListClustersPaginator = client.get_paginator("list_clusters")  # (2)
    async for item in paginator.paginate(...):
        item: ListClustersResponseTypeDef
        print(item)  # (3)
```

1. client: [EKSClient](./client.md)
2. paginator: [ListClustersPaginator](./paginators.md#listclusterspaginator)
3. item: [:material-code-braces: ListClustersResponseTypeDef](./type_defs.md#listclustersresponsetypedef) 


### paginate

Type annotations and code completion for `#!python ListClustersPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    include: Sequence[str] = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AsyncIterator[ListClustersResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListClustersResponseTypeDef](./type_defs.md#listclustersresponsetypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: ListClustersRequestListClustersPaginateTypeDef = {  # (1)
    "include": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListClustersRequestListClustersPaginateTypeDef](./type_defs.md#listclustersrequestlistclusterspaginatetypedef) 
## ListEksAnywhereSubscriptionsPaginator

Type annotations and code completion for `#!python session.create_client("eks").get_paginator("list_eks_anywhere_subscriptions")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/eks.html#EKS.Paginator.ListEksAnywhereSubscriptions)

```python
# ListEksAnywhereSubscriptionsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_eks.paginator import ListEksAnywhereSubscriptionsPaginator

session = get_session()
async with session.create_client("eks") as client:  # (1)
    paginator: ListEksAnywhereSubscriptionsPaginator = client.get_paginator("list_eks_anywhere_subscriptions")  # (2)
    async for item in paginator.paginate(...):
        item: ListEksAnywhereSubscriptionsResponseTypeDef
        print(item)  # (3)
```

1. client: [EKSClient](./client.md)
2. paginator: [ListEksAnywhereSubscriptionsPaginator](./paginators.md#listeksanywheresubscriptionspaginator)
3. item: [:material-code-braces: ListEksAnywhereSubscriptionsResponseTypeDef](./type_defs.md#listeksanywheresubscriptionsresponsetypedef) 


### paginate

Type annotations and code completion for `#!python ListEksAnywhereSubscriptionsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    includeStatus: Sequence[EksAnywhereSubscriptionStatusType] = ...,  # (1)
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (2)
) -> AsyncIterator[ListEksAnywhereSubscriptionsResponseTypeDef]:  # (3)
    ...
```

1. See [:material-code-brackets: EksAnywhereSubscriptionStatusType](./literals.md#eksanywheresubscriptionstatustype) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
3. See [:material-code-braces: ListEksAnywhereSubscriptionsResponseTypeDef](./type_defs.md#listeksanywheresubscriptionsresponsetypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: ListEksAnywhereSubscriptionsRequestListEksAnywhereSubscriptionsPaginateTypeDef = {  # (1)
    "includeStatus": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListEksAnywhereSubscriptionsRequestListEksAnywhereSubscriptionsPaginateTypeDef](./type_defs.md#listeksanywheresubscriptionsrequestlisteksanywheresubscriptionspaginatetypedef) 
## ListFargateProfilesPaginator

Type annotations and code completion for `#!python session.create_client("eks").get_paginator("list_fargate_profiles")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/eks.html#EKS.Paginator.ListFargateProfiles)

```python
# ListFargateProfilesPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_eks.paginator import ListFargateProfilesPaginator

session = get_session()
async with session.create_client("eks") as client:  # (1)
    paginator: ListFargateProfilesPaginator = client.get_paginator("list_fargate_profiles")  # (2)
    async for item in paginator.paginate(...):
        item: ListFargateProfilesResponseTypeDef
        print(item)  # (3)
```

1. client: [EKSClient](./client.md)
2. paginator: [ListFargateProfilesPaginator](./paginators.md#listfargateprofilespaginator)
3. item: [:material-code-braces: ListFargateProfilesResponseTypeDef](./type_defs.md#listfargateprofilesresponsetypedef) 


### paginate

Type annotations and code completion for `#!python ListFargateProfilesPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    clusterName: str,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AsyncIterator[ListFargateProfilesResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListFargateProfilesResponseTypeDef](./type_defs.md#listfargateprofilesresponsetypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: ListFargateProfilesRequestListFargateProfilesPaginateTypeDef = {  # (1)
    "clusterName": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListFargateProfilesRequestListFargateProfilesPaginateTypeDef](./type_defs.md#listfargateprofilesrequestlistfargateprofilespaginatetypedef) 
## ListIdentityProviderConfigsPaginator

Type annotations and code completion for `#!python session.create_client("eks").get_paginator("list_identity_provider_configs")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/eks.html#EKS.Paginator.ListIdentityProviderConfigs)

```python
# ListIdentityProviderConfigsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_eks.paginator import ListIdentityProviderConfigsPaginator

session = get_session()
async with session.create_client("eks") as client:  # (1)
    paginator: ListIdentityProviderConfigsPaginator = client.get_paginator("list_identity_provider_configs")  # (2)
    async for item in paginator.paginate(...):
        item: ListIdentityProviderConfigsResponseTypeDef
        print(item)  # (3)
```

1. client: [EKSClient](./client.md)
2. paginator: [ListIdentityProviderConfigsPaginator](./paginators.md#listidentityproviderconfigspaginator)
3. item: [:material-code-braces: ListIdentityProviderConfigsResponseTypeDef](./type_defs.md#listidentityproviderconfigsresponsetypedef) 


### paginate

Type annotations and code completion for `#!python ListIdentityProviderConfigsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    clusterName: str,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AsyncIterator[ListIdentityProviderConfigsResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListIdentityProviderConfigsResponseTypeDef](./type_defs.md#listidentityproviderconfigsresponsetypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: ListIdentityProviderConfigsRequestListIdentityProviderConfigsPaginateTypeDef = {  # (1)
    "clusterName": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListIdentityProviderConfigsRequestListIdentityProviderConfigsPaginateTypeDef](./type_defs.md#listidentityproviderconfigsrequestlistidentityproviderconfigspaginatetypedef) 
## ListInsightsPaginator

Type annotations and code completion for `#!python session.create_client("eks").get_paginator("list_insights")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/eks.html#EKS.Paginator.ListInsights)

```python
# ListInsightsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_eks.paginator import ListInsightsPaginator

session = get_session()
async with session.create_client("eks") as client:  # (1)
    paginator: ListInsightsPaginator = client.get_paginator("list_insights")  # (2)
    async for item in paginator.paginate(...):
        item: ListInsightsResponseTypeDef
        print(item)  # (3)
```

1. client: [EKSClient](./client.md)
2. paginator: [ListInsightsPaginator](./paginators.md#listinsightspaginator)
3. item: [:material-code-braces: ListInsightsResponseTypeDef](./type_defs.md#listinsightsresponsetypedef) 


### paginate

Type annotations and code completion for `#!python ListInsightsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    clusterName: str,
    filter: InsightsFilterTypeDef = ...,  # (1)
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (2)
) -> AsyncIterator[ListInsightsResponseTypeDef]:  # (3)
    ...
```

1. See [:material-code-braces: InsightsFilterTypeDef](./type_defs.md#insightsfiltertypedef) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
3. See [:material-code-braces: ListInsightsResponseTypeDef](./type_defs.md#listinsightsresponsetypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: ListInsightsRequestListInsightsPaginateTypeDef = {  # (1)
    "clusterName": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListInsightsRequestListInsightsPaginateTypeDef](./type_defs.md#listinsightsrequestlistinsightspaginatetypedef) 
## ListNodegroupsPaginator

Type annotations and code completion for `#!python session.create_client("eks").get_paginator("list_nodegroups")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/eks.html#EKS.Paginator.ListNodegroups)

```python
# ListNodegroupsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_eks.paginator import ListNodegroupsPaginator

session = get_session()
async with session.create_client("eks") as client:  # (1)
    paginator: ListNodegroupsPaginator = client.get_paginator("list_nodegroups")  # (2)
    async for item in paginator.paginate(...):
        item: ListNodegroupsResponseTypeDef
        print(item)  # (3)
```

1. client: [EKSClient](./client.md)
2. paginator: [ListNodegroupsPaginator](./paginators.md#listnodegroupspaginator)
3. item: [:material-code-braces: ListNodegroupsResponseTypeDef](./type_defs.md#listnodegroupsresponsetypedef) 


### paginate

Type annotations and code completion for `#!python ListNodegroupsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    clusterName: str,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AsyncIterator[ListNodegroupsResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListNodegroupsResponseTypeDef](./type_defs.md#listnodegroupsresponsetypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: ListNodegroupsRequestListNodegroupsPaginateTypeDef = {  # (1)
    "clusterName": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListNodegroupsRequestListNodegroupsPaginateTypeDef](./type_defs.md#listnodegroupsrequestlistnodegroupspaginatetypedef) 
## ListPodIdentityAssociationsPaginator

Type annotations and code completion for `#!python session.create_client("eks").get_paginator("list_pod_identity_associations")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/eks.html#EKS.Paginator.ListPodIdentityAssociations)

```python
# ListPodIdentityAssociationsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_eks.paginator import ListPodIdentityAssociationsPaginator

session = get_session()
async with session.create_client("eks") as client:  # (1)
    paginator: ListPodIdentityAssociationsPaginator = client.get_paginator("list_pod_identity_associations")  # (2)
    async for item in paginator.paginate(...):
        item: ListPodIdentityAssociationsResponseTypeDef
        print(item)  # (3)
```

1. client: [EKSClient](./client.md)
2. paginator: [ListPodIdentityAssociationsPaginator](./paginators.md#listpodidentityassociationspaginator)
3. item: [:material-code-braces: ListPodIdentityAssociationsResponseTypeDef](./type_defs.md#listpodidentityassociationsresponsetypedef) 


### paginate

Type annotations and code completion for `#!python ListPodIdentityAssociationsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    clusterName: str,
    namespace: str = ...,
    serviceAccount: str = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AsyncIterator[ListPodIdentityAssociationsResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListPodIdentityAssociationsResponseTypeDef](./type_defs.md#listpodidentityassociationsresponsetypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: ListPodIdentityAssociationsRequestListPodIdentityAssociationsPaginateTypeDef = {  # (1)
    "clusterName": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListPodIdentityAssociationsRequestListPodIdentityAssociationsPaginateTypeDef](./type_defs.md#listpodidentityassociationsrequestlistpodidentityassociationspaginatetypedef) 
## ListUpdatesPaginator

Type annotations and code completion for `#!python session.create_client("eks").get_paginator("list_updates")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/eks.html#EKS.Paginator.ListUpdates)

```python
# ListUpdatesPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_eks.paginator import ListUpdatesPaginator

session = get_session()
async with session.create_client("eks") as client:  # (1)
    paginator: ListUpdatesPaginator = client.get_paginator("list_updates")  # (2)
    async for item in paginator.paginate(...):
        item: ListUpdatesResponseTypeDef
        print(item)  # (3)
```

1. client: [EKSClient](./client.md)
2. paginator: [ListUpdatesPaginator](./paginators.md#listupdatespaginator)
3. item: [:material-code-braces: ListUpdatesResponseTypeDef](./type_defs.md#listupdatesresponsetypedef) 


### paginate

Type annotations and code completion for `#!python ListUpdatesPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    name: str,
    nodegroupName: str = ...,
    addonName: str = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AsyncIterator[ListUpdatesResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListUpdatesResponseTypeDef](./type_defs.md#listupdatesresponsetypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: ListUpdatesRequestListUpdatesPaginateTypeDef = {  # (1)
    "name": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListUpdatesRequestListUpdatesPaginateTypeDef](./type_defs.md#listupdatesrequestlistupdatespaginatetypedef) 
