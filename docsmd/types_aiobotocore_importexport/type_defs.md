# Type definitions

> [Index](../README.md) > [ImportExport](./README.md) > Type definitions

!!! note ""

    Auto-generated documentation for [ImportExport](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/importexport.html#ImportExport)
    type annotations stubs module [types-aiobotocore-importexport](https://pypi.org/project/types-aiobotocore-importexport/).



## ArtifactTypeDef

```python
# ArtifactTypeDef definition

class ArtifactTypeDef(TypedDict):
    Description: NotRequired[str],
    URL: NotRequired[str],
```

## CancelJobInputRequestTypeDef

```python
# CancelJobInputRequestTypeDef definition

class CancelJobInputRequestTypeDef(TypedDict):
    JobId: str,
    APIVersion: NotRequired[str],
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

## CreateJobInputRequestTypeDef

```python
# CreateJobInputRequestTypeDef definition

class CreateJobInputRequestTypeDef(TypedDict):
    JobType: JobTypeType,  # (1)
    Manifest: str,
    ValidateOnly: bool,
    ManifestAddendum: NotRequired[str],
    APIVersion: NotRequired[str],
```

1. See [:material-code-brackets: JobTypeType](./literals.md#jobtypetype) 
## GetShippingLabelInputRequestTypeDef

```python
# GetShippingLabelInputRequestTypeDef definition

class GetShippingLabelInputRequestTypeDef(TypedDict):
    jobIds: Sequence[str],
    name: NotRequired[str],
    company: NotRequired[str],
    phoneNumber: NotRequired[str],
    country: NotRequired[str],
    stateOrProvince: NotRequired[str],
    city: NotRequired[str],
    postalCode: NotRequired[str],
    street1: NotRequired[str],
    street2: NotRequired[str],
    street3: NotRequired[str],
    APIVersion: NotRequired[str],
```

## GetStatusInputRequestTypeDef

```python
# GetStatusInputRequestTypeDef definition

class GetStatusInputRequestTypeDef(TypedDict):
    JobId: str,
    APIVersion: NotRequired[str],
```

## JobTypeDef

```python
# JobTypeDef definition

class JobTypeDef(TypedDict):
    JobId: NotRequired[str],
    CreationDate: NotRequired[datetime],
    IsCanceled: NotRequired[bool],
    JobType: NotRequired[JobTypeType],  # (1)
```

1. See [:material-code-brackets: JobTypeType](./literals.md#jobtypetype) 
## PaginatorConfigTypeDef

```python
# PaginatorConfigTypeDef definition

class PaginatorConfigTypeDef(TypedDict):
    MaxItems: NotRequired[int],
    PageSize: NotRequired[int],
    StartingToken: NotRequired[str],
```

## ListJobsInputRequestTypeDef

```python
# ListJobsInputRequestTypeDef definition

class ListJobsInputRequestTypeDef(TypedDict):
    MaxJobs: NotRequired[int],
    Marker: NotRequired[str],
    APIVersion: NotRequired[str],
```

## UpdateJobInputRequestTypeDef

```python
# UpdateJobInputRequestTypeDef definition

class UpdateJobInputRequestTypeDef(TypedDict):
    JobId: str,
    Manifest: str,
    JobType: JobTypeType,  # (1)
    ValidateOnly: bool,
    APIVersion: NotRequired[str],
```

1. See [:material-code-brackets: JobTypeType](./literals.md#jobtypetype) 
## CancelJobOutputTypeDef

```python
# CancelJobOutputTypeDef definition

class CancelJobOutputTypeDef(TypedDict):
    Success: bool,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateJobOutputTypeDef

```python
# CreateJobOutputTypeDef definition

class CreateJobOutputTypeDef(TypedDict):
    JobId: str,
    JobType: JobTypeType,  # (1)
    Signature: str,
    SignatureFileContents: str,
    WarningMessage: str,
    ArtifactList: List[ArtifactTypeDef],  # (2)
    ResponseMetadata: ResponseMetadataTypeDef,  # (3)
```

1. See [:material-code-brackets: JobTypeType](./literals.md#jobtypetype) 
2. See [:material-code-braces: ArtifactTypeDef](./type_defs.md#artifacttypedef) 
3. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetShippingLabelOutputTypeDef

```python
# GetShippingLabelOutputTypeDef definition

class GetShippingLabelOutputTypeDef(TypedDict):
    ShippingLabelURL: str,
    Warning: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetStatusOutputTypeDef

```python
# GetStatusOutputTypeDef definition

class GetStatusOutputTypeDef(TypedDict):
    JobId: str,
    JobType: JobTypeType,  # (1)
    LocationCode: str,
    LocationMessage: str,
    ProgressCode: str,
    ProgressMessage: str,
    Carrier: str,
    TrackingNumber: str,
    LogBucket: str,
    LogKey: str,
    ErrorCount: int,
    Signature: str,
    SignatureFileContents: str,
    CurrentManifest: str,
    CreationDate: datetime,
    ArtifactList: List[ArtifactTypeDef],  # (2)
    ResponseMetadata: ResponseMetadataTypeDef,  # (3)
```

1. See [:material-code-brackets: JobTypeType](./literals.md#jobtypetype) 
2. See [:material-code-braces: ArtifactTypeDef](./type_defs.md#artifacttypedef) 
3. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdateJobOutputTypeDef

```python
# UpdateJobOutputTypeDef definition

class UpdateJobOutputTypeDef(TypedDict):
    Success: bool,
    WarningMessage: str,
    ArtifactList: List[ArtifactTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ArtifactTypeDef](./type_defs.md#artifacttypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListJobsOutputTypeDef

```python
# ListJobsOutputTypeDef definition

class ListJobsOutputTypeDef(TypedDict):
    Jobs: List[JobTypeDef],  # (1)
    IsTruncated: bool,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: JobTypeDef](./type_defs.md#jobtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListJobsInputListJobsPaginateTypeDef

```python
# ListJobsInputListJobsPaginateTypeDef definition

class ListJobsInputListJobsPaginateTypeDef(TypedDict):
    APIVersion: NotRequired[str],
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
