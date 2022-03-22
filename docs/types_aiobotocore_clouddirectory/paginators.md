<a id="paginators-for-aiobotocore-clouddirectory-module"></a>

# Paginators for aiobotocore CloudDirectory module

> [Index](../README.md) > [CloudDirectory](./README.md) > Paginators

Auto-generated documentation for
[CloudDirectory](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/clouddirectory.html#CloudDirectory)
type annotations stubs module
[types-aiobotocore-clouddirectory](https://pypi.org/project/types-aiobotocore-clouddirectory/).

- [Paginators for aiobotocore CloudDirectory module](#paginators-for-aiobotocore-clouddirectory-module)
  - [ListAppliedSchemaArnsPaginator](#listappliedschemaarnspaginator)
  - [ListAttachedIndicesPaginator](#listattachedindicespaginator)
  - [ListDevelopmentSchemaArnsPaginator](#listdevelopmentschemaarnspaginator)
  - [ListDirectoriesPaginator](#listdirectoriespaginator)
  - [ListFacetAttributesPaginator](#listfacetattributespaginator)
  - [ListFacetNamesPaginator](#listfacetnamespaginator)
  - [ListIncomingTypedLinksPaginator](#listincomingtypedlinkspaginator)
  - [ListIndexPaginator](#listindexpaginator)
  - [ListManagedSchemaArnsPaginator](#listmanagedschemaarnspaginator)
  - [ListObjectAttributesPaginator](#listobjectattributespaginator)
  - [ListObjectParentPathsPaginator](#listobjectparentpathspaginator)
  - [ListObjectPoliciesPaginator](#listobjectpoliciespaginator)
  - [ListOutgoingTypedLinksPaginator](#listoutgoingtypedlinkspaginator)
  - [ListPolicyAttachmentsPaginator](#listpolicyattachmentspaginator)
  - [ListPublishedSchemaArnsPaginator](#listpublishedschemaarnspaginator)
  - [ListTagsForResourcePaginator](#listtagsforresourcepaginator)
  - [ListTypedLinkFacetAttributesPaginator](#listtypedlinkfacetattributespaginator)
  - [ListTypedLinkFacetNamesPaginator](#listtypedlinkfacetnamespaginator)
  - [LookupPolicyPaginator](#lookuppolicypaginator)

<a id="listappliedschemaarnspaginator"></a>

## ListAppliedSchemaArnsPaginator

Type annotations for
`session.create_client("clouddirectory").get_paginator("list_applied_schema_arns")`.

Can be used directly:

```python
from aiobotocore.session import get_session

from types_aiobotocore_clouddirectory.paginator import ListAppliedSchemaArnsPaginator

session = get_session()
async with session.create_client("clouddirectory") as client:
    client: CloudDirectoryClient
    paginator: ListAppliedSchemaArnsPaginator = client.get_paginator("list_applied_schema_arns")
```

Boto3 documentation:
[CloudDirectory.Paginator.ListAppliedSchemaArns](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/clouddirectory.html#CloudDirectory.Paginator.ListAppliedSchemaArns)

Arguments for `ListAppliedSchemaArnsPaginator.paginate` method:

- `DirectoryArn`: `str` *(required)*
- `SchemaArn`: `str`
- `PaginationConfig`:
  [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)

`ListAppliedSchemaArnsPaginator.paginate` returns
`AsyncIterator`\[[ListAppliedSchemaArnsResponseTypeDef](./type_defs.md#listappliedschemaarnsresponsetypedef)\].

<a id="listattachedindicespaginator"></a>

## ListAttachedIndicesPaginator

Type annotations for
`session.create_client("clouddirectory").get_paginator("list_attached_indices")`.

Can be used directly:

```python
from aiobotocore.session import get_session

from types_aiobotocore_clouddirectory.paginator import ListAttachedIndicesPaginator

session = get_session()
async with session.create_client("clouddirectory") as client:
    client: CloudDirectoryClient
    paginator: ListAttachedIndicesPaginator = client.get_paginator("list_attached_indices")
```

Boto3 documentation:
[CloudDirectory.Paginator.ListAttachedIndices](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/clouddirectory.html#CloudDirectory.Paginator.ListAttachedIndices)

Arguments for `ListAttachedIndicesPaginator.paginate` method:

- `DirectoryArn`: `str` *(required)*
- `TargetReference`:
  [ObjectReferenceTypeDef](./type_defs.md#objectreferencetypedef) *(required)*
- `ConsistencyLevel`:
  [ConsistencyLevelType](./literals.md#consistencyleveltype)
- `PaginationConfig`:
  [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)

`ListAttachedIndicesPaginator.paginate` returns
`AsyncIterator`\[[ListAttachedIndicesResponseTypeDef](./type_defs.md#listattachedindicesresponsetypedef)\].

<a id="listdevelopmentschemaarnspaginator"></a>

## ListDevelopmentSchemaArnsPaginator

Type annotations for
`session.create_client("clouddirectory").get_paginator("list_development_schema_arns")`.

Can be used directly:

```python
from aiobotocore.session import get_session

from types_aiobotocore_clouddirectory.paginator import ListDevelopmentSchemaArnsPaginator

session = get_session()
async with session.create_client("clouddirectory") as client:
    client: CloudDirectoryClient
    paginator: ListDevelopmentSchemaArnsPaginator = client.get_paginator("list_development_schema_arns")
```

Boto3 documentation:
[CloudDirectory.Paginator.ListDevelopmentSchemaArns](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/clouddirectory.html#CloudDirectory.Paginator.ListDevelopmentSchemaArns)

Arguments for `ListDevelopmentSchemaArnsPaginator.paginate` method:

- `PaginationConfig`:
  [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)

`ListDevelopmentSchemaArnsPaginator.paginate` returns
`AsyncIterator`\[[ListDevelopmentSchemaArnsResponseTypeDef](./type_defs.md#listdevelopmentschemaarnsresponsetypedef)\].

<a id="listdirectoriespaginator"></a>

## ListDirectoriesPaginator

Type annotations for
`session.create_client("clouddirectory").get_paginator("list_directories")`.

Can be used directly:

```python
from aiobotocore.session import get_session

from types_aiobotocore_clouddirectory.paginator import ListDirectoriesPaginator

session = get_session()
async with session.create_client("clouddirectory") as client:
    client: CloudDirectoryClient
    paginator: ListDirectoriesPaginator = client.get_paginator("list_directories")
```

Boto3 documentation:
[CloudDirectory.Paginator.ListDirectories](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/clouddirectory.html#CloudDirectory.Paginator.ListDirectories)

Arguments for `ListDirectoriesPaginator.paginate` method:

- `state`: [DirectoryStateType](./literals.md#directorystatetype)
- `PaginationConfig`:
  [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)

`ListDirectoriesPaginator.paginate` returns
`AsyncIterator`\[[ListDirectoriesResponseTypeDef](./type_defs.md#listdirectoriesresponsetypedef)\].

<a id="listfacetattributespaginator"></a>

## ListFacetAttributesPaginator

Type annotations for
`session.create_client("clouddirectory").get_paginator("list_facet_attributes")`.

Can be used directly:

```python
from aiobotocore.session import get_session

from types_aiobotocore_clouddirectory.paginator import ListFacetAttributesPaginator

session = get_session()
async with session.create_client("clouddirectory") as client:
    client: CloudDirectoryClient
    paginator: ListFacetAttributesPaginator = client.get_paginator("list_facet_attributes")
```

Boto3 documentation:
[CloudDirectory.Paginator.ListFacetAttributes](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/clouddirectory.html#CloudDirectory.Paginator.ListFacetAttributes)

Arguments for `ListFacetAttributesPaginator.paginate` method:

- `SchemaArn`: `str` *(required)*
- `Name`: `str` *(required)*
- `PaginationConfig`:
  [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)

`ListFacetAttributesPaginator.paginate` returns
`AsyncIterator`\[[ListFacetAttributesResponseTypeDef](./type_defs.md#listfacetattributesresponsetypedef)\].

<a id="listfacetnamespaginator"></a>

## ListFacetNamesPaginator

Type annotations for
`session.create_client("clouddirectory").get_paginator("list_facet_names")`.

Can be used directly:

```python
from aiobotocore.session import get_session

from types_aiobotocore_clouddirectory.paginator import ListFacetNamesPaginator

session = get_session()
async with session.create_client("clouddirectory") as client:
    client: CloudDirectoryClient
    paginator: ListFacetNamesPaginator = client.get_paginator("list_facet_names")
```

Boto3 documentation:
[CloudDirectory.Paginator.ListFacetNames](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/clouddirectory.html#CloudDirectory.Paginator.ListFacetNames)

Arguments for `ListFacetNamesPaginator.paginate` method:

- `SchemaArn`: `str` *(required)*
- `PaginationConfig`:
  [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)

`ListFacetNamesPaginator.paginate` returns
`AsyncIterator`\[[ListFacetNamesResponseTypeDef](./type_defs.md#listfacetnamesresponsetypedef)\].

<a id="listincomingtypedlinkspaginator"></a>

## ListIncomingTypedLinksPaginator

Type annotations for
`session.create_client("clouddirectory").get_paginator("list_incoming_typed_links")`.

Can be used directly:

```python
from aiobotocore.session import get_session

from types_aiobotocore_clouddirectory.paginator import ListIncomingTypedLinksPaginator

session = get_session()
async with session.create_client("clouddirectory") as client:
    client: CloudDirectoryClient
    paginator: ListIncomingTypedLinksPaginator = client.get_paginator("list_incoming_typed_links")
```

Boto3 documentation:
[CloudDirectory.Paginator.ListIncomingTypedLinks](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/clouddirectory.html#CloudDirectory.Paginator.ListIncomingTypedLinks)

Arguments for `ListIncomingTypedLinksPaginator.paginate` method:

- `DirectoryArn`: `str` *(required)*
- `ObjectReference`:
  [ObjectReferenceTypeDef](./type_defs.md#objectreferencetypedef) *(required)*
- `FilterAttributeRanges`:
  `Sequence`\[[TypedLinkAttributeRangeTypeDef](./type_defs.md#typedlinkattributerangetypedef)\]
- `FilterTypedLink`:
  [TypedLinkSchemaAndFacetNameTypeDef](./type_defs.md#typedlinkschemaandfacetnametypedef)
- `ConsistencyLevel`:
  [ConsistencyLevelType](./literals.md#consistencyleveltype)
- `PaginationConfig`:
  [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)

`ListIncomingTypedLinksPaginator.paginate` returns
`AsyncIterator`\[[ListIncomingTypedLinksResponseTypeDef](./type_defs.md#listincomingtypedlinksresponsetypedef)\].

<a id="listindexpaginator"></a>

## ListIndexPaginator

Type annotations for
`session.create_client("clouddirectory").get_paginator("list_index")`.

Can be used directly:

```python
from aiobotocore.session import get_session

from types_aiobotocore_clouddirectory.paginator import ListIndexPaginator

session = get_session()
async with session.create_client("clouddirectory") as client:
    client: CloudDirectoryClient
    paginator: ListIndexPaginator = client.get_paginator("list_index")
```

Boto3 documentation:
[CloudDirectory.Paginator.ListIndex](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/clouddirectory.html#CloudDirectory.Paginator.ListIndex)

Arguments for `ListIndexPaginator.paginate` method:

- `DirectoryArn`: `str` *(required)*
- `IndexReference`:
  [ObjectReferenceTypeDef](./type_defs.md#objectreferencetypedef) *(required)*
- `RangesOnIndexedValues`:
  `Sequence`\[[ObjectAttributeRangeTypeDef](./type_defs.md#objectattributerangetypedef)\]
- `ConsistencyLevel`:
  [ConsistencyLevelType](./literals.md#consistencyleveltype)
- `PaginationConfig`:
  [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)

`ListIndexPaginator.paginate` returns
`AsyncIterator`\[[ListIndexResponseTypeDef](./type_defs.md#listindexresponsetypedef)\].

<a id="listmanagedschemaarnspaginator"></a>

## ListManagedSchemaArnsPaginator

Type annotations for
`session.create_client("clouddirectory").get_paginator("list_managed_schema_arns")`.

Can be used directly:

```python
from aiobotocore.session import get_session

from types_aiobotocore_clouddirectory.paginator import ListManagedSchemaArnsPaginator

session = get_session()
async with session.create_client("clouddirectory") as client:
    client: CloudDirectoryClient
    paginator: ListManagedSchemaArnsPaginator = client.get_paginator("list_managed_schema_arns")
```

Boto3 documentation:
[CloudDirectory.Paginator.ListManagedSchemaArns](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/clouddirectory.html#CloudDirectory.Paginator.ListManagedSchemaArns)

Arguments for `ListManagedSchemaArnsPaginator.paginate` method:

- `SchemaArn`: `str`
- `PaginationConfig`:
  [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)

`ListManagedSchemaArnsPaginator.paginate` returns
`AsyncIterator`\[[ListManagedSchemaArnsResponseTypeDef](./type_defs.md#listmanagedschemaarnsresponsetypedef)\].

<a id="listobjectattributespaginator"></a>

## ListObjectAttributesPaginator

Type annotations for
`session.create_client("clouddirectory").get_paginator("list_object_attributes")`.

Can be used directly:

```python
from aiobotocore.session import get_session

from types_aiobotocore_clouddirectory.paginator import ListObjectAttributesPaginator

session = get_session()
async with session.create_client("clouddirectory") as client:
    client: CloudDirectoryClient
    paginator: ListObjectAttributesPaginator = client.get_paginator("list_object_attributes")
```

Boto3 documentation:
[CloudDirectory.Paginator.ListObjectAttributes](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/clouddirectory.html#CloudDirectory.Paginator.ListObjectAttributes)

Arguments for `ListObjectAttributesPaginator.paginate` method:

- `DirectoryArn`: `str` *(required)*
- `ObjectReference`:
  [ObjectReferenceTypeDef](./type_defs.md#objectreferencetypedef) *(required)*
- `ConsistencyLevel`:
  [ConsistencyLevelType](./literals.md#consistencyleveltype)
- `FacetFilter`: [SchemaFacetTypeDef](./type_defs.md#schemafacettypedef)
- `PaginationConfig`:
  [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)

`ListObjectAttributesPaginator.paginate` returns
`AsyncIterator`\[[ListObjectAttributesResponseTypeDef](./type_defs.md#listobjectattributesresponsetypedef)\].

<a id="listobjectparentpathspaginator"></a>

## ListObjectParentPathsPaginator

Type annotations for
`session.create_client("clouddirectory").get_paginator("list_object_parent_paths")`.

Can be used directly:

```python
from aiobotocore.session import get_session

from types_aiobotocore_clouddirectory.paginator import ListObjectParentPathsPaginator

session = get_session()
async with session.create_client("clouddirectory") as client:
    client: CloudDirectoryClient
    paginator: ListObjectParentPathsPaginator = client.get_paginator("list_object_parent_paths")
```

Boto3 documentation:
[CloudDirectory.Paginator.ListObjectParentPaths](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/clouddirectory.html#CloudDirectory.Paginator.ListObjectParentPaths)

Arguments for `ListObjectParentPathsPaginator.paginate` method:

- `DirectoryArn`: `str` *(required)*
- `ObjectReference`:
  [ObjectReferenceTypeDef](./type_defs.md#objectreferencetypedef) *(required)*
- `PaginationConfig`:
  [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)

`ListObjectParentPathsPaginator.paginate` returns
`AsyncIterator`\[[ListObjectParentPathsResponseTypeDef](./type_defs.md#listobjectparentpathsresponsetypedef)\].

<a id="listobjectpoliciespaginator"></a>

## ListObjectPoliciesPaginator

Type annotations for
`session.create_client("clouddirectory").get_paginator("list_object_policies")`.

Can be used directly:

```python
from aiobotocore.session import get_session

from types_aiobotocore_clouddirectory.paginator import ListObjectPoliciesPaginator

session = get_session()
async with session.create_client("clouddirectory") as client:
    client: CloudDirectoryClient
    paginator: ListObjectPoliciesPaginator = client.get_paginator("list_object_policies")
```

Boto3 documentation:
[CloudDirectory.Paginator.ListObjectPolicies](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/clouddirectory.html#CloudDirectory.Paginator.ListObjectPolicies)

Arguments for `ListObjectPoliciesPaginator.paginate` method:

- `DirectoryArn`: `str` *(required)*
- `ObjectReference`:
  [ObjectReferenceTypeDef](./type_defs.md#objectreferencetypedef) *(required)*
- `ConsistencyLevel`:
  [ConsistencyLevelType](./literals.md#consistencyleveltype)
- `PaginationConfig`:
  [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)

`ListObjectPoliciesPaginator.paginate` returns
`AsyncIterator`\[[ListObjectPoliciesResponseTypeDef](./type_defs.md#listobjectpoliciesresponsetypedef)\].

<a id="listoutgoingtypedlinkspaginator"></a>

## ListOutgoingTypedLinksPaginator

Type annotations for
`session.create_client("clouddirectory").get_paginator("list_outgoing_typed_links")`.

Can be used directly:

```python
from aiobotocore.session import get_session

from types_aiobotocore_clouddirectory.paginator import ListOutgoingTypedLinksPaginator

session = get_session()
async with session.create_client("clouddirectory") as client:
    client: CloudDirectoryClient
    paginator: ListOutgoingTypedLinksPaginator = client.get_paginator("list_outgoing_typed_links")
```

Boto3 documentation:
[CloudDirectory.Paginator.ListOutgoingTypedLinks](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/clouddirectory.html#CloudDirectory.Paginator.ListOutgoingTypedLinks)

Arguments for `ListOutgoingTypedLinksPaginator.paginate` method:

- `DirectoryArn`: `str` *(required)*
- `ObjectReference`:
  [ObjectReferenceTypeDef](./type_defs.md#objectreferencetypedef) *(required)*
- `FilterAttributeRanges`:
  `Sequence`\[[TypedLinkAttributeRangeTypeDef](./type_defs.md#typedlinkattributerangetypedef)\]
- `FilterTypedLink`:
  [TypedLinkSchemaAndFacetNameTypeDef](./type_defs.md#typedlinkschemaandfacetnametypedef)
- `ConsistencyLevel`:
  [ConsistencyLevelType](./literals.md#consistencyleveltype)
- `PaginationConfig`:
  [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)

`ListOutgoingTypedLinksPaginator.paginate` returns
`AsyncIterator`\[[ListOutgoingTypedLinksResponseTypeDef](./type_defs.md#listoutgoingtypedlinksresponsetypedef)\].

<a id="listpolicyattachmentspaginator"></a>

## ListPolicyAttachmentsPaginator

Type annotations for
`session.create_client("clouddirectory").get_paginator("list_policy_attachments")`.

Can be used directly:

```python
from aiobotocore.session import get_session

from types_aiobotocore_clouddirectory.paginator import ListPolicyAttachmentsPaginator

session = get_session()
async with session.create_client("clouddirectory") as client:
    client: CloudDirectoryClient
    paginator: ListPolicyAttachmentsPaginator = client.get_paginator("list_policy_attachments")
```

Boto3 documentation:
[CloudDirectory.Paginator.ListPolicyAttachments](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/clouddirectory.html#CloudDirectory.Paginator.ListPolicyAttachments)

Arguments for `ListPolicyAttachmentsPaginator.paginate` method:

- `DirectoryArn`: `str` *(required)*
- `PolicyReference`:
  [ObjectReferenceTypeDef](./type_defs.md#objectreferencetypedef) *(required)*
- `ConsistencyLevel`:
  [ConsistencyLevelType](./literals.md#consistencyleveltype)
- `PaginationConfig`:
  [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)

`ListPolicyAttachmentsPaginator.paginate` returns
`AsyncIterator`\[[ListPolicyAttachmentsResponseTypeDef](./type_defs.md#listpolicyattachmentsresponsetypedef)\].

<a id="listpublishedschemaarnspaginator"></a>

## ListPublishedSchemaArnsPaginator

Type annotations for
`session.create_client("clouddirectory").get_paginator("list_published_schema_arns")`.

Can be used directly:

```python
from aiobotocore.session import get_session

from types_aiobotocore_clouddirectory.paginator import ListPublishedSchemaArnsPaginator

session = get_session()
async with session.create_client("clouddirectory") as client:
    client: CloudDirectoryClient
    paginator: ListPublishedSchemaArnsPaginator = client.get_paginator("list_published_schema_arns")
```

Boto3 documentation:
[CloudDirectory.Paginator.ListPublishedSchemaArns](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/clouddirectory.html#CloudDirectory.Paginator.ListPublishedSchemaArns)

Arguments for `ListPublishedSchemaArnsPaginator.paginate` method:

- `SchemaArn`: `str`
- `PaginationConfig`:
  [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)

`ListPublishedSchemaArnsPaginator.paginate` returns
`AsyncIterator`\[[ListPublishedSchemaArnsResponseTypeDef](./type_defs.md#listpublishedschemaarnsresponsetypedef)\].

<a id="listtagsforresourcepaginator"></a>

## ListTagsForResourcePaginator

Type annotations for
`session.create_client("clouddirectory").get_paginator("list_tags_for_resource")`.

Can be used directly:

```python
from aiobotocore.session import get_session

from types_aiobotocore_clouddirectory.paginator import ListTagsForResourcePaginator

session = get_session()
async with session.create_client("clouddirectory") as client:
    client: CloudDirectoryClient
    paginator: ListTagsForResourcePaginator = client.get_paginator("list_tags_for_resource")
```

Boto3 documentation:
[CloudDirectory.Paginator.ListTagsForResource](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/clouddirectory.html#CloudDirectory.Paginator.ListTagsForResource)

Arguments for `ListTagsForResourcePaginator.paginate` method:

- `ResourceArn`: `str` *(required)*
- `PaginationConfig`:
  [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)

`ListTagsForResourcePaginator.paginate` returns
`AsyncIterator`\[[ListTagsForResourceResponseTypeDef](./type_defs.md#listtagsforresourceresponsetypedef)\].

<a id="listtypedlinkfacetattributespaginator"></a>

## ListTypedLinkFacetAttributesPaginator

Type annotations for
`session.create_client("clouddirectory").get_paginator("list_typed_link_facet_attributes")`.

Can be used directly:

```python
from aiobotocore.session import get_session

from types_aiobotocore_clouddirectory.paginator import ListTypedLinkFacetAttributesPaginator

session = get_session()
async with session.create_client("clouddirectory") as client:
    client: CloudDirectoryClient
    paginator: ListTypedLinkFacetAttributesPaginator = client.get_paginator("list_typed_link_facet_attributes")
```

Boto3 documentation:
[CloudDirectory.Paginator.ListTypedLinkFacetAttributes](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/clouddirectory.html#CloudDirectory.Paginator.ListTypedLinkFacetAttributes)

Arguments for `ListTypedLinkFacetAttributesPaginator.paginate` method:

- `SchemaArn`: `str` *(required)*
- `Name`: `str` *(required)*
- `PaginationConfig`:
  [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)

`ListTypedLinkFacetAttributesPaginator.paginate` returns
`AsyncIterator`\[[ListTypedLinkFacetAttributesResponseTypeDef](./type_defs.md#listtypedlinkfacetattributesresponsetypedef)\].

<a id="listtypedlinkfacetnamespaginator"></a>

## ListTypedLinkFacetNamesPaginator

Type annotations for
`session.create_client("clouddirectory").get_paginator("list_typed_link_facet_names")`.

Can be used directly:

```python
from aiobotocore.session import get_session

from types_aiobotocore_clouddirectory.paginator import ListTypedLinkFacetNamesPaginator

session = get_session()
async with session.create_client("clouddirectory") as client:
    client: CloudDirectoryClient
    paginator: ListTypedLinkFacetNamesPaginator = client.get_paginator("list_typed_link_facet_names")
```

Boto3 documentation:
[CloudDirectory.Paginator.ListTypedLinkFacetNames](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/clouddirectory.html#CloudDirectory.Paginator.ListTypedLinkFacetNames)

Arguments for `ListTypedLinkFacetNamesPaginator.paginate` method:

- `SchemaArn`: `str` *(required)*
- `PaginationConfig`:
  [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)

`ListTypedLinkFacetNamesPaginator.paginate` returns
`AsyncIterator`\[[ListTypedLinkFacetNamesResponseTypeDef](./type_defs.md#listtypedlinkfacetnamesresponsetypedef)\].

<a id="lookuppolicypaginator"></a>

## LookupPolicyPaginator

Type annotations for
`session.create_client("clouddirectory").get_paginator("lookup_policy")`.

Can be used directly:

```python
from aiobotocore.session import get_session

from types_aiobotocore_clouddirectory.paginator import LookupPolicyPaginator

session = get_session()
async with session.create_client("clouddirectory") as client:
    client: CloudDirectoryClient
    paginator: LookupPolicyPaginator = client.get_paginator("lookup_policy")
```

Boto3 documentation:
[CloudDirectory.Paginator.LookupPolicy](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/clouddirectory.html#CloudDirectory.Paginator.LookupPolicy)

Arguments for `LookupPolicyPaginator.paginate` method:

- `DirectoryArn`: `str` *(required)*
- `ObjectReference`:
  [ObjectReferenceTypeDef](./type_defs.md#objectreferencetypedef) *(required)*
- `PaginationConfig`:
  [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)

`LookupPolicyPaginator.paginate` returns
`AsyncIterator`\[[LookupPolicyResponseTypeDef](./type_defs.md#lookuppolicyresponsetypedef)\].
