# Transfer module

> [Index](../README.md) > Transfer


!!! note ""

    Auto-generated documentation for [Transfer](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/transfer.html#Transfer)
    type annotations stubs module [types-aiobotocore-transfer](https://pypi.org/project/types-aiobotocore-transfer/).

## How to install



### From PyPI with pip

Install `types-aiobotocore` for `Transfer` service.

```bash
# install with aiobotocore type annotations
python -m pip install 'types-aiobotocore[transfer]'


# Lite version does not provide session.client/resource overloads
# it is more RAM-friendly, but requires explicit type annotations
python -m pip install 'types-aiobotocore-lite[transfer]'


# standalone installation
python -m pip install types-aiobotocore-transfer
```



## How to uninstall

```bash
python -m pip uninstall -y types-aiobotocore-transfer
```

## Usage

Code samples can be found in [Examples](./usage.md).

## TransferClient

Type annotations and code completion for  `#!python session.create_client("transfer")` as [TransferClient](./client.md)
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/transfer.html#Transfer.Client)

```python
# TransferClient usage example

from aiobotocore.session import get_session

from types_aiobotocore_transfer.client import TransferClient


session = get_session()
async with session.create_client("transfer") as client:
    client: TransferClient
```


## Paginators

Type annotations and code completion for
[paginators](./paginators.md)
from `#!python session.create_client("transfer").get_paginator("...")`.

```python
# ListAccessesPaginator usage example

from types_aiobotocore_transfer.paginator import ListAccessesPaginator

def get_list_accesses_paginator() -> ListAccessesPaginator:
    return client.get_paginator("list_accesses"))
```

- [ListAccessesPaginator](./paginators.md#listaccessespaginator)
- [ListAgreementsPaginator](./paginators.md#listagreementspaginator)
- [ListCertificatesPaginator](./paginators.md#listcertificatespaginator)
- [ListConnectorsPaginator](./paginators.md#listconnectorspaginator)
- [ListExecutionsPaginator](./paginators.md#listexecutionspaginator)
- [ListFileTransferResultsPaginator](./paginators.md#listfiletransferresultspaginator)
- [ListProfilesPaginator](./paginators.md#listprofilespaginator)
- [ListSecurityPoliciesPaginator](./paginators.md#listsecuritypoliciespaginator)
- [ListServersPaginator](./paginators.md#listserverspaginator)
- [ListTagsForResourcePaginator](./paginators.md#listtagsforresourcepaginator)
- [ListUsersPaginator](./paginators.md#listuserspaginator)
- [ListWorkflowsPaginator](./paginators.md#listworkflowspaginator)




## Waiters

Type annotations and code completion for
[waiters](./waiters.md)
from `#!python session.create_client("transfer").get_waiter("...")`.

```python
# ServerOfflineWaiter usage example

from types_aiobotocore_transfer.waiter import ServerOfflineWaiter

def get_server_offline_waiter() -> ServerOfflineWaiter:
    return Session().client("transfer").get_waiter("server_offline")
```

- [ServerOfflineWaiter](./waiters.md#serverofflinewaiter)
- [ServerOnlineWaiter](./waiters.md#serveronlinewaiter)






## Literals

Type annotations for [literals](./literals.md) used in methods and schema.

```python
# AgreementStatusTypeType usage example

from types_aiobotocore_transfer.literals import AgreementStatusTypeType

def get_value() -> AgreementStatusTypeType:
    return "ACTIVE"
```

- [AgreementStatusTypeType](./literals.md#agreementstatustypetype)
- [As2TransportType](./literals.md#as2transporttype)
- [CertificateStatusTypeType](./literals.md#certificatestatustypetype)
- [CertificateTypeType](./literals.md#certificatetypetype)
- [CertificateUsageTypeType](./literals.md#certificateusagetypetype)
- [CompressionEnumType](./literals.md#compressionenumtype)
- [CustomStepStatusType](./literals.md#customstepstatustype)
- [DirectoryListingOptimizationType](./literals.md#directorylistingoptimizationtype)
- [DomainType](./literals.md#domaintype)
- [EncryptionAlgType](./literals.md#encryptionalgtype)
- [EncryptionTypeType](./literals.md#encryptiontypetype)
- [EndpointTypeType](./literals.md#endpointtypetype)
- [ExecutionErrorTypeType](./literals.md#executionerrortypetype)
- [ExecutionStatusType](./literals.md#executionstatustype)
- [HomeDirectoryTypeType](./literals.md#homedirectorytypetype)
- [IdentityProviderTypeType](./literals.md#identityprovidertypetype)
- [ListAccessesPaginatorName](./literals.md#listaccessespaginatorname)
- [ListAgreementsPaginatorName](./literals.md#listagreementspaginatorname)
- [ListCertificatesPaginatorName](./literals.md#listcertificatespaginatorname)
- [ListConnectorsPaginatorName](./literals.md#listconnectorspaginatorname)
- [ListExecutionsPaginatorName](./literals.md#listexecutionspaginatorname)
- [ListFileTransferResultsPaginatorName](./literals.md#listfiletransferresultspaginatorname)
- [ListProfilesPaginatorName](./literals.md#listprofilespaginatorname)
- [ListSecurityPoliciesPaginatorName](./literals.md#listsecuritypoliciespaginatorname)
- [ListServersPaginatorName](./literals.md#listserverspaginatorname)
- [ListTagsForResourcePaginatorName](./literals.md#listtagsforresourcepaginatorname)
- [ListUsersPaginatorName](./literals.md#listuserspaginatorname)
- [ListWorkflowsPaginatorName](./literals.md#listworkflowspaginatorname)
- [MapTypeType](./literals.md#maptypetype)
- [MdnResponseType](./literals.md#mdnresponsetype)
- [MdnSigningAlgType](./literals.md#mdnsigningalgtype)
- [OverwriteExistingType](./literals.md#overwriteexistingtype)
- [ProfileTypeType](./literals.md#profiletypetype)
- [ProtocolType](./literals.md#protocoltype)
- [SecurityPolicyProtocolType](./literals.md#securitypolicyprotocoltype)
- [SecurityPolicyResourceTypeType](./literals.md#securitypolicyresourcetypetype)
- [ServerOfflineWaiterName](./literals.md#serverofflinewaitername)
- [ServerOnlineWaiterName](./literals.md#serveronlinewaitername)
- [SetStatOptionType](./literals.md#setstatoptiontype)
- [SftpAuthenticationMethodsType](./literals.md#sftpauthenticationmethodstype)
- [SigningAlgType](./literals.md#signingalgtype)
- [StateType](./literals.md#statetype)
- [TlsSessionResumptionModeType](./literals.md#tlssessionresumptionmodetype)
- [TransferTableStatusType](./literals.md#transfertablestatustype)
- [WorkflowStepTypeType](./literals.md#workflowsteptypetype)
- [TransferServiceName](./literals.md#transferservicename)
- [ServiceName](./literals.md#servicename)
- [ResourceServiceName](./literals.md#resourceservicename)
- [PaginatorName](./literals.md#paginatorname)
- [WaiterName](./literals.md#waitername)
- [RegionName](./literals.md#regionname)




## Type definitions

Type annotations for [type definitions](./type_defs.md) used in methods and schema.

- [As2ConnectorConfigTypeDef](./type_defs.md#as2connectorconfigtypedef)
- [ConnectorFileTransferResultTypeDef](./type_defs.md#connectorfiletransferresulttypedef)
- [HomeDirectoryMapEntryTypeDef](./type_defs.md#homedirectorymapentrytypedef)
- [PosixProfileTypeDef](./type_defs.md#posixprofiletypedef)
- [ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef)
- [TagTypeDef](./type_defs.md#tagtypedef)
- [SftpConnectorConfigTypeDef](./type_defs.md#sftpconnectorconfigtypedef)
- [EndpointDetailsTypeDef](./type_defs.md#endpointdetailstypedef)
- [IdentityProviderDetailsTypeDef](./type_defs.md#identityproviderdetailstypedef)
- [ProtocolDetailsTypeDef](./type_defs.md#protocoldetailstypedef)
- [S3StorageOptionsTypeDef](./type_defs.md#s3storageoptionstypedef)
- [CustomStepDetailsTypeDef](./type_defs.md#customstepdetailstypedef)
- [DeleteAccessRequestRequestTypeDef](./type_defs.md#deleteaccessrequestrequesttypedef)
- [DeleteAgreementRequestRequestTypeDef](./type_defs.md#deleteagreementrequestrequesttypedef)
- [DeleteCertificateRequestRequestTypeDef](./type_defs.md#deletecertificaterequestrequesttypedef)
- [DeleteConnectorRequestRequestTypeDef](./type_defs.md#deleteconnectorrequestrequesttypedef)
- [DeleteHostKeyRequestRequestTypeDef](./type_defs.md#deletehostkeyrequestrequesttypedef)
- [DeleteProfileRequestRequestTypeDef](./type_defs.md#deleteprofilerequestrequesttypedef)
- [DeleteServerRequestRequestTypeDef](./type_defs.md#deleteserverrequestrequesttypedef)
- [DeleteSshPublicKeyRequestRequestTypeDef](./type_defs.md#deletesshpublickeyrequestrequesttypedef)
- [DeleteStepDetailsTypeDef](./type_defs.md#deletestepdetailstypedef)
- [DeleteUserRequestRequestTypeDef](./type_defs.md#deleteuserrequestrequesttypedef)
- [DeleteWorkflowRequestRequestTypeDef](./type_defs.md#deleteworkflowrequestrequesttypedef)
- [DescribeAccessRequestRequestTypeDef](./type_defs.md#describeaccessrequestrequesttypedef)
- [DescribeAgreementRequestRequestTypeDef](./type_defs.md#describeagreementrequestrequesttypedef)
- [DescribeCertificateRequestRequestTypeDef](./type_defs.md#describecertificaterequestrequesttypedef)
- [DescribeConnectorRequestRequestTypeDef](./type_defs.md#describeconnectorrequestrequesttypedef)
- [DescribeExecutionRequestRequestTypeDef](./type_defs.md#describeexecutionrequestrequesttypedef)
- [DescribeHostKeyRequestRequestTypeDef](./type_defs.md#describehostkeyrequestrequesttypedef)
- [DescribeProfileRequestRequestTypeDef](./type_defs.md#describeprofilerequestrequesttypedef)
- [DescribeSecurityPolicyRequestRequestTypeDef](./type_defs.md#describesecuritypolicyrequestrequesttypedef)
- [DescribedSecurityPolicyTypeDef](./type_defs.md#describedsecuritypolicytypedef)
- [DescribeServerRequestRequestTypeDef](./type_defs.md#describeserverrequestrequesttypedef)
- [WaiterConfigTypeDef](./type_defs.md#waiterconfigtypedef)
- [DescribeUserRequestRequestTypeDef](./type_defs.md#describeuserrequestrequesttypedef)
- [DescribeWorkflowRequestRequestTypeDef](./type_defs.md#describeworkflowrequestrequesttypedef)
- [PosixProfileOutputTypeDef](./type_defs.md#posixprofileoutputtypedef)
- [SftpConnectorConfigOutputTypeDef](./type_defs.md#sftpconnectorconfigoutputtypedef)
- [LoggingConfigurationTypeDef](./type_defs.md#loggingconfigurationtypedef)
- [EndpointDetailsOutputTypeDef](./type_defs.md#endpointdetailsoutputtypedef)
- [ProtocolDetailsOutputTypeDef](./type_defs.md#protocoldetailsoutputtypedef)
- [SshPublicKeyTypeDef](./type_defs.md#sshpublickeytypedef)
- [EfsFileLocationTypeDef](./type_defs.md#efsfilelocationtypedef)
- [ExecutionErrorTypeDef](./type_defs.md#executionerrortypedef)
- [S3FileLocationTypeDef](./type_defs.md#s3filelocationtypedef)
- [TimestampTypeDef](./type_defs.md#timestamptypedef)
- [ImportSshPublicKeyRequestRequestTypeDef](./type_defs.md#importsshpublickeyrequestrequesttypedef)
- [S3InputFileLocationTypeDef](./type_defs.md#s3inputfilelocationtypedef)
- [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
- [ListAccessesRequestRequestTypeDef](./type_defs.md#listaccessesrequestrequesttypedef)
- [ListedAccessTypeDef](./type_defs.md#listedaccesstypedef)
- [ListAgreementsRequestRequestTypeDef](./type_defs.md#listagreementsrequestrequesttypedef)
- [ListedAgreementTypeDef](./type_defs.md#listedagreementtypedef)
- [ListCertificatesRequestRequestTypeDef](./type_defs.md#listcertificatesrequestrequesttypedef)
- [ListedCertificateTypeDef](./type_defs.md#listedcertificatetypedef)
- [ListConnectorsRequestRequestTypeDef](./type_defs.md#listconnectorsrequestrequesttypedef)
- [ListedConnectorTypeDef](./type_defs.md#listedconnectortypedef)
- [ListExecutionsRequestRequestTypeDef](./type_defs.md#listexecutionsrequestrequesttypedef)
- [ListFileTransferResultsRequestRequestTypeDef](./type_defs.md#listfiletransferresultsrequestrequesttypedef)
- [ListHostKeysRequestRequestTypeDef](./type_defs.md#listhostkeysrequestrequesttypedef)
- [ListedHostKeyTypeDef](./type_defs.md#listedhostkeytypedef)
- [ListProfilesRequestRequestTypeDef](./type_defs.md#listprofilesrequestrequesttypedef)
- [ListedProfileTypeDef](./type_defs.md#listedprofiletypedef)
- [ListSecurityPoliciesRequestRequestTypeDef](./type_defs.md#listsecuritypoliciesrequestrequesttypedef)
- [ListServersRequestRequestTypeDef](./type_defs.md#listserversrequestrequesttypedef)
- [ListedServerTypeDef](./type_defs.md#listedservertypedef)
- [ListTagsForResourceRequestRequestTypeDef](./type_defs.md#listtagsforresourcerequestrequesttypedef)
- [ListUsersRequestRequestTypeDef](./type_defs.md#listusersrequestrequesttypedef)
- [ListedUserTypeDef](./type_defs.md#listedusertypedef)
- [ListWorkflowsRequestRequestTypeDef](./type_defs.md#listworkflowsrequestrequesttypedef)
- [ListedWorkflowTypeDef](./type_defs.md#listedworkflowtypedef)
- [S3TagTypeDef](./type_defs.md#s3tagtypedef)
- [SendWorkflowStepStateRequestRequestTypeDef](./type_defs.md#sendworkflowstepstaterequestrequesttypedef)
- [UserDetailsTypeDef](./type_defs.md#userdetailstypedef)
- [StartDirectoryListingRequestRequestTypeDef](./type_defs.md#startdirectorylistingrequestrequesttypedef)
- [StartFileTransferRequestRequestTypeDef](./type_defs.md#startfiletransferrequestrequesttypedef)
- [StartServerRequestRequestTypeDef](./type_defs.md#startserverrequestrequesttypedef)
- [StopServerRequestRequestTypeDef](./type_defs.md#stopserverrequestrequesttypedef)
- [TestConnectionRequestRequestTypeDef](./type_defs.md#testconnectionrequestrequesttypedef)
- [TestIdentityProviderRequestRequestTypeDef](./type_defs.md#testidentityproviderrequestrequesttypedef)
- [UntagResourceRequestRequestTypeDef](./type_defs.md#untagresourcerequestrequesttypedef)
- [UpdateAgreementRequestRequestTypeDef](./type_defs.md#updateagreementrequestrequesttypedef)
- [UpdateHostKeyRequestRequestTypeDef](./type_defs.md#updatehostkeyrequestrequesttypedef)
- [UpdateProfileRequestRequestTypeDef](./type_defs.md#updateprofilerequestrequesttypedef)
- [WorkflowDetailTypeDef](./type_defs.md#workflowdetailtypedef)
- [CreateAccessRequestRequestTypeDef](./type_defs.md#createaccessrequestrequesttypedef)
- [UpdateAccessRequestRequestTypeDef](./type_defs.md#updateaccessrequestrequesttypedef)
- [UpdateUserRequestRequestTypeDef](./type_defs.md#updateuserrequestrequesttypedef)
- [CreateAccessResponseTypeDef](./type_defs.md#createaccessresponsetypedef)
- [CreateAgreementResponseTypeDef](./type_defs.md#createagreementresponsetypedef)
- [CreateConnectorResponseTypeDef](./type_defs.md#createconnectorresponsetypedef)
- [CreateProfileResponseTypeDef](./type_defs.md#createprofileresponsetypedef)
- [CreateServerResponseTypeDef](./type_defs.md#createserverresponsetypedef)
- [CreateUserResponseTypeDef](./type_defs.md#createuserresponsetypedef)
- [CreateWorkflowResponseTypeDef](./type_defs.md#createworkflowresponsetypedef)
- [EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef)
- [ImportCertificateResponseTypeDef](./type_defs.md#importcertificateresponsetypedef)
- [ImportHostKeyResponseTypeDef](./type_defs.md#importhostkeyresponsetypedef)
- [ImportSshPublicKeyResponseTypeDef](./type_defs.md#importsshpublickeyresponsetypedef)
- [ListFileTransferResultsResponseTypeDef](./type_defs.md#listfiletransferresultsresponsetypedef)
- [ListSecurityPoliciesResponseTypeDef](./type_defs.md#listsecuritypoliciesresponsetypedef)
- [StartDirectoryListingResponseTypeDef](./type_defs.md#startdirectorylistingresponsetypedef)
- [StartFileTransferResponseTypeDef](./type_defs.md#startfiletransferresponsetypedef)
- [TestConnectionResponseTypeDef](./type_defs.md#testconnectionresponsetypedef)
- [TestIdentityProviderResponseTypeDef](./type_defs.md#testidentityproviderresponsetypedef)
- [UpdateAccessResponseTypeDef](./type_defs.md#updateaccessresponsetypedef)
- [UpdateAgreementResponseTypeDef](./type_defs.md#updateagreementresponsetypedef)
- [UpdateCertificateResponseTypeDef](./type_defs.md#updatecertificateresponsetypedef)
- [UpdateConnectorResponseTypeDef](./type_defs.md#updateconnectorresponsetypedef)
- [UpdateHostKeyResponseTypeDef](./type_defs.md#updatehostkeyresponsetypedef)
- [UpdateProfileResponseTypeDef](./type_defs.md#updateprofileresponsetypedef)
- [UpdateServerResponseTypeDef](./type_defs.md#updateserverresponsetypedef)
- [UpdateUserResponseTypeDef](./type_defs.md#updateuserresponsetypedef)
- [CreateAgreementRequestRequestTypeDef](./type_defs.md#createagreementrequestrequesttypedef)
- [CreateProfileRequestRequestTypeDef](./type_defs.md#createprofilerequestrequesttypedef)
- [CreateUserRequestRequestTypeDef](./type_defs.md#createuserrequestrequesttypedef)
- [DescribedAgreementTypeDef](./type_defs.md#describedagreementtypedef)
- [DescribedCertificateTypeDef](./type_defs.md#describedcertificatetypedef)
- [DescribedHostKeyTypeDef](./type_defs.md#describedhostkeytypedef)
- [DescribedProfileTypeDef](./type_defs.md#describedprofiletypedef)
- [ImportHostKeyRequestRequestTypeDef](./type_defs.md#importhostkeyrequestrequesttypedef)
- [ListTagsForResourceResponseTypeDef](./type_defs.md#listtagsforresourceresponsetypedef)
- [TagResourceRequestRequestTypeDef](./type_defs.md#tagresourcerequestrequesttypedef)
- [CreateConnectorRequestRequestTypeDef](./type_defs.md#createconnectorrequestrequesttypedef)
- [UpdateConnectorRequestRequestTypeDef](./type_defs.md#updateconnectorrequestrequesttypedef)
- [DescribeSecurityPolicyResponseTypeDef](./type_defs.md#describesecuritypolicyresponsetypedef)
- [DescribeServerRequestServerOfflineWaitTypeDef](./type_defs.md#describeserverrequestserverofflinewaittypedef)
- [DescribeServerRequestServerOnlineWaitTypeDef](./type_defs.md#describeserverrequestserveronlinewaittypedef)
- [DescribedAccessTypeDef](./type_defs.md#describedaccesstypedef)
- [DescribedConnectorTypeDef](./type_defs.md#describedconnectortypedef)
- [DescribedUserTypeDef](./type_defs.md#describedusertypedef)
- [ExecutionStepResultTypeDef](./type_defs.md#executionstepresulttypedef)
- [FileLocationTypeDef](./type_defs.md#filelocationtypedef)
- [ImportCertificateRequestRequestTypeDef](./type_defs.md#importcertificaterequestrequesttypedef)
- [UpdateCertificateRequestRequestTypeDef](./type_defs.md#updatecertificaterequestrequesttypedef)
- [InputFileLocationTypeDef](./type_defs.md#inputfilelocationtypedef)
- [ListAccessesRequestListAccessesPaginateTypeDef](./type_defs.md#listaccessesrequestlistaccessespaginatetypedef)
- [ListAgreementsRequestListAgreementsPaginateTypeDef](./type_defs.md#listagreementsrequestlistagreementspaginatetypedef)
- [ListCertificatesRequestListCertificatesPaginateTypeDef](./type_defs.md#listcertificatesrequestlistcertificatespaginatetypedef)
- [ListConnectorsRequestListConnectorsPaginateTypeDef](./type_defs.md#listconnectorsrequestlistconnectorspaginatetypedef)
- [ListExecutionsRequestListExecutionsPaginateTypeDef](./type_defs.md#listexecutionsrequestlistexecutionspaginatetypedef)
- [ListFileTransferResultsRequestListFileTransferResultsPaginateTypeDef](./type_defs.md#listfiletransferresultsrequestlistfiletransferresultspaginatetypedef)
- [ListProfilesRequestListProfilesPaginateTypeDef](./type_defs.md#listprofilesrequestlistprofilespaginatetypedef)
- [ListSecurityPoliciesRequestListSecurityPoliciesPaginateTypeDef](./type_defs.md#listsecuritypoliciesrequestlistsecuritypoliciespaginatetypedef)
- [ListServersRequestListServersPaginateTypeDef](./type_defs.md#listserversrequestlistserverspaginatetypedef)
- [ListTagsForResourceRequestListTagsForResourcePaginateTypeDef](./type_defs.md#listtagsforresourcerequestlisttagsforresourcepaginatetypedef)
- [ListUsersRequestListUsersPaginateTypeDef](./type_defs.md#listusersrequestlistuserspaginatetypedef)
- [ListWorkflowsRequestListWorkflowsPaginateTypeDef](./type_defs.md#listworkflowsrequestlistworkflowspaginatetypedef)
- [ListAccessesResponseTypeDef](./type_defs.md#listaccessesresponsetypedef)
- [ListAgreementsResponseTypeDef](./type_defs.md#listagreementsresponsetypedef)
- [ListCertificatesResponseTypeDef](./type_defs.md#listcertificatesresponsetypedef)
- [ListConnectorsResponseTypeDef](./type_defs.md#listconnectorsresponsetypedef)
- [ListHostKeysResponseTypeDef](./type_defs.md#listhostkeysresponsetypedef)
- [ListProfilesResponseTypeDef](./type_defs.md#listprofilesresponsetypedef)
- [ListServersResponseTypeDef](./type_defs.md#listserversresponsetypedef)
- [ListUsersResponseTypeDef](./type_defs.md#listusersresponsetypedef)
- [ListWorkflowsResponseTypeDef](./type_defs.md#listworkflowsresponsetypedef)
- [TagStepDetailsOutputTypeDef](./type_defs.md#tagstepdetailsoutputtypedef)
- [TagStepDetailsTypeDef](./type_defs.md#tagstepdetailstypedef)
- [ServiceMetadataTypeDef](./type_defs.md#servicemetadatatypedef)
- [WorkflowDetailsOutputTypeDef](./type_defs.md#workflowdetailsoutputtypedef)
- [WorkflowDetailsTypeDef](./type_defs.md#workflowdetailstypedef)
- [DescribeAgreementResponseTypeDef](./type_defs.md#describeagreementresponsetypedef)
- [DescribeCertificateResponseTypeDef](./type_defs.md#describecertificateresponsetypedef)
- [DescribeHostKeyResponseTypeDef](./type_defs.md#describehostkeyresponsetypedef)
- [DescribeProfileResponseTypeDef](./type_defs.md#describeprofileresponsetypedef)
- [DescribeAccessResponseTypeDef](./type_defs.md#describeaccessresponsetypedef)
- [DescribeConnectorResponseTypeDef](./type_defs.md#describeconnectorresponsetypedef)
- [DescribeUserResponseTypeDef](./type_defs.md#describeuserresponsetypedef)
- [ExecutionResultsTypeDef](./type_defs.md#executionresultstypedef)
- [CopyStepDetailsTypeDef](./type_defs.md#copystepdetailstypedef)
- [DecryptStepDetailsTypeDef](./type_defs.md#decryptstepdetailstypedef)
- [TagStepDetailsUnionTypeDef](./type_defs.md#tagstepdetailsuniontypedef)
- [ListedExecutionTypeDef](./type_defs.md#listedexecutiontypedef)
- [DescribedServerTypeDef](./type_defs.md#describedservertypedef)
- [CreateServerRequestRequestTypeDef](./type_defs.md#createserverrequestrequesttypedef)
- [UpdateServerRequestRequestTypeDef](./type_defs.md#updateserverrequestrequesttypedef)
- [DescribedExecutionTypeDef](./type_defs.md#describedexecutiontypedef)
- [WorkflowStepOutputTypeDef](./type_defs.md#workflowstepoutputtypedef)
- [WorkflowStepTypeDef](./type_defs.md#workflowsteptypedef)
- [ListExecutionsResponseTypeDef](./type_defs.md#listexecutionsresponsetypedef)
- [DescribeServerResponseTypeDef](./type_defs.md#describeserverresponsetypedef)
- [DescribeExecutionResponseTypeDef](./type_defs.md#describeexecutionresponsetypedef)
- [DescribedWorkflowTypeDef](./type_defs.md#describedworkflowtypedef)
- [WorkflowStepUnionTypeDef](./type_defs.md#workflowstepuniontypedef)
- [DescribeWorkflowResponseTypeDef](./type_defs.md#describeworkflowresponsetypedef)
- [CreateWorkflowRequestRequestTypeDef](./type_defs.md#createworkflowrequestrequesttypedef)

