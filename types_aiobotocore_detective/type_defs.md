<a id="typed-dictionaries-for-aiobotocore-detective-module"></a>

# Typed dictionaries for aiobotocore Detective module

> [Index](..) > [Detective](.) > Typed dictionaries

Auto-generated documentation for
[Detective](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/detective.html#Detective)
type annotations stubs module
[types-aiobotocore-detective](https://pypi.org/project/types-aiobotocore-detective/).

- [Typed dictionaries for aiobotocore Detective module](#typed-dictionaries-for-aiobotocore-detective-module)
  - [AcceptInvitationRequestRequestTypeDef](#acceptinvitationrequestrequesttypedef)
  - [AccountTypeDef](#accounttypedef)
  - [CreateGraphRequestRequestTypeDef](#creategraphrequestrequesttypedef)
  - [CreateGraphResponseTypeDef](#creategraphresponsetypedef)
  - [CreateMembersRequestRequestTypeDef](#createmembersrequestrequesttypedef)
  - [CreateMembersResponseTypeDef](#createmembersresponsetypedef)
  - [DeleteGraphRequestRequestTypeDef](#deletegraphrequestrequesttypedef)
  - [DeleteMembersRequestRequestTypeDef](#deletemembersrequestrequesttypedef)
  - [DeleteMembersResponseTypeDef](#deletemembersresponsetypedef)
  - [DisassociateMembershipRequestRequestTypeDef](#disassociatemembershiprequestrequesttypedef)
  - [GetMembersRequestRequestTypeDef](#getmembersrequestrequesttypedef)
  - [GetMembersResponseTypeDef](#getmembersresponsetypedef)
  - [GraphTypeDef](#graphtypedef)
  - [ListGraphsRequestRequestTypeDef](#listgraphsrequestrequesttypedef)
  - [ListGraphsResponseTypeDef](#listgraphsresponsetypedef)
  - [ListInvitationsRequestRequestTypeDef](#listinvitationsrequestrequesttypedef)
  - [ListInvitationsResponseTypeDef](#listinvitationsresponsetypedef)
  - [ListMembersRequestRequestTypeDef](#listmembersrequestrequesttypedef)
  - [ListMembersResponseTypeDef](#listmembersresponsetypedef)
  - [ListTagsForResourceRequestRequestTypeDef](#listtagsforresourcerequestrequesttypedef)
  - [ListTagsForResourceResponseTypeDef](#listtagsforresourceresponsetypedef)
  - [MemberDetailTypeDef](#memberdetailtypedef)
  - [RejectInvitationRequestRequestTypeDef](#rejectinvitationrequestrequesttypedef)
  - [ResponseMetadataTypeDef](#responsemetadatatypedef)
  - [StartMonitoringMemberRequestRequestTypeDef](#startmonitoringmemberrequestrequesttypedef)
  - [TagResourceRequestRequestTypeDef](#tagresourcerequestrequesttypedef)
  - [UnprocessedAccountTypeDef](#unprocessedaccounttypedef)
  - [UntagResourceRequestRequestTypeDef](#untagresourcerequestrequesttypedef)

<a id="acceptinvitationrequestrequesttypedef"></a>

## AcceptInvitationRequestRequestTypeDef

```python
from types_aiobotocore_detective.type_defs import AcceptInvitationRequestRequestTypeDef
```

Required fields:

- `GraphArn`: `str`

<a id="accounttypedef"></a>

## AccountTypeDef

```python
from types_aiobotocore_detective.type_defs import AccountTypeDef
```

Required fields:

- `AccountId`: `str`
- `EmailAddress`: `str`

<a id="creategraphrequestrequesttypedef"></a>

## CreateGraphRequestRequestTypeDef

```python
from types_aiobotocore_detective.type_defs import CreateGraphRequestRequestTypeDef
```

Optional fields:

- `Tags`: `Mapping`\[`str`, `str`\]

<a id="creategraphresponsetypedef"></a>

## CreateGraphResponseTypeDef

```python
from types_aiobotocore_detective.type_defs import CreateGraphResponseTypeDef
```

Required fields:

- `GraphArn`: `str`
- `ResponseMetadata`:
  [ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef)

<a id="createmembersrequestrequesttypedef"></a>

## CreateMembersRequestRequestTypeDef

```python
from types_aiobotocore_detective.type_defs import CreateMembersRequestRequestTypeDef
```

Required fields:

- `GraphArn`: `str`
- `Accounts`: `Sequence`\[[AccountTypeDef](./type_defs.md#accounttypedef)\]

Optional fields:

- `Message`: `str`
- `DisableEmailNotification`: `bool`

<a id="createmembersresponsetypedef"></a>

## CreateMembersResponseTypeDef

```python
from types_aiobotocore_detective.type_defs import CreateMembersResponseTypeDef
```

Required fields:

- `Members`:
  `List`\[[MemberDetailTypeDef](./type_defs.md#memberdetailtypedef)\]
- `UnprocessedAccounts`:
  `List`\[[UnprocessedAccountTypeDef](./type_defs.md#unprocessedaccounttypedef)\]
- `ResponseMetadata`:
  [ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef)

<a id="deletegraphrequestrequesttypedef"></a>

## DeleteGraphRequestRequestTypeDef

```python
from types_aiobotocore_detective.type_defs import DeleteGraphRequestRequestTypeDef
```

Required fields:

- `GraphArn`: `str`

<a id="deletemembersrequestrequesttypedef"></a>

## DeleteMembersRequestRequestTypeDef

```python
from types_aiobotocore_detective.type_defs import DeleteMembersRequestRequestTypeDef
```

Required fields:

- `GraphArn`: `str`
- `AccountIds`: `Sequence`\[`str`\]

<a id="deletemembersresponsetypedef"></a>

## DeleteMembersResponseTypeDef

```python
from types_aiobotocore_detective.type_defs import DeleteMembersResponseTypeDef
```

Required fields:

- `AccountIds`: `List`\[`str`\]
- `UnprocessedAccounts`:
  `List`\[[UnprocessedAccountTypeDef](./type_defs.md#unprocessedaccounttypedef)\]
- `ResponseMetadata`:
  [ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef)

<a id="disassociatemembershiprequestrequesttypedef"></a>

## DisassociateMembershipRequestRequestTypeDef

```python
from types_aiobotocore_detective.type_defs import DisassociateMembershipRequestRequestTypeDef
```

Required fields:

- `GraphArn`: `str`

<a id="getmembersrequestrequesttypedef"></a>

## GetMembersRequestRequestTypeDef

```python
from types_aiobotocore_detective.type_defs import GetMembersRequestRequestTypeDef
```

Required fields:

- `GraphArn`: `str`
- `AccountIds`: `Sequence`\[`str`\]

<a id="getmembersresponsetypedef"></a>

## GetMembersResponseTypeDef

```python
from types_aiobotocore_detective.type_defs import GetMembersResponseTypeDef
```

Required fields:

- `MemberDetails`:
  `List`\[[MemberDetailTypeDef](./type_defs.md#memberdetailtypedef)\]
- `UnprocessedAccounts`:
  `List`\[[UnprocessedAccountTypeDef](./type_defs.md#unprocessedaccounttypedef)\]
- `ResponseMetadata`:
  [ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef)

<a id="graphtypedef"></a>

## GraphTypeDef

```python
from types_aiobotocore_detective.type_defs import GraphTypeDef
```

Optional fields:

- `Arn`: `str`
- `CreatedTime`: `datetime`

<a id="listgraphsrequestrequesttypedef"></a>

## ListGraphsRequestRequestTypeDef

```python
from types_aiobotocore_detective.type_defs import ListGraphsRequestRequestTypeDef
```

Optional fields:

- `NextToken`: `str`
- `MaxResults`: `int`

<a id="listgraphsresponsetypedef"></a>

## ListGraphsResponseTypeDef

```python
from types_aiobotocore_detective.type_defs import ListGraphsResponseTypeDef
```

Required fields:

- `GraphList`: `List`\[[GraphTypeDef](./type_defs.md#graphtypedef)\]
- `NextToken`: `str`
- `ResponseMetadata`:
  [ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef)

<a id="listinvitationsrequestrequesttypedef"></a>

## ListInvitationsRequestRequestTypeDef

```python
from types_aiobotocore_detective.type_defs import ListInvitationsRequestRequestTypeDef
```

Optional fields:

- `NextToken`: `str`
- `MaxResults`: `int`

<a id="listinvitationsresponsetypedef"></a>

## ListInvitationsResponseTypeDef

```python
from types_aiobotocore_detective.type_defs import ListInvitationsResponseTypeDef
```

Required fields:

- `Invitations`:
  `List`\[[MemberDetailTypeDef](./type_defs.md#memberdetailtypedef)\]
- `NextToken`: `str`
- `ResponseMetadata`:
  [ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef)

<a id="listmembersrequestrequesttypedef"></a>

## ListMembersRequestRequestTypeDef

```python
from types_aiobotocore_detective.type_defs import ListMembersRequestRequestTypeDef
```

Required fields:

- `GraphArn`: `str`

Optional fields:

- `NextToken`: `str`
- `MaxResults`: `int`

<a id="listmembersresponsetypedef"></a>

## ListMembersResponseTypeDef

```python
from types_aiobotocore_detective.type_defs import ListMembersResponseTypeDef
```

Required fields:

- `MemberDetails`:
  `List`\[[MemberDetailTypeDef](./type_defs.md#memberdetailtypedef)\]
- `NextToken`: `str`
- `ResponseMetadata`:
  [ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef)

<a id="listtagsforresourcerequestrequesttypedef"></a>

## ListTagsForResourceRequestRequestTypeDef

```python
from types_aiobotocore_detective.type_defs import ListTagsForResourceRequestRequestTypeDef
```

Required fields:

- `ResourceArn`: `str`

<a id="listtagsforresourceresponsetypedef"></a>

## ListTagsForResourceResponseTypeDef

```python
from types_aiobotocore_detective.type_defs import ListTagsForResourceResponseTypeDef
```

Required fields:

- `Tags`: `Dict`\[`str`, `str`\]
- `ResponseMetadata`:
  [ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef)

<a id="memberdetailtypedef"></a>

## MemberDetailTypeDef

```python
from types_aiobotocore_detective.type_defs import MemberDetailTypeDef
```

Optional fields:

- `AccountId`: `str`
- `EmailAddress`: `str`
- `GraphArn`: `str`
- `MasterId`: `str`
- `AdministratorId`: `str`
- `Status`: [MemberStatusType](./literals.md#memberstatustype)
- `DisabledReason`:
  [MemberDisabledReasonType](./literals.md#memberdisabledreasontype)
- `InvitedTime`: `datetime`
- `UpdatedTime`: `datetime`
- `VolumeUsageInBytes`: `int`
- `VolumeUsageUpdatedTime`: `datetime`
- `PercentOfGraphUtilization`: `float`
- `PercentOfGraphUtilizationUpdatedTime`: `datetime`

<a id="rejectinvitationrequestrequesttypedef"></a>

## RejectInvitationRequestRequestTypeDef

```python
from types_aiobotocore_detective.type_defs import RejectInvitationRequestRequestTypeDef
```

Required fields:

- `GraphArn`: `str`

<a id="responsemetadatatypedef"></a>

## ResponseMetadataTypeDef

```python
from types_aiobotocore_detective.type_defs import ResponseMetadataTypeDef
```

Required fields:

- `RequestId`: `str`
- `HostId`: `str`
- `HTTPStatusCode`: `int`
- `HTTPHeaders`: `Dict`\[`str`, `str`\]
- `RetryAttempts`: `int`

<a id="startmonitoringmemberrequestrequesttypedef"></a>

## StartMonitoringMemberRequestRequestTypeDef

```python
from types_aiobotocore_detective.type_defs import StartMonitoringMemberRequestRequestTypeDef
```

Required fields:

- `GraphArn`: `str`
- `AccountId`: `str`

<a id="tagresourcerequestrequesttypedef"></a>

## TagResourceRequestRequestTypeDef

```python
from types_aiobotocore_detective.type_defs import TagResourceRequestRequestTypeDef
```

Required fields:

- `ResourceArn`: `str`
- `Tags`: `Mapping`\[`str`, `str`\]

<a id="unprocessedaccounttypedef"></a>

## UnprocessedAccountTypeDef

```python
from types_aiobotocore_detective.type_defs import UnprocessedAccountTypeDef
```

Optional fields:

- `AccountId`: `str`
- `Reason`: `str`

<a id="untagresourcerequestrequesttypedef"></a>

## UntagResourceRequestRequestTypeDef

```python
from types_aiobotocore_detective.type_defs import UntagResourceRequestRequestTypeDef
```

Required fields:

- `ResourceArn`: `str`
- `TagKeys`: `Sequence`\[`str`\]
