# Type definitions

> [Index](../README.md) > [Macie](./README.md) > Type definitions

!!! note ""

    Auto-generated documentation for [Macie](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/macie.html#Macie)
    type annotations stubs module [types-aiobotocore-macie](https://pypi.org/project/types-aiobotocore-macie/).



## AssociateMemberAccountRequestRequestTypeDef

```python
# AssociateMemberAccountRequestRequestTypeDef definition

class AssociateMemberAccountRequestRequestTypeDef(TypedDict):
    memberAccountId: str,
```

## ResponseMetadataTypeDef

```python
# ResponseMetadataTypeDef definition

class ResponseMetadataTypeDef(TypedDict):
    RequestId: str,
    HostId: str,
    HTTPStatusCode: int,
    HTTPHeaders: Dict[str, str],
    RetryAttempts: int,
```

## ClassificationTypeTypeDef

```python
# ClassificationTypeTypeDef definition

class ClassificationTypeTypeDef(TypedDict):
    oneTime: S3OneTimeClassificationTypeType,  # (1)
    continuous: S3ContinuousClassificationTypeType,  # (2)
```

1. See [:material-code-brackets: S3OneTimeClassificationTypeType](./literals.md#s3onetimeclassificationtypetype) 
2. See [:material-code-brackets: S3ContinuousClassificationTypeType](./literals.md#s3continuousclassificationtypetype) 
## ClassificationTypeUpdateTypeDef

```python
# ClassificationTypeUpdateTypeDef definition

class ClassificationTypeUpdateTypeDef(TypedDict):
    oneTime: NotRequired[S3OneTimeClassificationTypeType],  # (1)
    continuous: NotRequired[S3ContinuousClassificationTypeType],  # (2)
```

1. See [:material-code-brackets: S3OneTimeClassificationTypeType](./literals.md#s3onetimeclassificationtypetype) 
2. See [:material-code-brackets: S3ContinuousClassificationTypeType](./literals.md#s3continuousclassificationtypetype) 
## DisassociateMemberAccountRequestRequestTypeDef

```python
# DisassociateMemberAccountRequestRequestTypeDef definition

class DisassociateMemberAccountRequestRequestTypeDef(TypedDict):
    memberAccountId: str,
```

## S3ResourceTypeDef

```python
# S3ResourceTypeDef definition

class S3ResourceTypeDef(TypedDict):
    bucketName: str,
    prefix: NotRequired[str],
```

## PaginatorConfigTypeDef

```python
# PaginatorConfigTypeDef definition

class PaginatorConfigTypeDef(TypedDict):
    MaxItems: NotRequired[int],
    PageSize: NotRequired[int],
    StartingToken: NotRequired[str],
```

## ListMemberAccountsRequestRequestTypeDef

```python
# ListMemberAccountsRequestRequestTypeDef definition

class ListMemberAccountsRequestRequestTypeDef(TypedDict):
    nextToken: NotRequired[str],
    maxResults: NotRequired[int],
```

## MemberAccountTypeDef

```python
# MemberAccountTypeDef definition

class MemberAccountTypeDef(TypedDict):
    accountId: NotRequired[str],
```

## ListS3ResourcesRequestRequestTypeDef

```python
# ListS3ResourcesRequestRequestTypeDef definition

class ListS3ResourcesRequestRequestTypeDef(TypedDict):
    memberAccountId: NotRequired[str],
    nextToken: NotRequired[str],
    maxResults: NotRequired[int],
```

## EmptyResponseMetadataTypeDef

```python
# EmptyResponseMetadataTypeDef definition

class EmptyResponseMetadataTypeDef(TypedDict):
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## S3ResourceClassificationTypeDef

```python
# S3ResourceClassificationTypeDef definition

class S3ResourceClassificationTypeDef(TypedDict):
    bucketName: str,
    classificationType: ClassificationTypeTypeDef,  # (1)
    prefix: NotRequired[str],
```

1. See [:material-code-braces: ClassificationTypeTypeDef](./type_defs.md#classificationtypetypedef) 
## S3ResourceClassificationUpdateTypeDef

```python
# S3ResourceClassificationUpdateTypeDef definition

class S3ResourceClassificationUpdateTypeDef(TypedDict):
    bucketName: str,
    classificationTypeUpdate: ClassificationTypeUpdateTypeDef,  # (1)
    prefix: NotRequired[str],
```

1. See [:material-code-braces: ClassificationTypeUpdateTypeDef](./type_defs.md#classificationtypeupdatetypedef) 
## DisassociateS3ResourcesRequestRequestTypeDef

```python
# DisassociateS3ResourcesRequestRequestTypeDef definition

class DisassociateS3ResourcesRequestRequestTypeDef(TypedDict):
    associatedS3Resources: Sequence[S3ResourceTypeDef],  # (1)
    memberAccountId: NotRequired[str],
```

1. See [:material-code-braces: S3ResourceTypeDef](./type_defs.md#s3resourcetypedef) 
## FailedS3ResourceTypeDef

```python
# FailedS3ResourceTypeDef definition

class FailedS3ResourceTypeDef(TypedDict):
    failedItem: NotRequired[S3ResourceTypeDef],  # (1)
    errorCode: NotRequired[str],
    errorMessage: NotRequired[str],
```

1. See [:material-code-braces: S3ResourceTypeDef](./type_defs.md#s3resourcetypedef) 
## ListMemberAccountsRequestListMemberAccountsPaginateTypeDef

```python
# ListMemberAccountsRequestListMemberAccountsPaginateTypeDef definition

class ListMemberAccountsRequestListMemberAccountsPaginateTypeDef(TypedDict):
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListS3ResourcesRequestListS3ResourcesPaginateTypeDef

```python
# ListS3ResourcesRequestListS3ResourcesPaginateTypeDef definition

class ListS3ResourcesRequestListS3ResourcesPaginateTypeDef(TypedDict):
    memberAccountId: NotRequired[str],
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListMemberAccountsResultTypeDef

```python
# ListMemberAccountsResultTypeDef definition

class ListMemberAccountsResultTypeDef(TypedDict):
    memberAccounts: List[MemberAccountTypeDef],  # (1)
    nextToken: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: MemberAccountTypeDef](./type_defs.md#memberaccounttypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## AssociateS3ResourcesRequestRequestTypeDef

```python
# AssociateS3ResourcesRequestRequestTypeDef definition

class AssociateS3ResourcesRequestRequestTypeDef(TypedDict):
    s3Resources: Sequence[S3ResourceClassificationTypeDef],  # (1)
    memberAccountId: NotRequired[str],
```

1. See [:material-code-braces: S3ResourceClassificationTypeDef](./type_defs.md#s3resourceclassificationtypedef) 
## ListS3ResourcesResultTypeDef

```python
# ListS3ResourcesResultTypeDef definition

class ListS3ResourcesResultTypeDef(TypedDict):
    s3Resources: List[S3ResourceClassificationTypeDef],  # (1)
    nextToken: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: S3ResourceClassificationTypeDef](./type_defs.md#s3resourceclassificationtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdateS3ResourcesRequestRequestTypeDef

```python
# UpdateS3ResourcesRequestRequestTypeDef definition

class UpdateS3ResourcesRequestRequestTypeDef(TypedDict):
    s3ResourcesUpdate: Sequence[S3ResourceClassificationUpdateTypeDef],  # (1)
    memberAccountId: NotRequired[str],
```

1. See [:material-code-braces: S3ResourceClassificationUpdateTypeDef](./type_defs.md#s3resourceclassificationupdatetypedef) 
## AssociateS3ResourcesResultTypeDef

```python
# AssociateS3ResourcesResultTypeDef definition

class AssociateS3ResourcesResultTypeDef(TypedDict):
    failedS3Resources: List[FailedS3ResourceTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: FailedS3ResourceTypeDef](./type_defs.md#faileds3resourcetypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DisassociateS3ResourcesResultTypeDef

```python
# DisassociateS3ResourcesResultTypeDef definition

class DisassociateS3ResourcesResultTypeDef(TypedDict):
    failedS3Resources: List[FailedS3ResourceTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: FailedS3ResourceTypeDef](./type_defs.md#faileds3resourcetypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdateS3ResourcesResultTypeDef

```python
# UpdateS3ResourcesResultTypeDef definition

class UpdateS3ResourcesResultTypeDef(TypedDict):
    failedS3Resources: List[FailedS3ResourceTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: FailedS3ResourceTypeDef](./type_defs.md#faileds3resourcetypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
