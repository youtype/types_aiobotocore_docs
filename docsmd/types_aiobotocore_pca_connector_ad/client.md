# PcaConnectorAdClient

> [Index](../README.md) > [PcaConnectorAd](./README.md) > PcaConnectorAdClient

!!! note ""

    Auto-generated documentation for [PcaConnectorAd](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pca-connector-ad.html#pcaconnectorad)
    type annotations stubs module [types-aiobotocore-pca-connector-ad](https://pypi.org/project/types-aiobotocore-pca-connector-ad/).

## PcaConnectorAdClient

Type annotations and code completion for `#!python session.create_client("pca-connector-ad")`
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pca-connector-ad.html#PcaConnectorAd.Client)

```python
# PcaConnectorAdClient usage example

from aiobotocore.session import get_session
from types_aiobotocore_pca_connector_ad.client import PcaConnectorAdClient

session = get_session()
async with session.create_client("pca-connector-ad") as client:
    client: PcaConnectorAdClient
```

## Exceptions


`aiobotocore` client exceptions are generated in runtime.
This class provides code completion for `#!python session.create_client("pca-connector-ad").exceptions` structure.

```python
# PcaConnectorAdClient.exceptions usage example

async with session.create_client("pca-connector-ad") as client:
    try:
        do_something(client)
    except (
            client.AccessDeniedException,
        client.ClientError,
        client.ConflictException,
        client.InternalServerException,
        client.ResourceNotFoundException,
        client.ServiceQuotaExceededException,
        client.ThrottlingException,
        client.ValidationException,
    ) as e:
        print(e)
```

```python
# PcaConnectorAdClient usage type checking example

from types_aiobotocore_pca_connector_ad.client import Exceptions

def handle_error(exc: Exceptions.AccessDeniedException) -> None:
    ...
```


## Methods


### can\_paginate



Type annotations and code completion for `#!python session.create_client("pca-connector-ad").can_paginate` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pca-connector-ad/client/can_paginate.html)

```python
# can_paginate method definition

def can_paginate(
    self,
    operation_name: str,
) -> bool:
    ...
```


### generate\_presigned\_url



Type annotations and code completion for `#!python session.create_client("pca-connector-ad").generate_presigned_url` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pca-connector-ad/client/generate_presigned_url.html)

```python
# generate_presigned_url method definition

await def generate_presigned_url(
    self,
    ClientMethod: str,
    Params: Mapping[str, Any] = ...,
    ExpiresIn: int = 3600,
    HttpMethod: str = ...,
) -> str:
    ...
```


### create\_connector

Creates a connector between Amazon Web Services Private CA and an Active
Directory.

Type annotations and code completion for `#!python session.create_client("pca-connector-ad").create_connector` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pca-connector-ad/client/create_connector.html)

```python
# create_connector method definition

await def create_connector(
    self,
    *,
    CertificateAuthorityArn: str,
    DirectoryId: str,
    VpcInformation: VpcInformationTypeDef,  # (1)
    ClientToken: str = ...,
    Tags: Mapping[str, str] = ...,
) -> CreateConnectorResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: VpcInformationTypeDef](./type_defs.md#vpcinformationtypedef) 
2. See [:material-code-braces: CreateConnectorResponseTypeDef](./type_defs.md#createconnectorresponsetypedef) 


```python
# create_connector method usage example with argument unpacking

kwargs: CreateConnectorRequestRequestTypeDef = {  # (1)
    "CertificateAuthorityArn": ...,
    "DirectoryId": ...,
    "VpcInformation": ...,
}

parent.create_connector(**kwargs)
```

1. See [:material-code-braces: CreateConnectorRequestRequestTypeDef](./type_defs.md#createconnectorrequestrequesttypedef) 

### create\_directory\_registration

Creates a directory registration that authorizes communication between Amazon
Web Services Private CA and an Active Directory.

Type annotations and code completion for `#!python session.create_client("pca-connector-ad").create_directory_registration` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pca-connector-ad/client/create_directory_registration.html)

```python
# create_directory_registration method definition

await def create_directory_registration(
    self,
    *,
    DirectoryId: str,
    ClientToken: str = ...,
    Tags: Mapping[str, str] = ...,
) -> CreateDirectoryRegistrationResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: CreateDirectoryRegistrationResponseTypeDef](./type_defs.md#createdirectoryregistrationresponsetypedef) 


```python
# create_directory_registration method usage example with argument unpacking

kwargs: CreateDirectoryRegistrationRequestRequestTypeDef = {  # (1)
    "DirectoryId": ...,
}

parent.create_directory_registration(**kwargs)
```

1. See [:material-code-braces: CreateDirectoryRegistrationRequestRequestTypeDef](./type_defs.md#createdirectoryregistrationrequestrequesttypedef) 

### create\_service\_principal\_name

Creates a service principal name (SPN) for the service account in Active
Directory.

Type annotations and code completion for `#!python session.create_client("pca-connector-ad").create_service_principal_name` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pca-connector-ad/client/create_service_principal_name.html)

```python
# create_service_principal_name method definition

await def create_service_principal_name(
    self,
    *,
    ConnectorArn: str,
    DirectoryRegistrationArn: str,
    ClientToken: str = ...,
) -> EmptyResponseMetadataTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef) 


```python
# create_service_principal_name method usage example with argument unpacking

kwargs: CreateServicePrincipalNameRequestRequestTypeDef = {  # (1)
    "ConnectorArn": ...,
    "DirectoryRegistrationArn": ...,
}

parent.create_service_principal_name(**kwargs)
```

1. See [:material-code-braces: CreateServicePrincipalNameRequestRequestTypeDef](./type_defs.md#createserviceprincipalnamerequestrequesttypedef) 

### create\_template

Creates an Active Directory compatible certificate template.

Type annotations and code completion for `#!python session.create_client("pca-connector-ad").create_template` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pca-connector-ad/client/create_template.html)

```python
# create_template method definition

await def create_template(
    self,
    *,
    ConnectorArn: str,
    Definition: TemplateDefinitionTypeDef,  # (1)
    Name: str,
    ClientToken: str = ...,
    Tags: Mapping[str, str] = ...,
) -> CreateTemplateResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: TemplateDefinitionTypeDef](./type_defs.md#templatedefinitiontypedef) 
2. See [:material-code-braces: CreateTemplateResponseTypeDef](./type_defs.md#createtemplateresponsetypedef) 


```python
# create_template method usage example with argument unpacking

kwargs: CreateTemplateRequestRequestTypeDef = {  # (1)
    "ConnectorArn": ...,
    "Definition": ...,
    "Name": ...,
}

parent.create_template(**kwargs)
```

1. See [:material-code-braces: CreateTemplateRequestRequestTypeDef](./type_defs.md#createtemplaterequestrequesttypedef) 

### create\_template\_group\_access\_control\_entry

Create a group access control entry.

Type annotations and code completion for `#!python session.create_client("pca-connector-ad").create_template_group_access_control_entry` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pca-connector-ad/client/create_template_group_access_control_entry.html)

```python
# create_template_group_access_control_entry method definition

await def create_template_group_access_control_entry(
    self,
    *,
    AccessRights: AccessRightsTypeDef,  # (1)
    GroupDisplayName: str,
    GroupSecurityIdentifier: str,
    TemplateArn: str,
    ClientToken: str = ...,
) -> EmptyResponseMetadataTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: AccessRightsTypeDef](./type_defs.md#accessrightstypedef) 
2. See [:material-code-braces: EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef) 


```python
# create_template_group_access_control_entry method usage example with argument unpacking

kwargs: CreateTemplateGroupAccessControlEntryRequestRequestTypeDef = {  # (1)
    "AccessRights": ...,
    "GroupDisplayName": ...,
    "GroupSecurityIdentifier": ...,
    "TemplateArn": ...,
}

parent.create_template_group_access_control_entry(**kwargs)
```

1. See [:material-code-braces: CreateTemplateGroupAccessControlEntryRequestRequestTypeDef](./type_defs.md#createtemplategroupaccesscontrolentryrequestrequesttypedef) 

### delete\_connector

Deletes a connector for Active Directory.

Type annotations and code completion for `#!python session.create_client("pca-connector-ad").delete_connector` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pca-connector-ad/client/delete_connector.html)

```python
# delete_connector method definition

await def delete_connector(
    self,
    *,
    ConnectorArn: str,
) -> EmptyResponseMetadataTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef) 


```python
# delete_connector method usage example with argument unpacking

kwargs: DeleteConnectorRequestRequestTypeDef = {  # (1)
    "ConnectorArn": ...,
}

parent.delete_connector(**kwargs)
```

1. See [:material-code-braces: DeleteConnectorRequestRequestTypeDef](./type_defs.md#deleteconnectorrequestrequesttypedef) 

### delete\_directory\_registration

Deletes a directory registration.

Type annotations and code completion for `#!python session.create_client("pca-connector-ad").delete_directory_registration` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pca-connector-ad/client/delete_directory_registration.html)

```python
# delete_directory_registration method definition

await def delete_directory_registration(
    self,
    *,
    DirectoryRegistrationArn: str,
) -> EmptyResponseMetadataTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef) 


```python
# delete_directory_registration method usage example with argument unpacking

kwargs: DeleteDirectoryRegistrationRequestRequestTypeDef = {  # (1)
    "DirectoryRegistrationArn": ...,
}

parent.delete_directory_registration(**kwargs)
```

1. See [:material-code-braces: DeleteDirectoryRegistrationRequestRequestTypeDef](./type_defs.md#deletedirectoryregistrationrequestrequesttypedef) 

### delete\_service\_principal\_name

Deletes the service principal name (SPN) used by a connector to authenticate
with your Active Directory.

Type annotations and code completion for `#!python session.create_client("pca-connector-ad").delete_service_principal_name` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pca-connector-ad/client/delete_service_principal_name.html)

```python
# delete_service_principal_name method definition

await def delete_service_principal_name(
    self,
    *,
    ConnectorArn: str,
    DirectoryRegistrationArn: str,
) -> EmptyResponseMetadataTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef) 


```python
# delete_service_principal_name method usage example with argument unpacking

kwargs: DeleteServicePrincipalNameRequestRequestTypeDef = {  # (1)
    "ConnectorArn": ...,
    "DirectoryRegistrationArn": ...,
}

parent.delete_service_principal_name(**kwargs)
```

1. See [:material-code-braces: DeleteServicePrincipalNameRequestRequestTypeDef](./type_defs.md#deleteserviceprincipalnamerequestrequesttypedef) 

### delete\_template

Deletes a template.

Type annotations and code completion for `#!python session.create_client("pca-connector-ad").delete_template` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pca-connector-ad/client/delete_template.html)

```python
# delete_template method definition

await def delete_template(
    self,
    *,
    TemplateArn: str,
) -> EmptyResponseMetadataTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef) 


```python
# delete_template method usage example with argument unpacking

kwargs: DeleteTemplateRequestRequestTypeDef = {  # (1)
    "TemplateArn": ...,
}

parent.delete_template(**kwargs)
```

1. See [:material-code-braces: DeleteTemplateRequestRequestTypeDef](./type_defs.md#deletetemplaterequestrequesttypedef) 

### delete\_template\_group\_access\_control\_entry

Deletes a group access control entry.

Type annotations and code completion for `#!python session.create_client("pca-connector-ad").delete_template_group_access_control_entry` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pca-connector-ad/client/delete_template_group_access_control_entry.html)

```python
# delete_template_group_access_control_entry method definition

await def delete_template_group_access_control_entry(
    self,
    *,
    GroupSecurityIdentifier: str,
    TemplateArn: str,
) -> EmptyResponseMetadataTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef) 


```python
# delete_template_group_access_control_entry method usage example with argument unpacking

kwargs: DeleteTemplateGroupAccessControlEntryRequestRequestTypeDef = {  # (1)
    "GroupSecurityIdentifier": ...,
    "TemplateArn": ...,
}

parent.delete_template_group_access_control_entry(**kwargs)
```

1. See [:material-code-braces: DeleteTemplateGroupAccessControlEntryRequestRequestTypeDef](./type_defs.md#deletetemplategroupaccesscontrolentryrequestrequesttypedef) 

### get\_connector

Lists information about your connector.

Type annotations and code completion for `#!python session.create_client("pca-connector-ad").get_connector` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pca-connector-ad/client/get_connector.html)

```python
# get_connector method definition

await def get_connector(
    self,
    *,
    ConnectorArn: str,
) -> GetConnectorResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetConnectorResponseTypeDef](./type_defs.md#getconnectorresponsetypedef) 


```python
# get_connector method usage example with argument unpacking

kwargs: GetConnectorRequestRequestTypeDef = {  # (1)
    "ConnectorArn": ...,
}

parent.get_connector(**kwargs)
```

1. See [:material-code-braces: GetConnectorRequestRequestTypeDef](./type_defs.md#getconnectorrequestrequesttypedef) 

### get\_directory\_registration

A structure that contains information about your directory registration.

Type annotations and code completion for `#!python session.create_client("pca-connector-ad").get_directory_registration` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pca-connector-ad/client/get_directory_registration.html)

```python
# get_directory_registration method definition

await def get_directory_registration(
    self,
    *,
    DirectoryRegistrationArn: str,
) -> GetDirectoryRegistrationResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetDirectoryRegistrationResponseTypeDef](./type_defs.md#getdirectoryregistrationresponsetypedef) 


```python
# get_directory_registration method usage example with argument unpacking

kwargs: GetDirectoryRegistrationRequestRequestTypeDef = {  # (1)
    "DirectoryRegistrationArn": ...,
}

parent.get_directory_registration(**kwargs)
```

1. See [:material-code-braces: GetDirectoryRegistrationRequestRequestTypeDef](./type_defs.md#getdirectoryregistrationrequestrequesttypedef) 

### get\_service\_principal\_name

Lists the service principal name that the connector uses to authenticate with
Active Directory.

Type annotations and code completion for `#!python session.create_client("pca-connector-ad").get_service_principal_name` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pca-connector-ad/client/get_service_principal_name.html)

```python
# get_service_principal_name method definition

await def get_service_principal_name(
    self,
    *,
    ConnectorArn: str,
    DirectoryRegistrationArn: str,
) -> GetServicePrincipalNameResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetServicePrincipalNameResponseTypeDef](./type_defs.md#getserviceprincipalnameresponsetypedef) 


```python
# get_service_principal_name method usage example with argument unpacking

kwargs: GetServicePrincipalNameRequestRequestTypeDef = {  # (1)
    "ConnectorArn": ...,
    "DirectoryRegistrationArn": ...,
}

parent.get_service_principal_name(**kwargs)
```

1. See [:material-code-braces: GetServicePrincipalNameRequestRequestTypeDef](./type_defs.md#getserviceprincipalnamerequestrequesttypedef) 

### get\_template

Retrieves a certificate template that the connector uses to issue certificates
from a private CA.

Type annotations and code completion for `#!python session.create_client("pca-connector-ad").get_template` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pca-connector-ad/client/get_template.html)

```python
# get_template method definition

await def get_template(
    self,
    *,
    TemplateArn: str,
) -> GetTemplateResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetTemplateResponseTypeDef](./type_defs.md#gettemplateresponsetypedef) 


```python
# get_template method usage example with argument unpacking

kwargs: GetTemplateRequestRequestTypeDef = {  # (1)
    "TemplateArn": ...,
}

parent.get_template(**kwargs)
```

1. See [:material-code-braces: GetTemplateRequestRequestTypeDef](./type_defs.md#gettemplaterequestrequesttypedef) 

### get\_template\_group\_access\_control\_entry

Retrieves the group access control entries for a template.

Type annotations and code completion for `#!python session.create_client("pca-connector-ad").get_template_group_access_control_entry` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pca-connector-ad/client/get_template_group_access_control_entry.html)

```python
# get_template_group_access_control_entry method definition

await def get_template_group_access_control_entry(
    self,
    *,
    GroupSecurityIdentifier: str,
    TemplateArn: str,
) -> GetTemplateGroupAccessControlEntryResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetTemplateGroupAccessControlEntryResponseTypeDef](./type_defs.md#gettemplategroupaccesscontrolentryresponsetypedef) 


```python
# get_template_group_access_control_entry method usage example with argument unpacking

kwargs: GetTemplateGroupAccessControlEntryRequestRequestTypeDef = {  # (1)
    "GroupSecurityIdentifier": ...,
    "TemplateArn": ...,
}

parent.get_template_group_access_control_entry(**kwargs)
```

1. See [:material-code-braces: GetTemplateGroupAccessControlEntryRequestRequestTypeDef](./type_defs.md#gettemplategroupaccesscontrolentryrequestrequesttypedef) 

### list\_connectors

Lists the connectors that you created by using the <a
href="https://docs.aws.amazon.com/pca-connector-ad/latest/APIReference/API_CreateConnector">https://docs.aws.amazon.com/pca-connector-ad/latest/APIReference/API_CreateConnector</a>
action.

Type annotations and code completion for `#!python session.create_client("pca-connector-ad").list_connectors` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pca-connector-ad/client/list_connectors.html)

```python
# list_connectors method definition

await def list_connectors(
    self,
    *,
    MaxResults: int = ...,
    NextToken: str = ...,
) -> ListConnectorsResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListConnectorsResponseTypeDef](./type_defs.md#listconnectorsresponsetypedef) 


```python
# list_connectors method usage example with argument unpacking

kwargs: ListConnectorsRequestRequestTypeDef = {  # (1)
    "MaxResults": ...,
}

parent.list_connectors(**kwargs)
```

1. See [:material-code-braces: ListConnectorsRequestRequestTypeDef](./type_defs.md#listconnectorsrequestrequesttypedef) 

### list\_directory\_registrations

Lists the directory registrations that you created by using the <a
href="https://docs.aws.amazon.com/pca-connector-ad/latest/APIReference/API_CreateDirectoryRegistration">https://docs.aws.amazon.com/pca-connector-ad/latest/APIReference/API_CreateDirectoryRegistration</a>
action.

Type annotations and code completion for `#!python session.create_client("pca-connector-ad").list_directory_registrations` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pca-connector-ad/client/list_directory_registrations.html)

```python
# list_directory_registrations method definition

await def list_directory_registrations(
    self,
    *,
    MaxResults: int = ...,
    NextToken: str = ...,
) -> ListDirectoryRegistrationsResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListDirectoryRegistrationsResponseTypeDef](./type_defs.md#listdirectoryregistrationsresponsetypedef) 


```python
# list_directory_registrations method usage example with argument unpacking

kwargs: ListDirectoryRegistrationsRequestRequestTypeDef = {  # (1)
    "MaxResults": ...,
}

parent.list_directory_registrations(**kwargs)
```

1. See [:material-code-braces: ListDirectoryRegistrationsRequestRequestTypeDef](./type_defs.md#listdirectoryregistrationsrequestrequesttypedef) 

### list\_service\_principal\_names

Lists the service principal names that the connector uses to authenticate with
Active Directory.

Type annotations and code completion for `#!python session.create_client("pca-connector-ad").list_service_principal_names` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pca-connector-ad/client/list_service_principal_names.html)

```python
# list_service_principal_names method definition

await def list_service_principal_names(
    self,
    *,
    DirectoryRegistrationArn: str,
    MaxResults: int = ...,
    NextToken: str = ...,
) -> ListServicePrincipalNamesResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListServicePrincipalNamesResponseTypeDef](./type_defs.md#listserviceprincipalnamesresponsetypedef) 


```python
# list_service_principal_names method usage example with argument unpacking

kwargs: ListServicePrincipalNamesRequestRequestTypeDef = {  # (1)
    "DirectoryRegistrationArn": ...,
}

parent.list_service_principal_names(**kwargs)
```

1. See [:material-code-braces: ListServicePrincipalNamesRequestRequestTypeDef](./type_defs.md#listserviceprincipalnamesrequestrequesttypedef) 

### list\_tags\_for\_resource

Lists the tags, if any, that are associated with your resource.

Type annotations and code completion for `#!python session.create_client("pca-connector-ad").list_tags_for_resource` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pca-connector-ad/client/list_tags_for_resource.html)

```python
# list_tags_for_resource method definition

await def list_tags_for_resource(
    self,
    *,
    ResourceArn: str,
) -> ListTagsForResourceResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListTagsForResourceResponseTypeDef](./type_defs.md#listtagsforresourceresponsetypedef) 


```python
# list_tags_for_resource method usage example with argument unpacking

kwargs: ListTagsForResourceRequestRequestTypeDef = {  # (1)
    "ResourceArn": ...,
}

parent.list_tags_for_resource(**kwargs)
```

1. See [:material-code-braces: ListTagsForResourceRequestRequestTypeDef](./type_defs.md#listtagsforresourcerequestrequesttypedef) 

### list\_template\_group\_access\_control\_entries

Lists group access control entries you created.

Type annotations and code completion for `#!python session.create_client("pca-connector-ad").list_template_group_access_control_entries` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pca-connector-ad/client/list_template_group_access_control_entries.html)

```python
# list_template_group_access_control_entries method definition

await def list_template_group_access_control_entries(
    self,
    *,
    TemplateArn: str,
    MaxResults: int = ...,
    NextToken: str = ...,
) -> ListTemplateGroupAccessControlEntriesResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListTemplateGroupAccessControlEntriesResponseTypeDef](./type_defs.md#listtemplategroupaccesscontrolentriesresponsetypedef) 


```python
# list_template_group_access_control_entries method usage example with argument unpacking

kwargs: ListTemplateGroupAccessControlEntriesRequestRequestTypeDef = {  # (1)
    "TemplateArn": ...,
}

parent.list_template_group_access_control_entries(**kwargs)
```

1. See [:material-code-braces: ListTemplateGroupAccessControlEntriesRequestRequestTypeDef](./type_defs.md#listtemplategroupaccesscontrolentriesrequestrequesttypedef) 

### list\_templates

Lists the templates, if any, that are associated with a connector.

Type annotations and code completion for `#!python session.create_client("pca-connector-ad").list_templates` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pca-connector-ad/client/list_templates.html)

```python
# list_templates method definition

await def list_templates(
    self,
    *,
    ConnectorArn: str,
    MaxResults: int = ...,
    NextToken: str = ...,
) -> ListTemplatesResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListTemplatesResponseTypeDef](./type_defs.md#listtemplatesresponsetypedef) 


```python
# list_templates method usage example with argument unpacking

kwargs: ListTemplatesRequestRequestTypeDef = {  # (1)
    "ConnectorArn": ...,
}

parent.list_templates(**kwargs)
```

1. See [:material-code-braces: ListTemplatesRequestRequestTypeDef](./type_defs.md#listtemplatesrequestrequesttypedef) 

### tag\_resource

Adds one or more tags to your resource.

Type annotations and code completion for `#!python session.create_client("pca-connector-ad").tag_resource` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pca-connector-ad/client/tag_resource.html)

```python
# tag_resource method definition

await def tag_resource(
    self,
    *,
    ResourceArn: str,
    Tags: Mapping[str, str],
) -> EmptyResponseMetadataTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef) 


```python
# tag_resource method usage example with argument unpacking

kwargs: TagResourceRequestRequestTypeDef = {  # (1)
    "ResourceArn": ...,
    "Tags": ...,
}

parent.tag_resource(**kwargs)
```

1. See [:material-code-braces: TagResourceRequestRequestTypeDef](./type_defs.md#tagresourcerequestrequesttypedef) 

### untag\_resource

Removes one or more tags from your resource.

Type annotations and code completion for `#!python session.create_client("pca-connector-ad").untag_resource` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pca-connector-ad/client/untag_resource.html)

```python
# untag_resource method definition

await def untag_resource(
    self,
    *,
    ResourceArn: str,
    TagKeys: Sequence[str],
) -> EmptyResponseMetadataTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef) 


```python
# untag_resource method usage example with argument unpacking

kwargs: UntagResourceRequestRequestTypeDef = {  # (1)
    "ResourceArn": ...,
    "TagKeys": ...,
}

parent.untag_resource(**kwargs)
```

1. See [:material-code-braces: UntagResourceRequestRequestTypeDef](./type_defs.md#untagresourcerequestrequesttypedef) 

### update\_template

Update template configuration to define the information included in
certificates.

Type annotations and code completion for `#!python session.create_client("pca-connector-ad").update_template` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pca-connector-ad/client/update_template.html)

```python
# update_template method definition

await def update_template(
    self,
    *,
    TemplateArn: str,
    Definition: TemplateDefinitionTypeDef = ...,  # (1)
    ReenrollAllCertificateHolders: bool = ...,
) -> EmptyResponseMetadataTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: TemplateDefinitionTypeDef](./type_defs.md#templatedefinitiontypedef) 
2. See [:material-code-braces: EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef) 


```python
# update_template method usage example with argument unpacking

kwargs: UpdateTemplateRequestRequestTypeDef = {  # (1)
    "TemplateArn": ...,
}

parent.update_template(**kwargs)
```

1. See [:material-code-braces: UpdateTemplateRequestRequestTypeDef](./type_defs.md#updatetemplaterequestrequesttypedef) 

### update\_template\_group\_access\_control\_entry

Update a group access control entry you created using <a
href="https://docs.aws.amazon.com/pca-connector-ad/latest/APIReference/API_CreateTemplateGroupAccessControlEntry.html">CreateTemplateGroupAccessControlEntry</a>.

Type annotations and code completion for `#!python session.create_client("pca-connector-ad").update_template_group_access_control_entry` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pca-connector-ad/client/update_template_group_access_control_entry.html)

```python
# update_template_group_access_control_entry method definition

await def update_template_group_access_control_entry(
    self,
    *,
    GroupSecurityIdentifier: str,
    TemplateArn: str,
    AccessRights: AccessRightsTypeDef = ...,  # (1)
    GroupDisplayName: str = ...,
) -> EmptyResponseMetadataTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: AccessRightsTypeDef](./type_defs.md#accessrightstypedef) 
2. See [:material-code-braces: EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef) 


```python
# update_template_group_access_control_entry method usage example with argument unpacking

kwargs: UpdateTemplateGroupAccessControlEntryRequestRequestTypeDef = {  # (1)
    "GroupSecurityIdentifier": ...,
    "TemplateArn": ...,
}

parent.update_template_group_access_control_entry(**kwargs)
```

1. See [:material-code-braces: UpdateTemplateGroupAccessControlEntryRequestRequestTypeDef](./type_defs.md#updatetemplategroupaccesscontrolentryrequestrequesttypedef) 

### \_\_aenter\_\_



Type annotations and code completion for `#!python session.create_client("pca-connector-ad").__aenter__` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pca-connector-ad.html#PcaConnectorAd.Client)

```python
# __aenter__ method definition

await def __aenter__(
    self,
) -> Self:
    ...
```


### \_\_aexit\_\_



Type annotations and code completion for `#!python session.create_client("pca-connector-ad").__aexit__` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pca-connector-ad.html#PcaConnectorAd.Client)

```python
# __aexit__ method definition

await def __aexit__(
    self,
    exc_type: Union[Type[BaseException], None],
    exc_val: Union[BaseException, None],
    exc_tb: Union[TracebackType, None],
) -> None:
    ...
```




### get_paginator

Type annotations and code completion for `#!python session.create_client("pca-connector-ad").get_paginator` method with overloads.

- `client.get_paginator("list_connectors")` -> [ListConnectorsPaginator](./paginators.md#listconnectorspaginator)
- `client.get_paginator("list_directory_registrations")` -> [ListDirectoryRegistrationsPaginator](./paginators.md#listdirectoryregistrationspaginator)
- `client.get_paginator("list_service_principal_names")` -> [ListServicePrincipalNamesPaginator](./paginators.md#listserviceprincipalnamespaginator)
- `client.get_paginator("list_template_group_access_control_entries")` -> [ListTemplateGroupAccessControlEntriesPaginator](./paginators.md#listtemplategroupaccesscontrolentriespaginator)
- `client.get_paginator("list_templates")` -> [ListTemplatesPaginator](./paginators.md#listtemplatespaginator)



