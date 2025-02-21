# Type definitions

> [Index](../README.md) > [Inspector2](./README.md) > Type definitions

!!! note ""

    Auto-generated documentation for [Inspector2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/inspector2.html#inspector2)
    type annotations stubs module [types-aiobotocore-inspector2](https://pypi.org/project/types-aiobotocore-inspector2/).

## BlobTypeDef

```python
# BlobTypeDef Union usage example

from types_aiobotocore_inspector2.type_defs import BlobTypeDef


def get_value() -> BlobTypeDef:
    return ...


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
# TimestampTypeDef Union usage example

from types_aiobotocore_inspector2.type_defs import TimestampTypeDef


def get_value() -> TimestampTypeDef:
    return ...


# TimestampTypeDef definition

TimestampTypeDef = Union[
    datetime,
    str,
]
```


## ResourceFilterCriteriaUnionTypeDef

```python
# ResourceFilterCriteriaUnionTypeDef Union usage example

from types_aiobotocore_inspector2.type_defs import ResourceFilterCriteriaUnionTypeDef


def get_value() -> ResourceFilterCriteriaUnionTypeDef:
    return ...


# ResourceFilterCriteriaUnionTypeDef definition

ResourceFilterCriteriaUnionTypeDef = Union[
    ResourceFilterCriteriaTypeDef,  # (1)
    ResourceFilterCriteriaOutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: ResourceFilterCriteriaTypeDef](./type_defs.md#resourcefiltercriteriatypedef) 
2. See [:material-code-braces: ResourceFilterCriteriaOutputTypeDef](./type_defs.md#resourcefiltercriteriaoutputtypedef) 

## ScheduleUnionTypeDef

```python
# ScheduleUnionTypeDef Union usage example

from types_aiobotocore_inspector2.type_defs import ScheduleUnionTypeDef


def get_value() -> ScheduleUnionTypeDef:
    return ...


# ScheduleUnionTypeDef definition

ScheduleUnionTypeDef = Union[
    ScheduleTypeDef,  # (1)
    ScheduleOutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: ScheduleTypeDef](./type_defs.md#scheduletypedef) 
2. See [:material-code-braces: ScheduleOutputTypeDef](./type_defs.md#scheduleoutputtypedef) 

## FilterCriteriaUnionTypeDef

```python
# FilterCriteriaUnionTypeDef Union usage example

from types_aiobotocore_inspector2.type_defs import FilterCriteriaUnionTypeDef


def get_value() -> FilterCriteriaUnionTypeDef:
    return ...


# FilterCriteriaUnionTypeDef definition

FilterCriteriaUnionTypeDef = Union[
    FilterCriteriaTypeDef,  # (1)
    FilterCriteriaOutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: FilterCriteriaTypeDef](./type_defs.md#filtercriteriatypedef) 
2. See [:material-code-braces: FilterCriteriaOutputTypeDef](./type_defs.md#filtercriteriaoutputtypedef) 



## SeverityCountsTypeDef

```python
# SeverityCountsTypeDef TypedDict usage example

from types_aiobotocore_inspector2.type_defs import SeverityCountsTypeDef


def get_value() -> SeverityCountsTypeDef:
    return {
        "all": ...,
    }


# SeverityCountsTypeDef definition

class SeverityCountsTypeDef(TypedDict):
    all: NotRequired[int],
    critical: NotRequired[int],
    high: NotRequired[int],
    medium: NotRequired[int],
```

## AccountAggregationTypeDef

```python
# AccountAggregationTypeDef TypedDict usage example

from types_aiobotocore_inspector2.type_defs import AccountAggregationTypeDef


def get_value() -> AccountAggregationTypeDef:
    return {
        "findingType": ...,
    }


# AccountAggregationTypeDef definition

class AccountAggregationTypeDef(TypedDict):
    findingType: NotRequired[AggregationFindingTypeType],  # (1)
    resourceType: NotRequired[AggregationResourceTypeType],  # (2)
    sortBy: NotRequired[AccountSortByType],  # (3)
    sortOrder: NotRequired[SortOrderType],  # (4)
```

1. See [:material-code-brackets: AggregationFindingTypeType](./literals.md#aggregationfindingtypetype) 
2. See [:material-code-brackets: AggregationResourceTypeType](./literals.md#aggregationresourcetypetype) 
3. See [:material-code-brackets: AccountSortByType](./literals.md#accountsortbytype) 
4. See [:material-code-brackets: SortOrderType](./literals.md#sortordertype) 
## StateTypeDef

```python
# StateTypeDef TypedDict usage example

from types_aiobotocore_inspector2.type_defs import StateTypeDef


def get_value() -> StateTypeDef:
    return {
        "errorCode": ...,
    }


# StateTypeDef definition

class StateTypeDef(TypedDict):
    errorCode: ErrorCodeType,  # (1)
    errorMessage: str,
    status: StatusType,  # (2)
```

1. See [:material-code-brackets: ErrorCodeType](./literals.md#errorcodetype) 
2. See [:material-code-brackets: StatusType](./literals.md#statustype) 
## ResourceStatusTypeDef

```python
# ResourceStatusTypeDef TypedDict usage example

from types_aiobotocore_inspector2.type_defs import ResourceStatusTypeDef


def get_value() -> ResourceStatusTypeDef:
    return {
        "ec2": ...,
    }


# ResourceStatusTypeDef definition

class ResourceStatusTypeDef(TypedDict):
    ec2: StatusType,  # (1)
    ecr: StatusType,  # (1)
    lambda: NotRequired[StatusType],  # (1)
    lambdaCode: NotRequired[StatusType],  # (1)
```

1. See [:material-code-brackets: StatusType](./literals.md#statustype) 
2. See [:material-code-brackets: StatusType](./literals.md#statustype) 
3. See [:material-code-brackets: StatusType](./literals.md#statustype) 
4. See [:material-code-brackets: StatusType](./literals.md#statustype) 
## FindingTypeAggregationTypeDef

```python
# FindingTypeAggregationTypeDef TypedDict usage example

from types_aiobotocore_inspector2.type_defs import FindingTypeAggregationTypeDef


def get_value() -> FindingTypeAggregationTypeDef:
    return {
        "findingType": ...,
    }


# FindingTypeAggregationTypeDef definition

class FindingTypeAggregationTypeDef(TypedDict):
    findingType: NotRequired[AggregationFindingTypeType],  # (1)
    resourceType: NotRequired[AggregationResourceTypeType],  # (2)
    sortBy: NotRequired[FindingTypeSortByType],  # (3)
    sortOrder: NotRequired[SortOrderType],  # (4)
```

1. See [:material-code-brackets: AggregationFindingTypeType](./literals.md#aggregationfindingtypetype) 
2. See [:material-code-brackets: AggregationResourceTypeType](./literals.md#aggregationresourcetypetype) 
3. See [:material-code-brackets: FindingTypeSortByType](./literals.md#findingtypesortbytype) 
4. See [:material-code-brackets: SortOrderType](./literals.md#sortordertype) 
## StringFilterTypeDef

```python
# StringFilterTypeDef TypedDict usage example

from types_aiobotocore_inspector2.type_defs import StringFilterTypeDef


def get_value() -> StringFilterTypeDef:
    return {
        "comparison": ...,
    }


# StringFilterTypeDef definition

class StringFilterTypeDef(TypedDict):
    comparison: StringComparisonType,  # (1)
    value: str,
```

1. See [:material-code-brackets: StringComparisonType](./literals.md#stringcomparisontype) 
## AssociateMemberRequestTypeDef

```python
# AssociateMemberRequestTypeDef TypedDict usage example

from types_aiobotocore_inspector2.type_defs import AssociateMemberRequestTypeDef


def get_value() -> AssociateMemberRequestTypeDef:
    return {
        "accountId": ...,
    }


# AssociateMemberRequestTypeDef definition

class AssociateMemberRequestTypeDef(TypedDict):
    accountId: str,
```

## ResponseMetadataTypeDef

```python
# ResponseMetadataTypeDef TypedDict usage example

from types_aiobotocore_inspector2.type_defs import ResponseMetadataTypeDef


def get_value() -> ResponseMetadataTypeDef:
    return {
        "RequestId": ...,
    }


# ResponseMetadataTypeDef definition

class ResponseMetadataTypeDef(TypedDict):
    RequestId: str,
    HTTPStatusCode: int,
    HTTPHeaders: Dict[str, str],
    RetryAttempts: int,
    HostId: NotRequired[str],
```

## AtigDataTypeDef

```python
# AtigDataTypeDef TypedDict usage example

from types_aiobotocore_inspector2.type_defs import AtigDataTypeDef


def get_value() -> AtigDataTypeDef:
    return {
        "firstSeen": ...,
    }


# AtigDataTypeDef definition

class AtigDataTypeDef(TypedDict):
    firstSeen: NotRequired[datetime],
    lastSeen: NotRequired[datetime],
    targets: NotRequired[List[str]],
    ttps: NotRequired[List[str]],
```

## AutoEnableTypeDef

```python
# AutoEnableTypeDef TypedDict usage example

from types_aiobotocore_inspector2.type_defs import AutoEnableTypeDef


def get_value() -> AutoEnableTypeDef:
    return {
        "ec2": ...,
    }


# AutoEnableTypeDef definition

class AutoEnableTypeDef(TypedDict):
    ec2: bool,
    ecr: bool,
    lambda: NotRequired[bool],
    lambdaCode: NotRequired[bool],
```

## AwsEc2InstanceDetailsTypeDef

```python
# AwsEc2InstanceDetailsTypeDef TypedDict usage example

from types_aiobotocore_inspector2.type_defs import AwsEc2InstanceDetailsTypeDef


def get_value() -> AwsEc2InstanceDetailsTypeDef:
    return {
        "iamInstanceProfileArn": ...,
    }


# AwsEc2InstanceDetailsTypeDef definition

class AwsEc2InstanceDetailsTypeDef(TypedDict):
    iamInstanceProfileArn: NotRequired[str],
    imageId: NotRequired[str],
    ipV4Addresses: NotRequired[List[str]],
    ipV6Addresses: NotRequired[List[str]],
    keyName: NotRequired[str],
    launchedAt: NotRequired[datetime],
    platform: NotRequired[str],
    subnetId: NotRequired[str],
    type: NotRequired[str],
    vpcId: NotRequired[str],
```

## AwsEcrContainerImageDetailsTypeDef

```python
# AwsEcrContainerImageDetailsTypeDef TypedDict usage example

from types_aiobotocore_inspector2.type_defs import AwsEcrContainerImageDetailsTypeDef


def get_value() -> AwsEcrContainerImageDetailsTypeDef:
    return {
        "architecture": ...,
    }


# AwsEcrContainerImageDetailsTypeDef definition

class AwsEcrContainerImageDetailsTypeDef(TypedDict):
    imageHash: str,
    registry: str,
    repositoryName: str,
    architecture: NotRequired[str],
    author: NotRequired[str],
    imageTags: NotRequired[List[str]],
    platform: NotRequired[str],
    pushedAt: NotRequired[datetime],
```

## LambdaVpcConfigTypeDef

```python
# LambdaVpcConfigTypeDef TypedDict usage example

from types_aiobotocore_inspector2.type_defs import LambdaVpcConfigTypeDef


def get_value() -> LambdaVpcConfigTypeDef:
    return {
        "securityGroupIds": ...,
    }


# LambdaVpcConfigTypeDef definition

class LambdaVpcConfigTypeDef(TypedDict):
    securityGroupIds: NotRequired[List[str]],
    subnetIds: NotRequired[List[str]],
    vpcId: NotRequired[str],
```

## BatchGetAccountStatusRequestTypeDef

```python
# BatchGetAccountStatusRequestTypeDef TypedDict usage example

from types_aiobotocore_inspector2.type_defs import BatchGetAccountStatusRequestTypeDef


def get_value() -> BatchGetAccountStatusRequestTypeDef:
    return {
        "accountIds": ...,
    }


# BatchGetAccountStatusRequestTypeDef definition

class BatchGetAccountStatusRequestTypeDef(TypedDict):
    accountIds: NotRequired[Sequence[str]],
```

## BatchGetCodeSnippetRequestTypeDef

```python
# BatchGetCodeSnippetRequestTypeDef TypedDict usage example

from types_aiobotocore_inspector2.type_defs import BatchGetCodeSnippetRequestTypeDef


def get_value() -> BatchGetCodeSnippetRequestTypeDef:
    return {
        "findingArns": ...,
    }


# BatchGetCodeSnippetRequestTypeDef definition

class BatchGetCodeSnippetRequestTypeDef(TypedDict):
    findingArns: Sequence[str],
```

## CodeSnippetErrorTypeDef

```python
# CodeSnippetErrorTypeDef TypedDict usage example

from types_aiobotocore_inspector2.type_defs import CodeSnippetErrorTypeDef


def get_value() -> CodeSnippetErrorTypeDef:
    return {
        "errorCode": ...,
    }


# CodeSnippetErrorTypeDef definition

class CodeSnippetErrorTypeDef(TypedDict):
    errorCode: CodeSnippetErrorCodeType,  # (1)
    errorMessage: str,
    findingArn: str,
```

1. See [:material-code-brackets: CodeSnippetErrorCodeType](./literals.md#codesnippeterrorcodetype) 
## BatchGetFindingDetailsRequestTypeDef

```python
# BatchGetFindingDetailsRequestTypeDef TypedDict usage example

from types_aiobotocore_inspector2.type_defs import BatchGetFindingDetailsRequestTypeDef


def get_value() -> BatchGetFindingDetailsRequestTypeDef:
    return {
        "findingArns": ...,
    }


# BatchGetFindingDetailsRequestTypeDef definition

class BatchGetFindingDetailsRequestTypeDef(TypedDict):
    findingArns: Sequence[str],
```

## FindingDetailsErrorTypeDef

```python
# FindingDetailsErrorTypeDef TypedDict usage example

from types_aiobotocore_inspector2.type_defs import FindingDetailsErrorTypeDef


def get_value() -> FindingDetailsErrorTypeDef:
    return {
        "errorCode": ...,
    }


# FindingDetailsErrorTypeDef definition

class FindingDetailsErrorTypeDef(TypedDict):
    errorCode: FindingDetailsErrorCodeType,  # (1)
    errorMessage: str,
    findingArn: str,
```

1. See [:material-code-brackets: FindingDetailsErrorCodeType](./literals.md#findingdetailserrorcodetype) 
## BatchGetFreeTrialInfoRequestTypeDef

```python
# BatchGetFreeTrialInfoRequestTypeDef TypedDict usage example

from types_aiobotocore_inspector2.type_defs import BatchGetFreeTrialInfoRequestTypeDef


def get_value() -> BatchGetFreeTrialInfoRequestTypeDef:
    return {
        "accountIds": ...,
    }


# BatchGetFreeTrialInfoRequestTypeDef definition

class BatchGetFreeTrialInfoRequestTypeDef(TypedDict):
    accountIds: Sequence[str],
```

## FreeTrialInfoErrorTypeDef

```python
# FreeTrialInfoErrorTypeDef TypedDict usage example

from types_aiobotocore_inspector2.type_defs import FreeTrialInfoErrorTypeDef


def get_value() -> FreeTrialInfoErrorTypeDef:
    return {
        "accountId": ...,
    }


# FreeTrialInfoErrorTypeDef definition

class FreeTrialInfoErrorTypeDef(TypedDict):
    accountId: str,
    code: FreeTrialInfoErrorCodeType,  # (1)
    message: str,
```

1. See [:material-code-brackets: FreeTrialInfoErrorCodeType](./literals.md#freetrialinfoerrorcodetype) 
## BatchGetMemberEc2DeepInspectionStatusRequestTypeDef

```python
# BatchGetMemberEc2DeepInspectionStatusRequestTypeDef TypedDict usage example

from types_aiobotocore_inspector2.type_defs import BatchGetMemberEc2DeepInspectionStatusRequestTypeDef


def get_value() -> BatchGetMemberEc2DeepInspectionStatusRequestTypeDef:
    return {
        "accountIds": ...,
    }


# BatchGetMemberEc2DeepInspectionStatusRequestTypeDef definition

class BatchGetMemberEc2DeepInspectionStatusRequestTypeDef(TypedDict):
    accountIds: NotRequired[Sequence[str]],
```

## FailedMemberAccountEc2DeepInspectionStatusStateTypeDef

```python
# FailedMemberAccountEc2DeepInspectionStatusStateTypeDef TypedDict usage example

from types_aiobotocore_inspector2.type_defs import FailedMemberAccountEc2DeepInspectionStatusStateTypeDef


def get_value() -> FailedMemberAccountEc2DeepInspectionStatusStateTypeDef:
    return {
        "accountId": ...,
    }


# FailedMemberAccountEc2DeepInspectionStatusStateTypeDef definition

class FailedMemberAccountEc2DeepInspectionStatusStateTypeDef(TypedDict):
    accountId: str,
    ec2ScanStatus: NotRequired[StatusType],  # (1)
    errorMessage: NotRequired[str],
```

1. See [:material-code-brackets: StatusType](./literals.md#statustype) 
## MemberAccountEc2DeepInspectionStatusStateTypeDef

```python
# MemberAccountEc2DeepInspectionStatusStateTypeDef TypedDict usage example

from types_aiobotocore_inspector2.type_defs import MemberAccountEc2DeepInspectionStatusStateTypeDef


def get_value() -> MemberAccountEc2DeepInspectionStatusStateTypeDef:
    return {
        "accountId": ...,
    }


# MemberAccountEc2DeepInspectionStatusStateTypeDef definition

class MemberAccountEc2DeepInspectionStatusStateTypeDef(TypedDict):
    accountId: str,
    errorMessage: NotRequired[str],
    status: NotRequired[Ec2DeepInspectionStatusType],  # (1)
```

1. See [:material-code-brackets: Ec2DeepInspectionStatusType](./literals.md#ec2deepinspectionstatustype) 
## MemberAccountEc2DeepInspectionStatusTypeDef

```python
# MemberAccountEc2DeepInspectionStatusTypeDef TypedDict usage example

from types_aiobotocore_inspector2.type_defs import MemberAccountEc2DeepInspectionStatusTypeDef


def get_value() -> MemberAccountEc2DeepInspectionStatusTypeDef:
    return {
        "accountId": ...,
    }


# MemberAccountEc2DeepInspectionStatusTypeDef definition

class MemberAccountEc2DeepInspectionStatusTypeDef(TypedDict):
    accountId: str,
    activateDeepInspection: bool,
```

## CancelFindingsReportRequestTypeDef

```python
# CancelFindingsReportRequestTypeDef TypedDict usage example

from types_aiobotocore_inspector2.type_defs import CancelFindingsReportRequestTypeDef


def get_value() -> CancelFindingsReportRequestTypeDef:
    return {
        "reportId": ...,
    }


# CancelFindingsReportRequestTypeDef definition

class CancelFindingsReportRequestTypeDef(TypedDict):
    reportId: str,
```

## CancelSbomExportRequestTypeDef

```python
# CancelSbomExportRequestTypeDef TypedDict usage example

from types_aiobotocore_inspector2.type_defs import CancelSbomExportRequestTypeDef


def get_value() -> CancelSbomExportRequestTypeDef:
    return {
        "reportId": ...,
    }


# CancelSbomExportRequestTypeDef definition

class CancelSbomExportRequestTypeDef(TypedDict):
    reportId: str,
```

## StatusCountsTypeDef

```python
# StatusCountsTypeDef TypedDict usage example

from types_aiobotocore_inspector2.type_defs import StatusCountsTypeDef


def get_value() -> StatusCountsTypeDef:
    return {
        "failed": ...,
    }


# StatusCountsTypeDef definition

class StatusCountsTypeDef(TypedDict):
    failed: NotRequired[int],
    passed: NotRequired[int],
    skipped: NotRequired[int],
```

## CisFindingStatusFilterTypeDef

```python
# CisFindingStatusFilterTypeDef TypedDict usage example

from types_aiobotocore_inspector2.type_defs import CisFindingStatusFilterTypeDef


def get_value() -> CisFindingStatusFilterTypeDef:
    return {
        "comparison": ...,
    }


# CisFindingStatusFilterTypeDef definition

class CisFindingStatusFilterTypeDef(TypedDict):
    comparison: CisFindingStatusComparisonType,  # (1)
    value: CisFindingStatusType,  # (2)
```

1. See [:material-code-brackets: CisFindingStatusComparisonType](./literals.md#cisfindingstatuscomparisontype) 
2. See [:material-code-brackets: CisFindingStatusType](./literals.md#cisfindingstatustype) 
## CisNumberFilterTypeDef

```python
# CisNumberFilterTypeDef TypedDict usage example

from types_aiobotocore_inspector2.type_defs import CisNumberFilterTypeDef


def get_value() -> CisNumberFilterTypeDef:
    return {
        "lowerInclusive": ...,
    }


# CisNumberFilterTypeDef definition

class CisNumberFilterTypeDef(TypedDict):
    lowerInclusive: NotRequired[int],
    upperInclusive: NotRequired[int],
```

## CisResultStatusFilterTypeDef

```python
# CisResultStatusFilterTypeDef TypedDict usage example

from types_aiobotocore_inspector2.type_defs import CisResultStatusFilterTypeDef


def get_value() -> CisResultStatusFilterTypeDef:
    return {
        "comparison": ...,
    }


# CisResultStatusFilterTypeDef definition

class CisResultStatusFilterTypeDef(TypedDict):
    comparison: CisResultStatusComparisonType,  # (1)
    value: CisResultStatusType,  # (2)
```

1. See [:material-code-brackets: CisResultStatusComparisonType](./literals.md#cisresultstatuscomparisontype) 
2. See [:material-code-brackets: CisResultStatusType](./literals.md#cisresultstatustype) 
## CisTargetsTypeDef

```python
# CisTargetsTypeDef TypedDict usage example

from types_aiobotocore_inspector2.type_defs import CisTargetsTypeDef


def get_value() -> CisTargetsTypeDef:
    return {
        "accountIds": ...,
    }


# CisTargetsTypeDef definition

class CisTargetsTypeDef(TypedDict):
    accountIds: NotRequired[List[str]],
    targetResourceTags: NotRequired[Dict[str, List[str]]],
```

## CisSecurityLevelFilterTypeDef

```python
# CisSecurityLevelFilterTypeDef TypedDict usage example

from types_aiobotocore_inspector2.type_defs import CisSecurityLevelFilterTypeDef


def get_value() -> CisSecurityLevelFilterTypeDef:
    return {
        "comparison": ...,
    }


# CisSecurityLevelFilterTypeDef definition

class CisSecurityLevelFilterTypeDef(TypedDict):
    comparison: CisSecurityLevelComparisonType,  # (1)
    value: CisSecurityLevelType,  # (2)
```

1. See [:material-code-brackets: CisSecurityLevelComparisonType](./literals.md#cissecuritylevelcomparisontype) 
2. See [:material-code-brackets: CisSecurityLevelType](./literals.md#cissecurityleveltype) 
## CisStringFilterTypeDef

```python
# CisStringFilterTypeDef TypedDict usage example

from types_aiobotocore_inspector2.type_defs import CisStringFilterTypeDef


def get_value() -> CisStringFilterTypeDef:
    return {
        "comparison": ...,
    }


# CisStringFilterTypeDef definition

class CisStringFilterTypeDef(TypedDict):
    comparison: CisStringComparisonType,  # (1)
    value: str,
```

1. See [:material-code-brackets: CisStringComparisonType](./literals.md#cisstringcomparisontype) 
## CisScanResultDetailsTypeDef

```python
# CisScanResultDetailsTypeDef TypedDict usage example

from types_aiobotocore_inspector2.type_defs import CisScanResultDetailsTypeDef


def get_value() -> CisScanResultDetailsTypeDef:
    return {
        "accountId": ...,
    }


# CisScanResultDetailsTypeDef definition

class CisScanResultDetailsTypeDef(TypedDict):
    scanArn: str,
    accountId: NotRequired[str],
    checkDescription: NotRequired[str],
    checkId: NotRequired[str],
    findingArn: NotRequired[str],
    level: NotRequired[CisSecurityLevelType],  # (1)
    platform: NotRequired[str],
    remediation: NotRequired[str],
    status: NotRequired[CisFindingStatusType],  # (2)
    statusReason: NotRequired[str],
    targetResourceId: NotRequired[str],
    title: NotRequired[str],
```

1. See [:material-code-brackets: CisSecurityLevelType](./literals.md#cissecurityleveltype) 
2. See [:material-code-brackets: CisFindingStatusType](./literals.md#cisfindingstatustype) 
## CisTargetStatusFilterTypeDef

```python
# CisTargetStatusFilterTypeDef TypedDict usage example

from types_aiobotocore_inspector2.type_defs import CisTargetStatusFilterTypeDef


def get_value() -> CisTargetStatusFilterTypeDef:
    return {
        "comparison": ...,
    }


# CisTargetStatusFilterTypeDef definition

class CisTargetStatusFilterTypeDef(TypedDict):
    comparison: CisTargetStatusComparisonType,  # (1)
    value: CisTargetStatusType,  # (2)
```

1. See [:material-code-brackets: CisTargetStatusComparisonType](./literals.md#cistargetstatuscomparisontype) 
2. See [:material-code-brackets: CisTargetStatusType](./literals.md#cistargetstatustype) 
## CisTargetStatusReasonFilterTypeDef

```python
# CisTargetStatusReasonFilterTypeDef TypedDict usage example

from types_aiobotocore_inspector2.type_defs import CisTargetStatusReasonFilterTypeDef


def get_value() -> CisTargetStatusReasonFilterTypeDef:
    return {
        "comparison": ...,
    }


# CisTargetStatusReasonFilterTypeDef definition

class CisTargetStatusReasonFilterTypeDef(TypedDict):
    comparison: CisTargetStatusComparisonType,  # (1)
    value: CisTargetStatusReasonType,  # (2)
```

1. See [:material-code-brackets: CisTargetStatusComparisonType](./literals.md#cistargetstatuscomparisontype) 
2. See [:material-code-brackets: CisTargetStatusReasonType](./literals.md#cistargetstatusreasontype) 
## TagFilterTypeDef

```python
# TagFilterTypeDef TypedDict usage example

from types_aiobotocore_inspector2.type_defs import TagFilterTypeDef


def get_value() -> TagFilterTypeDef:
    return {
        "comparison": ...,
    }


# TagFilterTypeDef definition

class TagFilterTypeDef(TypedDict):
    comparison: TagComparisonType,  # (1)
    key: str,
    value: str,
```

1. See [:material-code-brackets: TagComparisonType](./literals.md#tagcomparisontype) 
## CisScanStatusFilterTypeDef

```python
# CisScanStatusFilterTypeDef TypedDict usage example

from types_aiobotocore_inspector2.type_defs import CisScanStatusFilterTypeDef


def get_value() -> CisScanStatusFilterTypeDef:
    return {
        "comparison": ...,
    }


# CisScanStatusFilterTypeDef definition

class CisScanStatusFilterTypeDef(TypedDict):
    comparison: CisScanStatusComparisonType,  # (1)
    value: CisScanStatusType,  # (2)
```

1. See [:material-code-brackets: CisScanStatusComparisonType](./literals.md#cisscanstatuscomparisontype) 
2. See [:material-code-brackets: CisScanStatusType](./literals.md#cisscanstatustype) 
## CisaDataTypeDef

```python
# CisaDataTypeDef TypedDict usage example

from types_aiobotocore_inspector2.type_defs import CisaDataTypeDef


def get_value() -> CisaDataTypeDef:
    return {
        "action": ...,
    }


# CisaDataTypeDef definition

class CisaDataTypeDef(TypedDict):
    action: NotRequired[str],
    dateAdded: NotRequired[datetime],
    dateDue: NotRequired[datetime],
```

## CodeFilePathTypeDef

```python
# CodeFilePathTypeDef TypedDict usage example

from types_aiobotocore_inspector2.type_defs import CodeFilePathTypeDef


def get_value() -> CodeFilePathTypeDef:
    return {
        "endLine": ...,
    }


# CodeFilePathTypeDef definition

class CodeFilePathTypeDef(TypedDict):
    endLine: int,
    fileName: str,
    filePath: str,
    startLine: int,
```

## CodeLineTypeDef

```python
# CodeLineTypeDef TypedDict usage example

from types_aiobotocore_inspector2.type_defs import CodeLineTypeDef


def get_value() -> CodeLineTypeDef:
    return {
        "content": ...,
    }


# CodeLineTypeDef definition

class CodeLineTypeDef(TypedDict):
    content: str,
    lineNumber: int,
```

## SuggestedFixTypeDef

```python
# SuggestedFixTypeDef TypedDict usage example

from types_aiobotocore_inspector2.type_defs import SuggestedFixTypeDef


def get_value() -> SuggestedFixTypeDef:
    return {
        "code": ...,
    }


# SuggestedFixTypeDef definition

class SuggestedFixTypeDef(TypedDict):
    code: NotRequired[str],
    description: NotRequired[str],
```

## ComputePlatformTypeDef

```python
# ComputePlatformTypeDef TypedDict usage example

from types_aiobotocore_inspector2.type_defs import ComputePlatformTypeDef


def get_value() -> ComputePlatformTypeDef:
    return {
        "product": ...,
    }


# ComputePlatformTypeDef definition

class ComputePlatformTypeDef(TypedDict):
    product: NotRequired[str],
    vendor: NotRequired[str],
    version: NotRequired[str],
```

## CountsTypeDef

```python
# CountsTypeDef TypedDict usage example

from types_aiobotocore_inspector2.type_defs import CountsTypeDef


def get_value() -> CountsTypeDef:
    return {
        "count": ...,
    }


# CountsTypeDef definition

class CountsTypeDef(TypedDict):
    count: NotRequired[int],
    groupKey: NotRequired[GroupKeyType],  # (1)
```

1. See [:material-code-brackets: GroupKeyType](./literals.md#groupkeytype) 
## CoverageMapFilterTypeDef

```python
# CoverageMapFilterTypeDef TypedDict usage example

from types_aiobotocore_inspector2.type_defs import CoverageMapFilterTypeDef


def get_value() -> CoverageMapFilterTypeDef:
    return {
        "comparison": ...,
    }


# CoverageMapFilterTypeDef definition

class CoverageMapFilterTypeDef(TypedDict):
    comparison: CoverageMapComparisonType,  # (1)
    key: str,
    value: NotRequired[str],
```

1. See [:material-code-brackets: CoverageMapComparisonType](./literals.md#coveragemapcomparisontype) 
## CoverageStringFilterTypeDef

```python
# CoverageStringFilterTypeDef TypedDict usage example

from types_aiobotocore_inspector2.type_defs import CoverageStringFilterTypeDef


def get_value() -> CoverageStringFilterTypeDef:
    return {
        "comparison": ...,
    }


# CoverageStringFilterTypeDef definition

class CoverageStringFilterTypeDef(TypedDict):
    comparison: CoverageStringComparisonType,  # (1)
    value: str,
```

1. See [:material-code-brackets: CoverageStringComparisonType](./literals.md#coveragestringcomparisontype) 
## ScanStatusTypeDef

```python
# ScanStatusTypeDef TypedDict usage example

from types_aiobotocore_inspector2.type_defs import ScanStatusTypeDef


def get_value() -> ScanStatusTypeDef:
    return {
        "reason": ...,
    }


# ScanStatusTypeDef definition

class ScanStatusTypeDef(TypedDict):
    reason: ScanStatusReasonType,  # (1)
    statusCode: ScanStatusCodeType,  # (2)
```

1. See [:material-code-brackets: ScanStatusReasonType](./literals.md#scanstatusreasontype) 
2. See [:material-code-brackets: ScanStatusCodeType](./literals.md#scanstatuscodetype) 
## CreateCisTargetsTypeDef

```python
# CreateCisTargetsTypeDef TypedDict usage example

from types_aiobotocore_inspector2.type_defs import CreateCisTargetsTypeDef


def get_value() -> CreateCisTargetsTypeDef:
    return {
        "accountIds": ...,
    }


# CreateCisTargetsTypeDef definition

class CreateCisTargetsTypeDef(TypedDict):
    accountIds: Sequence[str],
    targetResourceTags: Mapping[str, Sequence[str]],
```

## DestinationTypeDef

```python
# DestinationTypeDef TypedDict usage example

from types_aiobotocore_inspector2.type_defs import DestinationTypeDef


def get_value() -> DestinationTypeDef:
    return {
        "bucketName": ...,
    }


# DestinationTypeDef definition

class DestinationTypeDef(TypedDict):
    bucketName: str,
    kmsKeyArn: str,
    keyPrefix: NotRequired[str],
```

## Cvss2TypeDef

```python
# Cvss2TypeDef TypedDict usage example

from types_aiobotocore_inspector2.type_defs import Cvss2TypeDef


def get_value() -> Cvss2TypeDef:
    return {
        "baseScore": ...,
    }


# Cvss2TypeDef definition

class Cvss2TypeDef(TypedDict):
    baseScore: NotRequired[float],
    scoringVector: NotRequired[str],
```

## Cvss3TypeDef

```python
# Cvss3TypeDef TypedDict usage example

from types_aiobotocore_inspector2.type_defs import Cvss3TypeDef


def get_value() -> Cvss3TypeDef:
    return {
        "baseScore": ...,
    }


# Cvss3TypeDef definition

class Cvss3TypeDef(TypedDict):
    baseScore: NotRequired[float],
    scoringVector: NotRequired[str],
```

## CvssScoreAdjustmentTypeDef

```python
# CvssScoreAdjustmentTypeDef TypedDict usage example

from types_aiobotocore_inspector2.type_defs import CvssScoreAdjustmentTypeDef


def get_value() -> CvssScoreAdjustmentTypeDef:
    return {
        "metric": ...,
    }


# CvssScoreAdjustmentTypeDef definition

class CvssScoreAdjustmentTypeDef(TypedDict):
    metric: str,
    reason: str,
```

## CvssScoreTypeDef

```python
# CvssScoreTypeDef TypedDict usage example

from types_aiobotocore_inspector2.type_defs import CvssScoreTypeDef


def get_value() -> CvssScoreTypeDef:
    return {
        "baseScore": ...,
    }


# CvssScoreTypeDef definition

class CvssScoreTypeDef(TypedDict):
    baseScore: float,
    scoringVector: str,
    source: str,
    version: str,
```

## TimeTypeDef

```python
# TimeTypeDef TypedDict usage example

from types_aiobotocore_inspector2.type_defs import TimeTypeDef


def get_value() -> TimeTypeDef:
    return {
        "timeOfDay": ...,
    }


# TimeTypeDef definition

class TimeTypeDef(TypedDict):
    timeOfDay: str,
    timezone: str,
```

## DateFilterOutputTypeDef

```python
# DateFilterOutputTypeDef TypedDict usage example

from types_aiobotocore_inspector2.type_defs import DateFilterOutputTypeDef


def get_value() -> DateFilterOutputTypeDef:
    return {
        "endInclusive": ...,
    }


# DateFilterOutputTypeDef definition

class DateFilterOutputTypeDef(TypedDict):
    endInclusive: NotRequired[datetime],
    startInclusive: NotRequired[datetime],
```

## DelegatedAdminAccountTypeDef

```python
# DelegatedAdminAccountTypeDef TypedDict usage example

from types_aiobotocore_inspector2.type_defs import DelegatedAdminAccountTypeDef


def get_value() -> DelegatedAdminAccountTypeDef:
    return {
        "accountId": ...,
    }


# DelegatedAdminAccountTypeDef definition

class DelegatedAdminAccountTypeDef(TypedDict):
    accountId: NotRequired[str],
    status: NotRequired[DelegatedAdminStatusType],  # (1)
```

1. See [:material-code-brackets: DelegatedAdminStatusType](./literals.md#delegatedadminstatustype) 
## DelegatedAdminTypeDef

```python
# DelegatedAdminTypeDef TypedDict usage example

from types_aiobotocore_inspector2.type_defs import DelegatedAdminTypeDef


def get_value() -> DelegatedAdminTypeDef:
    return {
        "accountId": ...,
    }


# DelegatedAdminTypeDef definition

class DelegatedAdminTypeDef(TypedDict):
    accountId: NotRequired[str],
    relationshipStatus: NotRequired[RelationshipStatusType],  # (1)
```

1. See [:material-code-brackets: RelationshipStatusType](./literals.md#relationshipstatustype) 
## DeleteCisScanConfigurationRequestTypeDef

```python
# DeleteCisScanConfigurationRequestTypeDef TypedDict usage example

from types_aiobotocore_inspector2.type_defs import DeleteCisScanConfigurationRequestTypeDef


def get_value() -> DeleteCisScanConfigurationRequestTypeDef:
    return {
        "scanConfigurationArn": ...,
    }


# DeleteCisScanConfigurationRequestTypeDef definition

class DeleteCisScanConfigurationRequestTypeDef(TypedDict):
    scanConfigurationArn: str,
```

## DeleteFilterRequestTypeDef

```python
# DeleteFilterRequestTypeDef TypedDict usage example

from types_aiobotocore_inspector2.type_defs import DeleteFilterRequestTypeDef


def get_value() -> DeleteFilterRequestTypeDef:
    return {
        "arn": ...,
    }


# DeleteFilterRequestTypeDef definition

class DeleteFilterRequestTypeDef(TypedDict):
    arn: str,
```

## DisableDelegatedAdminAccountRequestTypeDef

```python
# DisableDelegatedAdminAccountRequestTypeDef TypedDict usage example

from types_aiobotocore_inspector2.type_defs import DisableDelegatedAdminAccountRequestTypeDef


def get_value() -> DisableDelegatedAdminAccountRequestTypeDef:
    return {
        "delegatedAdminAccountId": ...,
    }


# DisableDelegatedAdminAccountRequestTypeDef definition

class DisableDelegatedAdminAccountRequestTypeDef(TypedDict):
    delegatedAdminAccountId: str,
```

## DisableRequestTypeDef

```python
# DisableRequestTypeDef TypedDict usage example

from types_aiobotocore_inspector2.type_defs import DisableRequestTypeDef


def get_value() -> DisableRequestTypeDef:
    return {
        "accountIds": ...,
    }


# DisableRequestTypeDef definition

class DisableRequestTypeDef(TypedDict):
    accountIds: NotRequired[Sequence[str]],
    resourceTypes: NotRequired[Sequence[ResourceScanTypeType]],  # (1)
```

1. See [:material-code-brackets: ResourceScanTypeType](./literals.md#resourcescantypetype) 
## DisassociateMemberRequestTypeDef

```python
# DisassociateMemberRequestTypeDef TypedDict usage example

from types_aiobotocore_inspector2.type_defs import DisassociateMemberRequestTypeDef


def get_value() -> DisassociateMemberRequestTypeDef:
    return {
        "accountId": ...,
    }


# DisassociateMemberRequestTypeDef definition

class DisassociateMemberRequestTypeDef(TypedDict):
    accountId: str,
```

## Ec2ScanModeStateTypeDef

```python
# Ec2ScanModeStateTypeDef TypedDict usage example

from types_aiobotocore_inspector2.type_defs import Ec2ScanModeStateTypeDef


def get_value() -> Ec2ScanModeStateTypeDef:
    return {
        "scanMode": ...,
    }


# Ec2ScanModeStateTypeDef definition

class Ec2ScanModeStateTypeDef(TypedDict):
    scanMode: NotRequired[Ec2ScanModeType],  # (1)
    scanModeStatus: NotRequired[Ec2ScanModeStatusType],  # (2)
```

1. See [:material-code-brackets: Ec2ScanModeType](./literals.md#ec2scanmodetype) 
2. See [:material-code-brackets: Ec2ScanModeStatusType](./literals.md#ec2scanmodestatustype) 
## Ec2ConfigurationTypeDef

```python
# Ec2ConfigurationTypeDef TypedDict usage example

from types_aiobotocore_inspector2.type_defs import Ec2ConfigurationTypeDef


def get_value() -> Ec2ConfigurationTypeDef:
    return {
        "scanMode": ...,
    }


# Ec2ConfigurationTypeDef definition

class Ec2ConfigurationTypeDef(TypedDict):
    scanMode: Ec2ScanModeType,  # (1)
```

1. See [:material-code-brackets: Ec2ScanModeType](./literals.md#ec2scanmodetype) 
## MapFilterTypeDef

```python
# MapFilterTypeDef TypedDict usage example

from types_aiobotocore_inspector2.type_defs import MapFilterTypeDef


def get_value() -> MapFilterTypeDef:
    return {
        "comparison": ...,
    }


# MapFilterTypeDef definition

class MapFilterTypeDef(TypedDict):
    comparison: MapComparisonType,  # (1)
    key: str,
    value: NotRequired[str],
```

1. See [:material-code-brackets: MapComparisonType](./literals.md#mapcomparisontype) 
## Ec2MetadataTypeDef

```python
# Ec2MetadataTypeDef TypedDict usage example

from types_aiobotocore_inspector2.type_defs import Ec2MetadataTypeDef


def get_value() -> Ec2MetadataTypeDef:
    return {
        "amiId": ...,
    }


# Ec2MetadataTypeDef definition

class Ec2MetadataTypeDef(TypedDict):
    amiId: NotRequired[str],
    platform: NotRequired[Ec2PlatformType],  # (1)
    tags: NotRequired[Dict[str, str]],
```

1. See [:material-code-brackets: Ec2PlatformType](./literals.md#ec2platformtype) 
## EcrRescanDurationStateTypeDef

```python
# EcrRescanDurationStateTypeDef TypedDict usage example

from types_aiobotocore_inspector2.type_defs import EcrRescanDurationStateTypeDef


def get_value() -> EcrRescanDurationStateTypeDef:
    return {
        "pullDateRescanDuration": ...,
    }


# EcrRescanDurationStateTypeDef definition

class EcrRescanDurationStateTypeDef(TypedDict):
    pullDateRescanDuration: NotRequired[EcrPullDateRescanDurationType],  # (1)
    rescanDuration: NotRequired[EcrRescanDurationType],  # (2)
    status: NotRequired[EcrRescanDurationStatusType],  # (3)
    updatedAt: NotRequired[datetime],
```

1. See [:material-code-brackets: EcrPullDateRescanDurationType](./literals.md#ecrpulldaterescandurationtype) 
2. See [:material-code-brackets: EcrRescanDurationType](./literals.md#ecrrescandurationtype) 
3. See [:material-code-brackets: EcrRescanDurationStatusType](./literals.md#ecrrescandurationstatustype) 
## EcrConfigurationTypeDef

```python
# EcrConfigurationTypeDef TypedDict usage example

from types_aiobotocore_inspector2.type_defs import EcrConfigurationTypeDef


def get_value() -> EcrConfigurationTypeDef:
    return {
        "pullDateRescanDuration": ...,
    }


# EcrConfigurationTypeDef definition

class EcrConfigurationTypeDef(TypedDict):
    rescanDuration: EcrRescanDurationType,  # (2)
    pullDateRescanDuration: NotRequired[EcrPullDateRescanDurationType],  # (1)
```

1. See [:material-code-brackets: EcrPullDateRescanDurationType](./literals.md#ecrpulldaterescandurationtype) 
2. See [:material-code-brackets: EcrRescanDurationType](./literals.md#ecrrescandurationtype) 
## EcrContainerImageMetadataTypeDef

```python
# EcrContainerImageMetadataTypeDef TypedDict usage example

from types_aiobotocore_inspector2.type_defs import EcrContainerImageMetadataTypeDef


def get_value() -> EcrContainerImageMetadataTypeDef:
    return {
        "imagePulledAt": ...,
    }


# EcrContainerImageMetadataTypeDef definition

class EcrContainerImageMetadataTypeDef(TypedDict):
    imagePulledAt: NotRequired[datetime],
    tags: NotRequired[List[str]],
```

## EcrRepositoryMetadataTypeDef

```python
# EcrRepositoryMetadataTypeDef TypedDict usage example

from types_aiobotocore_inspector2.type_defs import EcrRepositoryMetadataTypeDef


def get_value() -> EcrRepositoryMetadataTypeDef:
    return {
        "name": ...,
    }


# EcrRepositoryMetadataTypeDef definition

class EcrRepositoryMetadataTypeDef(TypedDict):
    name: NotRequired[str],
    scanFrequency: NotRequired[EcrScanFrequencyType],  # (1)
```

1. See [:material-code-brackets: EcrScanFrequencyType](./literals.md#ecrscanfrequencytype) 
## EnableDelegatedAdminAccountRequestTypeDef

```python
# EnableDelegatedAdminAccountRequestTypeDef TypedDict usage example

from types_aiobotocore_inspector2.type_defs import EnableDelegatedAdminAccountRequestTypeDef


def get_value() -> EnableDelegatedAdminAccountRequestTypeDef:
    return {
        "delegatedAdminAccountId": ...,
    }


# EnableDelegatedAdminAccountRequestTypeDef definition

class EnableDelegatedAdminAccountRequestTypeDef(TypedDict):
    delegatedAdminAccountId: str,
    clientToken: NotRequired[str],
```

## EnableRequestTypeDef

```python
# EnableRequestTypeDef TypedDict usage example

from types_aiobotocore_inspector2.type_defs import EnableRequestTypeDef


def get_value() -> EnableRequestTypeDef:
    return {
        "resourceTypes": ...,
    }


# EnableRequestTypeDef definition

class EnableRequestTypeDef(TypedDict):
    resourceTypes: Sequence[ResourceScanTypeType],  # (1)
    accountIds: NotRequired[Sequence[str]],
    clientToken: NotRequired[str],
```

1. See [:material-code-brackets: ResourceScanTypeType](./literals.md#resourcescantypetype) 
## EpssDetailsTypeDef

```python
# EpssDetailsTypeDef TypedDict usage example

from types_aiobotocore_inspector2.type_defs import EpssDetailsTypeDef


def get_value() -> EpssDetailsTypeDef:
    return {
        "score": ...,
    }


# EpssDetailsTypeDef definition

class EpssDetailsTypeDef(TypedDict):
    score: NotRequired[float],
```

## EpssTypeDef

```python
# EpssTypeDef TypedDict usage example

from types_aiobotocore_inspector2.type_defs import EpssTypeDef


def get_value() -> EpssTypeDef:
    return {
        "score": ...,
    }


# EpssTypeDef definition

class EpssTypeDef(TypedDict):
    score: NotRequired[float],
```

## EvidenceTypeDef

```python
# EvidenceTypeDef TypedDict usage example

from types_aiobotocore_inspector2.type_defs import EvidenceTypeDef


def get_value() -> EvidenceTypeDef:
    return {
        "evidenceDetail": ...,
    }


# EvidenceTypeDef definition

class EvidenceTypeDef(TypedDict):
    evidenceDetail: NotRequired[str],
    evidenceRule: NotRequired[str],
    severity: NotRequired[str],
```

## ExploitObservedTypeDef

```python
# ExploitObservedTypeDef TypedDict usage example

from types_aiobotocore_inspector2.type_defs import ExploitObservedTypeDef


def get_value() -> ExploitObservedTypeDef:
    return {
        "firstSeen": ...,
    }


# ExploitObservedTypeDef definition

class ExploitObservedTypeDef(TypedDict):
    firstSeen: NotRequired[datetime],
    lastSeen: NotRequired[datetime],
```

## ExploitabilityDetailsTypeDef

```python
# ExploitabilityDetailsTypeDef TypedDict usage example

from types_aiobotocore_inspector2.type_defs import ExploitabilityDetailsTypeDef


def get_value() -> ExploitabilityDetailsTypeDef:
    return {
        "lastKnownExploitAt": ...,
    }


# ExploitabilityDetailsTypeDef definition

class ExploitabilityDetailsTypeDef(TypedDict):
    lastKnownExploitAt: NotRequired[datetime],
```

## NumberFilterTypeDef

```python
# NumberFilterTypeDef TypedDict usage example

from types_aiobotocore_inspector2.type_defs import NumberFilterTypeDef


def get_value() -> NumberFilterTypeDef:
    return {
        "lowerInclusive": ...,
    }


# NumberFilterTypeDef definition

class NumberFilterTypeDef(TypedDict):
    lowerInclusive: NotRequired[float],
    upperInclusive: NotRequired[float],
```

## PortRangeFilterTypeDef

```python
# PortRangeFilterTypeDef TypedDict usage example

from types_aiobotocore_inspector2.type_defs import PortRangeFilterTypeDef


def get_value() -> PortRangeFilterTypeDef:
    return {
        "beginInclusive": ...,
    }


# PortRangeFilterTypeDef definition

class PortRangeFilterTypeDef(TypedDict):
    beginInclusive: NotRequired[int],
    endInclusive: NotRequired[int],
```

## FreeTrialInfoTypeDef

```python
# FreeTrialInfoTypeDef TypedDict usage example

from types_aiobotocore_inspector2.type_defs import FreeTrialInfoTypeDef


def get_value() -> FreeTrialInfoTypeDef:
    return {
        "end": ...,
    }


# FreeTrialInfoTypeDef definition

class FreeTrialInfoTypeDef(TypedDict):
    end: datetime,
    start: datetime,
    status: FreeTrialStatusType,  # (1)
    type: FreeTrialTypeType,  # (2)
```

1. See [:material-code-brackets: FreeTrialStatusType](./literals.md#freetrialstatustype) 
2. See [:material-code-brackets: FreeTrialTypeType](./literals.md#freetrialtypetype) 
## GetCisScanReportRequestTypeDef

```python
# GetCisScanReportRequestTypeDef TypedDict usage example

from types_aiobotocore_inspector2.type_defs import GetCisScanReportRequestTypeDef


def get_value() -> GetCisScanReportRequestTypeDef:
    return {
        "scanArn": ...,
    }


# GetCisScanReportRequestTypeDef definition

class GetCisScanReportRequestTypeDef(TypedDict):
    scanArn: str,
    reportFormat: NotRequired[CisReportFormatType],  # (1)
    targetAccounts: NotRequired[Sequence[str]],
```

1. See [:material-code-brackets: CisReportFormatType](./literals.md#cisreportformattype) 
## PaginatorConfigTypeDef

```python
# PaginatorConfigTypeDef TypedDict usage example

from types_aiobotocore_inspector2.type_defs import PaginatorConfigTypeDef


def get_value() -> PaginatorConfigTypeDef:
    return {
        "MaxItems": ...,
    }


# PaginatorConfigTypeDef definition

class PaginatorConfigTypeDef(TypedDict):
    MaxItems: NotRequired[int],
    PageSize: NotRequired[int],
    StartingToken: NotRequired[str],
```

## GetEncryptionKeyRequestTypeDef

```python
# GetEncryptionKeyRequestTypeDef TypedDict usage example

from types_aiobotocore_inspector2.type_defs import GetEncryptionKeyRequestTypeDef


def get_value() -> GetEncryptionKeyRequestTypeDef:
    return {
        "resourceType": ...,
    }


# GetEncryptionKeyRequestTypeDef definition

class GetEncryptionKeyRequestTypeDef(TypedDict):
    resourceType: ResourceTypeType,  # (1)
    scanType: ScanTypeType,  # (2)
```

1. See [:material-code-brackets: ResourceTypeType](./literals.md#resourcetypetype) 
2. See [:material-code-brackets: ScanTypeType](./literals.md#scantypetype) 
## GetFindingsReportStatusRequestTypeDef

```python
# GetFindingsReportStatusRequestTypeDef TypedDict usage example

from types_aiobotocore_inspector2.type_defs import GetFindingsReportStatusRequestTypeDef


def get_value() -> GetFindingsReportStatusRequestTypeDef:
    return {
        "reportId": ...,
    }


# GetFindingsReportStatusRequestTypeDef definition

class GetFindingsReportStatusRequestTypeDef(TypedDict):
    reportId: NotRequired[str],
```

## GetMemberRequestTypeDef

```python
# GetMemberRequestTypeDef TypedDict usage example

from types_aiobotocore_inspector2.type_defs import GetMemberRequestTypeDef


def get_value() -> GetMemberRequestTypeDef:
    return {
        "accountId": ...,
    }


# GetMemberRequestTypeDef definition

class GetMemberRequestTypeDef(TypedDict):
    accountId: str,
```

## MemberTypeDef

```python
# MemberTypeDef TypedDict usage example

from types_aiobotocore_inspector2.type_defs import MemberTypeDef


def get_value() -> MemberTypeDef:
    return {
        "accountId": ...,
    }


# MemberTypeDef definition

class MemberTypeDef(TypedDict):
    accountId: NotRequired[str],
    delegatedAdminAccountId: NotRequired[str],
    relationshipStatus: NotRequired[RelationshipStatusType],  # (1)
    updatedAt: NotRequired[datetime],
```

1. See [:material-code-brackets: RelationshipStatusType](./literals.md#relationshipstatustype) 
## GetSbomExportRequestTypeDef

```python
# GetSbomExportRequestTypeDef TypedDict usage example

from types_aiobotocore_inspector2.type_defs import GetSbomExportRequestTypeDef


def get_value() -> GetSbomExportRequestTypeDef:
    return {
        "reportId": ...,
    }


# GetSbomExportRequestTypeDef definition

class GetSbomExportRequestTypeDef(TypedDict):
    reportId: str,
```

## LambdaFunctionMetadataTypeDef

```python
# LambdaFunctionMetadataTypeDef TypedDict usage example

from types_aiobotocore_inspector2.type_defs import LambdaFunctionMetadataTypeDef


def get_value() -> LambdaFunctionMetadataTypeDef:
    return {
        "functionName": ...,
    }


# LambdaFunctionMetadataTypeDef definition

class LambdaFunctionMetadataTypeDef(TypedDict):
    functionName: NotRequired[str],
    functionTags: NotRequired[Dict[str, str]],
    layers: NotRequired[List[str]],
    runtime: NotRequired[RuntimeType],  # (1)
```

1. See [:material-code-brackets: RuntimeType](./literals.md#runtimetype) 
## ListAccountPermissionsRequestTypeDef

```python
# ListAccountPermissionsRequestTypeDef TypedDict usage example

from types_aiobotocore_inspector2.type_defs import ListAccountPermissionsRequestTypeDef


def get_value() -> ListAccountPermissionsRequestTypeDef:
    return {
        "maxResults": ...,
    }


# ListAccountPermissionsRequestTypeDef definition

class ListAccountPermissionsRequestTypeDef(TypedDict):
    maxResults: NotRequired[int],
    nextToken: NotRequired[str],
    service: NotRequired[ServiceType],  # (1)
```

1. See [:material-code-brackets: ServiceType](./literals.md#servicetype) 
## PermissionTypeDef

```python
# PermissionTypeDef TypedDict usage example

from types_aiobotocore_inspector2.type_defs import PermissionTypeDef


def get_value() -> PermissionTypeDef:
    return {
        "operation": ...,
    }


# PermissionTypeDef definition

class PermissionTypeDef(TypedDict):
    operation: OperationType,  # (1)
    service: ServiceType,  # (2)
```

1. See [:material-code-brackets: OperationType](./literals.md#operationtype) 
2. See [:material-code-brackets: ServiceType](./literals.md#servicetype) 
## ListDelegatedAdminAccountsRequestTypeDef

```python
# ListDelegatedAdminAccountsRequestTypeDef TypedDict usage example

from types_aiobotocore_inspector2.type_defs import ListDelegatedAdminAccountsRequestTypeDef


def get_value() -> ListDelegatedAdminAccountsRequestTypeDef:
    return {
        "maxResults": ...,
    }


# ListDelegatedAdminAccountsRequestTypeDef definition

class ListDelegatedAdminAccountsRequestTypeDef(TypedDict):
    maxResults: NotRequired[int],
    nextToken: NotRequired[str],
```

## ListFiltersRequestTypeDef

```python
# ListFiltersRequestTypeDef TypedDict usage example

from types_aiobotocore_inspector2.type_defs import ListFiltersRequestTypeDef


def get_value() -> ListFiltersRequestTypeDef:
    return {
        "action": ...,
    }


# ListFiltersRequestTypeDef definition

class ListFiltersRequestTypeDef(TypedDict):
    action: NotRequired[FilterActionType],  # (1)
    arns: NotRequired[Sequence[str]],
    maxResults: NotRequired[int],
    nextToken: NotRequired[str],
```

1. See [:material-code-brackets: FilterActionType](./literals.md#filteractiontype) 
## SortCriteriaTypeDef

```python
# SortCriteriaTypeDef TypedDict usage example

from types_aiobotocore_inspector2.type_defs import SortCriteriaTypeDef


def get_value() -> SortCriteriaTypeDef:
    return {
        "field": ...,
    }


# SortCriteriaTypeDef definition

class SortCriteriaTypeDef(TypedDict):
    field: SortFieldType,  # (1)
    sortOrder: SortOrderType,  # (2)
```

1. See [:material-code-brackets: SortFieldType](./literals.md#sortfieldtype) 
2. See [:material-code-brackets: SortOrderType](./literals.md#sortordertype) 
## ListMembersRequestTypeDef

```python
# ListMembersRequestTypeDef TypedDict usage example

from types_aiobotocore_inspector2.type_defs import ListMembersRequestTypeDef


def get_value() -> ListMembersRequestTypeDef:
    return {
        "maxResults": ...,
    }


# ListMembersRequestTypeDef definition

class ListMembersRequestTypeDef(TypedDict):
    maxResults: NotRequired[int],
    nextToken: NotRequired[str],
    onlyAssociated: NotRequired[bool],
```

## ListTagsForResourceRequestTypeDef

```python
# ListTagsForResourceRequestTypeDef TypedDict usage example

from types_aiobotocore_inspector2.type_defs import ListTagsForResourceRequestTypeDef


def get_value() -> ListTagsForResourceRequestTypeDef:
    return {
        "resourceArn": ...,
    }


# ListTagsForResourceRequestTypeDef definition

class ListTagsForResourceRequestTypeDef(TypedDict):
    resourceArn: str,
```

## ListUsageTotalsRequestTypeDef

```python
# ListUsageTotalsRequestTypeDef TypedDict usage example

from types_aiobotocore_inspector2.type_defs import ListUsageTotalsRequestTypeDef


def get_value() -> ListUsageTotalsRequestTypeDef:
    return {
        "accountIds": ...,
    }


# ListUsageTotalsRequestTypeDef definition

class ListUsageTotalsRequestTypeDef(TypedDict):
    accountIds: NotRequired[Sequence[str]],
    maxResults: NotRequired[int],
    nextToken: NotRequired[str],
```

## StepTypeDef

```python
# StepTypeDef TypedDict usage example

from types_aiobotocore_inspector2.type_defs import StepTypeDef


def get_value() -> StepTypeDef:
    return {
        "componentId": ...,
    }


# StepTypeDef definition

class StepTypeDef(TypedDict):
    componentId: str,
    componentType: str,
```

## PortRangeTypeDef

```python
# PortRangeTypeDef TypedDict usage example

from types_aiobotocore_inspector2.type_defs import PortRangeTypeDef


def get_value() -> PortRangeTypeDef:
    return {
        "begin": ...,
    }


# PortRangeTypeDef definition

class PortRangeTypeDef(TypedDict):
    begin: int,
    end: int,
```

## VulnerablePackageTypeDef

```python
# VulnerablePackageTypeDef TypedDict usage example

from types_aiobotocore_inspector2.type_defs import VulnerablePackageTypeDef


def get_value() -> VulnerablePackageTypeDef:
    return {
        "arch": ...,
    }


# VulnerablePackageTypeDef definition

class VulnerablePackageTypeDef(TypedDict):
    name: str,
    version: str,
    arch: NotRequired[str],
    epoch: NotRequired[int],
    filePath: NotRequired[str],
    fixedInVersion: NotRequired[str],
    packageManager: NotRequired[PackageManagerType],  # (1)
    release: NotRequired[str],
    remediation: NotRequired[str],
    sourceLambdaLayerArn: NotRequired[str],
    sourceLayerHash: NotRequired[str],
```

1. See [:material-code-brackets: PackageManagerType](./literals.md#packagemanagertype) 
## RecommendationTypeDef

```python
# RecommendationTypeDef TypedDict usage example

from types_aiobotocore_inspector2.type_defs import RecommendationTypeDef


def get_value() -> RecommendationTypeDef:
    return {
        "Url": ...,
    }


# RecommendationTypeDef definition

class RecommendationTypeDef(TypedDict):
    Url: NotRequired[str],
    text: NotRequired[str],
```

## ResetEncryptionKeyRequestTypeDef

```python
# ResetEncryptionKeyRequestTypeDef TypedDict usage example

from types_aiobotocore_inspector2.type_defs import ResetEncryptionKeyRequestTypeDef


def get_value() -> ResetEncryptionKeyRequestTypeDef:
    return {
        "resourceType": ...,
    }


# ResetEncryptionKeyRequestTypeDef definition

class ResetEncryptionKeyRequestTypeDef(TypedDict):
    resourceType: ResourceTypeType,  # (1)
    scanType: ScanTypeType,  # (2)
```

1. See [:material-code-brackets: ResourceTypeType](./literals.md#resourcetypetype) 
2. See [:material-code-brackets: ScanTypeType](./literals.md#scantypetype) 
## ResourceMapFilterTypeDef

```python
# ResourceMapFilterTypeDef TypedDict usage example

from types_aiobotocore_inspector2.type_defs import ResourceMapFilterTypeDef


def get_value() -> ResourceMapFilterTypeDef:
    return {
        "comparison": ...,
    }


# ResourceMapFilterTypeDef definition

class ResourceMapFilterTypeDef(TypedDict):
    comparison: ResourceMapComparisonType,  # (1)
    key: str,
    value: NotRequired[str],
```

1. See [:material-code-brackets: ResourceMapComparisonType](./literals.md#resourcemapcomparisontype) 
## ResourceStringFilterTypeDef

```python
# ResourceStringFilterTypeDef TypedDict usage example

from types_aiobotocore_inspector2.type_defs import ResourceStringFilterTypeDef


def get_value() -> ResourceStringFilterTypeDef:
    return {
        "comparison": ...,
    }


# ResourceStringFilterTypeDef definition

class ResourceStringFilterTypeDef(TypedDict):
    comparison: ResourceStringComparisonType,  # (1)
    value: str,
```

1. See [:material-code-brackets: ResourceStringComparisonType](./literals.md#resourcestringcomparisontype) 
## SearchVulnerabilitiesFilterCriteriaTypeDef

```python
# SearchVulnerabilitiesFilterCriteriaTypeDef TypedDict usage example

from types_aiobotocore_inspector2.type_defs import SearchVulnerabilitiesFilterCriteriaTypeDef


def get_value() -> SearchVulnerabilitiesFilterCriteriaTypeDef:
    return {
        "vulnerabilityIds": ...,
    }


# SearchVulnerabilitiesFilterCriteriaTypeDef definition

class SearchVulnerabilitiesFilterCriteriaTypeDef(TypedDict):
    vulnerabilityIds: Sequence[str],
```

## SendCisSessionHealthRequestTypeDef

```python
# SendCisSessionHealthRequestTypeDef TypedDict usage example

from types_aiobotocore_inspector2.type_defs import SendCisSessionHealthRequestTypeDef


def get_value() -> SendCisSessionHealthRequestTypeDef:
    return {
        "scanJobId": ...,
    }


# SendCisSessionHealthRequestTypeDef definition

class SendCisSessionHealthRequestTypeDef(TypedDict):
    scanJobId: str,
    sessionToken: str,
```

## StartCisSessionMessageTypeDef

```python
# StartCisSessionMessageTypeDef TypedDict usage example

from types_aiobotocore_inspector2.type_defs import StartCisSessionMessageTypeDef


def get_value() -> StartCisSessionMessageTypeDef:
    return {
        "sessionToken": ...,
    }


# StartCisSessionMessageTypeDef definition

class StartCisSessionMessageTypeDef(TypedDict):
    sessionToken: str,
```

## StopCisMessageProgressTypeDef

```python
# StopCisMessageProgressTypeDef TypedDict usage example

from types_aiobotocore_inspector2.type_defs import StopCisMessageProgressTypeDef


def get_value() -> StopCisMessageProgressTypeDef:
    return {
        "errorChecks": ...,
    }


# StopCisMessageProgressTypeDef definition

class StopCisMessageProgressTypeDef(TypedDict):
    errorChecks: NotRequired[int],
    failedChecks: NotRequired[int],
    informationalChecks: NotRequired[int],
    notApplicableChecks: NotRequired[int],
    notEvaluatedChecks: NotRequired[int],
    successfulChecks: NotRequired[int],
    totalChecks: NotRequired[int],
    unknownChecks: NotRequired[int],
```

## TagResourceRequestTypeDef

```python
# TagResourceRequestTypeDef TypedDict usage example

from types_aiobotocore_inspector2.type_defs import TagResourceRequestTypeDef


def get_value() -> TagResourceRequestTypeDef:
    return {
        "resourceArn": ...,
    }


# TagResourceRequestTypeDef definition

class TagResourceRequestTypeDef(TypedDict):
    resourceArn: str,
    tags: Mapping[str, str],
```

## UntagResourceRequestTypeDef

```python
# UntagResourceRequestTypeDef TypedDict usage example

from types_aiobotocore_inspector2.type_defs import UntagResourceRequestTypeDef


def get_value() -> UntagResourceRequestTypeDef:
    return {
        "resourceArn": ...,
    }


# UntagResourceRequestTypeDef definition

class UntagResourceRequestTypeDef(TypedDict):
    resourceArn: str,
    tagKeys: Sequence[str],
```

## UpdateCisTargetsTypeDef

```python
# UpdateCisTargetsTypeDef TypedDict usage example

from types_aiobotocore_inspector2.type_defs import UpdateCisTargetsTypeDef


def get_value() -> UpdateCisTargetsTypeDef:
    return {
        "accountIds": ...,
    }


# UpdateCisTargetsTypeDef definition

class UpdateCisTargetsTypeDef(TypedDict):
    accountIds: NotRequired[Sequence[str]],
    targetResourceTags: NotRequired[Mapping[str, Sequence[str]]],
```

## UpdateEc2DeepInspectionConfigurationRequestTypeDef

```python
# UpdateEc2DeepInspectionConfigurationRequestTypeDef TypedDict usage example

from types_aiobotocore_inspector2.type_defs import UpdateEc2DeepInspectionConfigurationRequestTypeDef


def get_value() -> UpdateEc2DeepInspectionConfigurationRequestTypeDef:
    return {
        "activateDeepInspection": ...,
    }


# UpdateEc2DeepInspectionConfigurationRequestTypeDef definition

class UpdateEc2DeepInspectionConfigurationRequestTypeDef(TypedDict):
    activateDeepInspection: NotRequired[bool],
    packagePaths: NotRequired[Sequence[str]],
```

## UpdateEncryptionKeyRequestTypeDef

```python
# UpdateEncryptionKeyRequestTypeDef TypedDict usage example

from types_aiobotocore_inspector2.type_defs import UpdateEncryptionKeyRequestTypeDef


def get_value() -> UpdateEncryptionKeyRequestTypeDef:
    return {
        "kmsKeyId": ...,
    }


# UpdateEncryptionKeyRequestTypeDef definition

class UpdateEncryptionKeyRequestTypeDef(TypedDict):
    kmsKeyId: str,
    resourceType: ResourceTypeType,  # (1)
    scanType: ScanTypeType,  # (2)
```

1. See [:material-code-brackets: ResourceTypeType](./literals.md#resourcetypetype) 
2. See [:material-code-brackets: ScanTypeType](./literals.md#scantypetype) 
## UpdateOrgEc2DeepInspectionConfigurationRequestTypeDef

```python
# UpdateOrgEc2DeepInspectionConfigurationRequestTypeDef TypedDict usage example

from types_aiobotocore_inspector2.type_defs import UpdateOrgEc2DeepInspectionConfigurationRequestTypeDef


def get_value() -> UpdateOrgEc2DeepInspectionConfigurationRequestTypeDef:
    return {
        "orgPackagePaths": ...,
    }


# UpdateOrgEc2DeepInspectionConfigurationRequestTypeDef definition

class UpdateOrgEc2DeepInspectionConfigurationRequestTypeDef(TypedDict):
    orgPackagePaths: Sequence[str],
```

## UsageTypeDef

```python
# UsageTypeDef TypedDict usage example

from types_aiobotocore_inspector2.type_defs import UsageTypeDef


def get_value() -> UsageTypeDef:
    return {
        "currency": ...,
    }


# UsageTypeDef definition

class UsageTypeDef(TypedDict):
    currency: NotRequired[CurrencyType],  # (1)
    estimatedMonthlyCost: NotRequired[float],
    total: NotRequired[float],
    type: NotRequired[UsageTypeType],  # (2)
```

1. See [:material-code-brackets: CurrencyType](./literals.md#currencytype) 
2. See [:material-code-brackets: UsageTypeType](./literals.md#usagetypetype) 
## AccountAggregationResponseTypeDef

```python
# AccountAggregationResponseTypeDef TypedDict usage example

from types_aiobotocore_inspector2.type_defs import AccountAggregationResponseTypeDef


def get_value() -> AccountAggregationResponseTypeDef:
    return {
        "accountId": ...,
    }


# AccountAggregationResponseTypeDef definition

class AccountAggregationResponseTypeDef(TypedDict):
    accountId: NotRequired[str],
    exploitAvailableCount: NotRequired[int],
    fixAvailableCount: NotRequired[int],
    severityCounts: NotRequired[SeverityCountsTypeDef],  # (1)
```

1. See [:material-code-braces: SeverityCountsTypeDef](./type_defs.md#severitycountstypedef) 
## AmiAggregationResponseTypeDef

```python
# AmiAggregationResponseTypeDef TypedDict usage example

from types_aiobotocore_inspector2.type_defs import AmiAggregationResponseTypeDef


def get_value() -> AmiAggregationResponseTypeDef:
    return {
        "accountId": ...,
    }


# AmiAggregationResponseTypeDef definition

class AmiAggregationResponseTypeDef(TypedDict):
    ami: str,
    accountId: NotRequired[str],
    affectedInstances: NotRequired[int],
    severityCounts: NotRequired[SeverityCountsTypeDef],  # (1)
```

1. See [:material-code-braces: SeverityCountsTypeDef](./type_defs.md#severitycountstypedef) 
## AwsEcrContainerAggregationResponseTypeDef

```python
# AwsEcrContainerAggregationResponseTypeDef TypedDict usage example

from types_aiobotocore_inspector2.type_defs import AwsEcrContainerAggregationResponseTypeDef


def get_value() -> AwsEcrContainerAggregationResponseTypeDef:
    return {
        "accountId": ...,
    }


# AwsEcrContainerAggregationResponseTypeDef definition

class AwsEcrContainerAggregationResponseTypeDef(TypedDict):
    resourceId: str,
    accountId: NotRequired[str],
    architecture: NotRequired[str],
    imageSha: NotRequired[str],
    imageTags: NotRequired[List[str]],
    repository: NotRequired[str],
    severityCounts: NotRequired[SeverityCountsTypeDef],  # (1)
```

1. See [:material-code-braces: SeverityCountsTypeDef](./type_defs.md#severitycountstypedef) 
## Ec2InstanceAggregationResponseTypeDef

```python
# Ec2InstanceAggregationResponseTypeDef TypedDict usage example

from types_aiobotocore_inspector2.type_defs import Ec2InstanceAggregationResponseTypeDef


def get_value() -> Ec2InstanceAggregationResponseTypeDef:
    return {
        "accountId": ...,
    }


# Ec2InstanceAggregationResponseTypeDef definition

class Ec2InstanceAggregationResponseTypeDef(TypedDict):
    instanceId: str,
    accountId: NotRequired[str],
    ami: NotRequired[str],
    instanceTags: NotRequired[Dict[str, str]],
    networkFindings: NotRequired[int],
    operatingSystem: NotRequired[str],
    severityCounts: NotRequired[SeverityCountsTypeDef],  # (1)
```

1. See [:material-code-braces: SeverityCountsTypeDef](./type_defs.md#severitycountstypedef) 
## FindingTypeAggregationResponseTypeDef

```python
# FindingTypeAggregationResponseTypeDef TypedDict usage example

from types_aiobotocore_inspector2.type_defs import FindingTypeAggregationResponseTypeDef


def get_value() -> FindingTypeAggregationResponseTypeDef:
    return {
        "accountId": ...,
    }


# FindingTypeAggregationResponseTypeDef definition

class FindingTypeAggregationResponseTypeDef(TypedDict):
    accountId: NotRequired[str],
    exploitAvailableCount: NotRequired[int],
    fixAvailableCount: NotRequired[int],
    severityCounts: NotRequired[SeverityCountsTypeDef],  # (1)
```

1. See [:material-code-braces: SeverityCountsTypeDef](./type_defs.md#severitycountstypedef) 
## ImageLayerAggregationResponseTypeDef

```python
# ImageLayerAggregationResponseTypeDef TypedDict usage example

from types_aiobotocore_inspector2.type_defs import ImageLayerAggregationResponseTypeDef


def get_value() -> ImageLayerAggregationResponseTypeDef:
    return {
        "accountId": ...,
    }


# ImageLayerAggregationResponseTypeDef definition

class ImageLayerAggregationResponseTypeDef(TypedDict):
    accountId: str,
    layerHash: str,
    repository: str,
    resourceId: str,
    severityCounts: NotRequired[SeverityCountsTypeDef],  # (1)
```

1. See [:material-code-braces: SeverityCountsTypeDef](./type_defs.md#severitycountstypedef) 
## LambdaFunctionAggregationResponseTypeDef

```python
# LambdaFunctionAggregationResponseTypeDef TypedDict usage example

from types_aiobotocore_inspector2.type_defs import LambdaFunctionAggregationResponseTypeDef


def get_value() -> LambdaFunctionAggregationResponseTypeDef:
    return {
        "accountId": ...,
    }


# LambdaFunctionAggregationResponseTypeDef definition

class LambdaFunctionAggregationResponseTypeDef(TypedDict):
    resourceId: str,
    accountId: NotRequired[str],
    functionName: NotRequired[str],
    lambdaTags: NotRequired[Dict[str, str]],
    lastModifiedAt: NotRequired[datetime],
    runtime: NotRequired[str],
    severityCounts: NotRequired[SeverityCountsTypeDef],  # (1)
```

1. See [:material-code-braces: SeverityCountsTypeDef](./type_defs.md#severitycountstypedef) 
## LambdaLayerAggregationResponseTypeDef

```python
# LambdaLayerAggregationResponseTypeDef TypedDict usage example

from types_aiobotocore_inspector2.type_defs import LambdaLayerAggregationResponseTypeDef


def get_value() -> LambdaLayerAggregationResponseTypeDef:
    return {
        "accountId": ...,
    }


# LambdaLayerAggregationResponseTypeDef definition

class LambdaLayerAggregationResponseTypeDef(TypedDict):
    accountId: str,
    functionName: str,
    layerArn: str,
    resourceId: str,
    severityCounts: NotRequired[SeverityCountsTypeDef],  # (1)
```

1. See [:material-code-braces: SeverityCountsTypeDef](./type_defs.md#severitycountstypedef) 
## PackageAggregationResponseTypeDef

```python
# PackageAggregationResponseTypeDef TypedDict usage example

from types_aiobotocore_inspector2.type_defs import PackageAggregationResponseTypeDef


def get_value() -> PackageAggregationResponseTypeDef:
    return {
        "accountId": ...,
    }


# PackageAggregationResponseTypeDef definition

class PackageAggregationResponseTypeDef(TypedDict):
    packageName: str,
    accountId: NotRequired[str],
    severityCounts: NotRequired[SeverityCountsTypeDef],  # (1)
```

1. See [:material-code-braces: SeverityCountsTypeDef](./type_defs.md#severitycountstypedef) 
## RepositoryAggregationResponseTypeDef

```python
# RepositoryAggregationResponseTypeDef TypedDict usage example

from types_aiobotocore_inspector2.type_defs import RepositoryAggregationResponseTypeDef


def get_value() -> RepositoryAggregationResponseTypeDef:
    return {
        "accountId": ...,
    }


# RepositoryAggregationResponseTypeDef definition

class RepositoryAggregationResponseTypeDef(TypedDict):
    repository: str,
    accountId: NotRequired[str],
    affectedImages: NotRequired[int],
    severityCounts: NotRequired[SeverityCountsTypeDef],  # (1)
```

1. See [:material-code-braces: SeverityCountsTypeDef](./type_defs.md#severitycountstypedef) 
## TitleAggregationResponseTypeDef

```python
# TitleAggregationResponseTypeDef TypedDict usage example

from types_aiobotocore_inspector2.type_defs import TitleAggregationResponseTypeDef


def get_value() -> TitleAggregationResponseTypeDef:
    return {
        "accountId": ...,
    }


# TitleAggregationResponseTypeDef definition

class TitleAggregationResponseTypeDef(TypedDict):
    title: str,
    accountId: NotRequired[str],
    severityCounts: NotRequired[SeverityCountsTypeDef],  # (1)
    vulnerabilityId: NotRequired[str],
```

1. See [:material-code-braces: SeverityCountsTypeDef](./type_defs.md#severitycountstypedef) 
## ResourceStateTypeDef

```python
# ResourceStateTypeDef TypedDict usage example

from types_aiobotocore_inspector2.type_defs import ResourceStateTypeDef


def get_value() -> ResourceStateTypeDef:
    return {
        "ec2": ...,
    }


# ResourceStateTypeDef definition

class ResourceStateTypeDef(TypedDict):
    ec2: StateTypeDef,  # (1)
    ecr: StateTypeDef,  # (1)
    lambda: NotRequired[StateTypeDef],  # (1)
    lambdaCode: NotRequired[StateTypeDef],  # (1)
```

1. See [:material-code-braces: StateTypeDef](./type_defs.md#statetypedef) 
2. See [:material-code-braces: StateTypeDef](./type_defs.md#statetypedef) 
3. See [:material-code-braces: StateTypeDef](./type_defs.md#statetypedef) 
4. See [:material-code-braces: StateTypeDef](./type_defs.md#statetypedef) 
## AccountTypeDef

```python
# AccountTypeDef TypedDict usage example

from types_aiobotocore_inspector2.type_defs import AccountTypeDef


def get_value() -> AccountTypeDef:
    return {
        "accountId": ...,
    }


# AccountTypeDef definition

class AccountTypeDef(TypedDict):
    accountId: str,
    resourceStatus: ResourceStatusTypeDef,  # (1)
    status: StatusType,  # (2)
```

1. See [:material-code-braces: ResourceStatusTypeDef](./type_defs.md#resourcestatustypedef) 
2. See [:material-code-brackets: StatusType](./literals.md#statustype) 
## FailedAccountTypeDef

```python
# FailedAccountTypeDef TypedDict usage example

from types_aiobotocore_inspector2.type_defs import FailedAccountTypeDef


def get_value() -> FailedAccountTypeDef:
    return {
        "accountId": ...,
    }


# FailedAccountTypeDef definition

class FailedAccountTypeDef(TypedDict):
    accountId: str,
    errorCode: ErrorCodeType,  # (1)
    errorMessage: str,
    resourceStatus: NotRequired[ResourceStatusTypeDef],  # (2)
    status: NotRequired[StatusType],  # (3)
```

1. See [:material-code-brackets: ErrorCodeType](./literals.md#errorcodetype) 
2. See [:material-code-braces: ResourceStatusTypeDef](./type_defs.md#resourcestatustypedef) 
3. See [:material-code-brackets: StatusType](./literals.md#statustype) 
## AmiAggregationTypeDef

```python
# AmiAggregationTypeDef TypedDict usage example

from types_aiobotocore_inspector2.type_defs import AmiAggregationTypeDef


def get_value() -> AmiAggregationTypeDef:
    return {
        "amis": ...,
    }


# AmiAggregationTypeDef definition

class AmiAggregationTypeDef(TypedDict):
    amis: NotRequired[Sequence[StringFilterTypeDef]],  # (1)
    sortBy: NotRequired[AmiSortByType],  # (2)
    sortOrder: NotRequired[SortOrderType],  # (3)
```

1. See [:material-code-braces: StringFilterTypeDef](./type_defs.md#stringfiltertypedef) 
2. See [:material-code-brackets: AmiSortByType](./literals.md#amisortbytype) 
3. See [:material-code-brackets: SortOrderType](./literals.md#sortordertype) 
## AwsEcrContainerAggregationTypeDef

```python
# AwsEcrContainerAggregationTypeDef TypedDict usage example

from types_aiobotocore_inspector2.type_defs import AwsEcrContainerAggregationTypeDef


def get_value() -> AwsEcrContainerAggregationTypeDef:
    return {
        "architectures": ...,
    }


# AwsEcrContainerAggregationTypeDef definition

class AwsEcrContainerAggregationTypeDef(TypedDict):
    architectures: NotRequired[Sequence[StringFilterTypeDef]],  # (1)
    imageShas: NotRequired[Sequence[StringFilterTypeDef]],  # (1)
    imageTags: NotRequired[Sequence[StringFilterTypeDef]],  # (1)
    repositories: NotRequired[Sequence[StringFilterTypeDef]],  # (1)
    resourceIds: NotRequired[Sequence[StringFilterTypeDef]],  # (1)
    sortBy: NotRequired[AwsEcrContainerSortByType],  # (6)
    sortOrder: NotRequired[SortOrderType],  # (7)
```

1. See [:material-code-braces: StringFilterTypeDef](./type_defs.md#stringfiltertypedef) 
2. See [:material-code-braces: StringFilterTypeDef](./type_defs.md#stringfiltertypedef) 
3. See [:material-code-braces: StringFilterTypeDef](./type_defs.md#stringfiltertypedef) 
4. See [:material-code-braces: StringFilterTypeDef](./type_defs.md#stringfiltertypedef) 
5. See [:material-code-braces: StringFilterTypeDef](./type_defs.md#stringfiltertypedef) 
6. See [:material-code-brackets: AwsEcrContainerSortByType](./literals.md#awsecrcontainersortbytype) 
7. See [:material-code-brackets: SortOrderType](./literals.md#sortordertype) 
## ImageLayerAggregationTypeDef

```python
# ImageLayerAggregationTypeDef TypedDict usage example

from types_aiobotocore_inspector2.type_defs import ImageLayerAggregationTypeDef


def get_value() -> ImageLayerAggregationTypeDef:
    return {
        "layerHashes": ...,
    }


# ImageLayerAggregationTypeDef definition

class ImageLayerAggregationTypeDef(TypedDict):
    layerHashes: NotRequired[Sequence[StringFilterTypeDef]],  # (1)
    repositories: NotRequired[Sequence[StringFilterTypeDef]],  # (1)
    resourceIds: NotRequired[Sequence[StringFilterTypeDef]],  # (1)
    sortBy: NotRequired[ImageLayerSortByType],  # (4)
    sortOrder: NotRequired[SortOrderType],  # (5)
```

1. See [:material-code-braces: StringFilterTypeDef](./type_defs.md#stringfiltertypedef) 
2. See [:material-code-braces: StringFilterTypeDef](./type_defs.md#stringfiltertypedef) 
3. See [:material-code-braces: StringFilterTypeDef](./type_defs.md#stringfiltertypedef) 
4. See [:material-code-brackets: ImageLayerSortByType](./literals.md#imagelayersortbytype) 
5. See [:material-code-brackets: SortOrderType](./literals.md#sortordertype) 
## LambdaLayerAggregationTypeDef

```python
# LambdaLayerAggregationTypeDef TypedDict usage example

from types_aiobotocore_inspector2.type_defs import LambdaLayerAggregationTypeDef


def get_value() -> LambdaLayerAggregationTypeDef:
    return {
        "functionNames": ...,
    }


# LambdaLayerAggregationTypeDef definition

class LambdaLayerAggregationTypeDef(TypedDict):
    functionNames: NotRequired[Sequence[StringFilterTypeDef]],  # (1)
    layerArns: NotRequired[Sequence[StringFilterTypeDef]],  # (1)
    resourceIds: NotRequired[Sequence[StringFilterTypeDef]],  # (1)
    sortBy: NotRequired[LambdaLayerSortByType],  # (4)
    sortOrder: NotRequired[SortOrderType],  # (5)
```

1. See [:material-code-braces: StringFilterTypeDef](./type_defs.md#stringfiltertypedef) 
2. See [:material-code-braces: StringFilterTypeDef](./type_defs.md#stringfiltertypedef) 
3. See [:material-code-braces: StringFilterTypeDef](./type_defs.md#stringfiltertypedef) 
4. See [:material-code-brackets: LambdaLayerSortByType](./literals.md#lambdalayersortbytype) 
5. See [:material-code-brackets: SortOrderType](./literals.md#sortordertype) 
## PackageAggregationTypeDef

```python
# PackageAggregationTypeDef TypedDict usage example

from types_aiobotocore_inspector2.type_defs import PackageAggregationTypeDef


def get_value() -> PackageAggregationTypeDef:
    return {
        "packageNames": ...,
    }


# PackageAggregationTypeDef definition

class PackageAggregationTypeDef(TypedDict):
    packageNames: NotRequired[Sequence[StringFilterTypeDef]],  # (1)
    sortBy: NotRequired[PackageSortByType],  # (2)
    sortOrder: NotRequired[SortOrderType],  # (3)
```

1. See [:material-code-braces: StringFilterTypeDef](./type_defs.md#stringfiltertypedef) 
2. See [:material-code-brackets: PackageSortByType](./literals.md#packagesortbytype) 
3. See [:material-code-brackets: SortOrderType](./literals.md#sortordertype) 
## RepositoryAggregationTypeDef

```python
# RepositoryAggregationTypeDef TypedDict usage example

from types_aiobotocore_inspector2.type_defs import RepositoryAggregationTypeDef


def get_value() -> RepositoryAggregationTypeDef:
    return {
        "repositories": ...,
    }


# RepositoryAggregationTypeDef definition

class RepositoryAggregationTypeDef(TypedDict):
    repositories: NotRequired[Sequence[StringFilterTypeDef]],  # (1)
    sortBy: NotRequired[RepositorySortByType],  # (2)
    sortOrder: NotRequired[SortOrderType],  # (3)
```

1. See [:material-code-braces: StringFilterTypeDef](./type_defs.md#stringfiltertypedef) 
2. See [:material-code-brackets: RepositorySortByType](./literals.md#repositorysortbytype) 
3. See [:material-code-brackets: SortOrderType](./literals.md#sortordertype) 
## TitleAggregationTypeDef

```python
# TitleAggregationTypeDef TypedDict usage example

from types_aiobotocore_inspector2.type_defs import TitleAggregationTypeDef


def get_value() -> TitleAggregationTypeDef:
    return {
        "findingType": ...,
    }


# TitleAggregationTypeDef definition

class TitleAggregationTypeDef(TypedDict):
    findingType: NotRequired[AggregationFindingTypeType],  # (1)
    resourceType: NotRequired[AggregationResourceTypeType],  # (2)
    sortBy: NotRequired[TitleSortByType],  # (3)
    sortOrder: NotRequired[SortOrderType],  # (4)
    titles: NotRequired[Sequence[StringFilterTypeDef]],  # (5)
    vulnerabilityIds: NotRequired[Sequence[StringFilterTypeDef]],  # (5)
```

1. See [:material-code-brackets: AggregationFindingTypeType](./literals.md#aggregationfindingtypetype) 
2. See [:material-code-brackets: AggregationResourceTypeType](./literals.md#aggregationresourcetypetype) 
3. See [:material-code-brackets: TitleSortByType](./literals.md#titlesortbytype) 
4. See [:material-code-brackets: SortOrderType](./literals.md#sortordertype) 
5. See [:material-code-braces: StringFilterTypeDef](./type_defs.md#stringfiltertypedef) 
6. See [:material-code-braces: StringFilterTypeDef](./type_defs.md#stringfiltertypedef) 
## AssociateMemberResponseTypeDef

```python
# AssociateMemberResponseTypeDef TypedDict usage example

from types_aiobotocore_inspector2.type_defs import AssociateMemberResponseTypeDef


def get_value() -> AssociateMemberResponseTypeDef:
    return {
        "accountId": ...,
    }


# AssociateMemberResponseTypeDef definition

class AssociateMemberResponseTypeDef(TypedDict):
    accountId: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CancelFindingsReportResponseTypeDef

```python
# CancelFindingsReportResponseTypeDef TypedDict usage example

from types_aiobotocore_inspector2.type_defs import CancelFindingsReportResponseTypeDef


def get_value() -> CancelFindingsReportResponseTypeDef:
    return {
        "reportId": ...,
    }


# CancelFindingsReportResponseTypeDef definition

class CancelFindingsReportResponseTypeDef(TypedDict):
    reportId: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CancelSbomExportResponseTypeDef

```python
# CancelSbomExportResponseTypeDef TypedDict usage example

from types_aiobotocore_inspector2.type_defs import CancelSbomExportResponseTypeDef


def get_value() -> CancelSbomExportResponseTypeDef:
    return {
        "reportId": ...,
    }


# CancelSbomExportResponseTypeDef definition

class CancelSbomExportResponseTypeDef(TypedDict):
    reportId: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateCisScanConfigurationResponseTypeDef

```python
# CreateCisScanConfigurationResponseTypeDef TypedDict usage example

from types_aiobotocore_inspector2.type_defs import CreateCisScanConfigurationResponseTypeDef


def get_value() -> CreateCisScanConfigurationResponseTypeDef:
    return {
        "scanConfigurationArn": ...,
    }


# CreateCisScanConfigurationResponseTypeDef definition

class CreateCisScanConfigurationResponseTypeDef(TypedDict):
    scanConfigurationArn: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateFilterResponseTypeDef

```python
# CreateFilterResponseTypeDef TypedDict usage example

from types_aiobotocore_inspector2.type_defs import CreateFilterResponseTypeDef


def get_value() -> CreateFilterResponseTypeDef:
    return {
        "arn": ...,
    }


# CreateFilterResponseTypeDef definition

class CreateFilterResponseTypeDef(TypedDict):
    arn: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateFindingsReportResponseTypeDef

```python
# CreateFindingsReportResponseTypeDef TypedDict usage example

from types_aiobotocore_inspector2.type_defs import CreateFindingsReportResponseTypeDef


def get_value() -> CreateFindingsReportResponseTypeDef:
    return {
        "reportId": ...,
    }


# CreateFindingsReportResponseTypeDef definition

class CreateFindingsReportResponseTypeDef(TypedDict):
    reportId: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateSbomExportResponseTypeDef

```python
# CreateSbomExportResponseTypeDef TypedDict usage example

from types_aiobotocore_inspector2.type_defs import CreateSbomExportResponseTypeDef


def get_value() -> CreateSbomExportResponseTypeDef:
    return {
        "reportId": ...,
    }


# CreateSbomExportResponseTypeDef definition

class CreateSbomExportResponseTypeDef(TypedDict):
    reportId: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DeleteCisScanConfigurationResponseTypeDef

```python
# DeleteCisScanConfigurationResponseTypeDef TypedDict usage example

from types_aiobotocore_inspector2.type_defs import DeleteCisScanConfigurationResponseTypeDef


def get_value() -> DeleteCisScanConfigurationResponseTypeDef:
    return {
        "scanConfigurationArn": ...,
    }


# DeleteCisScanConfigurationResponseTypeDef definition

class DeleteCisScanConfigurationResponseTypeDef(TypedDict):
    scanConfigurationArn: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DeleteFilterResponseTypeDef

```python
# DeleteFilterResponseTypeDef TypedDict usage example

from types_aiobotocore_inspector2.type_defs import DeleteFilterResponseTypeDef


def get_value() -> DeleteFilterResponseTypeDef:
    return {
        "arn": ...,
    }


# DeleteFilterResponseTypeDef definition

class DeleteFilterResponseTypeDef(TypedDict):
    arn: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DisableDelegatedAdminAccountResponseTypeDef

```python
# DisableDelegatedAdminAccountResponseTypeDef TypedDict usage example

from types_aiobotocore_inspector2.type_defs import DisableDelegatedAdminAccountResponseTypeDef


def get_value() -> DisableDelegatedAdminAccountResponseTypeDef:
    return {
        "delegatedAdminAccountId": ...,
    }


# DisableDelegatedAdminAccountResponseTypeDef definition

class DisableDelegatedAdminAccountResponseTypeDef(TypedDict):
    delegatedAdminAccountId: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DisassociateMemberResponseTypeDef

```python
# DisassociateMemberResponseTypeDef TypedDict usage example

from types_aiobotocore_inspector2.type_defs import DisassociateMemberResponseTypeDef


def get_value() -> DisassociateMemberResponseTypeDef:
    return {
        "accountId": ...,
    }


# DisassociateMemberResponseTypeDef definition

class DisassociateMemberResponseTypeDef(TypedDict):
    accountId: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## EnableDelegatedAdminAccountResponseTypeDef

```python
# EnableDelegatedAdminAccountResponseTypeDef TypedDict usage example

from types_aiobotocore_inspector2.type_defs import EnableDelegatedAdminAccountResponseTypeDef


def get_value() -> EnableDelegatedAdminAccountResponseTypeDef:
    return {
        "delegatedAdminAccountId": ...,
    }


# EnableDelegatedAdminAccountResponseTypeDef definition

class EnableDelegatedAdminAccountResponseTypeDef(TypedDict):
    delegatedAdminAccountId: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetCisScanReportResponseTypeDef

```python
# GetCisScanReportResponseTypeDef TypedDict usage example

from types_aiobotocore_inspector2.type_defs import GetCisScanReportResponseTypeDef


def get_value() -> GetCisScanReportResponseTypeDef:
    return {
        "status": ...,
    }


# GetCisScanReportResponseTypeDef definition

class GetCisScanReportResponseTypeDef(TypedDict):
    status: CisReportStatusType,  # (1)
    url: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-brackets: CisReportStatusType](./literals.md#cisreportstatustype) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetEc2DeepInspectionConfigurationResponseTypeDef

```python
# GetEc2DeepInspectionConfigurationResponseTypeDef TypedDict usage example

from types_aiobotocore_inspector2.type_defs import GetEc2DeepInspectionConfigurationResponseTypeDef


def get_value() -> GetEc2DeepInspectionConfigurationResponseTypeDef:
    return {
        "errorMessage": ...,
    }


# GetEc2DeepInspectionConfigurationResponseTypeDef definition

class GetEc2DeepInspectionConfigurationResponseTypeDef(TypedDict):
    errorMessage: str,
    orgPackagePaths: List[str],
    packagePaths: List[str],
    status: Ec2DeepInspectionStatusType,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-brackets: Ec2DeepInspectionStatusType](./literals.md#ec2deepinspectionstatustype) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetEncryptionKeyResponseTypeDef

```python
# GetEncryptionKeyResponseTypeDef TypedDict usage example

from types_aiobotocore_inspector2.type_defs import GetEncryptionKeyResponseTypeDef


def get_value() -> GetEncryptionKeyResponseTypeDef:
    return {
        "kmsKeyId": ...,
    }


# GetEncryptionKeyResponseTypeDef definition

class GetEncryptionKeyResponseTypeDef(TypedDict):
    kmsKeyId: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListTagsForResourceResponseTypeDef

```python
# ListTagsForResourceResponseTypeDef TypedDict usage example

from types_aiobotocore_inspector2.type_defs import ListTagsForResourceResponseTypeDef


def get_value() -> ListTagsForResourceResponseTypeDef:
    return {
        "tags": ...,
    }


# ListTagsForResourceResponseTypeDef definition

class ListTagsForResourceResponseTypeDef(TypedDict):
    tags: Dict[str, str],
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdateCisScanConfigurationResponseTypeDef

```python
# UpdateCisScanConfigurationResponseTypeDef TypedDict usage example

from types_aiobotocore_inspector2.type_defs import UpdateCisScanConfigurationResponseTypeDef


def get_value() -> UpdateCisScanConfigurationResponseTypeDef:
    return {
        "scanConfigurationArn": ...,
    }


# UpdateCisScanConfigurationResponseTypeDef definition

class UpdateCisScanConfigurationResponseTypeDef(TypedDict):
    scanConfigurationArn: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdateEc2DeepInspectionConfigurationResponseTypeDef

```python
# UpdateEc2DeepInspectionConfigurationResponseTypeDef TypedDict usage example

from types_aiobotocore_inspector2.type_defs import UpdateEc2DeepInspectionConfigurationResponseTypeDef


def get_value() -> UpdateEc2DeepInspectionConfigurationResponseTypeDef:
    return {
        "errorMessage": ...,
    }


# UpdateEc2DeepInspectionConfigurationResponseTypeDef definition

class UpdateEc2DeepInspectionConfigurationResponseTypeDef(TypedDict):
    errorMessage: str,
    orgPackagePaths: List[str],
    packagePaths: List[str],
    status: Ec2DeepInspectionStatusType,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-brackets: Ec2DeepInspectionStatusType](./literals.md#ec2deepinspectionstatustype) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdateFilterResponseTypeDef

```python
# UpdateFilterResponseTypeDef TypedDict usage example

from types_aiobotocore_inspector2.type_defs import UpdateFilterResponseTypeDef


def get_value() -> UpdateFilterResponseTypeDef:
    return {
        "arn": ...,
    }


# UpdateFilterResponseTypeDef definition

class UpdateFilterResponseTypeDef(TypedDict):
    arn: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DescribeOrganizationConfigurationResponseTypeDef

```python
# DescribeOrganizationConfigurationResponseTypeDef TypedDict usage example

from types_aiobotocore_inspector2.type_defs import DescribeOrganizationConfigurationResponseTypeDef


def get_value() -> DescribeOrganizationConfigurationResponseTypeDef:
    return {
        "autoEnable": ...,
    }


# DescribeOrganizationConfigurationResponseTypeDef definition

class DescribeOrganizationConfigurationResponseTypeDef(TypedDict):
    autoEnable: AutoEnableTypeDef,  # (1)
    maxAccountLimitReached: bool,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: AutoEnableTypeDef](./type_defs.md#autoenabletypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdateOrganizationConfigurationRequestTypeDef

```python
# UpdateOrganizationConfigurationRequestTypeDef TypedDict usage example

from types_aiobotocore_inspector2.type_defs import UpdateOrganizationConfigurationRequestTypeDef


def get_value() -> UpdateOrganizationConfigurationRequestTypeDef:
    return {
        "autoEnable": ...,
    }


# UpdateOrganizationConfigurationRequestTypeDef definition

class UpdateOrganizationConfigurationRequestTypeDef(TypedDict):
    autoEnable: AutoEnableTypeDef,  # (1)
```

1. See [:material-code-braces: AutoEnableTypeDef](./type_defs.md#autoenabletypedef) 
## UpdateOrganizationConfigurationResponseTypeDef

```python
# UpdateOrganizationConfigurationResponseTypeDef TypedDict usage example

from types_aiobotocore_inspector2.type_defs import UpdateOrganizationConfigurationResponseTypeDef


def get_value() -> UpdateOrganizationConfigurationResponseTypeDef:
    return {
        "autoEnable": ...,
    }


# UpdateOrganizationConfigurationResponseTypeDef definition

class UpdateOrganizationConfigurationResponseTypeDef(TypedDict):
    autoEnable: AutoEnableTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: AutoEnableTypeDef](./type_defs.md#autoenabletypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## AwsLambdaFunctionDetailsTypeDef

```python
# AwsLambdaFunctionDetailsTypeDef TypedDict usage example

from types_aiobotocore_inspector2.type_defs import AwsLambdaFunctionDetailsTypeDef


def get_value() -> AwsLambdaFunctionDetailsTypeDef:
    return {
        "architectures": ...,
    }


# AwsLambdaFunctionDetailsTypeDef definition

class AwsLambdaFunctionDetailsTypeDef(TypedDict):
    codeSha256: str,
    executionRoleArn: str,
    functionName: str,
    runtime: RuntimeType,  # (3)
    version: str,
    architectures: NotRequired[List[ArchitectureType]],  # (1)
    lastModifiedAt: NotRequired[datetime],
    layers: NotRequired[List[str]],
    packageType: NotRequired[PackageTypeType],  # (2)
    vpcConfig: NotRequired[LambdaVpcConfigTypeDef],  # (4)
```

1. See [:material-code-brackets: ArchitectureType](./literals.md#architecturetype) 
2. See [:material-code-brackets: PackageTypeType](./literals.md#packagetypetype) 
3. See [:material-code-brackets: RuntimeType](./literals.md#runtimetype) 
4. See [:material-code-braces: LambdaVpcConfigTypeDef](./type_defs.md#lambdavpcconfigtypedef) 
## BatchGetMemberEc2DeepInspectionStatusResponseTypeDef

```python
# BatchGetMemberEc2DeepInspectionStatusResponseTypeDef TypedDict usage example

from types_aiobotocore_inspector2.type_defs import BatchGetMemberEc2DeepInspectionStatusResponseTypeDef


def get_value() -> BatchGetMemberEc2DeepInspectionStatusResponseTypeDef:
    return {
        "accountIds": ...,
    }


# BatchGetMemberEc2DeepInspectionStatusResponseTypeDef definition

class BatchGetMemberEc2DeepInspectionStatusResponseTypeDef(TypedDict):
    accountIds: List[MemberAccountEc2DeepInspectionStatusStateTypeDef],  # (1)
    failedAccountIds: List[FailedMemberAccountEc2DeepInspectionStatusStateTypeDef],  # (2)
    ResponseMetadata: ResponseMetadataTypeDef,  # (3)
```

1. See [:material-code-braces: MemberAccountEc2DeepInspectionStatusStateTypeDef](./type_defs.md#memberaccountec2deepinspectionstatusstatetypedef) 
2. See [:material-code-braces: FailedMemberAccountEc2DeepInspectionStatusStateTypeDef](./type_defs.md#failedmemberaccountec2deepinspectionstatusstatetypedef) 
3. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## BatchUpdateMemberEc2DeepInspectionStatusResponseTypeDef

```python
# BatchUpdateMemberEc2DeepInspectionStatusResponseTypeDef TypedDict usage example

from types_aiobotocore_inspector2.type_defs import BatchUpdateMemberEc2DeepInspectionStatusResponseTypeDef


def get_value() -> BatchUpdateMemberEc2DeepInspectionStatusResponseTypeDef:
    return {
        "accountIds": ...,
    }


# BatchUpdateMemberEc2DeepInspectionStatusResponseTypeDef definition

class BatchUpdateMemberEc2DeepInspectionStatusResponseTypeDef(TypedDict):
    accountIds: List[MemberAccountEc2DeepInspectionStatusStateTypeDef],  # (1)
    failedAccountIds: List[FailedMemberAccountEc2DeepInspectionStatusStateTypeDef],  # (2)
    ResponseMetadata: ResponseMetadataTypeDef,  # (3)
```

1. See [:material-code-braces: MemberAccountEc2DeepInspectionStatusStateTypeDef](./type_defs.md#memberaccountec2deepinspectionstatusstatetypedef) 
2. See [:material-code-braces: FailedMemberAccountEc2DeepInspectionStatusStateTypeDef](./type_defs.md#failedmemberaccountec2deepinspectionstatusstatetypedef) 
3. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## BatchUpdateMemberEc2DeepInspectionStatusRequestTypeDef

```python
# BatchUpdateMemberEc2DeepInspectionStatusRequestTypeDef TypedDict usage example

from types_aiobotocore_inspector2.type_defs import BatchUpdateMemberEc2DeepInspectionStatusRequestTypeDef


def get_value() -> BatchUpdateMemberEc2DeepInspectionStatusRequestTypeDef:
    return {
        "accountIds": ...,
    }


# BatchUpdateMemberEc2DeepInspectionStatusRequestTypeDef definition

class BatchUpdateMemberEc2DeepInspectionStatusRequestTypeDef(TypedDict):
    accountIds: Sequence[MemberAccountEc2DeepInspectionStatusTypeDef],  # (1)
```

1. See [:material-code-braces: MemberAccountEc2DeepInspectionStatusTypeDef](./type_defs.md#memberaccountec2deepinspectionstatustypedef) 
## CisSessionMessageTypeDef

```python
# CisSessionMessageTypeDef TypedDict usage example

from types_aiobotocore_inspector2.type_defs import CisSessionMessageTypeDef


def get_value() -> CisSessionMessageTypeDef:
    return {
        "cisRuleDetails": ...,
    }


# CisSessionMessageTypeDef definition

class CisSessionMessageTypeDef(TypedDict):
    cisRuleDetails: BlobTypeDef,
    ruleId: str,
    status: CisRuleStatusType,  # (1)
```

1. See [:material-code-brackets: CisRuleStatusType](./literals.md#cisrulestatustype) 
## CisCheckAggregationTypeDef

```python
# CisCheckAggregationTypeDef TypedDict usage example

from types_aiobotocore_inspector2.type_defs import CisCheckAggregationTypeDef


def get_value() -> CisCheckAggregationTypeDef:
    return {
        "accountId": ...,
    }


# CisCheckAggregationTypeDef definition

class CisCheckAggregationTypeDef(TypedDict):
    scanArn: str,
    accountId: NotRequired[str],
    checkDescription: NotRequired[str],
    checkId: NotRequired[str],
    level: NotRequired[CisSecurityLevelType],  # (1)
    platform: NotRequired[str],
    statusCounts: NotRequired[StatusCountsTypeDef],  # (2)
    title: NotRequired[str],
```

1. See [:material-code-brackets: CisSecurityLevelType](./literals.md#cissecurityleveltype) 
2. See [:material-code-braces: StatusCountsTypeDef](./type_defs.md#statuscountstypedef) 
## CisTargetResourceAggregationTypeDef

```python
# CisTargetResourceAggregationTypeDef TypedDict usage example

from types_aiobotocore_inspector2.type_defs import CisTargetResourceAggregationTypeDef


def get_value() -> CisTargetResourceAggregationTypeDef:
    return {
        "accountId": ...,
    }


# CisTargetResourceAggregationTypeDef definition

class CisTargetResourceAggregationTypeDef(TypedDict):
    scanArn: str,
    accountId: NotRequired[str],
    platform: NotRequired[str],
    statusCounts: NotRequired[StatusCountsTypeDef],  # (1)
    targetResourceId: NotRequired[str],
    targetResourceTags: NotRequired[Dict[str, List[str]]],
    targetStatus: NotRequired[CisTargetStatusType],  # (2)
    targetStatusReason: NotRequired[CisTargetStatusReasonType],  # (3)
```

1. See [:material-code-braces: StatusCountsTypeDef](./type_defs.md#statuscountstypedef) 
2. See [:material-code-brackets: CisTargetStatusType](./literals.md#cistargetstatustype) 
3. See [:material-code-brackets: CisTargetStatusReasonType](./literals.md#cistargetstatusreasontype) 
## CisDateFilterTypeDef

```python
# CisDateFilterTypeDef TypedDict usage example

from types_aiobotocore_inspector2.type_defs import CisDateFilterTypeDef


def get_value() -> CisDateFilterTypeDef:
    return {
        "earliestScanStartTime": ...,
    }


# CisDateFilterTypeDef definition

class CisDateFilterTypeDef(TypedDict):
    earliestScanStartTime: NotRequired[TimestampTypeDef],
    latestScanStartTime: NotRequired[TimestampTypeDef],
```

## CoverageDateFilterTypeDef

```python
# CoverageDateFilterTypeDef TypedDict usage example

from types_aiobotocore_inspector2.type_defs import CoverageDateFilterTypeDef


def get_value() -> CoverageDateFilterTypeDef:
    return {
        "endInclusive": ...,
    }


# CoverageDateFilterTypeDef definition

class CoverageDateFilterTypeDef(TypedDict):
    endInclusive: NotRequired[TimestampTypeDef],
    startInclusive: NotRequired[TimestampTypeDef],
```

## DateFilterTypeDef

```python
# DateFilterTypeDef TypedDict usage example

from types_aiobotocore_inspector2.type_defs import DateFilterTypeDef


def get_value() -> DateFilterTypeDef:
    return {
        "endInclusive": ...,
    }


# DateFilterTypeDef definition

class DateFilterTypeDef(TypedDict):
    endInclusive: NotRequired[TimestampTypeDef],
    startInclusive: NotRequired[TimestampTypeDef],
```

## CisScanTypeDef

```python
# CisScanTypeDef TypedDict usage example

from types_aiobotocore_inspector2.type_defs import CisScanTypeDef


def get_value() -> CisScanTypeDef:
    return {
        "failedChecks": ...,
    }


# CisScanTypeDef definition

class CisScanTypeDef(TypedDict):
    scanArn: str,
    scanConfigurationArn: str,
    failedChecks: NotRequired[int],
    scanDate: NotRequired[datetime],
    scanName: NotRequired[str],
    scheduledBy: NotRequired[str],
    securityLevel: NotRequired[CisSecurityLevelType],  # (1)
    status: NotRequired[CisScanStatusType],  # (2)
    targets: NotRequired[CisTargetsTypeDef],  # (3)
    totalChecks: NotRequired[int],
```

1. See [:material-code-brackets: CisSecurityLevelType](./literals.md#cissecurityleveltype) 
2. See [:material-code-brackets: CisScanStatusType](./literals.md#cisscanstatustype) 
3. See [:material-code-braces: CisTargetsTypeDef](./type_defs.md#cistargetstypedef) 
## CisScanResultDetailsFilterCriteriaTypeDef

```python
# CisScanResultDetailsFilterCriteriaTypeDef TypedDict usage example

from types_aiobotocore_inspector2.type_defs import CisScanResultDetailsFilterCriteriaTypeDef


def get_value() -> CisScanResultDetailsFilterCriteriaTypeDef:
    return {
        "checkIdFilters": ...,
    }


# CisScanResultDetailsFilterCriteriaTypeDef definition

class CisScanResultDetailsFilterCriteriaTypeDef(TypedDict):
    checkIdFilters: NotRequired[Sequence[CisStringFilterTypeDef]],  # (1)
    findingArnFilters: NotRequired[Sequence[CisStringFilterTypeDef]],  # (1)
    findingStatusFilters: NotRequired[Sequence[CisFindingStatusFilterTypeDef]],  # (3)
    securityLevelFilters: NotRequired[Sequence[CisSecurityLevelFilterTypeDef]],  # (4)
    titleFilters: NotRequired[Sequence[CisStringFilterTypeDef]],  # (1)
```

1. See [:material-code-braces: CisStringFilterTypeDef](./type_defs.md#cisstringfiltertypedef) 
2. See [:material-code-braces: CisStringFilterTypeDef](./type_defs.md#cisstringfiltertypedef) 
3. See [:material-code-braces: CisFindingStatusFilterTypeDef](./type_defs.md#cisfindingstatusfiltertypedef) 
4. See [:material-code-braces: CisSecurityLevelFilterTypeDef](./type_defs.md#cissecuritylevelfiltertypedef) 
5. See [:material-code-braces: CisStringFilterTypeDef](./type_defs.md#cisstringfiltertypedef) 
## CisScanResultsAggregatedByChecksFilterCriteriaTypeDef

```python
# CisScanResultsAggregatedByChecksFilterCriteriaTypeDef TypedDict usage example

from types_aiobotocore_inspector2.type_defs import CisScanResultsAggregatedByChecksFilterCriteriaTypeDef


def get_value() -> CisScanResultsAggregatedByChecksFilterCriteriaTypeDef:
    return {
        "accountIdFilters": ...,
    }


# CisScanResultsAggregatedByChecksFilterCriteriaTypeDef definition

class CisScanResultsAggregatedByChecksFilterCriteriaTypeDef(TypedDict):
    accountIdFilters: NotRequired[Sequence[CisStringFilterTypeDef]],  # (1)
    checkIdFilters: NotRequired[Sequence[CisStringFilterTypeDef]],  # (1)
    failedResourcesFilters: NotRequired[Sequence[CisNumberFilterTypeDef]],  # (3)
    platformFilters: NotRequired[Sequence[CisStringFilterTypeDef]],  # (1)
    securityLevelFilters: NotRequired[Sequence[CisSecurityLevelFilterTypeDef]],  # (5)
    titleFilters: NotRequired[Sequence[CisStringFilterTypeDef]],  # (1)
```

1. See [:material-code-braces: CisStringFilterTypeDef](./type_defs.md#cisstringfiltertypedef) 
2. See [:material-code-braces: CisStringFilterTypeDef](./type_defs.md#cisstringfiltertypedef) 
3. See [:material-code-braces: CisNumberFilterTypeDef](./type_defs.md#cisnumberfiltertypedef) 
4. See [:material-code-braces: CisStringFilterTypeDef](./type_defs.md#cisstringfiltertypedef) 
5. See [:material-code-braces: CisSecurityLevelFilterTypeDef](./type_defs.md#cissecuritylevelfiltertypedef) 
6. See [:material-code-braces: CisStringFilterTypeDef](./type_defs.md#cisstringfiltertypedef) 
## GetCisScanResultDetailsResponseTypeDef

```python
# GetCisScanResultDetailsResponseTypeDef TypedDict usage example

from types_aiobotocore_inspector2.type_defs import GetCisScanResultDetailsResponseTypeDef


def get_value() -> GetCisScanResultDetailsResponseTypeDef:
    return {
        "nextToken": ...,
    }


# GetCisScanResultDetailsResponseTypeDef definition

class GetCisScanResultDetailsResponseTypeDef(TypedDict):
    scanResultDetails: List[CisScanResultDetailsTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    nextToken: NotRequired[str],
```

1. See [:material-code-braces: CisScanResultDetailsTypeDef](./type_defs.md#cisscanresultdetailstypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CisScanResultsAggregatedByTargetResourceFilterCriteriaTypeDef

```python
# CisScanResultsAggregatedByTargetResourceFilterCriteriaTypeDef TypedDict usage example

from types_aiobotocore_inspector2.type_defs import CisScanResultsAggregatedByTargetResourceFilterCriteriaTypeDef


def get_value() -> CisScanResultsAggregatedByTargetResourceFilterCriteriaTypeDef:
    return {
        "accountIdFilters": ...,
    }


# CisScanResultsAggregatedByTargetResourceFilterCriteriaTypeDef definition

class CisScanResultsAggregatedByTargetResourceFilterCriteriaTypeDef(TypedDict):
    accountIdFilters: NotRequired[Sequence[CisStringFilterTypeDef]],  # (1)
    checkIdFilters: NotRequired[Sequence[CisStringFilterTypeDef]],  # (1)
    failedChecksFilters: NotRequired[Sequence[CisNumberFilterTypeDef]],  # (3)
    platformFilters: NotRequired[Sequence[CisStringFilterTypeDef]],  # (1)
    statusFilters: NotRequired[Sequence[CisResultStatusFilterTypeDef]],  # (5)
    targetResourceIdFilters: NotRequired[Sequence[CisStringFilterTypeDef]],  # (1)
    targetResourceTagFilters: NotRequired[Sequence[TagFilterTypeDef]],  # (7)
    targetStatusFilters: NotRequired[Sequence[CisTargetStatusFilterTypeDef]],  # (8)
    targetStatusReasonFilters: NotRequired[Sequence[CisTargetStatusReasonFilterTypeDef]],  # (9)
```

1. See [:material-code-braces: CisStringFilterTypeDef](./type_defs.md#cisstringfiltertypedef) 
2. See [:material-code-braces: CisStringFilterTypeDef](./type_defs.md#cisstringfiltertypedef) 
3. See [:material-code-braces: CisNumberFilterTypeDef](./type_defs.md#cisnumberfiltertypedef) 
4. See [:material-code-braces: CisStringFilterTypeDef](./type_defs.md#cisstringfiltertypedef) 
5. See [:material-code-braces: CisResultStatusFilterTypeDef](./type_defs.md#cisresultstatusfiltertypedef) 
6. See [:material-code-braces: CisStringFilterTypeDef](./type_defs.md#cisstringfiltertypedef) 
7. See [:material-code-braces: TagFilterTypeDef](./type_defs.md#tagfiltertypedef) 
8. See [:material-code-braces: CisTargetStatusFilterTypeDef](./type_defs.md#cistargetstatusfiltertypedef) 
9. See [:material-code-braces: CisTargetStatusReasonFilterTypeDef](./type_defs.md#cistargetstatusreasonfiltertypedef) 
## ListCisScanConfigurationsFilterCriteriaTypeDef

```python
# ListCisScanConfigurationsFilterCriteriaTypeDef TypedDict usage example

from types_aiobotocore_inspector2.type_defs import ListCisScanConfigurationsFilterCriteriaTypeDef


def get_value() -> ListCisScanConfigurationsFilterCriteriaTypeDef:
    return {
        "scanConfigurationArnFilters": ...,
    }


# ListCisScanConfigurationsFilterCriteriaTypeDef definition

class ListCisScanConfigurationsFilterCriteriaTypeDef(TypedDict):
    scanConfigurationArnFilters: NotRequired[Sequence[CisStringFilterTypeDef]],  # (1)
    scanNameFilters: NotRequired[Sequence[CisStringFilterTypeDef]],  # (1)
    targetResourceTagFilters: NotRequired[Sequence[TagFilterTypeDef]],  # (3)
```

1. See [:material-code-braces: CisStringFilterTypeDef](./type_defs.md#cisstringfiltertypedef) 
2. See [:material-code-braces: CisStringFilterTypeDef](./type_defs.md#cisstringfiltertypedef) 
3. See [:material-code-braces: TagFilterTypeDef](./type_defs.md#tagfiltertypedef) 
## CodeVulnerabilityDetailsTypeDef

```python
# CodeVulnerabilityDetailsTypeDef TypedDict usage example

from types_aiobotocore_inspector2.type_defs import CodeVulnerabilityDetailsTypeDef


def get_value() -> CodeVulnerabilityDetailsTypeDef:
    return {
        "cwes": ...,
    }


# CodeVulnerabilityDetailsTypeDef definition

class CodeVulnerabilityDetailsTypeDef(TypedDict):
    cwes: List[str],
    detectorId: str,
    detectorName: str,
    filePath: CodeFilePathTypeDef,  # (1)
    detectorTags: NotRequired[List[str]],
    referenceUrls: NotRequired[List[str]],
    ruleId: NotRequired[str],
    sourceLambdaLayerArn: NotRequired[str],
```

1. See [:material-code-braces: CodeFilePathTypeDef](./type_defs.md#codefilepathtypedef) 
## CodeSnippetResultTypeDef

```python
# CodeSnippetResultTypeDef TypedDict usage example

from types_aiobotocore_inspector2.type_defs import CodeSnippetResultTypeDef


def get_value() -> CodeSnippetResultTypeDef:
    return {
        "codeSnippet": ...,
    }


# CodeSnippetResultTypeDef definition

class CodeSnippetResultTypeDef(TypedDict):
    codeSnippet: NotRequired[List[CodeLineTypeDef]],  # (1)
    endLine: NotRequired[int],
    findingArn: NotRequired[str],
    startLine: NotRequired[int],
    suggestedFixes: NotRequired[List[SuggestedFixTypeDef]],  # (2)
```

1. See [:material-code-braces: CodeLineTypeDef](./type_defs.md#codelinetypedef) 
2. See [:material-code-braces: SuggestedFixTypeDef](./type_defs.md#suggestedfixtypedef) 
## ListCoverageStatisticsResponseTypeDef

```python
# ListCoverageStatisticsResponseTypeDef TypedDict usage example

from types_aiobotocore_inspector2.type_defs import ListCoverageStatisticsResponseTypeDef


def get_value() -> ListCoverageStatisticsResponseTypeDef:
    return {
        "countsByGroup": ...,
    }


# ListCoverageStatisticsResponseTypeDef definition

class ListCoverageStatisticsResponseTypeDef(TypedDict):
    countsByGroup: List[CountsTypeDef],  # (1)
    totalCounts: int,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    nextToken: NotRequired[str],
```

1. See [:material-code-braces: CountsTypeDef](./type_defs.md#countstypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CvssScoreDetailsTypeDef

```python
# CvssScoreDetailsTypeDef TypedDict usage example

from types_aiobotocore_inspector2.type_defs import CvssScoreDetailsTypeDef


def get_value() -> CvssScoreDetailsTypeDef:
    return {
        "adjustments": ...,
    }


# CvssScoreDetailsTypeDef definition

class CvssScoreDetailsTypeDef(TypedDict):
    score: float,
    scoreSource: str,
    scoringVector: str,
    version: str,
    adjustments: NotRequired[List[CvssScoreAdjustmentTypeDef]],  # (1)
    cvssSource: NotRequired[str],
```

1. See [:material-code-braces: CvssScoreAdjustmentTypeDef](./type_defs.md#cvssscoreadjustmenttypedef) 
## DailyScheduleTypeDef

```python
# DailyScheduleTypeDef TypedDict usage example

from types_aiobotocore_inspector2.type_defs import DailyScheduleTypeDef


def get_value() -> DailyScheduleTypeDef:
    return {
        "startTime": ...,
    }


# DailyScheduleTypeDef definition

class DailyScheduleTypeDef(TypedDict):
    startTime: TimeTypeDef,  # (1)
```

1. See [:material-code-braces: TimeTypeDef](./type_defs.md#timetypedef) 
## MonthlyScheduleTypeDef

```python
# MonthlyScheduleTypeDef TypedDict usage example

from types_aiobotocore_inspector2.type_defs import MonthlyScheduleTypeDef


def get_value() -> MonthlyScheduleTypeDef:
    return {
        "day": ...,
    }


# MonthlyScheduleTypeDef definition

class MonthlyScheduleTypeDef(TypedDict):
    day: DayType,  # (1)
    startTime: TimeTypeDef,  # (2)
```

1. See [:material-code-brackets: DayType](./literals.md#daytype) 
2. See [:material-code-braces: TimeTypeDef](./type_defs.md#timetypedef) 
## WeeklyScheduleOutputTypeDef

```python
# WeeklyScheduleOutputTypeDef TypedDict usage example

from types_aiobotocore_inspector2.type_defs import WeeklyScheduleOutputTypeDef


def get_value() -> WeeklyScheduleOutputTypeDef:
    return {
        "days": ...,
    }


# WeeklyScheduleOutputTypeDef definition

class WeeklyScheduleOutputTypeDef(TypedDict):
    days: List[DayType],  # (1)
    startTime: TimeTypeDef,  # (2)
```

1. See [:material-code-brackets: DayType](./literals.md#daytype) 
2. See [:material-code-braces: TimeTypeDef](./type_defs.md#timetypedef) 
## WeeklyScheduleTypeDef

```python
# WeeklyScheduleTypeDef TypedDict usage example

from types_aiobotocore_inspector2.type_defs import WeeklyScheduleTypeDef


def get_value() -> WeeklyScheduleTypeDef:
    return {
        "days": ...,
    }


# WeeklyScheduleTypeDef definition

class WeeklyScheduleTypeDef(TypedDict):
    days: Sequence[DayType],  # (1)
    startTime: TimeTypeDef,  # (2)
```

1. See [:material-code-brackets: DayType](./literals.md#daytype) 
2. See [:material-code-braces: TimeTypeDef](./type_defs.md#timetypedef) 
## ListDelegatedAdminAccountsResponseTypeDef

```python
# ListDelegatedAdminAccountsResponseTypeDef TypedDict usage example

from types_aiobotocore_inspector2.type_defs import ListDelegatedAdminAccountsResponseTypeDef


def get_value() -> ListDelegatedAdminAccountsResponseTypeDef:
    return {
        "delegatedAdminAccounts": ...,
    }


# ListDelegatedAdminAccountsResponseTypeDef definition

class ListDelegatedAdminAccountsResponseTypeDef(TypedDict):
    delegatedAdminAccounts: List[DelegatedAdminAccountTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    nextToken: NotRequired[str],
```

1. See [:material-code-braces: DelegatedAdminAccountTypeDef](./type_defs.md#delegatedadminaccounttypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetDelegatedAdminAccountResponseTypeDef

```python
# GetDelegatedAdminAccountResponseTypeDef TypedDict usage example

from types_aiobotocore_inspector2.type_defs import GetDelegatedAdminAccountResponseTypeDef


def get_value() -> GetDelegatedAdminAccountResponseTypeDef:
    return {
        "delegatedAdmin": ...,
    }


# GetDelegatedAdminAccountResponseTypeDef definition

class GetDelegatedAdminAccountResponseTypeDef(TypedDict):
    delegatedAdmin: DelegatedAdminTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: DelegatedAdminTypeDef](./type_defs.md#delegatedadmintypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## Ec2ConfigurationStateTypeDef

```python
# Ec2ConfigurationStateTypeDef TypedDict usage example

from types_aiobotocore_inspector2.type_defs import Ec2ConfigurationStateTypeDef


def get_value() -> Ec2ConfigurationStateTypeDef:
    return {
        "scanModeState": ...,
    }


# Ec2ConfigurationStateTypeDef definition

class Ec2ConfigurationStateTypeDef(TypedDict):
    scanModeState: NotRequired[Ec2ScanModeStateTypeDef],  # (1)
```

1. See [:material-code-braces: Ec2ScanModeStateTypeDef](./type_defs.md#ec2scanmodestatetypedef) 
## Ec2InstanceAggregationTypeDef

```python
# Ec2InstanceAggregationTypeDef TypedDict usage example

from types_aiobotocore_inspector2.type_defs import Ec2InstanceAggregationTypeDef


def get_value() -> Ec2InstanceAggregationTypeDef:
    return {
        "amis": ...,
    }


# Ec2InstanceAggregationTypeDef definition

class Ec2InstanceAggregationTypeDef(TypedDict):
    amis: NotRequired[Sequence[StringFilterTypeDef]],  # (1)
    instanceIds: NotRequired[Sequence[StringFilterTypeDef]],  # (1)
    instanceTags: NotRequired[Sequence[MapFilterTypeDef]],  # (3)
    operatingSystems: NotRequired[Sequence[StringFilterTypeDef]],  # (1)
    sortBy: NotRequired[Ec2InstanceSortByType],  # (5)
    sortOrder: NotRequired[SortOrderType],  # (6)
```

1. See [:material-code-braces: StringFilterTypeDef](./type_defs.md#stringfiltertypedef) 
2. See [:material-code-braces: StringFilterTypeDef](./type_defs.md#stringfiltertypedef) 
3. See [:material-code-braces: MapFilterTypeDef](./type_defs.md#mapfiltertypedef) 
4. See [:material-code-braces: StringFilterTypeDef](./type_defs.md#stringfiltertypedef) 
5. See [:material-code-brackets: Ec2InstanceSortByType](./literals.md#ec2instancesortbytype) 
6. See [:material-code-brackets: SortOrderType](./literals.md#sortordertype) 
## LambdaFunctionAggregationTypeDef

```python
# LambdaFunctionAggregationTypeDef TypedDict usage example

from types_aiobotocore_inspector2.type_defs import LambdaFunctionAggregationTypeDef


def get_value() -> LambdaFunctionAggregationTypeDef:
    return {
        "functionNames": ...,
    }


# LambdaFunctionAggregationTypeDef definition

class LambdaFunctionAggregationTypeDef(TypedDict):
    functionNames: NotRequired[Sequence[StringFilterTypeDef]],  # (1)
    functionTags: NotRequired[Sequence[MapFilterTypeDef]],  # (2)
    resourceIds: NotRequired[Sequence[StringFilterTypeDef]],  # (1)
    runtimes: NotRequired[Sequence[StringFilterTypeDef]],  # (1)
    sortBy: NotRequired[LambdaFunctionSortByType],  # (5)
    sortOrder: NotRequired[SortOrderType],  # (6)
```

1. See [:material-code-braces: StringFilterTypeDef](./type_defs.md#stringfiltertypedef) 
2. See [:material-code-braces: MapFilterTypeDef](./type_defs.md#mapfiltertypedef) 
3. See [:material-code-braces: StringFilterTypeDef](./type_defs.md#stringfiltertypedef) 
4. See [:material-code-braces: StringFilterTypeDef](./type_defs.md#stringfiltertypedef) 
5. See [:material-code-brackets: LambdaFunctionSortByType](./literals.md#lambdafunctionsortbytype) 
6. See [:material-code-brackets: SortOrderType](./literals.md#sortordertype) 
## EcrConfigurationStateTypeDef

```python
# EcrConfigurationStateTypeDef TypedDict usage example

from types_aiobotocore_inspector2.type_defs import EcrConfigurationStateTypeDef


def get_value() -> EcrConfigurationStateTypeDef:
    return {
        "rescanDurationState": ...,
    }


# EcrConfigurationStateTypeDef definition

class EcrConfigurationStateTypeDef(TypedDict):
    rescanDurationState: NotRequired[EcrRescanDurationStateTypeDef],  # (1)
```

1. See [:material-code-braces: EcrRescanDurationStateTypeDef](./type_defs.md#ecrrescandurationstatetypedef) 
## UpdateConfigurationRequestTypeDef

```python
# UpdateConfigurationRequestTypeDef TypedDict usage example

from types_aiobotocore_inspector2.type_defs import UpdateConfigurationRequestTypeDef


def get_value() -> UpdateConfigurationRequestTypeDef:
    return {
        "ec2Configuration": ...,
    }


# UpdateConfigurationRequestTypeDef definition

class UpdateConfigurationRequestTypeDef(TypedDict):
    ec2Configuration: NotRequired[Ec2ConfigurationTypeDef],  # (1)
    ecrConfiguration: NotRequired[EcrConfigurationTypeDef],  # (2)
```

1. See [:material-code-braces: Ec2ConfigurationTypeDef](./type_defs.md#ec2configurationtypedef) 
2. See [:material-code-braces: EcrConfigurationTypeDef](./type_defs.md#ecrconfigurationtypedef) 
## FindingDetailTypeDef

```python
# FindingDetailTypeDef TypedDict usage example

from types_aiobotocore_inspector2.type_defs import FindingDetailTypeDef


def get_value() -> FindingDetailTypeDef:
    return {
        "cisaData": ...,
    }


# FindingDetailTypeDef definition

class FindingDetailTypeDef(TypedDict):
    cisaData: NotRequired[CisaDataTypeDef],  # (1)
    cwes: NotRequired[List[str]],
    epssScore: NotRequired[float],
    evidences: NotRequired[List[EvidenceTypeDef]],  # (2)
    exploitObserved: NotRequired[ExploitObservedTypeDef],  # (3)
    findingArn: NotRequired[str],
    referenceUrls: NotRequired[List[str]],
    riskScore: NotRequired[int],
    tools: NotRequired[List[str]],
    ttps: NotRequired[List[str]],
```

1. See [:material-code-braces: CisaDataTypeDef](./type_defs.md#cisadatatypedef) 
2. See [:material-code-braces: EvidenceTypeDef](./type_defs.md#evidencetypedef) 
3. See [:material-code-braces: ExploitObservedTypeDef](./type_defs.md#exploitobservedtypedef) 
## VulnerabilityTypeDef

```python
# VulnerabilityTypeDef TypedDict usage example

from types_aiobotocore_inspector2.type_defs import VulnerabilityTypeDef


def get_value() -> VulnerabilityTypeDef:
    return {
        "atigData": ...,
    }


# VulnerabilityTypeDef definition

class VulnerabilityTypeDef(TypedDict):
    id: str,
    atigData: NotRequired[AtigDataTypeDef],  # (1)
    cisaData: NotRequired[CisaDataTypeDef],  # (2)
    cvss2: NotRequired[Cvss2TypeDef],  # (3)
    cvss3: NotRequired[Cvss3TypeDef],  # (4)
    cwes: NotRequired[List[str]],
    description: NotRequired[str],
    detectionPlatforms: NotRequired[List[str]],
    epss: NotRequired[EpssTypeDef],  # (5)
    exploitObserved: NotRequired[ExploitObservedTypeDef],  # (6)
    referenceUrls: NotRequired[List[str]],
    relatedVulnerabilities: NotRequired[List[str]],
    source: NotRequired[VulnerabilitySourceType],  # (7)
    sourceUrl: NotRequired[str],
    vendorCreatedAt: NotRequired[datetime],
    vendorSeverity: NotRequired[str],
    vendorUpdatedAt: NotRequired[datetime],
```

1. See [:material-code-braces: AtigDataTypeDef](./type_defs.md#atigdatatypedef) 
2. See [:material-code-braces: CisaDataTypeDef](./type_defs.md#cisadatatypedef) 
3. See [:material-code-braces: Cvss2TypeDef](./type_defs.md#cvss2typedef) 
4. See [:material-code-braces: Cvss3TypeDef](./type_defs.md#cvss3typedef) 
5. See [:material-code-braces: EpssTypeDef](./type_defs.md#epsstypedef) 
6. See [:material-code-braces: ExploitObservedTypeDef](./type_defs.md#exploitobservedtypedef) 
7. See [:material-code-brackets: VulnerabilitySourceType](./literals.md#vulnerabilitysourcetype) 
## PackageFilterTypeDef

```python
# PackageFilterTypeDef TypedDict usage example

from types_aiobotocore_inspector2.type_defs import PackageFilterTypeDef


def get_value() -> PackageFilterTypeDef:
    return {
        "architecture": ...,
    }


# PackageFilterTypeDef definition

class PackageFilterTypeDef(TypedDict):
    architecture: NotRequired[StringFilterTypeDef],  # (1)
    epoch: NotRequired[NumberFilterTypeDef],  # (2)
    filePath: NotRequired[StringFilterTypeDef],  # (1)
    name: NotRequired[StringFilterTypeDef],  # (1)
    release: NotRequired[StringFilterTypeDef],  # (1)
    sourceLambdaLayerArn: NotRequired[StringFilterTypeDef],  # (1)
    sourceLayerHash: NotRequired[StringFilterTypeDef],  # (1)
    version: NotRequired[StringFilterTypeDef],  # (1)
```

1. See [:material-code-braces: StringFilterTypeDef](./type_defs.md#stringfiltertypedef) 
2. See [:material-code-braces: NumberFilterTypeDef](./type_defs.md#numberfiltertypedef) 
3. See [:material-code-braces: StringFilterTypeDef](./type_defs.md#stringfiltertypedef) 
4. See [:material-code-braces: StringFilterTypeDef](./type_defs.md#stringfiltertypedef) 
5. See [:material-code-braces: StringFilterTypeDef](./type_defs.md#stringfiltertypedef) 
6. See [:material-code-braces: StringFilterTypeDef](./type_defs.md#stringfiltertypedef) 
7. See [:material-code-braces: StringFilterTypeDef](./type_defs.md#stringfiltertypedef) 
8. See [:material-code-braces: StringFilterTypeDef](./type_defs.md#stringfiltertypedef) 
## FreeTrialAccountInfoTypeDef

```python
# FreeTrialAccountInfoTypeDef TypedDict usage example

from types_aiobotocore_inspector2.type_defs import FreeTrialAccountInfoTypeDef


def get_value() -> FreeTrialAccountInfoTypeDef:
    return {
        "accountId": ...,
    }


# FreeTrialAccountInfoTypeDef definition

class FreeTrialAccountInfoTypeDef(TypedDict):
    accountId: str,
    freeTrialInfo: List[FreeTrialInfoTypeDef],  # (1)
```

1. See [:material-code-braces: FreeTrialInfoTypeDef](./type_defs.md#freetrialinfotypedef) 
## ListAccountPermissionsRequestPaginateTypeDef

```python
# ListAccountPermissionsRequestPaginateTypeDef TypedDict usage example

from types_aiobotocore_inspector2.type_defs import ListAccountPermissionsRequestPaginateTypeDef


def get_value() -> ListAccountPermissionsRequestPaginateTypeDef:
    return {
        "service": ...,
    }


# ListAccountPermissionsRequestPaginateTypeDef definition

class ListAccountPermissionsRequestPaginateTypeDef(TypedDict):
    service: NotRequired[ServiceType],  # (1)
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (2)
```

1. See [:material-code-brackets: ServiceType](./literals.md#servicetype) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListDelegatedAdminAccountsRequestPaginateTypeDef

```python
# ListDelegatedAdminAccountsRequestPaginateTypeDef TypedDict usage example

from types_aiobotocore_inspector2.type_defs import ListDelegatedAdminAccountsRequestPaginateTypeDef


def get_value() -> ListDelegatedAdminAccountsRequestPaginateTypeDef:
    return {
        "PaginationConfig": ...,
    }


# ListDelegatedAdminAccountsRequestPaginateTypeDef definition

class ListDelegatedAdminAccountsRequestPaginateTypeDef(TypedDict):
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListFiltersRequestPaginateTypeDef

```python
# ListFiltersRequestPaginateTypeDef TypedDict usage example

from types_aiobotocore_inspector2.type_defs import ListFiltersRequestPaginateTypeDef


def get_value() -> ListFiltersRequestPaginateTypeDef:
    return {
        "action": ...,
    }


# ListFiltersRequestPaginateTypeDef definition

class ListFiltersRequestPaginateTypeDef(TypedDict):
    action: NotRequired[FilterActionType],  # (1)
    arns: NotRequired[Sequence[str]],
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (2)
```

1. See [:material-code-brackets: FilterActionType](./literals.md#filteractiontype) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListMembersRequestPaginateTypeDef

```python
# ListMembersRequestPaginateTypeDef TypedDict usage example

from types_aiobotocore_inspector2.type_defs import ListMembersRequestPaginateTypeDef


def get_value() -> ListMembersRequestPaginateTypeDef:
    return {
        "onlyAssociated": ...,
    }


# ListMembersRequestPaginateTypeDef definition

class ListMembersRequestPaginateTypeDef(TypedDict):
    onlyAssociated: NotRequired[bool],
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListUsageTotalsRequestPaginateTypeDef

```python
# ListUsageTotalsRequestPaginateTypeDef TypedDict usage example

from types_aiobotocore_inspector2.type_defs import ListUsageTotalsRequestPaginateTypeDef


def get_value() -> ListUsageTotalsRequestPaginateTypeDef:
    return {
        "accountIds": ...,
    }


# ListUsageTotalsRequestPaginateTypeDef definition

class ListUsageTotalsRequestPaginateTypeDef(TypedDict):
    accountIds: NotRequired[Sequence[str]],
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## GetMemberResponseTypeDef

```python
# GetMemberResponseTypeDef TypedDict usage example

from types_aiobotocore_inspector2.type_defs import GetMemberResponseTypeDef


def get_value() -> GetMemberResponseTypeDef:
    return {
        "member": ...,
    }


# GetMemberResponseTypeDef definition

class GetMemberResponseTypeDef(TypedDict):
    member: MemberTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: MemberTypeDef](./type_defs.md#membertypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListMembersResponseTypeDef

```python
# ListMembersResponseTypeDef TypedDict usage example

from types_aiobotocore_inspector2.type_defs import ListMembersResponseTypeDef


def get_value() -> ListMembersResponseTypeDef:
    return {
        "members": ...,
    }


# ListMembersResponseTypeDef definition

class ListMembersResponseTypeDef(TypedDict):
    members: List[MemberTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    nextToken: NotRequired[str],
```

1. See [:material-code-braces: MemberTypeDef](./type_defs.md#membertypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ResourceScanMetadataTypeDef

```python
# ResourceScanMetadataTypeDef TypedDict usage example

from types_aiobotocore_inspector2.type_defs import ResourceScanMetadataTypeDef


def get_value() -> ResourceScanMetadataTypeDef:
    return {
        "ec2": ...,
    }


# ResourceScanMetadataTypeDef definition

class ResourceScanMetadataTypeDef(TypedDict):
    ec2: NotRequired[Ec2MetadataTypeDef],  # (1)
    ecrImage: NotRequired[EcrContainerImageMetadataTypeDef],  # (2)
    ecrRepository: NotRequired[EcrRepositoryMetadataTypeDef],  # (3)
    lambdaFunction: NotRequired[LambdaFunctionMetadataTypeDef],  # (4)
```

1. See [:material-code-braces: Ec2MetadataTypeDef](./type_defs.md#ec2metadatatypedef) 
2. See [:material-code-braces: EcrContainerImageMetadataTypeDef](./type_defs.md#ecrcontainerimagemetadatatypedef) 
3. See [:material-code-braces: EcrRepositoryMetadataTypeDef](./type_defs.md#ecrrepositorymetadatatypedef) 
4. See [:material-code-braces: LambdaFunctionMetadataTypeDef](./type_defs.md#lambdafunctionmetadatatypedef) 
## ListAccountPermissionsResponseTypeDef

```python
# ListAccountPermissionsResponseTypeDef TypedDict usage example

from types_aiobotocore_inspector2.type_defs import ListAccountPermissionsResponseTypeDef


def get_value() -> ListAccountPermissionsResponseTypeDef:
    return {
        "nextToken": ...,
    }


# ListAccountPermissionsResponseTypeDef definition

class ListAccountPermissionsResponseTypeDef(TypedDict):
    permissions: List[PermissionTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    nextToken: NotRequired[str],
```

1. See [:material-code-braces: PermissionTypeDef](./type_defs.md#permissiontypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## NetworkPathTypeDef

```python
# NetworkPathTypeDef TypedDict usage example

from types_aiobotocore_inspector2.type_defs import NetworkPathTypeDef


def get_value() -> NetworkPathTypeDef:
    return {
        "steps": ...,
    }


# NetworkPathTypeDef definition

class NetworkPathTypeDef(TypedDict):
    steps: NotRequired[List[StepTypeDef]],  # (1)
```

1. See [:material-code-braces: StepTypeDef](./type_defs.md#steptypedef) 
## PackageVulnerabilityDetailsTypeDef

```python
# PackageVulnerabilityDetailsTypeDef TypedDict usage example

from types_aiobotocore_inspector2.type_defs import PackageVulnerabilityDetailsTypeDef


def get_value() -> PackageVulnerabilityDetailsTypeDef:
    return {
        "cvss": ...,
    }


# PackageVulnerabilityDetailsTypeDef definition

class PackageVulnerabilityDetailsTypeDef(TypedDict):
    source: str,
    vulnerabilityId: str,
    cvss: NotRequired[List[CvssScoreTypeDef]],  # (1)
    referenceUrls: NotRequired[List[str]],
    relatedVulnerabilities: NotRequired[List[str]],
    sourceUrl: NotRequired[str],
    vendorCreatedAt: NotRequired[datetime],
    vendorSeverity: NotRequired[str],
    vendorUpdatedAt: NotRequired[datetime],
    vulnerablePackages: NotRequired[List[VulnerablePackageTypeDef]],  # (2)
```

1. See [:material-code-braces: CvssScoreTypeDef](./type_defs.md#cvssscoretypedef) 
2. See [:material-code-braces: VulnerablePackageTypeDef](./type_defs.md#vulnerablepackagetypedef) 
## RemediationTypeDef

```python
# RemediationTypeDef TypedDict usage example

from types_aiobotocore_inspector2.type_defs import RemediationTypeDef


def get_value() -> RemediationTypeDef:
    return {
        "recommendation": ...,
    }


# RemediationTypeDef definition

class RemediationTypeDef(TypedDict):
    recommendation: NotRequired[RecommendationTypeDef],  # (1)
```

1. See [:material-code-braces: RecommendationTypeDef](./type_defs.md#recommendationtypedef) 
## ResourceFilterCriteriaOutputTypeDef

```python
# ResourceFilterCriteriaOutputTypeDef TypedDict usage example

from types_aiobotocore_inspector2.type_defs import ResourceFilterCriteriaOutputTypeDef


def get_value() -> ResourceFilterCriteriaOutputTypeDef:
    return {
        "accountId": ...,
    }


# ResourceFilterCriteriaOutputTypeDef definition

class ResourceFilterCriteriaOutputTypeDef(TypedDict):
    accountId: NotRequired[List[ResourceStringFilterTypeDef]],  # (1)
    ec2InstanceTags: NotRequired[List[ResourceMapFilterTypeDef]],  # (2)
    ecrImageTags: NotRequired[List[ResourceStringFilterTypeDef]],  # (1)
    ecrRepositoryName: NotRequired[List[ResourceStringFilterTypeDef]],  # (1)
    lambdaFunctionName: NotRequired[List[ResourceStringFilterTypeDef]],  # (1)
    lambdaFunctionTags: NotRequired[List[ResourceMapFilterTypeDef]],  # (2)
    resourceId: NotRequired[List[ResourceStringFilterTypeDef]],  # (1)
    resourceType: NotRequired[List[ResourceStringFilterTypeDef]],  # (1)
```

1. See [:material-code-braces: ResourceStringFilterTypeDef](./type_defs.md#resourcestringfiltertypedef) 
2. See [:material-code-braces: ResourceMapFilterTypeDef](./type_defs.md#resourcemapfiltertypedef) 
3. See [:material-code-braces: ResourceStringFilterTypeDef](./type_defs.md#resourcestringfiltertypedef) 
4. See [:material-code-braces: ResourceStringFilterTypeDef](./type_defs.md#resourcestringfiltertypedef) 
5. See [:material-code-braces: ResourceStringFilterTypeDef](./type_defs.md#resourcestringfiltertypedef) 
6. See [:material-code-braces: ResourceMapFilterTypeDef](./type_defs.md#resourcemapfiltertypedef) 
7. See [:material-code-braces: ResourceStringFilterTypeDef](./type_defs.md#resourcestringfiltertypedef) 
8. See [:material-code-braces: ResourceStringFilterTypeDef](./type_defs.md#resourcestringfiltertypedef) 
## ResourceFilterCriteriaTypeDef

```python
# ResourceFilterCriteriaTypeDef TypedDict usage example

from types_aiobotocore_inspector2.type_defs import ResourceFilterCriteriaTypeDef


def get_value() -> ResourceFilterCriteriaTypeDef:
    return {
        "accountId": ...,
    }


# ResourceFilterCriteriaTypeDef definition

class ResourceFilterCriteriaTypeDef(TypedDict):
    accountId: NotRequired[Sequence[ResourceStringFilterTypeDef]],  # (1)
    ec2InstanceTags: NotRequired[Sequence[ResourceMapFilterTypeDef]],  # (2)
    ecrImageTags: NotRequired[Sequence[ResourceStringFilterTypeDef]],  # (1)
    ecrRepositoryName: NotRequired[Sequence[ResourceStringFilterTypeDef]],  # (1)
    lambdaFunctionName: NotRequired[Sequence[ResourceStringFilterTypeDef]],  # (1)
    lambdaFunctionTags: NotRequired[Sequence[ResourceMapFilterTypeDef]],  # (2)
    resourceId: NotRequired[Sequence[ResourceStringFilterTypeDef]],  # (1)
    resourceType: NotRequired[Sequence[ResourceStringFilterTypeDef]],  # (1)
```

1. See [:material-code-braces: ResourceStringFilterTypeDef](./type_defs.md#resourcestringfiltertypedef) 
2. See [:material-code-braces: ResourceMapFilterTypeDef](./type_defs.md#resourcemapfiltertypedef) 
3. See [:material-code-braces: ResourceStringFilterTypeDef](./type_defs.md#resourcestringfiltertypedef) 
4. See [:material-code-braces: ResourceStringFilterTypeDef](./type_defs.md#resourcestringfiltertypedef) 
5. See [:material-code-braces: ResourceStringFilterTypeDef](./type_defs.md#resourcestringfiltertypedef) 
6. See [:material-code-braces: ResourceMapFilterTypeDef](./type_defs.md#resourcemapfiltertypedef) 
7. See [:material-code-braces: ResourceStringFilterTypeDef](./type_defs.md#resourcestringfiltertypedef) 
8. See [:material-code-braces: ResourceStringFilterTypeDef](./type_defs.md#resourcestringfiltertypedef) 
## SearchVulnerabilitiesRequestPaginateTypeDef

```python
# SearchVulnerabilitiesRequestPaginateTypeDef TypedDict usage example

from types_aiobotocore_inspector2.type_defs import SearchVulnerabilitiesRequestPaginateTypeDef


def get_value() -> SearchVulnerabilitiesRequestPaginateTypeDef:
    return {
        "filterCriteria": ...,
    }


# SearchVulnerabilitiesRequestPaginateTypeDef definition

class SearchVulnerabilitiesRequestPaginateTypeDef(TypedDict):
    filterCriteria: SearchVulnerabilitiesFilterCriteriaTypeDef,  # (1)
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (2)
```

1. See [:material-code-braces: SearchVulnerabilitiesFilterCriteriaTypeDef](./type_defs.md#searchvulnerabilitiesfiltercriteriatypedef) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## SearchVulnerabilitiesRequestTypeDef

```python
# SearchVulnerabilitiesRequestTypeDef TypedDict usage example

from types_aiobotocore_inspector2.type_defs import SearchVulnerabilitiesRequestTypeDef


def get_value() -> SearchVulnerabilitiesRequestTypeDef:
    return {
        "filterCriteria": ...,
    }


# SearchVulnerabilitiesRequestTypeDef definition

class SearchVulnerabilitiesRequestTypeDef(TypedDict):
    filterCriteria: SearchVulnerabilitiesFilterCriteriaTypeDef,  # (1)
    nextToken: NotRequired[str],
```

1. See [:material-code-braces: SearchVulnerabilitiesFilterCriteriaTypeDef](./type_defs.md#searchvulnerabilitiesfiltercriteriatypedef) 
## StartCisSessionRequestTypeDef

```python
# StartCisSessionRequestTypeDef TypedDict usage example

from types_aiobotocore_inspector2.type_defs import StartCisSessionRequestTypeDef


def get_value() -> StartCisSessionRequestTypeDef:
    return {
        "message": ...,
    }


# StartCisSessionRequestTypeDef definition

class StartCisSessionRequestTypeDef(TypedDict):
    message: StartCisSessionMessageTypeDef,  # (1)
    scanJobId: str,
```

1. See [:material-code-braces: StartCisSessionMessageTypeDef](./type_defs.md#startcissessionmessagetypedef) 
## StopCisSessionMessageTypeDef

```python
# StopCisSessionMessageTypeDef TypedDict usage example

from types_aiobotocore_inspector2.type_defs import StopCisSessionMessageTypeDef


def get_value() -> StopCisSessionMessageTypeDef:
    return {
        "benchmarkProfile": ...,
    }


# StopCisSessionMessageTypeDef definition

class StopCisSessionMessageTypeDef(TypedDict):
    progress: StopCisMessageProgressTypeDef,  # (2)
    status: StopCisSessionStatusType,  # (3)
    benchmarkProfile: NotRequired[str],
    benchmarkVersion: NotRequired[str],
    computePlatform: NotRequired[ComputePlatformTypeDef],  # (1)
    reason: NotRequired[str],
```

1. See [:material-code-braces: ComputePlatformTypeDef](./type_defs.md#computeplatformtypedef) 
2. See [:material-code-braces: StopCisMessageProgressTypeDef](./type_defs.md#stopcismessageprogresstypedef) 
3. See [:material-code-brackets: StopCisSessionStatusType](./literals.md#stopcissessionstatustype) 
## UsageTotalTypeDef

```python
# UsageTotalTypeDef TypedDict usage example

from types_aiobotocore_inspector2.type_defs import UsageTotalTypeDef


def get_value() -> UsageTotalTypeDef:
    return {
        "accountId": ...,
    }


# UsageTotalTypeDef definition

class UsageTotalTypeDef(TypedDict):
    accountId: NotRequired[str],
    usage: NotRequired[List[UsageTypeDef]],  # (1)
```

1. See [:material-code-braces: UsageTypeDef](./type_defs.md#usagetypedef) 
## AggregationResponseTypeDef

```python
# AggregationResponseTypeDef TypedDict usage example

from types_aiobotocore_inspector2.type_defs import AggregationResponseTypeDef


def get_value() -> AggregationResponseTypeDef:
    return {
        "accountAggregation": ...,
    }


# AggregationResponseTypeDef definition

class AggregationResponseTypeDef(TypedDict):
    accountAggregation: NotRequired[AccountAggregationResponseTypeDef],  # (1)
    amiAggregation: NotRequired[AmiAggregationResponseTypeDef],  # (2)
    awsEcrContainerAggregation: NotRequired[AwsEcrContainerAggregationResponseTypeDef],  # (3)
    ec2InstanceAggregation: NotRequired[Ec2InstanceAggregationResponseTypeDef],  # (4)
    findingTypeAggregation: NotRequired[FindingTypeAggregationResponseTypeDef],  # (5)
    imageLayerAggregation: NotRequired[ImageLayerAggregationResponseTypeDef],  # (6)
    lambdaFunctionAggregation: NotRequired[LambdaFunctionAggregationResponseTypeDef],  # (7)
    lambdaLayerAggregation: NotRequired[LambdaLayerAggregationResponseTypeDef],  # (8)
    packageAggregation: NotRequired[PackageAggregationResponseTypeDef],  # (9)
    repositoryAggregation: NotRequired[RepositoryAggregationResponseTypeDef],  # (10)
    titleAggregation: NotRequired[TitleAggregationResponseTypeDef],  # (11)
```

1. See [:material-code-braces: AccountAggregationResponseTypeDef](./type_defs.md#accountaggregationresponsetypedef) 
2. See [:material-code-braces: AmiAggregationResponseTypeDef](./type_defs.md#amiaggregationresponsetypedef) 
3. See [:material-code-braces: AwsEcrContainerAggregationResponseTypeDef](./type_defs.md#awsecrcontaineraggregationresponsetypedef) 
4. See [:material-code-braces: Ec2InstanceAggregationResponseTypeDef](./type_defs.md#ec2instanceaggregationresponsetypedef) 
5. See [:material-code-braces: FindingTypeAggregationResponseTypeDef](./type_defs.md#findingtypeaggregationresponsetypedef) 
6. See [:material-code-braces: ImageLayerAggregationResponseTypeDef](./type_defs.md#imagelayeraggregationresponsetypedef) 
7. See [:material-code-braces: LambdaFunctionAggregationResponseTypeDef](./type_defs.md#lambdafunctionaggregationresponsetypedef) 
8. See [:material-code-braces: LambdaLayerAggregationResponseTypeDef](./type_defs.md#lambdalayeraggregationresponsetypedef) 
9. See [:material-code-braces: PackageAggregationResponseTypeDef](./type_defs.md#packageaggregationresponsetypedef) 
10. See [:material-code-braces: RepositoryAggregationResponseTypeDef](./type_defs.md#repositoryaggregationresponsetypedef) 
11. See [:material-code-braces: TitleAggregationResponseTypeDef](./type_defs.md#titleaggregationresponsetypedef) 
## AccountStateTypeDef

```python
# AccountStateTypeDef TypedDict usage example

from types_aiobotocore_inspector2.type_defs import AccountStateTypeDef


def get_value() -> AccountStateTypeDef:
    return {
        "accountId": ...,
    }


# AccountStateTypeDef definition

class AccountStateTypeDef(TypedDict):
    accountId: str,
    resourceState: ResourceStateTypeDef,  # (1)
    state: StateTypeDef,  # (2)
```

1. See [:material-code-braces: ResourceStateTypeDef](./type_defs.md#resourcestatetypedef) 
2. See [:material-code-braces: StateTypeDef](./type_defs.md#statetypedef) 
## DisableResponseTypeDef

```python
# DisableResponseTypeDef TypedDict usage example

from types_aiobotocore_inspector2.type_defs import DisableResponseTypeDef


def get_value() -> DisableResponseTypeDef:
    return {
        "accounts": ...,
    }


# DisableResponseTypeDef definition

class DisableResponseTypeDef(TypedDict):
    accounts: List[AccountTypeDef],  # (1)
    failedAccounts: List[FailedAccountTypeDef],  # (2)
    ResponseMetadata: ResponseMetadataTypeDef,  # (3)
```

1. See [:material-code-braces: AccountTypeDef](./type_defs.md#accounttypedef) 
2. See [:material-code-braces: FailedAccountTypeDef](./type_defs.md#failedaccounttypedef) 
3. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## EnableResponseTypeDef

```python
# EnableResponseTypeDef TypedDict usage example

from types_aiobotocore_inspector2.type_defs import EnableResponseTypeDef


def get_value() -> EnableResponseTypeDef:
    return {
        "accounts": ...,
    }


# EnableResponseTypeDef definition

class EnableResponseTypeDef(TypedDict):
    accounts: List[AccountTypeDef],  # (1)
    failedAccounts: List[FailedAccountTypeDef],  # (2)
    ResponseMetadata: ResponseMetadataTypeDef,  # (3)
```

1. See [:material-code-braces: AccountTypeDef](./type_defs.md#accounttypedef) 
2. See [:material-code-braces: FailedAccountTypeDef](./type_defs.md#failedaccounttypedef) 
3. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ResourceDetailsTypeDef

```python
# ResourceDetailsTypeDef TypedDict usage example

from types_aiobotocore_inspector2.type_defs import ResourceDetailsTypeDef


def get_value() -> ResourceDetailsTypeDef:
    return {
        "awsEc2Instance": ...,
    }


# ResourceDetailsTypeDef definition

class ResourceDetailsTypeDef(TypedDict):
    awsEc2Instance: NotRequired[AwsEc2InstanceDetailsTypeDef],  # (1)
    awsEcrContainerImage: NotRequired[AwsEcrContainerImageDetailsTypeDef],  # (2)
    awsLambdaFunction: NotRequired[AwsLambdaFunctionDetailsTypeDef],  # (3)
```

1. See [:material-code-braces: AwsEc2InstanceDetailsTypeDef](./type_defs.md#awsec2instancedetailstypedef) 
2. See [:material-code-braces: AwsEcrContainerImageDetailsTypeDef](./type_defs.md#awsecrcontainerimagedetailstypedef) 
3. See [:material-code-braces: AwsLambdaFunctionDetailsTypeDef](./type_defs.md#awslambdafunctiondetailstypedef) 
## SendCisSessionTelemetryRequestTypeDef

```python
# SendCisSessionTelemetryRequestTypeDef TypedDict usage example

from types_aiobotocore_inspector2.type_defs import SendCisSessionTelemetryRequestTypeDef


def get_value() -> SendCisSessionTelemetryRequestTypeDef:
    return {
        "messages": ...,
    }


# SendCisSessionTelemetryRequestTypeDef definition

class SendCisSessionTelemetryRequestTypeDef(TypedDict):
    messages: Sequence[CisSessionMessageTypeDef],  # (1)
    scanJobId: str,
    sessionToken: str,
```

1. See [:material-code-braces: CisSessionMessageTypeDef](./type_defs.md#cissessionmessagetypedef) 
## ListCisScanResultsAggregatedByChecksResponseTypeDef

```python
# ListCisScanResultsAggregatedByChecksResponseTypeDef TypedDict usage example

from types_aiobotocore_inspector2.type_defs import ListCisScanResultsAggregatedByChecksResponseTypeDef


def get_value() -> ListCisScanResultsAggregatedByChecksResponseTypeDef:
    return {
        "checkAggregations": ...,
    }


# ListCisScanResultsAggregatedByChecksResponseTypeDef definition

class ListCisScanResultsAggregatedByChecksResponseTypeDef(TypedDict):
    checkAggregations: List[CisCheckAggregationTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    nextToken: NotRequired[str],
```

1. See [:material-code-braces: CisCheckAggregationTypeDef](./type_defs.md#cischeckaggregationtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListCisScanResultsAggregatedByTargetResourceResponseTypeDef

```python
# ListCisScanResultsAggregatedByTargetResourceResponseTypeDef TypedDict usage example

from types_aiobotocore_inspector2.type_defs import ListCisScanResultsAggregatedByTargetResourceResponseTypeDef


def get_value() -> ListCisScanResultsAggregatedByTargetResourceResponseTypeDef:
    return {
        "nextToken": ...,
    }


# ListCisScanResultsAggregatedByTargetResourceResponseTypeDef definition

class ListCisScanResultsAggregatedByTargetResourceResponseTypeDef(TypedDict):
    targetResourceAggregations: List[CisTargetResourceAggregationTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    nextToken: NotRequired[str],
```

1. See [:material-code-braces: CisTargetResourceAggregationTypeDef](./type_defs.md#cistargetresourceaggregationtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListCisScansFilterCriteriaTypeDef

```python
# ListCisScansFilterCriteriaTypeDef TypedDict usage example

from types_aiobotocore_inspector2.type_defs import ListCisScansFilterCriteriaTypeDef


def get_value() -> ListCisScansFilterCriteriaTypeDef:
    return {
        "failedChecksFilters": ...,
    }


# ListCisScansFilterCriteriaTypeDef definition

class ListCisScansFilterCriteriaTypeDef(TypedDict):
    failedChecksFilters: NotRequired[Sequence[CisNumberFilterTypeDef]],  # (1)
    scanArnFilters: NotRequired[Sequence[CisStringFilterTypeDef]],  # (2)
    scanAtFilters: NotRequired[Sequence[CisDateFilterTypeDef]],  # (3)
    scanConfigurationArnFilters: NotRequired[Sequence[CisStringFilterTypeDef]],  # (2)
    scanNameFilters: NotRequired[Sequence[CisStringFilterTypeDef]],  # (2)
    scanStatusFilters: NotRequired[Sequence[CisScanStatusFilterTypeDef]],  # (6)
    scheduledByFilters: NotRequired[Sequence[CisStringFilterTypeDef]],  # (2)
    targetAccountIdFilters: NotRequired[Sequence[CisStringFilterTypeDef]],  # (2)
    targetResourceIdFilters: NotRequired[Sequence[CisStringFilterTypeDef]],  # (2)
    targetResourceTagFilters: NotRequired[Sequence[TagFilterTypeDef]],  # (10)
```

1. See [:material-code-braces: CisNumberFilterTypeDef](./type_defs.md#cisnumberfiltertypedef) 
2. See [:material-code-braces: CisStringFilterTypeDef](./type_defs.md#cisstringfiltertypedef) 
3. See [:material-code-braces: CisDateFilterTypeDef](./type_defs.md#cisdatefiltertypedef) 
4. See [:material-code-braces: CisStringFilterTypeDef](./type_defs.md#cisstringfiltertypedef) 
5. See [:material-code-braces: CisStringFilterTypeDef](./type_defs.md#cisstringfiltertypedef) 
6. See [:material-code-braces: CisScanStatusFilterTypeDef](./type_defs.md#cisscanstatusfiltertypedef) 
7. See [:material-code-braces: CisStringFilterTypeDef](./type_defs.md#cisstringfiltertypedef) 
8. See [:material-code-braces: CisStringFilterTypeDef](./type_defs.md#cisstringfiltertypedef) 
9. See [:material-code-braces: CisStringFilterTypeDef](./type_defs.md#cisstringfiltertypedef) 
10. See [:material-code-braces: TagFilterTypeDef](./type_defs.md#tagfiltertypedef) 
## CoverageFilterCriteriaTypeDef

```python
# CoverageFilterCriteriaTypeDef TypedDict usage example

from types_aiobotocore_inspector2.type_defs import CoverageFilterCriteriaTypeDef


def get_value() -> CoverageFilterCriteriaTypeDef:
    return {
        "accountId": ...,
    }


# CoverageFilterCriteriaTypeDef definition

class CoverageFilterCriteriaTypeDef(TypedDict):
    accountId: NotRequired[Sequence[CoverageStringFilterTypeDef]],  # (1)
    ec2InstanceTags: NotRequired[Sequence[CoverageMapFilterTypeDef]],  # (2)
    ecrImageTags: NotRequired[Sequence[CoverageStringFilterTypeDef]],  # (1)
    ecrRepositoryName: NotRequired[Sequence[CoverageStringFilterTypeDef]],  # (1)
    imagePulledAt: NotRequired[Sequence[CoverageDateFilterTypeDef]],  # (5)
    lambdaFunctionName: NotRequired[Sequence[CoverageStringFilterTypeDef]],  # (1)
    lambdaFunctionRuntime: NotRequired[Sequence[CoverageStringFilterTypeDef]],  # (1)
    lambdaFunctionTags: NotRequired[Sequence[CoverageMapFilterTypeDef]],  # (2)
    lastScannedAt: NotRequired[Sequence[CoverageDateFilterTypeDef]],  # (5)
    resourceId: NotRequired[Sequence[CoverageStringFilterTypeDef]],  # (1)
    resourceType: NotRequired[Sequence[CoverageStringFilterTypeDef]],  # (1)
    scanMode: NotRequired[Sequence[CoverageStringFilterTypeDef]],  # (1)
    scanStatusCode: NotRequired[Sequence[CoverageStringFilterTypeDef]],  # (1)
    scanStatusReason: NotRequired[Sequence[CoverageStringFilterTypeDef]],  # (1)
    scanType: NotRequired[Sequence[CoverageStringFilterTypeDef]],  # (1)
```

1. See [:material-code-braces: CoverageStringFilterTypeDef](./type_defs.md#coveragestringfiltertypedef) 
2. See [:material-code-braces: CoverageMapFilterTypeDef](./type_defs.md#coveragemapfiltertypedef) 
3. See [:material-code-braces: CoverageStringFilterTypeDef](./type_defs.md#coveragestringfiltertypedef) 
4. See [:material-code-braces: CoverageStringFilterTypeDef](./type_defs.md#coveragestringfiltertypedef) 
5. See [:material-code-braces: CoverageDateFilterTypeDef](./type_defs.md#coveragedatefiltertypedef) 
6. See [:material-code-braces: CoverageStringFilterTypeDef](./type_defs.md#coveragestringfiltertypedef) 
7. See [:material-code-braces: CoverageStringFilterTypeDef](./type_defs.md#coveragestringfiltertypedef) 
8. See [:material-code-braces: CoverageMapFilterTypeDef](./type_defs.md#coveragemapfiltertypedef) 
9. See [:material-code-braces: CoverageDateFilterTypeDef](./type_defs.md#coveragedatefiltertypedef) 
10. See [:material-code-braces: CoverageStringFilterTypeDef](./type_defs.md#coveragestringfiltertypedef) 
11. See [:material-code-braces: CoverageStringFilterTypeDef](./type_defs.md#coveragestringfiltertypedef) 
12. See [:material-code-braces: CoverageStringFilterTypeDef](./type_defs.md#coveragestringfiltertypedef) 
13. See [:material-code-braces: CoverageStringFilterTypeDef](./type_defs.md#coveragestringfiltertypedef) 
14. See [:material-code-braces: CoverageStringFilterTypeDef](./type_defs.md#coveragestringfiltertypedef) 
15. See [:material-code-braces: CoverageStringFilterTypeDef](./type_defs.md#coveragestringfiltertypedef) 
## ListCisScansResponseTypeDef

```python
# ListCisScansResponseTypeDef TypedDict usage example

from types_aiobotocore_inspector2.type_defs import ListCisScansResponseTypeDef


def get_value() -> ListCisScansResponseTypeDef:
    return {
        "nextToken": ...,
    }


# ListCisScansResponseTypeDef definition

class ListCisScansResponseTypeDef(TypedDict):
    scans: List[CisScanTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    nextToken: NotRequired[str],
```

1. See [:material-code-braces: CisScanTypeDef](./type_defs.md#cisscantypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetCisScanResultDetailsRequestPaginateTypeDef

```python
# GetCisScanResultDetailsRequestPaginateTypeDef TypedDict usage example

from types_aiobotocore_inspector2.type_defs import GetCisScanResultDetailsRequestPaginateTypeDef


def get_value() -> GetCisScanResultDetailsRequestPaginateTypeDef:
    return {
        "accountId": ...,
    }


# GetCisScanResultDetailsRequestPaginateTypeDef definition

class GetCisScanResultDetailsRequestPaginateTypeDef(TypedDict):
    accountId: str,
    scanArn: str,
    targetResourceId: str,
    filterCriteria: NotRequired[CisScanResultDetailsFilterCriteriaTypeDef],  # (1)
    sortBy: NotRequired[CisScanResultDetailsSortByType],  # (2)
    sortOrder: NotRequired[CisSortOrderType],  # (3)
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (4)
```

1. See [:material-code-braces: CisScanResultDetailsFilterCriteriaTypeDef](./type_defs.md#cisscanresultdetailsfiltercriteriatypedef) 
2. See [:material-code-brackets: CisScanResultDetailsSortByType](./literals.md#cisscanresultdetailssortbytype) 
3. See [:material-code-brackets: CisSortOrderType](./literals.md#cissortordertype) 
4. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## GetCisScanResultDetailsRequestTypeDef

```python
# GetCisScanResultDetailsRequestTypeDef TypedDict usage example

from types_aiobotocore_inspector2.type_defs import GetCisScanResultDetailsRequestTypeDef


def get_value() -> GetCisScanResultDetailsRequestTypeDef:
    return {
        "accountId": ...,
    }


# GetCisScanResultDetailsRequestTypeDef definition

class GetCisScanResultDetailsRequestTypeDef(TypedDict):
    accountId: str,
    scanArn: str,
    targetResourceId: str,
    filterCriteria: NotRequired[CisScanResultDetailsFilterCriteriaTypeDef],  # (1)
    maxResults: NotRequired[int],
    nextToken: NotRequired[str],
    sortBy: NotRequired[CisScanResultDetailsSortByType],  # (2)
    sortOrder: NotRequired[CisSortOrderType],  # (3)
```

1. See [:material-code-braces: CisScanResultDetailsFilterCriteriaTypeDef](./type_defs.md#cisscanresultdetailsfiltercriteriatypedef) 
2. See [:material-code-brackets: CisScanResultDetailsSortByType](./literals.md#cisscanresultdetailssortbytype) 
3. See [:material-code-brackets: CisSortOrderType](./literals.md#cissortordertype) 
## ListCisScanResultsAggregatedByChecksRequestPaginateTypeDef

```python
# ListCisScanResultsAggregatedByChecksRequestPaginateTypeDef TypedDict usage example

from types_aiobotocore_inspector2.type_defs import ListCisScanResultsAggregatedByChecksRequestPaginateTypeDef


def get_value() -> ListCisScanResultsAggregatedByChecksRequestPaginateTypeDef:
    return {
        "scanArn": ...,
    }


# ListCisScanResultsAggregatedByChecksRequestPaginateTypeDef definition

class ListCisScanResultsAggregatedByChecksRequestPaginateTypeDef(TypedDict):
    scanArn: str,
    filterCriteria: NotRequired[CisScanResultsAggregatedByChecksFilterCriteriaTypeDef],  # (1)
    sortBy: NotRequired[CisScanResultsAggregatedByChecksSortByType],  # (2)
    sortOrder: NotRequired[CisSortOrderType],  # (3)
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (4)
```

1. See [:material-code-braces: CisScanResultsAggregatedByChecksFilterCriteriaTypeDef](./type_defs.md#cisscanresultsaggregatedbychecksfiltercriteriatypedef) 
2. See [:material-code-brackets: CisScanResultsAggregatedByChecksSortByType](./literals.md#cisscanresultsaggregatedbycheckssortbytype) 
3. See [:material-code-brackets: CisSortOrderType](./literals.md#cissortordertype) 
4. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListCisScanResultsAggregatedByChecksRequestTypeDef

```python
# ListCisScanResultsAggregatedByChecksRequestTypeDef TypedDict usage example

from types_aiobotocore_inspector2.type_defs import ListCisScanResultsAggregatedByChecksRequestTypeDef


def get_value() -> ListCisScanResultsAggregatedByChecksRequestTypeDef:
    return {
        "scanArn": ...,
    }


# ListCisScanResultsAggregatedByChecksRequestTypeDef definition

class ListCisScanResultsAggregatedByChecksRequestTypeDef(TypedDict):
    scanArn: str,
    filterCriteria: NotRequired[CisScanResultsAggregatedByChecksFilterCriteriaTypeDef],  # (1)
    maxResults: NotRequired[int],
    nextToken: NotRequired[str],
    sortBy: NotRequired[CisScanResultsAggregatedByChecksSortByType],  # (2)
    sortOrder: NotRequired[CisSortOrderType],  # (3)
```

1. See [:material-code-braces: CisScanResultsAggregatedByChecksFilterCriteriaTypeDef](./type_defs.md#cisscanresultsaggregatedbychecksfiltercriteriatypedef) 
2. See [:material-code-brackets: CisScanResultsAggregatedByChecksSortByType](./literals.md#cisscanresultsaggregatedbycheckssortbytype) 
3. See [:material-code-brackets: CisSortOrderType](./literals.md#cissortordertype) 
## ListCisScanResultsAggregatedByTargetResourceRequestPaginateTypeDef

```python
# ListCisScanResultsAggregatedByTargetResourceRequestPaginateTypeDef TypedDict usage example

from types_aiobotocore_inspector2.type_defs import ListCisScanResultsAggregatedByTargetResourceRequestPaginateTypeDef


def get_value() -> ListCisScanResultsAggregatedByTargetResourceRequestPaginateTypeDef:
    return {
        "scanArn": ...,
    }


# ListCisScanResultsAggregatedByTargetResourceRequestPaginateTypeDef definition

class ListCisScanResultsAggregatedByTargetResourceRequestPaginateTypeDef(TypedDict):
    scanArn: str,
    filterCriteria: NotRequired[CisScanResultsAggregatedByTargetResourceFilterCriteriaTypeDef],  # (1)
    sortBy: NotRequired[CisScanResultsAggregatedByTargetResourceSortByType],  # (2)
    sortOrder: NotRequired[CisSortOrderType],  # (3)
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (4)
```

1. See [:material-code-braces: CisScanResultsAggregatedByTargetResourceFilterCriteriaTypeDef](./type_defs.md#cisscanresultsaggregatedbytargetresourcefiltercriteriatypedef) 
2. See [:material-code-brackets: CisScanResultsAggregatedByTargetResourceSortByType](./literals.md#cisscanresultsaggregatedbytargetresourcesortbytype) 
3. See [:material-code-brackets: CisSortOrderType](./literals.md#cissortordertype) 
4. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListCisScanResultsAggregatedByTargetResourceRequestTypeDef

```python
# ListCisScanResultsAggregatedByTargetResourceRequestTypeDef TypedDict usage example

from types_aiobotocore_inspector2.type_defs import ListCisScanResultsAggregatedByTargetResourceRequestTypeDef


def get_value() -> ListCisScanResultsAggregatedByTargetResourceRequestTypeDef:
    return {
        "scanArn": ...,
    }


# ListCisScanResultsAggregatedByTargetResourceRequestTypeDef definition

class ListCisScanResultsAggregatedByTargetResourceRequestTypeDef(TypedDict):
    scanArn: str,
    filterCriteria: NotRequired[CisScanResultsAggregatedByTargetResourceFilterCriteriaTypeDef],  # (1)
    maxResults: NotRequired[int],
    nextToken: NotRequired[str],
    sortBy: NotRequired[CisScanResultsAggregatedByTargetResourceSortByType],  # (2)
    sortOrder: NotRequired[CisSortOrderType],  # (3)
```

1. See [:material-code-braces: CisScanResultsAggregatedByTargetResourceFilterCriteriaTypeDef](./type_defs.md#cisscanresultsaggregatedbytargetresourcefiltercriteriatypedef) 
2. See [:material-code-brackets: CisScanResultsAggregatedByTargetResourceSortByType](./literals.md#cisscanresultsaggregatedbytargetresourcesortbytype) 
3. See [:material-code-brackets: CisSortOrderType](./literals.md#cissortordertype) 
## ListCisScanConfigurationsRequestPaginateTypeDef

```python
# ListCisScanConfigurationsRequestPaginateTypeDef TypedDict usage example

from types_aiobotocore_inspector2.type_defs import ListCisScanConfigurationsRequestPaginateTypeDef


def get_value() -> ListCisScanConfigurationsRequestPaginateTypeDef:
    return {
        "filterCriteria": ...,
    }


# ListCisScanConfigurationsRequestPaginateTypeDef definition

class ListCisScanConfigurationsRequestPaginateTypeDef(TypedDict):
    filterCriteria: NotRequired[ListCisScanConfigurationsFilterCriteriaTypeDef],  # (1)
    sortBy: NotRequired[CisScanConfigurationsSortByType],  # (2)
    sortOrder: NotRequired[CisSortOrderType],  # (3)
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (4)
```

1. See [:material-code-braces: ListCisScanConfigurationsFilterCriteriaTypeDef](./type_defs.md#listcisscanconfigurationsfiltercriteriatypedef) 
2. See [:material-code-brackets: CisScanConfigurationsSortByType](./literals.md#cisscanconfigurationssortbytype) 
3. See [:material-code-brackets: CisSortOrderType](./literals.md#cissortordertype) 
4. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListCisScanConfigurationsRequestTypeDef

```python
# ListCisScanConfigurationsRequestTypeDef TypedDict usage example

from types_aiobotocore_inspector2.type_defs import ListCisScanConfigurationsRequestTypeDef


def get_value() -> ListCisScanConfigurationsRequestTypeDef:
    return {
        "filterCriteria": ...,
    }


# ListCisScanConfigurationsRequestTypeDef definition

class ListCisScanConfigurationsRequestTypeDef(TypedDict):
    filterCriteria: NotRequired[ListCisScanConfigurationsFilterCriteriaTypeDef],  # (1)
    maxResults: NotRequired[int],
    nextToken: NotRequired[str],
    sortBy: NotRequired[CisScanConfigurationsSortByType],  # (2)
    sortOrder: NotRequired[CisSortOrderType],  # (3)
```

1. See [:material-code-braces: ListCisScanConfigurationsFilterCriteriaTypeDef](./type_defs.md#listcisscanconfigurationsfiltercriteriatypedef) 
2. See [:material-code-brackets: CisScanConfigurationsSortByType](./literals.md#cisscanconfigurationssortbytype) 
3. See [:material-code-brackets: CisSortOrderType](./literals.md#cissortordertype) 
## BatchGetCodeSnippetResponseTypeDef

```python
# BatchGetCodeSnippetResponseTypeDef TypedDict usage example

from types_aiobotocore_inspector2.type_defs import BatchGetCodeSnippetResponseTypeDef


def get_value() -> BatchGetCodeSnippetResponseTypeDef:
    return {
        "codeSnippetResults": ...,
    }


# BatchGetCodeSnippetResponseTypeDef definition

class BatchGetCodeSnippetResponseTypeDef(TypedDict):
    codeSnippetResults: List[CodeSnippetResultTypeDef],  # (1)
    errors: List[CodeSnippetErrorTypeDef],  # (2)
    ResponseMetadata: ResponseMetadataTypeDef,  # (3)
```

1. See [:material-code-braces: CodeSnippetResultTypeDef](./type_defs.md#codesnippetresulttypedef) 
2. See [:material-code-braces: CodeSnippetErrorTypeDef](./type_defs.md#codesnippeterrortypedef) 
3. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## InspectorScoreDetailsTypeDef

```python
# InspectorScoreDetailsTypeDef TypedDict usage example

from types_aiobotocore_inspector2.type_defs import InspectorScoreDetailsTypeDef


def get_value() -> InspectorScoreDetailsTypeDef:
    return {
        "adjustedCvss": ...,
    }


# InspectorScoreDetailsTypeDef definition

class InspectorScoreDetailsTypeDef(TypedDict):
    adjustedCvss: NotRequired[CvssScoreDetailsTypeDef],  # (1)
```

1. See [:material-code-braces: CvssScoreDetailsTypeDef](./type_defs.md#cvssscoredetailstypedef) 
## ScheduleOutputTypeDef

```python
# ScheduleOutputTypeDef TypedDict usage example

from types_aiobotocore_inspector2.type_defs import ScheduleOutputTypeDef


def get_value() -> ScheduleOutputTypeDef:
    return {
        "daily": ...,
    }


# ScheduleOutputTypeDef definition

class ScheduleOutputTypeDef(TypedDict):
    daily: NotRequired[DailyScheduleTypeDef],  # (1)
    monthly: NotRequired[MonthlyScheduleTypeDef],  # (2)
    oneTime: NotRequired[Dict[str, Any]],
    weekly: NotRequired[WeeklyScheduleOutputTypeDef],  # (3)
```

1. See [:material-code-braces: DailyScheduleTypeDef](./type_defs.md#dailyscheduletypedef) 
2. See [:material-code-braces: MonthlyScheduleTypeDef](./type_defs.md#monthlyscheduletypedef) 
3. See [:material-code-braces: WeeklyScheduleOutputTypeDef](./type_defs.md#weeklyscheduleoutputtypedef) 
## ScheduleTypeDef

```python
# ScheduleTypeDef TypedDict usage example

from types_aiobotocore_inspector2.type_defs import ScheduleTypeDef


def get_value() -> ScheduleTypeDef:
    return {
        "daily": ...,
    }


# ScheduleTypeDef definition

class ScheduleTypeDef(TypedDict):
    daily: NotRequired[DailyScheduleTypeDef],  # (1)
    monthly: NotRequired[MonthlyScheduleTypeDef],  # (2)
    oneTime: NotRequired[Mapping[str, Any]],
    weekly: NotRequired[WeeklyScheduleTypeDef],  # (3)
```

1. See [:material-code-braces: DailyScheduleTypeDef](./type_defs.md#dailyscheduletypedef) 
2. See [:material-code-braces: MonthlyScheduleTypeDef](./type_defs.md#monthlyscheduletypedef) 
3. See [:material-code-braces: WeeklyScheduleTypeDef](./type_defs.md#weeklyscheduletypedef) 
## AggregationRequestTypeDef

```python
# AggregationRequestTypeDef TypedDict usage example

from types_aiobotocore_inspector2.type_defs import AggregationRequestTypeDef


def get_value() -> AggregationRequestTypeDef:
    return {
        "accountAggregation": ...,
    }


# AggregationRequestTypeDef definition

class AggregationRequestTypeDef(TypedDict):
    accountAggregation: NotRequired[AccountAggregationTypeDef],  # (1)
    amiAggregation: NotRequired[AmiAggregationTypeDef],  # (2)
    awsEcrContainerAggregation: NotRequired[AwsEcrContainerAggregationTypeDef],  # (3)
    ec2InstanceAggregation: NotRequired[Ec2InstanceAggregationTypeDef],  # (4)
    findingTypeAggregation: NotRequired[FindingTypeAggregationTypeDef],  # (5)
    imageLayerAggregation: NotRequired[ImageLayerAggregationTypeDef],  # (6)
    lambdaFunctionAggregation: NotRequired[LambdaFunctionAggregationTypeDef],  # (7)
    lambdaLayerAggregation: NotRequired[LambdaLayerAggregationTypeDef],  # (8)
    packageAggregation: NotRequired[PackageAggregationTypeDef],  # (9)
    repositoryAggregation: NotRequired[RepositoryAggregationTypeDef],  # (10)
    titleAggregation: NotRequired[TitleAggregationTypeDef],  # (11)
```

1. See [:material-code-braces: AccountAggregationTypeDef](./type_defs.md#accountaggregationtypedef) 
2. See [:material-code-braces: AmiAggregationTypeDef](./type_defs.md#amiaggregationtypedef) 
3. See [:material-code-braces: AwsEcrContainerAggregationTypeDef](./type_defs.md#awsecrcontaineraggregationtypedef) 
4. See [:material-code-braces: Ec2InstanceAggregationTypeDef](./type_defs.md#ec2instanceaggregationtypedef) 
5. See [:material-code-braces: FindingTypeAggregationTypeDef](./type_defs.md#findingtypeaggregationtypedef) 
6. See [:material-code-braces: ImageLayerAggregationTypeDef](./type_defs.md#imagelayeraggregationtypedef) 
7. See [:material-code-braces: LambdaFunctionAggregationTypeDef](./type_defs.md#lambdafunctionaggregationtypedef) 
8. See [:material-code-braces: LambdaLayerAggregationTypeDef](./type_defs.md#lambdalayeraggregationtypedef) 
9. See [:material-code-braces: PackageAggregationTypeDef](./type_defs.md#packageaggregationtypedef) 
10. See [:material-code-braces: RepositoryAggregationTypeDef](./type_defs.md#repositoryaggregationtypedef) 
11. See [:material-code-braces: TitleAggregationTypeDef](./type_defs.md#titleaggregationtypedef) 
## GetConfigurationResponseTypeDef

```python
# GetConfigurationResponseTypeDef TypedDict usage example

from types_aiobotocore_inspector2.type_defs import GetConfigurationResponseTypeDef


def get_value() -> GetConfigurationResponseTypeDef:
    return {
        "ec2Configuration": ...,
    }


# GetConfigurationResponseTypeDef definition

class GetConfigurationResponseTypeDef(TypedDict):
    ec2Configuration: Ec2ConfigurationStateTypeDef,  # (1)
    ecrConfiguration: EcrConfigurationStateTypeDef,  # (2)
    ResponseMetadata: ResponseMetadataTypeDef,  # (3)
```

1. See [:material-code-braces: Ec2ConfigurationStateTypeDef](./type_defs.md#ec2configurationstatetypedef) 
2. See [:material-code-braces: EcrConfigurationStateTypeDef](./type_defs.md#ecrconfigurationstatetypedef) 
3. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## BatchGetFindingDetailsResponseTypeDef

```python
# BatchGetFindingDetailsResponseTypeDef TypedDict usage example

from types_aiobotocore_inspector2.type_defs import BatchGetFindingDetailsResponseTypeDef


def get_value() -> BatchGetFindingDetailsResponseTypeDef:
    return {
        "errors": ...,
    }


# BatchGetFindingDetailsResponseTypeDef definition

class BatchGetFindingDetailsResponseTypeDef(TypedDict):
    errors: List[FindingDetailsErrorTypeDef],  # (1)
    findingDetails: List[FindingDetailTypeDef],  # (2)
    ResponseMetadata: ResponseMetadataTypeDef,  # (3)
```

1. See [:material-code-braces: FindingDetailsErrorTypeDef](./type_defs.md#findingdetailserrortypedef) 
2. See [:material-code-braces: FindingDetailTypeDef](./type_defs.md#findingdetailtypedef) 
3. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## SearchVulnerabilitiesResponseTypeDef

```python
# SearchVulnerabilitiesResponseTypeDef TypedDict usage example

from types_aiobotocore_inspector2.type_defs import SearchVulnerabilitiesResponseTypeDef


def get_value() -> SearchVulnerabilitiesResponseTypeDef:
    return {
        "nextToken": ...,
    }


# SearchVulnerabilitiesResponseTypeDef definition

class SearchVulnerabilitiesResponseTypeDef(TypedDict):
    vulnerabilities: List[VulnerabilityTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    nextToken: NotRequired[str],
```

1. See [:material-code-braces: VulnerabilityTypeDef](./type_defs.md#vulnerabilitytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## FilterCriteriaOutputTypeDef

```python
# FilterCriteriaOutputTypeDef TypedDict usage example

from types_aiobotocore_inspector2.type_defs import FilterCriteriaOutputTypeDef


def get_value() -> FilterCriteriaOutputTypeDef:
    return {
        "awsAccountId": ...,
    }


# FilterCriteriaOutputTypeDef definition

class FilterCriteriaOutputTypeDef(TypedDict):
    awsAccountId: NotRequired[List[StringFilterTypeDef]],  # (1)
    codeVulnerabilityDetectorName: NotRequired[List[StringFilterTypeDef]],  # (1)
    codeVulnerabilityDetectorTags: NotRequired[List[StringFilterTypeDef]],  # (1)
    codeVulnerabilityFilePath: NotRequired[List[StringFilterTypeDef]],  # (1)
    componentId: NotRequired[List[StringFilterTypeDef]],  # (1)
    componentType: NotRequired[List[StringFilterTypeDef]],  # (1)
    ec2InstanceImageId: NotRequired[List[StringFilterTypeDef]],  # (1)
    ec2InstanceSubnetId: NotRequired[List[StringFilterTypeDef]],  # (1)
    ec2InstanceVpcId: NotRequired[List[StringFilterTypeDef]],  # (1)
    ecrImageArchitecture: NotRequired[List[StringFilterTypeDef]],  # (1)
    ecrImageHash: NotRequired[List[StringFilterTypeDef]],  # (1)
    ecrImagePushedAt: NotRequired[List[DateFilterOutputTypeDef]],  # (12)
    ecrImageRegistry: NotRequired[List[StringFilterTypeDef]],  # (1)
    ecrImageRepositoryName: NotRequired[List[StringFilterTypeDef]],  # (1)
    ecrImageTags: NotRequired[List[StringFilterTypeDef]],  # (1)
    epssScore: NotRequired[List[NumberFilterTypeDef]],  # (16)
    exploitAvailable: NotRequired[List[StringFilterTypeDef]],  # (1)
    findingArn: NotRequired[List[StringFilterTypeDef]],  # (1)
    findingStatus: NotRequired[List[StringFilterTypeDef]],  # (1)
    findingType: NotRequired[List[StringFilterTypeDef]],  # (1)
    firstObservedAt: NotRequired[List[DateFilterOutputTypeDef]],  # (12)
    fixAvailable: NotRequired[List[StringFilterTypeDef]],  # (1)
    inspectorScore: NotRequired[List[NumberFilterTypeDef]],  # (16)
    lambdaFunctionExecutionRoleArn: NotRequired[List[StringFilterTypeDef]],  # (1)
    lambdaFunctionLastModifiedAt: NotRequired[List[DateFilterOutputTypeDef]],  # (12)
    lambdaFunctionLayers: NotRequired[List[StringFilterTypeDef]],  # (1)
    lambdaFunctionName: NotRequired[List[StringFilterTypeDef]],  # (1)
    lambdaFunctionRuntime: NotRequired[List[StringFilterTypeDef]],  # (1)
    lastObservedAt: NotRequired[List[DateFilterOutputTypeDef]],  # (12)
    networkProtocol: NotRequired[List[StringFilterTypeDef]],  # (1)
    portRange: NotRequired[List[PortRangeFilterTypeDef]],  # (31)
    relatedVulnerabilities: NotRequired[List[StringFilterTypeDef]],  # (1)
    resourceId: NotRequired[List[StringFilterTypeDef]],  # (1)
    resourceTags: NotRequired[List[MapFilterTypeDef]],  # (34)
    resourceType: NotRequired[List[StringFilterTypeDef]],  # (1)
    severity: NotRequired[List[StringFilterTypeDef]],  # (1)
    title: NotRequired[List[StringFilterTypeDef]],  # (1)
    updatedAt: NotRequired[List[DateFilterOutputTypeDef]],  # (12)
    vendorSeverity: NotRequired[List[StringFilterTypeDef]],  # (1)
    vulnerabilityId: NotRequired[List[StringFilterTypeDef]],  # (1)
    vulnerabilitySource: NotRequired[List[StringFilterTypeDef]],  # (1)
    vulnerablePackages: NotRequired[List[PackageFilterTypeDef]],  # (42)
```

1. See [:material-code-braces: StringFilterTypeDef](./type_defs.md#stringfiltertypedef) 
2. See [:material-code-braces: StringFilterTypeDef](./type_defs.md#stringfiltertypedef) 
3. See [:material-code-braces: StringFilterTypeDef](./type_defs.md#stringfiltertypedef) 
4. See [:material-code-braces: StringFilterTypeDef](./type_defs.md#stringfiltertypedef) 
5. See [:material-code-braces: StringFilterTypeDef](./type_defs.md#stringfiltertypedef) 
6. See [:material-code-braces: StringFilterTypeDef](./type_defs.md#stringfiltertypedef) 
7. See [:material-code-braces: StringFilterTypeDef](./type_defs.md#stringfiltertypedef) 
8. See [:material-code-braces: StringFilterTypeDef](./type_defs.md#stringfiltertypedef) 
9. See [:material-code-braces: StringFilterTypeDef](./type_defs.md#stringfiltertypedef) 
10. See [:material-code-braces: StringFilterTypeDef](./type_defs.md#stringfiltertypedef) 
11. See [:material-code-braces: StringFilterTypeDef](./type_defs.md#stringfiltertypedef) 
12. See [:material-code-braces: DateFilterOutputTypeDef](./type_defs.md#datefilteroutputtypedef) 
13. See [:material-code-braces: StringFilterTypeDef](./type_defs.md#stringfiltertypedef) 
14. See [:material-code-braces: StringFilterTypeDef](./type_defs.md#stringfiltertypedef) 
15. See [:material-code-braces: StringFilterTypeDef](./type_defs.md#stringfiltertypedef) 
16. See [:material-code-braces: NumberFilterTypeDef](./type_defs.md#numberfiltertypedef) 
17. See [:material-code-braces: StringFilterTypeDef](./type_defs.md#stringfiltertypedef) 
18. See [:material-code-braces: StringFilterTypeDef](./type_defs.md#stringfiltertypedef) 
19. See [:material-code-braces: StringFilterTypeDef](./type_defs.md#stringfiltertypedef) 
20. See [:material-code-braces: StringFilterTypeDef](./type_defs.md#stringfiltertypedef) 
21. See [:material-code-braces: DateFilterOutputTypeDef](./type_defs.md#datefilteroutputtypedef) 
22. See [:material-code-braces: StringFilterTypeDef](./type_defs.md#stringfiltertypedef) 
23. See [:material-code-braces: NumberFilterTypeDef](./type_defs.md#numberfiltertypedef) 
24. See [:material-code-braces: StringFilterTypeDef](./type_defs.md#stringfiltertypedef) 
25. See [:material-code-braces: DateFilterOutputTypeDef](./type_defs.md#datefilteroutputtypedef) 
26. See [:material-code-braces: StringFilterTypeDef](./type_defs.md#stringfiltertypedef) 
27. See [:material-code-braces: StringFilterTypeDef](./type_defs.md#stringfiltertypedef) 
28. See [:material-code-braces: StringFilterTypeDef](./type_defs.md#stringfiltertypedef) 
29. See [:material-code-braces: DateFilterOutputTypeDef](./type_defs.md#datefilteroutputtypedef) 
30. See [:material-code-braces: StringFilterTypeDef](./type_defs.md#stringfiltertypedef) 
31. See [:material-code-braces: PortRangeFilterTypeDef](./type_defs.md#portrangefiltertypedef) 
32. See [:material-code-braces: StringFilterTypeDef](./type_defs.md#stringfiltertypedef) 
33. See [:material-code-braces: StringFilterTypeDef](./type_defs.md#stringfiltertypedef) 
34. See [:material-code-braces: MapFilterTypeDef](./type_defs.md#mapfiltertypedef) 
35. See [:material-code-braces: StringFilterTypeDef](./type_defs.md#stringfiltertypedef) 
36. See [:material-code-braces: StringFilterTypeDef](./type_defs.md#stringfiltertypedef) 
37. See [:material-code-braces: StringFilterTypeDef](./type_defs.md#stringfiltertypedef) 
38. See [:material-code-braces: DateFilterOutputTypeDef](./type_defs.md#datefilteroutputtypedef) 
39. See [:material-code-braces: StringFilterTypeDef](./type_defs.md#stringfiltertypedef) 
40. See [:material-code-braces: StringFilterTypeDef](./type_defs.md#stringfiltertypedef) 
41. See [:material-code-braces: StringFilterTypeDef](./type_defs.md#stringfiltertypedef) 
42. See [:material-code-braces: PackageFilterTypeDef](./type_defs.md#packagefiltertypedef) 
## FilterCriteriaTypeDef

```python
# FilterCriteriaTypeDef TypedDict usage example

from types_aiobotocore_inspector2.type_defs import FilterCriteriaTypeDef


def get_value() -> FilterCriteriaTypeDef:
    return {
        "awsAccountId": ...,
    }


# FilterCriteriaTypeDef definition

class FilterCriteriaTypeDef(TypedDict):
    awsAccountId: NotRequired[Sequence[StringFilterTypeDef]],  # (1)
    codeVulnerabilityDetectorName: NotRequired[Sequence[StringFilterTypeDef]],  # (1)
    codeVulnerabilityDetectorTags: NotRequired[Sequence[StringFilterTypeDef]],  # (1)
    codeVulnerabilityFilePath: NotRequired[Sequence[StringFilterTypeDef]],  # (1)
    componentId: NotRequired[Sequence[StringFilterTypeDef]],  # (1)
    componentType: NotRequired[Sequence[StringFilterTypeDef]],  # (1)
    ec2InstanceImageId: NotRequired[Sequence[StringFilterTypeDef]],  # (1)
    ec2InstanceSubnetId: NotRequired[Sequence[StringFilterTypeDef]],  # (1)
    ec2InstanceVpcId: NotRequired[Sequence[StringFilterTypeDef]],  # (1)
    ecrImageArchitecture: NotRequired[Sequence[StringFilterTypeDef]],  # (1)
    ecrImageHash: NotRequired[Sequence[StringFilterTypeDef]],  # (1)
    ecrImagePushedAt: NotRequired[Sequence[DateFilterTypeDef]],  # (12)
    ecrImageRegistry: NotRequired[Sequence[StringFilterTypeDef]],  # (1)
    ecrImageRepositoryName: NotRequired[Sequence[StringFilterTypeDef]],  # (1)
    ecrImageTags: NotRequired[Sequence[StringFilterTypeDef]],  # (1)
    epssScore: NotRequired[Sequence[NumberFilterTypeDef]],  # (16)
    exploitAvailable: NotRequired[Sequence[StringFilterTypeDef]],  # (1)
    findingArn: NotRequired[Sequence[StringFilterTypeDef]],  # (1)
    findingStatus: NotRequired[Sequence[StringFilterTypeDef]],  # (1)
    findingType: NotRequired[Sequence[StringFilterTypeDef]],  # (1)
    firstObservedAt: NotRequired[Sequence[DateFilterTypeDef]],  # (12)
    fixAvailable: NotRequired[Sequence[StringFilterTypeDef]],  # (1)
    inspectorScore: NotRequired[Sequence[NumberFilterTypeDef]],  # (16)
    lambdaFunctionExecutionRoleArn: NotRequired[Sequence[StringFilterTypeDef]],  # (1)
    lambdaFunctionLastModifiedAt: NotRequired[Sequence[DateFilterTypeDef]],  # (12)
    lambdaFunctionLayers: NotRequired[Sequence[StringFilterTypeDef]],  # (1)
    lambdaFunctionName: NotRequired[Sequence[StringFilterTypeDef]],  # (1)
    lambdaFunctionRuntime: NotRequired[Sequence[StringFilterTypeDef]],  # (1)
    lastObservedAt: NotRequired[Sequence[DateFilterTypeDef]],  # (12)
    networkProtocol: NotRequired[Sequence[StringFilterTypeDef]],  # (1)
    portRange: NotRequired[Sequence[PortRangeFilterTypeDef]],  # (31)
    relatedVulnerabilities: NotRequired[Sequence[StringFilterTypeDef]],  # (1)
    resourceId: NotRequired[Sequence[StringFilterTypeDef]],  # (1)
    resourceTags: NotRequired[Sequence[MapFilterTypeDef]],  # (34)
    resourceType: NotRequired[Sequence[StringFilterTypeDef]],  # (1)
    severity: NotRequired[Sequence[StringFilterTypeDef]],  # (1)
    title: NotRequired[Sequence[StringFilterTypeDef]],  # (1)
    updatedAt: NotRequired[Sequence[DateFilterTypeDef]],  # (12)
    vendorSeverity: NotRequired[Sequence[StringFilterTypeDef]],  # (1)
    vulnerabilityId: NotRequired[Sequence[StringFilterTypeDef]],  # (1)
    vulnerabilitySource: NotRequired[Sequence[StringFilterTypeDef]],  # (1)
    vulnerablePackages: NotRequired[Sequence[PackageFilterTypeDef]],  # (42)
```

1. See [:material-code-braces: StringFilterTypeDef](./type_defs.md#stringfiltertypedef) 
2. See [:material-code-braces: StringFilterTypeDef](./type_defs.md#stringfiltertypedef) 
3. See [:material-code-braces: StringFilterTypeDef](./type_defs.md#stringfiltertypedef) 
4. See [:material-code-braces: StringFilterTypeDef](./type_defs.md#stringfiltertypedef) 
5. See [:material-code-braces: StringFilterTypeDef](./type_defs.md#stringfiltertypedef) 
6. See [:material-code-braces: StringFilterTypeDef](./type_defs.md#stringfiltertypedef) 
7. See [:material-code-braces: StringFilterTypeDef](./type_defs.md#stringfiltertypedef) 
8. See [:material-code-braces: StringFilterTypeDef](./type_defs.md#stringfiltertypedef) 
9. See [:material-code-braces: StringFilterTypeDef](./type_defs.md#stringfiltertypedef) 
10. See [:material-code-braces: StringFilterTypeDef](./type_defs.md#stringfiltertypedef) 
11. See [:material-code-braces: StringFilterTypeDef](./type_defs.md#stringfiltertypedef) 
12. See [:material-code-braces: DateFilterTypeDef](./type_defs.md#datefiltertypedef) 
13. See [:material-code-braces: StringFilterTypeDef](./type_defs.md#stringfiltertypedef) 
14. See [:material-code-braces: StringFilterTypeDef](./type_defs.md#stringfiltertypedef) 
15. See [:material-code-braces: StringFilterTypeDef](./type_defs.md#stringfiltertypedef) 
16. See [:material-code-braces: NumberFilterTypeDef](./type_defs.md#numberfiltertypedef) 
17. See [:material-code-braces: StringFilterTypeDef](./type_defs.md#stringfiltertypedef) 
18. See [:material-code-braces: StringFilterTypeDef](./type_defs.md#stringfiltertypedef) 
19. See [:material-code-braces: StringFilterTypeDef](./type_defs.md#stringfiltertypedef) 
20. See [:material-code-braces: StringFilterTypeDef](./type_defs.md#stringfiltertypedef) 
21. See [:material-code-braces: DateFilterTypeDef](./type_defs.md#datefiltertypedef) 
22. See [:material-code-braces: StringFilterTypeDef](./type_defs.md#stringfiltertypedef) 
23. See [:material-code-braces: NumberFilterTypeDef](./type_defs.md#numberfiltertypedef) 
24. See [:material-code-braces: StringFilterTypeDef](./type_defs.md#stringfiltertypedef) 
25. See [:material-code-braces: DateFilterTypeDef](./type_defs.md#datefiltertypedef) 
26. See [:material-code-braces: StringFilterTypeDef](./type_defs.md#stringfiltertypedef) 
27. See [:material-code-braces: StringFilterTypeDef](./type_defs.md#stringfiltertypedef) 
28. See [:material-code-braces: StringFilterTypeDef](./type_defs.md#stringfiltertypedef) 
29. See [:material-code-braces: DateFilterTypeDef](./type_defs.md#datefiltertypedef) 
30. See [:material-code-braces: StringFilterTypeDef](./type_defs.md#stringfiltertypedef) 
31. See [:material-code-braces: PortRangeFilterTypeDef](./type_defs.md#portrangefiltertypedef) 
32. See [:material-code-braces: StringFilterTypeDef](./type_defs.md#stringfiltertypedef) 
33. See [:material-code-braces: StringFilterTypeDef](./type_defs.md#stringfiltertypedef) 
34. See [:material-code-braces: MapFilterTypeDef](./type_defs.md#mapfiltertypedef) 
35. See [:material-code-braces: StringFilterTypeDef](./type_defs.md#stringfiltertypedef) 
36. See [:material-code-braces: StringFilterTypeDef](./type_defs.md#stringfiltertypedef) 
37. See [:material-code-braces: StringFilterTypeDef](./type_defs.md#stringfiltertypedef) 
38. See [:material-code-braces: DateFilterTypeDef](./type_defs.md#datefiltertypedef) 
39. See [:material-code-braces: StringFilterTypeDef](./type_defs.md#stringfiltertypedef) 
40. See [:material-code-braces: StringFilterTypeDef](./type_defs.md#stringfiltertypedef) 
41. See [:material-code-braces: StringFilterTypeDef](./type_defs.md#stringfiltertypedef) 
42. See [:material-code-braces: PackageFilterTypeDef](./type_defs.md#packagefiltertypedef) 
## BatchGetFreeTrialInfoResponseTypeDef

```python
# BatchGetFreeTrialInfoResponseTypeDef TypedDict usage example

from types_aiobotocore_inspector2.type_defs import BatchGetFreeTrialInfoResponseTypeDef


def get_value() -> BatchGetFreeTrialInfoResponseTypeDef:
    return {
        "accounts": ...,
    }


# BatchGetFreeTrialInfoResponseTypeDef definition

class BatchGetFreeTrialInfoResponseTypeDef(TypedDict):
    accounts: List[FreeTrialAccountInfoTypeDef],  # (1)
    failedAccounts: List[FreeTrialInfoErrorTypeDef],  # (2)
    ResponseMetadata: ResponseMetadataTypeDef,  # (3)
```

1. See [:material-code-braces: FreeTrialAccountInfoTypeDef](./type_defs.md#freetrialaccountinfotypedef) 
2. See [:material-code-braces: FreeTrialInfoErrorTypeDef](./type_defs.md#freetrialinfoerrortypedef) 
3. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CoveredResourceTypeDef

```python
# CoveredResourceTypeDef TypedDict usage example

from types_aiobotocore_inspector2.type_defs import CoveredResourceTypeDef


def get_value() -> CoveredResourceTypeDef:
    return {
        "accountId": ...,
    }


# CoveredResourceTypeDef definition

class CoveredResourceTypeDef(TypedDict):
    accountId: str,
    resourceId: str,
    resourceType: CoverageResourceTypeType,  # (2)
    scanType: ScanTypeType,  # (5)
    lastScannedAt: NotRequired[datetime],
    resourceMetadata: NotRequired[ResourceScanMetadataTypeDef],  # (1)
    scanMode: NotRequired[ScanModeType],  # (3)
    scanStatus: NotRequired[ScanStatusTypeDef],  # (4)
```

1. See [:material-code-braces: ResourceScanMetadataTypeDef](./type_defs.md#resourcescanmetadatatypedef) 
2. See [:material-code-brackets: CoverageResourceTypeType](./literals.md#coverageresourcetypetype) 
3. See [:material-code-brackets: ScanModeType](./literals.md#scanmodetype) 
4. See [:material-code-braces: ScanStatusTypeDef](./type_defs.md#scanstatustypedef) 
5. See [:material-code-brackets: ScanTypeType](./literals.md#scantypetype) 
## NetworkReachabilityDetailsTypeDef

```python
# NetworkReachabilityDetailsTypeDef TypedDict usage example

from types_aiobotocore_inspector2.type_defs import NetworkReachabilityDetailsTypeDef


def get_value() -> NetworkReachabilityDetailsTypeDef:
    return {
        "networkPath": ...,
    }


# NetworkReachabilityDetailsTypeDef definition

class NetworkReachabilityDetailsTypeDef(TypedDict):
    networkPath: NetworkPathTypeDef,  # (1)
    openPortRange: PortRangeTypeDef,  # (2)
    protocol: NetworkProtocolType,  # (3)
```

1. See [:material-code-braces: NetworkPathTypeDef](./type_defs.md#networkpathtypedef) 
2. See [:material-code-braces: PortRangeTypeDef](./type_defs.md#portrangetypedef) 
3. See [:material-code-brackets: NetworkProtocolType](./literals.md#networkprotocoltype) 
## GetSbomExportResponseTypeDef

```python
# GetSbomExportResponseTypeDef TypedDict usage example

from types_aiobotocore_inspector2.type_defs import GetSbomExportResponseTypeDef


def get_value() -> GetSbomExportResponseTypeDef:
    return {
        "errorCode": ...,
    }


# GetSbomExportResponseTypeDef definition

class GetSbomExportResponseTypeDef(TypedDict):
    errorCode: ReportingErrorCodeType,  # (1)
    errorMessage: str,
    filterCriteria: ResourceFilterCriteriaOutputTypeDef,  # (2)
    format: SbomReportFormatType,  # (3)
    reportId: str,
    s3Destination: DestinationTypeDef,  # (4)
    status: ExternalReportStatusType,  # (5)
    ResponseMetadata: ResponseMetadataTypeDef,  # (6)
```

1. See [:material-code-brackets: ReportingErrorCodeType](./literals.md#reportingerrorcodetype) 
2. See [:material-code-braces: ResourceFilterCriteriaOutputTypeDef](./type_defs.md#resourcefiltercriteriaoutputtypedef) 
3. See [:material-code-brackets: SbomReportFormatType](./literals.md#sbomreportformattype) 
4. See [:material-code-braces: DestinationTypeDef](./type_defs.md#destinationtypedef) 
5. See [:material-code-brackets: ExternalReportStatusType](./literals.md#externalreportstatustype) 
6. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## StopCisSessionRequestTypeDef

```python
# StopCisSessionRequestTypeDef TypedDict usage example

from types_aiobotocore_inspector2.type_defs import StopCisSessionRequestTypeDef


def get_value() -> StopCisSessionRequestTypeDef:
    return {
        "message": ...,
    }


# StopCisSessionRequestTypeDef definition

class StopCisSessionRequestTypeDef(TypedDict):
    message: StopCisSessionMessageTypeDef,  # (1)
    scanJobId: str,
    sessionToken: str,
```

1. See [:material-code-braces: StopCisSessionMessageTypeDef](./type_defs.md#stopcissessionmessagetypedef) 
## ListUsageTotalsResponseTypeDef

```python
# ListUsageTotalsResponseTypeDef TypedDict usage example

from types_aiobotocore_inspector2.type_defs import ListUsageTotalsResponseTypeDef


def get_value() -> ListUsageTotalsResponseTypeDef:
    return {
        "nextToken": ...,
    }


# ListUsageTotalsResponseTypeDef definition

class ListUsageTotalsResponseTypeDef(TypedDict):
    totals: List[UsageTotalTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    nextToken: NotRequired[str],
```

1. See [:material-code-braces: UsageTotalTypeDef](./type_defs.md#usagetotaltypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListFindingAggregationsResponseTypeDef

```python
# ListFindingAggregationsResponseTypeDef TypedDict usage example

from types_aiobotocore_inspector2.type_defs import ListFindingAggregationsResponseTypeDef


def get_value() -> ListFindingAggregationsResponseTypeDef:
    return {
        "aggregationType": ...,
    }


# ListFindingAggregationsResponseTypeDef definition

class ListFindingAggregationsResponseTypeDef(TypedDict):
    aggregationType: AggregationTypeType,  # (1)
    responses: List[AggregationResponseTypeDef],  # (2)
    ResponseMetadata: ResponseMetadataTypeDef,  # (3)
    nextToken: NotRequired[str],
```

1. See [:material-code-brackets: AggregationTypeType](./literals.md#aggregationtypetype) 
2. See [:material-code-braces: AggregationResponseTypeDef](./type_defs.md#aggregationresponsetypedef) 
3. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## BatchGetAccountStatusResponseTypeDef

```python
# BatchGetAccountStatusResponseTypeDef TypedDict usage example

from types_aiobotocore_inspector2.type_defs import BatchGetAccountStatusResponseTypeDef


def get_value() -> BatchGetAccountStatusResponseTypeDef:
    return {
        "accounts": ...,
    }


# BatchGetAccountStatusResponseTypeDef definition

class BatchGetAccountStatusResponseTypeDef(TypedDict):
    accounts: List[AccountStateTypeDef],  # (1)
    failedAccounts: List[FailedAccountTypeDef],  # (2)
    ResponseMetadata: ResponseMetadataTypeDef,  # (3)
```

1. See [:material-code-braces: AccountStateTypeDef](./type_defs.md#accountstatetypedef) 
2. See [:material-code-braces: FailedAccountTypeDef](./type_defs.md#failedaccounttypedef) 
3. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ResourceTypeDef

```python
# ResourceTypeDef TypedDict usage example

from types_aiobotocore_inspector2.type_defs import ResourceTypeDef


def get_value() -> ResourceTypeDef:
    return {
        "details": ...,
    }


# ResourceTypeDef definition

class ResourceTypeDef(TypedDict):
    id: str,
    type: ResourceTypeType,  # (2)
    details: NotRequired[ResourceDetailsTypeDef],  # (1)
    partition: NotRequired[str],
    region: NotRequired[str],
    tags: NotRequired[Dict[str, str]],
```

1. See [:material-code-braces: ResourceDetailsTypeDef](./type_defs.md#resourcedetailstypedef) 
2. See [:material-code-brackets: ResourceTypeType](./literals.md#resourcetypetype) 
## ListCisScansRequestPaginateTypeDef

```python
# ListCisScansRequestPaginateTypeDef TypedDict usage example

from types_aiobotocore_inspector2.type_defs import ListCisScansRequestPaginateTypeDef


def get_value() -> ListCisScansRequestPaginateTypeDef:
    return {
        "detailLevel": ...,
    }


# ListCisScansRequestPaginateTypeDef definition

class ListCisScansRequestPaginateTypeDef(TypedDict):
    detailLevel: NotRequired[ListCisScansDetailLevelType],  # (1)
    filterCriteria: NotRequired[ListCisScansFilterCriteriaTypeDef],  # (2)
    sortBy: NotRequired[ListCisScansSortByType],  # (3)
    sortOrder: NotRequired[CisSortOrderType],  # (4)
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (5)
```

1. See [:material-code-brackets: ListCisScansDetailLevelType](./literals.md#listcisscansdetailleveltype) 
2. See [:material-code-braces: ListCisScansFilterCriteriaTypeDef](./type_defs.md#listcisscansfiltercriteriatypedef) 
3. See [:material-code-brackets: ListCisScansSortByType](./literals.md#listcisscanssortbytype) 
4. See [:material-code-brackets: CisSortOrderType](./literals.md#cissortordertype) 
5. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListCisScansRequestTypeDef

```python
# ListCisScansRequestTypeDef TypedDict usage example

from types_aiobotocore_inspector2.type_defs import ListCisScansRequestTypeDef


def get_value() -> ListCisScansRequestTypeDef:
    return {
        "detailLevel": ...,
    }


# ListCisScansRequestTypeDef definition

class ListCisScansRequestTypeDef(TypedDict):
    detailLevel: NotRequired[ListCisScansDetailLevelType],  # (1)
    filterCriteria: NotRequired[ListCisScansFilterCriteriaTypeDef],  # (2)
    maxResults: NotRequired[int],
    nextToken: NotRequired[str],
    sortBy: NotRequired[ListCisScansSortByType],  # (3)
    sortOrder: NotRequired[CisSortOrderType],  # (4)
```

1. See [:material-code-brackets: ListCisScansDetailLevelType](./literals.md#listcisscansdetailleveltype) 
2. See [:material-code-braces: ListCisScansFilterCriteriaTypeDef](./type_defs.md#listcisscansfiltercriteriatypedef) 
3. See [:material-code-brackets: ListCisScansSortByType](./literals.md#listcisscanssortbytype) 
4. See [:material-code-brackets: CisSortOrderType](./literals.md#cissortordertype) 
## ListCoverageRequestPaginateTypeDef

```python
# ListCoverageRequestPaginateTypeDef TypedDict usage example

from types_aiobotocore_inspector2.type_defs import ListCoverageRequestPaginateTypeDef


def get_value() -> ListCoverageRequestPaginateTypeDef:
    return {
        "filterCriteria": ...,
    }


# ListCoverageRequestPaginateTypeDef definition

class ListCoverageRequestPaginateTypeDef(TypedDict):
    filterCriteria: NotRequired[CoverageFilterCriteriaTypeDef],  # (1)
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (2)
```

1. See [:material-code-braces: CoverageFilterCriteriaTypeDef](./type_defs.md#coveragefiltercriteriatypedef) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListCoverageRequestTypeDef

```python
# ListCoverageRequestTypeDef TypedDict usage example

from types_aiobotocore_inspector2.type_defs import ListCoverageRequestTypeDef


def get_value() -> ListCoverageRequestTypeDef:
    return {
        "filterCriteria": ...,
    }


# ListCoverageRequestTypeDef definition

class ListCoverageRequestTypeDef(TypedDict):
    filterCriteria: NotRequired[CoverageFilterCriteriaTypeDef],  # (1)
    maxResults: NotRequired[int],
    nextToken: NotRequired[str],
```

1. See [:material-code-braces: CoverageFilterCriteriaTypeDef](./type_defs.md#coveragefiltercriteriatypedef) 
## ListCoverageStatisticsRequestPaginateTypeDef

```python
# ListCoverageStatisticsRequestPaginateTypeDef TypedDict usage example

from types_aiobotocore_inspector2.type_defs import ListCoverageStatisticsRequestPaginateTypeDef


def get_value() -> ListCoverageStatisticsRequestPaginateTypeDef:
    return {
        "filterCriteria": ...,
    }


# ListCoverageStatisticsRequestPaginateTypeDef definition

class ListCoverageStatisticsRequestPaginateTypeDef(TypedDict):
    filterCriteria: NotRequired[CoverageFilterCriteriaTypeDef],  # (1)
    groupBy: NotRequired[GroupKeyType],  # (2)
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (3)
```

1. See [:material-code-braces: CoverageFilterCriteriaTypeDef](./type_defs.md#coveragefiltercriteriatypedef) 
2. See [:material-code-brackets: GroupKeyType](./literals.md#groupkeytype) 
3. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListCoverageStatisticsRequestTypeDef

```python
# ListCoverageStatisticsRequestTypeDef TypedDict usage example

from types_aiobotocore_inspector2.type_defs import ListCoverageStatisticsRequestTypeDef


def get_value() -> ListCoverageStatisticsRequestTypeDef:
    return {
        "filterCriteria": ...,
    }


# ListCoverageStatisticsRequestTypeDef definition

class ListCoverageStatisticsRequestTypeDef(TypedDict):
    filterCriteria: NotRequired[CoverageFilterCriteriaTypeDef],  # (1)
    groupBy: NotRequired[GroupKeyType],  # (2)
    nextToken: NotRequired[str],
```

1. See [:material-code-braces: CoverageFilterCriteriaTypeDef](./type_defs.md#coveragefiltercriteriatypedef) 
2. See [:material-code-brackets: GroupKeyType](./literals.md#groupkeytype) 
## CisScanConfigurationTypeDef

```python
# CisScanConfigurationTypeDef TypedDict usage example

from types_aiobotocore_inspector2.type_defs import CisScanConfigurationTypeDef


def get_value() -> CisScanConfigurationTypeDef:
    return {
        "ownerId": ...,
    }


# CisScanConfigurationTypeDef definition

class CisScanConfigurationTypeDef(TypedDict):
    scanConfigurationArn: str,
    ownerId: NotRequired[str],
    scanName: NotRequired[str],
    schedule: NotRequired[ScheduleOutputTypeDef],  # (1)
    securityLevel: NotRequired[CisSecurityLevelType],  # (2)
    tags: NotRequired[Dict[str, str]],
    targets: NotRequired[CisTargetsTypeDef],  # (3)
```

1. See [:material-code-braces: ScheduleOutputTypeDef](./type_defs.md#scheduleoutputtypedef) 
2. See [:material-code-brackets: CisSecurityLevelType](./literals.md#cissecurityleveltype) 
3. See [:material-code-braces: CisTargetsTypeDef](./type_defs.md#cistargetstypedef) 
## ListFindingAggregationsRequestPaginateTypeDef

```python
# ListFindingAggregationsRequestPaginateTypeDef TypedDict usage example

from types_aiobotocore_inspector2.type_defs import ListFindingAggregationsRequestPaginateTypeDef


def get_value() -> ListFindingAggregationsRequestPaginateTypeDef:
    return {
        "aggregationType": ...,
    }


# ListFindingAggregationsRequestPaginateTypeDef definition

class ListFindingAggregationsRequestPaginateTypeDef(TypedDict):
    aggregationType: AggregationTypeType,  # (1)
    accountIds: NotRequired[Sequence[StringFilterTypeDef]],  # (2)
    aggregationRequest: NotRequired[AggregationRequestTypeDef],  # (3)
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (4)
```

1. See [:material-code-brackets: AggregationTypeType](./literals.md#aggregationtypetype) 
2. See [:material-code-braces: StringFilterTypeDef](./type_defs.md#stringfiltertypedef) 
3. See [:material-code-braces: AggregationRequestTypeDef](./type_defs.md#aggregationrequesttypedef) 
4. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListFindingAggregationsRequestTypeDef

```python
# ListFindingAggregationsRequestTypeDef TypedDict usage example

from types_aiobotocore_inspector2.type_defs import ListFindingAggregationsRequestTypeDef


def get_value() -> ListFindingAggregationsRequestTypeDef:
    return {
        "aggregationType": ...,
    }


# ListFindingAggregationsRequestTypeDef definition

class ListFindingAggregationsRequestTypeDef(TypedDict):
    aggregationType: AggregationTypeType,  # (1)
    accountIds: NotRequired[Sequence[StringFilterTypeDef]],  # (2)
    aggregationRequest: NotRequired[AggregationRequestTypeDef],  # (3)
    maxResults: NotRequired[int],
    nextToken: NotRequired[str],
```

1. See [:material-code-brackets: AggregationTypeType](./literals.md#aggregationtypetype) 
2. See [:material-code-braces: StringFilterTypeDef](./type_defs.md#stringfiltertypedef) 
3. See [:material-code-braces: AggregationRequestTypeDef](./type_defs.md#aggregationrequesttypedef) 
## FilterTypeDef

```python
# FilterTypeDef TypedDict usage example

from types_aiobotocore_inspector2.type_defs import FilterTypeDef


def get_value() -> FilterTypeDef:
    return {
        "action": ...,
    }


# FilterTypeDef definition

class FilterTypeDef(TypedDict):
    action: FilterActionType,  # (1)
    arn: str,
    createdAt: datetime,
    criteria: FilterCriteriaOutputTypeDef,  # (2)
    name: str,
    ownerId: str,
    updatedAt: datetime,
    description: NotRequired[str],
    reason: NotRequired[str],
    tags: NotRequired[Dict[str, str]],
```

1. See [:material-code-brackets: FilterActionType](./literals.md#filteractiontype) 
2. See [:material-code-braces: FilterCriteriaOutputTypeDef](./type_defs.md#filtercriteriaoutputtypedef) 
## GetFindingsReportStatusResponseTypeDef

```python
# GetFindingsReportStatusResponseTypeDef TypedDict usage example

from types_aiobotocore_inspector2.type_defs import GetFindingsReportStatusResponseTypeDef


def get_value() -> GetFindingsReportStatusResponseTypeDef:
    return {
        "destination": ...,
    }


# GetFindingsReportStatusResponseTypeDef definition

class GetFindingsReportStatusResponseTypeDef(TypedDict):
    destination: DestinationTypeDef,  # (1)
    errorCode: ReportingErrorCodeType,  # (2)
    errorMessage: str,
    filterCriteria: FilterCriteriaOutputTypeDef,  # (3)
    reportId: str,
    status: ExternalReportStatusType,  # (4)
    ResponseMetadata: ResponseMetadataTypeDef,  # (5)
```

1. See [:material-code-braces: DestinationTypeDef](./type_defs.md#destinationtypedef) 
2. See [:material-code-brackets: ReportingErrorCodeType](./literals.md#reportingerrorcodetype) 
3. See [:material-code-braces: FilterCriteriaOutputTypeDef](./type_defs.md#filtercriteriaoutputtypedef) 
4. See [:material-code-brackets: ExternalReportStatusType](./literals.md#externalreportstatustype) 
5. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListCoverageResponseTypeDef

```python
# ListCoverageResponseTypeDef TypedDict usage example

from types_aiobotocore_inspector2.type_defs import ListCoverageResponseTypeDef


def get_value() -> ListCoverageResponseTypeDef:
    return {
        "coveredResources": ...,
    }


# ListCoverageResponseTypeDef definition

class ListCoverageResponseTypeDef(TypedDict):
    coveredResources: List[CoveredResourceTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    nextToken: NotRequired[str],
```

1. See [:material-code-braces: CoveredResourceTypeDef](./type_defs.md#coveredresourcetypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateSbomExportRequestTypeDef

```python
# CreateSbomExportRequestTypeDef TypedDict usage example

from types_aiobotocore_inspector2.type_defs import CreateSbomExportRequestTypeDef


def get_value() -> CreateSbomExportRequestTypeDef:
    return {
        "reportFormat": ...,
    }


# CreateSbomExportRequestTypeDef definition

class CreateSbomExportRequestTypeDef(TypedDict):
    reportFormat: SbomReportFormatType,  # (1)
    s3Destination: DestinationTypeDef,  # (2)
    resourceFilterCriteria: NotRequired[ResourceFilterCriteriaUnionTypeDef],  # (3)
```

1. See [:material-code-brackets: SbomReportFormatType](./literals.md#sbomreportformattype) 
2. See [:material-code-braces: DestinationTypeDef](./type_defs.md#destinationtypedef) 
3. See [:material-code-braces: ResourceFilterCriteriaTypeDef](./type_defs.md#resourcefiltercriteriatypedef) [:material-code-braces: ResourceFilterCriteriaOutputTypeDef](./type_defs.md#resourcefiltercriteriaoutputtypedef) 
## FindingTypeDef

```python
# FindingTypeDef TypedDict usage example

from types_aiobotocore_inspector2.type_defs import FindingTypeDef


def get_value() -> FindingTypeDef:
    return {
        "awsAccountId": ...,
    }


# FindingTypeDef definition

class FindingTypeDef(TypedDict):
    awsAccountId: str,
    description: str,
    findingArn: str,
    firstObservedAt: datetime,
    lastObservedAt: datetime,
    remediation: RemediationTypeDef,  # (9)
    resources: List[ResourceTypeDef],  # (10)
    severity: SeverityType,  # (11)
    status: FindingStatusType,  # (12)
    type: FindingTypeType,  # (13)
    codeVulnerabilityDetails: NotRequired[CodeVulnerabilityDetailsTypeDef],  # (1)
    epss: NotRequired[EpssDetailsTypeDef],  # (2)
    exploitAvailable: NotRequired[ExploitAvailableType],  # (3)
    exploitabilityDetails: NotRequired[ExploitabilityDetailsTypeDef],  # (4)
    fixAvailable: NotRequired[FixAvailableType],  # (5)
    inspectorScore: NotRequired[float],
    inspectorScoreDetails: NotRequired[InspectorScoreDetailsTypeDef],  # (6)
    networkReachabilityDetails: NotRequired[NetworkReachabilityDetailsTypeDef],  # (7)
    packageVulnerabilityDetails: NotRequired[PackageVulnerabilityDetailsTypeDef],  # (8)
    title: NotRequired[str],
    updatedAt: NotRequired[datetime],
```

1. See [:material-code-braces: CodeVulnerabilityDetailsTypeDef](./type_defs.md#codevulnerabilitydetailstypedef) 
2. See [:material-code-braces: EpssDetailsTypeDef](./type_defs.md#epssdetailstypedef) 
3. See [:material-code-brackets: ExploitAvailableType](./literals.md#exploitavailabletype) 
4. See [:material-code-braces: ExploitabilityDetailsTypeDef](./type_defs.md#exploitabilitydetailstypedef) 
5. See [:material-code-brackets: FixAvailableType](./literals.md#fixavailabletype) 
6. See [:material-code-braces: InspectorScoreDetailsTypeDef](./type_defs.md#inspectorscoredetailstypedef) 
7. See [:material-code-braces: NetworkReachabilityDetailsTypeDef](./type_defs.md#networkreachabilitydetailstypedef) 
8. See [:material-code-braces: PackageVulnerabilityDetailsTypeDef](./type_defs.md#packagevulnerabilitydetailstypedef) 
9. See [:material-code-braces: RemediationTypeDef](./type_defs.md#remediationtypedef) 
10. See [:material-code-braces: ResourceTypeDef](./type_defs.md#resourcetypedef) 
11. See [:material-code-brackets: SeverityType](./literals.md#severitytype) 
12. See [:material-code-brackets: FindingStatusType](./literals.md#findingstatustype) 
13. See [:material-code-brackets: FindingTypeType](./literals.md#findingtypetype) 
## ListCisScanConfigurationsResponseTypeDef

```python
# ListCisScanConfigurationsResponseTypeDef TypedDict usage example

from types_aiobotocore_inspector2.type_defs import ListCisScanConfigurationsResponseTypeDef


def get_value() -> ListCisScanConfigurationsResponseTypeDef:
    return {
        "nextToken": ...,
    }


# ListCisScanConfigurationsResponseTypeDef definition

class ListCisScanConfigurationsResponseTypeDef(TypedDict):
    scanConfigurations: List[CisScanConfigurationTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    nextToken: NotRequired[str],
```

1. See [:material-code-braces: CisScanConfigurationTypeDef](./type_defs.md#cisscanconfigurationtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateCisScanConfigurationRequestTypeDef

```python
# CreateCisScanConfigurationRequestTypeDef TypedDict usage example

from types_aiobotocore_inspector2.type_defs import CreateCisScanConfigurationRequestTypeDef


def get_value() -> CreateCisScanConfigurationRequestTypeDef:
    return {
        "scanName": ...,
    }


# CreateCisScanConfigurationRequestTypeDef definition

class CreateCisScanConfigurationRequestTypeDef(TypedDict):
    scanName: str,
    schedule: ScheduleUnionTypeDef,  # (1)
    securityLevel: CisSecurityLevelType,  # (2)
    targets: CreateCisTargetsTypeDef,  # (3)
    tags: NotRequired[Mapping[str, str]],
```

1. See [:material-code-braces: ScheduleTypeDef](./type_defs.md#scheduletypedef) [:material-code-braces: ScheduleOutputTypeDef](./type_defs.md#scheduleoutputtypedef) 
2. See [:material-code-brackets: CisSecurityLevelType](./literals.md#cissecurityleveltype) 
3. See [:material-code-braces: CreateCisTargetsTypeDef](./type_defs.md#createcistargetstypedef) 
## UpdateCisScanConfigurationRequestTypeDef

```python
# UpdateCisScanConfigurationRequestTypeDef TypedDict usage example

from types_aiobotocore_inspector2.type_defs import UpdateCisScanConfigurationRequestTypeDef


def get_value() -> UpdateCisScanConfigurationRequestTypeDef:
    return {
        "scanConfigurationArn": ...,
    }


# UpdateCisScanConfigurationRequestTypeDef definition

class UpdateCisScanConfigurationRequestTypeDef(TypedDict):
    scanConfigurationArn: str,
    scanName: NotRequired[str],
    schedule: NotRequired[ScheduleUnionTypeDef],  # (1)
    securityLevel: NotRequired[CisSecurityLevelType],  # (2)
    targets: NotRequired[UpdateCisTargetsTypeDef],  # (3)
```

1. See [:material-code-braces: ScheduleTypeDef](./type_defs.md#scheduletypedef) [:material-code-braces: ScheduleOutputTypeDef](./type_defs.md#scheduleoutputtypedef) 
2. See [:material-code-brackets: CisSecurityLevelType](./literals.md#cissecurityleveltype) 
3. See [:material-code-braces: UpdateCisTargetsTypeDef](./type_defs.md#updatecistargetstypedef) 
## ListFiltersResponseTypeDef

```python
# ListFiltersResponseTypeDef TypedDict usage example

from types_aiobotocore_inspector2.type_defs import ListFiltersResponseTypeDef


def get_value() -> ListFiltersResponseTypeDef:
    return {
        "filters": ...,
    }


# ListFiltersResponseTypeDef definition

class ListFiltersResponseTypeDef(TypedDict):
    filters: List[FilterTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    nextToken: NotRequired[str],
```

1. See [:material-code-braces: FilterTypeDef](./type_defs.md#filtertypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateFilterRequestTypeDef

```python
# CreateFilterRequestTypeDef TypedDict usage example

from types_aiobotocore_inspector2.type_defs import CreateFilterRequestTypeDef


def get_value() -> CreateFilterRequestTypeDef:
    return {
        "action": ...,
    }


# CreateFilterRequestTypeDef definition

class CreateFilterRequestTypeDef(TypedDict):
    action: FilterActionType,  # (1)
    filterCriteria: FilterCriteriaUnionTypeDef,  # (2)
    name: str,
    description: NotRequired[str],
    reason: NotRequired[str],
    tags: NotRequired[Mapping[str, str]],
```

1. See [:material-code-brackets: FilterActionType](./literals.md#filteractiontype) 
2. See [:material-code-braces: FilterCriteriaTypeDef](./type_defs.md#filtercriteriatypedef) [:material-code-braces: FilterCriteriaOutputTypeDef](./type_defs.md#filtercriteriaoutputtypedef) 
## CreateFindingsReportRequestTypeDef

```python
# CreateFindingsReportRequestTypeDef TypedDict usage example

from types_aiobotocore_inspector2.type_defs import CreateFindingsReportRequestTypeDef


def get_value() -> CreateFindingsReportRequestTypeDef:
    return {
        "reportFormat": ...,
    }


# CreateFindingsReportRequestTypeDef definition

class CreateFindingsReportRequestTypeDef(TypedDict):
    reportFormat: ReportFormatType,  # (1)
    s3Destination: DestinationTypeDef,  # (2)
    filterCriteria: NotRequired[FilterCriteriaUnionTypeDef],  # (3)
```

1. See [:material-code-brackets: ReportFormatType](./literals.md#reportformattype) 
2. See [:material-code-braces: DestinationTypeDef](./type_defs.md#destinationtypedef) 
3. See [:material-code-braces: FilterCriteriaTypeDef](./type_defs.md#filtercriteriatypedef) [:material-code-braces: FilterCriteriaOutputTypeDef](./type_defs.md#filtercriteriaoutputtypedef) 
## ListFindingsRequestPaginateTypeDef

```python
# ListFindingsRequestPaginateTypeDef TypedDict usage example

from types_aiobotocore_inspector2.type_defs import ListFindingsRequestPaginateTypeDef


def get_value() -> ListFindingsRequestPaginateTypeDef:
    return {
        "filterCriteria": ...,
    }


# ListFindingsRequestPaginateTypeDef definition

class ListFindingsRequestPaginateTypeDef(TypedDict):
    filterCriteria: NotRequired[FilterCriteriaUnionTypeDef],  # (1)
    sortCriteria: NotRequired[SortCriteriaTypeDef],  # (2)
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (3)
```

1. See [:material-code-braces: FilterCriteriaTypeDef](./type_defs.md#filtercriteriatypedef) [:material-code-braces: FilterCriteriaOutputTypeDef](./type_defs.md#filtercriteriaoutputtypedef) 
2. See [:material-code-braces: SortCriteriaTypeDef](./type_defs.md#sortcriteriatypedef) 
3. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListFindingsRequestTypeDef

```python
# ListFindingsRequestTypeDef TypedDict usage example

from types_aiobotocore_inspector2.type_defs import ListFindingsRequestTypeDef


def get_value() -> ListFindingsRequestTypeDef:
    return {
        "filterCriteria": ...,
    }


# ListFindingsRequestTypeDef definition

class ListFindingsRequestTypeDef(TypedDict):
    filterCriteria: NotRequired[FilterCriteriaUnionTypeDef],  # (1)
    maxResults: NotRequired[int],
    nextToken: NotRequired[str],
    sortCriteria: NotRequired[SortCriteriaTypeDef],  # (2)
```

1. See [:material-code-braces: FilterCriteriaTypeDef](./type_defs.md#filtercriteriatypedef) [:material-code-braces: FilterCriteriaOutputTypeDef](./type_defs.md#filtercriteriaoutputtypedef) 
2. See [:material-code-braces: SortCriteriaTypeDef](./type_defs.md#sortcriteriatypedef) 
## UpdateFilterRequestTypeDef

```python
# UpdateFilterRequestTypeDef TypedDict usage example

from types_aiobotocore_inspector2.type_defs import UpdateFilterRequestTypeDef


def get_value() -> UpdateFilterRequestTypeDef:
    return {
        "filterArn": ...,
    }


# UpdateFilterRequestTypeDef definition

class UpdateFilterRequestTypeDef(TypedDict):
    filterArn: str,
    action: NotRequired[FilterActionType],  # (1)
    description: NotRequired[str],
    filterCriteria: NotRequired[FilterCriteriaUnionTypeDef],  # (2)
    name: NotRequired[str],
    reason: NotRequired[str],
```

1. See [:material-code-brackets: FilterActionType](./literals.md#filteractiontype) 
2. See [:material-code-braces: FilterCriteriaTypeDef](./type_defs.md#filtercriteriatypedef) [:material-code-braces: FilterCriteriaOutputTypeDef](./type_defs.md#filtercriteriaoutputtypedef) 
## ListFindingsResponseTypeDef

```python
# ListFindingsResponseTypeDef TypedDict usage example

from types_aiobotocore_inspector2.type_defs import ListFindingsResponseTypeDef


def get_value() -> ListFindingsResponseTypeDef:
    return {
        "findings": ...,
    }


# ListFindingsResponseTypeDef definition

class ListFindingsResponseTypeDef(TypedDict):
    findings: List[FindingTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    nextToken: NotRequired[str],
```

1. See [:material-code-braces: FindingTypeDef](./type_defs.md#findingtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
