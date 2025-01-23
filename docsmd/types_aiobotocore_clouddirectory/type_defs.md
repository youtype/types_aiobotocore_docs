# Type definitions

> [Index](../README.md) > [CloudDirectory](./README.md) > Type definitions

!!! note ""

    Auto-generated documentation for [CloudDirectory](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/clouddirectory.html#clouddirectory)
    type annotations stubs module [types-aiobotocore-clouddirectory](https://pypi.org/project/types-aiobotocore-clouddirectory/).

## BlobTypeDef

```python
# BlobTypeDef definition

BlobTypeDef = Union[
    str,
    bytes,
    IO[Any],
    StreamingBody,
]
```


## TimestampTypeDef

```python
# TimestampTypeDef definition

TimestampTypeDef = Union[
    datetime,
    str,
]
```


## RuleUnionTypeDef

```python
# RuleUnionTypeDef definition

RuleUnionTypeDef = Union[
    RuleTypeDef,  # (1)
    RuleOutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: RuleTypeDef](./type_defs.md#ruletypedef) 
2. See [:material-code-braces: RuleOutputTypeDef](./type_defs.md#ruleoutputtypedef) 

## TypedAttributeValueUnionTypeDef

```python
# TypedAttributeValueUnionTypeDef definition

TypedAttributeValueUnionTypeDef = Union[
    TypedAttributeValueTypeDef,  # (1)
    TypedAttributeValueOutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: TypedAttributeValueTypeDef](./type_defs.md#typedattributevaluetypedef) 
2. See [:material-code-braces: TypedAttributeValueOutputTypeDef](./type_defs.md#typedattributevalueoutputtypedef) 

## AttributeKeyAndValueUnionTypeDef

```python
# AttributeKeyAndValueUnionTypeDef definition

AttributeKeyAndValueUnionTypeDef = Union[
    AttributeKeyAndValueTypeDef,  # (1)
    AttributeKeyAndValueOutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: AttributeKeyAndValueTypeDef](./type_defs.md#attributekeyandvaluetypedef) 
2. See [:material-code-braces: AttributeKeyAndValueOutputTypeDef](./type_defs.md#attributekeyandvalueoutputtypedef) 

## AttributeNameAndValueUnionTypeDef

```python
# AttributeNameAndValueUnionTypeDef definition

AttributeNameAndValueUnionTypeDef = Union[
    AttributeNameAndValueTypeDef,  # (1)
    AttributeNameAndValueOutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: AttributeNameAndValueTypeDef](./type_defs.md#attributenameandvaluetypedef) 
2. See [:material-code-braces: AttributeNameAndValueOutputTypeDef](./type_defs.md#attributenameandvalueoutputtypedef) 

## FacetAttributeDefinitionUnionTypeDef

```python
# FacetAttributeDefinitionUnionTypeDef definition

FacetAttributeDefinitionUnionTypeDef = Union[
    FacetAttributeDefinitionTypeDef,  # (1)
    FacetAttributeDefinitionOutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: FacetAttributeDefinitionTypeDef](./type_defs.md#facetattributedefinitiontypedef) 
2. See [:material-code-braces: FacetAttributeDefinitionOutputTypeDef](./type_defs.md#facetattributedefinitionoutputtypedef) 

## TypedLinkAttributeDefinitionUnionTypeDef

```python
# TypedLinkAttributeDefinitionUnionTypeDef definition

TypedLinkAttributeDefinitionUnionTypeDef = Union[
    TypedLinkAttributeDefinitionTypeDef,  # (1)
    TypedLinkAttributeDefinitionOutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: TypedLinkAttributeDefinitionTypeDef](./type_defs.md#typedlinkattributedefinitiontypedef) 
2. See [:material-code-braces: TypedLinkAttributeDefinitionOutputTypeDef](./type_defs.md#typedlinkattributedefinitionoutputtypedef) 

## TypedLinkSpecifierUnionTypeDef

```python
# TypedLinkSpecifierUnionTypeDef definition

TypedLinkSpecifierUnionTypeDef = Union[
    TypedLinkSpecifierTypeDef,  # (1)
    TypedLinkSpecifierOutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: TypedLinkSpecifierTypeDef](./type_defs.md#typedlinkspecifiertypedef) 
2. See [:material-code-braces: TypedLinkSpecifierOutputTypeDef](./type_defs.md#typedlinkspecifieroutputtypedef) 

## FacetAttributeUnionTypeDef

```python
# FacetAttributeUnionTypeDef definition

FacetAttributeUnionTypeDef = Union[
    FacetAttributeTypeDef,  # (1)
    FacetAttributeOutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: FacetAttributeTypeDef](./type_defs.md#facetattributetypedef) 
2. See [:material-code-braces: FacetAttributeOutputTypeDef](./type_defs.md#facetattributeoutputtypedef) 



## ObjectReferenceTypeDef

```python
# ObjectReferenceTypeDef definition

class ObjectReferenceTypeDef(TypedDict):
    Selector: NotRequired[str],
```

## SchemaFacetTypeDef

```python
# SchemaFacetTypeDef definition

class SchemaFacetTypeDef(TypedDict):
    SchemaArn: NotRequired[str],
    FacetName: NotRequired[str],
```

## ApplySchemaRequestRequestTypeDef

```python
# ApplySchemaRequestRequestTypeDef definition

class ApplySchemaRequestRequestTypeDef(TypedDict):
    PublishedSchemaArn: str,
    DirectoryArn: str,
```

## ResponseMetadataTypeDef

```python
# ResponseMetadataTypeDef definition

class ResponseMetadataTypeDef(TypedDict):
    RequestId: str,
    HTTPStatusCode: int,
    HTTPHeaders: Dict[str, str],
    RetryAttempts: int,
    HostId: NotRequired[str],
```

## TypedLinkSchemaAndFacetNameTypeDef

```python
# TypedLinkSchemaAndFacetNameTypeDef definition

class TypedLinkSchemaAndFacetNameTypeDef(TypedDict):
    SchemaArn: str,
    TypedLinkName: str,
```

## AttributeKeyTypeDef

```python
# AttributeKeyTypeDef definition

class AttributeKeyTypeDef(TypedDict):
    SchemaArn: str,
    FacetName: str,
    Name: str,
```

## TypedAttributeValueOutputTypeDef

```python
# TypedAttributeValueOutputTypeDef definition

class TypedAttributeValueOutputTypeDef(TypedDict):
    StringValue: NotRequired[str],
    BinaryValue: NotRequired[bytes],
    BooleanValue: NotRequired[bool],
    NumberValue: NotRequired[str],
    DatetimeValue: NotRequired[datetime],
```

## BatchAttachObjectResponseTypeDef

```python
# BatchAttachObjectResponseTypeDef definition

class BatchAttachObjectResponseTypeDef(TypedDict):
    attachedObjectIdentifier: NotRequired[str],
```

## BatchAttachToIndexResponseTypeDef

```python
# BatchAttachToIndexResponseTypeDef definition

class BatchAttachToIndexResponseTypeDef(TypedDict):
    AttachedObjectIdentifier: NotRequired[str],
```

## BatchCreateIndexResponseTypeDef

```python
# BatchCreateIndexResponseTypeDef definition

class BatchCreateIndexResponseTypeDef(TypedDict):
    ObjectIdentifier: NotRequired[str],
```

## BatchCreateObjectResponseTypeDef

```python
# BatchCreateObjectResponseTypeDef definition

class BatchCreateObjectResponseTypeDef(TypedDict):
    ObjectIdentifier: NotRequired[str],
```

## BatchDetachFromIndexResponseTypeDef

```python
# BatchDetachFromIndexResponseTypeDef definition

class BatchDetachFromIndexResponseTypeDef(TypedDict):
    DetachedObjectIdentifier: NotRequired[str],
```

## BatchDetachObjectResponseTypeDef

```python
# BatchDetachObjectResponseTypeDef definition

class BatchDetachObjectResponseTypeDef(TypedDict):
    detachedObjectIdentifier: NotRequired[str],
```

## BatchListObjectChildrenResponseTypeDef

```python
# BatchListObjectChildrenResponseTypeDef definition

class BatchListObjectChildrenResponseTypeDef(TypedDict):
    Children: NotRequired[Dict[str, str]],
    NextToken: NotRequired[str],
```

## PathToObjectIdentifiersTypeDef

```python
# PathToObjectIdentifiersTypeDef definition

class PathToObjectIdentifiersTypeDef(TypedDict):
    Path: NotRequired[str],
    ObjectIdentifiers: NotRequired[List[str]],
```

## ObjectIdentifierAndLinkNameTupleTypeDef

```python
# ObjectIdentifierAndLinkNameTupleTypeDef definition

class ObjectIdentifierAndLinkNameTupleTypeDef(TypedDict):
    ObjectIdentifier: NotRequired[str],
    LinkName: NotRequired[str],
```

## BatchListObjectPoliciesResponseTypeDef

```python
# BatchListObjectPoliciesResponseTypeDef definition

class BatchListObjectPoliciesResponseTypeDef(TypedDict):
    AttachedPolicyIds: NotRequired[List[str]],
    NextToken: NotRequired[str],
```

## BatchListPolicyAttachmentsResponseTypeDef

```python
# BatchListPolicyAttachmentsResponseTypeDef definition

class BatchListPolicyAttachmentsResponseTypeDef(TypedDict):
    ObjectIdentifiers: NotRequired[List[str]],
    NextToken: NotRequired[str],
```

## BatchReadExceptionTypeDef

```python
# BatchReadExceptionTypeDef definition

class BatchReadExceptionTypeDef(TypedDict):
    Type: NotRequired[BatchReadExceptionTypeType],  # (1)
    Message: NotRequired[str],
```

1. See [:material-code-brackets: BatchReadExceptionTypeType](./literals.md#batchreadexceptiontypetype) 
## BatchUpdateObjectAttributesResponseTypeDef

```python
# BatchUpdateObjectAttributesResponseTypeDef definition

class BatchUpdateObjectAttributesResponseTypeDef(TypedDict):
    ObjectIdentifier: NotRequired[str],
```

## CreateDirectoryRequestRequestTypeDef

```python
# CreateDirectoryRequestRequestTypeDef definition

class CreateDirectoryRequestRequestTypeDef(TypedDict):
    Name: str,
    SchemaArn: str,
```

## CreateSchemaRequestRequestTypeDef

```python
# CreateSchemaRequestRequestTypeDef definition

class CreateSchemaRequestRequestTypeDef(TypedDict):
    Name: str,
```

## DeleteDirectoryRequestRequestTypeDef

```python
# DeleteDirectoryRequestRequestTypeDef definition

class DeleteDirectoryRequestRequestTypeDef(TypedDict):
    DirectoryArn: str,
```

## DeleteFacetRequestRequestTypeDef

```python
# DeleteFacetRequestRequestTypeDef definition

class DeleteFacetRequestRequestTypeDef(TypedDict):
    SchemaArn: str,
    Name: str,
```

## DeleteSchemaRequestRequestTypeDef

```python
# DeleteSchemaRequestRequestTypeDef definition

class DeleteSchemaRequestRequestTypeDef(TypedDict):
    SchemaArn: str,
```

## DeleteTypedLinkFacetRequestRequestTypeDef

```python
# DeleteTypedLinkFacetRequestRequestTypeDef definition

class DeleteTypedLinkFacetRequestRequestTypeDef(TypedDict):
    SchemaArn: str,
    Name: str,
```

## DirectoryTypeDef

```python
# DirectoryTypeDef definition

class DirectoryTypeDef(TypedDict):
    Name: NotRequired[str],
    DirectoryArn: NotRequired[str],
    State: NotRequired[DirectoryStateType],  # (1)
    CreationDateTime: NotRequired[datetime],
```

1. See [:material-code-brackets: DirectoryStateType](./literals.md#directorystatetype) 
## DisableDirectoryRequestRequestTypeDef

```python
# DisableDirectoryRequestRequestTypeDef definition

class DisableDirectoryRequestRequestTypeDef(TypedDict):
    DirectoryArn: str,
```

## EnableDirectoryRequestRequestTypeDef

```python
# EnableDirectoryRequestRequestTypeDef definition

class EnableDirectoryRequestRequestTypeDef(TypedDict):
    DirectoryArn: str,
```

## RuleOutputTypeDef

```python
# RuleOutputTypeDef definition

class RuleOutputTypeDef(TypedDict):
    Type: NotRequired[RuleTypeType],  # (1)
    Parameters: NotRequired[Dict[str, str]],
```

1. See [:material-code-brackets: RuleTypeType](./literals.md#ruletypetype) 
## FacetAttributeReferenceTypeDef

```python
# FacetAttributeReferenceTypeDef definition

class FacetAttributeReferenceTypeDef(TypedDict):
    TargetFacetName: str,
    TargetAttributeName: str,
```

## FacetTypeDef

```python
# FacetTypeDef definition

class FacetTypeDef(TypedDict):
    Name: NotRequired[str],
    ObjectType: NotRequired[ObjectTypeType],  # (1)
    FacetStyle: NotRequired[FacetStyleType],  # (2)
```

1. See [:material-code-brackets: ObjectTypeType](./literals.md#objecttypetype) 
2. See [:material-code-brackets: FacetStyleType](./literals.md#facetstyletype) 
## GetAppliedSchemaVersionRequestRequestTypeDef

```python
# GetAppliedSchemaVersionRequestRequestTypeDef definition

class GetAppliedSchemaVersionRequestRequestTypeDef(TypedDict):
    SchemaArn: str,
```

## GetDirectoryRequestRequestTypeDef

```python
# GetDirectoryRequestRequestTypeDef definition

class GetDirectoryRequestRequestTypeDef(TypedDict):
    DirectoryArn: str,
```

## GetFacetRequestRequestTypeDef

```python
# GetFacetRequestRequestTypeDef definition

class GetFacetRequestRequestTypeDef(TypedDict):
    SchemaArn: str,
    Name: str,
```

## GetSchemaAsJsonRequestRequestTypeDef

```python
# GetSchemaAsJsonRequestRequestTypeDef definition

class GetSchemaAsJsonRequestRequestTypeDef(TypedDict):
    SchemaArn: str,
```

## GetTypedLinkFacetInformationRequestRequestTypeDef

```python
# GetTypedLinkFacetInformationRequestRequestTypeDef definition

class GetTypedLinkFacetInformationRequestRequestTypeDef(TypedDict):
    SchemaArn: str,
    Name: str,
```

## PaginatorConfigTypeDef

```python
# PaginatorConfigTypeDef definition

class PaginatorConfigTypeDef(TypedDict):
    MaxItems: NotRequired[int],
    PageSize: NotRequired[int],
    StartingToken: NotRequired[str],
```

## ListAppliedSchemaArnsRequestRequestTypeDef

```python
# ListAppliedSchemaArnsRequestRequestTypeDef definition

class ListAppliedSchemaArnsRequestRequestTypeDef(TypedDict):
    DirectoryArn: str,
    SchemaArn: NotRequired[str],
    NextToken: NotRequired[str],
    MaxResults: NotRequired[int],
```

## ListDevelopmentSchemaArnsRequestRequestTypeDef

```python
# ListDevelopmentSchemaArnsRequestRequestTypeDef definition

class ListDevelopmentSchemaArnsRequestRequestTypeDef(TypedDict):
    NextToken: NotRequired[str],
    MaxResults: NotRequired[int],
```

## ListDirectoriesRequestRequestTypeDef

```python
# ListDirectoriesRequestRequestTypeDef definition

class ListDirectoriesRequestRequestTypeDef(TypedDict):
    NextToken: NotRequired[str],
    MaxResults: NotRequired[int],
    state: NotRequired[DirectoryStateType],  # (1)
```

1. See [:material-code-brackets: DirectoryStateType](./literals.md#directorystatetype) 
## ListFacetAttributesRequestRequestTypeDef

```python
# ListFacetAttributesRequestRequestTypeDef definition

class ListFacetAttributesRequestRequestTypeDef(TypedDict):
    SchemaArn: str,
    Name: str,
    NextToken: NotRequired[str],
    MaxResults: NotRequired[int],
```

## ListFacetNamesRequestRequestTypeDef

```python
# ListFacetNamesRequestRequestTypeDef definition

class ListFacetNamesRequestRequestTypeDef(TypedDict):
    SchemaArn: str,
    NextToken: NotRequired[str],
    MaxResults: NotRequired[int],
```

## ListManagedSchemaArnsRequestRequestTypeDef

```python
# ListManagedSchemaArnsRequestRequestTypeDef definition

class ListManagedSchemaArnsRequestRequestTypeDef(TypedDict):
    SchemaArn: NotRequired[str],
    NextToken: NotRequired[str],
    MaxResults: NotRequired[int],
```

## ListPublishedSchemaArnsRequestRequestTypeDef

```python
# ListPublishedSchemaArnsRequestRequestTypeDef definition

class ListPublishedSchemaArnsRequestRequestTypeDef(TypedDict):
    SchemaArn: NotRequired[str],
    NextToken: NotRequired[str],
    MaxResults: NotRequired[int],
```

## ListTagsForResourceRequestRequestTypeDef

```python
# ListTagsForResourceRequestRequestTypeDef definition

class ListTagsForResourceRequestRequestTypeDef(TypedDict):
    ResourceArn: str,
    NextToken: NotRequired[str],
    MaxResults: NotRequired[int],
```

## TagTypeDef

```python
# TagTypeDef definition

class TagTypeDef(TypedDict):
    Key: NotRequired[str],
    Value: NotRequired[str],
```

## ListTypedLinkFacetAttributesRequestRequestTypeDef

```python
# ListTypedLinkFacetAttributesRequestRequestTypeDef definition

class ListTypedLinkFacetAttributesRequestRequestTypeDef(TypedDict):
    SchemaArn: str,
    Name: str,
    NextToken: NotRequired[str],
    MaxResults: NotRequired[int],
```

## ListTypedLinkFacetNamesRequestRequestTypeDef

```python
# ListTypedLinkFacetNamesRequestRequestTypeDef definition

class ListTypedLinkFacetNamesRequestRequestTypeDef(TypedDict):
    SchemaArn: str,
    NextToken: NotRequired[str],
    MaxResults: NotRequired[int],
```

## PolicyAttachmentTypeDef

```python
# PolicyAttachmentTypeDef definition

class PolicyAttachmentTypeDef(TypedDict):
    PolicyId: NotRequired[str],
    ObjectIdentifier: NotRequired[str],
    PolicyType: NotRequired[str],
```

## PublishSchemaRequestRequestTypeDef

```python
# PublishSchemaRequestRequestTypeDef definition

class PublishSchemaRequestRequestTypeDef(TypedDict):
    DevelopmentSchemaArn: str,
    Version: str,
    MinorVersion: NotRequired[str],
    Name: NotRequired[str],
```

## PutSchemaFromJsonRequestRequestTypeDef

```python
# PutSchemaFromJsonRequestRequestTypeDef definition

class PutSchemaFromJsonRequestRequestTypeDef(TypedDict):
    SchemaArn: str,
    Document: str,
```

## RuleTypeDef

```python
# RuleTypeDef definition

class RuleTypeDef(TypedDict):
    Type: NotRequired[RuleTypeType],  # (1)
    Parameters: NotRequired[Mapping[str, str]],
```

1. See [:material-code-brackets: RuleTypeType](./literals.md#ruletypetype) 
## UntagResourceRequestRequestTypeDef

```python
# UntagResourceRequestRequestTypeDef definition

class UntagResourceRequestRequestTypeDef(TypedDict):
    ResourceArn: str,
    TagKeys: Sequence[str],
```

## UpdateSchemaRequestRequestTypeDef

```python
# UpdateSchemaRequestRequestTypeDef definition

class UpdateSchemaRequestRequestTypeDef(TypedDict):
    SchemaArn: str,
    Name: str,
```

## UpgradeAppliedSchemaRequestRequestTypeDef

```python
# UpgradeAppliedSchemaRequestRequestTypeDef definition

class UpgradeAppliedSchemaRequestRequestTypeDef(TypedDict):
    PublishedSchemaArn: str,
    DirectoryArn: str,
    DryRun: NotRequired[bool],
```

## UpgradePublishedSchemaRequestRequestTypeDef

```python
# UpgradePublishedSchemaRequestRequestTypeDef definition

class UpgradePublishedSchemaRequestRequestTypeDef(TypedDict):
    DevelopmentSchemaArn: str,
    PublishedSchemaArn: str,
    MinorVersion: str,
    DryRun: NotRequired[bool],
```

## AttachObjectRequestRequestTypeDef

```python
# AttachObjectRequestRequestTypeDef definition

class AttachObjectRequestRequestTypeDef(TypedDict):
    DirectoryArn: str,
    ParentReference: ObjectReferenceTypeDef,  # (1)
    ChildReference: ObjectReferenceTypeDef,  # (1)
    LinkName: str,
```

1. See [:material-code-braces: ObjectReferenceTypeDef](./type_defs.md#objectreferencetypedef) 
2. See [:material-code-braces: ObjectReferenceTypeDef](./type_defs.md#objectreferencetypedef) 
## AttachPolicyRequestRequestTypeDef

```python
# AttachPolicyRequestRequestTypeDef definition

class AttachPolicyRequestRequestTypeDef(TypedDict):
    DirectoryArn: str,
    PolicyReference: ObjectReferenceTypeDef,  # (1)
    ObjectReference: ObjectReferenceTypeDef,  # (1)
```

1. See [:material-code-braces: ObjectReferenceTypeDef](./type_defs.md#objectreferencetypedef) 
2. See [:material-code-braces: ObjectReferenceTypeDef](./type_defs.md#objectreferencetypedef) 
## AttachToIndexRequestRequestTypeDef

```python
# AttachToIndexRequestRequestTypeDef definition

class AttachToIndexRequestRequestTypeDef(TypedDict):
    DirectoryArn: str,
    IndexReference: ObjectReferenceTypeDef,  # (1)
    TargetReference: ObjectReferenceTypeDef,  # (1)
```

1. See [:material-code-braces: ObjectReferenceTypeDef](./type_defs.md#objectreferencetypedef) 
2. See [:material-code-braces: ObjectReferenceTypeDef](./type_defs.md#objectreferencetypedef) 
## BatchAttachObjectTypeDef

```python
# BatchAttachObjectTypeDef definition

class BatchAttachObjectTypeDef(TypedDict):
    ParentReference: ObjectReferenceTypeDef,  # (1)
    ChildReference: ObjectReferenceTypeDef,  # (1)
    LinkName: str,
```

1. See [:material-code-braces: ObjectReferenceTypeDef](./type_defs.md#objectreferencetypedef) 
2. See [:material-code-braces: ObjectReferenceTypeDef](./type_defs.md#objectreferencetypedef) 
## BatchAttachPolicyTypeDef

```python
# BatchAttachPolicyTypeDef definition

class BatchAttachPolicyTypeDef(TypedDict):
    PolicyReference: ObjectReferenceTypeDef,  # (1)
    ObjectReference: ObjectReferenceTypeDef,  # (1)
```

1. See [:material-code-braces: ObjectReferenceTypeDef](./type_defs.md#objectreferencetypedef) 
2. See [:material-code-braces: ObjectReferenceTypeDef](./type_defs.md#objectreferencetypedef) 
## BatchAttachToIndexTypeDef

```python
# BatchAttachToIndexTypeDef definition

class BatchAttachToIndexTypeDef(TypedDict):
    IndexReference: ObjectReferenceTypeDef,  # (1)
    TargetReference: ObjectReferenceTypeDef,  # (1)
```

1. See [:material-code-braces: ObjectReferenceTypeDef](./type_defs.md#objectreferencetypedef) 
2. See [:material-code-braces: ObjectReferenceTypeDef](./type_defs.md#objectreferencetypedef) 
## BatchDeleteObjectTypeDef

```python
# BatchDeleteObjectTypeDef definition

class BatchDeleteObjectTypeDef(TypedDict):
    ObjectReference: ObjectReferenceTypeDef,  # (1)
```

1. See [:material-code-braces: ObjectReferenceTypeDef](./type_defs.md#objectreferencetypedef) 
## BatchDetachFromIndexTypeDef

```python
# BatchDetachFromIndexTypeDef definition

class BatchDetachFromIndexTypeDef(TypedDict):
    IndexReference: ObjectReferenceTypeDef,  # (1)
    TargetReference: ObjectReferenceTypeDef,  # (1)
```

1. See [:material-code-braces: ObjectReferenceTypeDef](./type_defs.md#objectreferencetypedef) 
2. See [:material-code-braces: ObjectReferenceTypeDef](./type_defs.md#objectreferencetypedef) 
## BatchDetachObjectTypeDef

```python
# BatchDetachObjectTypeDef definition

class BatchDetachObjectTypeDef(TypedDict):
    ParentReference: ObjectReferenceTypeDef,  # (1)
    LinkName: str,
    BatchReferenceName: NotRequired[str],
```

1. See [:material-code-braces: ObjectReferenceTypeDef](./type_defs.md#objectreferencetypedef) 
## BatchDetachPolicyTypeDef

```python
# BatchDetachPolicyTypeDef definition

class BatchDetachPolicyTypeDef(TypedDict):
    PolicyReference: ObjectReferenceTypeDef,  # (1)
    ObjectReference: ObjectReferenceTypeDef,  # (1)
```

1. See [:material-code-braces: ObjectReferenceTypeDef](./type_defs.md#objectreferencetypedef) 
2. See [:material-code-braces: ObjectReferenceTypeDef](./type_defs.md#objectreferencetypedef) 
## BatchGetObjectInformationTypeDef

```python
# BatchGetObjectInformationTypeDef definition

class BatchGetObjectInformationTypeDef(TypedDict):
    ObjectReference: ObjectReferenceTypeDef,  # (1)
```

1. See [:material-code-braces: ObjectReferenceTypeDef](./type_defs.md#objectreferencetypedef) 
## BatchListAttachedIndicesTypeDef

```python
# BatchListAttachedIndicesTypeDef definition

class BatchListAttachedIndicesTypeDef(TypedDict):
    TargetReference: ObjectReferenceTypeDef,  # (1)
    NextToken: NotRequired[str],
    MaxResults: NotRequired[int],
```

1. See [:material-code-braces: ObjectReferenceTypeDef](./type_defs.md#objectreferencetypedef) 
## BatchListObjectChildrenTypeDef

```python
# BatchListObjectChildrenTypeDef definition

class BatchListObjectChildrenTypeDef(TypedDict):
    ObjectReference: ObjectReferenceTypeDef,  # (1)
    NextToken: NotRequired[str],
    MaxResults: NotRequired[int],
```

1. See [:material-code-braces: ObjectReferenceTypeDef](./type_defs.md#objectreferencetypedef) 
## BatchListObjectParentPathsTypeDef

```python
# BatchListObjectParentPathsTypeDef definition

class BatchListObjectParentPathsTypeDef(TypedDict):
    ObjectReference: ObjectReferenceTypeDef,  # (1)
    NextToken: NotRequired[str],
    MaxResults: NotRequired[int],
```

1. See [:material-code-braces: ObjectReferenceTypeDef](./type_defs.md#objectreferencetypedef) 
## BatchListObjectParentsTypeDef

```python
# BatchListObjectParentsTypeDef definition

class BatchListObjectParentsTypeDef(TypedDict):
    ObjectReference: ObjectReferenceTypeDef,  # (1)
    NextToken: NotRequired[str],
    MaxResults: NotRequired[int],
```

1. See [:material-code-braces: ObjectReferenceTypeDef](./type_defs.md#objectreferencetypedef) 
## BatchListObjectPoliciesTypeDef

```python
# BatchListObjectPoliciesTypeDef definition

class BatchListObjectPoliciesTypeDef(TypedDict):
    ObjectReference: ObjectReferenceTypeDef,  # (1)
    NextToken: NotRequired[str],
    MaxResults: NotRequired[int],
```

1. See [:material-code-braces: ObjectReferenceTypeDef](./type_defs.md#objectreferencetypedef) 
## BatchListPolicyAttachmentsTypeDef

```python
# BatchListPolicyAttachmentsTypeDef definition

class BatchListPolicyAttachmentsTypeDef(TypedDict):
    PolicyReference: ObjectReferenceTypeDef,  # (1)
    NextToken: NotRequired[str],
    MaxResults: NotRequired[int],
```

1. See [:material-code-braces: ObjectReferenceTypeDef](./type_defs.md#objectreferencetypedef) 
## BatchLookupPolicyTypeDef

```python
# BatchLookupPolicyTypeDef definition

class BatchLookupPolicyTypeDef(TypedDict):
    ObjectReference: ObjectReferenceTypeDef,  # (1)
    NextToken: NotRequired[str],
    MaxResults: NotRequired[int],
```

1. See [:material-code-braces: ObjectReferenceTypeDef](./type_defs.md#objectreferencetypedef) 
## DeleteObjectRequestRequestTypeDef

```python
# DeleteObjectRequestRequestTypeDef definition

class DeleteObjectRequestRequestTypeDef(TypedDict):
    DirectoryArn: str,
    ObjectReference: ObjectReferenceTypeDef,  # (1)
```

1. See [:material-code-braces: ObjectReferenceTypeDef](./type_defs.md#objectreferencetypedef) 
## DetachFromIndexRequestRequestTypeDef

```python
# DetachFromIndexRequestRequestTypeDef definition

class DetachFromIndexRequestRequestTypeDef(TypedDict):
    DirectoryArn: str,
    IndexReference: ObjectReferenceTypeDef,  # (1)
    TargetReference: ObjectReferenceTypeDef,  # (1)
```

1. See [:material-code-braces: ObjectReferenceTypeDef](./type_defs.md#objectreferencetypedef) 
2. See [:material-code-braces: ObjectReferenceTypeDef](./type_defs.md#objectreferencetypedef) 
## DetachObjectRequestRequestTypeDef

```python
# DetachObjectRequestRequestTypeDef definition

class DetachObjectRequestRequestTypeDef(TypedDict):
    DirectoryArn: str,
    ParentReference: ObjectReferenceTypeDef,  # (1)
    LinkName: str,
```

1. See [:material-code-braces: ObjectReferenceTypeDef](./type_defs.md#objectreferencetypedef) 
## DetachPolicyRequestRequestTypeDef

```python
# DetachPolicyRequestRequestTypeDef definition

class DetachPolicyRequestRequestTypeDef(TypedDict):
    DirectoryArn: str,
    PolicyReference: ObjectReferenceTypeDef,  # (1)
    ObjectReference: ObjectReferenceTypeDef,  # (1)
```

1. See [:material-code-braces: ObjectReferenceTypeDef](./type_defs.md#objectreferencetypedef) 
2. See [:material-code-braces: ObjectReferenceTypeDef](./type_defs.md#objectreferencetypedef) 
## GetObjectInformationRequestRequestTypeDef

```python
# GetObjectInformationRequestRequestTypeDef definition

class GetObjectInformationRequestRequestTypeDef(TypedDict):
    DirectoryArn: str,
    ObjectReference: ObjectReferenceTypeDef,  # (1)
    ConsistencyLevel: NotRequired[ConsistencyLevelType],  # (2)
```

1. See [:material-code-braces: ObjectReferenceTypeDef](./type_defs.md#objectreferencetypedef) 
2. See [:material-code-brackets: ConsistencyLevelType](./literals.md#consistencyleveltype) 
## ListAttachedIndicesRequestRequestTypeDef

```python
# ListAttachedIndicesRequestRequestTypeDef definition

class ListAttachedIndicesRequestRequestTypeDef(TypedDict):
    DirectoryArn: str,
    TargetReference: ObjectReferenceTypeDef,  # (1)
    NextToken: NotRequired[str],
    MaxResults: NotRequired[int],
    ConsistencyLevel: NotRequired[ConsistencyLevelType],  # (2)
```

1. See [:material-code-braces: ObjectReferenceTypeDef](./type_defs.md#objectreferencetypedef) 
2. See [:material-code-brackets: ConsistencyLevelType](./literals.md#consistencyleveltype) 
## ListObjectChildrenRequestRequestTypeDef

```python
# ListObjectChildrenRequestRequestTypeDef definition

class ListObjectChildrenRequestRequestTypeDef(TypedDict):
    DirectoryArn: str,
    ObjectReference: ObjectReferenceTypeDef,  # (1)
    NextToken: NotRequired[str],
    MaxResults: NotRequired[int],
    ConsistencyLevel: NotRequired[ConsistencyLevelType],  # (2)
```

1. See [:material-code-braces: ObjectReferenceTypeDef](./type_defs.md#objectreferencetypedef) 
2. See [:material-code-brackets: ConsistencyLevelType](./literals.md#consistencyleveltype) 
## ListObjectParentPathsRequestRequestTypeDef

```python
# ListObjectParentPathsRequestRequestTypeDef definition

class ListObjectParentPathsRequestRequestTypeDef(TypedDict):
    DirectoryArn: str,
    ObjectReference: ObjectReferenceTypeDef,  # (1)
    NextToken: NotRequired[str],
    MaxResults: NotRequired[int],
```

1. See [:material-code-braces: ObjectReferenceTypeDef](./type_defs.md#objectreferencetypedef) 
## ListObjectParentsRequestRequestTypeDef

```python
# ListObjectParentsRequestRequestTypeDef definition

class ListObjectParentsRequestRequestTypeDef(TypedDict):
    DirectoryArn: str,
    ObjectReference: ObjectReferenceTypeDef,  # (1)
    NextToken: NotRequired[str],
    MaxResults: NotRequired[int],
    ConsistencyLevel: NotRequired[ConsistencyLevelType],  # (2)
    IncludeAllLinksToEachParent: NotRequired[bool],
```

1. See [:material-code-braces: ObjectReferenceTypeDef](./type_defs.md#objectreferencetypedef) 
2. See [:material-code-brackets: ConsistencyLevelType](./literals.md#consistencyleveltype) 
## ListObjectPoliciesRequestRequestTypeDef

```python
# ListObjectPoliciesRequestRequestTypeDef definition

class ListObjectPoliciesRequestRequestTypeDef(TypedDict):
    DirectoryArn: str,
    ObjectReference: ObjectReferenceTypeDef,  # (1)
    NextToken: NotRequired[str],
    MaxResults: NotRequired[int],
    ConsistencyLevel: NotRequired[ConsistencyLevelType],  # (2)
```

1. See [:material-code-braces: ObjectReferenceTypeDef](./type_defs.md#objectreferencetypedef) 
2. See [:material-code-brackets: ConsistencyLevelType](./literals.md#consistencyleveltype) 
## ListPolicyAttachmentsRequestRequestTypeDef

```python
# ListPolicyAttachmentsRequestRequestTypeDef definition

class ListPolicyAttachmentsRequestRequestTypeDef(TypedDict):
    DirectoryArn: str,
    PolicyReference: ObjectReferenceTypeDef,  # (1)
    NextToken: NotRequired[str],
    MaxResults: NotRequired[int],
    ConsistencyLevel: NotRequired[ConsistencyLevelType],  # (2)
```

1. See [:material-code-braces: ObjectReferenceTypeDef](./type_defs.md#objectreferencetypedef) 
2. See [:material-code-brackets: ConsistencyLevelType](./literals.md#consistencyleveltype) 
## LookupPolicyRequestRequestTypeDef

```python
# LookupPolicyRequestRequestTypeDef definition

class LookupPolicyRequestRequestTypeDef(TypedDict):
    DirectoryArn: str,
    ObjectReference: ObjectReferenceTypeDef,  # (1)
    NextToken: NotRequired[str],
    MaxResults: NotRequired[int],
```

1. See [:material-code-braces: ObjectReferenceTypeDef](./type_defs.md#objectreferencetypedef) 
## BatchGetObjectAttributesTypeDef

```python
# BatchGetObjectAttributesTypeDef definition

class BatchGetObjectAttributesTypeDef(TypedDict):
    ObjectReference: ObjectReferenceTypeDef,  # (1)
    SchemaFacet: SchemaFacetTypeDef,  # (2)
    AttributeNames: Sequence[str],
```

1. See [:material-code-braces: ObjectReferenceTypeDef](./type_defs.md#objectreferencetypedef) 
2. See [:material-code-braces: SchemaFacetTypeDef](./type_defs.md#schemafacettypedef) 
## BatchGetObjectInformationResponseTypeDef

```python
# BatchGetObjectInformationResponseTypeDef definition

class BatchGetObjectInformationResponseTypeDef(TypedDict):
    SchemaFacets: NotRequired[List[SchemaFacetTypeDef]],  # (1)
    ObjectIdentifier: NotRequired[str],
```

1. See [:material-code-braces: SchemaFacetTypeDef](./type_defs.md#schemafacettypedef) 
## BatchListObjectAttributesTypeDef

```python
# BatchListObjectAttributesTypeDef definition

class BatchListObjectAttributesTypeDef(TypedDict):
    ObjectReference: ObjectReferenceTypeDef,  # (1)
    NextToken: NotRequired[str],
    MaxResults: NotRequired[int],
    FacetFilter: NotRequired[SchemaFacetTypeDef],  # (2)
```

1. See [:material-code-braces: ObjectReferenceTypeDef](./type_defs.md#objectreferencetypedef) 
2. See [:material-code-braces: SchemaFacetTypeDef](./type_defs.md#schemafacettypedef) 
## BatchRemoveFacetFromObjectTypeDef

```python
# BatchRemoveFacetFromObjectTypeDef definition

class BatchRemoveFacetFromObjectTypeDef(TypedDict):
    SchemaFacet: SchemaFacetTypeDef,  # (1)
    ObjectReference: ObjectReferenceTypeDef,  # (2)
```

1. See [:material-code-braces: SchemaFacetTypeDef](./type_defs.md#schemafacettypedef) 
2. See [:material-code-braces: ObjectReferenceTypeDef](./type_defs.md#objectreferencetypedef) 
## GetObjectAttributesRequestRequestTypeDef

```python
# GetObjectAttributesRequestRequestTypeDef definition

class GetObjectAttributesRequestRequestTypeDef(TypedDict):
    DirectoryArn: str,
    ObjectReference: ObjectReferenceTypeDef,  # (1)
    SchemaFacet: SchemaFacetTypeDef,  # (2)
    AttributeNames: Sequence[str],
    ConsistencyLevel: NotRequired[ConsistencyLevelType],  # (3)
```

1. See [:material-code-braces: ObjectReferenceTypeDef](./type_defs.md#objectreferencetypedef) 
2. See [:material-code-braces: SchemaFacetTypeDef](./type_defs.md#schemafacettypedef) 
3. See [:material-code-brackets: ConsistencyLevelType](./literals.md#consistencyleveltype) 
## ListObjectAttributesRequestRequestTypeDef

```python
# ListObjectAttributesRequestRequestTypeDef definition

class ListObjectAttributesRequestRequestTypeDef(TypedDict):
    DirectoryArn: str,
    ObjectReference: ObjectReferenceTypeDef,  # (1)
    NextToken: NotRequired[str],
    MaxResults: NotRequired[int],
    ConsistencyLevel: NotRequired[ConsistencyLevelType],  # (2)
    FacetFilter: NotRequired[SchemaFacetTypeDef],  # (3)
```

1. See [:material-code-braces: ObjectReferenceTypeDef](./type_defs.md#objectreferencetypedef) 
2. See [:material-code-brackets: ConsistencyLevelType](./literals.md#consistencyleveltype) 
3. See [:material-code-braces: SchemaFacetTypeDef](./type_defs.md#schemafacettypedef) 
## RemoveFacetFromObjectRequestRequestTypeDef

```python
# RemoveFacetFromObjectRequestRequestTypeDef definition

class RemoveFacetFromObjectRequestRequestTypeDef(TypedDict):
    DirectoryArn: str,
    SchemaFacet: SchemaFacetTypeDef,  # (1)
    ObjectReference: ObjectReferenceTypeDef,  # (2)
```

1. See [:material-code-braces: SchemaFacetTypeDef](./type_defs.md#schemafacettypedef) 
2. See [:material-code-braces: ObjectReferenceTypeDef](./type_defs.md#objectreferencetypedef) 
## ApplySchemaResponseTypeDef

```python
# ApplySchemaResponseTypeDef definition

class ApplySchemaResponseTypeDef(TypedDict):
    AppliedSchemaArn: str,
    DirectoryArn: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## AttachObjectResponseTypeDef

```python
# AttachObjectResponseTypeDef definition

class AttachObjectResponseTypeDef(TypedDict):
    AttachedObjectIdentifier: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## AttachToIndexResponseTypeDef

```python
# AttachToIndexResponseTypeDef definition

class AttachToIndexResponseTypeDef(TypedDict):
    AttachedObjectIdentifier: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateDirectoryResponseTypeDef

```python
# CreateDirectoryResponseTypeDef definition

class CreateDirectoryResponseTypeDef(TypedDict):
    DirectoryArn: str,
    Name: str,
    ObjectIdentifier: str,
    AppliedSchemaArn: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateIndexResponseTypeDef

```python
# CreateIndexResponseTypeDef definition

class CreateIndexResponseTypeDef(TypedDict):
    ObjectIdentifier: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateObjectResponseTypeDef

```python
# CreateObjectResponseTypeDef definition

class CreateObjectResponseTypeDef(TypedDict):
    ObjectIdentifier: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateSchemaResponseTypeDef

```python
# CreateSchemaResponseTypeDef definition

class CreateSchemaResponseTypeDef(TypedDict):
    SchemaArn: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DeleteDirectoryResponseTypeDef

```python
# DeleteDirectoryResponseTypeDef definition

class DeleteDirectoryResponseTypeDef(TypedDict):
    DirectoryArn: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DeleteSchemaResponseTypeDef

```python
# DeleteSchemaResponseTypeDef definition

class DeleteSchemaResponseTypeDef(TypedDict):
    SchemaArn: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DetachFromIndexResponseTypeDef

```python
# DetachFromIndexResponseTypeDef definition

class DetachFromIndexResponseTypeDef(TypedDict):
    DetachedObjectIdentifier: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DetachObjectResponseTypeDef

```python
# DetachObjectResponseTypeDef definition

class DetachObjectResponseTypeDef(TypedDict):
    DetachedObjectIdentifier: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DisableDirectoryResponseTypeDef

```python
# DisableDirectoryResponseTypeDef definition

class DisableDirectoryResponseTypeDef(TypedDict):
    DirectoryArn: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## EmptyResponseMetadataTypeDef

```python
# EmptyResponseMetadataTypeDef definition

class EmptyResponseMetadataTypeDef(TypedDict):
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## EnableDirectoryResponseTypeDef

```python
# EnableDirectoryResponseTypeDef definition

class EnableDirectoryResponseTypeDef(TypedDict):
    DirectoryArn: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetAppliedSchemaVersionResponseTypeDef

```python
# GetAppliedSchemaVersionResponseTypeDef definition

class GetAppliedSchemaVersionResponseTypeDef(TypedDict):
    AppliedSchemaArn: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetObjectInformationResponseTypeDef

```python
# GetObjectInformationResponseTypeDef definition

class GetObjectInformationResponseTypeDef(TypedDict):
    SchemaFacets: List[SchemaFacetTypeDef],  # (1)
    ObjectIdentifier: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: SchemaFacetTypeDef](./type_defs.md#schemafacettypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetSchemaAsJsonResponseTypeDef

```python
# GetSchemaAsJsonResponseTypeDef definition

class GetSchemaAsJsonResponseTypeDef(TypedDict):
    Name: str,
    Document: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetTypedLinkFacetInformationResponseTypeDef

```python
# GetTypedLinkFacetInformationResponseTypeDef definition

class GetTypedLinkFacetInformationResponseTypeDef(TypedDict):
    IdentityAttributeOrder: List[str],
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListAppliedSchemaArnsResponseTypeDef

```python
# ListAppliedSchemaArnsResponseTypeDef definition

class ListAppliedSchemaArnsResponseTypeDef(TypedDict):
    SchemaArns: List[str],
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListDevelopmentSchemaArnsResponseTypeDef

```python
# ListDevelopmentSchemaArnsResponseTypeDef definition

class ListDevelopmentSchemaArnsResponseTypeDef(TypedDict):
    SchemaArns: List[str],
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListFacetNamesResponseTypeDef

```python
# ListFacetNamesResponseTypeDef definition

class ListFacetNamesResponseTypeDef(TypedDict):
    FacetNames: List[str],
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListManagedSchemaArnsResponseTypeDef

```python
# ListManagedSchemaArnsResponseTypeDef definition

class ListManagedSchemaArnsResponseTypeDef(TypedDict):
    SchemaArns: List[str],
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListObjectChildrenResponseTypeDef

```python
# ListObjectChildrenResponseTypeDef definition

class ListObjectChildrenResponseTypeDef(TypedDict):
    Children: Dict[str, str],
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListObjectPoliciesResponseTypeDef

```python
# ListObjectPoliciesResponseTypeDef definition

class ListObjectPoliciesResponseTypeDef(TypedDict):
    AttachedPolicyIds: List[str],
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListPolicyAttachmentsResponseTypeDef

```python
# ListPolicyAttachmentsResponseTypeDef definition

class ListPolicyAttachmentsResponseTypeDef(TypedDict):
    ObjectIdentifiers: List[str],
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListPublishedSchemaArnsResponseTypeDef

```python
# ListPublishedSchemaArnsResponseTypeDef definition

class ListPublishedSchemaArnsResponseTypeDef(TypedDict):
    SchemaArns: List[str],
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListTypedLinkFacetNamesResponseTypeDef

```python
# ListTypedLinkFacetNamesResponseTypeDef definition

class ListTypedLinkFacetNamesResponseTypeDef(TypedDict):
    FacetNames: List[str],
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## PublishSchemaResponseTypeDef

```python
# PublishSchemaResponseTypeDef definition

class PublishSchemaResponseTypeDef(TypedDict):
    PublishedSchemaArn: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## PutSchemaFromJsonResponseTypeDef

```python
# PutSchemaFromJsonResponseTypeDef definition

class PutSchemaFromJsonResponseTypeDef(TypedDict):
    Arn: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdateObjectAttributesResponseTypeDef

```python
# UpdateObjectAttributesResponseTypeDef definition

class UpdateObjectAttributesResponseTypeDef(TypedDict):
    ObjectIdentifier: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdateSchemaResponseTypeDef

```python
# UpdateSchemaResponseTypeDef definition

class UpdateSchemaResponseTypeDef(TypedDict):
    SchemaArn: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpgradeAppliedSchemaResponseTypeDef

```python
# UpgradeAppliedSchemaResponseTypeDef definition

class UpgradeAppliedSchemaResponseTypeDef(TypedDict):
    UpgradedSchemaArn: str,
    DirectoryArn: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpgradePublishedSchemaResponseTypeDef

```python
# UpgradePublishedSchemaResponseTypeDef definition

class UpgradePublishedSchemaResponseTypeDef(TypedDict):
    UpgradedSchemaArn: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## BatchCreateIndexTypeDef

```python
# BatchCreateIndexTypeDef definition

class BatchCreateIndexTypeDef(TypedDict):
    OrderedIndexedAttributeList: Sequence[AttributeKeyTypeDef],  # (1)
    IsUnique: bool,
    ParentReference: NotRequired[ObjectReferenceTypeDef],  # (2)
    LinkName: NotRequired[str],
    BatchReferenceName: NotRequired[str],
```

1. See [:material-code-braces: AttributeKeyTypeDef](./type_defs.md#attributekeytypedef) 
2. See [:material-code-braces: ObjectReferenceTypeDef](./type_defs.md#objectreferencetypedef) 
## CreateIndexRequestRequestTypeDef

```python
# CreateIndexRequestRequestTypeDef definition

class CreateIndexRequestRequestTypeDef(TypedDict):
    DirectoryArn: str,
    OrderedIndexedAttributeList: Sequence[AttributeKeyTypeDef],  # (1)
    IsUnique: bool,
    ParentReference: NotRequired[ObjectReferenceTypeDef],  # (2)
    LinkName: NotRequired[str],
```

1. See [:material-code-braces: AttributeKeyTypeDef](./type_defs.md#attributekeytypedef) 
2. See [:material-code-braces: ObjectReferenceTypeDef](./type_defs.md#objectreferencetypedef) 
## AttributeKeyAndValueOutputTypeDef

```python
# AttributeKeyAndValueOutputTypeDef definition

class AttributeKeyAndValueOutputTypeDef(TypedDict):
    Key: AttributeKeyTypeDef,  # (1)
    Value: TypedAttributeValueOutputTypeDef,  # (2)
```

1. See [:material-code-braces: AttributeKeyTypeDef](./type_defs.md#attributekeytypedef) 
2. See [:material-code-braces: TypedAttributeValueOutputTypeDef](./type_defs.md#typedattributevalueoutputtypedef) 
## AttributeNameAndValueOutputTypeDef

```python
# AttributeNameAndValueOutputTypeDef definition

class AttributeNameAndValueOutputTypeDef(TypedDict):
    AttributeName: str,
    Value: TypedAttributeValueOutputTypeDef,  # (1)
```

1. See [:material-code-braces: TypedAttributeValueOutputTypeDef](./type_defs.md#typedattributevalueoutputtypedef) 
## BatchListObjectParentPathsResponseTypeDef

```python
# BatchListObjectParentPathsResponseTypeDef definition

class BatchListObjectParentPathsResponseTypeDef(TypedDict):
    PathToObjectIdentifiersList: NotRequired[List[PathToObjectIdentifiersTypeDef]],  # (1)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: PathToObjectIdentifiersTypeDef](./type_defs.md#pathtoobjectidentifierstypedef) 
## ListObjectParentPathsResponseTypeDef

```python
# ListObjectParentPathsResponseTypeDef definition

class ListObjectParentPathsResponseTypeDef(TypedDict):
    PathToObjectIdentifiersList: List[PathToObjectIdentifiersTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: PathToObjectIdentifiersTypeDef](./type_defs.md#pathtoobjectidentifierstypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## BatchListObjectParentsResponseTypeDef

```python
# BatchListObjectParentsResponseTypeDef definition

class BatchListObjectParentsResponseTypeDef(TypedDict):
    ParentLinks: NotRequired[List[ObjectIdentifierAndLinkNameTupleTypeDef]],  # (1)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: ObjectIdentifierAndLinkNameTupleTypeDef](./type_defs.md#objectidentifierandlinknametupletypedef) 
## ListObjectParentsResponseTypeDef

```python
# ListObjectParentsResponseTypeDef definition

class ListObjectParentsResponseTypeDef(TypedDict):
    Parents: Dict[str, str],
    ParentLinks: List[ObjectIdentifierAndLinkNameTupleTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: ObjectIdentifierAndLinkNameTupleTypeDef](./type_defs.md#objectidentifierandlinknametupletypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetDirectoryResponseTypeDef

```python
# GetDirectoryResponseTypeDef definition

class GetDirectoryResponseTypeDef(TypedDict):
    Directory: DirectoryTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: DirectoryTypeDef](./type_defs.md#directorytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListDirectoriesResponseTypeDef

```python
# ListDirectoriesResponseTypeDef definition

class ListDirectoriesResponseTypeDef(TypedDict):
    Directories: List[DirectoryTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: DirectoryTypeDef](./type_defs.md#directorytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## FacetAttributeDefinitionOutputTypeDef

```python
# FacetAttributeDefinitionOutputTypeDef definition

class FacetAttributeDefinitionOutputTypeDef(TypedDict):
    Type: FacetAttributeTypeType,  # (1)
    DefaultValue: NotRequired[TypedAttributeValueOutputTypeDef],  # (2)
    IsImmutable: NotRequired[bool],
    Rules: NotRequired[Dict[str, RuleOutputTypeDef]],  # (3)
```

1. See [:material-code-brackets: FacetAttributeTypeType](./literals.md#facetattributetypetype) 
2. See [:material-code-braces: TypedAttributeValueOutputTypeDef](./type_defs.md#typedattributevalueoutputtypedef) 
3. See [:material-code-braces: RuleOutputTypeDef](./type_defs.md#ruleoutputtypedef) 
## TypedLinkAttributeDefinitionOutputTypeDef

```python
# TypedLinkAttributeDefinitionOutputTypeDef definition

class TypedLinkAttributeDefinitionOutputTypeDef(TypedDict):
    Name: str,
    Type: FacetAttributeTypeType,  # (1)
    RequiredBehavior: RequiredAttributeBehaviorType,  # (4)
    DefaultValue: NotRequired[TypedAttributeValueOutputTypeDef],  # (2)
    IsImmutable: NotRequired[bool],
    Rules: NotRequired[Dict[str, RuleOutputTypeDef]],  # (3)
```

1. See [:material-code-brackets: FacetAttributeTypeType](./literals.md#facetattributetypetype) 
2. See [:material-code-braces: TypedAttributeValueOutputTypeDef](./type_defs.md#typedattributevalueoutputtypedef) 
3. See [:material-code-braces: RuleOutputTypeDef](./type_defs.md#ruleoutputtypedef) 
4. See [:material-code-brackets: RequiredAttributeBehaviorType](./literals.md#requiredattributebehaviortype) 
## GetFacetResponseTypeDef

```python
# GetFacetResponseTypeDef definition

class GetFacetResponseTypeDef(TypedDict):
    Facet: FacetTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: FacetTypeDef](./type_defs.md#facettypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListAppliedSchemaArnsRequestPaginateTypeDef

```python
# ListAppliedSchemaArnsRequestPaginateTypeDef definition

class ListAppliedSchemaArnsRequestPaginateTypeDef(TypedDict):
    DirectoryArn: str,
    SchemaArn: NotRequired[str],
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListAttachedIndicesRequestPaginateTypeDef

```python
# ListAttachedIndicesRequestPaginateTypeDef definition

class ListAttachedIndicesRequestPaginateTypeDef(TypedDict):
    DirectoryArn: str,
    TargetReference: ObjectReferenceTypeDef,  # (1)
    ConsistencyLevel: NotRequired[ConsistencyLevelType],  # (2)
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (3)
```

1. See [:material-code-braces: ObjectReferenceTypeDef](./type_defs.md#objectreferencetypedef) 
2. See [:material-code-brackets: ConsistencyLevelType](./literals.md#consistencyleveltype) 
3. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListDevelopmentSchemaArnsRequestPaginateTypeDef

```python
# ListDevelopmentSchemaArnsRequestPaginateTypeDef definition

class ListDevelopmentSchemaArnsRequestPaginateTypeDef(TypedDict):
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListDirectoriesRequestPaginateTypeDef

```python
# ListDirectoriesRequestPaginateTypeDef definition

class ListDirectoriesRequestPaginateTypeDef(TypedDict):
    state: NotRequired[DirectoryStateType],  # (1)
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (2)
```

1. See [:material-code-brackets: DirectoryStateType](./literals.md#directorystatetype) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListFacetAttributesRequestPaginateTypeDef

```python
# ListFacetAttributesRequestPaginateTypeDef definition

class ListFacetAttributesRequestPaginateTypeDef(TypedDict):
    SchemaArn: str,
    Name: str,
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListFacetNamesRequestPaginateTypeDef

```python
# ListFacetNamesRequestPaginateTypeDef definition

class ListFacetNamesRequestPaginateTypeDef(TypedDict):
    SchemaArn: str,
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListManagedSchemaArnsRequestPaginateTypeDef

```python
# ListManagedSchemaArnsRequestPaginateTypeDef definition

class ListManagedSchemaArnsRequestPaginateTypeDef(TypedDict):
    SchemaArn: NotRequired[str],
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListObjectAttributesRequestPaginateTypeDef

```python
# ListObjectAttributesRequestPaginateTypeDef definition

class ListObjectAttributesRequestPaginateTypeDef(TypedDict):
    DirectoryArn: str,
    ObjectReference: ObjectReferenceTypeDef,  # (1)
    ConsistencyLevel: NotRequired[ConsistencyLevelType],  # (2)
    FacetFilter: NotRequired[SchemaFacetTypeDef],  # (3)
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (4)
```

1. See [:material-code-braces: ObjectReferenceTypeDef](./type_defs.md#objectreferencetypedef) 
2. See [:material-code-brackets: ConsistencyLevelType](./literals.md#consistencyleveltype) 
3. See [:material-code-braces: SchemaFacetTypeDef](./type_defs.md#schemafacettypedef) 
4. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListObjectParentPathsRequestPaginateTypeDef

```python
# ListObjectParentPathsRequestPaginateTypeDef definition

class ListObjectParentPathsRequestPaginateTypeDef(TypedDict):
    DirectoryArn: str,
    ObjectReference: ObjectReferenceTypeDef,  # (1)
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (2)
```

1. See [:material-code-braces: ObjectReferenceTypeDef](./type_defs.md#objectreferencetypedef) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListObjectPoliciesRequestPaginateTypeDef

```python
# ListObjectPoliciesRequestPaginateTypeDef definition

class ListObjectPoliciesRequestPaginateTypeDef(TypedDict):
    DirectoryArn: str,
    ObjectReference: ObjectReferenceTypeDef,  # (1)
    ConsistencyLevel: NotRequired[ConsistencyLevelType],  # (2)
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (3)
```

1. See [:material-code-braces: ObjectReferenceTypeDef](./type_defs.md#objectreferencetypedef) 
2. See [:material-code-brackets: ConsistencyLevelType](./literals.md#consistencyleveltype) 
3. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListPolicyAttachmentsRequestPaginateTypeDef

```python
# ListPolicyAttachmentsRequestPaginateTypeDef definition

class ListPolicyAttachmentsRequestPaginateTypeDef(TypedDict):
    DirectoryArn: str,
    PolicyReference: ObjectReferenceTypeDef,  # (1)
    ConsistencyLevel: NotRequired[ConsistencyLevelType],  # (2)
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (3)
```

1. See [:material-code-braces: ObjectReferenceTypeDef](./type_defs.md#objectreferencetypedef) 
2. See [:material-code-brackets: ConsistencyLevelType](./literals.md#consistencyleveltype) 
3. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListPublishedSchemaArnsRequestPaginateTypeDef

```python
# ListPublishedSchemaArnsRequestPaginateTypeDef definition

class ListPublishedSchemaArnsRequestPaginateTypeDef(TypedDict):
    SchemaArn: NotRequired[str],
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListTagsForResourceRequestPaginateTypeDef

```python
# ListTagsForResourceRequestPaginateTypeDef definition

class ListTagsForResourceRequestPaginateTypeDef(TypedDict):
    ResourceArn: str,
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListTypedLinkFacetAttributesRequestPaginateTypeDef

```python
# ListTypedLinkFacetAttributesRequestPaginateTypeDef definition

class ListTypedLinkFacetAttributesRequestPaginateTypeDef(TypedDict):
    SchemaArn: str,
    Name: str,
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListTypedLinkFacetNamesRequestPaginateTypeDef

```python
# ListTypedLinkFacetNamesRequestPaginateTypeDef definition

class ListTypedLinkFacetNamesRequestPaginateTypeDef(TypedDict):
    SchemaArn: str,
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## LookupPolicyRequestPaginateTypeDef

```python
# LookupPolicyRequestPaginateTypeDef definition

class LookupPolicyRequestPaginateTypeDef(TypedDict):
    DirectoryArn: str,
    ObjectReference: ObjectReferenceTypeDef,  # (1)
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (2)
```

1. See [:material-code-braces: ObjectReferenceTypeDef](./type_defs.md#objectreferencetypedef) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListTagsForResourceResponseTypeDef

```python
# ListTagsForResourceResponseTypeDef definition

class ListTagsForResourceResponseTypeDef(TypedDict):
    Tags: List[TagTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## TagResourceRequestRequestTypeDef

```python
# TagResourceRequestRequestTypeDef definition

class TagResourceRequestRequestTypeDef(TypedDict):
    ResourceArn: str,
    Tags: Sequence[TagTypeDef],  # (1)
```

1. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
## PolicyToPathTypeDef

```python
# PolicyToPathTypeDef definition

class PolicyToPathTypeDef(TypedDict):
    Path: NotRequired[str],
    Policies: NotRequired[List[PolicyAttachmentTypeDef]],  # (1)
```

1. See [:material-code-braces: PolicyAttachmentTypeDef](./type_defs.md#policyattachmenttypedef) 
## TypedAttributeValueTypeDef

```python
# TypedAttributeValueTypeDef definition

class TypedAttributeValueTypeDef(TypedDict):
    StringValue: NotRequired[str],
    BinaryValue: NotRequired[BlobTypeDef],
    BooleanValue: NotRequired[bool],
    NumberValue: NotRequired[str],
    DatetimeValue: NotRequired[TimestampTypeDef],
```

## BatchGetLinkAttributesResponseTypeDef

```python
# BatchGetLinkAttributesResponseTypeDef definition

class BatchGetLinkAttributesResponseTypeDef(TypedDict):
    Attributes: NotRequired[List[AttributeKeyAndValueOutputTypeDef]],  # (1)
```

1. See [:material-code-braces: AttributeKeyAndValueOutputTypeDef](./type_defs.md#attributekeyandvalueoutputtypedef) 
## BatchGetObjectAttributesResponseTypeDef

```python
# BatchGetObjectAttributesResponseTypeDef definition

class BatchGetObjectAttributesResponseTypeDef(TypedDict):
    Attributes: NotRequired[List[AttributeKeyAndValueOutputTypeDef]],  # (1)
```

1. See [:material-code-braces: AttributeKeyAndValueOutputTypeDef](./type_defs.md#attributekeyandvalueoutputtypedef) 
## BatchListObjectAttributesResponseTypeDef

```python
# BatchListObjectAttributesResponseTypeDef definition

class BatchListObjectAttributesResponseTypeDef(TypedDict):
    Attributes: NotRequired[List[AttributeKeyAndValueOutputTypeDef]],  # (1)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: AttributeKeyAndValueOutputTypeDef](./type_defs.md#attributekeyandvalueoutputtypedef) 
## GetLinkAttributesResponseTypeDef

```python
# GetLinkAttributesResponseTypeDef definition

class GetLinkAttributesResponseTypeDef(TypedDict):
    Attributes: List[AttributeKeyAndValueOutputTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: AttributeKeyAndValueOutputTypeDef](./type_defs.md#attributekeyandvalueoutputtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetObjectAttributesResponseTypeDef

```python
# GetObjectAttributesResponseTypeDef definition

class GetObjectAttributesResponseTypeDef(TypedDict):
    Attributes: List[AttributeKeyAndValueOutputTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: AttributeKeyAndValueOutputTypeDef](./type_defs.md#attributekeyandvalueoutputtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## IndexAttachmentTypeDef

```python
# IndexAttachmentTypeDef definition

class IndexAttachmentTypeDef(TypedDict):
    IndexedAttributes: NotRequired[List[AttributeKeyAndValueOutputTypeDef]],  # (1)
    ObjectIdentifier: NotRequired[str],
```

1. See [:material-code-braces: AttributeKeyAndValueOutputTypeDef](./type_defs.md#attributekeyandvalueoutputtypedef) 
## ListObjectAttributesResponseTypeDef

```python
# ListObjectAttributesResponseTypeDef definition

class ListObjectAttributesResponseTypeDef(TypedDict):
    Attributes: List[AttributeKeyAndValueOutputTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: AttributeKeyAndValueOutputTypeDef](./type_defs.md#attributekeyandvalueoutputtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## TypedLinkSpecifierOutputTypeDef

```python
# TypedLinkSpecifierOutputTypeDef definition

class TypedLinkSpecifierOutputTypeDef(TypedDict):
    TypedLinkFacet: TypedLinkSchemaAndFacetNameTypeDef,  # (1)
    SourceObjectReference: ObjectReferenceTypeDef,  # (2)
    TargetObjectReference: ObjectReferenceTypeDef,  # (2)
    IdentityAttributeValues: List[AttributeNameAndValueOutputTypeDef],  # (4)
```

1. See [:material-code-braces: TypedLinkSchemaAndFacetNameTypeDef](./type_defs.md#typedlinkschemaandfacetnametypedef) 
2. See [:material-code-braces: ObjectReferenceTypeDef](./type_defs.md#objectreferencetypedef) 
3. See [:material-code-braces: ObjectReferenceTypeDef](./type_defs.md#objectreferencetypedef) 
4. See [:material-code-braces: AttributeNameAndValueOutputTypeDef](./type_defs.md#attributenameandvalueoutputtypedef) 
## FacetAttributeOutputTypeDef

```python
# FacetAttributeOutputTypeDef definition

class FacetAttributeOutputTypeDef(TypedDict):
    Name: str,
    AttributeDefinition: NotRequired[FacetAttributeDefinitionOutputTypeDef],  # (1)
    AttributeReference: NotRequired[FacetAttributeReferenceTypeDef],  # (2)
    RequiredBehavior: NotRequired[RequiredAttributeBehaviorType],  # (3)
```

1. See [:material-code-braces: FacetAttributeDefinitionOutputTypeDef](./type_defs.md#facetattributedefinitionoutputtypedef) 
2. See [:material-code-braces: FacetAttributeReferenceTypeDef](./type_defs.md#facetattributereferencetypedef) 
3. See [:material-code-brackets: RequiredAttributeBehaviorType](./literals.md#requiredattributebehaviortype) 
## ListTypedLinkFacetAttributesResponseTypeDef

```python
# ListTypedLinkFacetAttributesResponseTypeDef definition

class ListTypedLinkFacetAttributesResponseTypeDef(TypedDict):
    Attributes: List[TypedLinkAttributeDefinitionOutputTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: TypedLinkAttributeDefinitionOutputTypeDef](./type_defs.md#typedlinkattributedefinitionoutputtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## BatchLookupPolicyResponseTypeDef

```python
# BatchLookupPolicyResponseTypeDef definition

class BatchLookupPolicyResponseTypeDef(TypedDict):
    PolicyToPathList: NotRequired[List[PolicyToPathTypeDef]],  # (1)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: PolicyToPathTypeDef](./type_defs.md#policytopathtypedef) 
## LookupPolicyResponseTypeDef

```python
# LookupPolicyResponseTypeDef definition

class LookupPolicyResponseTypeDef(TypedDict):
    PolicyToPathList: List[PolicyToPathTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: PolicyToPathTypeDef](./type_defs.md#policytopathtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## BatchListAttachedIndicesResponseTypeDef

```python
# BatchListAttachedIndicesResponseTypeDef definition

class BatchListAttachedIndicesResponseTypeDef(TypedDict):
    IndexAttachments: NotRequired[List[IndexAttachmentTypeDef]],  # (1)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: IndexAttachmentTypeDef](./type_defs.md#indexattachmenttypedef) 
## BatchListIndexResponseTypeDef

```python
# BatchListIndexResponseTypeDef definition

class BatchListIndexResponseTypeDef(TypedDict):
    IndexAttachments: NotRequired[List[IndexAttachmentTypeDef]],  # (1)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: IndexAttachmentTypeDef](./type_defs.md#indexattachmenttypedef) 
## ListAttachedIndicesResponseTypeDef

```python
# ListAttachedIndicesResponseTypeDef definition

class ListAttachedIndicesResponseTypeDef(TypedDict):
    IndexAttachments: List[IndexAttachmentTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: IndexAttachmentTypeDef](./type_defs.md#indexattachmenttypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListIndexResponseTypeDef

```python
# ListIndexResponseTypeDef definition

class ListIndexResponseTypeDef(TypedDict):
    IndexAttachments: List[IndexAttachmentTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: IndexAttachmentTypeDef](./type_defs.md#indexattachmenttypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## AttachTypedLinkResponseTypeDef

```python
# AttachTypedLinkResponseTypeDef definition

class AttachTypedLinkResponseTypeDef(TypedDict):
    TypedLinkSpecifier: TypedLinkSpecifierOutputTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: TypedLinkSpecifierOutputTypeDef](./type_defs.md#typedlinkspecifieroutputtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## BatchAttachTypedLinkResponseTypeDef

```python
# BatchAttachTypedLinkResponseTypeDef definition

class BatchAttachTypedLinkResponseTypeDef(TypedDict):
    TypedLinkSpecifier: NotRequired[TypedLinkSpecifierOutputTypeDef],  # (1)
```

1. See [:material-code-braces: TypedLinkSpecifierOutputTypeDef](./type_defs.md#typedlinkspecifieroutputtypedef) 
## BatchListIncomingTypedLinksResponseTypeDef

```python
# BatchListIncomingTypedLinksResponseTypeDef definition

class BatchListIncomingTypedLinksResponseTypeDef(TypedDict):
    LinkSpecifiers: NotRequired[List[TypedLinkSpecifierOutputTypeDef]],  # (1)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: TypedLinkSpecifierOutputTypeDef](./type_defs.md#typedlinkspecifieroutputtypedef) 
## BatchListOutgoingTypedLinksResponseTypeDef

```python
# BatchListOutgoingTypedLinksResponseTypeDef definition

class BatchListOutgoingTypedLinksResponseTypeDef(TypedDict):
    TypedLinkSpecifiers: NotRequired[List[TypedLinkSpecifierOutputTypeDef]],  # (1)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: TypedLinkSpecifierOutputTypeDef](./type_defs.md#typedlinkspecifieroutputtypedef) 
## ListIncomingTypedLinksResponseTypeDef

```python
# ListIncomingTypedLinksResponseTypeDef definition

class ListIncomingTypedLinksResponseTypeDef(TypedDict):
    LinkSpecifiers: List[TypedLinkSpecifierOutputTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: TypedLinkSpecifierOutputTypeDef](./type_defs.md#typedlinkspecifieroutputtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListOutgoingTypedLinksResponseTypeDef

```python
# ListOutgoingTypedLinksResponseTypeDef definition

class ListOutgoingTypedLinksResponseTypeDef(TypedDict):
    TypedLinkSpecifiers: List[TypedLinkSpecifierOutputTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: TypedLinkSpecifierOutputTypeDef](./type_defs.md#typedlinkspecifieroutputtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListFacetAttributesResponseTypeDef

```python
# ListFacetAttributesResponseTypeDef definition

class ListFacetAttributesResponseTypeDef(TypedDict):
    Attributes: List[FacetAttributeOutputTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: FacetAttributeOutputTypeDef](./type_defs.md#facetattributeoutputtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## AttributeKeyAndValueTypeDef

```python
# AttributeKeyAndValueTypeDef definition

class AttributeKeyAndValueTypeDef(TypedDict):
    Key: AttributeKeyTypeDef,  # (1)
    Value: TypedAttributeValueUnionTypeDef,  # (2)
```

1. See [:material-code-braces: AttributeKeyTypeDef](./type_defs.md#attributekeytypedef) 
2. See [:material-code-braces: TypedAttributeValueTypeDef](./type_defs.md#typedattributevaluetypedef) [:material-code-braces: TypedAttributeValueOutputTypeDef](./type_defs.md#typedattributevalueoutputtypedef) 
## AttributeNameAndValueTypeDef

```python
# AttributeNameAndValueTypeDef definition

class AttributeNameAndValueTypeDef(TypedDict):
    AttributeName: str,
    Value: TypedAttributeValueUnionTypeDef,  # (1)
```

1. See [:material-code-braces: TypedAttributeValueTypeDef](./type_defs.md#typedattributevaluetypedef) [:material-code-braces: TypedAttributeValueOutputTypeDef](./type_defs.md#typedattributevalueoutputtypedef) 
## FacetAttributeDefinitionTypeDef

```python
# FacetAttributeDefinitionTypeDef definition

class FacetAttributeDefinitionTypeDef(TypedDict):
    Type: FacetAttributeTypeType,  # (1)
    DefaultValue: NotRequired[TypedAttributeValueUnionTypeDef],  # (2)
    IsImmutable: NotRequired[bool],
    Rules: NotRequired[Mapping[str, RuleUnionTypeDef]],  # (3)
```

1. See [:material-code-brackets: FacetAttributeTypeType](./literals.md#facetattributetypetype) 
2. See [:material-code-braces: TypedAttributeValueTypeDef](./type_defs.md#typedattributevaluetypedef) [:material-code-braces: TypedAttributeValueOutputTypeDef](./type_defs.md#typedattributevalueoutputtypedef) 
3. See [:material-code-braces: RuleTypeDef](./type_defs.md#ruletypedef) [:material-code-braces: RuleOutputTypeDef](./type_defs.md#ruleoutputtypedef) 
## LinkAttributeActionTypeDef

```python
# LinkAttributeActionTypeDef definition

class LinkAttributeActionTypeDef(TypedDict):
    AttributeActionType: NotRequired[UpdateActionTypeType],  # (1)
    AttributeUpdateValue: NotRequired[TypedAttributeValueUnionTypeDef],  # (2)
```

1. See [:material-code-brackets: UpdateActionTypeType](./literals.md#updateactiontypetype) 
2. See [:material-code-braces: TypedAttributeValueTypeDef](./type_defs.md#typedattributevaluetypedef) [:material-code-braces: TypedAttributeValueOutputTypeDef](./type_defs.md#typedattributevalueoutputtypedef) 
## ObjectAttributeActionTypeDef

```python
# ObjectAttributeActionTypeDef definition

class ObjectAttributeActionTypeDef(TypedDict):
    ObjectAttributeActionType: NotRequired[UpdateActionTypeType],  # (1)
    ObjectAttributeUpdateValue: NotRequired[TypedAttributeValueUnionTypeDef],  # (2)
```

1. See [:material-code-brackets: UpdateActionTypeType](./literals.md#updateactiontypetype) 
2. See [:material-code-braces: TypedAttributeValueTypeDef](./type_defs.md#typedattributevaluetypedef) [:material-code-braces: TypedAttributeValueOutputTypeDef](./type_defs.md#typedattributevalueoutputtypedef) 
## TypedAttributeValueRangeTypeDef

```python
# TypedAttributeValueRangeTypeDef definition

class TypedAttributeValueRangeTypeDef(TypedDict):
    StartMode: RangeModeType,  # (1)
    EndMode: RangeModeType,  # (1)
    StartValue: NotRequired[TypedAttributeValueUnionTypeDef],  # (2)
    EndValue: NotRequired[TypedAttributeValueUnionTypeDef],  # (2)
```

1. See [:material-code-brackets: RangeModeType](./literals.md#rangemodetype) 
2. See [:material-code-braces: TypedAttributeValueTypeDef](./type_defs.md#typedattributevaluetypedef) [:material-code-braces: TypedAttributeValueOutputTypeDef](./type_defs.md#typedattributevalueoutputtypedef) 
3. See [:material-code-brackets: RangeModeType](./literals.md#rangemodetype) 
4. See [:material-code-braces: TypedAttributeValueTypeDef](./type_defs.md#typedattributevaluetypedef) [:material-code-braces: TypedAttributeValueOutputTypeDef](./type_defs.md#typedattributevalueoutputtypedef) 
## TypedLinkAttributeDefinitionTypeDef

```python
# TypedLinkAttributeDefinitionTypeDef definition

class TypedLinkAttributeDefinitionTypeDef(TypedDict):
    Name: str,
    Type: FacetAttributeTypeType,  # (1)
    RequiredBehavior: RequiredAttributeBehaviorType,  # (4)
    DefaultValue: NotRequired[TypedAttributeValueUnionTypeDef],  # (2)
    IsImmutable: NotRequired[bool],
    Rules: NotRequired[Mapping[str, RuleUnionTypeDef]],  # (3)
```

1. See [:material-code-brackets: FacetAttributeTypeType](./literals.md#facetattributetypetype) 
2. See [:material-code-braces: TypedAttributeValueTypeDef](./type_defs.md#typedattributevaluetypedef) [:material-code-braces: TypedAttributeValueOutputTypeDef](./type_defs.md#typedattributevalueoutputtypedef) 
3. See [:material-code-braces: RuleTypeDef](./type_defs.md#ruletypedef) [:material-code-braces: RuleOutputTypeDef](./type_defs.md#ruleoutputtypedef) 
4. See [:material-code-brackets: RequiredAttributeBehaviorType](./literals.md#requiredattributebehaviortype) 
## BatchWriteOperationResponseTypeDef

```python
# BatchWriteOperationResponseTypeDef definition

class BatchWriteOperationResponseTypeDef(TypedDict):
    CreateObject: NotRequired[BatchCreateObjectResponseTypeDef],  # (1)
    AttachObject: NotRequired[BatchAttachObjectResponseTypeDef],  # (2)
    DetachObject: NotRequired[BatchDetachObjectResponseTypeDef],  # (3)
    UpdateObjectAttributes: NotRequired[BatchUpdateObjectAttributesResponseTypeDef],  # (4)
    DeleteObject: NotRequired[Dict[str, Any]],
    AddFacetToObject: NotRequired[Dict[str, Any]],
    RemoveFacetFromObject: NotRequired[Dict[str, Any]],
    AttachPolicy: NotRequired[Dict[str, Any]],
    DetachPolicy: NotRequired[Dict[str, Any]],
    CreateIndex: NotRequired[BatchCreateIndexResponseTypeDef],  # (5)
    AttachToIndex: NotRequired[BatchAttachToIndexResponseTypeDef],  # (6)
    DetachFromIndex: NotRequired[BatchDetachFromIndexResponseTypeDef],  # (7)
    AttachTypedLink: NotRequired[BatchAttachTypedLinkResponseTypeDef],  # (8)
    DetachTypedLink: NotRequired[Dict[str, Any]],
    UpdateLinkAttributes: NotRequired[Dict[str, Any]],
```

1. See [:material-code-braces: BatchCreateObjectResponseTypeDef](./type_defs.md#batchcreateobjectresponsetypedef) 
2. See [:material-code-braces: BatchAttachObjectResponseTypeDef](./type_defs.md#batchattachobjectresponsetypedef) 
3. See [:material-code-braces: BatchDetachObjectResponseTypeDef](./type_defs.md#batchdetachobjectresponsetypedef) 
4. See [:material-code-braces: BatchUpdateObjectAttributesResponseTypeDef](./type_defs.md#batchupdateobjectattributesresponsetypedef) 
5. See [:material-code-braces: BatchCreateIndexResponseTypeDef](./type_defs.md#batchcreateindexresponsetypedef) 
6. See [:material-code-braces: BatchAttachToIndexResponseTypeDef](./type_defs.md#batchattachtoindexresponsetypedef) 
7. See [:material-code-braces: BatchDetachFromIndexResponseTypeDef](./type_defs.md#batchdetachfromindexresponsetypedef) 
8. See [:material-code-braces: BatchAttachTypedLinkResponseTypeDef](./type_defs.md#batchattachtypedlinkresponsetypedef) 
## BatchReadSuccessfulResponseTypeDef

```python
# BatchReadSuccessfulResponseTypeDef definition

class BatchReadSuccessfulResponseTypeDef(TypedDict):
    ListObjectAttributes: NotRequired[BatchListObjectAttributesResponseTypeDef],  # (1)
    ListObjectChildren: NotRequired[BatchListObjectChildrenResponseTypeDef],  # (2)
    GetObjectInformation: NotRequired[BatchGetObjectInformationResponseTypeDef],  # (3)
    GetObjectAttributes: NotRequired[BatchGetObjectAttributesResponseTypeDef],  # (4)
    ListAttachedIndices: NotRequired[BatchListAttachedIndicesResponseTypeDef],  # (5)
    ListObjectParentPaths: NotRequired[BatchListObjectParentPathsResponseTypeDef],  # (6)
    ListObjectPolicies: NotRequired[BatchListObjectPoliciesResponseTypeDef],  # (7)
    ListPolicyAttachments: NotRequired[BatchListPolicyAttachmentsResponseTypeDef],  # (8)
    LookupPolicy: NotRequired[BatchLookupPolicyResponseTypeDef],  # (9)
    ListIndex: NotRequired[BatchListIndexResponseTypeDef],  # (10)
    ListOutgoingTypedLinks: NotRequired[BatchListOutgoingTypedLinksResponseTypeDef],  # (11)
    ListIncomingTypedLinks: NotRequired[BatchListIncomingTypedLinksResponseTypeDef],  # (12)
    GetLinkAttributes: NotRequired[BatchGetLinkAttributesResponseTypeDef],  # (13)
    ListObjectParents: NotRequired[BatchListObjectParentsResponseTypeDef],  # (14)
```

1. See [:material-code-braces: BatchListObjectAttributesResponseTypeDef](./type_defs.md#batchlistobjectattributesresponsetypedef) 
2. See [:material-code-braces: BatchListObjectChildrenResponseTypeDef](./type_defs.md#batchlistobjectchildrenresponsetypedef) 
3. See [:material-code-braces: BatchGetObjectInformationResponseTypeDef](./type_defs.md#batchgetobjectinformationresponsetypedef) 
4. See [:material-code-braces: BatchGetObjectAttributesResponseTypeDef](./type_defs.md#batchgetobjectattributesresponsetypedef) 
5. See [:material-code-braces: BatchListAttachedIndicesResponseTypeDef](./type_defs.md#batchlistattachedindicesresponsetypedef) 
6. See [:material-code-braces: BatchListObjectParentPathsResponseTypeDef](./type_defs.md#batchlistobjectparentpathsresponsetypedef) 
7. See [:material-code-braces: BatchListObjectPoliciesResponseTypeDef](./type_defs.md#batchlistobjectpoliciesresponsetypedef) 
8. See [:material-code-braces: BatchListPolicyAttachmentsResponseTypeDef](./type_defs.md#batchlistpolicyattachmentsresponsetypedef) 
9. See [:material-code-braces: BatchLookupPolicyResponseTypeDef](./type_defs.md#batchlookuppolicyresponsetypedef) 
10. See [:material-code-braces: BatchListIndexResponseTypeDef](./type_defs.md#batchlistindexresponsetypedef) 
11. See [:material-code-braces: BatchListOutgoingTypedLinksResponseTypeDef](./type_defs.md#batchlistoutgoingtypedlinksresponsetypedef) 
12. See [:material-code-braces: BatchListIncomingTypedLinksResponseTypeDef](./type_defs.md#batchlistincomingtypedlinksresponsetypedef) 
13. See [:material-code-braces: BatchGetLinkAttributesResponseTypeDef](./type_defs.md#batchgetlinkattributesresponsetypedef) 
14. See [:material-code-braces: BatchListObjectParentsResponseTypeDef](./type_defs.md#batchlistobjectparentsresponsetypedef) 
## BatchCreateObjectTypeDef

```python
# BatchCreateObjectTypeDef definition

class BatchCreateObjectTypeDef(TypedDict):
    SchemaFacet: Sequence[SchemaFacetTypeDef],  # (1)
    ObjectAttributeList: Sequence[AttributeKeyAndValueTypeDef],  # (2)
    ParentReference: NotRequired[ObjectReferenceTypeDef],  # (3)
    LinkName: NotRequired[str],
    BatchReferenceName: NotRequired[str],
```

1. See [:material-code-braces: SchemaFacetTypeDef](./type_defs.md#schemafacettypedef) 
2. See [:material-code-braces: AttributeKeyAndValueTypeDef](./type_defs.md#attributekeyandvaluetypedef) 
3. See [:material-code-braces: ObjectReferenceTypeDef](./type_defs.md#objectreferencetypedef) 
## CreateObjectRequestRequestTypeDef

```python
# CreateObjectRequestRequestTypeDef definition

class CreateObjectRequestRequestTypeDef(TypedDict):
    DirectoryArn: str,
    SchemaFacets: Sequence[SchemaFacetTypeDef],  # (1)
    ObjectAttributeList: NotRequired[Sequence[AttributeKeyAndValueTypeDef]],  # (2)
    ParentReference: NotRequired[ObjectReferenceTypeDef],  # (3)
    LinkName: NotRequired[str],
```

1. See [:material-code-braces: SchemaFacetTypeDef](./type_defs.md#schemafacettypedef) 
2. See [:material-code-braces: AttributeKeyAndValueTypeDef](./type_defs.md#attributekeyandvaluetypedef) 
3. See [:material-code-braces: ObjectReferenceTypeDef](./type_defs.md#objectreferencetypedef) 
## LinkAttributeUpdateTypeDef

```python
# LinkAttributeUpdateTypeDef definition

class LinkAttributeUpdateTypeDef(TypedDict):
    AttributeKey: NotRequired[AttributeKeyTypeDef],  # (1)
    AttributeAction: NotRequired[LinkAttributeActionTypeDef],  # (2)
```

1. See [:material-code-braces: AttributeKeyTypeDef](./type_defs.md#attributekeytypedef) 
2. See [:material-code-braces: LinkAttributeActionTypeDef](./type_defs.md#linkattributeactiontypedef) 
## ObjectAttributeUpdateTypeDef

```python
# ObjectAttributeUpdateTypeDef definition

class ObjectAttributeUpdateTypeDef(TypedDict):
    ObjectAttributeKey: NotRequired[AttributeKeyTypeDef],  # (1)
    ObjectAttributeAction: NotRequired[ObjectAttributeActionTypeDef],  # (2)
```

1. See [:material-code-braces: AttributeKeyTypeDef](./type_defs.md#attributekeytypedef) 
2. See [:material-code-braces: ObjectAttributeActionTypeDef](./type_defs.md#objectattributeactiontypedef) 
## ObjectAttributeRangeTypeDef

```python
# ObjectAttributeRangeTypeDef definition

class ObjectAttributeRangeTypeDef(TypedDict):
    AttributeKey: NotRequired[AttributeKeyTypeDef],  # (1)
    Range: NotRequired[TypedAttributeValueRangeTypeDef],  # (2)
```

1. See [:material-code-braces: AttributeKeyTypeDef](./type_defs.md#attributekeytypedef) 
2. See [:material-code-braces: TypedAttributeValueRangeTypeDef](./type_defs.md#typedattributevaluerangetypedef) 
## TypedLinkAttributeRangeTypeDef

```python
# TypedLinkAttributeRangeTypeDef definition

class TypedLinkAttributeRangeTypeDef(TypedDict):
    Range: TypedAttributeValueRangeTypeDef,  # (1)
    AttributeName: NotRequired[str],
```

1. See [:material-code-braces: TypedAttributeValueRangeTypeDef](./type_defs.md#typedattributevaluerangetypedef) 
## BatchWriteResponseTypeDef

```python
# BatchWriteResponseTypeDef definition

class BatchWriteResponseTypeDef(TypedDict):
    Responses: List[BatchWriteOperationResponseTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: BatchWriteOperationResponseTypeDef](./type_defs.md#batchwriteoperationresponsetypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## BatchReadOperationResponseTypeDef

```python
# BatchReadOperationResponseTypeDef definition

class BatchReadOperationResponseTypeDef(TypedDict):
    SuccessfulResponse: NotRequired[BatchReadSuccessfulResponseTypeDef],  # (1)
    ExceptionResponse: NotRequired[BatchReadExceptionTypeDef],  # (2)
```

1. See [:material-code-braces: BatchReadSuccessfulResponseTypeDef](./type_defs.md#batchreadsuccessfulresponsetypedef) 
2. See [:material-code-braces: BatchReadExceptionTypeDef](./type_defs.md#batchreadexceptiontypedef) 
## AddFacetToObjectRequestRequestTypeDef

```python
# AddFacetToObjectRequestRequestTypeDef definition

class AddFacetToObjectRequestRequestTypeDef(TypedDict):
    DirectoryArn: str,
    SchemaFacet: SchemaFacetTypeDef,  # (1)
    ObjectReference: ObjectReferenceTypeDef,  # (2)
    ObjectAttributeList: NotRequired[Sequence[AttributeKeyAndValueUnionTypeDef]],  # (3)
```

1. See [:material-code-braces: SchemaFacetTypeDef](./type_defs.md#schemafacettypedef) 
2. See [:material-code-braces: ObjectReferenceTypeDef](./type_defs.md#objectreferencetypedef) 
3. See [:material-code-braces: AttributeKeyAndValueTypeDef](./type_defs.md#attributekeyandvaluetypedef) [:material-code-braces: AttributeKeyAndValueOutputTypeDef](./type_defs.md#attributekeyandvalueoutputtypedef) 
## BatchAddFacetToObjectTypeDef

```python
# BatchAddFacetToObjectTypeDef definition

class BatchAddFacetToObjectTypeDef(TypedDict):
    SchemaFacet: SchemaFacetTypeDef,  # (1)
    ObjectAttributeList: Sequence[AttributeKeyAndValueUnionTypeDef],  # (2)
    ObjectReference: ObjectReferenceTypeDef,  # (3)
```

1. See [:material-code-braces: SchemaFacetTypeDef](./type_defs.md#schemafacettypedef) 
2. See [:material-code-braces: AttributeKeyAndValueTypeDef](./type_defs.md#attributekeyandvaluetypedef) [:material-code-braces: AttributeKeyAndValueOutputTypeDef](./type_defs.md#attributekeyandvalueoutputtypedef) 
3. See [:material-code-braces: ObjectReferenceTypeDef](./type_defs.md#objectreferencetypedef) 
## AttachTypedLinkRequestRequestTypeDef

```python
# AttachTypedLinkRequestRequestTypeDef definition

class AttachTypedLinkRequestRequestTypeDef(TypedDict):
    DirectoryArn: str,
    SourceObjectReference: ObjectReferenceTypeDef,  # (1)
    TargetObjectReference: ObjectReferenceTypeDef,  # (1)
    TypedLinkFacet: TypedLinkSchemaAndFacetNameTypeDef,  # (3)
    Attributes: Sequence[AttributeNameAndValueUnionTypeDef],  # (4)
```

1. See [:material-code-braces: ObjectReferenceTypeDef](./type_defs.md#objectreferencetypedef) 
2. See [:material-code-braces: ObjectReferenceTypeDef](./type_defs.md#objectreferencetypedef) 
3. See [:material-code-braces: TypedLinkSchemaAndFacetNameTypeDef](./type_defs.md#typedlinkschemaandfacetnametypedef) 
4. See [:material-code-braces: AttributeNameAndValueTypeDef](./type_defs.md#attributenameandvaluetypedef) [:material-code-braces: AttributeNameAndValueOutputTypeDef](./type_defs.md#attributenameandvalueoutputtypedef) 
## BatchAttachTypedLinkTypeDef

```python
# BatchAttachTypedLinkTypeDef definition

class BatchAttachTypedLinkTypeDef(TypedDict):
    SourceObjectReference: ObjectReferenceTypeDef,  # (1)
    TargetObjectReference: ObjectReferenceTypeDef,  # (1)
    TypedLinkFacet: TypedLinkSchemaAndFacetNameTypeDef,  # (3)
    Attributes: Sequence[AttributeNameAndValueUnionTypeDef],  # (4)
```

1. See [:material-code-braces: ObjectReferenceTypeDef](./type_defs.md#objectreferencetypedef) 
2. See [:material-code-braces: ObjectReferenceTypeDef](./type_defs.md#objectreferencetypedef) 
3. See [:material-code-braces: TypedLinkSchemaAndFacetNameTypeDef](./type_defs.md#typedlinkschemaandfacetnametypedef) 
4. See [:material-code-braces: AttributeNameAndValueTypeDef](./type_defs.md#attributenameandvaluetypedef) [:material-code-braces: AttributeNameAndValueOutputTypeDef](./type_defs.md#attributenameandvalueoutputtypedef) 
## TypedLinkSpecifierTypeDef

```python
# TypedLinkSpecifierTypeDef definition

class TypedLinkSpecifierTypeDef(TypedDict):
    TypedLinkFacet: TypedLinkSchemaAndFacetNameTypeDef,  # (1)
    SourceObjectReference: ObjectReferenceTypeDef,  # (2)
    TargetObjectReference: ObjectReferenceTypeDef,  # (2)
    IdentityAttributeValues: Sequence[AttributeNameAndValueUnionTypeDef],  # (4)
```

1. See [:material-code-braces: TypedLinkSchemaAndFacetNameTypeDef](./type_defs.md#typedlinkschemaandfacetnametypedef) 
2. See [:material-code-braces: ObjectReferenceTypeDef](./type_defs.md#objectreferencetypedef) 
3. See [:material-code-braces: ObjectReferenceTypeDef](./type_defs.md#objectreferencetypedef) 
4. See [:material-code-braces: AttributeNameAndValueTypeDef](./type_defs.md#attributenameandvaluetypedef) [:material-code-braces: AttributeNameAndValueOutputTypeDef](./type_defs.md#attributenameandvalueoutputtypedef) 
## FacetAttributeTypeDef

```python
# FacetAttributeTypeDef definition

class FacetAttributeTypeDef(TypedDict):
    Name: str,
    AttributeDefinition: NotRequired[FacetAttributeDefinitionUnionTypeDef],  # (1)
    AttributeReference: NotRequired[FacetAttributeReferenceTypeDef],  # (2)
    RequiredBehavior: NotRequired[RequiredAttributeBehaviorType],  # (3)
```

1. See [:material-code-braces: FacetAttributeDefinitionTypeDef](./type_defs.md#facetattributedefinitiontypedef) [:material-code-braces: FacetAttributeDefinitionOutputTypeDef](./type_defs.md#facetattributedefinitionoutputtypedef) 
2. See [:material-code-braces: FacetAttributeReferenceTypeDef](./type_defs.md#facetattributereferencetypedef) 
3. See [:material-code-brackets: RequiredAttributeBehaviorType](./literals.md#requiredattributebehaviortype) 
## BatchUpdateObjectAttributesTypeDef

```python
# BatchUpdateObjectAttributesTypeDef definition

class BatchUpdateObjectAttributesTypeDef(TypedDict):
    ObjectReference: ObjectReferenceTypeDef,  # (1)
    AttributeUpdates: Sequence[ObjectAttributeUpdateTypeDef],  # (2)
```

1. See [:material-code-braces: ObjectReferenceTypeDef](./type_defs.md#objectreferencetypedef) 
2. See [:material-code-braces: ObjectAttributeUpdateTypeDef](./type_defs.md#objectattributeupdatetypedef) 
## UpdateObjectAttributesRequestRequestTypeDef

```python
# UpdateObjectAttributesRequestRequestTypeDef definition

class UpdateObjectAttributesRequestRequestTypeDef(TypedDict):
    DirectoryArn: str,
    ObjectReference: ObjectReferenceTypeDef,  # (1)
    AttributeUpdates: Sequence[ObjectAttributeUpdateTypeDef],  # (2)
```

1. See [:material-code-braces: ObjectReferenceTypeDef](./type_defs.md#objectreferencetypedef) 
2. See [:material-code-braces: ObjectAttributeUpdateTypeDef](./type_defs.md#objectattributeupdatetypedef) 
## BatchListIndexTypeDef

```python
# BatchListIndexTypeDef definition

class BatchListIndexTypeDef(TypedDict):
    IndexReference: ObjectReferenceTypeDef,  # (2)
    RangesOnIndexedValues: NotRequired[Sequence[ObjectAttributeRangeTypeDef]],  # (1)
    MaxResults: NotRequired[int],
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: ObjectAttributeRangeTypeDef](./type_defs.md#objectattributerangetypedef) 
2. See [:material-code-braces: ObjectReferenceTypeDef](./type_defs.md#objectreferencetypedef) 
## ListIndexRequestPaginateTypeDef

```python
# ListIndexRequestPaginateTypeDef definition

class ListIndexRequestPaginateTypeDef(TypedDict):
    DirectoryArn: str,
    IndexReference: ObjectReferenceTypeDef,  # (1)
    RangesOnIndexedValues: NotRequired[Sequence[ObjectAttributeRangeTypeDef]],  # (2)
    ConsistencyLevel: NotRequired[ConsistencyLevelType],  # (3)
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (4)
```

1. See [:material-code-braces: ObjectReferenceTypeDef](./type_defs.md#objectreferencetypedef) 
2. See [:material-code-braces: ObjectAttributeRangeTypeDef](./type_defs.md#objectattributerangetypedef) 
3. See [:material-code-brackets: ConsistencyLevelType](./literals.md#consistencyleveltype) 
4. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListIndexRequestRequestTypeDef

```python
# ListIndexRequestRequestTypeDef definition

class ListIndexRequestRequestTypeDef(TypedDict):
    DirectoryArn: str,
    IndexReference: ObjectReferenceTypeDef,  # (1)
    RangesOnIndexedValues: NotRequired[Sequence[ObjectAttributeRangeTypeDef]],  # (2)
    MaxResults: NotRequired[int],
    NextToken: NotRequired[str],
    ConsistencyLevel: NotRequired[ConsistencyLevelType],  # (3)
```

1. See [:material-code-braces: ObjectReferenceTypeDef](./type_defs.md#objectreferencetypedef) 
2. See [:material-code-braces: ObjectAttributeRangeTypeDef](./type_defs.md#objectattributerangetypedef) 
3. See [:material-code-brackets: ConsistencyLevelType](./literals.md#consistencyleveltype) 
## BatchListIncomingTypedLinksTypeDef

```python
# BatchListIncomingTypedLinksTypeDef definition

class BatchListIncomingTypedLinksTypeDef(TypedDict):
    ObjectReference: ObjectReferenceTypeDef,  # (1)
    FilterAttributeRanges: NotRequired[Sequence[TypedLinkAttributeRangeTypeDef]],  # (2)
    FilterTypedLink: NotRequired[TypedLinkSchemaAndFacetNameTypeDef],  # (3)
    NextToken: NotRequired[str],
    MaxResults: NotRequired[int],
```

1. See [:material-code-braces: ObjectReferenceTypeDef](./type_defs.md#objectreferencetypedef) 
2. See [:material-code-braces: TypedLinkAttributeRangeTypeDef](./type_defs.md#typedlinkattributerangetypedef) 
3. See [:material-code-braces: TypedLinkSchemaAndFacetNameTypeDef](./type_defs.md#typedlinkschemaandfacetnametypedef) 
## BatchListOutgoingTypedLinksTypeDef

```python
# BatchListOutgoingTypedLinksTypeDef definition

class BatchListOutgoingTypedLinksTypeDef(TypedDict):
    ObjectReference: ObjectReferenceTypeDef,  # (1)
    FilterAttributeRanges: NotRequired[Sequence[TypedLinkAttributeRangeTypeDef]],  # (2)
    FilterTypedLink: NotRequired[TypedLinkSchemaAndFacetNameTypeDef],  # (3)
    NextToken: NotRequired[str],
    MaxResults: NotRequired[int],
```

1. See [:material-code-braces: ObjectReferenceTypeDef](./type_defs.md#objectreferencetypedef) 
2. See [:material-code-braces: TypedLinkAttributeRangeTypeDef](./type_defs.md#typedlinkattributerangetypedef) 
3. See [:material-code-braces: TypedLinkSchemaAndFacetNameTypeDef](./type_defs.md#typedlinkschemaandfacetnametypedef) 
## ListIncomingTypedLinksRequestPaginateTypeDef

```python
# ListIncomingTypedLinksRequestPaginateTypeDef definition

class ListIncomingTypedLinksRequestPaginateTypeDef(TypedDict):
    DirectoryArn: str,
    ObjectReference: ObjectReferenceTypeDef,  # (1)
    FilterAttributeRanges: NotRequired[Sequence[TypedLinkAttributeRangeTypeDef]],  # (2)
    FilterTypedLink: NotRequired[TypedLinkSchemaAndFacetNameTypeDef],  # (3)
    ConsistencyLevel: NotRequired[ConsistencyLevelType],  # (4)
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (5)
```

1. See [:material-code-braces: ObjectReferenceTypeDef](./type_defs.md#objectreferencetypedef) 
2. See [:material-code-braces: TypedLinkAttributeRangeTypeDef](./type_defs.md#typedlinkattributerangetypedef) 
3. See [:material-code-braces: TypedLinkSchemaAndFacetNameTypeDef](./type_defs.md#typedlinkschemaandfacetnametypedef) 
4. See [:material-code-brackets: ConsistencyLevelType](./literals.md#consistencyleveltype) 
5. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListIncomingTypedLinksRequestRequestTypeDef

```python
# ListIncomingTypedLinksRequestRequestTypeDef definition

class ListIncomingTypedLinksRequestRequestTypeDef(TypedDict):
    DirectoryArn: str,
    ObjectReference: ObjectReferenceTypeDef,  # (1)
    FilterAttributeRanges: NotRequired[Sequence[TypedLinkAttributeRangeTypeDef]],  # (2)
    FilterTypedLink: NotRequired[TypedLinkSchemaAndFacetNameTypeDef],  # (3)
    NextToken: NotRequired[str],
    MaxResults: NotRequired[int],
    ConsistencyLevel: NotRequired[ConsistencyLevelType],  # (4)
```

1. See [:material-code-braces: ObjectReferenceTypeDef](./type_defs.md#objectreferencetypedef) 
2. See [:material-code-braces: TypedLinkAttributeRangeTypeDef](./type_defs.md#typedlinkattributerangetypedef) 
3. See [:material-code-braces: TypedLinkSchemaAndFacetNameTypeDef](./type_defs.md#typedlinkschemaandfacetnametypedef) 
4. See [:material-code-brackets: ConsistencyLevelType](./literals.md#consistencyleveltype) 
## ListOutgoingTypedLinksRequestPaginateTypeDef

```python
# ListOutgoingTypedLinksRequestPaginateTypeDef definition

class ListOutgoingTypedLinksRequestPaginateTypeDef(TypedDict):
    DirectoryArn: str,
    ObjectReference: ObjectReferenceTypeDef,  # (1)
    FilterAttributeRanges: NotRequired[Sequence[TypedLinkAttributeRangeTypeDef]],  # (2)
    FilterTypedLink: NotRequired[TypedLinkSchemaAndFacetNameTypeDef],  # (3)
    ConsistencyLevel: NotRequired[ConsistencyLevelType],  # (4)
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (5)
```

1. See [:material-code-braces: ObjectReferenceTypeDef](./type_defs.md#objectreferencetypedef) 
2. See [:material-code-braces: TypedLinkAttributeRangeTypeDef](./type_defs.md#typedlinkattributerangetypedef) 
3. See [:material-code-braces: TypedLinkSchemaAndFacetNameTypeDef](./type_defs.md#typedlinkschemaandfacetnametypedef) 
4. See [:material-code-brackets: ConsistencyLevelType](./literals.md#consistencyleveltype) 
5. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListOutgoingTypedLinksRequestRequestTypeDef

```python
# ListOutgoingTypedLinksRequestRequestTypeDef definition

class ListOutgoingTypedLinksRequestRequestTypeDef(TypedDict):
    DirectoryArn: str,
    ObjectReference: ObjectReferenceTypeDef,  # (1)
    FilterAttributeRanges: NotRequired[Sequence[TypedLinkAttributeRangeTypeDef]],  # (2)
    FilterTypedLink: NotRequired[TypedLinkSchemaAndFacetNameTypeDef],  # (3)
    NextToken: NotRequired[str],
    MaxResults: NotRequired[int],
    ConsistencyLevel: NotRequired[ConsistencyLevelType],  # (4)
```

1. See [:material-code-braces: ObjectReferenceTypeDef](./type_defs.md#objectreferencetypedef) 
2. See [:material-code-braces: TypedLinkAttributeRangeTypeDef](./type_defs.md#typedlinkattributerangetypedef) 
3. See [:material-code-braces: TypedLinkSchemaAndFacetNameTypeDef](./type_defs.md#typedlinkschemaandfacetnametypedef) 
4. See [:material-code-brackets: ConsistencyLevelType](./literals.md#consistencyleveltype) 
## TypedLinkFacetAttributeUpdateTypeDef

```python
# TypedLinkFacetAttributeUpdateTypeDef definition

class TypedLinkFacetAttributeUpdateTypeDef(TypedDict):
    Attribute: TypedLinkAttributeDefinitionUnionTypeDef,  # (1)
    Action: UpdateActionTypeType,  # (2)
```

1. See [:material-code-braces: TypedLinkAttributeDefinitionTypeDef](./type_defs.md#typedlinkattributedefinitiontypedef) [:material-code-braces: TypedLinkAttributeDefinitionOutputTypeDef](./type_defs.md#typedlinkattributedefinitionoutputtypedef) 
2. See [:material-code-brackets: UpdateActionTypeType](./literals.md#updateactiontypetype) 
## TypedLinkFacetTypeDef

```python
# TypedLinkFacetTypeDef definition

class TypedLinkFacetTypeDef(TypedDict):
    Name: str,
    Attributes: Sequence[TypedLinkAttributeDefinitionUnionTypeDef],  # (1)
    IdentityAttributeOrder: Sequence[str],
```

1. See [:material-code-braces: TypedLinkAttributeDefinitionTypeDef](./type_defs.md#typedlinkattributedefinitiontypedef) [:material-code-braces: TypedLinkAttributeDefinitionOutputTypeDef](./type_defs.md#typedlinkattributedefinitionoutputtypedef) 
## BatchReadResponseTypeDef

```python
# BatchReadResponseTypeDef definition

class BatchReadResponseTypeDef(TypedDict):
    Responses: List[BatchReadOperationResponseTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: BatchReadOperationResponseTypeDef](./type_defs.md#batchreadoperationresponsetypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DetachTypedLinkRequestRequestTypeDef

```python
# DetachTypedLinkRequestRequestTypeDef definition

class DetachTypedLinkRequestRequestTypeDef(TypedDict):
    DirectoryArn: str,
    TypedLinkSpecifier: TypedLinkSpecifierTypeDef,  # (1)
```

1. See [:material-code-braces: TypedLinkSpecifierTypeDef](./type_defs.md#typedlinkspecifiertypedef) 
## GetLinkAttributesRequestRequestTypeDef

```python
# GetLinkAttributesRequestRequestTypeDef definition

class GetLinkAttributesRequestRequestTypeDef(TypedDict):
    DirectoryArn: str,
    TypedLinkSpecifier: TypedLinkSpecifierTypeDef,  # (1)
    AttributeNames: Sequence[str],
    ConsistencyLevel: NotRequired[ConsistencyLevelType],  # (2)
```

1. See [:material-code-braces: TypedLinkSpecifierTypeDef](./type_defs.md#typedlinkspecifiertypedef) 
2. See [:material-code-brackets: ConsistencyLevelType](./literals.md#consistencyleveltype) 
## UpdateLinkAttributesRequestRequestTypeDef

```python
# UpdateLinkAttributesRequestRequestTypeDef definition

class UpdateLinkAttributesRequestRequestTypeDef(TypedDict):
    DirectoryArn: str,
    TypedLinkSpecifier: TypedLinkSpecifierTypeDef,  # (1)
    AttributeUpdates: Sequence[LinkAttributeUpdateTypeDef],  # (2)
```

1. See [:material-code-braces: TypedLinkSpecifierTypeDef](./type_defs.md#typedlinkspecifiertypedef) 
2. See [:material-code-braces: LinkAttributeUpdateTypeDef](./type_defs.md#linkattributeupdatetypedef) 
## UpdateTypedLinkFacetRequestRequestTypeDef

```python
# UpdateTypedLinkFacetRequestRequestTypeDef definition

class UpdateTypedLinkFacetRequestRequestTypeDef(TypedDict):
    SchemaArn: str,
    Name: str,
    AttributeUpdates: Sequence[TypedLinkFacetAttributeUpdateTypeDef],  # (1)
    IdentityAttributeOrder: Sequence[str],
```

1. See [:material-code-braces: TypedLinkFacetAttributeUpdateTypeDef](./type_defs.md#typedlinkfacetattributeupdatetypedef) 
## CreateTypedLinkFacetRequestRequestTypeDef

```python
# CreateTypedLinkFacetRequestRequestTypeDef definition

class CreateTypedLinkFacetRequestRequestTypeDef(TypedDict):
    SchemaArn: str,
    Facet: TypedLinkFacetTypeDef,  # (1)
```

1. See [:material-code-braces: TypedLinkFacetTypeDef](./type_defs.md#typedlinkfacettypedef) 
## BatchDetachTypedLinkTypeDef

```python
# BatchDetachTypedLinkTypeDef definition

class BatchDetachTypedLinkTypeDef(TypedDict):
    TypedLinkSpecifier: TypedLinkSpecifierUnionTypeDef,  # (1)
```

1. See [:material-code-braces: TypedLinkSpecifierTypeDef](./type_defs.md#typedlinkspecifiertypedef) [:material-code-braces: TypedLinkSpecifierOutputTypeDef](./type_defs.md#typedlinkspecifieroutputtypedef) 
## BatchGetLinkAttributesTypeDef

```python
# BatchGetLinkAttributesTypeDef definition

class BatchGetLinkAttributesTypeDef(TypedDict):
    TypedLinkSpecifier: TypedLinkSpecifierUnionTypeDef,  # (1)
    AttributeNames: Sequence[str],
```

1. See [:material-code-braces: TypedLinkSpecifierTypeDef](./type_defs.md#typedlinkspecifiertypedef) [:material-code-braces: TypedLinkSpecifierOutputTypeDef](./type_defs.md#typedlinkspecifieroutputtypedef) 
## BatchUpdateLinkAttributesTypeDef

```python
# BatchUpdateLinkAttributesTypeDef definition

class BatchUpdateLinkAttributesTypeDef(TypedDict):
    TypedLinkSpecifier: TypedLinkSpecifierUnionTypeDef,  # (1)
    AttributeUpdates: Sequence[LinkAttributeUpdateTypeDef],  # (2)
```

1. See [:material-code-braces: TypedLinkSpecifierTypeDef](./type_defs.md#typedlinkspecifiertypedef) [:material-code-braces: TypedLinkSpecifierOutputTypeDef](./type_defs.md#typedlinkspecifieroutputtypedef) 
2. See [:material-code-braces: LinkAttributeUpdateTypeDef](./type_defs.md#linkattributeupdatetypedef) 
## CreateFacetRequestRequestTypeDef

```python
# CreateFacetRequestRequestTypeDef definition

class CreateFacetRequestRequestTypeDef(TypedDict):
    SchemaArn: str,
    Name: str,
    Attributes: NotRequired[Sequence[FacetAttributeUnionTypeDef]],  # (1)
    ObjectType: NotRequired[ObjectTypeType],  # (2)
    FacetStyle: NotRequired[FacetStyleType],  # (3)
```

1. See [:material-code-braces: FacetAttributeTypeDef](./type_defs.md#facetattributetypedef) [:material-code-braces: FacetAttributeOutputTypeDef](./type_defs.md#facetattributeoutputtypedef) 
2. See [:material-code-brackets: ObjectTypeType](./literals.md#objecttypetype) 
3. See [:material-code-brackets: FacetStyleType](./literals.md#facetstyletype) 
## FacetAttributeUpdateTypeDef

```python
# FacetAttributeUpdateTypeDef definition

class FacetAttributeUpdateTypeDef(TypedDict):
    Attribute: NotRequired[FacetAttributeUnionTypeDef],  # (1)
    Action: NotRequired[UpdateActionTypeType],  # (2)
```

1. See [:material-code-braces: FacetAttributeTypeDef](./type_defs.md#facetattributetypedef) [:material-code-braces: FacetAttributeOutputTypeDef](./type_defs.md#facetattributeoutputtypedef) 
2. See [:material-code-brackets: UpdateActionTypeType](./literals.md#updateactiontypetype) 
## BatchReadOperationTypeDef

```python
# BatchReadOperationTypeDef definition

class BatchReadOperationTypeDef(TypedDict):
    ListObjectAttributes: NotRequired[BatchListObjectAttributesTypeDef],  # (1)
    ListObjectChildren: NotRequired[BatchListObjectChildrenTypeDef],  # (2)
    ListAttachedIndices: NotRequired[BatchListAttachedIndicesTypeDef],  # (3)
    ListObjectParentPaths: NotRequired[BatchListObjectParentPathsTypeDef],  # (4)
    GetObjectInformation: NotRequired[BatchGetObjectInformationTypeDef],  # (5)
    GetObjectAttributes: NotRequired[BatchGetObjectAttributesTypeDef],  # (6)
    ListObjectParents: NotRequired[BatchListObjectParentsTypeDef],  # (7)
    ListObjectPolicies: NotRequired[BatchListObjectPoliciesTypeDef],  # (8)
    ListPolicyAttachments: NotRequired[BatchListPolicyAttachmentsTypeDef],  # (9)
    LookupPolicy: NotRequired[BatchLookupPolicyTypeDef],  # (10)
    ListIndex: NotRequired[BatchListIndexTypeDef],  # (11)
    ListOutgoingTypedLinks: NotRequired[BatchListOutgoingTypedLinksTypeDef],  # (12)
    ListIncomingTypedLinks: NotRequired[BatchListIncomingTypedLinksTypeDef],  # (13)
    GetLinkAttributes: NotRequired[BatchGetLinkAttributesTypeDef],  # (14)
```

1. See [:material-code-braces: BatchListObjectAttributesTypeDef](./type_defs.md#batchlistobjectattributestypedef) 
2. See [:material-code-braces: BatchListObjectChildrenTypeDef](./type_defs.md#batchlistobjectchildrentypedef) 
3. See [:material-code-braces: BatchListAttachedIndicesTypeDef](./type_defs.md#batchlistattachedindicestypedef) 
4. See [:material-code-braces: BatchListObjectParentPathsTypeDef](./type_defs.md#batchlistobjectparentpathstypedef) 
5. See [:material-code-braces: BatchGetObjectInformationTypeDef](./type_defs.md#batchgetobjectinformationtypedef) 
6. See [:material-code-braces: BatchGetObjectAttributesTypeDef](./type_defs.md#batchgetobjectattributestypedef) 
7. See [:material-code-braces: BatchListObjectParentsTypeDef](./type_defs.md#batchlistobjectparentstypedef) 
8. See [:material-code-braces: BatchListObjectPoliciesTypeDef](./type_defs.md#batchlistobjectpoliciestypedef) 
9. See [:material-code-braces: BatchListPolicyAttachmentsTypeDef](./type_defs.md#batchlistpolicyattachmentstypedef) 
10. See [:material-code-braces: BatchLookupPolicyTypeDef](./type_defs.md#batchlookuppolicytypedef) 
11. See [:material-code-braces: BatchListIndexTypeDef](./type_defs.md#batchlistindextypedef) 
12. See [:material-code-braces: BatchListOutgoingTypedLinksTypeDef](./type_defs.md#batchlistoutgoingtypedlinkstypedef) 
13. See [:material-code-braces: BatchListIncomingTypedLinksTypeDef](./type_defs.md#batchlistincomingtypedlinkstypedef) 
14. See [:material-code-braces: BatchGetLinkAttributesTypeDef](./type_defs.md#batchgetlinkattributestypedef) 
## BatchWriteOperationTypeDef

```python
# BatchWriteOperationTypeDef definition

class BatchWriteOperationTypeDef(TypedDict):
    CreateObject: NotRequired[BatchCreateObjectTypeDef],  # (1)
    AttachObject: NotRequired[BatchAttachObjectTypeDef],  # (2)
    DetachObject: NotRequired[BatchDetachObjectTypeDef],  # (3)
    UpdateObjectAttributes: NotRequired[BatchUpdateObjectAttributesTypeDef],  # (4)
    DeleteObject: NotRequired[BatchDeleteObjectTypeDef],  # (5)
    AddFacetToObject: NotRequired[BatchAddFacetToObjectTypeDef],  # (6)
    RemoveFacetFromObject: NotRequired[BatchRemoveFacetFromObjectTypeDef],  # (7)
    AttachPolicy: NotRequired[BatchAttachPolicyTypeDef],  # (8)
    DetachPolicy: NotRequired[BatchDetachPolicyTypeDef],  # (9)
    CreateIndex: NotRequired[BatchCreateIndexTypeDef],  # (10)
    AttachToIndex: NotRequired[BatchAttachToIndexTypeDef],  # (11)
    DetachFromIndex: NotRequired[BatchDetachFromIndexTypeDef],  # (12)
    AttachTypedLink: NotRequired[BatchAttachTypedLinkTypeDef],  # (13)
    DetachTypedLink: NotRequired[BatchDetachTypedLinkTypeDef],  # (14)
    UpdateLinkAttributes: NotRequired[BatchUpdateLinkAttributesTypeDef],  # (15)
```

1. See [:material-code-braces: BatchCreateObjectTypeDef](./type_defs.md#batchcreateobjecttypedef) 
2. See [:material-code-braces: BatchAttachObjectTypeDef](./type_defs.md#batchattachobjecttypedef) 
3. See [:material-code-braces: BatchDetachObjectTypeDef](./type_defs.md#batchdetachobjecttypedef) 
4. See [:material-code-braces: BatchUpdateObjectAttributesTypeDef](./type_defs.md#batchupdateobjectattributestypedef) 
5. See [:material-code-braces: BatchDeleteObjectTypeDef](./type_defs.md#batchdeleteobjecttypedef) 
6. See [:material-code-braces: BatchAddFacetToObjectTypeDef](./type_defs.md#batchaddfacettoobjecttypedef) 
7. See [:material-code-braces: BatchRemoveFacetFromObjectTypeDef](./type_defs.md#batchremovefacetfromobjecttypedef) 
8. See [:material-code-braces: BatchAttachPolicyTypeDef](./type_defs.md#batchattachpolicytypedef) 
9. See [:material-code-braces: BatchDetachPolicyTypeDef](./type_defs.md#batchdetachpolicytypedef) 
10. See [:material-code-braces: BatchCreateIndexTypeDef](./type_defs.md#batchcreateindextypedef) 
11. See [:material-code-braces: BatchAttachToIndexTypeDef](./type_defs.md#batchattachtoindextypedef) 
12. See [:material-code-braces: BatchDetachFromIndexTypeDef](./type_defs.md#batchdetachfromindextypedef) 
13. See [:material-code-braces: BatchAttachTypedLinkTypeDef](./type_defs.md#batchattachtypedlinktypedef) 
14. See [:material-code-braces: BatchDetachTypedLinkTypeDef](./type_defs.md#batchdetachtypedlinktypedef) 
15. See [:material-code-braces: BatchUpdateLinkAttributesTypeDef](./type_defs.md#batchupdatelinkattributestypedef) 
## UpdateFacetRequestRequestTypeDef

```python
# UpdateFacetRequestRequestTypeDef definition

class UpdateFacetRequestRequestTypeDef(TypedDict):
    SchemaArn: str,
    Name: str,
    AttributeUpdates: NotRequired[Sequence[FacetAttributeUpdateTypeDef]],  # (1)
    ObjectType: NotRequired[ObjectTypeType],  # (2)
```

1. See [:material-code-braces: FacetAttributeUpdateTypeDef](./type_defs.md#facetattributeupdatetypedef) 
2. See [:material-code-brackets: ObjectTypeType](./literals.md#objecttypetype) 
## BatchReadRequestRequestTypeDef

```python
# BatchReadRequestRequestTypeDef definition

class BatchReadRequestRequestTypeDef(TypedDict):
    DirectoryArn: str,
    Operations: Sequence[BatchReadOperationTypeDef],  # (1)
    ConsistencyLevel: NotRequired[ConsistencyLevelType],  # (2)
```

1. See [:material-code-braces: BatchReadOperationTypeDef](./type_defs.md#batchreadoperationtypedef) 
2. See [:material-code-brackets: ConsistencyLevelType](./literals.md#consistencyleveltype) 
## BatchWriteRequestRequestTypeDef

```python
# BatchWriteRequestRequestTypeDef definition

class BatchWriteRequestRequestTypeDef(TypedDict):
    DirectoryArn: str,
    Operations: Sequence[BatchWriteOperationTypeDef],  # (1)
```

1. See [:material-code-braces: BatchWriteOperationTypeDef](./type_defs.md#batchwriteoperationtypedef) 
