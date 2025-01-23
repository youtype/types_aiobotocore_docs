# Type definitions

> [Index](../README.md) > [SSO](./README.md) > Type definitions

!!! note ""

    Auto-generated documentation for [SSO](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sso.html#sso)
    type annotations stubs module [types-aiobotocore-sso](https://pypi.org/project/types-aiobotocore-sso/).



## AccountInfoTypeDef

```python
# AccountInfoTypeDef definition

class AccountInfoTypeDef(TypedDict):
    accountId: NotRequired[str],
    accountName: NotRequired[str],
    emailAddress: NotRequired[str],
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

## GetRoleCredentialsRequestRequestTypeDef

```python
# GetRoleCredentialsRequestRequestTypeDef definition

class GetRoleCredentialsRequestRequestTypeDef(TypedDict):
    roleName: str,
    accountId: str,
    accessToken: str,
```

## RoleCredentialsTypeDef

```python
# RoleCredentialsTypeDef definition

class RoleCredentialsTypeDef(TypedDict):
    accessKeyId: NotRequired[str],
    secretAccessKey: NotRequired[str],
    sessionToken: NotRequired[str],
    expiration: NotRequired[int],
```

## PaginatorConfigTypeDef

```python
# PaginatorConfigTypeDef definition

class PaginatorConfigTypeDef(TypedDict):
    MaxItems: NotRequired[int],
    PageSize: NotRequired[int],
    StartingToken: NotRequired[str],
```

## ListAccountRolesRequestRequestTypeDef

```python
# ListAccountRolesRequestRequestTypeDef definition

class ListAccountRolesRequestRequestTypeDef(TypedDict):
    accessToken: str,
    accountId: str,
    nextToken: NotRequired[str],
    maxResults: NotRequired[int],
```

## RoleInfoTypeDef

```python
# RoleInfoTypeDef definition

class RoleInfoTypeDef(TypedDict):
    roleName: NotRequired[str],
    accountId: NotRequired[str],
```

## ListAccountsRequestRequestTypeDef

```python
# ListAccountsRequestRequestTypeDef definition

class ListAccountsRequestRequestTypeDef(TypedDict):
    accessToken: str,
    nextToken: NotRequired[str],
    maxResults: NotRequired[int],
```

## LogoutRequestRequestTypeDef

```python
# LogoutRequestRequestTypeDef definition

class LogoutRequestRequestTypeDef(TypedDict):
    accessToken: str,
```

## EmptyResponseMetadataTypeDef

```python
# EmptyResponseMetadataTypeDef definition

class EmptyResponseMetadataTypeDef(TypedDict):
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListAccountsResponseTypeDef

```python
# ListAccountsResponseTypeDef definition

class ListAccountsResponseTypeDef(TypedDict):
    accountList: List[AccountInfoTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    nextToken: NotRequired[str],
```

1. See [:material-code-braces: AccountInfoTypeDef](./type_defs.md#accountinfotypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetRoleCredentialsResponseTypeDef

```python
# GetRoleCredentialsResponseTypeDef definition

class GetRoleCredentialsResponseTypeDef(TypedDict):
    roleCredentials: RoleCredentialsTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: RoleCredentialsTypeDef](./type_defs.md#rolecredentialstypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListAccountRolesRequestPaginateTypeDef

```python
# ListAccountRolesRequestPaginateTypeDef definition

class ListAccountRolesRequestPaginateTypeDef(TypedDict):
    accessToken: str,
    accountId: str,
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListAccountsRequestPaginateTypeDef

```python
# ListAccountsRequestPaginateTypeDef definition

class ListAccountsRequestPaginateTypeDef(TypedDict):
    accessToken: str,
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListAccountRolesResponseTypeDef

```python
# ListAccountRolesResponseTypeDef definition

class ListAccountRolesResponseTypeDef(TypedDict):
    roleList: List[RoleInfoTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    nextToken: NotRequired[str],
```

1. See [:material-code-braces: RoleInfoTypeDef](./type_defs.md#roleinfotypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
