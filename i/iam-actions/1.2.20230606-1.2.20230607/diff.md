# Comparing `tmp/iam_actions-1.2.20230606.tar.gz` & `tmp/iam_actions-1.2.20230607.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "iam_actions-1.2.20230606.tar", max compression
+gzip compressed data, was "iam_actions-1.2.20230607.tar", max compression
```

## Comparing `iam_actions-1.2.20230606.tar` & `iam_actions-1.2.20230607.tar`

### file list

```diff
@@ -1,18 +1,18 @@
--rw-r--r--   0        0        0     1071 2023-06-06 02:50:17.229081 iam_actions-1.2.20230606/LICENSE
--rw-r--r--   0        0        0     2302 2023-06-06 02:50:17.229081 iam_actions-1.2.20230606/README.md
--rw-r--r--   0        0        0      228 2023-06-06 02:50:17.229081 iam_actions-1.2.20230606/iam_actions/__init__.py
--rw-r--r--   0        0        0  4148664 2023-06-06 02:51:34.434502 iam_actions-1.2.20230606/iam_actions/actions.json
--rw-r--r--   0        0        0      496 2023-06-06 02:50:17.229081 iam_actions-1.2.20230606/iam_actions/data.py
--rw-r--r--   0        0        0       80 2023-06-06 02:50:17.229081 iam_actions-1.2.20230606/iam_actions/generate/__init__.py
--rw-r--r--   0        0        0     3097 2023-06-06 02:50:17.229081 iam_actions-1.2.20230606/iam_actions/generate/action_map.py
--rw-r--r--   0        0        0    23329 2023-06-06 02:50:17.229081 iam_actions-1.2.20230606/iam_actions/generate/aws_docs.py
--rw-r--r--   0        0        0     3739 2023-06-06 02:50:17.229081 iam_actions-1.2.20230606/iam_actions/generate/generate.py
--rw-r--r--   0        0        0     3272 2023-06-06 02:50:17.229081 iam_actions-1.2.20230606/iam_actions/generate/notifier.py
--rw-r--r--   0        0        0     1902 2023-06-06 02:50:17.229081 iam_actions-1.2.20230606/iam_actions/generate/resource_type.py
--rw-r--r--   0        0        0     2277 2023-06-06 02:50:17.229081 iam_actions-1.2.20230606/iam_actions/generate/services.py
--rw-r--r--   0        0        0   551306 2023-06-06 02:51:34.434502 iam_actions-1.2.20230606/iam_actions/policies.json
--rw-r--r--   0        0        0   183844 2023-06-06 02:51:34.434502 iam_actions-1.2.20230606/iam_actions/resourcetypes.json
--rw-r--r--   0        0        0   534766 2023-06-06 02:51:34.434502 iam_actions-1.2.20230606/iam_actions/services.json
--rw-r--r--   0        0        0     1154 2023-06-06 02:51:35.338519 iam_actions-1.2.20230606/pyproject.toml
--rw-r--r--   0        0        0     3024 1970-01-01 00:00:00.000000 iam_actions-1.2.20230606/setup.py
--rw-r--r--   0        0        0     2915 1970-01-01 00:00:00.000000 iam_actions-1.2.20230606/PKG-INFO
+-rw-r--r--   0        0        0     1071 2023-06-07 02:48:33.539629 iam_actions-1.2.20230607/LICENSE
+-rw-r--r--   0        0        0     2302 2023-06-07 02:48:33.539629 iam_actions-1.2.20230607/README.md
+-rw-r--r--   0        0        0      228 2023-06-07 02:48:33.539629 iam_actions-1.2.20230607/iam_actions/__init__.py
+-rw-r--r--   0        0        0  4294396 2023-06-07 02:50:27.539640 iam_actions-1.2.20230607/iam_actions/actions.json
+-rw-r--r--   0        0        0      496 2023-06-07 02:48:33.539629 iam_actions-1.2.20230607/iam_actions/data.py
+-rw-r--r--   0        0        0       80 2023-06-07 02:48:33.539629 iam_actions-1.2.20230607/iam_actions/generate/__init__.py
+-rw-r--r--   0        0        0     3097 2023-06-07 02:48:33.539629 iam_actions-1.2.20230607/iam_actions/generate/action_map.py
+-rw-r--r--   0        0        0    23329 2023-06-07 02:48:33.539629 iam_actions-1.2.20230607/iam_actions/generate/aws_docs.py
+-rw-r--r--   0        0        0     3739 2023-06-07 02:48:33.539629 iam_actions-1.2.20230607/iam_actions/generate/generate.py
+-rw-r--r--   0        0        0     3272 2023-06-07 02:48:33.539629 iam_actions-1.2.20230607/iam_actions/generate/notifier.py
+-rw-r--r--   0        0        0     1902 2023-06-07 02:48:33.539629 iam_actions-1.2.20230607/iam_actions/generate/resource_type.py
+-rw-r--r--   0        0        0     2277 2023-06-07 02:48:33.539629 iam_actions-1.2.20230607/iam_actions/generate/services.py
+-rw-r--r--   0        0        0   552341 2023-06-07 02:50:27.539640 iam_actions-1.2.20230607/iam_actions/policies.json
+-rw-r--r--   0        0        0   195776 2023-06-07 02:50:27.539640 iam_actions-1.2.20230607/iam_actions/resourcetypes.json
+-rw-r--r--   0        0        0   535757 2023-06-07 02:50:27.539640 iam_actions-1.2.20230607/iam_actions/services.json
+-rw-r--r--   0        0        0     1154 2023-06-07 02:50:28.327637 iam_actions-1.2.20230607/pyproject.toml
+-rw-r--r--   0        0        0     3024 1970-01-01 00:00:00.000000 iam_actions-1.2.20230607/setup.py
+-rw-r--r--   0        0        0     2915 1970-01-01 00:00:00.000000 iam_actions-1.2.20230607/PKG-INFO
```

### Comparing `iam_actions-1.2.20230606/LICENSE` & `iam_actions-1.2.20230607/LICENSE`

 * *Files identical despite different names*

### Comparing `iam_actions-1.2.20230606/README.md` & `iam_actions-1.2.20230607/README.md`

 * *Files identical despite different names*

### Comparing `iam_actions-1.2.20230606/iam_actions/actions.json` & `iam_actions-1.2.20230607/iam_actions/actions.json`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9986202927869061%*

 * *Differences: {"'ec2'": "{'DescribeStoreImageTasks': {'access_level': 'List', 'condition_keys': ['ec2:Region'], "*

 * *          "'description': 'Grants permission to describe the progress of the AMI store tasks'}, "*

 * *          "'GetVpnTunnelReplacementStatus': {'access_level': 'List', 'condition_keys': "*

 * *          "['aws:ResourceTag/${TagKey}', 'ec2:Region', 'ec2:ResourceTag/${TagKey}'], "*

 * *          "'description': 'Grants permission to view available tunnel endpoint maintenance "*

 * *          "events', 'resources': ['vpn-connec […]*

```diff
@@ -42370,4858 +42370,9922 @@
             "resources": [
                 "snapshot"
             ]
         }
     },
     "ec2": {
         "AcceptAddressTransfer": {
-            "access_level": "Undocumented",
+            "access_level": "Write",
             "action": "AcceptAddressTransfer",
-            "condition_keys": [],
-            "description": "Not Documented by AWS",
+            "condition_keys": [
+                "aws:RequestTag/${TagKey}",
+                "aws:TagKeys",
+                "ec2:AllocationId",
+                "ec2:Domain",
+                "ec2:PublicIpAddress",
+                "ec2:Region"
+            ],
+            "description": "Grants permission to accept an Elastic IP address transfer",
             "orphan": false,
-            "resources": []
+            "resources": [
+                "elastic-ip"
+            ]
         },
         "AcceptReservedInstancesExchangeQuote": {
-            "access_level": "Undocumented",
+            "access_level": "Write",
             "action": "AcceptReservedInstancesExchangeQuote",
-            "condition_keys": [],
-            "description": "Not Documented by AWS",
+            "condition_keys": [
+                "ec2:Region"
+            ],
+            "description": "Grants permission to accept a Convertible Reserved Instance exchange quote",
             "orphan": false,
             "resources": []
         },
         "AcceptTransitGatewayMulticastDomainAssociations": {
-            "access_level": "Undocumented",
+            "access_level": "Write",
             "action": "AcceptTransitGatewayMulticastDomainAssociations",
-            "condition_keys": [],
-            "description": "Not Documented by AWS",
+            "condition_keys": [
+                "aws:ResourceTag/${TagKey}",
+                "ec2:Region",
+                "ec2:ResourceTag/${TagKey}"
+            ],
+            "description": "Grants permission to accept a request to associate subnets with a transit gateway multicast domain",
             "orphan": false,
-            "resources": []
+            "resources": [
+                "transit-gateway-attachment",
+                "transit-gateway-multicast-domain"
+            ]
         },
         "AcceptTransitGatewayPeeringAttachment": {
-            "access_level": "Undocumented",
+            "access_level": "Write",
             "action": "AcceptTransitGatewayPeeringAttachment",
-            "condition_keys": [],
-            "description": "Not Documented by AWS",
+            "condition_keys": [
+                "aws:ResourceTag/${TagKey}",
+                "ec2:Region",
+                "ec2:ResourceTag/${TagKey}"
+            ],
+            "description": "Grants permission to accept a transit gateway peering attachment request",
             "orphan": false,
-            "resources": []
+            "resources": [
+                "transit-gateway-attachment"
+            ]
         },
         "AcceptTransitGatewayVpcAttachment": {
-            "access_level": "Undocumented",
+            "access_level": "Write",
             "action": "AcceptTransitGatewayVpcAttachment",
-            "condition_keys": [],
-            "description": "Not Documented by AWS",
+            "condition_keys": [
+                "aws:ResourceTag/${TagKey}",
+                "ec2:Region",
+                "ec2:ResourceTag/${TagKey}"
+            ],
+            "description": "Grants permission to accept a request to attach a VPC to a transit gateway",
             "orphan": false,
-            "resources": []
+            "resources": [
+                "transit-gateway-attachment"
+            ]
         },
         "AcceptVpcEndpointConnections": {
-            "access_level": "Undocumented",
+            "access_level": "Write",
             "action": "AcceptVpcEndpointConnections",
-            "condition_keys": [],
-            "description": "Not Documented by AWS",
+            "condition_keys": [
+                "aws:ResourceTag/${TagKey}",
+                "ec2:Region",
+                "ec2:ResourceTag/${TagKey}"
+            ],
+            "description": "Grants permission to accept one or more interface VPC endpoint connections to your VPC endpoint service",
             "orphan": false,
-            "resources": []
+            "resources": [
+                "vpc-endpoint-service"
+            ]
         },
         "AcceptVpcPeeringConnection": {
-            "access_level": "Undocumented",
+            "access_level": "Write",
             "action": "AcceptVpcPeeringConnection",
-            "condition_keys": [],
-            "description": "Not Documented by AWS",
+            "condition_keys": [
+                "aws:ResourceTag/${TagKey}",
+                "ec2:AccepterVpc",
+                "ec2:Region",
+                "ec2:RequesterVpc",
+                "ec2:ResourceTag/${TagKey}",
+                "ec2:Tenancy",
+                "ec2:VpcID",
+                "ec2:VpcPeeringConnectionID"
+            ],
+            "description": "Grants permission to accept a VPC peering connection request",
             "orphan": false,
-            "resources": []
+            "resources": [
+                "vpc",
+                "vpc-peering-connection"
+            ]
         },
         "AdvertiseByoipCidr": {
-            "access_level": "Undocumented",
+            "access_level": "Write",
             "action": "AdvertiseByoipCidr",
-            "condition_keys": [],
-            "description": "Not Documented by AWS",
+            "condition_keys": [
+                "ec2:Region"
+            ],
+            "description": "Grants permission to advertise an IP address range that is provisioned for use in AWS through bring your own IP addresses (BYOIP)",
             "orphan": false,
             "resources": []
         },
         "AllocateAddress": {
-            "access_level": "Undocumented",
+            "access_level": "Write",
             "action": "AllocateAddress",
-            "condition_keys": [],
-            "description": "Not Documented by AWS",
+            "condition_keys": [
+                "aws:RequestTag/${TagKey}",
+                "aws:ResourceTag/${TagKey}",
+                "aws:TagKeys",
+                "ec2:Region",
+                "ec2:ResourceTag/${TagKey}"
+            ],
+            "description": "Grants permission to allocate an Elastic IP address (EIP) to your account",
             "orphan": false,
-            "resources": []
+            "resources": [
+                "elastic-ip",
+                "ipv4pool-ec2"
+            ]
         },
         "AllocateHosts": {
-            "access_level": "Undocumented",
+            "access_level": "Write",
             "action": "AllocateHosts",
-            "condition_keys": [],
-            "description": "Not Documented by AWS",
+            "condition_keys": [
+                "aws:RequestTag/${TagKey}",
+                "aws:TagKeys",
+                "ec2:AutoPlacement",
+                "ec2:AvailabilityZone",
+                "ec2:HostRecovery",
+                "ec2:InstanceType",
+                "ec2:Quantity",
+                "ec2:Region"
+            ],
+            "description": "Grants permission to allocate a Dedicated Host to your account",
             "orphan": false,
-            "resources": []
+            "resources": [
+                "dedicated-host"
+            ]
         },
         "AllocateIpamPoolCidr": {
-            "access_level": "Undocumented",
+            "access_level": "Write",
             "action": "AllocateIpamPoolCidr",
-            "condition_keys": [],
-            "description": "Not Documented by AWS",
+            "condition_keys": [
+                "aws:ResourceTag/${TagKey}",
+                "ec2:Region",
+                "ec2:ResourceTag/${TagKey}"
+            ],
+            "description": "Grants permission to allocate a CIDR from an Amazon VPC IP Address Manager (IPAM) pool",
             "orphan": false,
-            "resources": []
+            "resources": [
+                "ipam-pool"
+            ]
         },
         "ApplySecurityGroupsToClientVpnTargetNetwork": {
-            "access_level": "Undocumented",
+            "access_level": "Write",
             "action": "ApplySecurityGroupsToClientVpnTargetNetwork",
-            "condition_keys": [],
-            "description": "Not Documented by AWS",
-            "orphan": false,
-            "resources": []
+            "condition_keys": [
+                "aws:ResourceTag/${TagKey}",
+                "ec2:ClientRootCertificateChainArn",
+                "ec2:CloudwatchLogGroupArn",
+                "ec2:CloudwatchLogStreamArn",
+                "ec2:DirectoryArn",
+                "ec2:Region",
+                "ec2:ResourceTag/${TagKey}",
+                "ec2:SamlProviderArn",
+                "ec2:SecurityGroupID",
+                "ec2:ServerCertificateArn",
+                "ec2:VpcID"
+            ],
+            "description": "Grants permission to apply a security group to the association between a Client VPN endpoint and a target network",
+            "orphan": false,
+            "resources": [
+                "client-vpn-endpoint",
+                "security-group",
+                "vpc"
+            ]
         },
         "AssignIpv6Addresses": {
-            "access_level": "Undocumented",
+            "access_level": "Write",
             "action": "AssignIpv6Addresses",
-            "condition_keys": [],
-            "description": "Not Documented by AWS",
+            "condition_keys": [
+                "aws:ResourceTag/${TagKey}",
+                "ec2:AvailabilityZone",
+                "ec2:NetworkInterfaceID",
+                "ec2:Region",
+                "ec2:ResourceTag/${TagKey}",
+                "ec2:Subnet",
+                "ec2:Vpc"
+            ],
+            "description": "Grants permission to assign one or more IPv6 addresses to a network interface",
             "orphan": false,
-            "resources": []
+            "resources": [
+                "network-interface"
+            ]
         },
         "AssignPrivateIpAddresses": {
-            "access_level": "Undocumented",
+            "access_level": "Write",
             "action": "AssignPrivateIpAddresses",
-            "condition_keys": [],
-            "description": "Not Documented by AWS",
+            "condition_keys": [
+                "aws:ResourceTag/${TagKey}",
+                "ec2:AvailabilityZone",
+                "ec2:NetworkInterfaceID",
+                "ec2:Region",
+                "ec2:ResourceTag/${TagKey}",
+                "ec2:Subnet",
+                "ec2:Vpc"
+            ],
+            "description": "Grants permission to assign one or more secondary private IP addresses to a network interface",
             "orphan": false,
-            "resources": []
+            "resources": [
+                "network-interface"
+            ]
         },
         "AssignPrivateNatGatewayAddress": {
-            "access_level": "Undocumented",
+            "access_level": "Write",
             "action": "AssignPrivateNatGatewayAddress",
-            "condition_keys": [],
-            "description": "Not Documented by AWS",
+            "condition_keys": [
+                "aws:ResourceTag/${TagKey}",
+                "ec2:Region",
+                "ec2:ResourceTag/${TagKey}"
+            ],
+            "description": "Grants permission to assign one or more secondary private IP addresses to a private NAT gateway",
             "orphan": false,
-            "resources": []
+            "resources": [
+                "natgateway"
+            ]
         },
         "AssociateAddress": {
-            "access_level": "Undocumented",
+            "access_level": "Write",
             "action": "AssociateAddress",
-            "condition_keys": [],
-            "description": "Not Documented by AWS",
+            "condition_keys": [
+                "aws:ResourceTag/${TagKey}",
+                "ec2:AllocationId",
+                "ec2:AvailabilityZone",
+                "ec2:Domain",
+                "ec2:EbsOptimized",
+                "ec2:InstanceAutoRecovery",
+                "ec2:InstanceID",
+                "ec2:InstanceMarketType",
+                "ec2:InstanceMetadataTags",
+                "ec2:InstanceProfile",
+                "ec2:InstanceType",
+                "ec2:MetadataHttpEndpoint",
+                "ec2:MetadataHttpPutResponseHopLimit",
+                "ec2:MetadataHttpTokens",
+                "ec2:NetworkInterfaceID",
+                "ec2:PlacementGroup",
+                "ec2:ProductCode",
+                "ec2:PublicIpAddress",
+                "ec2:Region",
+                "ec2:ResourceTag/${TagKey}",
+                "ec2:RootDeviceType",
+                "ec2:Subnet",
+                "ec2:Tenancy",
+                "ec2:Vpc"
+            ],
+            "description": "Grants permission to associate an Elastic IP address (EIP) with an instance or a network interface",
             "orphan": false,
-            "resources": []
+            "resources": [
+                "elastic-ip",
+                "instance",
+                "network-interface"
+            ]
         },
         "AssociateClientVpnTargetNetwork": {
-            "access_level": "Undocumented",
+            "access_level": "Write",
             "action": "AssociateClientVpnTargetNetwork",
-            "condition_keys": [],
-            "description": "Not Documented by AWS",
+            "condition_keys": [
+                "aws:ResourceTag/${TagKey}",
+                "ec2:ClientRootCertificateChainArn",
+                "ec2:CloudwatchLogGroupArn",
+                "ec2:CloudwatchLogStreamArn",
+                "ec2:DirectoryArn",
+                "ec2:Region",
+                "ec2:ResourceTag/${TagKey}",
+                "ec2:SamlProviderArn",
+                "ec2:ServerCertificateArn",
+                "ec2:SubnetID"
+            ],
+            "description": "Grants permission to associate a target network with a Client VPN endpoint",
             "orphan": false,
-            "resources": []
+            "resources": [
+                "client-vpn-endpoint",
+                "subnet"
+            ]
         },
         "AssociateDhcpOptions": {
-            "access_level": "Undocumented",
+            "access_level": "Write",
             "action": "AssociateDhcpOptions",
-            "condition_keys": [],
-            "description": "Not Documented by AWS",
+            "condition_keys": [
+                "aws:ResourceTag/${TagKey}",
+                "ec2:DhcpOptionsID",
+                "ec2:Region",
+                "ec2:ResourceTag/${TagKey}",
+                "ec2:Tenancy",
+                "ec2:VpcID"
+            ],
+            "description": "Grants permission to associate or disassociate a set of DHCP options with a VPC",
             "orphan": false,
-            "resources": []
+            "resources": [
+                "dhcp-options",
+                "vpc"
+            ]
         },
         "AssociateEnclaveCertificateIamRole": {
-            "access_level": "Undocumented",
+            "access_level": "Write",
             "action": "AssociateEnclaveCertificateIamRole",
-            "condition_keys": [],
-            "description": "Not Documented by AWS",
+            "condition_keys": [
+                "ec2:Region"
+            ],
+            "description": "Grants permission to associate an ACM certificate with an IAM role to be used in an EC2 Enclave",
             "orphan": false,
-            "resources": []
+            "resources": [
+                "certificate",
+                "role"
+            ]
         },
         "AssociateIamInstanceProfile": {
-            "access_level": "Undocumented",
+            "access_level": "Write",
             "action": "AssociateIamInstanceProfile",
-            "condition_keys": [],
-            "description": "Not Documented by AWS",
+            "condition_keys": [
+                "aws:ResourceTag/${TagKey}",
+                "ec2:AvailabilityZone",
+                "ec2:EbsOptimized",
+                "ec2:InstanceAutoRecovery",
+                "ec2:InstanceID",
+                "ec2:InstanceMarketType",
+                "ec2:InstanceMetadataTags",
+                "ec2:InstanceProfile",
+                "ec2:InstanceType",
+                "ec2:MetadataHttpEndpoint",
+                "ec2:MetadataHttpPutResponseHopLimit",
+                "ec2:MetadataHttpTokens",
+                "ec2:NewInstanceProfile",
+                "ec2:PlacementGroup",
+                "ec2:ProductCode",
+                "ec2:Region",
+                "ec2:ResourceTag/${TagKey}",
+                "ec2:RootDeviceType",
+                "ec2:Tenancy"
+            ],
+            "description": "Grants permission to associate an IAM instance profile with a running or stopped instance",
             "orphan": false,
-            "resources": []
+            "resources": [
+                "instance"
+            ]
         },
         "AssociateInstanceEventWindow": {
-            "access_level": "Undocumented",
+            "access_level": "Write",
             "action": "AssociateInstanceEventWindow",
-            "condition_keys": [],
-            "description": "Not Documented by AWS",
+            "condition_keys": [
+                "aws:ResourceTag/${TagKey}",
+                "ec2:Region",
+                "ec2:ResourceTag/${TagKey}"
+            ],
+            "description": "Grants permission to associate one or more targets with an event window",
             "orphan": false,
-            "resources": []
+            "resources": [
+                "instance-event-window"
+            ]
         },
         "AssociateIpamResourceDiscovery": {
-            "access_level": "Undocumented",
+            "access_level": "Write",
             "action": "AssociateIpamResourceDiscovery",
-            "condition_keys": [],
-            "description": "Not Documented by AWS",
+            "condition_keys": [
+                "aws:RequestTag/${TagKey}",
+                "aws:ResourceTag/${TagKey}",
+                "aws:TagKeys",
+                "ec2:Region",
+                "ec2:ResourceTag/${TagKey}"
+            ],
+            "description": "Grants permission to associate an IPAM resource discovery with an Amazon VPC IPAM",
             "orphan": false,
-            "resources": []
+            "resources": [
+                "ipam",
+                "ipam-resource-discovery",
+                "ipam-resource-discovery-association"
+            ]
         },
         "AssociateNatGatewayAddress": {
-            "access_level": "Undocumented",
+            "access_level": "Write",
             "action": "AssociateNatGatewayAddress",
-            "condition_keys": [],
-            "description": "Not Documented by AWS",
+            "condition_keys": [
+                "aws:ResourceTag/${TagKey}",
+                "ec2:AllocationId",
+                "ec2:Domain",
+                "ec2:PublicIpAddress",
+                "ec2:Region",
+                "ec2:ResourceTag/${TagKey}"
+            ],
+            "description": "Grants permission to associate an Elastic IP address and private IP address with a public Nat gateway",
             "orphan": false,
-            "resources": []
+            "resources": [
+                "elastic-ip",
+                "natgateway"
+            ]
         },
         "AssociateRouteTable": {
-            "access_level": "Undocumented",
+            "access_level": "Write",
             "action": "AssociateRouteTable",
-            "condition_keys": [],
-            "description": "Not Documented by AWS",
+            "condition_keys": [
+                "aws:ResourceTag/${TagKey}",
+                "ec2:AvailabilityZone",
+                "ec2:InternetGatewayID",
+                "ec2:Region",
+                "ec2:ResourceTag/${TagKey}",
+                "ec2:RouteTableID",
+                "ec2:SubnetID",
+                "ec2:Vpc"
+            ],
+            "description": "Grants permission to associate a subnet or gateway with a route table",
             "orphan": false,
-            "resources": []
+            "resources": [
+                "internet-gateway",
+                "route-table",
+                "subnet",
+                "vpn-gateway"
+            ]
         },
         "AssociateSubnetCidrBlock": {
-            "access_level": "Undocumented",
+            "access_level": "Write",
             "action": "AssociateSubnetCidrBlock",
-            "condition_keys": [],
-            "description": "Not Documented by AWS",
+            "condition_keys": [
+                "aws:ResourceTag/${TagKey}",
+                "ec2:AvailabilityZone",
+                "ec2:Region",
+                "ec2:ResourceTag/${TagKey}",
+                "ec2:SubnetID",
+                "ec2:Vpc"
+            ],
+            "description": "Grants permission to associate a CIDR block with a subnet",
             "orphan": false,
-            "resources": []
+            "resources": [
+                "subnet"
+            ]
         },
         "AssociateTransitGatewayMulticastDomain": {
-            "access_level": "Undocumented",
+            "access_level": "Write",
             "action": "AssociateTransitGatewayMulticastDomain",
-            "condition_keys": [],
-            "description": "Not Documented by AWS",
+            "condition_keys": [
+                "aws:ResourceTag/${TagKey}",
+                "ec2:AvailabilityZone",
+                "ec2:Region",
+                "ec2:ResourceTag/${TagKey}",
+                "ec2:SubnetID",
+                "ec2:Vpc"
+            ],
+            "description": "Grants permission to associate an attachment and list of subnets with a transit gateway multicast domain",
             "orphan": false,
-            "resources": []
+            "resources": [
+                "subnet",
+                "transit-gateway-attachment",
+                "transit-gateway-multicast-domain"
+            ]
         },
         "AssociateTransitGatewayPolicyTable": {
-            "access_level": "Undocumented",
+            "access_level": "Write",
             "action": "AssociateTransitGatewayPolicyTable",
-            "condition_keys": [],
-            "description": "Not Documented by AWS",
+            "condition_keys": [
+                "aws:ResourceTag/${TagKey}",
+                "ec2:Region",
+                "ec2:ResourceTag/${TagKey}"
+            ],
+            "description": "Grants permission to associate a policy table with a transit gateway attachment",
             "orphan": false,
-            "resources": []
+            "resources": [
+                "transit-gateway-attachment",
+                "transit-gateway-policy-table"
+            ]
         },
         "AssociateTransitGatewayRouteTable": {
-            "access_level": "Undocumented",
+            "access_level": "Write",
             "action": "AssociateTransitGatewayRouteTable",
-            "condition_keys": [],
-            "description": "Not Documented by AWS",
+            "condition_keys": [
+                "aws:ResourceTag/${TagKey}",
+                "ec2:Region",
+                "ec2:ResourceTag/${TagKey}"
+            ],
+            "description": "Grants permission to associate an attachment with a transit gateway route table",
             "orphan": false,
-            "resources": []
+            "resources": [
+                "transit-gateway-attachment",
+                "transit-gateway-route-table"
+            ]
         },
         "AssociateTrunkInterface": {
-            "access_level": "Undocumented",
+            "access_level": "Write",
             "action": "AssociateTrunkInterface",
-            "condition_keys": [],
-            "description": "Not Documented by AWS",
+            "condition_keys": [
+                "ec2:Region"
+            ],
+            "description": "Grants permission to associate a branch network interface with a trunk network interface",
             "orphan": false,
             "resources": []
         },
         "AssociateVerifiedAccessInstanceWebAcl": {
-            "access_level": "Undocumented",
+            "access_level": "Write",
             "action": "AssociateVerifiedAccessInstanceWebAcl",
-            "condition_keys": [],
-            "description": "Not Documented by AWS",
+            "condition_keys": [
+                "aws:ResourceTag/${TagKey}",
+                "ec2:Region",
+                "ec2:ResourceTag/${TagKey}"
+            ],
+            "description": "Grants permission to associate an AWS Web Application Firewall (WAF) web access control list (ACL) with a Verified Access instance",
             "orphan": false,
-            "resources": []
+            "resources": [
+                "verified-access-instance"
+            ]
         },
         "AssociateVpcCidrBlock": {
-            "access_level": "Undocumented",
+            "access_level": "Write",
             "action": "AssociateVpcCidrBlock",
-            "condition_keys": [],
-            "description": "Not Documented by AWS",
+            "condition_keys": [
+                "aws:ResourceTag/${TagKey}",
+                "ec2:Ipv4IpamPoolId",
+                "ec2:Ipv6IpamPoolId",
+                "ec2:Region",
+                "ec2:ResourceTag/${TagKey}",
+                "ec2:Tenancy",
+                "ec2:VpcID"
+            ],
+            "description": "Grants permission to associate a CIDR block with a VPC",
             "orphan": false,
-            "resources": []
+            "resources": [
+                "ipam-pool",
+                "ipv6pool-ec2",
+                "vpc"
+            ]
         },
         "AttachClassicLinkVpc": {
-            "access_level": "Undocumented",
+            "access_level": "Write",
             "action": "AttachClassicLinkVpc",
-            "condition_keys": [],
-            "description": "Not Documented by AWS",
+            "condition_keys": [
+                "aws:ResourceTag/${TagKey}",
+                "ec2:AvailabilityZone",
+                "ec2:EbsOptimized",
+                "ec2:InstanceID",
+                "ec2:InstanceMarketType",
+                "ec2:InstanceProfile",
+                "ec2:InstanceType",
+                "ec2:MetadataHttpEndpoint",
+                "ec2:MetadataHttpPutResponseHopLimit",
+                "ec2:MetadataHttpTokens",
+                "ec2:PlacementGroup",
+                "ec2:Region",
+                "ec2:ResourceTag/${TagKey}",
+                "ec2:RootDeviceType",
+                "ec2:SecurityGroupID",
+                "ec2:Tenancy",
+                "ec2:Vpc",
+                "ec2:VpcID"
+            ],
+            "description": "Grants permission to link an EC2-Classic instance to a ClassicLink-enabled VPC through one or more of the VPC's security groups",
             "orphan": false,
-            "resources": []
+            "resources": [
+                "instance",
+                "security-group",
+                "vpc"
+            ]
         },
         "AttachInternetGateway": {
-            "access_level": "Undocumented",
+            "access_level": "Write",
             "action": "AttachInternetGateway",
-            "condition_keys": [],
-            "description": "Not Documented by AWS",
+            "condition_keys": [
+                "aws:ResourceTag/${TagKey}",
+                "ec2:InternetGatewayID",
+                "ec2:Region",
+                "ec2:ResourceTag/${TagKey}",
+                "ec2:Tenancy",
+                "ec2:VpcID"
+            ],
+            "description": "Grants permission to attach an internet gateway to a VPC",
             "orphan": false,
-            "resources": []
+            "resources": [
+                "internet-gateway",
+                "vpc"
+            ]
         },
         "AttachNetworkInterface": {
-            "access_level": "Undocumented",
+            "access_level": "Write",
             "action": "AttachNetworkInterface",
-            "condition_keys": [],
-            "description": "Not Documented by AWS",
+            "condition_keys": [
+                "aws:ResourceTag/${TagKey}",
+                "ec2:AvailabilityZone",
+                "ec2:EbsOptimized",
+                "ec2:InstanceAutoRecovery",
+                "ec2:InstanceID",
+                "ec2:InstanceMarketType",
+                "ec2:InstanceMetadataTags",
+                "ec2:InstanceProfile",
+                "ec2:InstanceType",
+                "ec2:MetadataHttpEndpoint",
+                "ec2:MetadataHttpPutResponseHopLimit",
+                "ec2:MetadataHttpTokens",
+                "ec2:NetworkInterfaceID",
+                "ec2:PlacementGroup",
+                "ec2:ProductCode",
+                "ec2:Region",
+                "ec2:ResourceTag/${TagKey}",
+                "ec2:RootDeviceType",
+                "ec2:Subnet",
+                "ec2:Tenancy",
+                "ec2:Vpc"
+            ],
+            "description": "Grants permission to attach a network interface to an instance",
             "orphan": false,
-            "resources": []
+            "resources": [
+                "instance",
+                "network-interface"
+            ]
         },
         "AttachVerifiedAccessTrustProvider": {
-            "access_level": "Undocumented",
+            "access_level": "Write",
             "action": "AttachVerifiedAccessTrustProvider",
-            "condition_keys": [],
-            "description": "Not Documented by AWS",
+            "condition_keys": [
+                "aws:ResourceTag/${TagKey}",
+                "ec2:Region",
+                "ec2:ResourceTag/${TagKey}"
+            ],
+            "description": "Grants permission to attach a trust provider to a Verified Access instance",
             "orphan": false,
-            "resources": []
+            "resources": [
+                "verified-access-instance",
+                "verified-access-trust-provider"
+            ]
         },
         "AttachVolume": {
-            "access_level": "Undocumented",
+            "access_level": "Write",
             "action": "AttachVolume",
-            "condition_keys": [],
-            "description": "Not Documented by AWS",
+            "condition_keys": [
+                "aws:ResourceTag/${TagKey}",
+                "ec2:AvailabilityZone",
+                "ec2:EbsOptimized",
+                "ec2:Encrypted",
+                "ec2:InstanceID",
+                "ec2:InstanceMarketType",
+                "ec2:InstanceProfile",
+                "ec2:InstanceType",
+                "ec2:MetadataHttpEndpoint",
+                "ec2:MetadataHttpPutResponseHopLimit",
+                "ec2:MetadataHttpTokens",
+                "ec2:ParentSnapshot",
+                "ec2:PlacementGroup",
+                "ec2:ProductCode",
+                "ec2:Region",
+                "ec2:ResourceTag/${TagKey}",
+                "ec2:RootDeviceType",
+                "ec2:Tenancy",
+                "ec2:VolumeID",
+                "ec2:VolumeIops",
+                "ec2:VolumeSize",
+                "ec2:VolumeThroughput",
+                "ec2:VolumeType"
+            ],
+            "description": "Grants permission to attach an EBS volume to a running or stopped instance and expose it to the instance with the specified device name",
             "orphan": false,
-            "resources": []
+            "resources": [
+                "instance",
+                "volume"
+            ]
         },
         "AttachVpnGateway": {
-            "access_level": "Undocumented",
+            "access_level": "Write",
             "action": "AttachVpnGateway",
-            "condition_keys": [],
-            "description": "Not Documented by AWS",
+            "condition_keys": [
+                "aws:ResourceTag/${TagKey}",
+                "ec2:Region",
+                "ec2:ResourceTag/${TagKey}",
+                "ec2:Tenancy",
+                "ec2:VpcID"
+            ],
+            "description": "Grants permission to attach a virtual private gateway to a VPC",
             "orphan": false,
-            "resources": []
+            "resources": [
+                "vpc",
+                "vpn-gateway"
+            ]
         },
         "AuthorizeClientVpnIngress": {
-            "access_level": "Undocumented",
+            "access_level": "Write",
             "action": "AuthorizeClientVpnIngress",
-            "condition_keys": [],
-            "description": "Not Documented by AWS",
+            "condition_keys": [
+                "aws:ResourceTag/${TagKey}",
+                "ec2:ClientRootCertificateChainArn",
+                "ec2:CloudwatchLogGroupArn",
+                "ec2:CloudwatchLogStreamArn",
+                "ec2:DirectoryArn",
+                "ec2:Region",
+                "ec2:ResourceTag/${TagKey}",
+                "ec2:SamlProviderArn",
+                "ec2:ServerCertificateArn"
+            ],
+            "description": "Grants permission to add an inbound authorization rule to a Client VPN endpoint",
             "orphan": false,
-            "resources": []
+            "resources": [
+                "client-vpn-endpoint"
+            ]
         },
         "AuthorizeSecurityGroupEgress": {
-            "access_level": "Undocumented",
+            "access_level": "Write",
             "action": "AuthorizeSecurityGroupEgress",
-            "condition_keys": [],
-            "description": "Not Documented by AWS",
+            "condition_keys": [
+                "aws:RequestTag/${TagKey}",
+                "aws:ResourceTag/${TagKey}",
+                "aws:TagKeys",
+                "ec2:Region",
+                "ec2:ResourceTag/${TagKey}",
+                "ec2:SecurityGroupID",
+                "ec2:Vpc"
+            ],
+            "description": "Grants permission to add one or more outbound rules to a VPC security group. Policies using the security-group-rule resource-level permission are only enforced when the API request includes TagSpecifications",
             "orphan": false,
-            "resources": []
+            "resources": [
+                "security-group",
+                "security-group-rule"
+            ]
         },
         "AuthorizeSecurityGroupIngress": {
-            "access_level": "Undocumented",
+            "access_level": "Write",
             "action": "AuthorizeSecurityGroupIngress",
-            "condition_keys": [],
-            "description": "Not Documented by AWS",
+            "condition_keys": [
+                "aws:RequestTag/${TagKey}",
+                "aws:ResourceTag/${TagKey}",
+                "aws:TagKeys",
+                "ec2:Region",
+                "ec2:ResourceTag/${TagKey}",
+                "ec2:SecurityGroupID",
+                "ec2:Vpc"
+            ],
+            "description": "Grants permission to add one or more inbound rules to a VPC security group. Policies using the security-group-rule resource-level permission are only enforced when the API request includes TagSpecifications",
             "orphan": false,
-            "resources": []
+            "resources": [
+                "security-group",
+                "security-group-rule"
+            ]
         },
         "BundleInstance": {
-            "access_level": "Undocumented",
+            "access_level": "Write",
             "action": "BundleInstance",
-            "condition_keys": [],
-            "description": "Not Documented by AWS",
+            "condition_keys": [
+                "ec2:Region"
+            ],
+            "description": "Grants permission to bundle an instance store-backed Windows instance",
             "orphan": false,
             "resources": []
         },
         "CancelBundleTask": {
-            "access_level": "Undocumented",
+            "access_level": "Write",
             "action": "CancelBundleTask",
-            "condition_keys": [],
-            "description": "Not Documented by AWS",
+            "condition_keys": [
+                "ec2:Region"
+            ],
+            "description": "Grants permission to cancel a bundling operation",
             "orphan": false,
             "resources": []
         },
         "CancelCapacityReservation": {
-            "access_level": "Undocumented",
+            "access_level": "Write",
             "action": "CancelCapacityReservation",
-            "condition_keys": [],
-            "description": "Not Documented by AWS",
+            "condition_keys": [
+                "aws:ResourceTag/${TagKey}",
+                "ec2:CapacityReservationFleet",
+                "ec2:Region",
+                "ec2:ResourceTag/${TagKey}"
+            ],
+            "description": "Grants permission to cancel a Capacity Reservation and release the reserved capacity",
             "orphan": false,
-            "resources": []
+            "resources": [
+                "capacity-reservation"
+            ]
         },
         "CancelCapacityReservationFleets": {
-            "access_level": "Undocumented",
+            "access_level": "Write",
             "action": "CancelCapacityReservationFleets",
-            "condition_keys": [],
-            "description": "Not Documented by AWS",
+            "condition_keys": [
+                "aws:ResourceTag/${TagKey}",
+                "ec2:Region",
+                "ec2:ResourceTag/${TagKey}"
+            ],
+            "description": "Grants permission to cancel one or more Capacity Reservation Fleets",
             "orphan": false,
-            "resources": []
+            "resources": [
+                "capacity-reservation-fleet"
+            ]
         },
         "CancelConversionTask": {
-            "access_level": "Undocumented",
+            "access_level": "Write",
             "action": "CancelConversionTask",
-            "condition_keys": [],
-            "description": "Not Documented by AWS",
+            "condition_keys": [
+                "ec2:Region"
+            ],
+            "description": "Grants permission to cancel an active conversion task",
             "orphan": false,
             "resources": []
         },
         "CancelExportTask": {
-            "access_level": "Undocumented",
+            "access_level": "Write",
             "action": "CancelExportTask",
-            "condition_keys": [],
-            "description": "Not Documented by AWS",
+            "condition_keys": [
+                "aws:ResourceTag/${TagKey}",
+                "ec2:Region",
+                "ec2:ResourceTag/${TagKey}"
+            ],
+            "description": "Grants permission to cancel an active export task",
             "orphan": false,
-            "resources": []
+            "resources": [
+                "export-image-task",
+                "export-instance-task"
+            ]
         },
         "CancelImageLaunchPermission": {
-            "access_level": "Undocumented",
+            "access_level": "Write",
             "action": "CancelImageLaunchPermission",
-            "condition_keys": [],
-            "description": "Not Documented by AWS",
+            "condition_keys": [
+                "aws:ResourceTag/${TagKey}",
+                "ec2:ImageID",
+                "ec2:ImageType",
+                "ec2:Owner",
+                "ec2:Public",
+                "ec2:Region",
+                "ec2:ResourceTag/${TagKey}",
+                "ec2:RootDeviceType"
+            ],
+            "description": "Grants permission to remove your AWS account from the launch permissions for the specified AMI",
             "orphan": false,
-            "resources": []
+            "resources": [
+                "image"
+            ]
         },
         "CancelImportTask": {
-            "access_level": "Undocumented",
+            "access_level": "Write",
             "action": "CancelImportTask",
-            "condition_keys": [],
-            "description": "Not Documented by AWS",
+            "condition_keys": [
+                "aws:ResourceTag/${TagKey}",
+                "ec2:Region",
+                "ec2:ResourceTag/${TagKey}"
+            ],
+            "description": "Grants permission to cancel an in-process import virtual machine or import snapshot task",
             "orphan": false,
-            "resources": []
+            "resources": [
+                "import-image-task",
+                "import-snapshot-task"
+            ]
         },
         "CancelReservedInstancesListing": {
-            "access_level": "Undocumented",
+            "access_level": "Write",
             "action": "CancelReservedInstancesListing",
-            "condition_keys": [],
-            "description": "Not Documented by AWS",
+            "condition_keys": [
+                "ec2:Region"
+            ],
+            "description": "Grants permission to cancel a Reserved Instance listing on the Reserved Instance Marketplace",
             "orphan": false,
             "resources": []
         },
         "CancelSpotFleetRequests": {
-            "access_level": "Undocumented",
+            "access_level": "Write",
             "action": "CancelSpotFleetRequests",
-            "condition_keys": [],
-            "description": "Not Documented by AWS",
+            "condition_keys": [
+                "aws:ResourceTag/${TagKey}",
+                "ec2:Region",
+                "ec2:ResourceTag/${TagKey}"
+            ],
+            "description": "Grants permission to cancel one or more Spot Fleet requests",
             "orphan": false,
-            "resources": []
+            "resources": [
+                "spot-fleet-request"
+            ]
         },
         "CancelSpotInstanceRequests": {
-            "access_level": "Undocumented",
+            "access_level": "Write",
             "action": "CancelSpotInstanceRequests",
-            "condition_keys": [],
-            "description": "Not Documented by AWS",
+            "condition_keys": [
+                "aws:ResourceTag/${TagKey}",
+                "ec2:Region",
+                "ec2:ResourceTag/${TagKey}"
+            ],
+            "description": "Grants permission to cancel one or more Spot Instance requests",
             "orphan": false,
-            "resources": []
+            "resources": [
+                "spot-instances-request"
+            ]
         },
         "ConfirmProductInstance": {
-            "access_level": "Undocumented",
+            "access_level": "Write",
             "action": "ConfirmProductInstance",
-            "condition_keys": [],
-            "description": "Not Documented by AWS",
+            "condition_keys": [
+                "ec2:Region"
+            ],
+            "description": "Grants permission to determine whether an owned product code is associated with an instance",
             "orphan": false,
             "resources": []
         },
         "CopyFpgaImage": {
-            "access_level": "Undocumented",
+            "access_level": "Write",
             "action": "CopyFpgaImage",
-            "condition_keys": [],
-            "description": "Not Documented by AWS",
+            "condition_keys": [
+                "ec2:Owner",
+                "ec2:Region"
+            ],
+            "description": "Grants permission to copy a source Amazon FPGA image (AFI) to the current Region. Resource-level permissions specified for this action apply to the new AFI only. They do not apply to the source AFI",
             "orphan": false,
-            "resources": []
+            "resources": [
+                "fpga-image"
+            ]
         },
         "CopyImage": {
-            "access_level": "Undocumented",
+            "access_level": "Write",
             "action": "CopyImage",
-            "condition_keys": [],
-            "description": "Not Documented by AWS",
+            "condition_keys": [
+                "ec2:ImageID",
+                "ec2:Owner",
+                "ec2:Region"
+            ],
+            "description": "Grants permission to copy an Amazon Machine Image (AMI) from a source Region to the current Region. Resource-level permissions specified for this action apply to the new AMI only. They do not apply to the source AMI",
             "orphan": false,
-            "resources": []
+            "resources": [
+                "image"
+            ]
         },
         "CopySnapshot": {
-            "access_level": "Undocumented",
+            "access_level": "Write",
             "action": "CopySnapshot",
-            "condition_keys": [],
-            "description": "Not Documented by AWS",
+            "condition_keys": [
+                "aws:RequestTag/${TagKey}",
+                "aws:TagKeys",
+                "ec2:OutpostArn",
+                "ec2:Region",
+                "ec2:SnapshotID"
+            ],
+            "description": "Grants permission to copy a point-in-time snapshot of an EBS volume and store it in Amazon S3. Resource-level permissions specified for this action apply to the new snapshot only. They do not apply to the source snapshot",
             "orphan": false,
-            "resources": []
+            "resources": [
+                "snapshot"
+            ]
         },
         "CreateCapacityReservation": {
-            "access_level": "Undocumented",
+            "access_level": "Write",
             "action": "CreateCapacityReservation",
-            "condition_keys": [],
-            "description": "Not Documented by AWS",
+            "condition_keys": [
+                "aws:RequestTag/${TagKey}",
+                "aws:TagKeys",
+                "ec2:CapacityReservationFleet",
+                "ec2:Region"
+            ],
+            "description": "Grants permission to create a Capacity Reservation",
             "orphan": false,
-            "resources": []
+            "resources": [
+                "capacity-reservation"
+            ]
         },
         "CreateCapacityReservationFleet": {
-            "access_level": "Undocumented",
+            "access_level": "Write",
             "action": "CreateCapacityReservationFleet",
-            "condition_keys": [],
-            "description": "Not Documented by AWS",
+            "condition_keys": [
+                "aws:RequestTag/${TagKey}",
+                "aws:TagKeys",
+                "ec2:Region"
+            ],
+            "description": "Grants permission to create a Capacity Reservation Fleet",
             "orphan": false,
-            "resources": []
+            "resources": [
+                "capacity-reservation-fleet"
+            ]
         },
         "CreateCarrierGateway": {
-            "access_level": "Undocumented",
+            "access_level": "Write",
             "action": "CreateCarrierGateway",
-            "condition_keys": [],
-            "description": "Not Documented by AWS",
+            "condition_keys": [
+                "aws:RequestTag/${TagKey}",
+                "aws:ResourceTag/${TagKey}",
+                "aws:TagKeys",
+                "ec2:Region",
+                "ec2:ResourceTag/${TagKey}",
+                "ec2:Tenancy",
+                "ec2:VpcID"
+            ],
+            "description": "Grants permission to create a carrier gateway and provides CSP connectivity to VPC customers",
             "orphan": false,
-            "resources": []
+            "resources": [
+                "carrier-gateway",
+                "vpc"
+            ]
         },
         "CreateClientVpnEndpoint": {
-            "access_level": "Undocumented",
+            "access_level": "Write",
             "action": "CreateClientVpnEndpoint",
-            "condition_keys": [],
-            "description": "Not Documented by AWS",
-            "orphan": false,
-            "resources": []
+            "condition_keys": [
+                "aws:RequestTag/${TagKey}",
+                "aws:ResourceTag/${TagKey}",
+                "aws:TagKeys",
+                "ec2:ClientRootCertificateChainArn",
+                "ec2:CloudwatchLogGroupArn",
+                "ec2:CloudwatchLogStreamArn",
+                "ec2:DirectoryArn",
+                "ec2:Region",
+                "ec2:ResourceTag/${TagKey}",
+                "ec2:SamlProviderArn",
+                "ec2:SecurityGroupID",
+                "ec2:ServerCertificateArn",
+                "ec2:VpcID"
+            ],
+            "description": "Grants permission to create a Client VPN endpoint",
+            "orphan": false,
+            "resources": [
+                "client-vpn-endpoint",
+                "security-group",
+                "vpc"
+            ]
         },
         "CreateClientVpnRoute": {
-            "access_level": "Undocumented",
+            "access_level": "Write",
             "action": "CreateClientVpnRoute",
-            "condition_keys": [],
-            "description": "Not Documented by AWS",
+            "condition_keys": [
+                "aws:ResourceTag/${TagKey}",
+                "ec2:ClientRootCertificateChainArn",
+                "ec2:CloudwatchLogGroupArn",
+                "ec2:CloudwatchLogStreamArn",
+                "ec2:DirectoryArn",
+                "ec2:Region",
+                "ec2:ResourceTag/${TagKey}",
+                "ec2:SamlProviderArn",
+                "ec2:ServerCertificateArn",
+                "ec2:SubnetID"
+            ],
+            "description": "Grants permission to add a network route to a Client VPN endpoint's route table",
             "orphan": false,
-            "resources": []
+            "resources": [
+                "client-vpn-endpoint",
+                "subnet"
+            ]
         },
         "CreateCoipCidr": {
-            "access_level": "Undocumented",
+            "access_level": "Write",
             "action": "CreateCoipCidr",
-            "condition_keys": [],
-            "description": "Not Documented by AWS",
+            "condition_keys": [
+                "aws:ResourceTag/${TagKey}",
+                "ec2:Region",
+                "ec2:ResourceTag/${TagKey}"
+            ],
+            "description": "Grants permission to create a range of customer-owned IP (CoIP) addresses",
             "orphan": false,
-            "resources": []
+            "resources": [
+                "coip-pool"
+            ]
         },
         "CreateCoipPool": {
-            "access_level": "Undocumented",
+            "access_level": "Write",
             "action": "CreateCoipPool",
-            "condition_keys": [],
-            "description": "Not Documented by AWS",
+            "condition_keys": [
+                "aws:RequestTag/${TagKey}",
+                "aws:ResourceTag/${TagKey}",
+                "aws:TagKeys",
+                "ec2:Region",
+                "ec2:ResourceTag/${TagKey}"
+            ],
+            "description": "Grants permission to create a pool of customer-owned IP (CoIP) addresses",
             "orphan": false,
-            "resources": []
+            "resources": [
+                "coip-pool",
+                "local-gateway-route-table"
+            ]
         },
         "CreateCoipPoolPermission": {
-            "access_level": "Undocumented",
+            "access_level": "Write",
             "action": "CreateCoipPoolPermission",
-            "condition_keys": [],
-            "description": "Not Documented by AWS",
+            "condition_keys": [
+                "aws:ResourceTag/${TagKey}",
+                "ec2:Region",
+                "ec2:ResourceTag/${TagKey}"
+            ],
+            "description": "Grants permission to allow a service to access a customer-owned IP (CoIP) pool",
             "orphan": false,
-            "resources": []
+            "resources": [
+                "coip-pool"
+            ]
         },
         "CreateCustomerGateway": {
-            "access_level": "Undocumented",
+            "access_level": "Write",
             "action": "CreateCustomerGateway",
-            "condition_keys": [],
-            "description": "Not Documented by AWS",
+            "condition_keys": [
+                "aws:RequestTag/${TagKey}",
+                "aws:TagKeys",
+                "ec2:Region"
+            ],
+            "description": "Grants permission to create a customer gateway, which provides information to AWS about your customer gateway device",
             "orphan": false,
-            "resources": []
+            "resources": [
+                "customer-gateway"
+            ]
         },
         "CreateDefaultSubnet": {
-            "access_level": "Undocumented",
+            "access_level": "Write",
             "action": "CreateDefaultSubnet",
-            "condition_keys": [],
-            "description": "Not Documented by AWS",
+            "condition_keys": [
+                "ec2:Region"
+            ],
+            "description": "Grants permission to create a default subnet in a specified Availability Zone in a default VPC",
             "orphan": false,
             "resources": []
         },
         "CreateDefaultVpc": {
-            "access_level": "Undocumented",
+            "access_level": "Write",
             "action": "CreateDefaultVpc",
-            "condition_keys": [],
-            "description": "Not Documented by AWS",
+            "condition_keys": [
+                "ec2:Region"
+            ],
+            "description": "Grants permission to create a default VPC with a default subnet in each Availability Zone",
             "orphan": false,
             "resources": []
         },
         "CreateDhcpOptions": {
-            "access_level": "Undocumented",
+            "access_level": "Write",
             "action": "CreateDhcpOptions",
-            "condition_keys": [],
-            "description": "Not Documented by AWS",
+            "condition_keys": [
+                "aws:RequestTag/${TagKey}",
+                "aws:TagKeys",
+                "ec2:DhcpOptionsID",
+                "ec2:Region"
+            ],
+            "description": "Grants permission to create a set of DHCP options for a VPC",
             "orphan": false,
-            "resources": []
+            "resources": [
+                "dhcp-options"
+            ]
         },
         "CreateEgressOnlyInternetGateway": {
-            "access_level": "Undocumented",
+            "access_level": "Write",
             "action": "CreateEgressOnlyInternetGateway",
-            "condition_keys": [],
-            "description": "Not Documented by AWS",
+            "condition_keys": [
+                "aws:RequestTag/${TagKey}",
+                "aws:ResourceTag/${TagKey}",
+                "aws:TagKeys",
+                "ec2:Region",
+                "ec2:ResourceTag/${TagKey}",
+                "ec2:Tenancy",
+                "ec2:VpcID"
+            ],
+            "description": "Grants permission to create an egress-only internet gateway for a VPC",
             "orphan": false,
-            "resources": []
+            "resources": [
+                "egress-only-internet-gateway",
+                "vpc"
+            ]
         },
         "CreateFleet": {
-            "access_level": "Undocumented",
+            "access_level": "Write",
             "action": "CreateFleet",
-            "condition_keys": [],
-            "description": "Not Documented by AWS",
+            "condition_keys": [
+                "aws:RequestTag/${TagKey}",
+                "aws:ResourceTag/${TagKey}",
+                "aws:TagKeys",
+                "ec2:AvailabilityZone",
+                "ec2:EbsOptimized",
+                "ec2:Encrypted",
+                "ec2:ImageID",
+                "ec2:ImageType",
+                "ec2:InstanceID",
+                "ec2:InstanceProfile",
+                "ec2:InstanceType",
+                "ec2:KeyPairName",
+                "ec2:KeyPairType",
+                "ec2:KmsKeyId",
+                "ec2:NetworkInterfaceID",
+                "ec2:Owner",
+                "ec2:ParentSnapshot",
+                "ec2:ParentVolume",
+                "ec2:PlacementGroup",
+                "ec2:PlacementGroupName",
+                "ec2:PlacementGroupStrategy",
+                "ec2:Public",
+                "ec2:Region",
+                "ec2:ResourceTag/${TagKey}",
+                "ec2:RootDeviceType",
+                "ec2:SecurityGroupID",
+                "ec2:SnapshotID",
+                "ec2:SnapshotTime",
+                "ec2:Subnet",
+                "ec2:SubnetID",
+                "ec2:Tenancy",
+                "ec2:VolumeID",
+                "ec2:VolumeIops",
+                "ec2:VolumeSize",
+                "ec2:VolumeThroughput",
+                "ec2:VolumeType",
+                "ec2:Vpc"
+            ],
+            "description": "Grants permission to launch an EC2 Fleet",
             "orphan": false,
-            "resources": []
+            "resources": [
+                "fleet",
+                "image",
+                "instance",
+                "key-pair",
+                "launch-template",
+                "network-interface",
+                "placement-group",
+                "security-group",
+                "snapshot",
+                "subnet",
+                "volume"
+            ]
         },
         "CreateFlowLogs": {
-            "access_level": "Undocumented",
+            "access_level": "Write",
             "action": "CreateFlowLogs",
-            "condition_keys": [],
-            "description": "Not Documented by AWS",
-            "orphan": false,
-            "resources": []
+            "condition_keys": [
+                "aws:RequestTag/${TagKey}",
+                "aws:ResourceTag/${TagKey}",
+                "aws:TagKeys",
+                "ec2:AvailabilityZone",
+                "ec2:NetworkInterfaceID",
+                "ec2:Region",
+                "ec2:ResourceTag/${TagKey}",
+                "ec2:Subnet",
+                "ec2:SubnetID",
+                "ec2:Tenancy",
+                "ec2:Vpc",
+                "ec2:VpcID"
+            ],
+            "description": "Grants permission to create one or more flow logs to capture IP traffic for a network interface",
+            "orphan": false,
+            "resources": [
+                "network-interface",
+                "subnet",
+                "vpc",
+                "vpc-flow-log"
+            ]
         },
         "CreateFpgaImage": {
-            "access_level": "Undocumented",
+            "access_level": "Write",
             "action": "CreateFpgaImage",
-            "condition_keys": [],
-            "description": "Not Documented by AWS",
+            "condition_keys": [
+                "aws:RequestTag/${TagKey}",
+                "aws:TagKeys",
+                "ec2:Owner",
+                "ec2:Public",
+                "ec2:Region"
+            ],
+            "description": "Grants permission to create an Amazon FPGA Image (AFI) from a design checkpoint (DCP)",
             "orphan": false,
-            "resources": []
+            "resources": [
+                "fpga-image"
+            ]
         },
         "CreateImage": {
-            "access_level": "Undocumented",
+            "access_level": "Write",
             "action": "CreateImage",
-            "condition_keys": [],
-            "description": "Not Documented by AWS",
+            "condition_keys": [
+                "aws:RequestTag/${TagKey}",
+                "aws:ResourceTag/${TagKey}",
+                "aws:TagKeys",
+                "ec2:AvailabilityZone",
+                "ec2:EbsOptimized",
+                "ec2:ImageID",
+                "ec2:InstanceAutoRecovery",
+                "ec2:InstanceID",
+                "ec2:InstanceMarketType",
+                "ec2:InstanceMetadataTags",
+                "ec2:InstanceProfile",
+                "ec2:InstanceType",
+                "ec2:MetadataHttpEndpoint",
+                "ec2:MetadataHttpPutResponseHopLimit",
+                "ec2:MetadataHttpTokens",
+                "ec2:OutpostArn",
+                "ec2:Owner",
+                "ec2:ParentVolume",
+                "ec2:PlacementGroup",
+                "ec2:ProductCode",
+                "ec2:Region",
+                "ec2:ResourceTag/${TagKey}",
+                "ec2:RootDeviceType",
+                "ec2:SnapshotID",
+                "ec2:SnapshotTime",
+                "ec2:SourceOutpostArn",
+                "ec2:Tenancy",
+                "ec2:VolumeSize"
+            ],
+            "description": "Grants permission to create an Amazon EBS-backed AMI from a stopped or running Amazon EBS-backed instance",
             "orphan": false,
-            "resources": []
+            "resources": [
+                "image",
+                "instance",
+                "snapshot"
+            ]
         },
         "CreateInstanceEventWindow": {
-            "access_level": "Undocumented",
+            "access_level": "Write",
             "action": "CreateInstanceEventWindow",
-            "condition_keys": [],
-            "description": "Not Documented by AWS",
+            "condition_keys": [
+                "aws:RequestTag/${TagKey}",
+                "aws:TagKeys",
+                "ec2:Region"
+            ],
+            "description": "Grants permission to create an event window in which scheduled events for the associated Amazon EC2 instances can run",
             "orphan": false,
-            "resources": []
+            "resources": [
+                "instance-event-window"
+            ]
         },
         "CreateInstanceExportTask": {
-            "access_level": "Undocumented",
+            "access_level": "Write",
             "action": "CreateInstanceExportTask",
-            "condition_keys": [],
-            "description": "Not Documented by AWS",
+            "condition_keys": [
+                "aws:RequestTag/${TagKey}",
+                "aws:ResourceTag/${TagKey}",
+                "aws:TagKeys",
+                "ec2:AvailabilityZone",
+                "ec2:EbsOptimized",
+                "ec2:InstanceAutoRecovery",
+                "ec2:InstanceID",
+                "ec2:InstanceMarketType",
+                "ec2:InstanceMetadataTags",
+                "ec2:InstanceProfile",
+                "ec2:InstanceType",
+                "ec2:MetadataHttpEndpoint",
+                "ec2:MetadataHttpPutResponseHopLimit",
+                "ec2:MetadataHttpTokens",
+                "ec2:ProductCode",
+                "ec2:Region",
+                "ec2:ResourceTag/${TagKey}",
+                "ec2:RootDeviceType",
+                "ec2:Tenancy"
+            ],
+            "description": "Grants permission to export a running or stopped instance to an Amazon S3 bucket",
             "orphan": false,
-            "resources": []
+            "resources": [
+                "export-instance-task",
+                "instance"
+            ]
         },
         "CreateInternetGateway": {
-            "access_level": "Undocumented",
+            "access_level": "Write",
             "action": "CreateInternetGateway",
-            "condition_keys": [],
-            "description": "Not Documented by AWS",
+            "condition_keys": [
+                "aws:RequestTag/${TagKey}",
+                "aws:TagKeys",
+                "ec2:InternetGatewayID",
+                "ec2:Region"
+            ],
+            "description": "Grants permission to create an internet gateway for a VPC",
             "orphan": false,
-            "resources": []
+            "resources": [
+                "internet-gateway"
+            ]
         },
         "CreateIpam": {
-            "access_level": "Undocumented",
+            "access_level": "Write",
             "action": "CreateIpam",
-            "condition_keys": [],
-            "description": "Not Documented by AWS",
+            "condition_keys": [
+                "aws:RequestTag/${TagKey}",
+                "aws:TagKeys",
+                "ec2:Region"
+            ],
+            "description": "Grants permission to create an Amazon VPC IP Address Manager (IPAM)",
             "orphan": false,
-            "resources": []
+            "resources": [
+                "ipam"
+            ]
         },
         "CreateIpamPool": {
-            "access_level": "Undocumented",
+            "access_level": "Write",
             "action": "CreateIpamPool",
-            "condition_keys": [],
-            "description": "Not Documented by AWS",
+            "condition_keys": [
+                "aws:RequestTag/${TagKey}",
+                "aws:ResourceTag/${TagKey}",
+                "aws:TagKeys",
+                "ec2:Region",
+                "ec2:ResourceTag/${TagKey}"
+            ],
+            "description": "Grants permission to create an IP address pool for Amazon VPC IP Address Manager (IPAM), which is a collection of contiguous IP address CIDRs",
             "orphan": false,
-            "resources": []
+            "resources": [
+                "ipam-pool",
+                "ipam-scope"
+            ]
         },
         "CreateIpamResourceDiscovery": {
-            "access_level": "Undocumented",
+            "access_level": "Write",
             "action": "CreateIpamResourceDiscovery",
-            "condition_keys": [],
-            "description": "Not Documented by AWS",
+            "condition_keys": [
+                "aws:RequestTag/${TagKey}",
+                "aws:TagKeys",
+                "ec2:Region"
+            ],
+            "description": "Grants permission to create an IPAM resource discovery",
             "orphan": false,
-            "resources": []
+            "resources": [
+                "ipam-resource-discovery"
+            ]
         },
         "CreateIpamScope": {
-            "access_level": "Undocumented",
+            "access_level": "Write",
             "action": "CreateIpamScope",
-            "condition_keys": [],
-            "description": "Not Documented by AWS",
+            "condition_keys": [
+                "aws:RequestTag/${TagKey}",
+                "aws:ResourceTag/${TagKey}",
+                "aws:TagKeys",
+                "ec2:Region",
+                "ec2:ResourceTag/${TagKey}"
+            ],
+            "description": "Grants permission to create an Amazon VPC IP Address Manager (IPAM) scope, which is the highest-level container within IPAM",
             "orphan": false,
-            "resources": []
+            "resources": [
+                "ipam",
+                "ipam-scope"
+            ]
         },
         "CreateKeyPair": {
-            "access_level": "Undocumented",
+            "access_level": "Write",
             "action": "CreateKeyPair",
-            "condition_keys": [],
-            "description": "Not Documented by AWS",
+            "condition_keys": [
+                "aws:RequestTag/${TagKey}",
+                "aws:TagKeys",
+                "ec2:KeyPairType",
+                "ec2:Region"
+            ],
+            "description": "Grants permission to create a 2048-bit RSA key pair",
             "orphan": false,
-            "resources": []
+            "resources": [
+                "key-pair"
+            ]
         },
         "CreateLaunchTemplate": {
-            "access_level": "Undocumented",
+            "access_level": "Write",
             "action": "CreateLaunchTemplate",
-            "condition_keys": [],
-            "description": "Not Documented by AWS",
+            "condition_keys": [
+                "aws:RequestTag/${TagKey}",
+                "aws:TagKeys",
+                "ec2:Region"
+            ],
+            "description": "Grants permission to create a launch template",
             "orphan": false,
-            "resources": []
+            "resources": [
+                "launch-template"
+            ]
         },
         "CreateLaunchTemplateVersion": {
-            "access_level": "Undocumented",
+            "access_level": "Write",
             "action": "CreateLaunchTemplateVersion",
-            "condition_keys": [],
-            "description": "Not Documented by AWS",
+            "condition_keys": [
+                "aws:ResourceTag/${TagKey}",
+                "ec2:Region",
+                "ec2:ResourceTag/${TagKey}"
+            ],
+            "description": "Grants permission to create a new version of a launch template",
             "orphan": false,
-            "resources": []
+            "resources": [
+                "launch-template"
+            ]
         },
         "CreateLocalGatewayRoute": {
-            "access_level": "Undocumented",
+            "access_level": "Write",
             "action": "CreateLocalGatewayRoute",
-            "condition_keys": [],
-            "description": "Not Documented by AWS",
+            "condition_keys": [
+                "aws:ResourceTag/${TagKey}",
+                "ec2:AvailabilityZone",
+                "ec2:NetworkInterfaceID",
+                "ec2:Region",
+                "ec2:ResourceTag/${TagKey}",
+                "ec2:Subnet",
+                "ec2:Vpc"
+            ],
+            "description": "Grants permission to create a static route for a local gateway route table",
             "orphan": false,
-            "resources": []
+            "resources": [
+                "local-gateway-route-table",
+                "local-gateway-virtual-interface-group",
+                "network-interface",
+                "prefix-list"
+            ]
         },
         "CreateLocalGatewayRouteTable": {
-            "access_level": "Undocumented",
+            "access_level": "Write",
             "action": "CreateLocalGatewayRouteTable",
-            "condition_keys": [],
-            "description": "Not Documented by AWS",
+            "condition_keys": [
+                "aws:RequestTag/${TagKey}",
+                "aws:ResourceTag/${TagKey}",
+                "aws:TagKeys",
+                "ec2:Region",
+                "ec2:ResourceTag/${TagKey}"
+            ],
+            "description": "Grants permission to create a local gateway route table",
             "orphan": false,
-            "resources": []
+            "resources": [
+                "local-gateway",
+                "local-gateway-route-table"
+            ]
         },
         "CreateLocalGatewayRouteTablePermission": {
-            "access_level": "Undocumented",
+            "access_level": "Write",
             "action": "CreateLocalGatewayRouteTablePermission",
-            "condition_keys": [],
-            "description": "Not Documented by AWS",
+            "condition_keys": [
+                "aws:ResourceTag/${TagKey}",
+                "ec2:Region",
+                "ec2:ResourceTag/${TagKey}"
+            ],
+            "description": "Grants permission to allow a service to access a local gateway route table",
             "orphan": false,
-            "resources": []
+            "resources": [
+                "local-gateway-route-table"
+            ]
         },
         "CreateLocalGatewayRouteTableVirtualInterfaceGroupAssociation": {
-            "access_level": "Undocumented",
+            "access_level": "Write",
             "action": "CreateLocalGatewayRouteTableVirtualInterfaceGroupAssociation",
-            "condition_keys": [],
-            "description": "Not Documented by AWS",
+            "condition_keys": [
+                "aws:RequestTag/${TagKey}",
+                "aws:ResourceTag/${TagKey}",
+                "aws:TagKeys",
+                "ec2:Region",
+                "ec2:ResourceTag/${TagKey}"
+            ],
+            "description": "Grants permission to create a local gateway route table virtual interface group association",
             "orphan": false,
-            "resources": []
+            "resources": [
+                "local-gateway-route-table",
+                "local-gateway-route-table-virtual-interface-group-association",
+                "local-gateway-virtual-interface-group"
+            ]
         },
         "CreateLocalGatewayRouteTableVpcAssociation": {
-            "access_level": "Undocumented",
+            "access_level": "Write",
             "action": "CreateLocalGatewayRouteTableVpcAssociation",
-            "condition_keys": [],
-            "description": "Not Documented by AWS",
+            "condition_keys": [
+                "aws:RequestTag/${TagKey}",
+                "aws:ResourceTag/${TagKey}",
+                "aws:TagKeys",
+                "ec2:Region",
+                "ec2:ResourceTag/${TagKey}",
+                "ec2:Tenancy",
+                "ec2:VpcID"
+            ],
+            "description": "Grants permission to associate a VPC with a local gateway route table",
             "orphan": false,
-            "resources": []
+            "resources": [
+                "local-gateway-route-table",
+                "local-gateway-route-table-vpc-association",
+                "vpc"
+            ]
         },
         "CreateManagedPrefixList": {
-            "access_level": "Undocumented",
+            "access_level": "Write",
             "action": "CreateManagedPrefixList",
-            "condition_keys": [],
-            "description": "Not Documented by AWS",
+            "condition_keys": [
+                "aws:RequestTag/${TagKey}",
+                "aws:TagKeys",
+                "ec2:Region"
+            ],
+            "description": "Grants permission to create a managed prefix list",
             "orphan": false,
-            "resources": []
+            "resources": [
+                "prefix-list"
+            ]
         },
         "CreateNatGateway": {
-            "access_level": "Undocumented",
+            "access_level": "Write",
             "action": "CreateNatGateway",
-            "condition_keys": [],
-            "description": "Not Documented by AWS",
+            "condition_keys": [
+                "aws:RequestTag/${TagKey}",
+                "aws:ResourceTag/${TagKey}",
+                "aws:TagKeys",
+                "ec2:AllocationId",
+                "ec2:AvailabilityZone",
+                "ec2:Domain",
+                "ec2:PublicIpAddress",
+                "ec2:Region",
+                "ec2:ResourceTag/${TagKey}",
+                "ec2:SubnetID",
+                "ec2:Vpc"
+            ],
+            "description": "Grants permission to create a NAT gateway in a subnet",
             "orphan": false,
-            "resources": []
+            "resources": [
+                "elastic-ip",
+                "natgateway",
+                "subnet"
+            ]
         },
         "CreateNetworkAcl": {
-            "access_level": "Undocumented",
+            "access_level": "Write",
             "action": "CreateNetworkAcl",
-            "condition_keys": [],
-            "description": "Not Documented by AWS",
+            "condition_keys": [
+                "aws:RequestTag/${TagKey}",
+                "aws:ResourceTag/${TagKey}",
+                "aws:TagKeys",
+                "ec2:NetworkAclID",
+                "ec2:Region",
+                "ec2:ResourceTag/${TagKey}",
+                "ec2:Tenancy",
+                "ec2:VpcID"
+            ],
+            "description": "Grants permission to create a network ACL in a VPC",
             "orphan": false,
-            "resources": []
+            "resources": [
+                "network-acl",
+                "vpc"
+            ]
         },
         "CreateNetworkAclEntry": {
-            "access_level": "Undocumented",
+            "access_level": "Write",
             "action": "CreateNetworkAclEntry",
-            "condition_keys": [],
-            "description": "Not Documented by AWS",
+            "condition_keys": [
+                "aws:ResourceTag/${TagKey}",
+                "ec2:NetworkAclID",
+                "ec2:Region",
+                "ec2:ResourceTag/${TagKey}",
+                "ec2:Vpc"
+            ],
+            "description": "Grants permission to create a numbered entry (a rule) in a network ACL",
             "orphan": false,
-            "resources": []
+            "resources": [
+                "network-acl"
+            ]
         },
         "CreateNetworkInsightsAccessScope": {
-            "access_level": "Undocumented",
+            "access_level": "Write",
             "action": "CreateNetworkInsightsAccessScope",
-            "condition_keys": [],
-            "description": "Not Documented by AWS",
+            "condition_keys": [
+                "aws:RequestTag/${TagKey}",
+                "aws:TagKeys",
+                "ec2:Region"
+            ],
+            "description": "Grants permission to create a Network Access Scope",
             "orphan": false,
-            "resources": []
+            "resources": [
+                "network-insights-access-scope"
+            ]
         },
         "CreateNetworkInsightsPath": {
-            "access_level": "Undocumented",
+            "access_level": "Write",
             "action": "CreateNetworkInsightsPath",
-            "condition_keys": [],
-            "description": "Not Documented by AWS",
+            "condition_keys": [
+                "aws:RequestTag/${TagKey}",
+                "aws:ResourceTag/${TagKey}",
+                "aws:TagKeys",
+                "ec2:AccepterVpc",
+                "ec2:AvailabilityZone",
+                "ec2:EbsOptimized",
+                "ec2:InstanceID",
+                "ec2:InstanceProfile",
+                "ec2:InstanceType",
+                "ec2:InternetGatewayID",
+                "ec2:NetworkInterfaceID",
+                "ec2:PlacementGroup",
+                "ec2:Region",
+                "ec2:RequesterVpc",
+                "ec2:ResourceTag/${TagKey}",
+                "ec2:RootDeviceType",
+                "ec2:Subnet",
+                "ec2:Tenancy",
+                "ec2:Vpc",
+                "ec2:VpcPeeringConnectionID"
+            ],
+            "description": "Grants permission to create a path to analyze for reachability",
             "orphan": false,
-            "resources": []
+            "resources": [
+                "instance",
+                "internet-gateway",
+                "network-insights-path",
+                "network-interface",
+                "transit-gateway",
+                "vpc-endpoint",
+                "vpc-endpoint-service",
+                "vpc-peering-connection",
+                "vpn-gateway"
+            ]
         },
         "CreateNetworkInterface": {
-            "access_level": "Undocumented",
+            "access_level": "Write",
             "action": "CreateNetworkInterface",
-            "condition_keys": [],
-            "description": "Not Documented by AWS",
+            "condition_keys": [
+                "aws:RequestTag/${TagKey}",
+                "aws:ResourceTag/${TagKey}",
+                "aws:TagKeys",
+                "ec2:AvailabilityZone",
+                "ec2:NetworkInterfaceID",
+                "ec2:Region",
+                "ec2:ResourceTag/${TagKey}",
+                "ec2:SecurityGroupID",
+                "ec2:SubnetID",
+                "ec2:Vpc"
+            ],
+            "description": "Grants permission to create a network interface in a subnet",
             "orphan": false,
-            "resources": []
+            "resources": [
+                "network-interface",
+                "security-group",
+                "subnet"
+            ]
         },
         "CreateNetworkInterfacePermission": {
-            "access_level": "Undocumented",
+            "access_level": "Permissions management",
             "action": "CreateNetworkInterfacePermission",
-            "condition_keys": [],
-            "description": "Not Documented by AWS",
+            "condition_keys": [
+                "aws:ResourceTag/${TagKey}",
+                "ec2:AuthorizedService",
+                "ec2:AuthorizedUser",
+                "ec2:AvailabilityZone",
+                "ec2:NetworkInterfaceID",
+                "ec2:Permission",
+                "ec2:Region",
+                "ec2:ResourceTag/${TagKey}",
+                "ec2:Subnet",
+                "ec2:Vpc"
+            ],
+            "description": "Grants permission to create a permission for an AWS-authorized user to perform certain operations on a network interface",
             "orphan": false,
-            "resources": []
+            "resources": [
+                "network-interface"
+            ]
         },
         "CreatePlacementGroup": {
-            "access_level": "Undocumented",
+            "access_level": "Write",
             "action": "CreatePlacementGroup",
-            "condition_keys": [],
-            "description": "Not Documented by AWS",
+            "condition_keys": [
+                "aws:RequestTag/${TagKey}",
+                "aws:TagKeys",
+                "ec2:PlacementGroupName",
+                "ec2:PlacementGroupStrategy",
+                "ec2:Region"
+            ],
+            "description": "Grants permission to create a placement group",
             "orphan": false,
-            "resources": []
+            "resources": [
+                "placement-group"
+            ]
         },
         "CreatePublicIpv4Pool": {
-            "access_level": "Undocumented",
+            "access_level": "Write",
             "action": "CreatePublicIpv4Pool",
-            "condition_keys": [],
-            "description": "Not Documented by AWS",
+            "condition_keys": [
+                "aws:RequestTag/${TagKey}",
+                "aws:TagKeys",
+                "ec2:Region"
+            ],
+            "description": "Grants permission to create a public IPv4 address pool for public IPv4 CIDRs that you own and bring to Amazon to manage with Amazon VPC IP Address Manager (IPAM)",
             "orphan": false,
-            "resources": []
+            "resources": [
+                "ipv4pool-ec2"
+            ]
         },
         "CreateReplaceRootVolumeTask": {
-            "access_level": "Undocumented",
+            "access_level": "Write",
             "action": "CreateReplaceRootVolumeTask",
-            "condition_keys": [],
-            "description": "Not Documented by AWS",
+            "condition_keys": [
+                "aws:RequestTag/${TagKey}",
+                "aws:ResourceTag/${TagKey}",
+                "aws:TagKeys",
+                "ec2:AvailabilityZone",
+                "ec2:EbsOptimized",
+                "ec2:ImageID",
+                "ec2:ImageType",
+                "ec2:InstanceAutoRecovery",
+                "ec2:InstanceID",
+                "ec2:InstanceMarketType",
+                "ec2:InstanceMetadataTags",
+                "ec2:InstanceProfile",
+                "ec2:InstanceType",
+                "ec2:MetadataHttpEndpoint",
+                "ec2:MetadataHttpPutResponseHopLimit",
+                "ec2:MetadataHttpTokens",
+                "ec2:Owner",
+                "ec2:ParentVolume",
+                "ec2:PlacementGroup",
+                "ec2:ProductCode",
+                "ec2:Public",
+                "ec2:Region",
+                "ec2:ResourceTag/${TagKey}",
+                "ec2:RootDeviceType",
+                "ec2:SnapshotID",
+                "ec2:SnapshotTime",
+                "ec2:Tenancy",
+                "ec2:VolumeID",
+                "ec2:VolumeSize"
+            ],
+            "description": "Grants permission to create a root volume replacement task",
             "orphan": false,
-            "resources": []
+            "resources": [
+                "image",
+                "instance",
+                "replace-root-volume-task",
+                "snapshot",
+                "volume"
+            ]
         },
         "CreateReservedInstancesListing": {
-            "access_level": "Undocumented",
+            "access_level": "Write",
             "action": "CreateReservedInstancesListing",
-            "condition_keys": [],
-            "description": "Not Documented by AWS",
+            "condition_keys": [
+                "ec2:Region"
+            ],
+            "description": "Grants permission to create a listing for Standard Reserved Instances to be sold in the Reserved Instance Marketplace",
             "orphan": false,
             "resources": []
         },
         "CreateRestoreImageTask": {
-            "access_level": "Undocumented",
+            "access_level": "Write",
             "action": "CreateRestoreImageTask",
-            "condition_keys": [],
-            "description": "Not Documented by AWS",
+            "condition_keys": [
+                "aws:RequestTag/${TagKey}",
+                "aws:TagKeys",
+                "ec2:ImageID",
+                "ec2:Owner",
+                "ec2:Region"
+            ],
+            "description": "Grants permission to start a task that restores an AMI from an S3 object previously created by using CreateStoreImageTask",
             "orphan": false,
-            "resources": []
+            "resources": [
+                "image"
+            ]
         },
         "CreateRoute": {
-            "access_level": "Undocumented",
+            "access_level": "Write",
             "action": "CreateRoute",
-            "condition_keys": [],
-            "description": "Not Documented by AWS",
+            "condition_keys": [
+                "aws:ResourceTag/${TagKey}",
+                "ec2:Region",
+                "ec2:ResourceTag/${TagKey}",
+                "ec2:RouteTableID",
+                "ec2:Vpc"
+            ],
+            "description": "Grants permission to create a route in a VPC route table",
             "orphan": false,
-            "resources": []
+            "resources": [
+                "route-table"
+            ]
         },
         "CreateRouteTable": {
-            "access_level": "Undocumented",
+            "access_level": "Write",
             "action": "CreateRouteTable",
-            "condition_keys": [],
-            "description": "Not Documented by AWS",
+            "condition_keys": [
+                "aws:RequestTag/${TagKey}",
+                "aws:ResourceTag/${TagKey}",
+                "aws:TagKeys",
+                "ec2:Region",
+                "ec2:ResourceTag/${TagKey}",
+                "ec2:RouteTableID",
+                "ec2:Tenancy",
+                "ec2:VpcID"
+            ],
+            "description": "Grants permission to create a route table for a VPC",
             "orphan": false,
-            "resources": []
+            "resources": [
+                "route-table",
+                "vpc"
+            ]
         },
         "CreateSecurityGroup": {
-            "access_level": "Undocumented",
+            "access_level": "Write",
             "action": "CreateSecurityGroup",
-            "condition_keys": [],
-            "description": "Not Documented by AWS",
+            "condition_keys": [
+                "aws:RequestTag/${TagKey}",
+                "aws:ResourceTag/${TagKey}",
+                "aws:TagKeys",
+                "ec2:Region",
+                "ec2:ResourceTag/${TagKey}",
+                "ec2:SecurityGroupID",
+                "ec2:Tenancy",
+                "ec2:VpcID"
+            ],
+            "description": "Grants permission to create a security group",
             "orphan": false,
-            "resources": []
+            "resources": [
+                "security-group",
+                "vpc"
+            ]
         },
         "CreateSnapshot": {
-            "access_level": "Undocumented",
+            "access_level": "Write",
             "action": "CreateSnapshot",
-            "condition_keys": [],
-            "description": "Not Documented by AWS",
+            "condition_keys": [
+                "aws:RequestTag/${TagKey}",
+                "aws:ResourceTag/${TagKey}",
+                "aws:TagKeys",
+                "ec2:Encrypted",
+                "ec2:OutpostArn",
+                "ec2:ParentVolume",
+                "ec2:Region",
+                "ec2:ResourceTag/${TagKey}",
+                "ec2:SnapshotID",
+                "ec2:SourceOutpostArn",
+                "ec2:VolumeID",
+                "ec2:VolumeIops",
+                "ec2:VolumeSize",
+                "ec2:VolumeThroughput",
+                "ec2:VolumeType"
+            ],
+            "description": "Grants permission to create a snapshot of an EBS volume and store it in Amazon S3",
             "orphan": false,
-            "resources": []
+            "resources": [
+                "snapshot",
+                "volume"
+            ]
         },
         "CreateSnapshots": {
-            "access_level": "Undocumented",
+            "access_level": "Write",
             "action": "CreateSnapshots",
-            "condition_keys": [],
-            "description": "Not Documented by AWS",
+            "condition_keys": [
+                "aws:RequestTag/${TagKey}",
+                "aws:ResourceTag/${TagKey}",
+                "aws:TagKeys",
+                "ec2:AvailabilityZone",
+                "ec2:EbsOptimized",
+                "ec2:Encrypted",
+                "ec2:InstanceID",
+                "ec2:InstanceProfile",
+                "ec2:InstanceType",
+                "ec2:OutpostArn",
+                "ec2:ParentVolume",
+                "ec2:PlacementGroup",
+                "ec2:Region",
+                "ec2:ResourceTag/${TagKey}",
+                "ec2:RootDeviceType",
+                "ec2:SnapshotID",
+                "ec2:SourceOutpostArn",
+                "ec2:Tenancy",
+                "ec2:VolumeID",
+                "ec2:VolumeIops",
+                "ec2:VolumeSize",
+                "ec2:VolumeThroughput",
+                "ec2:VolumeType"
+            ],
+            "description": "Grants permission to create crash-consistent snapshots of multiple EBS volumes and store them in Amazon S3",
             "orphan": false,
-            "resources": []
+            "resources": [
+                "instance",
+                "snapshot",
+                "volume"
+            ]
         },
         "CreateSpotDatafeedSubscription": {
-            "access_level": "Undocumented",
+            "access_level": "Write",
             "action": "CreateSpotDatafeedSubscription",
-            "condition_keys": [],
-            "description": "Not Documented by AWS",
+            "condition_keys": [
+                "ec2:Region"
+            ],
+            "description": "Grants permission to create a data feed for Spot Instances to view Spot Instance usage logs",
             "orphan": false,
             "resources": []
         },
         "CreateStoreImageTask": {
-            "access_level": "Undocumented",
+            "access_level": "Write",
             "action": "CreateStoreImageTask",
-            "condition_keys": [],
-            "description": "Not Documented by AWS",
+            "condition_keys": [
+                "aws:ResourceTag/${TagKey}",
+                "ec2:ImageID",
+                "ec2:ImageType",
+                "ec2:Owner",
+                "ec2:Public",
+                "ec2:Region",
+                "ec2:ResourceTag/${TagKey}",
+                "ec2:RootDeviceType"
+            ],
+            "description": "Grants permission to store an AMI as a single object in an S3 bucket",
             "orphan": false,
-            "resources": []
+            "resources": [
+                "image"
+            ]
         },
         "CreateSubnet": {
-            "access_level": "Undocumented",
+            "access_level": "Write",
             "action": "CreateSubnet",
-            "condition_keys": [],
-            "description": "Not Documented by AWS",
+            "condition_keys": [
+                "aws:RequestTag/${TagKey}",
+                "aws:ResourceTag/${TagKey}",
+                "aws:TagKeys",
+                "ec2:Region",
+                "ec2:ResourceTag/${TagKey}",
+                "ec2:SubnetID",
+                "ec2:Tenancy",
+                "ec2:VpcID"
+            ],
+            "description": "Grants permission to create a subnet in a VPC",
             "orphan": false,
-            "resources": []
+            "resources": [
+                "subnet",
+                "vpc"
+            ]
         },
         "CreateSubnetCidrReservation": {
-            "access_level": "Undocumented",
+            "access_level": "Write",
             "action": "CreateSubnetCidrReservation",
-            "condition_keys": [],
-            "description": "Not Documented by AWS",
+            "condition_keys": [
+                "ec2:Region"
+            ],
+            "description": "Grants permission to create a subnet CIDR reservation",
             "orphan": false,
             "resources": []
         },
         "CreateTags": {
-            "access_level": "Undocumented",
+            "access_level": "Tagging",
             "action": "CreateTags",
-            "condition_keys": [],
-            "description": "Not Documented by AWS",
-            "orphan": false,
-            "resources": []
+            "condition_keys": [
+                "aws:ResourceTag/${TagKey}",
+                "ec2:AccepterVpc",
+                "ec2:AllocationId",
+                "ec2:AuthenticationType",
+                "ec2:AuthorizedUser",
+                "ec2:AutoPlacement",
+                "ec2:AvailabilityZone",
+                "ec2:ClientRootCertificateChainArn",
+                "ec2:CloudwatchLogGroupArn",
+                "ec2:CloudwatchLogStreamArn",
+                "ec2:CreateAction",
+                "ec2:DPDTimeoutSeconds",
+                "ec2:DhcpOptionsID",
+                "ec2:DirectoryArn",
+                "ec2:Domain",
+                "ec2:EbsOptimized",
+                "ec2:ElasticGpuType",
+                "ec2:Encrypted",
+                "ec2:GatewayType",
+                "ec2:HostRecovery",
+                "ec2:IKEVersions",
+                "ec2:ImageID",
+                "ec2:ImageType",
+                "ec2:InsideTunnelCidr",
+                "ec2:InsideTunnelIpv6Cidr",
+                "ec2:InstanceAutoRecovery",
+                "ec2:InstanceID",
+                "ec2:InstanceMarketType",
+                "ec2:InstanceMetadataTags",
+                "ec2:InstanceProfile",
+                "ec2:InstanceType",
+                "ec2:InternetGatewayID",
+                "ec2:KeyPairName",
+                "ec2:KeyPairType",
+                "ec2:MetadataHttpEndpoint",
+                "ec2:MetadataHttpPutResponseHopLimit",
+                "ec2:MetadataHttpTokens",
+                "ec2:NetworkAclID",
+                "ec2:NetworkInterfaceID",
+                "ec2:Owner",
+                "ec2:ParentSnapshot",
+                "ec2:ParentVolume",
+                "ec2:Permission",
+                "ec2:Phase1DHGroup",
+                "ec2:Phase1EncryptionAlgorithms",
+                "ec2:Phase1IntegrityAlgorithms",
+                "ec2:Phase1LifetimeSeconds",
+                "ec2:Phase2DHGroup",
+                "ec2:Phase2EncryptionAlgorithms",
+                "ec2:Phase2IntegrityAlgorithms",
+                "ec2:Phase2LifetimeSeconds",
+                "ec2:PlacementGroup",
+                "ec2:PlacementGroupName",
+                "ec2:PlacementGroupStrategy",
+                "ec2:PreSharedKeys",
+                "ec2:ProductCode",
+                "ec2:Public",
+                "ec2:PublicIpAddress",
+                "ec2:Quantity",
+                "ec2:Region",
+                "ec2:RekeyFuzzPercentage",
+                "ec2:RekeyMarginTimeSeconds",
+                "ec2:ReplayWindowSizePackets",
+                "ec2:RequesterVpc",
+                "ec2:ReservedInstancesOfferingType",
+                "ec2:ResourceTag/${TagKey}",
+                "ec2:RootDeviceType",
+                "ec2:RouteTableID",
+                "ec2:RoutingType",
+                "ec2:SamlProviderArn",
+                "ec2:SecurityGroupID",
+                "ec2:ServerCertificateArn",
+                "ec2:SnapshotID",
+                "ec2:SnapshotTime",
+                "ec2:Subnet",
+                "ec2:SubnetID",
+                "ec2:Tenancy",
+                "ec2:VolumeID",
+                "ec2:VolumeIops",
+                "ec2:VolumeSize",
+                "ec2:VolumeThroughput",
+                "ec2:VolumeType",
+                "ec2:Vpc",
+                "ec2:VpcID",
+                "ec2:VpcPeeringConnectionID"
+            ],
+            "description": "Grants permission to add or overwrite one or more tags for Amazon EC2 resources",
+            "orphan": false,
+            "resources": [
+                "capacity-reservation",
+                "capacity-reservation-fleet",
+                "carrier-gateway",
+                "client-vpn-endpoint",
+                "coip-pool",
+                "customer-gateway",
+                "dedicated-host",
+                "dhcp-options",
+                "egress-only-internet-gateway",
+                "elastic-gpu",
+                "elastic-ip",
+                "export-image-task",
+                "export-instance-task",
+                "fleet",
+                "fpga-image",
+                "host-reservation",
+                "image",
+                "import-image-task",
+                "import-snapshot-task",
+                "instance",
+                "instance-event-window",
+                "internet-gateway",
+                "ipam",
+                "ipam-pool",
+                "ipam-resource-discovery",
+                "ipam-resource-discovery-association",
+                "ipam-scope",
+                "ipv4pool-ec2",
+                "ipv6pool-ec2",
+                "key-pair",
+                "launch-template",
+                "local-gateway",
+                "local-gateway-route-table",
+                "local-gateway-route-table-virtual-interface-group-association",
+                "local-gateway-route-table-vpc-association",
+                "local-gateway-virtual-interface",
+                "local-gateway-virtual-interface-group",
+                "natgateway",
+                "network-acl",
+                "network-insights-access-scope",
+                "network-insights-access-scope-analysis",
+                "network-insights-analysis",
+                "network-insights-path",
+                "network-interface",
+                "placement-group",
+                "prefix-list",
+                "replace-root-volume-task",
+                "reserved-instances",
+                "route-table",
+                "security-group",
+                "security-group-rule",
+                "snapshot",
+                "spot-fleet-request",
+                "spot-instances-request",
+                "subnet",
+                "subnet-cidr-reservation",
+                "traffic-mirror-filter",
+                "traffic-mirror-session",
+                "traffic-mirror-target",
+                "transit-gateway",
+                "transit-gateway-attachment",
+                "transit-gateway-connect-peer",
+                "transit-gateway-multicast-domain",
+                "transit-gateway-policy-table",
+                "transit-gateway-route-table",
+                "transit-gateway-route-table-announcement",
+                "verified-access-endpoint",
+                "verified-access-group",
+                "verified-access-instance",
+                "verified-access-policy",
+                "verified-access-trust-provider",
+                "volume",
+                "vpc",
+                "vpc-endpoint",
+                "vpc-endpoint-connection",
+                "vpc-endpoint-service",
+                "vpc-endpoint-service-permission",
+                "vpc-flow-log",
+                "vpc-peering-connection",
+                "vpn-connection",
+                "vpn-gateway"
+            ]
         },
         "CreateTrafficMirrorFilter": {
-            "access_level": "Undocumented",
+            "access_level": "Write",
             "action": "CreateTrafficMirrorFilter",
-            "condition_keys": [],
-            "description": "Not Documented by AWS",
+            "condition_keys": [
+                "aws:RequestTag/${TagKey}",
+                "aws:TagKeys",
+                "ec2:Region"
+            ],
+            "description": "Grants permission to create a traffic mirror filter",
             "orphan": false,
-            "resources": []
+            "resources": [
+                "traffic-mirror-filter"
+            ]
         },
         "CreateTrafficMirrorFilterRule": {
-            "access_level": "Undocumented",
+            "access_level": "Write",
             "action": "CreateTrafficMirrorFilterRule",
-            "condition_keys": [],
-            "description": "Not Documented by AWS",
+            "condition_keys": [
+                "aws:ResourceTag/${TagKey}",
+                "ec2:Region",
+                "ec2:ResourceTag/${TagKey}"
+            ],
+            "description": "Grants permission to create a traffic mirror filter rule",
             "orphan": false,
-            "resources": []
+            "resources": [
+                "traffic-mirror-filter"
+            ]
         },
         "CreateTrafficMirrorSession": {
-            "access_level": "Undocumented",
+            "access_level": "Write",
             "action": "CreateTrafficMirrorSession",
-            "condition_keys": [],
-            "description": "Not Documented by AWS",
+            "condition_keys": [
+                "aws:RequestTag/${TagKey}",
+                "aws:ResourceTag/${TagKey}",
+                "aws:TagKeys",
+                "ec2:NetworkInterfaceID",
+                "ec2:Region",
+                "ec2:ResourceTag/${TagKey}"
+            ],
+            "description": "Grants permission to create a traffic mirror session",
             "orphan": false,
-            "resources": []
+            "resources": [
+                "network-interface",
+                "traffic-mirror-filter",
+                "traffic-mirror-session",
+                "traffic-mirror-target"
+            ]
         },
         "CreateTrafficMirrorTarget": {
-            "access_level": "Undocumented",
+            "access_level": "Write",
             "action": "CreateTrafficMirrorTarget",
-            "condition_keys": [],
-            "description": "Not Documented by AWS",
+            "condition_keys": [
+                "aws:RequestTag/${TagKey}",
+                "aws:ResourceTag/${TagKey}",
+                "aws:TagKeys",
+                "ec2:NetworkInterfaceID",
+                "ec2:Region",
+                "ec2:ResourceTag/${TagKey}",
+                "ec2:VpceServiceName",
+                "ec2:VpceServiceOwner"
+            ],
+            "description": "Grants permission to create a traffic mirror target",
             "orphan": false,
-            "resources": []
+            "resources": [
+                "network-interface",
+                "traffic-mirror-target",
+                "vpc-endpoint"
+            ]
         },
         "CreateTransitGateway": {
-            "access_level": "Undocumented",
+            "access_level": "Write",
             "action": "CreateTransitGateway",
-            "condition_keys": [],
-            "description": "Not Documented by AWS",
+            "condition_keys": [
+                "aws:RequestTag/${TagKey}",
+                "aws:TagKeys",
+                "ec2:Region"
+            ],
+            "description": "Grants permission to create a transit gateway",
             "orphan": false,
-            "resources": []
+            "resources": [
+                "transit-gateway"
+            ]
         },
         "CreateTransitGatewayConnect": {
-            "access_level": "Undocumented",
+            "access_level": "Write",
             "action": "CreateTransitGatewayConnect",
-            "condition_keys": [],
-            "description": "Not Documented by AWS",
+            "condition_keys": [
+                "aws:RequestTag/${TagKey}",
+                "aws:TagKeys",
+                "ec2:Region"
+            ],
+            "description": "Grants permission to create a Connect attachment from a specified transit gateway attachment",
             "orphan": false,
-            "resources": []
+            "resources": [
+                "transit-gateway-attachment"
+            ]
         },
         "CreateTransitGatewayConnectPeer": {
-            "access_level": "Undocumented",
+            "access_level": "Write",
             "action": "CreateTransitGatewayConnectPeer",
-            "condition_keys": [],
-            "description": "Not Documented by AWS",
+            "condition_keys": [
+                "aws:RequestTag/${TagKey}",
+                "aws:ResourceTag/${TagKey}",
+                "aws:TagKeys",
+                "ec2:Region",
+                "ec2:ResourceTag/${TagKey}"
+            ],
+            "description": "Grants permission to create a Connect peer between a transit gateway and an appliance",
             "orphan": false,
-            "resources": []
+            "resources": [
+                "transit-gateway-attachment",
+                "transit-gateway-connect-peer"
+            ]
         },
         "CreateTransitGatewayMulticastDomain": {
-            "access_level": "Undocumented",
+            "access_level": "Write",
             "action": "CreateTransitGatewayMulticastDomain",
-            "condition_keys": [],
-            "description": "Not Documented by AWS",
+            "condition_keys": [
+                "aws:RequestTag/${TagKey}",
+                "aws:ResourceTag/${TagKey}",
+                "aws:TagKeys",
+                "ec2:Region",
+                "ec2:ResourceTag/${TagKey}"
+            ],
+            "description": "Grants permission to create a multicast domain for a transit gateway",
             "orphan": false,
-            "resources": []
+            "resources": [
+                "transit-gateway",
+                "transit-gateway-multicast-domain"
+            ]
         },
         "CreateTransitGatewayPeeringAttachment": {
-            "access_level": "Undocumented",
+            "access_level": "Write",
             "action": "CreateTransitGatewayPeeringAttachment",
-            "condition_keys": [],
-            "description": "Not Documented by AWS",
+            "condition_keys": [
+                "aws:RequestTag/${TagKey}",
+                "aws:ResourceTag/${TagKey}",
+                "aws:TagKeys",
+                "ec2:Region",
+                "ec2:ResourceTag/${TagKey}"
+            ],
+            "description": "Grants permission to request a transit gateway peering attachment between a requester and accepter transit gateway",
             "orphan": false,
-            "resources": []
+            "resources": [
+                "transit-gateway",
+                "transit-gateway-attachment"
+            ]
         },
         "CreateTransitGatewayPolicyTable": {
-            "access_level": "Undocumented",
+            "access_level": "Write",
             "action": "CreateTransitGatewayPolicyTable",
-            "condition_keys": [],
-            "description": "Not Documented by AWS",
+            "condition_keys": [
+                "aws:RequestTag/${TagKey}",
+                "aws:ResourceTag/${TagKey}",
+                "aws:TagKeys",
+                "ec2:Region",
+                "ec2:ResourceTag/${TagKey}"
+            ],
+            "description": "Grants permission to create a transit gateway policy table",
             "orphan": false,
-            "resources": []
+            "resources": [
+                "transit-gateway",
+                "transit-gateway-policy-table"
+            ]
         },
         "CreateTransitGatewayPrefixListReference": {
-            "access_level": "Undocumented",
+            "access_level": "Write",
             "action": "CreateTransitGatewayPrefixListReference",
-            "condition_keys": [],
-            "description": "Not Documented by AWS",
+            "condition_keys": [
+                "aws:ResourceTag/${TagKey}",
+                "ec2:Region",
+                "ec2:ResourceTag/${TagKey}"
+            ],
+            "description": "Grants permission to create a transit gateway prefix list reference",
             "orphan": false,
-            "resources": []
+            "resources": [
+                "prefix-list",
+                "transit-gateway-attachment",
+                "transit-gateway-route-table"
+            ]
         },
         "CreateTransitGatewayRoute": {
-            "access_level": "Undocumented",
+            "access_level": "Write",
             "action": "CreateTransitGatewayRoute",
-            "condition_keys": [],
-            "description": "Not Documented by AWS",
+            "condition_keys": [
+                "aws:ResourceTag/${TagKey}",
+                "ec2:Region",
+                "ec2:ResourceTag/${TagKey}"
+            ],
+            "description": "Grants permission to create a static route for a transit gateway route table",
             "orphan": false,
-            "resources": []
+            "resources": [
+                "transit-gateway-attachment",
+                "transit-gateway-route-table"
+            ]
         },
         "CreateTransitGatewayRouteTable": {
-            "access_level": "Undocumented",
+            "access_level": "Write",
             "action": "CreateTransitGatewayRouteTable",
-            "condition_keys": [],
-            "description": "Not Documented by AWS",
+            "condition_keys": [
+                "aws:RequestTag/${TagKey}",
+                "aws:ResourceTag/${TagKey}",
+                "aws:TagKeys",
+                "ec2:Region",
+                "ec2:ResourceTag/${TagKey}"
+            ],
+            "description": "Grants permission to create a route table for a transit gateway",
             "orphan": false,
-            "resources": []
+            "resources": [
+                "transit-gateway",
+                "transit-gateway-route-table"
+            ]
         },
         "CreateTransitGatewayRouteTableAnnouncement": {
-            "access_level": "Undocumented",
+            "access_level": "Write",
             "action": "CreateTransitGatewayRouteTableAnnouncement",
-            "condition_keys": [],
-            "description": "Not Documented by AWS",
+            "condition_keys": [
+                "aws:RequestTag/${TagKey}",
+                "aws:ResourceTag/${TagKey}",
+                "aws:TagKeys",
+                "ec2:Region",
+                "ec2:ResourceTag/${TagKey}"
+            ],
+            "description": "Grants permission to create an announcement for a transit gateway route table",
             "orphan": false,
-            "resources": []
+            "resources": [
+                "transit-gateway-attachment",
+                "transit-gateway-route-table",
+                "transit-gateway-route-table-announcement"
+            ]
         },
         "CreateTransitGatewayVpcAttachment": {
-            "access_level": "Undocumented",
+            "access_level": "Write",
             "action": "CreateTransitGatewayVpcAttachment",
-            "condition_keys": [],
-            "description": "Not Documented by AWS",
+            "condition_keys": [
+                "aws:RequestTag/${TagKey}",
+                "aws:ResourceTag/${TagKey}",
+                "aws:TagKeys",
+                "ec2:AvailabilityZone",
+                "ec2:Region",
+                "ec2:ResourceTag/${TagKey}",
+                "ec2:SubnetID",
+                "ec2:Tenancy",
+                "ec2:Vpc",
+                "ec2:VpcID"
+            ],
+            "description": "Grants permission to attach a VPC to a transit gateway",
             "orphan": false,
-            "resources": []
+            "resources": [
+                "subnet",
+                "transit-gateway",
+                "transit-gateway-attachment",
+                "vpc"
+            ]
         },
         "CreateVerifiedAccessEndpoint": {
-            "access_level": "Undocumented",
+            "access_level": "Write",
             "action": "CreateVerifiedAccessEndpoint",
-            "condition_keys": [],
-            "description": "Not Documented by AWS",
-            "orphan": false,
-            "resources": []
+            "condition_keys": [
+                "aws:RequestTag/${TagKey}",
+                "aws:ResourceTag/${TagKey}",
+                "aws:TagKeys",
+                "ec2:AuthorizedUser",
+                "ec2:AvailabilityZone",
+                "ec2:NetworkInterfaceID",
+                "ec2:Permission",
+                "ec2:Region",
+                "ec2:ResourceTag/${TagKey}",
+                "ec2:SecurityGroupID",
+                "ec2:Subnet",
+                "ec2:SubnetID",
+                "ec2:Vpc"
+            ],
+            "description": "Grants permission to create a Verified Access endpoint",
+            "orphan": false,
+            "resources": [
+                "network-interface",
+                "security-group",
+                "subnet",
+                "verified-access-endpoint",
+                "verified-access-group"
+            ]
         },
         "CreateVerifiedAccessGroup": {
-            "access_level": "Undocumented",
+            "access_level": "Write",
             "action": "CreateVerifiedAccessGroup",
-            "condition_keys": [],
-            "description": "Not Documented by AWS",
+            "condition_keys": [
+                "aws:RequestTag/${TagKey}",
+                "aws:ResourceTag/${TagKey}",
+                "aws:TagKeys",
+                "ec2:Region",
+                "ec2:ResourceTag/${TagKey}"
+            ],
+            "description": "Grants permission to create a Verified Access group",
             "orphan": false,
-            "resources": []
+            "resources": [
+                "verified-access-group",
+                "verified-access-instance"
+            ]
         },
         "CreateVerifiedAccessInstance": {
-            "access_level": "Undocumented",
+            "access_level": "Write",
             "action": "CreateVerifiedAccessInstance",
-            "condition_keys": [],
-            "description": "Not Documented by AWS",
+            "condition_keys": [
+                "aws:RequestTag/${TagKey}",
+                "aws:TagKeys",
+                "ec2:Region"
+            ],
+            "description": "Grants permission to create a Verified Access instance",
             "orphan": false,
-            "resources": []
+            "resources": [
+                "verified-access-instance"
+            ]
         },
         "CreateVerifiedAccessTrustProvider": {
-            "access_level": "Undocumented",
+            "access_level": "Write",
             "action": "CreateVerifiedAccessTrustProvider",
-            "condition_keys": [],
-            "description": "Not Documented by AWS",
+            "condition_keys": [
+                "aws:RequestTag/${TagKey}",
+                "aws:TagKeys",
+                "ec2:Region"
+            ],
+            "description": "Grants permission to create a verified trust provider",
             "orphan": false,
-            "resources": []
+            "resources": [
+                "verified-access-trust-provider"
+            ]
         },
         "CreateVolume": {
-            "access_level": "Undocumented",
+            "access_level": "Write",
             "action": "CreateVolume",
-            "condition_keys": [],
-            "description": "Not Documented by AWS",
+            "condition_keys": [
+                "aws:RequestTag/${TagKey}",
+                "aws:TagKeys",
+                "ec2:AvailabilityZone",
+                "ec2:Encrypted",
+                "ec2:KmsKeyId",
+                "ec2:ParentSnapshot",
+                "ec2:Region",
+                "ec2:VolumeID",
+                "ec2:VolumeIops",
+                "ec2:VolumeSize",
+                "ec2:VolumeThroughput",
+                "ec2:VolumeType"
+            ],
+            "description": "Grants permission to create an EBS volume",
             "orphan": false,
-            "resources": []
+            "resources": [
+                "volume"
+            ]
         },
         "CreateVpc": {
-            "access_level": "Undocumented",
+            "access_level": "Write",
             "action": "CreateVpc",
-            "condition_keys": [],
-            "description": "Not Documented by AWS",
+            "condition_keys": [
+                "aws:RequestTag/${TagKey}",
+                "aws:ResourceTag/${TagKey}",
+                "aws:TagKeys",
+                "ec2:Ipv4IpamPoolId",
+                "ec2:Ipv6IpamPoolId",
+                "ec2:Region",
+                "ec2:ResourceTag/${TagKey}",
+                "ec2:VpcID"
+            ],
+            "description": "Grants permission to create a VPC with a specified CIDR block",
             "orphan": false,
-            "resources": []
+            "resources": [
+                "ipam-pool",
+                "ipv6pool-ec2",
+                "vpc"
+            ]
         },
         "CreateVpcEndpoint": {
-            "access_level": "Undocumented",
+            "access_level": "Write",
             "action": "CreateVpcEndpoint",
-            "condition_keys": [],
-            "description": "Not Documented by AWS",
-            "orphan": false,
-            "resources": []
+            "condition_keys": [
+                "aws:RequestTag/${TagKey}",
+                "aws:ResourceTag/${TagKey}",
+                "aws:TagKeys",
+                "ec2:Region",
+                "ec2:ResourceTag/${TagKey}",
+                "ec2:RouteTableID",
+                "ec2:SecurityGroupID",
+                "ec2:SubnetID",
+                "ec2:VpcID",
+                "ec2:VpceServiceName",
+                "ec2:VpceServiceOwner"
+            ],
+            "description": "Grants permission to create a VPC endpoint for an AWS service",
+            "orphan": false,
+            "resources": [
+                "route-table",
+                "security-group",
+                "subnet",
+                "vpc",
+                "vpc-endpoint"
+            ]
         },
         "CreateVpcEndpointConnectionNotification": {
-            "access_level": "Undocumented",
+            "access_level": "Write",
             "action": "CreateVpcEndpointConnectionNotification",
-            "condition_keys": [],
-            "description": "Not Documented by AWS",
+            "condition_keys": [
+                "aws:ResourceTag/${TagKey}",
+                "ec2:Region",
+                "ec2:ResourceTag/${TagKey}"
+            ],
+            "description": "Grants permission to create a connection notification for a VPC endpoint or VPC endpoint service",
             "orphan": false,
-            "resources": []
+            "resources": [
+                "vpc-endpoint",
+                "vpc-endpoint-service"
+            ]
         },
         "CreateVpcEndpointServiceConfiguration": {
-            "access_level": "Undocumented",
+            "access_level": "Write",
             "action": "CreateVpcEndpointServiceConfiguration",
-            "condition_keys": [],
-            "description": "Not Documented by AWS",
+            "condition_keys": [
+                "aws:RequestTag/${TagKey}",
+                "aws:TagKeys",
+                "ec2:Region",
+                "ec2:VpceServicePrivateDnsName"
+            ],
+            "description": "Grants permission to create a VPC endpoint service configuration to which service consumers (AWS accounts, IAM users, and IAM roles) can connect",
             "orphan": false,
-            "resources": []
+            "resources": [
+                "vpc-endpoint-service"
+            ]
         },
         "CreateVpcPeeringConnection": {
-            "access_level": "Undocumented",
+            "access_level": "Write",
             "action": "CreateVpcPeeringConnection",
-            "condition_keys": [],
-            "description": "Not Documented by AWS",
+            "condition_keys": [
+                "aws:RequestTag/${TagKey}",
+                "aws:ResourceTag/${TagKey}",
+                "aws:TagKeys",
+                "ec2:AccepterVpc",
+                "ec2:Region",
+                "ec2:RequesterVpc",
+                "ec2:ResourceTag/${TagKey}",
+                "ec2:Tenancy",
+                "ec2:VpcID",
+                "ec2:VpcPeeringConnectionID"
+            ],
+            "description": "Grants permission to request a VPC peering connection between two VPCs",
             "orphan": false,
-            "resources": []
+            "resources": [
+                "vpc",
+                "vpc-peering-connection"
+            ]
         },
         "CreateVpnConnection": {
-            "access_level": "Undocumented",
+            "access_level": "Write",
             "action": "CreateVpnConnection",
-            "condition_keys": [],
-            "description": "Not Documented by AWS",
-            "orphan": false,
-            "resources": []
+            "condition_keys": [
+                "aws:RequestTag/${TagKey}",
+                "aws:ResourceTag/${TagKey}",
+                "aws:TagKeys",
+                "ec2:AuthenticationType",
+                "ec2:DPDTimeoutSeconds",
+                "ec2:GatewayType",
+                "ec2:IKEVersions",
+                "ec2:InsideTunnelCidr",
+                "ec2:InsideTunnelIpv6Cidr",
+                "ec2:Phase1DHGroup",
+                "ec2:Phase1EncryptionAlgorithms",
+                "ec2:Phase1IntegrityAlgorithms",
+                "ec2:Phase1LifetimeSeconds",
+                "ec2:Phase2DHGroup",
+                "ec2:Phase2EncryptionAlgorithms",
+                "ec2:Phase2IntegrityAlgorithms",
+                "ec2:Phase2LifetimeSeconds",
+                "ec2:PreSharedKeys",
+                "ec2:Region",
+                "ec2:RekeyFuzzPercentage",
+                "ec2:RekeyMarginTimeSeconds",
+                "ec2:ReplayWindowSizePackets",
+                "ec2:ResourceTag/${TagKey}",
+                "ec2:RoutingType"
+            ],
+            "description": "Grants permission to create a VPN connection between a virtual private gateway or transit gateway and a customer gateway",
+            "orphan": false,
+            "resources": [
+                "customer-gateway",
+                "transit-gateway",
+                "transit-gateway-attachment",
+                "vpn-connection",
+                "vpn-gateway"
+            ]
         },
         "CreateVpnConnectionRoute": {
-            "access_level": "Undocumented",
+            "access_level": "Write",
             "action": "CreateVpnConnectionRoute",
-            "condition_keys": [],
-            "description": "Not Documented by AWS",
+            "condition_keys": [
+                "aws:ResourceTag/${TagKey}",
+                "ec2:Region",
+                "ec2:ResourceTag/${TagKey}"
+            ],
+            "description": "Grants permission to create a static route for a VPN connection between a virtual private gateway and a customer gateway",
             "orphan": false,
-            "resources": []
+            "resources": [
+                "vpn-connection"
+            ]
         },
         "CreateVpnGateway": {
-            "access_level": "Undocumented",
+            "access_level": "Write",
             "action": "CreateVpnGateway",
-            "condition_keys": [],
-            "description": "Not Documented by AWS",
+            "condition_keys": [
+                "aws:RequestTag/${TagKey}",
+                "aws:TagKeys",
+                "ec2:Region"
+            ],
+            "description": "Grants permission to create a virtual private gateway",
             "orphan": false,
-            "resources": []
+            "resources": [
+                "vpn-gateway"
+            ]
         },
         "DeleteCarrierGateway": {
-            "access_level": "Undocumented",
+            "access_level": "Write",
             "action": "DeleteCarrierGateway",
-            "condition_keys": [],
-            "description": "Not Documented by AWS",
+            "condition_keys": [
+                "aws:ResourceTag/${TagKey}",
+                "ec2:Region",
+                "ec2:ResourceTag/${TagKey}"
+            ],
+            "description": "Grants permission to delete a carrier gateway",
             "orphan": false,
-            "resources": []
+            "resources": [
+                "carrier-gateway"
+            ]
         },
         "DeleteClientVpnEndpoint": {
-            "access_level": "Undocumented",
+            "access_level": "Write",
             "action": "DeleteClientVpnEndpoint",
-            "condition_keys": [],
-            "description": "Not Documented by AWS",
+            "condition_keys": [
+                "aws:ResourceTag/${TagKey}",
+                "ec2:ClientRootCertificateChainArn",
+                "ec2:CloudwatchLogGroupArn",
+                "ec2:CloudwatchLogStreamArn",
+                "ec2:DirectoryArn",
+                "ec2:Region",
+                "ec2:ResourceTag/${TagKey}",
+                "ec2:SamlProviderArn",
+                "ec2:ServerCertificateArn"
+            ],
+            "description": "Grants permission to delete a Client VPN endpoint",
             "orphan": false,
-            "resources": []
+            "resources": [
+                "client-vpn-endpoint"
+            ]
         },
         "DeleteClientVpnRoute": {
-            "access_level": "Undocumented",
+            "access_level": "Write",
             "action": "DeleteClientVpnRoute",
-            "condition_keys": [],
-            "description": "Not Documented by AWS",
+            "condition_keys": [
+                "aws:ResourceTag/${TagKey}",
+                "ec2:AvailabilityZone",
+                "ec2:ClientRootCertificateChainArn",
+                "ec2:CloudwatchLogGroupArn",
+                "ec2:CloudwatchLogStreamArn",
+                "ec2:DirectoryArn",
+                "ec2:Region",
+                "ec2:ResourceTag/${TagKey}",
+                "ec2:SamlProviderArn",
+                "ec2:ServerCertificateArn",
+                "ec2:SubnetID",
+                "ec2:Vpc"
+            ],
+            "description": "Grants permission to delete a route from a Client VPN endpoint",
             "orphan": false,
-            "resources": []
+            "resources": [
+                "client-vpn-endpoint",
+                "subnet"
+            ]
         },
         "DeleteCoipCidr": {
-            "access_level": "Undocumented",
+            "access_level": "Write",
             "action": "DeleteCoipCidr",
-            "condition_keys": [],
-            "description": "Not Documented by AWS",
+            "condition_keys": [
+                "aws:ResourceTag/${TagKey}",
+                "ec2:Region",
+                "ec2:ResourceTag/${TagKey}"
+            ],
+            "description": "Grants permission to delete a range of customer-owned IP (CoIP) addresses",
             "orphan": false,
-            "resources": []
+            "resources": [
+                "coip-pool"
+            ]
         },
         "DeleteCoipPool": {
-            "access_level": "Undocumented",
+            "access_level": "Write",
             "action": "DeleteCoipPool",
-            "condition_keys": [],
-            "description": "Not Documented by AWS",
+            "condition_keys": [
+                "aws:ResourceTag/${TagKey}",
+                "ec2:Region",
+                "ec2:ResourceTag/${TagKey}"
+            ],
+            "description": "Grants permission to delete a pool of customer-owned IP (CoIP) addresses",
             "orphan": false,
-            "resources": []
+            "resources": [
+                "coip-pool"
+            ]
         },
         "DeleteCoipPoolPermission": {
-            "access_level": "Undocumented",
+            "access_level": "Write",
             "action": "DeleteCoipPoolPermission",
-            "condition_keys": [],
-            "description": "Not Documented by AWS",
+            "condition_keys": [
+                "aws:ResourceTag/${TagKey}",
+                "ec2:Region",
+                "ec2:ResourceTag/${TagKey}"
+            ],
+            "description": "Grants permission to deny a service from accessing a customer-owned IP (CoIP) pool",
             "orphan": false,
-            "resources": []
+            "resources": [
+                "coip-pool"
+            ]
         },
         "DeleteCustomerGateway": {
-            "access_level": "Undocumented",
+            "access_level": "Write",
             "action": "DeleteCustomerGateway",
-            "condition_keys": [],
-            "description": "Not Documented by AWS",
+            "condition_keys": [
+                "aws:ResourceTag/${TagKey}",
+                "ec2:Region",
+                "ec2:ResourceTag/${TagKey}"
+            ],
+            "description": "Grants permission to delete a customer gateway",
             "orphan": false,
-            "resources": []
+            "resources": [
+                "customer-gateway"
+            ]
         },
         "DeleteDhcpOptions": {
-            "access_level": "Undocumented",
+            "access_level": "Write",
             "action": "DeleteDhcpOptions",
-            "condition_keys": [],
-            "description": "Not Documented by AWS",
+            "condition_keys": [
+                "aws:ResourceTag/${TagKey}",
+                "ec2:DhcpOptionsID",
+                "ec2:Region",
+                "ec2:ResourceTag/${TagKey}"
+            ],
+            "description": "Grants permission to delete a set of DHCP options",
             "orphan": false,
-            "resources": []
+            "resources": [
+                "dhcp-options"
+            ]
         },
         "DeleteEgressOnlyInternetGateway": {
-            "access_level": "Undocumented",
+            "access_level": "Write",
             "action": "DeleteEgressOnlyInternetGateway",
-            "condition_keys": [],
-            "description": "Not Documented by AWS",
+            "condition_keys": [
+                "aws:ResourceTag/${TagKey}",
+                "ec2:Region",
+                "ec2:ResourceTag/${TagKey}"
+            ],
+            "description": "Grants permission to delete an egress-only internet gateway",
             "orphan": false,
-            "resources": []
+            "resources": [
+                "egress-only-internet-gateway"
+            ]
         },
         "DeleteFleets": {
-            "access_level": "Undocumented",
+            "access_level": "Write",
             "action": "DeleteFleets",
-            "condition_keys": [],
-            "description": "Not Documented by AWS",
+            "condition_keys": [
+                "aws:ResourceTag/${TagKey}",
+                "ec2:Region",
+                "ec2:ResourceTag/${TagKey}"
+            ],
+            "description": "Grants permission to delete one or more EC2 Fleets",
             "orphan": false,
-            "resources": []
+            "resources": [
+                "fleet"
+            ]
         },
         "DeleteFlowLogs": {
-            "access_level": "Undocumented",
+            "access_level": "Write",
             "action": "DeleteFlowLogs",
-            "condition_keys": [],
-            "description": "Not Documented by AWS",
+            "condition_keys": [
+                "aws:ResourceTag/${TagKey}",
+                "ec2:Region",
+                "ec2:ResourceTag/${TagKey}"
+            ],
+            "description": "Grants permission to delete one or more flow logs",
             "orphan": false,
-            "resources": []
+            "resources": [
+                "vpc-flow-log"
+            ]
         },
         "DeleteFpgaImage": {
-            "access_level": "Undocumented",
+            "access_level": "Write",
             "action": "DeleteFpgaImage",
-            "condition_keys": [],
-            "description": "Not Documented by AWS",
+            "condition_keys": [
+                "aws:ResourceTag/${TagKey}",
+                "ec2:Owner",
+                "ec2:Public",
+                "ec2:Region",
+                "ec2:ResourceTag/${TagKey}"
+            ],
+            "description": "Grants permission to delete an Amazon FPGA Image (AFI)",
             "orphan": false,
-            "resources": []
+            "resources": [
+                "fpga-image"
+            ]
         },
         "DeleteInstanceEventWindow": {
-            "access_level": "Undocumented",
+            "access_level": "Write",
             "action": "DeleteInstanceEventWindow",
-            "condition_keys": [],
-            "description": "Not Documented by AWS",
+            "condition_keys": [
+                "aws:ResourceTag/${TagKey}",
+                "ec2:Region",
+                "ec2:ResourceTag/${TagKey}"
+            ],
+            "description": "Grants permission to delete the specified event window",
             "orphan": false,
-            "resources": []
+            "resources": [
+                "instance-event-window"
+            ]
         },
         "DeleteInternetGateway": {
-            "access_level": "Undocumented",
+            "access_level": "Write",
             "action": "DeleteInternetGateway",
-            "condition_keys": [],
-            "description": "Not Documented by AWS",
+            "condition_keys": [
+                "aws:ResourceTag/${TagKey}",
+                "ec2:InternetGatewayID",
+                "ec2:Region",
+                "ec2:ResourceTag/${TagKey}"
+            ],
+            "description": "Grants permission to delete an internet gateway",
             "orphan": false,
-            "resources": []
+            "resources": [
+                "internet-gateway"
+            ]
         },
         "DeleteIpam": {
-            "access_level": "Undocumented",
+            "access_level": "Write",
             "action": "DeleteIpam",
-            "condition_keys": [],
-            "description": "Not Documented by AWS",
+            "condition_keys": [
+                "aws:ResourceTag/${TagKey}",
+                "ec2:Region",
+                "ec2:ResourceTag/${TagKey}"
+            ],
+            "description": "Grants permission to delete an Amazon VPC IP Address Manager (IPAM) and remove all monitored data associated with the IPAM including the historical data for CIDRs",
             "orphan": false,
-            "resources": []
+            "resources": [
+                "ipam"
+            ]
         },
         "DeleteIpamPool": {
-            "access_level": "Undocumented",
+            "access_level": "Write",
             "action": "DeleteIpamPool",
-            "condition_keys": [],
-            "description": "Not Documented by AWS",
+            "condition_keys": [
+                "aws:ResourceTag/${TagKey}",
+                "ec2:Region",
+                "ec2:ResourceTag/${TagKey}"
+            ],
+            "description": "Grants permission to delete an Amazon VPC IP Address Manager (IPAM) pool",
             "orphan": false,
-            "resources": []
+            "resources": [
+                "ipam-pool"
+            ]
         },
         "DeleteIpamResourceDiscovery": {
-            "access_level": "Undocumented",
+            "access_level": "Write",
             "action": "DeleteIpamResourceDiscovery",
-            "condition_keys": [],
-            "description": "Not Documented by AWS",
+            "condition_keys": [
+                "aws:ResourceTag/${TagKey}",
+                "ec2:Region",
+                "ec2:ResourceTag/${TagKey}"
+            ],
+            "description": "Grants permission to delete an IPAM resource discovery",
             "orphan": false,
-            "resources": []
+            "resources": [
+                "ipam-resource-discovery"
+            ]
         },
         "DeleteIpamScope": {
-            "access_level": "Undocumented",
+            "access_level": "Write",
             "action": "DeleteIpamScope",
-            "condition_keys": [],
-            "description": "Not Documented by AWS",
+            "condition_keys": [
+                "aws:ResourceTag/${TagKey}",
+                "ec2:Region",
+                "ec2:ResourceTag/${TagKey}"
+            ],
+            "description": "Grants permission to delete the scope for an Amazon VPC IP Address Manager (IPAM)",
             "orphan": false,
-            "resources": []
+            "resources": [
+                "ipam-scope"
+            ]
         },
         "DeleteKeyPair": {
-            "access_level": "Undocumented",
+            "access_level": "Write",
             "action": "DeleteKeyPair",
-            "condition_keys": [],
-            "description": "Not Documented by AWS",
+            "condition_keys": [
+                "aws:ResourceTag/${TagKey}",
+                "ec2:KeyPairName",
+                "ec2:KeyPairType",
+                "ec2:Region",
+                "ec2:ResourceTag/${TagKey}"
+            ],
+            "description": "Grants permission to delete a key pair by removing the public key from Amazon EC2",
             "orphan": false,
-            "resources": []
+            "resources": [
+                "key-pair"
+            ]
         },
         "DeleteLaunchTemplate": {
-            "access_level": "Undocumented",
+            "access_level": "Write",
             "action": "DeleteLaunchTemplate",
-            "condition_keys": [],
-            "description": "Not Documented by AWS",
+            "condition_keys": [
+                "aws:ResourceTag/${TagKey}",
+                "ec2:Region",
+                "ec2:ResourceTag/${TagKey}"
+            ],
+            "description": "Grants permission to delete a launch template and its associated versions",
             "orphan": false,
-            "resources": []
+            "resources": [
+                "launch-template"
+            ]
         },
         "DeleteLaunchTemplateVersions": {
-            "access_level": "Undocumented",
+            "access_level": "Write",
             "action": "DeleteLaunchTemplateVersions",
-            "condition_keys": [],
-            "description": "Not Documented by AWS",
+            "condition_keys": [
+                "aws:ResourceTag/${TagKey}",
+                "ec2:Region",
+                "ec2:ResourceTag/${TagKey}"
+            ],
+            "description": "Grants permission to delete one or more versions of a launch template",
             "orphan": false,
-            "resources": []
+            "resources": [
+                "launch-template"
+            ]
         },
         "DeleteLocalGatewayRoute": {
-            "access_level": "Undocumented",
+            "access_level": "Write",
             "action": "DeleteLocalGatewayRoute",
-            "condition_keys": [],
-            "description": "Not Documented by AWS",
+            "condition_keys": [
+                "aws:ResourceTag/${TagKey}",
+                "ec2:Region",
+                "ec2:ResourceTag/${TagKey}"
+            ],
+            "description": "Grants permission to delete a route from a local gateway route table",
             "orphan": false,
-            "resources": []
+            "resources": [
+                "local-gateway-route-table",
+                "prefix-list"
+            ]
         },
         "DeleteLocalGatewayRouteTable": {
-            "access_level": "Undocumented",
+            "access_level": "Write",
             "action": "DeleteLocalGatewayRouteTable",
-            "condition_keys": [],
-            "description": "Not Documented by AWS",
+            "condition_keys": [
+                "aws:ResourceTag/${TagKey}",
+                "ec2:Region",
+                "ec2:ResourceTag/${TagKey}"
+            ],
+            "description": "Grants permission to delete a local gateway route table",
             "orphan": false,
-            "resources": []
+            "resources": [
+                "local-gateway-route-table"
+            ]
         },
         "DeleteLocalGatewayRouteTablePermission": {
-            "access_level": "Undocumented",
+            "access_level": "Write",
             "action": "DeleteLocalGatewayRouteTablePermission",
-            "condition_keys": [],
-            "description": "Not Documented by AWS",
+            "condition_keys": [
+                "aws:ResourceTag/${TagKey}",
+                "ec2:Region",
+                "ec2:ResourceTag/${TagKey}"
+            ],
+            "description": "Grants permission to deny a service from accessing a local gateway route table",
             "orphan": false,
-            "resources": []
+            "resources": [
+                "local-gateway-route-table"
+            ]
         },
         "DeleteLocalGatewayRouteTableVirtualInterfaceGroupAssociation": {
-            "access_level": "Undocumented",
+            "access_level": "Write",
             "action": "DeleteLocalGatewayRouteTableVirtualInterfaceGroupAssociation",
-            "condition_keys": [],
-            "description": "Not Documented by AWS",
+            "condition_keys": [
+                "aws:ResourceTag/${TagKey}",
+                "ec2:Region",
+                "ec2:ResourceTag/${TagKey}"
+            ],
+            "description": "Grants permission to delete a local gateway route table virtual interface group association",
             "orphan": false,
-            "resources": []
+            "resources": [
+                "local-gateway-route-table-virtual-interface-group-association"
+            ]
         },
         "DeleteLocalGatewayRouteTableVpcAssociation": {
-            "access_level": "Undocumented",
+            "access_level": "Write",
             "action": "DeleteLocalGatewayRouteTableVpcAssociation",
-            "condition_keys": [],
-            "description": "Not Documented by AWS",
+            "condition_keys": [
+                "aws:ResourceTag/${TagKey}",
+                "ec2:Region",
+                "ec2:ResourceTag/${TagKey}"
+            ],
+            "description": "Grants permission to delete an association between a VPC and local gateway route table",
             "orphan": false,
-            "resources": []
+            "resources": [
+                "local-gateway-route-table-vpc-association"
+            ]
         },
         "DeleteManagedPrefixList": {
-            "access_level": "Undocumented",
+            "access_level": "Write",
             "action": "DeleteManagedPrefixList",
-            "condition_keys": [],
-            "description": "Not Documented by AWS",
+            "condition_keys": [
+                "aws:ResourceTag/${TagKey}",
+                "ec2:Region",
+                "ec2:ResourceTag/${TagKey}"
+            ],
+            "description": "Grants permission to delete a managed prefix list",
             "orphan": false,
-            "resources": []
+            "resources": [
+                "prefix-list"
+            ]
         },
         "DeleteNatGateway": {
-            "access_level": "Undocumented",
+            "access_level": "Write",
             "action": "DeleteNatGateway",
-            "condition_keys": [],
-            "description": "Not Documented by AWS",
+            "condition_keys": [
+                "aws:ResourceTag/${TagKey}",
+                "ec2:Region",
+                "ec2:ResourceTag/${TagKey}"
+            ],
+            "description": "Grants permission to delete a NAT gateway",
             "orphan": false,
-            "resources": []
+            "resources": [
+                "natgateway"
+            ]
         },
         "DeleteNetworkAcl": {
-            "access_level": "Undocumented",
+            "access_level": "Write",
             "action": "DeleteNetworkAcl",
-            "condition_keys": [],
-            "description": "Not Documented by AWS",
+            "condition_keys": [
+                "aws:ResourceTag/${TagKey}",
+                "ec2:NetworkAclID",
+                "ec2:Region",
+                "ec2:ResourceTag/${TagKey}",
+                "ec2:Vpc"
+            ],
+            "description": "Grants permission to delete a network ACL",
             "orphan": false,
-            "resources": []
+            "resources": [
+                "network-acl"
+            ]
         },
         "DeleteNetworkAclEntry": {
-            "access_level": "Undocumented",
+            "access_level": "Write",
             "action": "DeleteNetworkAclEntry",
-            "condition_keys": [],
-            "description": "Not Documented by AWS",
+            "condition_keys": [
+                "aws:ResourceTag/${TagKey}",
+                "ec2:NetworkAclID",
+                "ec2:Region",
+                "ec2:ResourceTag/${TagKey}",
+                "ec2:Vpc"
+            ],
+            "description": "Grants permission to delete an inbound or outbound entry (rule) from a network ACL",
             "orphan": false,
-            "resources": []
+            "resources": [
+                "network-acl"
+            ]
         },
         "DeleteNetworkInsightsAccessScope": {
-            "access_level": "Undocumented",
+            "access_level": "Write",
             "action": "DeleteNetworkInsightsAccessScope",
-            "condition_keys": [],
-            "description": "Not Documented by AWS",
+            "condition_keys": [
+                "aws:ResourceTag/${TagKey}",
+                "ec2:Region",
+                "ec2:ResourceTag/${TagKey}"
+            ],
+            "description": "Grants permission to delete a Network Access Scope",
             "orphan": false,
-            "resources": []
+            "resources": [
+                "network-insights-access-scope"
+            ]
         },
         "DeleteNetworkInsightsAccessScopeAnalysis": {
-            "access_level": "Undocumented",
+            "access_level": "Write",
             "action": "DeleteNetworkInsightsAccessScopeAnalysis",
-            "condition_keys": [],
-            "description": "Not Documented by AWS",
+            "condition_keys": [
+                "aws:ResourceTag/${TagKey}",
+                "ec2:Region",
+                "ec2:ResourceTag/${TagKey}"
+            ],
+            "description": "Grants permission to delete a Network Access Scope analysis",
             "orphan": false,
-            "resources": []
+            "resources": [
+                "network-insights-access-scope-analysis"
+            ]
         },
         "DeleteNetworkInsightsAnalysis": {
-            "access_level": "Undocumented",
+            "access_level": "Write",
             "action": "DeleteNetworkInsightsAnalysis",
-            "condition_keys": [],
-            "description": "Not Documented by AWS",
+            "condition_keys": [
+                "aws:ResourceTag/${TagKey}",
+                "ec2:Region",
+                "ec2:ResourceTag/${TagKey}"
+            ],
+            "description": "Grants permission to delete a network insights analysis",
             "orphan": false,
-            "resources": []
+            "resources": [
+                "network-insights-analysis"
+            ]
         },
         "DeleteNetworkInsightsPath": {
-            "access_level": "Undocumented",
+            "access_level": "Write",
             "action": "DeleteNetworkInsightsPath",
-            "condition_keys": [],
-            "description": "Not Documented by AWS",
+            "condition_keys": [
+                "aws:ResourceTag/${TagKey}",
+                "ec2:Region",
+                "ec2:ResourceTag/${TagKey}"
+            ],
+            "description": "Grants permission to delete a network insights path",
             "orphan": false,
-            "resources": []
+            "resources": [
+                "network-insights-path"
+            ]
         },
         "DeleteNetworkInterface": {
-            "access_level": "Undocumented",
+            "access_level": "Write",
             "action": "DeleteNetworkInterface",
-            "condition_keys": [],
-            "description": "Not Documented by AWS",
+            "condition_keys": [
+                "aws:ResourceTag/${TagKey}",
+                "ec2:AvailabilityZone",
+                "ec2:NetworkInterfaceID",
+                "ec2:Region",
+                "ec2:ResourceTag/${TagKey}",
+                "ec2:Subnet",
+                "ec2:Vpc"
+            ],
+            "description": "Grants permission to delete a detached network interface",
             "orphan": false,
-            "resources": []
+            "resources": [
+                "network-interface"
+            ]
         },
         "DeleteNetworkInterfacePermission": {
-            "access_level": "Undocumented",
+            "access_level": "Permissions management",
             "action": "DeleteNetworkInterfacePermission",
-            "condition_keys": [],
-            "description": "Not Documented by AWS",
+            "condition_keys": [
+                "aws:ResourceTag/${TagKey}",
+                "ec2:AvailabilityZone",
+                "ec2:NetworkInterfaceID",
+                "ec2:Region",
+                "ec2:ResourceTag/${TagKey}",
+                "ec2:Subnet",
+                "ec2:Vpc"
+            ],
+            "description": "Grants permission to delete a permission that is associated with a network interface",
             "orphan": false,
-            "resources": []
+            "resources": [
+                "network-interface"
+            ]
         },
         "DeletePlacementGroup": {
-            "access_level": "Undocumented",
+            "access_level": "Write",
             "action": "DeletePlacementGroup",
-            "condition_keys": [],
-            "description": "Not Documented by AWS",
+            "condition_keys": [
+                "aws:ResourceTag/${TagKey}",
+                "ec2:PlacementGroupName",
+                "ec2:PlacementGroupStrategy",
+                "ec2:Region",
+                "ec2:ResourceTag/${TagKey}"
+            ],
+            "description": "Grants permission to delete a placement group",
             "orphan": false,
-            "resources": []
+            "resources": [
+                "placement-group"
+            ]
         },
         "DeletePublicIpv4Pool": {
-            "access_level": "Undocumented",
+            "access_level": "Write",
             "action": "DeletePublicIpv4Pool",
-            "condition_keys": [],
-            "description": "Not Documented by AWS",
+            "condition_keys": [
+                "aws:ResourceTag/${TagKey}",
+                "ec2:Region",
+                "ec2:ResourceTag/${TagKey}"
+            ],
+            "description": "Grants permission to delete a public IPv4 address pool for public IPv4 CIDRs that you own and brought to Amazon to manage with Amazon VPC IP Address Manager (IPAM)",
             "orphan": false,
-            "resources": []
+            "resources": [
+                "ipv4pool-ec2"
+            ]
         },
         "DeleteQueuedReservedInstances": {
-            "access_level": "Undocumented",
+            "access_level": "Write",
             "action": "DeleteQueuedReservedInstances",
-            "condition_keys": [],
-            "description": "Not Documented by AWS",
+            "condition_keys": [
+                "ec2:Region"
+            ],
+            "description": "Grants permission to delete the queued purchases for the specified Reserved Instances",
             "orphan": false,
             "resources": []
         },
         "DeleteResourcePolicy": {
-            "access_level": "Undocumented",
+            "access_level": "Write",
             "action": "DeleteResourcePolicy",
-            "condition_keys": [],
-            "description": "Not Documented by AWS",
+            "condition_keys": [
+                "aws:ResourceTag/${TagKey}",
+                "ec2:PlacementGroupName",
+                "ec2:PlacementGroupStrategy",
+                "ec2:Region",
+                "ec2:ResourceTag/${TagKey}"
+            ],
+            "description": "Grants permission to remove an IAM policy that enables cross-account sharing from a resource",
             "orphan": false,
-            "resources": []
+            "resources": [
+                "ipam-pool",
+                "placement-group",
+                "verified-access-group"
+            ]
         },
         "DeleteRoute": {
-            "access_level": "Undocumented",
+            "access_level": "Write",
             "action": "DeleteRoute",
-            "condition_keys": [],
-            "description": "Not Documented by AWS",
+            "condition_keys": [
+                "aws:ResourceTag/${TagKey}",
+                "ec2:Region",
+                "ec2:ResourceTag/${TagKey}",
+                "ec2:RouteTableID",
+                "ec2:Vpc"
+            ],
+            "description": "Grants permission to delete a route from a route table",
             "orphan": false,
-            "resources": []
+            "resources": [
+                "route-table"
+            ]
         },
         "DeleteRouteTable": {
-            "access_level": "Undocumented",
+            "access_level": "Write",
             "action": "DeleteRouteTable",
-            "condition_keys": [],
-            "description": "Not Documented by AWS",
+            "condition_keys": [
+                "aws:ResourceTag/${TagKey}",
+                "ec2:Region",
+                "ec2:ResourceTag/${TagKey}",
+                "ec2:RouteTableID",
+                "ec2:Vpc"
+            ],
+            "description": "Grants permission to delete a route table",
             "orphan": false,
-            "resources": []
+            "resources": [
+                "route-table"
+            ]
         },
         "DeleteSecurityGroup": {
-            "access_level": "Undocumented",
+            "access_level": "Write",
             "action": "DeleteSecurityGroup",
-            "condition_keys": [],
-            "description": "Not Documented by AWS",
+            "condition_keys": [
+                "aws:ResourceTag/${TagKey}",
+                "ec2:Region",
+                "ec2:ResourceTag/${TagKey}",
+                "ec2:SecurityGroupID",
+                "ec2:Vpc"
+            ],
+            "description": "Grants permission to delete a security group",
             "orphan": false,
-            "resources": []
+            "resources": [
+                "security-group"
+            ]
         },
         "DeleteSnapshot": {
-            "access_level": "Undocumented",
+            "access_level": "Write",
             "action": "DeleteSnapshot",
-            "condition_keys": [],
-            "description": "Not Documented by AWS",
+            "condition_keys": [
+                "aws:ResourceTag/${TagKey}",
+                "ec2:OutpostArn",
+                "ec2:Owner",
+                "ec2:ParentVolume",
+                "ec2:Region",
+                "ec2:ResourceTag/${TagKey}",
+                "ec2:SnapshotID",
+                "ec2:SnapshotTime",
+                "ec2:VolumeSize"
+            ],
+            "description": "Grants permission to delete a snapshot of an EBS volume",
             "orphan": false,
-            "resources": []
+            "resources": [
+                "snapshot"
+            ]
         },
         "DeleteSpotDatafeedSubscription": {
-            "access_level": "Undocumented",
+            "access_level": "Write",
             "action": "DeleteSpotDatafeedSubscription",
-            "condition_keys": [],
-            "description": "Not Documented by AWS",
+            "condition_keys": [
+                "ec2:Region"
+            ],
+            "description": "Grants permission to delete a data feed for Spot Instances",
             "orphan": false,
             "resources": []
         },
         "DeleteSubnet": {
-            "access_level": "Undocumented",
+            "access_level": "Write",
             "action": "DeleteSubnet",
-            "condition_keys": [],
-            "description": "Not Documented by AWS",
+            "condition_keys": [
+                "aws:ResourceTag/${TagKey}",
+                "ec2:AvailabilityZone",
+                "ec2:Region",
+                "ec2:ResourceTag/${TagKey}",
+                "ec2:SubnetID",
+                "ec2:Vpc"
+            ],
+            "description": "Grants permission to delete a subnet",
             "orphan": false,
-            "resources": []
+            "resources": [
+                "subnet"
+            ]
         },
         "DeleteSubnetCidrReservation": {
-            "access_level": "Undocumented",
+            "access_level": "Write",
             "action": "DeleteSubnetCidrReservation",
-            "condition_keys": [],
-            "description": "Not Documented by AWS",
+            "condition_keys": [
+                "ec2:Region"
+            ],
+            "description": "Grants permission to delete a subnet CIDR reservation",
             "orphan": false,
             "resources": []
         },
         "DeleteTags": {
-            "access_level": "Undocumented",
+            "access_level": "Tagging",
             "action": "DeleteTags",
-            "condition_keys": [],
-            "description": "Not Documented by AWS",
+            "condition_keys": [
+                "aws:ResourceTag/${TagKey}",
+                "aws:TagKeys",
+                "ec2:Region",
+                "ec2:ResourceTag/${TagKey}"
+            ],
+            "description": "Grants permission to delete one or more tags from Amazon EC2 resources",
             "orphan": false,
-            "resources": []
+            "resources": [
+                "capacity-reservation",
+                "capacity-reservation-fleet",
+                "carrier-gateway",
+                "client-vpn-endpoint",
+                "coip-pool",
+                "customer-gateway",
+                "dedicated-host",
+                "dhcp-options",
+                "egress-only-internet-gateway",
+                "elastic-gpu",
+                "elastic-ip",
+                "export-image-task",
+                "export-instance-task",
+                "fleet",
+                "fpga-image",
+                "host-reservation",
+                "image",
+                "import-image-task",
+                "import-snapshot-task",
+                "instance",
+                "instance-event-window",
+                "internet-gateway",
+                "ipam",
+                "ipam-pool",
+                "ipam-resource-discovery",
+                "ipam-resource-discovery-association",
+                "ipam-scope",
+                "ipv4pool-ec2",
+                "ipv6pool-ec2",
+                "key-pair",
+                "launch-template",
+                "local-gateway",
+                "local-gateway-route-table",
+                "local-gateway-route-table-virtual-interface-group-association",
+                "local-gateway-route-table-vpc-association",
+                "local-gateway-virtual-interface",
+                "local-gateway-virtual-interface-group",
+                "natgateway",
+                "network-acl",
+                "network-insights-access-scope",
+                "network-insights-access-scope-analysis",
+                "network-insights-analysis",
+                "network-insights-path",
+                "network-interface",
+                "placement-group",
+                "prefix-list",
+                "replace-root-volume-task",
+                "reserved-instances",
+                "route-table",
+                "security-group",
+                "security-group-rule",
+                "snapshot",
+                "spot-fleet-request",
+                "spot-instances-request",
+                "subnet",
+                "subnet-cidr-reservation",
+                "traffic-mirror-filter",
+                "traffic-mirror-session",
+                "traffic-mirror-target",
+                "transit-gateway",
+                "transit-gateway-attachment",
+                "transit-gateway-connect-peer",
+                "transit-gateway-multicast-domain",
+                "transit-gateway-policy-table",
+                "transit-gateway-route-table",
+                "transit-gateway-route-table-announcement",
+                "verified-access-endpoint",
+                "verified-access-group",
+                "verified-access-instance",
+                "verified-access-policy",
+                "verified-access-trust-provider",
+                "volume",
+                "vpc",
+                "vpc-endpoint",
+                "vpc-endpoint-connection",
+                "vpc-endpoint-service",
+                "vpc-endpoint-service-permission",
+                "vpc-flow-log",
+                "vpc-peering-connection",
+                "vpn-connection",
+                "vpn-gateway"
+            ]
         },
         "DeleteTrafficMirrorFilter": {
-            "access_level": "Undocumented",
+            "access_level": "Write",
             "action": "DeleteTrafficMirrorFilter",
-            "condition_keys": [],
-            "description": "Not Documented by AWS",
+            "condition_keys": [
+                "aws:ResourceTag/${TagKey}",
+                "ec2:Region",
+                "ec2:ResourceTag/${TagKey}"
+            ],
+            "description": "Grants permission to delete a traffic mirror filter",
             "orphan": false,
-            "resources": []
+            "resources": [
+                "traffic-mirror-filter"
+            ]
         },
         "DeleteTrafficMirrorFilterRule": {
-            "access_level": "Undocumented",
+            "access_level": "Write",
             "action": "DeleteTrafficMirrorFilterRule",
-            "condition_keys": [],
-            "description": "Not Documented by AWS",
+            "condition_keys": [
+                "aws:ResourceTag/${TagKey}",
+                "ec2:Region",
+                "ec2:ResourceTag/${TagKey}"
+            ],
+            "description": "Grants permission to delete a traffic mirror filter rule",
             "orphan": false,
-            "resources": []
+            "resources": [
+                "traffic-mirror-filter",
+                "traffic-mirror-filter-rule"
+            ]
         },
         "DeleteTrafficMirrorSession": {
-            "access_level": "Undocumented",
+            "access_level": "Write",
             "action": "DeleteTrafficMirrorSession",
-            "condition_keys": [],
-            "description": "Not Documented by AWS",
+            "condition_keys": [
+                "aws:ResourceTag/${TagKey}",
+                "ec2:Region",
+                "ec2:ResourceTag/${TagKey}"
+            ],
+            "description": "Grants permission to delete a traffic mirror session",
             "orphan": false,
-            "resources": []
+            "resources": [
+                "traffic-mirror-session"
+            ]
         },
         "DeleteTrafficMirrorTarget": {
-            "access_level": "Undocumented",
+            "access_level": "Write",
             "action": "DeleteTrafficMirrorTarget",
-            "condition_keys": [],
-            "description": "Not Documented by AWS",
+            "condition_keys": [
+                "aws:ResourceTag/${TagKey}",
+                "ec2:Region",
+                "ec2:ResourceTag/${TagKey}"
+            ],
+            "description": "Grants permission to delete a traffic mirror target",
             "orphan": false,
-            "resources": []
+            "resources": [
+                "traffic-mirror-target"
+            ]
         },
         "DeleteTransitGateway": {
-            "access_level": "Undocumented",
+            "access_level": "Write",
             "action": "DeleteTransitGateway",
-            "condition_keys": [],
-            "description": "Not Documented by AWS",
+            "condition_keys": [
+                "aws:ResourceTag/${TagKey}",
+                "ec2:Region",
+                "ec2:ResourceTag/${TagKey}"
+            ],
+            "description": "Grants permission to delete a transit gateway",
             "orphan": false,
-            "resources": []
+            "resources": [
+                "transit-gateway"
+            ]
         },
         "DeleteTransitGatewayConnect": {
-            "access_level": "Undocumented",
+            "access_level": "Write",
             "action": "DeleteTransitGatewayConnect",
-            "condition_keys": [],
-            "description": "Not Documented by AWS",
+            "condition_keys": [
+                "aws:ResourceTag/${TagKey}",
+                "ec2:Region",
+                "ec2:ResourceTag/${TagKey}"
+            ],
+            "description": "Grants permission to delete a transit gateway connect attachment",
             "orphan": false,
-            "resources": []
+            "resources": [
+                "transit-gateway-attachment"
+            ]
         },
         "DeleteTransitGatewayConnectPeer": {
-            "access_level": "Undocumented",
+            "access_level": "Write",
             "action": "DeleteTransitGatewayConnectPeer",
-            "condition_keys": [],
-            "description": "Not Documented by AWS",
+            "condition_keys": [
+                "aws:ResourceTag/${TagKey}",
+                "ec2:Region",
+                "ec2:ResourceTag/${TagKey}"
+            ],
+            "description": "Grants permission to delete a transit gateway connect peer",
             "orphan": false,
-            "resources": []
+            "resources": [
+                "transit-gateway-connect-peer"
+            ]
         },
         "DeleteTransitGatewayMulticastDomain": {
-            "access_level": "Undocumented",
+            "access_level": "Write",
             "action": "DeleteTransitGatewayMulticastDomain",
-            "condition_keys": [],
-            "description": "Not Documented by AWS",
+            "condition_keys": [
+                "aws:ResourceTag/${TagKey}",
+                "ec2:Region",
+                "ec2:ResourceTag/${TagKey}"
+            ],
+            "description": "Grants permission to delete a transit gateway multicast domain",
             "orphan": false,
-            "resources": []
+            "resources": [
+                "transit-gateway-multicast-domain"
+            ]
         },
         "DeleteTransitGatewayPeeringAttachment": {
-            "access_level": "Undocumented",
+            "access_level": "Write",
             "action": "DeleteTransitGatewayPeeringAttachment",
-            "condition_keys": [],
-            "description": "Not Documented by AWS",
+            "condition_keys": [
+                "aws:ResourceTag/${TagKey}",
+                "ec2:Region",
+                "ec2:ResourceTag/${TagKey}"
+            ],
+            "description": "Grants permission to delete a peering attachment from a transit gateway",
             "orphan": false,
-            "resources": []
+            "resources": [
+                "transit-gateway-attachment"
+            ]
         },
         "DeleteTransitGatewayPolicyTable": {
-            "access_level": "Undocumented",
+            "access_level": "Write",
             "action": "DeleteTransitGatewayPolicyTable",
-            "condition_keys": [],
-            "description": "Not Documented by AWS",
+            "condition_keys": [
+                "aws:ResourceTag/${TagKey}",
+                "ec2:Region",
+                "ec2:ResourceTag/${TagKey}"
+            ],
+            "description": "Grants permission to delete a transit gateway policy table",
             "orphan": false,
-            "resources": []
+            "resources": [
+                "transit-gateway-policy-table"
+            ]
         },
         "DeleteTransitGatewayPrefixListReference": {
-            "access_level": "Undocumented",
+            "access_level": "Write",
             "action": "DeleteTransitGatewayPrefixListReference",
-            "condition_keys": [],
-            "description": "Not Documented by AWS",
+            "condition_keys": [
+                "aws:ResourceTag/${TagKey}",
+                "ec2:Region",
+                "ec2:ResourceTag/${TagKey}"
+            ],
+            "description": "Grants permission to delete a transit gateway prefix list reference",
             "orphan": false,
-            "resources": []
+            "resources": [
+                "prefix-list",
+                "transit-gateway-route-table"
+            ]
         },
         "DeleteTransitGatewayRoute": {
-            "access_level": "Undocumented",
+            "access_level": "Write",
             "action": "DeleteTransitGatewayRoute",
-            "condition_keys": [],
-            "description": "Not Documented by AWS",
+            "condition_keys": [
+                "aws:ResourceTag/${TagKey}",
+                "ec2:Region",
+                "ec2:ResourceTag/${TagKey}"
+            ],
+            "description": "Grants permission to delete a route from a transit gateway route table",
             "orphan": false,
-            "resources": []
+            "resources": [
+                "transit-gateway-route-table"
+            ]
         },
         "DeleteTransitGatewayRouteTable": {
-            "access_level": "Undocumented",
+            "access_level": "Write",
             "action": "DeleteTransitGatewayRouteTable",
-            "condition_keys": [],
-            "description": "Not Documented by AWS",
+            "condition_keys": [
+                "aws:ResourceTag/${TagKey}",
+                "ec2:Region",
+                "ec2:ResourceTag/${TagKey}"
+            ],
+            "description": "Grants permission to delete a transit gateway route table",
             "orphan": false,
-            "resources": []
+            "resources": [
+                "transit-gateway-route-table"
+            ]
         },
         "DeleteTransitGatewayRouteTableAnnouncement": {
-            "access_level": "Undocumented",
+            "access_level": "Write",
             "action": "DeleteTransitGatewayRouteTableAnnouncement",
-            "condition_keys": [],
-            "description": "Not Documented by AWS",
+            "condition_keys": [
+                "aws:ResourceTag/${TagKey}",
+                "ec2:Region",
+                "ec2:ResourceTag/${TagKey}"
+            ],
+            "description": "Grants permission to delete a transit gateway route table announcement",
             "orphan": false,
-            "resources": []
+            "resources": [
+                "transit-gateway-route-table-announcement"
+            ]
         },
         "DeleteTransitGatewayVpcAttachment": {
-            "access_level": "Undocumented",
+            "access_level": "Write",
             "action": "DeleteTransitGatewayVpcAttachment",
-            "condition_keys": [],
-            "description": "Not Documented by AWS",
+            "condition_keys": [
+                "aws:ResourceTag/${TagKey}",
+                "ec2:Region",
+                "ec2:ResourceTag/${TagKey}"
+            ],
+            "description": "Grants permission to delete a VPC attachment from a transit gateway",
             "orphan": false,
-            "resources": []
+            "resources": [
+                "transit-gateway-attachment"
+            ]
         },
         "DeleteVerifiedAccessEndpoint": {
-            "access_level": "Undocumented",
+            "access_level": "Write",
             "action": "DeleteVerifiedAccessEndpoint",
-            "condition_keys": [],
-            "description": "Not Documented by AWS",
+            "condition_keys": [
+                "aws:ResourceTag/${TagKey}",
+                "ec2:Region",
+                "ec2:ResourceTag/${TagKey}"
+            ],
+            "description": "Grants permission to delete a Verified Access endpoint",
             "orphan": false,
-            "resources": []
+            "resources": [
+                "verified-access-endpoint"
+            ]
         },
         "DeleteVerifiedAccessGroup": {
-            "access_level": "Undocumented",
+            "access_level": "Write",
             "action": "DeleteVerifiedAccessGroup",
-            "condition_keys": [],
-            "description": "Not Documented by AWS",
+            "condition_keys": [
+                "aws:ResourceTag/${TagKey}",
+                "ec2:Region",
+                "ec2:ResourceTag/${TagKey}"
+            ],
+            "description": "Grants permission to delete a Verified Access group",
             "orphan": false,
-            "resources": []
+            "resources": [
+                "verified-access-group"
+            ]
         },
         "DeleteVerifiedAccessInstance": {
-            "access_level": "Undocumented",
+            "access_level": "Write",
             "action": "DeleteVerifiedAccessInstance",
-            "condition_keys": [],
-            "description": "Not Documented by AWS",
+            "condition_keys": [
+                "aws:ResourceTag/${TagKey}",
+                "ec2:Region",
+                "ec2:ResourceTag/${TagKey}"
+            ],
+            "description": "Grants permission to delete a Verified Access instance",
             "orphan": false,
-            "resources": []
+            "resources": [
+                "verified-access-instance"
+            ]
         },
         "DeleteVerifiedAccessTrustProvider": {
-            "access_level": "Undocumented",
+            "access_level": "Write",
             "action": "DeleteVerifiedAccessTrustProvider",
-            "condition_keys": [],
-            "description": "Not Documented by AWS",
+            "condition_keys": [
+                "aws:ResourceTag/${TagKey}",
+                "ec2:Region",
+                "ec2:ResourceTag/${TagKey}"
+            ],
+            "description": "Grants permission to delete a verified trust provider",
             "orphan": false,
-            "resources": []
+            "resources": [
+                "verified-access-trust-provider"
+            ]
         },
         "DeleteVolume": {
-            "access_level": "Undocumented",
+            "access_level": "Write",
             "action": "DeleteVolume",
-            "condition_keys": [],
-            "description": "Not Documented by AWS",
+            "condition_keys": [
+                "aws:ResourceTag/${TagKey}",
+                "ec2:AvailabilityZone",
+                "ec2:Encrypted",
+                "ec2:ParentSnapshot",
+                "ec2:Region",
+                "ec2:ResourceTag/${TagKey}",
+                "ec2:VolumeID",
+                "ec2:VolumeIops",
+                "ec2:VolumeSize",
+                "ec2:VolumeThroughput",
+                "ec2:VolumeType"
+            ],
+            "description": "Grants permission to delete an EBS volume",
             "orphan": false,
-            "resources": []
+            "resources": [
+                "volume"
+            ]
         },
         "DeleteVpc": {
-            "access_level": "Undocumented",
+            "access_level": "Write",
             "action": "DeleteVpc",
-            "condition_keys": [],
-            "description": "Not Documented by AWS",
+            "condition_keys": [
+                "aws:ResourceTag/${TagKey}",
+                "ec2:Region",
+                "ec2:ResourceTag/${TagKey}",
+                "ec2:Tenancy",
+                "ec2:VpcID"
+            ],
+            "description": "Grants permission to delete a VPC",
             "orphan": false,
-            "resources": []
+            "resources": [
+                "vpc"
+            ]
         },
         "DeleteVpcEndpointConnectionNotifications": {
-            "access_level": "Undocumented",
+            "access_level": "Write",
             "action": "DeleteVpcEndpointConnectionNotifications",
-            "condition_keys": [],
-            "description": "Not Documented by AWS",
+            "condition_keys": [
+                "aws:ResourceTag/${TagKey}",
+                "ec2:Region",
+                "ec2:ResourceTag/${TagKey}"
+            ],
+            "description": "Grants permission to delete one or more VPC endpoint connection notifications",
             "orphan": false,
-            "resources": []
+            "resources": [
+                "vpc-endpoint",
+                "vpc-endpoint-service"
+            ]
         },
         "DeleteVpcEndpointServiceConfigurations": {
-            "access_level": "Undocumented",
+            "access_level": "Write",
             "action": "DeleteVpcEndpointServiceConfigurations",
-            "condition_keys": [],
-            "description": "Not Documented by AWS",
+            "condition_keys": [
+                "aws:ResourceTag/${TagKey}",
+                "ec2:Region",
+                "ec2:ResourceTag/${TagKey}"
+            ],
+            "description": "Grants permission to delete one or more VPC endpoint service configurations",
             "orphan": false,
-            "resources": []
+            "resources": [
+                "vpc-endpoint-service"
+            ]
         },
         "DeleteVpcEndpoints": {
-            "access_level": "Undocumented",
+            "access_level": "Write",
             "action": "DeleteVpcEndpoints",
-            "condition_keys": [],
-            "description": "Not Documented by AWS",
+            "condition_keys": [
+                "aws:ResourceTag/${TagKey}",
+                "ec2:Region",
+                "ec2:ResourceTag/${TagKey}",
+                "ec2:VpceServiceName"
+            ],
+            "description": "Grants permission to delete one or more VPC endpoints",
             "orphan": false,
-            "resources": []
+            "resources": [
+                "vpc-endpoint"
+            ]
         },
         "DeleteVpcPeeringConnection": {
-            "access_level": "Undocumented",
+            "access_level": "Write",
             "action": "DeleteVpcPeeringConnection",
-            "condition_keys": [],
-            "description": "Not Documented by AWS",
+            "condition_keys": [
+                "aws:ResourceTag/${TagKey}",
+                "ec2:AccepterVpc",
+                "ec2:Region",
+                "ec2:RequesterVpc",
+                "ec2:ResourceTag/${TagKey}",
+                "ec2:VpcPeeringConnectionID"
+            ],
+            "description": "Grants permission to delete a VPC peering connection",
             "orphan": false,
-            "resources": []
+            "resources": [
+                "vpc-peering-connection"
+            ]
         },
         "DeleteVpnConnection": {
-            "access_level": "Undocumented",
+            "access_level": "Write",
             "action": "DeleteVpnConnection",
-            "condition_keys": [],
-            "description": "Not Documented by AWS",
+            "condition_keys": [
+                "aws:ResourceTag/${TagKey}",
+                "ec2:Region",
+                "ec2:ResourceTag/${TagKey}"
+            ],
+            "description": "Grants permission to delete a VPN connection",
             "orphan": false,
-            "resources": []
+            "resources": [
+                "vpn-connection"
+            ]
         },
         "DeleteVpnConnectionRoute": {
-            "access_level": "Undocumented",
+            "access_level": "Write",
             "action": "DeleteVpnConnectionRoute",
-            "condition_keys": [],
-            "description": "Not Documented by AWS",
+            "condition_keys": [
+                "aws:ResourceTag/${TagKey}",
+                "ec2:Region",
+                "ec2:ResourceTag/${TagKey}"
+            ],
+            "description": "Grants permission to delete a static route for a VPN connection between a virtual private gateway and a customer gateway",
             "orphan": false,
-            "resources": []
+            "resources": [
+                "vpn-connection"
+            ]
         },
         "DeleteVpnGateway": {
-            "access_level": "Undocumented",
+            "access_level": "Write",
             "action": "DeleteVpnGateway",
-            "condition_keys": [],
-            "description": "Not Documented by AWS",
+            "condition_keys": [
+                "aws:ResourceTag/${TagKey}",
+                "ec2:Region",
+                "ec2:ResourceTag/${TagKey}"
+            ],
+            "description": "Grants permission to delete a virtual private gateway",
             "orphan": false,
-            "resources": []
+            "resources": [
+                "vpn-gateway"
+            ]
         },
         "DeprovisionByoipCidr": {
-            "access_level": "Undocumented",
+            "access_level": "Write",
             "action": "DeprovisionByoipCidr",
-            "condition_keys": [],
-            "description": "Not Documented by AWS",
+            "condition_keys": [
+                "ec2:Region"
+            ],
+            "description": "Grants permission to release an IP address range that was provisioned through bring your own IP addresses (BYOIP), and to delete the corresponding address pool",
             "orphan": false,
             "resources": []
         },
         "DeprovisionIpamPoolCidr": {
-            "access_level": "Undocumented",
+            "access_level": "Write",
             "action": "DeprovisionIpamPoolCidr",
-            "condition_keys": [],
-            "description": "Not Documented by AWS",
+            "condition_keys": [
+                "aws:ResourceTag/${TagKey}",
+                "ec2:Region",
+                "ec2:ResourceTag/${TagKey}"
+            ],
+            "description": "Grants permission to deprovision a CIDR provisioned from an Amazon VPC IP Address Manager (IPAM) pool",
             "orphan": false,
-            "resources": []
+            "resources": [
+                "ipam-pool"
+            ]
         },
         "DeprovisionPublicIpv4PoolCidr": {
-            "access_level": "Undocumented",
+            "access_level": "Write",
             "action": "DeprovisionPublicIpv4PoolCidr",
-            "condition_keys": [],
-            "description": "Not Documented by AWS",
+            "condition_keys": [
+                "aws:ResourceTag/${TagKey}",
+                "ec2:Region",
+                "ec2:ResourceTag/${TagKey}"
+            ],
+            "description": "Grants permission to deprovision a CIDR from a public IPv4 pool",
             "orphan": false,
-            "resources": []
+            "resources": [
+                "ipv4pool-ec2"
+            ]
         },
         "DeregisterImage": {
-            "access_level": "Undocumented",
+            "access_level": "Write",
             "action": "DeregisterImage",
-            "condition_keys": [],
-            "description": "Not Documented by AWS",
+            "condition_keys": [
+                "aws:ResourceTag/${TagKey}",
+                "ec2:ImageID",
+                "ec2:ImageType",
+                "ec2:Owner",
+                "ec2:Public",
+                "ec2:Region",
+                "ec2:ResourceTag/${TagKey}",
+                "ec2:RootDeviceType"
+            ],
+            "description": "Grants permission to deregister an Amazon Machine Image (AMI)",
             "orphan": false,
-            "resources": []
+            "resources": [
+                "image"
+            ]
         },
         "DeregisterInstanceEventNotificationAttributes": {
-            "access_level": "Undocumented",
+            "access_level": "Write",
             "action": "DeregisterInstanceEventNotificationAttributes",
-            "condition_keys": [],
-            "description": "Not Documented by AWS",
+            "condition_keys": [
+                "ec2:Region"
+            ],
+            "description": "Grants permission to remove tags from the set of tags to include in notifications about scheduled events for your instances",
             "orphan": false,
             "resources": []
         },
         "DeregisterTransitGatewayMulticastGroupMembers": {
-            "access_level": "Undocumented",
+            "access_level": "Write",
             "action": "DeregisterTransitGatewayMulticastGroupMembers",
-            "condition_keys": [],
-            "description": "Not Documented by AWS",
+            "condition_keys": [
+                "aws:ResourceTag/${TagKey}",
+                "ec2:AvailabilityZone",
+                "ec2:NetworkInterfaceID",
+                "ec2:Region",
+                "ec2:ResourceTag/${TagKey}",
+                "ec2:Subnet",
+                "ec2:Vpc"
+            ],
+            "description": "Grants permission to deregister one or more network interface members from a group IP address in a transit gateway multicast domain",
             "orphan": false,
-            "resources": []
+            "resources": [
+                "network-interface",
+                "transit-gateway-multicast-domain"
+            ]
         },
         "DeregisterTransitGatewayMulticastGroupSources": {
-            "access_level": "Undocumented",
+            "access_level": "Write",
             "action": "DeregisterTransitGatewayMulticastGroupSources",
-            "condition_keys": [],
-            "description": "Not Documented by AWS",
+            "condition_keys": [
+                "aws:ResourceTag/${TagKey}",
+                "ec2:AvailabilityZone",
+                "ec2:NetworkInterfaceID",
+                "ec2:Region",
+                "ec2:ResourceTag/${TagKey}",
+                "ec2:Subnet",
+                "ec2:Vpc"
+            ],
+            "description": "Grants permission to deregister one or more network interface sources from a group IP address in a transit gateway multicast domain",
             "orphan": false,
-            "resources": []
+            "resources": [
+                "network-interface",
+                "transit-gateway-multicast-domain"
+            ]
         },
         "DescribeAccountAttributes": {
-            "access_level": "Undocumented",
+            "access_level": "List",
             "action": "DescribeAccountAttributes",
-            "condition_keys": [],
-            "description": "Not Documented by AWS",
+            "condition_keys": [
+                "ec2:Region"
+            ],
+            "description": "Grants permission to describe the attributes of the AWS account",
             "orphan": false,
             "resources": []
         },
         "DescribeAddressTransfers": {
-            "access_level": "Undocumented",
+            "access_level": "List",
             "action": "DescribeAddressTransfers",
-            "condition_keys": [],
-            "description": "Not Documented by AWS",
+            "condition_keys": [
+                "ec2:Region"
+            ],
+            "description": "Grants permission to describe an Elastic IP address transfer",
             "orphan": false,
             "resources": []
         },
         "DescribeAddresses": {
-            "access_level": "Undocumented",
+            "access_level": "List",
             "action": "DescribeAddresses",
-            "condition_keys": [],
-            "description": "Not Documented by AWS",
+            "condition_keys": [
+                "ec2:Region"
+            ],
+            "description": "Grants permission to describe one or more Elastic IP addresses",
             "orphan": false,
             "resources": []
         },
         "DescribeAddressesAttribute": {
-            "access_level": "Undocumented",
+            "access_level": "List",
             "action": "DescribeAddressesAttribute",
-            "condition_keys": [],
-            "description": "Not Documented by AWS",
+            "condition_keys": [
+                "aws:ResourceTag/${TagKey}",
+                "ec2:AllocationId",
+                "ec2:Domain",
+                "ec2:PublicIpAddress",
+                "ec2:Region",
+                "ec2:ResourceTag/${TagKey}"
+            ],
+            "description": "Grants permission to describe the attributes of the specified Elastic IP addresses",
             "orphan": false,
-            "resources": []
+            "resources": [
+                "elastic-ip"
+            ]
         },
         "DescribeAggregateIdFormat": {
-            "access_level": "Undocumented",
+            "access_level": "List",
             "action": "DescribeAggregateIdFormat",
-            "condition_keys": [],
-            "description": "Not Documented by AWS",
+            "condition_keys": [
+                "ec2:Region"
+            ],
+            "description": "Grants permission to describe the longer ID format settings for all resource types",
             "orphan": false,
             "resources": []
         },
         "DescribeAvailabilityZones": {
-            "access_level": "Undocumented",
+            "access_level": "List",
             "action": "DescribeAvailabilityZones",
-            "condition_keys": [],
-            "description": "Not Documented by AWS",
+            "condition_keys": [
+                "ec2:Region"
+            ],
+            "description": "Grants permission to describe one or more of the Availability Zones that are available to you",
             "orphan": false,
             "resources": []
         },
         "DescribeAwsNetworkPerformanceMetricSubscriptions": {
-            "access_level": "Undocumented",
+            "access_level": "List",
             "action": "DescribeAwsNetworkPerformanceMetricSubscriptions",
-            "condition_keys": [],
-            "description": "Not Documented by AWS",
+            "condition_keys": [
+                "ec2:Region"
+            ],
+            "description": "Grants permission to describe the current infrastructure performance metric subscriptions",
             "orphan": false,
             "resources": []
         },
         "DescribeBundleTasks": {
-            "access_level": "Undocumented",
+            "access_level": "List",
             "action": "DescribeBundleTasks",
-            "condition_keys": [],
-            "description": "Not Documented by AWS",
+            "condition_keys": [
+                "ec2:Region"
+            ],
+            "description": "Grants permission to describe one or more bundling tasks",
             "orphan": false,
             "resources": []
         },
         "DescribeByoipCidrs": {
-            "access_level": "Undocumented",
+            "access_level": "List",
             "action": "DescribeByoipCidrs",
-            "condition_keys": [],
-            "description": "Not Documented by AWS",
+            "condition_keys": [
+                "ec2:Region"
+            ],
+            "description": "Grants permission to describe the IP address ranges that were provisioned through bring your own IP addresses (BYOIP)",
             "orphan": false,
             "resources": []
         },
         "DescribeCapacityReservationFleets": {
-            "access_level": "Undocumented",
+            "access_level": "List",
             "action": "DescribeCapacityReservationFleets",
-            "condition_keys": [],
-            "description": "Not Documented by AWS",
+            "condition_keys": [
+                "ec2:Region"
+            ],
+            "description": "Grants permission to describe one or more Capacity Reservation Fleets",
             "orphan": false,
             "resources": []
         },
         "DescribeCapacityReservations": {
-            "access_level": "Undocumented",
+            "access_level": "List",
             "action": "DescribeCapacityReservations",
-            "condition_keys": [],
-            "description": "Not Documented by AWS",
+            "condition_keys": [
+                "ec2:Region"
+            ],
+            "description": "Grants permission to describe one or more Capacity Reservations",
             "orphan": false,
             "resources": []
         },
         "DescribeCarrierGateways": {
-            "access_level": "Undocumented",
+            "access_level": "List",
             "action": "DescribeCarrierGateways",
-            "condition_keys": [],
-            "description": "Not Documented by AWS",
+            "condition_keys": [
+                "ec2:Region"
+            ],
+            "description": "Grants permission to describe one or more Carrier Gateways",
             "orphan": false,
             "resources": []
         },
         "DescribeClassicLinkInstances": {
-            "access_level": "Undocumented",
+            "access_level": "List",
             "action": "DescribeClassicLinkInstances",
-            "condition_keys": [],
-            "description": "Not Documented by AWS",
+            "condition_keys": [
+                "ec2:Region"
+            ],
+            "description": "Grants permission to describe one or more linked EC2-Classic instances",
             "orphan": false,
             "resources": []
         },
         "DescribeClientVpnAuthorizationRules": {
-            "access_level": "Undocumented",
+            "access_level": "List",
             "action": "DescribeClientVpnAuthorizationRules",
-            "condition_keys": [],
-            "description": "Not Documented by AWS",
+            "condition_keys": [
+                "aws:ResourceTag/${TagKey}",
+                "ec2:Region",
+                "ec2:ResourceTag/${TagKey}"
+            ],
+            "description": "Grants permission to describe the authorization rules for a Client VPN endpoint",
             "orphan": false,
-            "resources": []
+            "resources": [
+                "client-vpn-endpoint"
+            ]
         },
         "DescribeClientVpnConnections": {
-            "access_level": "Undocumented",
+            "access_level": "List",
             "action": "DescribeClientVpnConnections",
-            "condition_keys": [],
-            "description": "Not Documented by AWS",
+            "condition_keys": [
+                "aws:ResourceTag/${TagKey}",
+                "ec2:ClientRootCertificateChainArn",
+                "ec2:CloudwatchLogGroupArn",
+                "ec2:CloudwatchLogStreamArn",
+                "ec2:DirectoryArn",
+                "ec2:Region",
+                "ec2:ResourceTag/${TagKey}",
+                "ec2:SamlProviderArn",
+                "ec2:ServerCertificateArn"
+            ],
+            "description": "Grants permission to describe active client connections and connections that have been terminated within the last 60 minutes for a Client VPN endpoint",
             "orphan": false,
-            "resources": []
+            "resources": [
+                "client-vpn-endpoint"
+            ]
         },
         "DescribeClientVpnEndpoints": {
-            "access_level": "Undocumented",
+            "access_level": "List",
             "action": "DescribeClientVpnEndpoints",
-            "condition_keys": [],
-            "description": "Not Documented by AWS",
+            "condition_keys": [
+                "aws:ResourceTag/${TagKey}",
+                "ec2:ClientRootCertificateChainArn",
+                "ec2:CloudwatchLogGroupArn",
+                "ec2:CloudwatchLogStreamArn",
+                "ec2:DirectoryArn",
+                "ec2:Region",
+                "ec2:ResourceTag/${TagKey}",
+                "ec2:SamlProviderArn",
+                "ec2:ServerCertificateArn"
+            ],
+            "description": "Grants permission to describe one or more Client VPN endpoints",
             "orphan": false,
-            "resources": []
+            "resources": [
+                "client-vpn-endpoint"
+            ]
         },
         "DescribeClientVpnRoutes": {
-            "access_level": "Undocumented",
+            "access_level": "List",
             "action": "DescribeClientVpnRoutes",
-            "condition_keys": [],
-            "description": "Not Documented by AWS",
+            "condition_keys": [
+                "aws:ResourceTag/${TagKey}",
+                "ec2:ClientRootCertificateChainArn",
+                "ec2:CloudwatchLogGroupArn",
+                "ec2:CloudwatchLogStreamArn",
+                "ec2:DirectoryArn",
+                "ec2:Region",
+                "ec2:ResourceTag/${TagKey}",
+                "ec2:SamlProviderArn",
+                "ec2:ServerCertificateArn"
+            ],
+            "description": "Grants permission to describe the routes for a Client VPN endpoint",
             "orphan": false,
-            "resources": []
+            "resources": [
+                "client-vpn-endpoint"
+            ]
         },
         "DescribeClientVpnTargetNetworks": {
-            "access_level": "Undocumented",
+            "access_level": "List",
             "action": "DescribeClientVpnTargetNetworks",
-            "condition_keys": [],
-            "description": "Not Documented by AWS",
+            "condition_keys": [
+                "aws:ResourceTag/${TagKey}",
+                "ec2:ClientRootCertificateChainArn",
+                "ec2:CloudwatchLogGroupArn",
+                "ec2:CloudwatchLogStreamArn",
+                "ec2:DirectoryArn",
+                "ec2:Region",
+                "ec2:ResourceTag/${TagKey}",
+                "ec2:SamlProviderArn",
+                "ec2:ServerCertificateArn"
+            ],
+            "description": "Grants permission to describe the target networks that are associated with a Client VPN endpoint",
             "orphan": false,
-            "resources": []
+            "resources": [
+                "client-vpn-endpoint"
+            ]
         },
         "DescribeCoipPools": {
-            "access_level": "Undocumented",
+            "access_level": "List",
             "action": "DescribeCoipPools",
-            "condition_keys": [],
-            "description": "Not Documented by AWS",
+            "condition_keys": [
+                "ec2:Region"
+            ],
+            "description": "Grants permission to describe the specified customer-owned address pools or all of your customer-owned address pools",
             "orphan": false,
             "resources": []
         },
         "DescribeConversionTasks": {
-            "access_level": "Undocumented",
+            "access_level": "List",
             "action": "DescribeConversionTasks",
-            "condition_keys": [],
-            "description": "Not Documented by AWS",
+            "condition_keys": [
+                "ec2:Region"
+            ],
+            "description": "Grants permission to describe one or more conversion tasks",
             "orphan": false,
             "resources": []
         },
         "DescribeCustomerGateways": {
-            "access_level": "Undocumented",
+            "access_level": "List",
             "action": "DescribeCustomerGateways",
-            "condition_keys": [],
-            "description": "Not Documented by AWS",
+            "condition_keys": [
+                "ec2:Region"
+            ],
+            "description": "Grants permission to describe one or more customer gateways",
             "orphan": false,
             "resources": []
         },
         "DescribeDhcpOptions": {
-            "access_level": "Undocumented",
+            "access_level": "List",
             "action": "DescribeDhcpOptions",
-            "condition_keys": [],
-            "description": "Not Documented by AWS",
+            "condition_keys": [
+                "ec2:Region"
+            ],
+            "description": "Grants permission to describe one or more DHCP options sets",
             "orphan": false,
             "resources": []
         },
         "DescribeEgressOnlyInternetGateways": {
-            "access_level": "Undocumented",
+            "access_level": "List",
             "action": "DescribeEgressOnlyInternetGateways",
-            "condition_keys": [],
-            "description": "Not Documented by AWS",
+            "condition_keys": [
+                "ec2:Region"
+            ],
+            "description": "Grants permission to describe one or more egress-only internet gateways",
             "orphan": false,
             "resources": []
         },
         "DescribeElasticGpus": {
-            "access_level": "Undocumented",
+            "access_level": "List",
             "action": "DescribeElasticGpus",
-            "condition_keys": [],
-            "description": "Not Documented by AWS",
+            "condition_keys": [
+                "ec2:Region"
+            ],
+            "description": "Grants permission to describe an Elastic Graphics accelerator that is associated with an instance",
             "orphan": false,
             "resources": []
         },
         "DescribeExportImageTasks": {
-            "access_level": "Undocumented",
+            "access_level": "List",
             "action": "DescribeExportImageTasks",
-            "condition_keys": [],
-            "description": "Not Documented by AWS",
+            "condition_keys": [
+                "ec2:Region"
+            ],
+            "description": "Grants permission to describe one or more export image tasks",
             "orphan": false,
             "resources": []
         },
         "DescribeExportTasks": {
-            "access_level": "Undocumented",
+            "access_level": "List",
             "action": "DescribeExportTasks",
-            "condition_keys": [],
-            "description": "Not Documented by AWS",
+            "condition_keys": [
+                "ec2:Region"
+            ],
+            "description": "Grants permission to describe one or more export instance tasks",
             "orphan": false,
             "resources": []
         },
         "DescribeFastLaunchImages": {
-            "access_level": "Undocumented",
+            "access_level": "List",
             "action": "DescribeFastLaunchImages",
-            "condition_keys": [],
-            "description": "Not Documented by AWS",
+            "condition_keys": [
+                "aws:ResourceTag/${TagKey}",
+                "ec2:ImageID",
+                "ec2:ImageType",
+                "ec2:Owner",
+                "ec2:Public",
+                "ec2:Region",
+                "ec2:ResourceTag/${TagKey}",
+                "ec2:RootDeviceType"
+            ],
+            "description": "Grants permission to describe fast-launch enabled Windows AMIs",
             "orphan": false,
-            "resources": []
+            "resources": [
+                "image"
+            ]
         },
         "DescribeFastSnapshotRestores": {
-            "access_level": "Undocumented",
+            "access_level": "List",
             "action": "DescribeFastSnapshotRestores",
-            "condition_keys": [],
-            "description": "Not Documented by AWS",
+            "condition_keys": [
+                "ec2:Region"
+            ],
+            "description": "Grants permission to describe the state of fast snapshot restores for snapshots",
             "orphan": false,
             "resources": []
         },
         "DescribeFleetHistory": {
-            "access_level": "Undocumented",
+            "access_level": "List",
             "action": "DescribeFleetHistory",
-            "condition_keys": [],
-            "description": "Not Documented by AWS",
+            "condition_keys": [
+                "aws:ResourceTag/${TagKey}",
+                "ec2:Region",
+                "ec2:ResourceTag/${TagKey}"
+            ],
+            "description": "Grants permission to describe the events for an EC2 Fleet during a specified time",
             "orphan": false,
-            "resources": []
+            "resources": [
+                "fleet"
+            ]
         },
         "DescribeFleetInstances": {
-            "access_level": "Undocumented",
+            "access_level": "List",
             "action": "DescribeFleetInstances",
-            "condition_keys": [],
-            "description": "Not Documented by AWS",
+            "condition_keys": [
+                "aws:ResourceTag/${TagKey}",
+                "ec2:Region",
+                "ec2:ResourceTag/${TagKey}"
+            ],
+            "description": "Grants permission to describe the running instances for an EC2 Fleet",
             "orphan": false,
-            "resources": []
+            "resources": [
+                "fleet"
+            ]
         },
         "DescribeFleets": {
-            "access_level": "Undocumented",
+            "access_level": "List",
             "action": "DescribeFleets",
-            "condition_keys": [],
-            "description": "Not Documented by AWS",
+            "condition_keys": [
+                "ec2:Region"
+            ],
+            "description": "Grants permission to describe one or more EC2 Fleets",
             "orphan": false,
             "resources": []
         },
         "DescribeFlowLogs": {
-            "access_level": "Undocumented",
+            "access_level": "List",
             "action": "DescribeFlowLogs",
-            "condition_keys": [],
-            "description": "Not Documented by AWS",
+            "condition_keys": [
+                "ec2:Region"
+            ],
+            "description": "Grants permission to describe one or more flow logs",
             "orphan": false,
             "resources": []
         },
         "DescribeFpgaImageAttribute": {
-            "access_level": "Undocumented",
+            "access_level": "List",
             "action": "DescribeFpgaImageAttribute",
-            "condition_keys": [],
-            "description": "Not Documented by AWS",
+            "condition_keys": [
+                "aws:ResourceTag/${TagKey}",
+                "ec2:Owner",
+                "ec2:Region",
+                "ec2:ResourceTag/${TagKey}"
+            ],
+            "description": "Grants permission to describe the attributes of an Amazon FPGA Image (AFI)",
             "orphan": false,
-            "resources": []
+            "resources": [
+                "fpga-image"
+            ]
         },
         "DescribeFpgaImages": {
-            "access_level": "Undocumented",
+            "access_level": "List",
             "action": "DescribeFpgaImages",
-            "condition_keys": [],
-            "description": "Not Documented by AWS",
+            "condition_keys": [
+                "ec2:Region"
+            ],
+            "description": "Grants permission to describe one or more Amazon FPGA Images (AFIs)",
             "orphan": false,
             "resources": []
         },
         "DescribeHostReservationOfferings": {
-            "access_level": "Undocumented",
+            "access_level": "List",
             "action": "DescribeHostReservationOfferings",
-            "condition_keys": [],
-            "description": "Not Documented by AWS",
+            "condition_keys": [
+                "ec2:Region"
+            ],
+            "description": "Grants permission to describe the Dedicated Host Reservations that are available to purchase",
             "orphan": false,
             "resources": []
         },
         "DescribeHostReservations": {
-            "access_level": "Undocumented",
+            "access_level": "List",
             "action": "DescribeHostReservations",
-            "condition_keys": [],
-            "description": "Not Documented by AWS",
+            "condition_keys": [
+                "ec2:Region"
+            ],
+            "description": "Grants permission to describe the Dedicated Host Reservations that are associated with Dedicated Hosts in the AWS account",
             "orphan": false,
             "resources": []
         },
         "DescribeHosts": {
-            "access_level": "Undocumented",
+            "access_level": "List",
             "action": "DescribeHosts",
-            "condition_keys": [],
-            "description": "Not Documented by AWS",
+            "condition_keys": [
+                "ec2:Region"
+            ],
+            "description": "Grants permission to describe one or more Dedicated Hosts",
             "orphan": false,
             "resources": []
         },
         "DescribeIamInstanceProfileAssociations": {
-            "access_level": "Undocumented",
+            "access_level": "List",
             "action": "DescribeIamInstanceProfileAssociations",
-            "condition_keys": [],
-            "description": "Not Documented by AWS",
+            "condition_keys": [
+                "ec2:Region"
+            ],
+            "description": "Grants permission to describe the IAM instance profile associations",
             "orphan": false,
             "resources": []
         },
         "DescribeIdFormat": {
-            "access_level": "Undocumented",
+            "access_level": "List",
             "action": "DescribeIdFormat",
-            "condition_keys": [],
-            "description": "Not Documented by AWS",
+            "condition_keys": [
+                "ec2:Region"
+            ],
+            "description": "Grants permission to describe the ID format settings for resources",
             "orphan": false,
             "resources": []
         },
         "DescribeIdentityIdFormat": {
-            "access_level": "Undocumented",
+            "access_level": "List",
             "action": "DescribeIdentityIdFormat",
-            "condition_keys": [],
-            "description": "Not Documented by AWS",
+            "condition_keys": [
+                "ec2:Region"
+            ],
+            "description": "Grants permission to describe the ID format settings for resources for an IAM user, IAM role, or root user",
             "orphan": false,
             "resources": []
         },
         "DescribeImageAttribute": {
-            "access_level": "Undocumented",
+            "access_level": "List",
             "action": "DescribeImageAttribute",
-            "condition_keys": [],
-            "description": "Not Documented by AWS",
+            "condition_keys": [
+                "aws:ResourceTag/${TagKey}",
+                "ec2:ImageID",
+                "ec2:ImageType",
+                "ec2:Owner",
+                "ec2:Public",
+                "ec2:Region",
+                "ec2:ResourceTag/${TagKey}",
+                "ec2:RootDeviceType"
+            ],
+            "description": "Grants permission to describe an attribute of an Amazon Machine Image (AMI)",
             "orphan": false,
-            "resources": []
+            "resources": [
+                "image"
+            ]
         },
         "DescribeImages": {
-            "access_level": "Undocumented",
+            "access_level": "List",
             "action": "DescribeImages",
-            "condition_keys": [],
-            "description": "Not Documented by AWS",
+            "condition_keys": [
+                "ec2:Region"
+            ],
+            "description": "Grants permission to describe one or more images (AMIs, AKIs, and ARIs)",
             "orphan": false,
             "resources": []
         },
         "DescribeImportImageTasks": {
-            "access_level": "Undocumented",
+            "access_level": "List",
             "action": "DescribeImportImageTasks",
-            "condition_keys": [],
-            "description": "Not Documented by AWS",
+            "condition_keys": [
+                "ec2:Region"
+            ],
+            "description": "Grants permission to describe import virtual machine or import snapshot tasks",
             "orphan": false,
             "resources": []
         },
         "DescribeImportSnapshotTasks": {
-            "access_level": "Undocumented",
+            "access_level": "List",
             "action": "DescribeImportSnapshotTasks",
-            "condition_keys": [],
-            "description": "Not Documented by AWS",
+            "condition_keys": [
+                "ec2:Region"
+            ],
+            "description": "Grants permission to describe import snapshot tasks",
             "orphan": false,
             "resources": []
         },
         "DescribeInstanceAttribute": {
-            "access_level": "Undocumented",
+            "access_level": "List",
             "action": "DescribeInstanceAttribute",
-            "condition_keys": [],
-            "description": "Not Documented by AWS",
+            "condition_keys": [
+                "aws:ResourceTag/${TagKey}",
+                "ec2:AvailabilityZone",
+                "ec2:EbsOptimized",
+                "ec2:InstanceAutoRecovery",
+                "ec2:InstanceID",
+                "ec2:InstanceMarketType",
+                "ec2:InstanceMetadataTags",
+                "ec2:InstanceProfile",
+                "ec2:InstanceType",
+                "ec2:MetadataHttpEndpoint",
+                "ec2:MetadataHttpPutResponseHopLimit",
+                "ec2:MetadataHttpTokens",
+                "ec2:PlacementGroup",
+                "ec2:ProductCode",
+                "ec2:Region",
+                "ec2:ResourceTag/${TagKey}",
+                "ec2:RootDeviceType",
+                "ec2:Tenancy"
+            ],
+            "description": "Grants permission to describe the attributes of an instance",
             "orphan": false,
-            "resources": []
+            "resources": [
+                "instance"
+            ]
         },
         "DescribeInstanceCreditSpecifications": {
-            "access_level": "Undocumented",
+            "access_level": "List",
             "action": "DescribeInstanceCreditSpecifications",
-            "condition_keys": [],
-            "description": "Not Documented by AWS",
+            "condition_keys": [
+                "ec2:Region"
+            ],
+            "description": "Grants permission to describe the credit option for CPU usage of one or more burstable performance instances",
             "orphan": false,
             "resources": []
         },
         "DescribeInstanceEventNotificationAttributes": {
-            "access_level": "Undocumented",
+            "access_level": "List",
             "action": "DescribeInstanceEventNotificationAttributes",
-            "condition_keys": [],
-            "description": "Not Documented by AWS",
+            "condition_keys": [
+                "ec2:Region"
+            ],
+            "description": "Grants permission to describe the set of tags to include in notifications about scheduled events for your instances",
             "orphan": false,
             "resources": []
         },
         "DescribeInstanceEventWindows": {
-            "access_level": "Undocumented",
+            "access_level": "List",
             "action": "DescribeInstanceEventWindows",
-            "condition_keys": [],
-            "description": "Not Documented by AWS",
+            "condition_keys": [
+                "ec2:Region"
+            ],
+            "description": "Grants permission to describe the specified event windows or all event windows",
             "orphan": false,
             "resources": []
         },
         "DescribeInstanceStatus": {
-            "access_level": "Undocumented",
+            "access_level": "List",
             "action": "DescribeInstanceStatus",
-            "condition_keys": [],
-            "description": "Not Documented by AWS",
+            "condition_keys": [
+                "ec2:Region"
+            ],
+            "description": "Grants permission to describe the status of one or more instances",
             "orphan": false,
             "resources": []
         },
         "DescribeInstanceTypeOfferings": {
-            "access_level": "Undocumented",
+            "access_level": "List",
             "action": "DescribeInstanceTypeOfferings",
-            "condition_keys": [],
-            "description": "Not Documented by AWS",
+            "condition_keys": [
+                "ec2:Region"
+            ],
+            "description": "Grants permission to describe the set of instance types that are offered in a location",
             "orphan": false,
             "resources": []
         },
         "DescribeInstanceTypes": {
-            "access_level": "Undocumented",
+            "access_level": "List",
             "action": "DescribeInstanceTypes",
-            "condition_keys": [],
-            "description": "Not Documented by AWS",
+            "condition_keys": [
+                "ec2:Region"
+            ],
+            "description": "Grants permission to describe the details of instance types that are offered in a location",
             "orphan": false,
             "resources": []
         },
         "DescribeInstances": {
-            "access_level": "Undocumented",
+            "access_level": "List",
             "action": "DescribeInstances",
-            "condition_keys": [],
-            "description": "Not Documented by AWS",
+            "condition_keys": [
+                "ec2:Region"
+            ],
+            "description": "Grants permission to describe one or more instances",
             "orphan": false,
             "resources": []
         },
         "DescribeInternetGateways": {
-            "access_level": "Undocumented",
+            "access_level": "List",
             "action": "DescribeInternetGateways",
-            "condition_keys": [],
-            "description": "Not Documented by AWS",
+            "condition_keys": [
+                "ec2:Region"
+            ],
+            "description": "Grants permission to describe one or more internet gateways",
             "orphan": false,
             "resources": []
         },
         "DescribeIpamPools": {
-            "access_level": "Undocumented",
+            "access_level": "List",
             "action": "DescribeIpamPools",
-            "condition_keys": [],
-            "description": "Not Documented by AWS",
+            "condition_keys": [
+                "ec2:Region"
+            ],
+            "description": "Grants permission to describe Amazon VPC IP Address Manager (IPAM) pools",
             "orphan": false,
             "resources": []
         },
         "DescribeIpamResourceDiscoveries": {
-            "access_level": "Undocumented",
+            "access_level": "List",
             "action": "DescribeIpamResourceDiscoveries",
-            "condition_keys": [],
-            "description": "Not Documented by AWS",
+            "condition_keys": [
+                "ec2:Region"
+            ],
+            "description": "Grants permission to describe IPAM resource discoveries",
             "orphan": false,
             "resources": []
         },
         "DescribeIpamResourceDiscoveryAssociations": {
-            "access_level": "Undocumented",
+            "access_level": "List",
             "action": "DescribeIpamResourceDiscoveryAssociations",
-            "condition_keys": [],
-            "description": "Not Documented by AWS",
+            "condition_keys": [
+                "ec2:Region"
+            ],
+            "description": "Grants permission to describe resource discovery associations with an Amazon VPC IPAM",
             "orphan": false,
             "resources": []
         },
         "DescribeIpamScopes": {
-            "access_level": "Undocumented",
+            "access_level": "List",
             "action": "DescribeIpamScopes",
-            "condition_keys": [],
-            "description": "Not Documented by AWS",
+            "condition_keys": [
+                "ec2:Region"
+            ],
+            "description": "Grants permission to describe Amazon VPC IP Address Manager (IPAM) scopes",
             "orphan": false,
             "resources": []
         },
         "DescribeIpams": {
-            "access_level": "Undocumented",
+            "access_level": "List",
             "action": "DescribeIpams",
-            "condition_keys": [],
-            "description": "Not Documented by AWS",
+            "condition_keys": [
+                "ec2:Region"
+            ],
+            "description": "Grants permission to describe an Amazon VPC IP Address Manager (IPAM)",
             "orphan": false,
             "resources": []
         },
         "DescribeIpv6Pools": {
-            "access_level": "Undocumented",
+            "access_level": "List",
             "action": "DescribeIpv6Pools",
-            "condition_keys": [],
-            "description": "Not Documented by AWS",
+            "condition_keys": [
+                "ec2:Region"
+            ],
+            "description": "Grants permission to describe one or more IPv6 address pools",
             "orphan": false,
             "resources": []
         },
         "DescribeKeyPairs": {
-            "access_level": "Undocumented",
+            "access_level": "List",
             "action": "DescribeKeyPairs",
-            "condition_keys": [],
-            "description": "Not Documented by AWS",
+            "condition_keys": [
+                "ec2:Region"
+            ],
+            "description": "Grants permission to describe one or more key pairs",
             "orphan": false,
             "resources": []
         },
         "DescribeLaunchTemplateVersions": {
-            "access_level": "Undocumented",
+            "access_level": "List",
             "action": "DescribeLaunchTemplateVersions",
-            "condition_keys": [],
-            "description": "Not Documented by AWS",
+            "condition_keys": [
+                "ec2:Region"
+            ],
+            "description": "Grants permission to describe one or more launch template versions",
             "orphan": false,
             "resources": []
         },
         "DescribeLaunchTemplates": {
-            "access_level": "Undocumented",
+            "access_level": "List",
             "action": "DescribeLaunchTemplates",
-            "condition_keys": [],
-            "description": "Not Documented by AWS",
+            "condition_keys": [
+                "ec2:Region"
+            ],
+            "description": "Grants permission to describe one or more launch templates",
             "orphan": false,
             "resources": []
         },
         "DescribeLocalGatewayRouteTablePermissions": {
-            "access_level": "Undocumented",
+            "access_level": "List",
             "action": "DescribeLocalGatewayRouteTablePermissions",
-            "condition_keys": [],
-            "description": "Not Documented by AWS",
+            "condition_keys": [
+                "ec2:Region"
+            ],
+            "description": "Grants permission to allow a service to describe local gateway route table permissions",
             "orphan": false,
             "resources": []
         },
         "DescribeLocalGatewayRouteTableVirtualInterfaceGroupAssociations": {
-            "access_level": "Undocumented",
+            "access_level": "List",
             "action": "DescribeLocalGatewayRouteTableVirtualInterfaceGroupAssociations",
-            "condition_keys": [],
-            "description": "Not Documented by AWS",
+            "condition_keys": [
+                "ec2:Region"
+            ],
+            "description": "Grants permission to describe the associations between virtual interface groups and local gateway route tables",
             "orphan": false,
             "resources": []
         },
         "DescribeLocalGatewayRouteTableVpcAssociations": {
-            "access_level": "Undocumented",
+            "access_level": "List",
             "action": "DescribeLocalGatewayRouteTableVpcAssociations",
-            "condition_keys": [],
-            "description": "Not Documented by AWS",
+            "condition_keys": [
+                "ec2:Region"
+            ],
+            "description": "Grants permission to describe an association between VPCs and local gateway route tables",
             "orphan": false,
             "resources": []
         },
         "DescribeLocalGatewayRouteTables": {
-            "access_level": "Undocumented",
+            "access_level": "List",
             "action": "DescribeLocalGatewayRouteTables",
-            "condition_keys": [],
-            "description": "Not Documented by AWS",
+            "condition_keys": [
+                "ec2:Region"
+            ],
+            "description": "Grants permission to describe one or more local gateway route tables",
             "orphan": false,
             "resources": []
         },
         "DescribeLocalGatewayVirtualInterfaceGroups": {
-            "access_level": "Undocumented",
+            "access_level": "List",
             "action": "DescribeLocalGatewayVirtualInterfaceGroups",
-            "condition_keys": [],
-            "description": "Not Documented by AWS",
+            "condition_keys": [
+                "ec2:Region"
+            ],
+            "description": "Grants permission to describe local gateway virtual interface groups",
             "orphan": false,
             "resources": []
         },
         "DescribeLocalGatewayVirtualInterfaces": {
-            "access_level": "Undocumented",
+            "access_level": "List",
             "action": "DescribeLocalGatewayVirtualInterfaces",
-            "condition_keys": [],
-            "description": "Not Documented by AWS",
+            "condition_keys": [
+                "ec2:Region"
+            ],
+            "description": "Grants permission to describe local gateway virtual interfaces",
             "orphan": false,
             "resources": []
         },
         "DescribeLocalGateways": {
-            "access_level": "Undocumented",
+            "access_level": "List",
             "action": "DescribeLocalGateways",
-            "condition_keys": [],
-            "description": "Not Documented by AWS",
+            "condition_keys": [
+                "ec2:Region"
+            ],
+            "description": "Grants permission to describe one or more local gateways",
             "orphan": false,
             "resources": []
         },
         "DescribeManagedPrefixLists": {
-            "access_level": "Undocumented",
+            "access_level": "List",
             "action": "DescribeManagedPrefixLists",
-            "condition_keys": [],
-            "description": "Not Documented by AWS",
+            "condition_keys": [
+                "ec2:Region"
+            ],
+            "description": "Grants permission to describe your managed prefix lists and any AWS-managed prefix lists",
             "orphan": false,
             "resources": []
         },
         "DescribeMovingAddresses": {
-            "access_level": "Undocumented",
+            "access_level": "List",
             "action": "DescribeMovingAddresses",
-            "condition_keys": [],
-            "description": "Not Documented by AWS",
+            "condition_keys": [
+                "ec2:Region"
+            ],
+            "description": "Grants permission to describe Elastic IP addresses that are being moved to the EC2-VPC platform",
             "orphan": false,
             "resources": []
         },
         "DescribeNatGateways": {
-            "access_level": "Undocumented",
+            "access_level": "List",
             "action": "DescribeNatGateways",
-            "condition_keys": [],
-            "description": "Not Documented by AWS",
+            "condition_keys": [
+                "ec2:Region"
+            ],
+            "description": "Grants permission to describe one or more NAT gateways",
             "orphan": false,
             "resources": []
         },
         "DescribeNetworkAcls": {
-            "access_level": "Undocumented",
+            "access_level": "List",
             "action": "DescribeNetworkAcls",
-            "condition_keys": [],
-            "description": "Not Documented by AWS",
+            "condition_keys": [
+                "ec2:Region"
+            ],
+            "description": "Grants permission to describe one or more network ACLs",
             "orphan": false,
             "resources": []
         },
         "DescribeNetworkInsightsAccessScopeAnalyses": {
-            "access_level": "Undocumented",
+            "access_level": "List",
             "action": "DescribeNetworkInsightsAccessScopeAnalyses",
-            "condition_keys": [],
-            "description": "Not Documented by AWS",
+            "condition_keys": [
+                "ec2:Region"
+            ],
+            "description": "Grants permission to describe one or more Network Access Scope analyses",
             "orphan": false,
             "resources": []
         },
         "DescribeNetworkInsightsAccessScopes": {
-            "access_level": "Undocumented",
+            "access_level": "List",
             "action": "DescribeNetworkInsightsAccessScopes",
-            "condition_keys": [],
-            "description": "Not Documented by AWS",
+            "condition_keys": [
+                "ec2:Region"
+            ],
+            "description": "Grants permission to describe the Network Access Scopes",
             "orphan": false,
             "resources": []
         },
         "DescribeNetworkInsightsAnalyses": {
-            "access_level": "Undocumented",
+            "access_level": "List",
             "action": "DescribeNetworkInsightsAnalyses",
-            "condition_keys": [],
-            "description": "Not Documented by AWS",
+            "condition_keys": [
+                "ec2:Region"
+            ],
+            "description": "Grants permission to describe one or more network insights analyses",
             "orphan": false,
             "resources": []
         },
         "DescribeNetworkInsightsPaths": {
-            "access_level": "Undocumented",
+            "access_level": "List",
             "action": "DescribeNetworkInsightsPaths",
-            "condition_keys": [],
-            "description": "Not Documented by AWS",
+            "condition_keys": [
+                "ec2:Region"
+            ],
+            "description": "Grants permission to describe one or more network insights paths",
             "orphan": false,
             "resources": []
         },
         "DescribeNetworkInterfaceAttribute": {
-            "access_level": "Undocumented",
+            "access_level": "List",
             "action": "DescribeNetworkInterfaceAttribute",
-            "condition_keys": [],
-            "description": "Not Documented by AWS",
+            "condition_keys": [
+                "ec2:Region"
+            ],
+            "description": "Grants permission to describe a network interface attribute",
             "orphan": false,
             "resources": []
         },
         "DescribeNetworkInterfacePermissions": {
-            "access_level": "Undocumented",
+            "access_level": "List",
             "action": "DescribeNetworkInterfacePermissions",
-            "condition_keys": [],
-            "description": "Not Documented by AWS",
+            "condition_keys": [
+                "ec2:Region"
+            ],
+            "description": "Grants permission to describe the permissions that are associated with a network interface",
             "orphan": false,
             "resources": []
         },
         "DescribeNetworkInterfaces": {
-            "access_level": "Undocumented",
+            "access_level": "List",
             "action": "DescribeNetworkInterfaces",
-            "condition_keys": [],
-            "description": "Not Documented by AWS",
+            "condition_keys": [
+                "ec2:Region"
+            ],
+            "description": "Grants permission to describe one or more network interfaces",
             "orphan": false,
             "resources": []
         },
         "DescribePlacementGroups": {
-            "access_level": "Undocumented",
+            "access_level": "List",
             "action": "DescribePlacementGroups",
-            "condition_keys": [],
-            "description": "Not Documented by AWS",
+            "condition_keys": [
+                "ec2:Region"
+            ],
+            "description": "Grants permission to describe one or more placement groups",
             "orphan": false,
             "resources": []
         },
         "DescribePrefixLists": {
-            "access_level": "Undocumented",
+            "access_level": "List",
             "action": "DescribePrefixLists",
-            "condition_keys": [],
-            "description": "Not Documented by AWS",
+            "condition_keys": [
+                "ec2:Region"
+            ],
+            "description": "Grants permission to describe available AWS services in a prefix list format",
             "orphan": false,
             "resources": []
         },
         "DescribePrincipalIdFormat": {
-            "access_level": "Undocumented",
+            "access_level": "List",
             "action": "DescribePrincipalIdFormat",
-            "condition_keys": [],
-            "description": "Not Documented by AWS",
+            "condition_keys": [
+                "ec2:Region"
+            ],
+            "description": "Grants permission to describe the ID format settings for the root user and all IAM roles and IAM users that have explicitly specified a longer ID (17-character ID) preference",
             "orphan": false,
             "resources": []
         },
         "DescribePublicIpv4Pools": {
-            "access_level": "Undocumented",
+            "access_level": "List",
             "action": "DescribePublicIpv4Pools",
-            "condition_keys": [],
-            "description": "Not Documented by AWS",
+            "condition_keys": [
+                "ec2:Region"
+            ],
+            "description": "Grants permission to describe one or more IPv4 address pools",
             "orphan": false,
             "resources": []
         },
         "DescribeRegions": {
-            "access_level": "Undocumented",
+            "access_level": "List",
             "action": "DescribeRegions",
-            "condition_keys": [],
-            "description": "Not Documented by AWS",
+            "condition_keys": [
+                "ec2:Region"
+            ],
+            "description": "Grants permission to describe one or more AWS Regions that are currently available in your account",
             "orphan": false,
             "resources": []
         },
         "DescribeReplaceRootVolumeTasks": {
-            "access_level": "Undocumented",
+            "access_level": "List",
             "action": "DescribeReplaceRootVolumeTasks",
-            "condition_keys": [],
-            "description": "Not Documented by AWS",
+            "condition_keys": [
+                "ec2:Region"
+            ],
+            "description": "Grants permission to describe a root volume replacement task",
             "orphan": false,
             "resources": []
         },
         "DescribeReservedInstances": {
-            "access_level": "Undocumented",
+            "access_level": "List",
             "action": "DescribeReservedInstances",
-            "condition_keys": [],
-            "description": "Not Documented by AWS",
+            "condition_keys": [
+                "ec2:Region"
+            ],
+            "description": "Grants permission to describe one or more purchased Reserved Instances in your account",
             "orphan": false,
             "resources": []
         },
         "DescribeReservedInstancesListings": {
-            "access_level": "Undocumented",
+            "access_level": "List",
             "action": "DescribeReservedInstancesListings",
-            "condition_keys": [],
-            "description": "Not Documented by AWS",
+            "condition_keys": [
+                "ec2:Region"
+            ],
+            "description": "Grants permission to describe your account's Reserved Instance listings in the Reserved Instance Marketplace",
             "orphan": false,
             "resources": []
         },
         "DescribeReservedInstancesModifications": {
-            "access_level": "Undocumented",
+            "access_level": "List",
             "action": "DescribeReservedInstancesModifications",
-            "condition_keys": [],
-            "description": "Not Documented by AWS",
+            "condition_keys": [
+                "ec2:Region"
+            ],
+            "description": "Grants permission to describe the modifications made to one or more Reserved Instances",
             "orphan": false,
             "resources": []
         },
         "DescribeReservedInstancesOfferings": {
-            "access_level": "Undocumented",
+            "access_level": "List",
             "action": "DescribeReservedInstancesOfferings",
-            "condition_keys": [],
-            "description": "Not Documented by AWS",
+            "condition_keys": [
+                "ec2:Region"
+            ],
+            "description": "Grants permission to describe the Reserved Instance offerings that are available for purchase",
             "orphan": false,
             "resources": []
         },
         "DescribeRouteTables": {
-            "access_level": "Undocumented",
+            "access_level": "List",
             "action": "DescribeRouteTables",
-            "condition_keys": [],
-            "description": "Not Documented by AWS",
+            "condition_keys": [
+                "ec2:Region"
+            ],
+            "description": "Grants permission to describe one or more route tables",
             "orphan": false,
             "resources": []
         },
         "DescribeScheduledInstanceAvailability": {
-            "access_level": "Undocumented",
+            "access_level": "List",
             "action": "DescribeScheduledInstanceAvailability",
-            "condition_keys": [],
-            "description": "Not Documented by AWS",
+            "condition_keys": [
+                "ec2:Region"
+            ],
+            "description": "Grants permission to find available schedules for Scheduled Instances",
             "orphan": false,
             "resources": []
         },
         "DescribeScheduledInstances": {
-            "access_level": "Undocumented",
+            "access_level": "List",
             "action": "DescribeScheduledInstances",
-            "condition_keys": [],
-            "description": "Not Documented by AWS",
+            "condition_keys": [
+                "ec2:Region"
+            ],
+            "description": "Grants permission to describe one or more Scheduled Instances in your account",
             "orphan": false,
             "resources": []
         },
         "DescribeSecurityGroupReferences": {
-            "access_level": "Undocumented",
+            "access_level": "List",
             "action": "DescribeSecurityGroupReferences",
-            "condition_keys": [],
-            "description": "Not Documented by AWS",
+            "condition_keys": [
+                "ec2:Region"
+            ],
+            "description": "Grants permission to describe the VPCs on the other side of a VPC peering connection that are referencing specified VPC security groups",
             "orphan": false,
             "resources": []
         },
         "DescribeSecurityGroupRules": {
-            "access_level": "Undocumented",
+            "access_level": "List",
             "action": "DescribeSecurityGroupRules",
-            "condition_keys": [],
-            "description": "Not Documented by AWS",
+            "condition_keys": [
+                "ec2:Region"
+            ],
+            "description": "Grants permission to describe one or more of your security group rules",
             "orphan": false,
             "resources": []
         },
         "DescribeSecurityGroups": {
-            "access_level": "Undocumented",
+            "access_level": "List",
             "action": "DescribeSecurityGroups",
-            "condition_keys": [],
-            "description": "Not Documented by AWS",
+            "condition_keys": [
+                "ec2:Region"
+            ],
+            "description": "Grants permission to describe one or more security groups",
             "orphan": false,
             "resources": []
         },
         "DescribeSnapshotAttribute": {
-            "access_level": "Undocumented",
+            "access_level": "List",
             "action": "DescribeSnapshotAttribute",
-            "condition_keys": [],
-            "description": "Not Documented by AWS",
+            "condition_keys": [
+                "aws:ResourceTag/${TagKey}",
+                "ec2:Encrypted",
+                "ec2:OutpostArn",
+                "ec2:Owner",
+                "ec2:ParentVolume",
+                "ec2:Region",
+                "ec2:ResourceTag/${TagKey}",
+                "ec2:SnapshotID",
+                "ec2:SnapshotTime",
+                "ec2:SourceOutpostArn",
+                "ec2:VolumeSize"
+            ],
+            "description": "Grants permission to describe an attribute of a snapshot",
             "orphan": false,
-            "resources": []
+            "resources": [
+                "snapshot"
+            ]
         },
         "DescribeSnapshotTierStatus": {
-            "access_level": "Undocumented",
+            "access_level": "List",
             "action": "DescribeSnapshotTierStatus",
-            "condition_keys": [],
-            "description": "Not Documented by AWS",
+            "condition_keys": [
+                "ec2:Region"
+            ],
+            "description": "Grants permission to describe the storage tier status for Amazon EBS snapshots",
             "orphan": false,
             "resources": []
         },
         "DescribeSnapshots": {
-            "access_level": "Undocumented",
+            "access_level": "List",
             "action": "DescribeSnapshots",
-            "condition_keys": [],
-            "description": "Not Documented by AWS",
+            "condition_keys": [
+                "ec2:Region"
+            ],
+            "description": "Grants permission to describe one or more EBS snapshots",
             "orphan": false,
             "resources": []
         },
         "DescribeSpotDatafeedSubscription": {
-            "access_level": "Undocumented",
+            "access_level": "List",
             "action": "DescribeSpotDatafeedSubscription",
-            "condition_keys": [],
-            "description": "Not Documented by AWS",
+            "condition_keys": [
+                "ec2:Region"
+            ],
+            "description": "Grants permission to describe the data feed for Spot Instances",
             "orphan": false,
             "resources": []
         },
         "DescribeSpotFleetInstances": {
-            "access_level": "Undocumented",
+            "access_level": "List",
             "action": "DescribeSpotFleetInstances",
-            "condition_keys": [],
-            "description": "Not Documented by AWS",
+            "condition_keys": [
+                "aws:ResourceTag/${TagKey}",
+                "ec2:Region",
+                "ec2:ResourceTag/${TagKey}"
+            ],
+            "description": "Grants permission to describe the running instances for a Spot Fleet",
             "orphan": false,
-            "resources": []
+            "resources": [
+                "spot-fleet-request"
+            ]
         },
         "DescribeSpotFleetRequestHistory": {
-            "access_level": "Undocumented",
+            "access_level": "List",
             "action": "DescribeSpotFleetRequestHistory",
-            "condition_keys": [],
-            "description": "Not Documented by AWS",
+            "condition_keys": [
+                "aws:ResourceTag/${TagKey}",
+                "ec2:Region",
+                "ec2:ResourceTag/${TagKey}"
+            ],
+            "description": "Grants permission to describe the events for a Spot Fleet request during a specified time",
             "orphan": false,
-            "resources": []
+            "resources": [
+                "spot-fleet-request"
+            ]
         },
         "DescribeSpotFleetRequests": {
-            "access_level": "Undocumented",
+            "access_level": "List",
             "action": "DescribeSpotFleetRequests",
-            "condition_keys": [],
-            "description": "Not Documented by AWS",
+            "condition_keys": [
+                "ec2:Region"
+            ],
+            "description": "Grants permission to describe one or more Spot Fleet requests",
             "orphan": false,
             "resources": []
         },
         "DescribeSpotInstanceRequests": {
-            "access_level": "Undocumented",
+            "access_level": "List",
             "action": "DescribeSpotInstanceRequests",
-            "condition_keys": [],
-            "description": "Not Documented by AWS",
+            "condition_keys": [
+                "ec2:Region"
+            ],
+            "description": "Grants permission to describe one or more Spot Instance requests",
             "orphan": false,
             "resources": []
         },
         "DescribeSpotPriceHistory": {
-            "access_level": "Undocumented",
+            "access_level": "List",
             "action": "DescribeSpotPriceHistory",
-            "condition_keys": [],
-            "description": "Not Documented by AWS",
+            "condition_keys": [
+                "ec2:Region"
+            ],
+            "description": "Grants permission to describe the Spot Instance price history",
             "orphan": false,
             "resources": []
         },
         "DescribeStaleSecurityGroups": {
-            "access_level": "Undocumented",
+            "access_level": "List",
             "action": "DescribeStaleSecurityGroups",
-            "condition_keys": [],
-            "description": "Not Documented by AWS",
+            "condition_keys": [
+                "ec2:Region"
+            ],
+            "description": "Grants permission to describe the stale security group rules for security groups in a specified VPC",
             "orphan": false,
             "resources": []
         },
         "DescribeStoreImageTasks": {
-            "access_level": "Undocumented",
+            "access_level": "List",
             "action": "DescribeStoreImageTasks",
-            "condition_keys": [],
-            "description": "Not Documented by AWS",
+            "condition_keys": [
+                "ec2:Region"
+            ],
+            "description": "Grants permission to describe the progress of the AMI store tasks",
             "orphan": false,
             "resources": []
         },
         "DescribeSubnets": {
-            "access_level": "Undocumented",
+            "access_level": "List",
             "action": "DescribeSubnets",
-            "condition_keys": [],
-            "description": "Not Documented by AWS",
+            "condition_keys": [
+                "ec2:Region"
+            ],
+            "description": "Grants permission to describe one or more subnets",
             "orphan": false,
             "resources": []
         },
         "DescribeTags": {
-            "access_level": "Undocumented",
+            "access_level": "List",
             "action": "DescribeTags",
-            "condition_keys": [],
-            "description": "Not Documented by AWS",
+            "condition_keys": [
+                "ec2:Region"
+            ],
+            "description": "Grants permission to describe one or more tags for an Amazon EC2 resource",
             "orphan": false,
             "resources": []
         },
         "DescribeTrafficMirrorFilters": {
-            "access_level": "Undocumented",
+            "access_level": "List",
             "action": "DescribeTrafficMirrorFilters",
-            "condition_keys": [],
-            "description": "Not Documented by AWS",
+            "condition_keys": [
+                "ec2:Region"
+            ],
+            "description": "Grants permission to describe one or more traffic mirror filters",
             "orphan": false,
             "resources": []
         },
         "DescribeTrafficMirrorSessions": {
-            "access_level": "Undocumented",
+            "access_level": "List",
             "action": "DescribeTrafficMirrorSessions",
-            "condition_keys": [],
-            "description": "Not Documented by AWS",
+            "condition_keys": [
+                "ec2:Region"
+            ],
+            "description": "Grants permission to describe one or more traffic mirror sessions",
             "orphan": false,
             "resources": []
         },
         "DescribeTrafficMirrorTargets": {
-            "access_level": "Undocumented",
+            "access_level": "List",
             "action": "DescribeTrafficMirrorTargets",
-            "condition_keys": [],
-            "description": "Not Documented by AWS",
+            "condition_keys": [
+                "ec2:Region"
+            ],
+            "description": "Grants permission to describe one or more traffic mirror targets",
             "orphan": false,
             "resources": []
         },
         "DescribeTransitGatewayAttachments": {
-            "access_level": "Undocumented",
+            "access_level": "List",
             "action": "DescribeTransitGatewayAttachments",
-            "condition_keys": [],
-            "description": "Not Documented by AWS",
+            "condition_keys": [
+                "ec2:Region"
+            ],
+            "description": "Grants permission to describe one or more attachments between resources and transit gateways",
             "orphan": false,
             "resources": []
         },
         "DescribeTransitGatewayConnectPeers": {
-            "access_level": "Undocumented",
+            "access_level": "List",
             "action": "DescribeTransitGatewayConnectPeers",
-            "condition_keys": [],
-            "description": "Not Documented by AWS",
+            "condition_keys": [
+                "ec2:Region"
+            ],
+            "description": "Grants permission to describe one or more transit gateway connect peers",
             "orphan": false,
             "resources": []
         },
         "DescribeTransitGatewayConnects": {
-            "access_level": "Undocumented",
+            "access_level": "List",
             "action": "DescribeTransitGatewayConnects",
-            "condition_keys": [],
-            "description": "Not Documented by AWS",
+            "condition_keys": [
+                "ec2:Region"
+            ],
+            "description": "Grants permission to describe one or more transit gateway connect attachments",
             "orphan": false,
             "resources": []
         },
         "DescribeTransitGatewayMulticastDomains": {
-            "access_level": "Undocumented",
+            "access_level": "List",
             "action": "DescribeTransitGatewayMulticastDomains",
-            "condition_keys": [],
-            "description": "Not Documented by AWS",
+            "condition_keys": [
+                "ec2:Region"
+            ],
+            "description": "Grants permission to describe one or more transit gateway multicast domains",
             "orphan": false,
             "resources": []
         },
         "DescribeTransitGatewayPeeringAttachments": {
-            "access_level": "Undocumented",
+            "access_level": "List",
             "action": "DescribeTransitGatewayPeeringAttachments",
-            "condition_keys": [],
-            "description": "Not Documented by AWS",
+            "condition_keys": [
+                "ec2:Region"
+            ],
+            "description": "Grants permission to describe one or more transit gateway peering attachments",
             "orphan": false,
             "resources": []
         },
         "DescribeTransitGatewayPolicyTables": {
-            "access_level": "Undocumented",
+            "access_level": "List",
             "action": "DescribeTransitGatewayPolicyTables",
-            "condition_keys": [],
-            "description": "Not Documented by AWS",
+            "condition_keys": [
+                "ec2:Region"
+            ],
+            "description": "Grants permission to describe a transit gateway policy table",
             "orphan": false,
             "resources": []
         },
         "DescribeTransitGatewayRouteTableAnnouncements": {
-            "access_level": "Undocumented",
+            "access_level": "List",
             "action": "DescribeTransitGatewayRouteTableAnnouncements",
-            "condition_keys": [],
-            "description": "Not Documented by AWS",
+            "condition_keys": [
+                "ec2:Region"
+            ],
+            "description": "Grants permission to describe a transit gateway route table announcement",
             "orphan": false,
             "resources": []
         },
         "DescribeTransitGatewayRouteTables": {
-            "access_level": "Undocumented",
+            "access_level": "List",
             "action": "DescribeTransitGatewayRouteTables",
-            "condition_keys": [],
-            "description": "Not Documented by AWS",
+            "condition_keys": [
+                "ec2:Region"
+            ],
+            "description": "Grants permission to describe one or more transit gateway route tables",
             "orphan": false,
             "resources": []
         },
         "DescribeTransitGatewayVpcAttachments": {
-            "access_level": "Undocumented",
+            "access_level": "List",
             "action": "DescribeTransitGatewayVpcAttachments",
-            "condition_keys": [],
-            "description": "Not Documented by AWS",
+            "condition_keys": [
+                "ec2:Region"
+            ],
+            "description": "Grants permission to describe one or more VPC attachments on a transit gateway",
             "orphan": false,
             "resources": []
         },
         "DescribeTransitGateways": {
-            "access_level": "Undocumented",
+            "access_level": "List",
             "action": "DescribeTransitGateways",
-            "condition_keys": [],
-            "description": "Not Documented by AWS",
+            "condition_keys": [
+                "ec2:Region"
+            ],
+            "description": "Grants permission to describe one or more transit gateways",
             "orphan": false,
             "resources": []
         },
         "DescribeTrunkInterfaceAssociations": {
-            "access_level": "Undocumented",
+            "access_level": "List",
             "action": "DescribeTrunkInterfaceAssociations",
-            "condition_keys": [],
-            "description": "Not Documented by AWS",
+            "condition_keys": [
+                "ec2:Region"
+            ],
+            "description": "Grants permission to describe one or more network interface trunk associations",
             "orphan": false,
             "resources": []
         },
         "DescribeVerifiedAccessEndpoints": {
-            "access_level": "Undocumented",
+            "access_level": "List",
             "action": "DescribeVerifiedAccessEndpoints",
-            "condition_keys": [],
-            "description": "Not Documented by AWS",
+            "condition_keys": [
+                "ec2:Region"
+            ],
+            "description": "Grants permission to describe the specified Verified Access endpoints or all Verified Access endpoints",
             "orphan": false,
             "resources": []
         },
         "DescribeVerifiedAccessGroups": {
-            "access_level": "Undocumented",
+            "access_level": "List",
             "action": "DescribeVerifiedAccessGroups",
-            "condition_keys": [],
-            "description": "Not Documented by AWS",
+            "condition_keys": [
+                "ec2:Region"
+            ],
+            "description": "Grants permission to describe the specified Verified Access groups or all Verified Access groups",
             "orphan": false,
             "resources": []
         },
         "DescribeVerifiedAccessInstanceLoggingConfigurations": {
-            "access_level": "Undocumented",
+            "access_level": "List",
             "action": "DescribeVerifiedAccessInstanceLoggingConfigurations",
-            "condition_keys": [],
-            "description": "Not Documented by AWS",
+            "condition_keys": [
+                "ec2:Region"
+            ],
+            "description": "Grants permission to describe the current logging configuration for the Verified Access instances",
             "orphan": false,
             "resources": []
         },
         "DescribeVerifiedAccessInstanceWebAclAssociations": {
-            "access_level": "Undocumented",
+            "access_level": "List",
             "action": "DescribeVerifiedAccessInstanceWebAclAssociations",
-            "condition_keys": [],
-            "description": "Not Documented by AWS",
+            "condition_keys": [
+                "ec2:Region"
+            ],
+            "description": "Grants permission to describe the AWS Web Application Firewall (WAF) web access control list (ACL) associations for a Verified Access instance",
             "orphan": false,
             "resources": []
         },
         "DescribeVerifiedAccessInstances": {
-            "access_level": "Undocumented",
+            "access_level": "List",
             "action": "DescribeVerifiedAccessInstances",
-            "condition_keys": [],
-            "description": "Not Documented by AWS",
+            "condition_keys": [
+                "ec2:Region"
+            ],
+            "description": "Grants permission to describe the specified Verified Access instances or all Verified Access instances",
             "orphan": false,
             "resources": []
         },
         "DescribeVerifiedAccessTrustProviders": {
-            "access_level": "Undocumented",
+            "access_level": "List",
             "action": "DescribeVerifiedAccessTrustProviders",
-            "condition_keys": [],
-            "description": "Not Documented by AWS",
+            "condition_keys": [
+                "ec2:Region"
+            ],
+            "description": "Grants permission to describe details of existing Verified Access trust providers",
             "orphan": false,
             "resources": []
         },
         "DescribeVolumeAttribute": {
-            "access_level": "Undocumented",
+            "access_level": "List",
             "action": "DescribeVolumeAttribute",
-            "condition_keys": [],
-            "description": "Not Documented by AWS",
+            "condition_keys": [
+                "aws:ResourceTag/${TagKey}",
+                "ec2:AvailabilityZone",
+                "ec2:Encrypted",
+                "ec2:ParentSnapshot",
+                "ec2:Region",
+                "ec2:ResourceTag/${TagKey}",
+                "ec2:VolumeID",
+                "ec2:VolumeIops",
+                "ec2:VolumeSize",
+                "ec2:VolumeThroughput",
+                "ec2:VolumeType"
+            ],
+            "description": "Grants permission to describe an attribute of an EBS volume",
             "orphan": false,
-            "resources": []
+            "resources": [
+                "volume"
+            ]
         },
         "DescribeVolumeStatus": {
-            "access_level": "Undocumented",
+            "access_level": "List",
             "action": "DescribeVolumeStatus",
-            "condition_keys": [],
-            "description": "Not Documented by AWS",
+            "condition_keys": [
+                "ec2:Region"
+            ],
+            "description": "Grants permission to describe the status of one or more EBS volumes",
             "orphan": false,
             "resources": []
         },
         "DescribeVolumes": {
-            "access_level": "Undocumented",
+            "access_level": "List",
             "action": "DescribeVolumes",
-            "condition_keys": [],
-            "description": "Not Documented by AWS",
+            "condition_keys": [
+                "ec2:Region"
+            ],
+            "description": "Grants permission to describe one or more EBS volumes",
             "orphan": false,
             "resources": []
         },
         "DescribeVolumesModifications": {
-            "access_level": "Undocumented",
+            "access_level": "List",
             "action": "DescribeVolumesModifications",
-            "condition_keys": [],
-            "description": "Not Documented by AWS",
+            "condition_keys": [
+                "ec2:Region"
+            ],
+            "description": "Grants permission to describe the current modification status of one or more EBS volumes",
             "orphan": false,
             "resources": []
         },
         "DescribeVpcAttribute": {
-            "access_level": "Undocumented",
+            "access_level": "List",
             "action": "DescribeVpcAttribute",
-            "condition_keys": [],
-            "description": "Not Documented by AWS",
+            "condition_keys": [
+                "aws:ResourceTag/${TagKey}",
+                "ec2:Region",
+                "ec2:ResourceTag/${TagKey}",
+                "ec2:Tenancy",
+                "ec2:VpcID"
+            ],
+            "description": "Grants permission to describe an attribute of a VPC",
             "orphan": false,
-            "resources": []
+            "resources": [
+                "vpc"
+            ]
         },
         "DescribeVpcClassicLink": {
-            "access_level": "Undocumented",
+            "access_level": "List",
             "action": "DescribeVpcClassicLink",
-            "condition_keys": [],
-            "description": "Not Documented by AWS",
+            "condition_keys": [
+                "ec2:Region"
+            ],
+            "description": "Grants permission to describe the ClassicLink status of one or more VPCs",
             "orphan": false,
             "resources": []
         },
         "DescribeVpcClassicLinkDnsSupport": {
-            "access_level": "Undocumented",
+            "access_level": "List",
             "action": "DescribeVpcClassicLinkDnsSupport",
-            "condition_keys": [],
-            "description": "Not Documented by AWS",
+            "condition_keys": [
+                "ec2:Region"
+            ],
+            "description": "Grants permission to describe the ClassicLink DNS support status of one or more VPCs",
             "orphan": false,
             "resources": []
         },
         "DescribeVpcEndpointConnectionNotifications": {
-            "access_level": "Undocumented",
+            "access_level": "List",
             "action": "DescribeVpcEndpointConnectionNotifications",
-            "condition_keys": [],
-            "description": "Not Documented by AWS",
+            "condition_keys": [
+                "ec2:Region"
+            ],
+            "description": "Grants permission to describe the connection notifications for VPC endpoints and VPC endpoint services",
             "orphan": false,
             "resources": []
         },
         "DescribeVpcEndpointConnections": {
-            "access_level": "Undocumented",
+            "access_level": "List",
             "action": "DescribeVpcEndpointConnections",
-            "condition_keys": [],
-            "description": "Not Documented by AWS",
+            "condition_keys": [
+                "ec2:Region"
+            ],
+            "description": "Grants permission to describe the VPC endpoint connections to your VPC endpoint services",
             "orphan": false,
             "resources": []
         },
         "DescribeVpcEndpointServiceConfigurations": {
-            "access_level": "Undocumented",
+            "access_level": "List",
             "action": "DescribeVpcEndpointServiceConfigurations",
-            "condition_keys": [],
-            "description": "Not Documented by AWS",
+            "condition_keys": [
+                "ec2:Region"
+            ],
+            "description": "Grants permission to describe VPC endpoint service configurations (your services)",
             "orphan": false,
             "resources": []
         },
         "DescribeVpcEndpointServicePermissions": {
-            "access_level": "Undocumented",
+            "access_level": "List",
             "action": "DescribeVpcEndpointServicePermissions",
-            "condition_keys": [],
-            "description": "Not Documented by AWS",
+            "condition_keys": [
+                "aws:ResourceTag/${TagKey}",
+                "ec2:Region",
+                "ec2:ResourceTag/${TagKey}"
+            ],
+            "description": "Grants permission to describe the principals (service consumers) that are permitted to discover your VPC endpoint service",
             "orphan": false,
-            "resources": []
+            "resources": [
+                "vpc-endpoint-service"
+            ]
         },
         "DescribeVpcEndpointServices": {
-            "access_level": "Undocumented",
+            "access_level": "List",
             "action": "DescribeVpcEndpointServices",
-            "condition_keys": [],
-            "description": "Not Documented by AWS",
+            "condition_keys": [
+                "ec2:Region"
+            ],
+            "description": "Grants permission to describe all supported AWS services that can be specified when creating a VPC endpoint",
             "orphan": false,
             "resources": []
         },
         "DescribeVpcEndpoints": {
-            "access_level": "Undocumented",
+            "access_level": "List",
             "action": "DescribeVpcEndpoints",
-            "condition_keys": [],
-            "description": "Not Documented by AWS",
+            "condition_keys": [
+                "ec2:Region"
+            ],
+            "description": "Grants permission to describe one or more VPC endpoints",
             "orphan": false,
             "resources": []
         },
         "DescribeVpcPeeringConnections": {
-            "access_level": "Undocumented",
+            "access_level": "List",
             "action": "DescribeVpcPeeringConnections",
-            "condition_keys": [],
-            "description": "Not Documented by AWS",
+            "condition_keys": [
+                "ec2:Region"
+            ],
+            "description": "Grants permission to describe one or more VPC peering connections",
             "orphan": false,
             "resources": []
         },
         "DescribeVpcs": {
-            "access_level": "Undocumented",
+            "access_level": "List",
             "action": "DescribeVpcs",
-            "condition_keys": [],
-            "description": "Not Documented by AWS",
+            "condition_keys": [
+                "ec2:Region"
+            ],
+            "description": "Grants permission to describe one or more VPCs",
             "orphan": false,
             "resources": []
         },
         "DescribeVpnConnections": {
-            "access_level": "Undocumented",
+            "access_level": "List",
             "action": "DescribeVpnConnections",
-            "condition_keys": [],
-            "description": "Not Documented by AWS",
+            "condition_keys": [
+                "ec2:Region"
+            ],
+            "description": "Grants permission to describe one or more VPN connections",
             "orphan": false,
             "resources": []
         },
         "DescribeVpnGateways": {
-            "access_level": "Undocumented",
+            "access_level": "List",
             "action": "DescribeVpnGateways",
-            "condition_keys": [],
-            "description": "Not Documented by AWS",
+            "condition_keys": [
+                "ec2:Region"
+            ],
+            "description": "Grants permission to describe one or more virtual private gateways",
             "orphan": false,
             "resources": []
         },
         "DetachClassicLinkVpc": {
-            "access_level": "Undocumented",
+            "access_level": "Write",
             "action": "DetachClassicLinkVpc",
-            "condition_keys": [],
-            "description": "Not Documented by AWS",
+            "condition_keys": [
+                "aws:ResourceTag/${TagKey}",
+                "ec2:AvailabilityZone",
+                "ec2:EbsOptimized",
+                "ec2:InstanceID",
+                "ec2:InstanceMarketType",
+                "ec2:InstanceProfile",
+                "ec2:InstanceType",
+                "ec2:MetadataHttpEndpoint",
+                "ec2:MetadataHttpPutResponseHopLimit",
+                "ec2:MetadataHttpTokens",
+                "ec2:PlacementGroup",
+                "ec2:Region",
+                "ec2:ResourceTag/${TagKey}",
+                "ec2:RootDeviceType",
+                "ec2:Tenancy",
+                "ec2:VpcID"
+            ],
+            "description": "Grants permission to unlink (detach) a linked EC2-Classic instance from a VPC",
             "orphan": false,
-            "resources": []
+            "resources": [
+                "instance",
+                "vpc"
+            ]
         },
         "DetachInternetGateway": {
-            "access_level": "Undocumented",
+            "access_level": "Write",
             "action": "DetachInternetGateway",
-            "condition_keys": [],
-            "description": "Not Documented by AWS",
+            "condition_keys": [
+                "aws:ResourceTag/${TagKey}",
+                "ec2:InternetGatewayID",
+                "ec2:Region",
+                "ec2:ResourceTag/${TagKey}",
+                "ec2:Tenancy",
+                "ec2:VpcID"
+            ],
+            "description": "Grants permission to detach an internet gateway from a VPC",
             "orphan": false,
-            "resources": []
+            "resources": [
+                "internet-gateway",
+                "vpc"
+            ]
         },
         "DetachNetworkInterface": {
-            "access_level": "Undocumented",
+            "access_level": "Write",
             "action": "DetachNetworkInterface",
-            "condition_keys": [],
-            "description": "Not Documented by AWS",
+            "condition_keys": [
+                "aws:ResourceTag/${TagKey}",
+                "ec2:AvailabilityZone",
+                "ec2:EbsOptimized",
+                "ec2:InstanceAutoRecovery",
+                "ec2:InstanceID",
+                "ec2:InstanceMarketType",
+                "ec2:InstanceMetadataTags",
+                "ec2:InstanceProfile",
+                "ec2:InstanceType",
+                "ec2:MetadataHttpEndpoint",
+                "ec2:MetadataHttpPutResponseHopLimit",
+                "ec2:MetadataHttpTokens",
+                "ec2:NetworkInterfaceID",
+                "ec2:PlacementGroup",
+                "ec2:ProductCode",
+                "ec2:Region",
+                "ec2:ResourceTag/${TagKey}",
+                "ec2:RootDeviceType",
+                "ec2:Subnet",
+                "ec2:Tenancy",
+                "ec2:Vpc"
+            ],
+            "description": "Grants permission to detach a network interface from an instance",
             "orphan": false,
-            "resources": []
+            "resources": [
+                "instance",
+                "network-interface"
+            ]
         },
         "DetachVerifiedAccessTrustProvider": {
-            "access_level": "Undocumented",
+            "access_level": "Write",
             "action": "DetachVerifiedAccessTrustProvider",
-            "condition_keys": [],
-            "description": "Not Documented by AWS",
+            "condition_keys": [
+                "aws:ResourceTag/${TagKey}",
+                "ec2:Region",
+                "ec2:ResourceTag/${TagKey}"
+            ],
+            "description": "Grants permission to detach a trust provider from a Verified Access instance",
             "orphan": false,
-            "resources": []
+            "resources": [
+                "verified-access-instance",
+                "verified-access-trust-provider"
+            ]
         },
         "DetachVolume": {
-            "access_level": "Undocumented",
+            "access_level": "Write",
             "action": "DetachVolume",
-            "condition_keys": [],
-            "description": "Not Documented by AWS",
+            "condition_keys": [
+                "aws:ResourceTag/${TagKey}",
+                "ec2:AvailabilityZone",
+                "ec2:EbsOptimized",
+                "ec2:Encrypted",
+                "ec2:InstanceID",
+                "ec2:InstanceMarketType",
+                "ec2:InstanceProfile",
+                "ec2:InstanceType",
+                "ec2:MetadataHttpEndpoint",
+                "ec2:MetadataHttpPutResponseHopLimit",
+                "ec2:MetadataHttpTokens",
+                "ec2:ParentSnapshot",
+                "ec2:PlacementGroup",
+                "ec2:ProductCode",
+                "ec2:Region",
+                "ec2:ResourceTag/${TagKey}",
+                "ec2:RootDeviceType",
+                "ec2:Tenancy",
+                "ec2:VolumeID",
+                "ec2:VolumeIops",
+                "ec2:VolumeSize",
+                "ec2:VolumeThroughput",
+                "ec2:VolumeType"
+            ],
+            "description": "Grants permission to detach an EBS volume from an instance",
             "orphan": false,
-            "resources": []
+            "resources": [
+                "instance",
+                "volume"
+            ]
         },
         "DetachVpnGateway": {
-            "access_level": "Undocumented",
+            "access_level": "Write",
             "action": "DetachVpnGateway",
-            "condition_keys": [],
-            "description": "Not Documented by AWS",
+            "condition_keys": [
+                "aws:ResourceTag/${TagKey}",
+                "ec2:Region",
+                "ec2:ResourceTag/${TagKey}",
+                "ec2:Tenancy",
+                "ec2:VpcID"
+            ],
+            "description": "Grants permission to detach a virtual private gateway from a VPC",
             "orphan": false,
-            "resources": []
+            "resources": [
+                "vpc",
+                "vpn-gateway"
+            ]
         },
         "DisableAddressTransfer": {
-            "access_level": "Undocumented",
+            "access_level": "Write",
             "action": "DisableAddressTransfer",
-            "condition_keys": [],
-            "description": "Not Documented by AWS",
+            "condition_keys": [
+                "aws:ResourceTag/${TagKey}",
+                "ec2:AllocationId",
+                "ec2:Domain",
+                "ec2:PublicIpAddress",
+                "ec2:Region",
+                "ec2:ResourceTag/${TagKey}"
+            ],
+            "description": "Grants permission to disable Elastic IP address transfer",
             "orphan": false,
-            "resources": []
+            "resources": [
+                "elastic-ip"
+            ]
         },
         "DisableAwsNetworkPerformanceMetricSubscription": {
-            "access_level": "Undocumented",
+            "access_level": "Write",
             "action": "DisableAwsNetworkPerformanceMetricSubscription",
-            "condition_keys": [],
-            "description": "Not Documented by AWS",
+            "condition_keys": [
+                "ec2:Region"
+            ],
+            "description": "Grants permission to disable infrastructure performance metric subscriptions",
             "orphan": false,
             "resources": []
         },
         "DisableEbsEncryptionByDefault": {
-            "access_level": "Undocumented",
+            "access_level": "Write",
             "action": "DisableEbsEncryptionByDefault",
-            "condition_keys": [],
-            "description": "Not Documented by AWS",
+            "condition_keys": [
+                "ec2:Region"
+            ],
+            "description": "Grants permission to disable EBS encryption by default for your account",
             "orphan": false,
             "resources": []
         },
         "DisableFastLaunch": {
-            "access_level": "Undocumented",
+            "access_level": "Write",
             "action": "DisableFastLaunch",
-            "condition_keys": [],
-            "description": "Not Documented by AWS",
+            "condition_keys": [
+                "aws:ResourceTag/${TagKey}",
+                "ec2:ImageID",
+                "ec2:ImageType",
+                "ec2:Owner",
+                "ec2:Public",
+                "ec2:Region",
+                "ec2:ResourceTag/${TagKey}",
+                "ec2:RootDeviceType"
+            ],
+            "description": "Grants permission to disable faster launching for Windows AMIs",
             "orphan": false,
-            "resources": []
+            "resources": [
+                "image"
+            ]
         },
         "DisableFastSnapshotRestores": {
-            "access_level": "Undocumented",
+            "access_level": "Write",
             "action": "DisableFastSnapshotRestores",
-            "condition_keys": [],
-            "description": "Not Documented by AWS",
+            "condition_keys": [
+                "aws:ResourceTag/${TagKey}",
+                "ec2:AvailabilityZone",
+                "ec2:Encrypted",
+                "ec2:Owner",
+                "ec2:ParentVolume",
+                "ec2:Region",
+                "ec2:ResourceTag/${TagKey}",
+                "ec2:SnapshotID",
+                "ec2:SnapshotTime",
+                "ec2:VolumeSize"
+            ],
+            "description": "Grants permission to disable fast snapshot restores for one or more snapshots in specified Availability Zones",
             "orphan": false,
-            "resources": []
+            "resources": [
+                "snapshot"
+            ]
         },
         "DisableImageDeprecation": {
-            "access_level": "Undocumented",
+            "access_level": "Write",
             "action": "DisableImageDeprecation",
-            "condition_keys": [],
-            "description": "Not Documented by AWS",
+            "condition_keys": [
+                "aws:ResourceTag/${TagKey}",
+                "ec2:ImageID",
+                "ec2:ImageType",
+                "ec2:Owner",
+                "ec2:Public",
+                "ec2:Region",
+                "ec2:ResourceTag/${TagKey}",
+                "ec2:RootDeviceType"
+            ],
+            "description": "Grants permission to cancel the deprecation of the specified AMI",
             "orphan": false,
-            "resources": []
+            "resources": [
+                "image"
+            ]
         },
         "DisableIpamOrganizationAdminAccount": {
-            "access_level": "Undocumented",
+            "access_level": "Write",
             "action": "DisableIpamOrganizationAdminAccount",
-            "condition_keys": [],
-            "description": "Not Documented by AWS",
+            "condition_keys": [
+                "ec2:Region"
+            ],
+            "description": "Grants permission to disable an AWS Organizations member account as an Amazon VPC IP Address Manager (IPAM) admin account",
             "orphan": false,
             "resources": []
         },
         "DisableSerialConsoleAccess": {
-            "access_level": "Undocumented",
+            "access_level": "Write",
             "action": "DisableSerialConsoleAccess",
-            "condition_keys": [],
-            "description": "Not Documented by AWS",
+            "condition_keys": [
+                "ec2:Region"
+            ],
+            "description": "Grants permission to disable access to the EC2 serial console of all instances for your account",
             "orphan": false,
             "resources": []
         },
         "DisableTransitGatewayRouteTablePropagation": {
-            "access_level": "Undocumented",
+            "access_level": "Write",
             "action": "DisableTransitGatewayRouteTablePropagation",
-            "condition_keys": [],
-            "description": "Not Documented by AWS",
+            "condition_keys": [
+                "aws:ResourceTag/${TagKey}",
+                "ec2:Region",
+                "ec2:ResourceTag/${TagKey}"
+            ],
+            "description": "Grants permission to disable a resource attachment from propagating routes to the specified propagation route table",
             "orphan": false,
-            "resources": []
+            "resources": [
+                "transit-gateway-attachment",
+                "transit-gateway-route-table",
+                "transit-gateway-route-table-announcement"
+            ]
         },
         "DisableVgwRoutePropagation": {
-            "access_level": "Undocumented",
+            "access_level": "Write",
             "action": "DisableVgwRoutePropagation",
-            "condition_keys": [],
-            "description": "Not Documented by AWS",
+            "condition_keys": [
+                "aws:ResourceTag/${TagKey}",
+                "ec2:Region",
+                "ec2:ResourceTag/${TagKey}",
+                "ec2:RouteTableID",
+                "ec2:Vpc"
+            ],
+            "description": "Grants permission to disable a virtual private gateway from propagating routes to a specified route table of a VPC",
             "orphan": false,
-            "resources": []
+            "resources": [
+                "route-table",
+                "vpn-gateway"
+            ]
         },
         "DisableVpcClassicLink": {
-            "access_level": "Undocumented",
+            "access_level": "Write",
             "action": "DisableVpcClassicLink",
-            "condition_keys": [],
-            "description": "Not Documented by AWS",
+            "condition_keys": [
+                "aws:ResourceTag/${TagKey}",
+                "ec2:Region",
+                "ec2:ResourceTag/${TagKey}",
+                "ec2:Tenancy",
+                "ec2:VpcID"
+            ],
+            "description": "Grants permission to disable ClassicLink for a VPC",
             "orphan": false,
-            "resources": []
+            "resources": [
+                "vpc"
+            ]
         },
         "DisableVpcClassicLinkDnsSupport": {
-            "access_level": "Undocumented",
+            "access_level": "Write",
             "action": "DisableVpcClassicLinkDnsSupport",
-            "condition_keys": [],
-            "description": "Not Documented by AWS",
+            "condition_keys": [
+                "aws:ResourceTag/${TagKey}",
+                "ec2:Region",
+                "ec2:ResourceTag/${TagKey}",
+                "ec2:Tenancy",
+                "ec2:VpcID"
+            ],
+            "description": "Grants permission to disable ClassicLink DNS support for a VPC",
             "orphan": false,
-            "resources": []
+            "resources": [
+                "vpc"
+            ]
         },
         "DisassociateAddress": {
-            "access_level": "Undocumented",
+            "access_level": "Write",
             "action": "DisassociateAddress",
-            "condition_keys": [],
-            "description": "Not Documented by AWS",
+            "condition_keys": [
+                "aws:ResourceTag/${TagKey}",
+                "ec2:AllocationId",
+                "ec2:AvailabilityZone",
+                "ec2:Domain",
+                "ec2:NetworkInterfaceID",
+                "ec2:PublicIpAddress",
+                "ec2:Region",
+                "ec2:ResourceTag/${TagKey}",
+                "ec2:Subnet",
+                "ec2:Vpc"
+            ],
+            "description": "Grants permission to disassociate an Elastic IP address from an instance or network interface",
             "orphan": false,
-            "resources": []
+            "resources": [
+                "elastic-ip",
+                "network-interface"
+            ]
         },
         "DisassociateClientVpnTargetNetwork": {
-            "access_level": "Undocumented",
+            "access_level": "Write",
             "action": "DisassociateClientVpnTargetNetwork",
-            "condition_keys": [],
-            "description": "Not Documented by AWS",
+            "condition_keys": [
+                "aws:ResourceTag/${TagKey}",
+                "ec2:ClientRootCertificateChainArn",
+                "ec2:CloudwatchLogGroupArn",
+                "ec2:CloudwatchLogStreamArn",
+                "ec2:DirectoryArn",
+                "ec2:Region",
+                "ec2:ResourceTag/${TagKey}",
+                "ec2:SamlProviderArn",
+                "ec2:ServerCertificateArn"
+            ],
+            "description": "Grants permission to disassociate a target network from a Client VPN endpoint",
             "orphan": false,
-            "resources": []
+            "resources": [
+                "client-vpn-endpoint"
+            ]
         },
         "DisassociateEnclaveCertificateIamRole": {
-            "access_level": "Undocumented",
+            "access_level": "Write",
             "action": "DisassociateEnclaveCertificateIamRole",
-            "condition_keys": [],
-            "description": "Not Documented by AWS",
+            "condition_keys": [
+                "ec2:Region"
+            ],
+            "description": "Grants permission to disassociate an ACM certificate from a IAM role",
             "orphan": false,
-            "resources": []
+            "resources": [
+                "certificate",
+                "role"
+            ]
         },
         "DisassociateIamInstanceProfile": {
-            "access_level": "Undocumented",
+            "access_level": "Write",
             "action": "DisassociateIamInstanceProfile",
-            "condition_keys": [],
-            "description": "Not Documented by AWS",
+            "condition_keys": [
+                "aws:ResourceTag/${TagKey}",
+                "ec2:AvailabilityZone",
+                "ec2:EbsOptimized",
+                "ec2:InstanceAutoRecovery",
+                "ec2:InstanceID",
+                "ec2:InstanceMarketType",
+                "ec2:InstanceMetadataTags",
+                "ec2:InstanceProfile",
+                "ec2:InstanceType",
+                "ec2:MetadataHttpEndpoint",
+                "ec2:MetadataHttpPutResponseHopLimit",
+                "ec2:MetadataHttpTokens",
+                "ec2:PlacementGroup",
+                "ec2:ProductCode",
+                "ec2:Region",
+                "ec2:ResourceTag/${TagKey}",
+                "ec2:RootDeviceType",
+                "ec2:Tenancy"
+            ],
+            "description": "Grants permission to disassociate an IAM instance profile from a running or stopped instance",
             "orphan": false,
-            "resources": []
+            "resources": [
+                "instance"
+            ]
         },
         "DisassociateInstanceEventWindow": {
-            "access_level": "Undocumented",
+            "access_level": "Write",
             "action": "DisassociateInstanceEventWindow",
-            "condition_keys": [],
-            "description": "Not Documented by AWS",
+            "condition_keys": [
+                "aws:ResourceTag/${TagKey}",
+                "ec2:Region",
+                "ec2:ResourceTag/${TagKey}"
+            ],
+            "description": "Grants permission to disassociate one or more targets from an event window",
             "orphan": false,
-            "resources": []
+            "resources": [
+                "instance-event-window"
+            ]
         },
         "DisassociateIpamResourceDiscovery": {
-            "access_level": "Undocumented",
+            "access_level": "Write",
             "action": "DisassociateIpamResourceDiscovery",
-            "condition_keys": [],
-            "description": "Not Documented by AWS",
+            "condition_keys": [
+                "aws:ResourceTag/${TagKey}",
+                "ec2:Region",
+                "ec2:ResourceTag/${TagKey}"
+            ],
+            "description": "Grants permission to disassociate a resource discovery from an Amazon VPC IPAM",
             "orphan": false,
-            "resources": []
+            "resources": [
+                "ipam-resource-discovery-association"
+            ]
         },
         "DisassociateNatGatewayAddress": {
-            "access_level": "Undocumented",
+            "access_level": "Write",
             "action": "DisassociateNatGatewayAddress",
-            "condition_keys": [],
-            "description": "Not Documented by AWS",
-            "orphan": false,
-            "resources": []
+            "condition_keys": [
+                "aws:ResourceTag/${TagKey}",
+                "ec2:AllocationId",
+                "ec2:AuthorizedUser",
+                "ec2:AvailabilityZone",
+                "ec2:Domain",
+                "ec2:NetworkInterfaceID",
+                "ec2:Permission",
+                "ec2:PublicIpAddress",
+                "ec2:Region",
+                "ec2:ResourceTag/${TagKey}",
+                "ec2:Subnet",
+                "ec2:Vpc"
+            ],
+            "description": "Grants permission to disassociate a secondary Elastic IP address from a public NAT gateway",
+            "orphan": false,
+            "resources": [
+                "elastic-ip",
+                "natgateway",
+                "network-interface"
+            ]
         },
         "DisassociateRouteTable": {
-            "access_level": "Undocumented",
+            "access_level": "Write",
             "action": "DisassociateRouteTable",
-            "condition_keys": [],
-            "description": "Not Documented by AWS",
-            "orphan": false,
-            "resources": []
+            "condition_keys": [
+                "aws:ResourceTag/${TagKey}",
+                "ec2:AvailabilityZone",
+                "ec2:InternetGatewayID",
+                "ec2:Region",
+                "ec2:ResourceTag/${TagKey}",
+                "ec2:RouteTableID",
+                "ec2:SubnetID",
+                "ec2:Vpc"
+            ],
+            "description": "Grants permission to disassociate a subnet from a route table",
+            "orphan": false,
+            "resources": [
+                "internet-gateway",
+                "ipv4pool-ec2",
+                "ipv6pool-ec2",
+                "route-table",
+                "subnet",
+                "vpn-gateway"
+            ]
         },
         "DisassociateSubnetCidrBlock": {
-            "access_level": "Undocumented",
+            "access_level": "Write",
             "action": "DisassociateSubnetCidrBlock",
-            "condition_keys": [],
-            "description": "Not Documented by AWS",
+            "condition_keys": [
+                "aws:ResourceTag/${TagKey}",
+                "ec2:AvailabilityZone",
+                "ec2:Region",
+                "ec2:ResourceTag/${TagKey}",
+                "ec2:SubnetID",
+                "ec2:Vpc"
+            ],
+            "description": "Grants permission to disassociate a CIDR block from a subnet",
             "orphan": false,
-            "resources": []
+            "resources": [
+                "subnet"
+            ]
         },
         "DisassociateTransitGatewayMulticastDomain": {
-            "access_level": "Undocumented",
+            "access_level": "Write",
             "action": "DisassociateTransitGatewayMulticastDomain",
-            "condition_keys": [],
-            "description": "Not Documented by AWS",
+            "condition_keys": [
+                "aws:ResourceTag/${TagKey}",
+                "ec2:AvailabilityZone",
+                "ec2:Region",
+                "ec2:ResourceTag/${TagKey}",
+                "ec2:SubnetID",
+                "ec2:Vpc"
+            ],
+            "description": "Grants permission to disassociate one or more subnets from a transit gateway multicast domain",
             "orphan": false,
-            "resources": []
+            "resources": [
+                "subnet",
+                "transit-gateway-attachment",
+                "transit-gateway-multicast-domain"
+            ]
         },
         "DisassociateTransitGatewayPolicyTable": {
-            "access_level": "Undocumented",
+            "access_level": "Write",
             "action": "DisassociateTransitGatewayPolicyTable",
-            "condition_keys": [],
-            "description": "Not Documented by AWS",
+            "condition_keys": [
+                "aws:ResourceTag/${TagKey}",
+                "ec2:Region",
+                "ec2:ResourceTag/${TagKey}"
+            ],
+            "description": "Grants permission to disassociate a policy table from a transit gateway",
             "orphan": false,
-            "resources": []
+            "resources": [
+                "transit-gateway-attachment",
+                "transit-gateway-policy-table"
+            ]
         },
         "DisassociateTransitGatewayRouteTable": {
-            "access_level": "Undocumented",
+            "access_level": "Write",
             "action": "DisassociateTransitGatewayRouteTable",
-            "condition_keys": [],
-            "description": "Not Documented by AWS",
+            "condition_keys": [
+                "aws:ResourceTag/${TagKey}",
+                "ec2:Region",
+                "ec2:ResourceTag/${TagKey}"
+            ],
+            "description": "Grants permission to disassociate a resource attachment from a transit gateway route table",
             "orphan": false,
-            "resources": []
+            "resources": [
+                "transit-gateway-attachment",
+                "transit-gateway-route-table"
+            ]
         },
         "DisassociateTrunkInterface": {
-            "access_level": "Undocumented",
+            "access_level": "Write",
             "action": "DisassociateTrunkInterface",
-            "condition_keys": [],
-            "description": "Not Documented by AWS",
+            "condition_keys": [
+                "ec2:Region"
+            ],
+            "description": "Grants permission to disassociate a branch network interface to a trunk network interface",
             "orphan": false,
             "resources": []
         },
         "DisassociateVerifiedAccessInstanceWebAcl": {
-            "access_level": "Undocumented",
+            "access_level": "Write",
             "action": "DisassociateVerifiedAccessInstanceWebAcl",
-            "condition_keys": [],
-            "description": "Not Documented by AWS",
+            "condition_keys": [
+                "aws:ResourceTag/${TagKey}",
+                "ec2:Region",
+                "ec2:ResourceTag/${TagKey}"
+            ],
+            "description": "Grants permission to disassociate an AWS Web Application Firewall (WAF) web access control list (ACL) from a Verified Access instance",
             "orphan": false,
-            "resources": []
+            "resources": [
+                "verified-access-instance"
+            ]
         },
         "DisassociateVpcCidrBlock": {
-            "access_level": "Undocumented",
+            "access_level": "Write",
             "action": "DisassociateVpcCidrBlock",
-            "condition_keys": [],
-            "description": "Not Documented by AWS",
+            "condition_keys": [
+                "aws:ResourceTag/${TagKey}",
+                "ec2:Region",
+                "ec2:ResourceTag/${TagKey}",
+                "ec2:Tenancy",
+                "ec2:VpcID"
+            ],
+            "description": "Grants permission to disassociate a CIDR block from a VPC",
             "orphan": false,
-            "resources": []
+            "resources": [
+                "vpc"
+            ]
         },
         "EnableAddressTransfer": {
-            "access_level": "Undocumented",
+            "access_level": "Write",
             "action": "EnableAddressTransfer",
-            "condition_keys": [],
-            "description": "Not Documented by AWS",
+            "condition_keys": [
+                "aws:ResourceTag/${TagKey}",
+                "ec2:AllocationId",
+                "ec2:Domain",
+                "ec2:PublicIpAddress",
+                "ec2:Region",
+                "ec2:ResourceTag/${TagKey}"
+            ],
+            "description": "Grants permission to enable Elastic IP address transfer",
             "orphan": false,
-            "resources": []
+            "resources": [
+                "elastic-ip"
+            ]
         },
         "EnableAwsNetworkPerformanceMetricSubscription": {
-            "access_level": "Undocumented",
+            "access_level": "Write",
             "action": "EnableAwsNetworkPerformanceMetricSubscription",
-            "condition_keys": [],
-            "description": "Not Documented by AWS",
+            "condition_keys": [
+                "ec2:Region"
+            ],
+            "description": "Grants permission to enable infrastructure performance subscriptions",
             "orphan": false,
             "resources": []
         },
         "EnableEbsEncryptionByDefault": {
-            "access_level": "Undocumented",
+            "access_level": "Write",
             "action": "EnableEbsEncryptionByDefault",
-            "condition_keys": [],
-            "description": "Not Documented by AWS",
+            "condition_keys": [
+                "ec2:Region"
+            ],
+            "description": "Grants permission to enable EBS encryption by default for your account",
             "orphan": false,
             "resources": []
         },
         "EnableFastLaunch": {
-            "access_level": "Undocumented",
+            "access_level": "Write",
             "action": "EnableFastLaunch",
-            "condition_keys": [],
-            "description": "Not Documented by AWS",
+            "condition_keys": [
+                "aws:ResourceTag/${TagKey}",
+                "ec2:ImageID",
+                "ec2:ImageType",
+                "ec2:Owner",
+                "ec2:Public",
+                "ec2:Region",
+                "ec2:ResourceTag/${TagKey}",
+                "ec2:RootDeviceType"
+            ],
+            "description": "Grants permission to enable faster launching for Windows AMIs",
             "orphan": false,
-            "resources": []
+            "resources": [
+                "image",
+                "launch-template"
+            ]
         },
         "EnableFastSnapshotRestores": {
-            "access_level": "Undocumented",
+            "access_level": "Write",
             "action": "EnableFastSnapshotRestores",
-            "condition_keys": [],
-            "description": "Not Documented by AWS",
+            "condition_keys": [
+                "aws:ResourceTag/${TagKey}",
+                "ec2:AvailabilityZone",
+                "ec2:Encrypted",
+                "ec2:Owner",
+                "ec2:ParentVolume",
+                "ec2:Region",
+                "ec2:ResourceTag/${TagKey}",
+                "ec2:SnapshotID",
+                "ec2:SnapshotTime",
+                "ec2:VolumeSize"
+            ],
+            "description": "Grants permission to enable fast snapshot restores for one or more snapshots in specified Availability Zones",
             "orphan": false,
-            "resources": []
+            "resources": [
+                "snapshot"
+            ]
         },
         "EnableImageDeprecation": {
-            "access_level": "Undocumented",
+            "access_level": "Write",
             "action": "EnableImageDeprecation",
-            "condition_keys": [],
-            "description": "Not Documented by AWS",
+            "condition_keys": [
+                "aws:ResourceTag/${TagKey}",
+                "ec2:ImageID",
+                "ec2:ImageType",
+                "ec2:Owner",
+                "ec2:Public",
+                "ec2:Region",
+                "ec2:ResourceTag/${TagKey}",
+                "ec2:RootDeviceType"
+            ],
+            "description": "Grants permission to enable deprecation of the specified AMI at the specified date and time",
             "orphan": false,
-            "resources": []
+            "resources": [
+                "image"
+            ]
         },
         "EnableIpamOrganizationAdminAccount": {
-            "access_level": "Undocumented",
+            "access_level": "Write",
             "action": "EnableIpamOrganizationAdminAccount",
-            "condition_keys": [],
-            "description": "Not Documented by AWS",
+            "condition_keys": [
+                "ec2:Region"
+            ],
+            "description": "Grants permission to enable an AWS Organizations member account as an Amazon VPC IP Address Manager (IPAM) admin account",
             "orphan": false,
             "resources": []
         },
         "EnableReachabilityAnalyzerOrganizationSharing": {
-            "access_level": "Undocumented",
+            "access_level": "Write",
             "action": "EnableReachabilityAnalyzerOrganizationSharing",
-            "condition_keys": [],
-            "description": "Not Documented by AWS",
+            "condition_keys": [
+                "ec2:Region"
+            ],
+            "description": "Grants permission to enable organization sharing of reachability analyzer",
             "orphan": false,
             "resources": []
         },
         "EnableSerialConsoleAccess": {
-            "access_level": "Undocumented",
+            "access_level": "Write",
             "action": "EnableSerialConsoleAccess",
-            "condition_keys": [],
-            "description": "Not Documented by AWS",
+            "condition_keys": [
+                "ec2:Region"
+            ],
+            "description": "Grants permission to enable access to the EC2 serial console of all instances for your account",
             "orphan": false,
             "resources": []
         },
         "EnableTransitGatewayRouteTablePropagation": {
-            "access_level": "Undocumented",
+            "access_level": "Write",
             "action": "EnableTransitGatewayRouteTablePropagation",
-            "condition_keys": [],
-            "description": "Not Documented by AWS",
+            "condition_keys": [
+                "aws:ResourceTag/${TagKey}",
+                "ec2:Region",
+                "ec2:ResourceTag/${TagKey}"
+            ],
+            "description": "Grants permission to enable an attachment to propagate routes to a propagation route table",
             "orphan": false,
-            "resources": []
+            "resources": [
+                "transit-gateway-attachment",
+                "transit-gateway-route-table",
+                "transit-gateway-route-table-announcement"
+            ]
         },
         "EnableVgwRoutePropagation": {
-            "access_level": "Undocumented",
+            "access_level": "Write",
             "action": "EnableVgwRoutePropagation",
-            "condition_keys": [],
-            "description": "Not Documented by AWS",
+            "condition_keys": [
+                "aws:ResourceTag/${TagKey}",
+                "ec2:Region",
+                "ec2:ResourceTag/${TagKey}",
+                "ec2:RouteTableID",
+                "ec2:Vpc"
+            ],
+            "description": "Grants permission to enable a virtual private gateway to propagate routes to a VPC route table",
             "orphan": false,
-            "resources": []
+            "resources": [
+                "route-table",
+                "vpn-gateway"
+            ]
         },
         "EnableVolumeIO": {
-            "access_level": "Undocumented",
+            "access_level": "Write",
             "action": "EnableVolumeIO",
-            "condition_keys": [],
-            "description": "Not Documented by AWS",
+            "condition_keys": [
+                "aws:ResourceTag/${TagKey}",
+                "ec2:AvailabilityZone",
+                "ec2:Encrypted",
+                "ec2:ParentSnapshot",
+                "ec2:Region",
+                "ec2:ResourceTag/${TagKey}",
+                "ec2:VolumeID",
+                "ec2:VolumeIops",
+                "ec2:VolumeSize",
+                "ec2:VolumeThroughput",
+                "ec2:VolumeType"
+            ],
+            "description": "Grants permission to enable I/O operations for a volume that had I/O operations disabled",
             "orphan": false,
-            "resources": []
+            "resources": [
+                "volume"
+            ]
         },
         "EnableVpcClassicLink": {
-            "access_level": "Undocumented",
+            "access_level": "Write",
             "action": "EnableVpcClassicLink",
-            "condition_keys": [],
-            "description": "Not Documented by AWS",
+            "condition_keys": [
+                "aws:ResourceTag/${TagKey}",
+                "ec2:Region",
+                "ec2:ResourceTag/${TagKey}",
+                "ec2:Tenancy",
+                "ec2:VpcID"
+            ],
+            "description": "Grants permission to enable a VPC for ClassicLink",
             "orphan": false,
-            "resources": []
+            "resources": [
+                "vpc"
+            ]
         },
         "EnableVpcClassicLinkDnsSupport": {
-            "access_level": "Undocumented",
+            "access_level": "Write",
             "action": "EnableVpcClassicLinkDnsSupport",
-            "condition_keys": [],
-            "description": "Not Documented by AWS",
+            "condition_keys": [
+                "aws:ResourceTag/${TagKey}",
+                "ec2:Region",
+                "ec2:ResourceTag/${TagKey}",
+                "ec2:Tenancy",
+                "ec2:VpcID"
+            ],
+            "description": "Grants permission to enable a VPC to support DNS hostname resolution for ClassicLink",
             "orphan": false,
-            "resources": []
+            "resources": [
+                "vpc"
+            ]
         },
         "ExportClientVpnClientCertificateRevocationList": {
-            "access_level": "Undocumented",
+            "access_level": "Read",
             "action": "ExportClientVpnClientCertificateRevocationList",
-            "condition_keys": [],
-            "description": "Not Documented by AWS",
+            "condition_keys": [
+                "aws:ResourceTag/${TagKey}",
+                "ec2:ClientRootCertificateChainArn",
+                "ec2:CloudwatchLogGroupArn",
+                "ec2:CloudwatchLogStreamArn",
+                "ec2:DirectoryArn",
+                "ec2:Region",
+                "ec2:ResourceTag/${TagKey}",
+                "ec2:SamlProviderArn",
+                "ec2:ServerCertificateArn"
+            ],
+            "description": "Grants permission to download the client certificate revocation list for a Client VPN endpoint",
             "orphan": false,
-            "resources": []
+            "resources": [
+                "client-vpn-endpoint"
+            ]
         },
         "ExportClientVpnClientConfiguration": {
-            "access_level": "Undocumented",
+            "access_level": "Read",
             "action": "ExportClientVpnClientConfiguration",
-            "condition_keys": [],
-            "description": "Not Documented by AWS",
+            "condition_keys": [
+                "aws:ResourceTag/${TagKey}",
+                "ec2:ClientRootCertificateChainArn",
+                "ec2:CloudwatchLogGroupArn",
+                "ec2:CloudwatchLogStreamArn",
+                "ec2:DirectoryArn",
+                "ec2:Region",
+                "ec2:ResourceTag/${TagKey}",
+                "ec2:SamlProviderArn",
+                "ec2:ServerCertificateArn"
+            ],
+            "description": "Grants permission to download the contents of the Client VPN endpoint configuration file for a Client VPN endpoint",
             "orphan": false,
-            "resources": []
+            "resources": [
+                "client-vpn-endpoint"
+            ]
         },
         "ExportImage": {
-            "access_level": "Undocumented",
+            "access_level": "Write",
             "action": "ExportImage",
-            "condition_keys": [],
-            "description": "Not Documented by AWS",
+            "condition_keys": [
+                "aws:RequestTag/${TagKey}",
+                "aws:ResourceTag/${TagKey}",
+                "aws:TagKeys",
+                "ec2:ImageID",
+                "ec2:ImageType",
+                "ec2:Owner",
+                "ec2:Public",
+                "ec2:Region",
+                "ec2:ResourceTag/${TagKey}",
+                "ec2:RootDeviceType"
+            ],
+            "description": "Grants permission to export an Amazon Machine Image (AMI) to a VM file",
             "orphan": false,
-            "resources": []
+            "resources": [
+                "export-image-task",
+                "image"
+            ]
         },
         "ExportTransitGatewayRoutes": {
-            "access_level": "Undocumented",
+            "access_level": "Write",
             "action": "ExportTransitGatewayRoutes",
-            "condition_keys": [],
-            "description": "Not Documented by AWS",
+            "condition_keys": [
+                "ec2:Region"
+            ],
+            "description": "Grants permission to export routes from a transit gateway route table to an Amazon S3 bucket",
             "orphan": false,
             "resources": []
         },
         "GetAssociatedEnclaveCertificateIamRoles": {
-            "access_level": "Undocumented",
+            "access_level": "Read",
             "action": "GetAssociatedEnclaveCertificateIamRoles",
-            "condition_keys": [],
-            "description": "Not Documented by AWS",
+            "condition_keys": [
+                "ec2:Region"
+            ],
+            "description": "Grants permission to get the list of roles associated with an ACM certificate",
             "orphan": false,
-            "resources": []
+            "resources": [
+                "certificate"
+            ]
         },
         "GetAssociatedIpv6PoolCidrs": {
-            "access_level": "Undocumented",
+            "access_level": "Read",
             "action": "GetAssociatedIpv6PoolCidrs",
-            "condition_keys": [],
-            "description": "Not Documented by AWS",
+            "condition_keys": [
+                "ec2:Region"
+            ],
+            "description": "Grants permission to get information about the IPv6 CIDR block associations for a specified IPv6 address pool",
             "orphan": false,
             "resources": []
         },
         "GetAwsNetworkPerformanceData": {
-            "access_level": "Undocumented",
+            "access_level": "Read",
             "action": "GetAwsNetworkPerformanceData",
-            "condition_keys": [],
-            "description": "Not Documented by AWS",
+            "condition_keys": [
+                "ec2:Region"
+            ],
+            "description": "Grants permission to get network performance data",
             "orphan": false,
             "resources": []
         },
         "GetCapacityReservationUsage": {
-            "access_level": "Undocumented",
+            "access_level": "Read",
             "action": "GetCapacityReservationUsage",
-            "condition_keys": [],
-            "description": "Not Documented by AWS",
+            "condition_keys": [
+                "aws:ResourceTag/${TagKey}",
+                "ec2:CapacityReservationFleet",
+                "ec2:Region",
+                "ec2:ResourceTag/${TagKey}"
+            ],
+            "description": "Grants permission to get usage information about a Capacity Reservation",
             "orphan": false,
-            "resources": []
+            "resources": [
+                "capacity-reservation"
+            ]
         },
         "GetCoipPoolUsage": {
-            "access_level": "Undocumented",
+            "access_level": "Read",
             "action": "GetCoipPoolUsage",
-            "condition_keys": [],
-            "description": "Not Documented by AWS",
+            "condition_keys": [
+                "aws:ResourceTag/${TagKey}",
+                "ec2:Region",
+                "ec2:ResourceTag/${TagKey}"
+            ],
+            "description": "Grants permission to describe the allocations from the specified customer-owned address pool",
             "orphan": false,
-            "resources": []
+            "resources": [
+                "coip-pool"
+            ]
         },
         "GetConsoleOutput": {
-            "access_level": "Undocumented",
+            "access_level": "Read",
             "action": "GetConsoleOutput",
-            "condition_keys": [],
-            "description": "Not Documented by AWS",
+            "condition_keys": [
+                "aws:ResourceTag/${TagKey}",
+                "ec2:AvailabilityZone",
+                "ec2:EbsOptimized",
+                "ec2:InstanceAutoRecovery",
+                "ec2:InstanceID",
+                "ec2:InstanceMarketType",
+                "ec2:InstanceMetadataTags",
+                "ec2:InstanceProfile",
+                "ec2:InstanceType",
+                "ec2:MetadataHttpEndpoint",
+                "ec2:MetadataHttpPutResponseHopLimit",
+                "ec2:MetadataHttpTokens",
+                "ec2:PlacementGroup",
+                "ec2:ProductCode",
+                "ec2:Region",
+                "ec2:ResourceTag/${TagKey}",
+                "ec2:RootDeviceType",
+                "ec2:Tenancy"
+            ],
+            "description": "Grants permission to get the console output for an instance",
             "orphan": false,
-            "resources": []
+            "resources": [
+                "instance"
+            ]
         },
         "GetConsoleScreenshot": {
-            "access_level": "Undocumented",
+            "access_level": "Read",
             "action": "GetConsoleScreenshot",
-            "condition_keys": [],
-            "description": "Not Documented by AWS",
+            "condition_keys": [
+                "aws:ResourceTag/${TagKey}",
+                "ec2:AvailabilityZone",
+                "ec2:EbsOptimized",
+                "ec2:InstanceAutoRecovery",
+                "ec2:InstanceID",
+                "ec2:InstanceMarketType",
+                "ec2:InstanceMetadataTags",
+                "ec2:InstanceProfile",
+                "ec2:InstanceType",
+                "ec2:MetadataHttpEndpoint",
+                "ec2:MetadataHttpPutResponseHopLimit",
+                "ec2:MetadataHttpTokens",
+                "ec2:NewInstanceProfile",
+                "ec2:PlacementGroup",
+                "ec2:ProductCode",
+                "ec2:Region",
+                "ec2:ResourceTag/${TagKey}",
+                "ec2:RootDeviceType",
+                "ec2:Tenancy"
+            ],
+            "description": "Grants permission to retrieve a JPG-format screenshot of a running instance",
             "orphan": false,
-            "resources": []
+            "resources": [
+                "instance"
+            ]
         },
         "GetDefaultCreditSpecification": {
-            "access_level": "Undocumented",
+            "access_level": "Read",
             "action": "GetDefaultCreditSpecification",
-            "condition_keys": [],
-            "description": "Not Documented by AWS",
+            "condition_keys": [
+                "ec2:Region"
+            ],
+            "description": "Grants permission to get the default credit option for CPU usage of a burstable performance instance family",
             "orphan": false,
             "resources": []
         },
         "GetEbsDefaultKmsKeyId": {
-            "access_level": "Undocumented",
+            "access_level": "Read",
             "action": "GetEbsDefaultKmsKeyId",
-            "condition_keys": [],
-            "description": "Not Documented by AWS",
+            "condition_keys": [
+                "ec2:Region"
+            ],
+            "description": "Grants permission to get the ID of the default customer master key (CMK) for EBS encryption by default",
             "orphan": false,
             "resources": []
         },
         "GetEbsEncryptionByDefault": {
-            "access_level": "Undocumented",
+            "access_level": "Read",
             "action": "GetEbsEncryptionByDefault",
-            "condition_keys": [],
-            "description": "Not Documented by AWS",
+            "condition_keys": [
+                "ec2:Region"
+            ],
+            "description": "Grants permission to describe whether EBS encryption by default is enabled for your account",
             "orphan": false,
             "resources": []
         },
         "GetFlowLogsIntegrationTemplate": {
-            "access_level": "Undocumented",
+            "access_level": "Read",
             "action": "GetFlowLogsIntegrationTemplate",
-            "condition_keys": [],
-            "description": "Not Documented by AWS",
+            "condition_keys": [
+                "aws:ResourceTag/${TagKey}",
+                "ec2:Region",
+                "ec2:ResourceTag/${TagKey}"
+            ],
+            "description": "Grants permission to generate a CloudFormation template to streamline the integration of VPC flow logs with Amazon Athena",
             "orphan": false,
-            "resources": []
+            "resources": [
+                "vpc-flow-log"
+            ]
         },
         "GetGroupsForCapacityReservation": {
-            "access_level": "Undocumented",
+            "access_level": "List",
             "action": "GetGroupsForCapacityReservation",
-            "condition_keys": [],
-            "description": "Not Documented by AWS",
+            "condition_keys": [
+                "aws:ResourceTag/${TagKey}",
+                "ec2:CapacityReservationFleet",
+                "ec2:Region",
+                "ec2:ResourceTag/${TagKey}"
+            ],
+            "description": "Grants permission to list the resource groups to which a Capacity Reservation has been added",
             "orphan": false,
-            "resources": []
+            "resources": [
+                "capacity-reservation"
+            ]
         },
         "GetHostReservationPurchasePreview": {
-            "access_level": "Undocumented",
+            "access_level": "Read",
             "action": "GetHostReservationPurchasePreview",
-            "condition_keys": [],
-            "description": "Not Documented by AWS",
+            "condition_keys": [
+                "ec2:Region"
+            ],
+            "description": "Grants permission to preview a reservation purchase with configurations that match those of a Dedicated Host",
             "orphan": false,
             "resources": []
         },
         "GetInstanceTypesFromInstanceRequirements": {
-            "access_level": "Undocumented",
+            "access_level": "List",
             "action": "GetInstanceTypesFromInstanceRequirements",
-            "condition_keys": [],
-            "description": "Not Documented by AWS",
+            "condition_keys": [
+                "ec2:Region"
+            ],
+            "description": "Grants permission to view a list of instance types with specified instance attributes",
             "orphan": false,
             "resources": []
         },
         "GetInstanceUefiData": {
-            "access_level": "Undocumented",
+            "access_level": "Read",
             "action": "GetInstanceUefiData",
-            "condition_keys": [],
-            "description": "Not Documented by AWS",
+            "condition_keys": [
+                "aws:ResourceTag/${TagKey}",
+                "ec2:AvailabilityZone",
+                "ec2:EbsOptimized",
+                "ec2:InstanceAutoRecovery",
+                "ec2:InstanceID",
+                "ec2:InstanceMarketType",
+                "ec2:InstanceMetadataTags",
+                "ec2:InstanceProfile",
+                "ec2:InstanceType",
+                "ec2:MetadataHttpEndpoint",
+                "ec2:MetadataHttpPutResponseHopLimit",
+                "ec2:MetadataHttpTokens",
+                "ec2:NewInstanceProfile",
+                "ec2:PlacementGroup",
+                "ec2:ProductCode",
+                "ec2:Region",
+                "ec2:ResourceTag/${TagKey}",
+                "ec2:RootDeviceType",
+                "ec2:Tenancy"
+            ],
+            "description": "Grants permission to retrieve the binary representation of the UEFI variable store",
             "orphan": false,
-            "resources": []
+            "resources": [
+                "instance"
+            ]
         },
         "GetIpamAddressHistory": {
-            "access_level": "Undocumented",
+            "access_level": "Read",
             "action": "GetIpamAddressHistory",
-            "condition_keys": [],
-            "description": "Not Documented by AWS",
+            "condition_keys": [
+                "aws:ResourceTag/${TagKey}",
+                "ec2:Region",
+                "ec2:ResourceTag/${TagKey}"
+            ],
+            "description": "Grants permission to retrieve historical information about a CIDR within an Amazon VPC IP Address Manager (IPAM) scope",
             "orphan": false,
-            "resources": []
+            "resources": [
+                "ipam-scope"
+            ]
         },
         "GetIpamDiscoveredAccounts": {
-            "access_level": "Undocumented",
+            "access_level": "Read",
             "action": "GetIpamDiscoveredAccounts",
-            "condition_keys": [],
-            "description": "Not Documented by AWS",
+            "condition_keys": [
+                "aws:ResourceTag/${TagKey}",
+                "ec2:Region",
+                "ec2:ResourceTag/${TagKey}"
+            ],
+            "description": "Grants permission to retrieve IPAM discovered accounts",
             "orphan": false,
-            "resources": []
+            "resources": [
+                "ipam-resource-discovery"
+            ]
         },
         "GetIpamDiscoveredResourceCidrs": {
-            "access_level": "Undocumented",
+            "access_level": "Read",
             "action": "GetIpamDiscoveredResourceCidrs",
-            "condition_keys": [],
-            "description": "Not Documented by AWS",
+            "condition_keys": [
+                "aws:ResourceTag/${TagKey}",
+                "ec2:Region",
+                "ec2:ResourceTag/${TagKey}"
+            ],
+            "description": "Grants permission to retrieve the resource CIDRs that are monitored as part of a resource discovery",
             "orphan": false,
-            "resources": []
+            "resources": [
+                "ipam-resource-discovery"
+            ]
         },
         "GetIpamPoolAllocations": {
-            "access_level": "Undocumented",
+            "access_level": "List",
             "action": "GetIpamPoolAllocations",
-            "condition_keys": [],
-            "description": "Not Documented by AWS",
+            "condition_keys": [
+                "aws:ResourceTag/${TagKey}",
+                "ec2:Region",
+                "ec2:ResourceTag/${TagKey}"
+            ],
+            "description": "Grants permission to get a list of all the CIDR allocations in an Amazon VPC IP Address Manager (IPAM) pool",
             "orphan": false,
-            "resources": []
+            "resources": [
+                "ipam-pool"
+            ]
         },
         "GetIpamPoolCidrs": {
-            "access_level": "Undocumented",
+            "access_level": "Read",
             "action": "GetIpamPoolCidrs",
-            "condition_keys": [],
-            "description": "Not Documented by AWS",
+            "condition_keys": [
+                "aws:ResourceTag/${TagKey}",
+                "ec2:Region",
+                "ec2:ResourceTag/${TagKey}"
+            ],
+            "description": "Grants permission to get the CIDRs provisioned to an Amazon VPC IP Address Manager (IPAM) pool",
             "orphan": false,
-            "resources": []
+            "resources": [
+                "ipam-pool"
+            ]
         },
         "GetIpamResourceCidrs": {
-            "access_level": "Undocumented",
+            "access_level": "Read",
             "action": "GetIpamResourceCidrs",
-            "condition_keys": [],
-            "description": "Not Documented by AWS",
+            "condition_keys": [
+                "aws:ResourceTag/${TagKey}",
+                "ec2:Region",
+                "ec2:ResourceTag/${TagKey}"
+            ],
+            "description": "Grants permission to get information about the resources in an Amazon VPC IP Address Manager (IPAM) scope",
             "orphan": false,
-            "resources": []
+            "resources": [
+                "ipam-pool",
+                "ipam-scope"
+            ]
         },
         "GetLaunchTemplateData": {
-            "access_level": "Undocumented",
+            "access_level": "Read",
             "action": "GetLaunchTemplateData",
-            "condition_keys": [],
-            "description": "Not Documented by AWS",
+            "condition_keys": [
+                "aws:ResourceTag/${TagKey}",
+                "ec2:AvailabilityZone",
+                "ec2:EbsOptimized",
+                "ec2:InstanceAutoRecovery",
+                "ec2:InstanceID",
+                "ec2:InstanceMarketType",
+                "ec2:InstanceMetadataTags",
+                "ec2:InstanceProfile",
+                "ec2:InstanceType",
+                "ec2:MetadataHttpEndpoint",
+                "ec2:MetadataHttpPutResponseHopLimit",
+                "ec2:MetadataHttpTokens",
+                "ec2:PlacementGroup",
+                "ec2:ProductCode",
+                "ec2:Region",
+                "ec2:ResourceTag/${TagKey}",
+                "ec2:RootDeviceType",
+                "ec2:Tenancy"
+            ],
+            "description": "Grants permission to get the configuration data of the specified instance for use with a new launch template or launch template version",
             "orphan": false,
-            "resources": []
+            "resources": [
+                "instance"
+            ]
         },
         "GetManagedPrefixListAssociations": {
-            "access_level": "Undocumented",
+            "access_level": "Read",
             "action": "GetManagedPrefixListAssociations",
-            "condition_keys": [],
-            "description": "Not Documented by AWS",
+            "condition_keys": [
+                "aws:ResourceTag/${TagKey}",
+                "ec2:Region",
+                "ec2:ResourceTag/${TagKey}"
+            ],
+            "description": "Grants permission to get information about the resources that are associated with the specified managed prefix list",
             "orphan": false,
-            "resources": []
+            "resources": [
+                "prefix-list"
+            ]
         },
         "GetManagedPrefixListEntries": {
-            "access_level": "Undocumented",
+            "access_level": "Read",
             "action": "GetManagedPrefixListEntries",
-            "condition_keys": [],
-            "description": "Not Documented by AWS",
+            "condition_keys": [
+                "aws:ResourceTag/${TagKey}",
+                "ec2:Region",
+                "ec2:ResourceTag/${TagKey}"
+            ],
+            "description": "Grants permission to get information about the entries for a specified managed prefix list",
             "orphan": false,
-            "resources": []
+            "resources": [
+                "prefix-list"
+            ]
         },
         "GetNetworkInsightsAccessScopeAnalysisFindings": {
-            "access_level": "Undocumented",
+            "access_level": "Read",
             "action": "GetNetworkInsightsAccessScopeAnalysisFindings",
-            "condition_keys": [],
-            "description": "Not Documented by AWS",
+            "condition_keys": [
+                "ec2:Region"
+            ],
+            "description": "Grants permission to get the findings for one or more Network Access Scope analyses",
             "orphan": false,
             "resources": []
         },
         "GetNetworkInsightsAccessScopeContent": {
-            "access_level": "Undocumented",
+            "access_level": "Read",
             "action": "GetNetworkInsightsAccessScopeContent",
-            "condition_keys": [],
-            "description": "Not Documented by AWS",
+            "condition_keys": [
+                "ec2:Region"
+            ],
+            "description": "Grants permission to get the content for a specified Network Access Scope",
             "orphan": false,
             "resources": []
         },
         "GetPasswordData": {
-            "access_level": "Undocumented",
+            "access_level": "Read",
             "action": "GetPasswordData",
-            "condition_keys": [],
-            "description": "Not Documented by AWS",
+            "condition_keys": [
+                "aws:ResourceTag/${TagKey}",
+                "ec2:AvailabilityZone",
+                "ec2:EbsOptimized",
+                "ec2:InstanceAutoRecovery",
+                "ec2:InstanceID",
+                "ec2:InstanceMarketType",
+                "ec2:InstanceMetadataTags",
+                "ec2:InstanceProfile",
+                "ec2:InstanceType",
+                "ec2:MetadataHttpEndpoint",
+                "ec2:MetadataHttpPutResponseHopLimit",
+                "ec2:MetadataHttpTokens",
+                "ec2:PlacementGroup",
+                "ec2:ProductCode",
+                "ec2:Region",
+                "ec2:ResourceTag/${TagKey}",
+                "ec2:RootDeviceType",
+                "ec2:Tenancy"
+            ],
+            "description": "Grants permission to retrieve the encrypted administrator password for a running Windows instance",
             "orphan": false,
-            "resources": []
+            "resources": [
+                "instance"
+            ]
         },
         "GetReservedInstancesExchangeQuote": {
-            "access_level": "Undocumented",
+            "access_level": "Read",
             "action": "GetReservedInstancesExchangeQuote",
-            "condition_keys": [],
-            "description": "Not Documented by AWS",
+            "condition_keys": [
+                "ec2:Region"
+            ],
+            "description": "Grants permission to return a quote and exchange information for exchanging one or more Convertible Reserved Instances for a new Convertible Reserved Instance",
             "orphan": false,
             "resources": []
         },
         "GetResourcePolicy": {
-            "access_level": "Undocumented",
+            "access_level": "Read",
             "action": "GetResourcePolicy",
-            "condition_keys": [],
-            "description": "Not Documented by AWS",
+            "condition_keys": [
+                "aws:ResourceTag/${TagKey}",
+                "ec2:PlacementGroupName",
+                "ec2:PlacementGroupStrategy",
+                "ec2:Region",
+                "ec2:ResourceTag/${TagKey}"
+            ],
+            "description": "Grants permission to describe an IAM policy that enables cross-account sharing",
             "orphan": false,
-            "resources": []
+            "resources": [
+                "ipam-pool",
+                "placement-group",
+                "verified-access-group"
+            ]
         },
         "GetSerialConsoleAccessStatus": {
-            "access_level": "Undocumented",
+            "access_level": "Read",
             "action": "GetSerialConsoleAccessStatus",
-            "condition_keys": [],
-            "description": "Not Documented by AWS",
+            "condition_keys": [
+                "ec2:Region"
+            ],
+            "description": "Grants permission to retrieve the access status of your account to the EC2 serial console of all instances",
             "orphan": false,
             "resources": []
         },
         "GetSpotPlacementScores": {
-            "access_level": "Undocumented",
+            "access_level": "Read",
             "action": "GetSpotPlacementScores",
-            "condition_keys": [],
-            "description": "Not Documented by AWS",
+            "condition_keys": [
+                "ec2:Region"
+            ],
+            "description": "Grants permission to calculate the Spot placement score for a Region or Availability Zone based on the specified target capacity and compute requirements",
             "orphan": false,
             "resources": []
         },
         "GetSubnetCidrReservations": {
-            "access_level": "Undocumented",
+            "access_level": "Read",
             "action": "GetSubnetCidrReservations",
-            "condition_keys": [],
-            "description": "Not Documented by AWS",
+            "condition_keys": [
+                "ec2:Region"
+            ],
+            "description": "Grants permission to retrieve information about the subnet CIDR reservations",
             "orphan": false,
             "resources": []
         },
         "GetTransitGatewayAttachmentPropagations": {
-            "access_level": "Undocumented",
+            "access_level": "List",
             "action": "GetTransitGatewayAttachmentPropagations",
-            "condition_keys": [],
-            "description": "Not Documented by AWS",
+            "condition_keys": [
+                "ec2:Region"
+            ],
+            "description": "Grants permission to list the route tables to which a resource attachment propagates routes",
             "orphan": false,
             "resources": []
         },
         "GetTransitGatewayMulticastDomainAssociations": {
-            "access_level": "Undocumented",
+            "access_level": "List",
             "action": "GetTransitGatewayMulticastDomainAssociations",
-            "condition_keys": [],
-            "description": "Not Documented by AWS",
+            "condition_keys": [
+                "aws:ResourceTag/${TagKey}",
+                "ec2:Region",
+                "ec2:ResourceTag/${TagKey}"
+            ],
+            "description": "Grants permission to get information about the associations for a transit gateway multicast domain",
             "orphan": false,
-            "resources": []
+            "resources": [
+                "transit-gateway-multicast-domain"
+            ]
         },
         "GetTransitGatewayPolicyTableAssociations": {
-            "access_level": "Undocumented",
+            "access_level": "List",
             "action": "GetTransitGatewayPolicyTableAssociations",
-            "condition_keys": [],
-            "description": "Not Documented by AWS",
+            "condition_keys": [
+                "aws:ResourceTag/${TagKey}",
+                "ec2:Region",
+                "ec2:ResourceTag/${TagKey}"
+            ],
+            "description": "Grants permission to get information about associations for a transit gateway policy table",
             "orphan": false,
-            "resources": []
+            "resources": [
+                "transit-gateway-policy-table"
+            ]
         },
         "GetTransitGatewayPolicyTableEntries": {
-            "access_level": "Undocumented",
+            "access_level": "List",
             "action": "GetTransitGatewayPolicyTableEntries",
-            "condition_keys": [],
-            "description": "Not Documented by AWS",
+            "condition_keys": [
+                "aws:ResourceTag/${TagKey}",
+                "ec2:Region",
+                "ec2:ResourceTag/${TagKey}"
+            ],
+            "description": "Grants permission to get information about associations for a transit gateway policy table entry",
             "orphan": false,
-            "resources": []
+            "resources": [
+                "transit-gateway-policy-table"
+            ]
         },
         "GetTransitGatewayPrefixListReferences": {
-            "access_level": "Undocumented",
+            "access_level": "List",
             "action": "GetTransitGatewayPrefixListReferences",
-            "condition_keys": [],
-            "description": "Not Documented by AWS",
+            "condition_keys": [
+                "ec2:Region"
+            ],
+            "description": "Grants permission to get information about prefix list references for a transit gateway route table",
             "orphan": false,
             "resources": []
         },
         "GetTransitGatewayRouteTableAssociations": {
-            "access_level": "Undocumented",
+            "access_level": "List",
             "action": "GetTransitGatewayRouteTableAssociations",
-            "condition_keys": [],
-            "description": "Not Documented by AWS",
+            "condition_keys": [
+                "ec2:Region"
+            ],
+            "description": "Grants permission to get information about associations for a transit gateway route table",
             "orphan": false,
             "resources": []
         },
         "GetTransitGatewayRouteTablePropagations": {
-            "access_level": "Undocumented",
+            "access_level": "List",
             "action": "GetTransitGatewayRouteTablePropagations",
-            "condition_keys": [],
-            "description": "Not Documented by AWS",
+            "condition_keys": [
+                "ec2:Region"
+            ],
+            "description": "Grants permission to get information about the route table propagations for a transit gateway route table",
             "orphan": false,
             "resources": []
         },
         "GetVerifiedAccessEndpointPolicy": {
-            "access_level": "Undocumented",
+            "access_level": "List",
             "action": "GetVerifiedAccessEndpointPolicy",
-            "condition_keys": [],
-            "description": "Not Documented by AWS",
+            "condition_keys": [
+                "aws:ResourceTag/${TagKey}",
+                "ec2:Region",
+                "ec2:ResourceTag/${TagKey}"
+            ],
+            "description": "Grants permission to show the Verified Access policy associated with the endpoint",
             "orphan": false,
-            "resources": []
+            "resources": [
+                "verified-access-endpoint"
+            ]
         },
         "GetVerifiedAccessGroupPolicy": {
-            "access_level": "Undocumented",
+            "access_level": "List",
             "action": "GetVerifiedAccessGroupPolicy",
-            "condition_keys": [],
-            "description": "Not Documented by AWS",
+            "condition_keys": [
+                "aws:ResourceTag/${TagKey}",
+                "ec2:Region",
+                "ec2:ResourceTag/${TagKey}"
+            ],
+            "description": "Grants permission to show the contents of the Verified Access policy associated with the group",
             "orphan": false,
-            "resources": []
+            "resources": [
+                "verified-access-group"
+            ]
         },
         "GetVerifiedAccessInstanceWebAcl": {
-            "access_level": "Undocumented",
+            "access_level": "List",
             "action": "GetVerifiedAccessInstanceWebAcl",
-            "condition_keys": [],
-            "description": "Not Documented by AWS",
+            "condition_keys": [
+                "aws:ResourceTag/${TagKey}",
+                "ec2:Region",
+                "ec2:ResourceTag/${TagKey}"
+            ],
+            "description": "Grants permission to show the AWS Web Application Firewall (WAF) web access control list (ACL) for a Verified Access instance",
             "orphan": false,
-            "resources": []
+            "resources": [
+                "verified-access-instance"
+            ]
         },
         "GetVpnConnectionDeviceSampleConfiguration": {
-            "access_level": "Undocumented",
+            "access_level": "List",
             "action": "GetVpnConnectionDeviceSampleConfiguration",
-            "condition_keys": [],
-            "description": "Not Documented by AWS",
+            "condition_keys": [
+                "aws:ResourceTag/${TagKey}",
+                "ec2:Region",
+                "ec2:ResourceTag/${TagKey}"
+            ],
+            "description": "Grants permission to download an AWS-provided sample configuration file to be used with the customer gateway device",
             "orphan": false,
-            "resources": []
+            "resources": [
+                "vpn-connection",
+                "vpn-connection-device-type"
+            ]
         },
         "GetVpnConnectionDeviceTypes": {
-            "access_level": "Undocumented",
+            "access_level": "List",
             "action": "GetVpnConnectionDeviceTypes",
-            "condition_keys": [],
-            "description": "Not Documented by AWS",
+            "condition_keys": [
+                "ec2:Region"
+            ],
+            "description": "Grants permission to obtain a list of customer gateway devices for which sample configuration files can be provided",
             "orphan": false,
             "resources": []
         },
         "GetVpnTunnelReplacementStatus": {
-            "access_level": "Undocumented",
+            "access_level": "List",
             "action": "GetVpnTunnelReplacementStatus",
-            "condition_keys": [],
-            "description": "Not Documented by AWS",
+            "condition_keys": [
+                "aws:ResourceTag/${TagKey}",
+                "ec2:Region",
+                "ec2:ResourceTag/${TagKey}"
+            ],
+            "description": "Grants permission to view available tunnel endpoint maintenance events",
             "orphan": false,
-            "resources": []
+            "resources": [
+                "vpn-connection"
+            ]
         },
         "ImportByoipCidrToIpam": {
-            "access_level": "Undocumented",
+            "access_level": "Write",
             "action": "ImportByoipCidrToIpam",
-            "condition_keys": [],
-            "description": "Not Documented by AWS",
+            "condition_keys": [
+                "aws:ResourceTag/${TagKey}",
+                "ec2:Region",
+                "ec2:ResourceTag/${TagKey}"
+            ],
+            "description": "Grants permission to transfer existing BYOIP IPv4 CIDRs to IPAM",
             "orphan": false,
-            "resources": []
+            "resources": [
+                "ipam-pool"
+            ]
         },
         "ImportClientVpnClientCertificateRevocationList": {
-            "access_level": "Undocumented",
+            "access_level": "Write",
             "action": "ImportClientVpnClientCertificateRevocationList",
-            "condition_keys": [],
-            "description": "Not Documented by AWS",
+            "condition_keys": [
+                "aws:ResourceTag/${TagKey}",
+                "ec2:ClientRootCertificateChainArn",
+                "ec2:CloudwatchLogGroupArn",
+                "ec2:CloudwatchLogStreamArn",
+                "ec2:DirectoryArn",
+                "ec2:Region",
+                "ec2:ResourceTag/${TagKey}",
+                "ec2:SamlProviderArn",
+                "ec2:ServerCertificateArn"
+            ],
+            "description": "Grants permission to upload a client certificate revocation list to a Client VPN endpoint",
             "orphan": false,
-            "resources": []
+            "resources": [
+                "client-vpn-endpoint"
+            ]
         },
         "ImportImage": {
-            "access_level": "Undocumented",
+            "access_level": "Write",
             "action": "ImportImage",
-            "condition_keys": [],
-            "description": "Not Documented by AWS",
+            "condition_keys": [
+                "aws:RequestTag/${TagKey}",
+                "aws:ResourceTag/${TagKey}",
+                "aws:TagKeys",
+                "ec2:ImageID",
+                "ec2:ImageType",
+                "ec2:Owner",
+                "ec2:ParentVolume",
+                "ec2:Public",
+                "ec2:Region",
+                "ec2:ResourceTag/${TagKey}",
+                "ec2:RootDeviceType",
+                "ec2:SnapshotID",
+                "ec2:SnapshotTime",
+                "ec2:VolumeSize"
+            ],
+            "description": "Grants permission to import single or multi-volume disk images or EBS snapshots into an Amazon Machine Image (AMI)",
             "orphan": false,
-            "resources": []
+            "resources": [
+                "image",
+                "import-image-task",
+                "snapshot"
+            ]
         },
         "ImportInstance": {
-            "access_level": "Undocumented",
+            "access_level": "Write",
             "action": "ImportInstance",
-            "condition_keys": [],
-            "description": "Not Documented by AWS",
+            "condition_keys": [
+                "aws:ResourceTag/${TagKey}",
+                "ec2:AvailabilityZone",
+                "ec2:Encrypted",
+                "ec2:InstanceID",
+                "ec2:ParentSnapshot",
+                "ec2:Region",
+                "ec2:ResourceTag/${TagKey}",
+                "ec2:SecurityGroupID",
+                "ec2:SubnetID",
+                "ec2:VolumeID",
+                "ec2:VolumeIops",
+                "ec2:VolumeSize",
+                "ec2:VolumeThroughput",
+                "ec2:VolumeType",
+                "ec2:Vpc"
+            ],
+            "description": "Grants permission to create an import instance task using metadata from a disk image",
             "orphan": false,
-            "resources": []
+            "resources": [
+                "instance",
+                "security-group",
+                "subnet",
+                "volume"
+            ]
         },
         "ImportKeyPair": {
-            "access_level": "Undocumented",
+            "access_level": "Write",
             "action": "ImportKeyPair",
-            "condition_keys": [],
-            "description": "Not Documented by AWS",
+            "condition_keys": [
+                "aws:RequestTag/${TagKey}",
+                "aws:TagKeys",
+                "ec2:Region"
+            ],
+            "description": "Grants permission to import a public key from an RSA key pair that was created with a third-party tool",
             "orphan": false,
-            "resources": []
+            "resources": [
+                "key-pair"
+            ]
         },
         "ImportSnapshot": {
-            "access_level": "Undocumented",
+            "access_level": "Write",
             "action": "ImportSnapshot",
-            "condition_keys": [],
-            "description": "Not Documented by AWS",
+            "condition_keys": [
+                "aws:RequestTag/${TagKey}",
+                "aws:TagKeys",
+                "ec2:Owner",
+                "ec2:ParentVolume",
+                "ec2:Region",
+                "ec2:SnapshotID",
+                "ec2:SnapshotTime",
+                "ec2:VolumeSize"
+            ],
+            "description": "Grants permission to import a disk into an EBS snapshot",
             "orphan": false,
-            "resources": []
+            "resources": [
+                "import-snapshot-task",
+                "snapshot"
+            ]
         },
         "ImportVolume": {
-            "access_level": "Undocumented",
+            "access_level": "Write",
             "action": "ImportVolume",
-            "condition_keys": [],
-            "description": "Not Documented by AWS",
+            "condition_keys": [
+                "aws:ResourceTag/${TagKey}",
+                "ec2:AvailabilityZone",
+                "ec2:Encrypted",
+                "ec2:ParentSnapshot",
+                "ec2:Region",
+                "ec2:ResourceTag/${TagKey}",
+                "ec2:VolumeID",
+                "ec2:VolumeIops",
+                "ec2:VolumeSize",
+                "ec2:VolumeThroughput",
+                "ec2:VolumeType"
+            ],
+            "description": "Grants permission to create an import volume task using metadata from a disk image",
             "orphan": false,
-            "resources": []
+            "resources": [
+                "volume"
+            ]
         },
         "ListImagesInRecycleBin": {
-            "access_level": "Undocumented",
+            "access_level": "List",
             "action": "ListImagesInRecycleBin",
-            "condition_keys": [],
-            "description": "Not Documented by AWS",
+            "condition_keys": [
+                "ec2:Region"
+            ],
+            "description": "Grants permission to list Amazon Machine Images (AMIs) that are currently in the Recycle Bin",
             "orphan": false,
             "resources": []
         },
         "ListSnapshotsInRecycleBin": {
-            "access_level": "Undocumented",
+            "access_level": "List",
             "action": "ListSnapshotsInRecycleBin",
-            "condition_keys": [],
-            "description": "Not Documented by AWS",
+            "condition_keys": [
+                "ec2:Region"
+            ],
+            "description": "Grants permission to list the Amazon EBS snapshots that are currently in the Recycle Bin",
             "orphan": false,
             "resources": []
         },
         "ModifyAddressAttribute": {
-            "access_level": "Undocumented",
+            "access_level": "Write",
             "action": "ModifyAddressAttribute",
-            "condition_keys": [],
-            "description": "Not Documented by AWS",
+            "condition_keys": [
+                "aws:ResourceTag/${TagKey}",
+                "ec2:AllocationId",
+                "ec2:Attribute",
+                "ec2:Attribute/${AttributeName}",
+                "ec2:Domain",
+                "ec2:PublicIpAddress",
+                "ec2:Region",
+                "ec2:ResourceTag/${TagKey}"
+            ],
+            "description": "Grants permission to modify an attribute of the specified Elastic IP address",
             "orphan": false,
-            "resources": []
+            "resources": [
+                "elastic-ip"
+            ]
         },
         "ModifyAvailabilityZoneGroup": {
-            "access_level": "Undocumented",
+            "access_level": "Write",
             "action": "ModifyAvailabilityZoneGroup",
-            "condition_keys": [],
-            "description": "Not Documented by AWS",
+            "condition_keys": [
+                "ec2:Region"
+            ],
+            "description": "Grants permission to modify the opt-in status of the Local Zone and Wavelength Zone group for your account",
             "orphan": false,
             "resources": []
         },
         "ModifyCapacityReservation": {
-            "access_level": "Undocumented",
+            "access_level": "Write",
             "action": "ModifyCapacityReservation",
-            "condition_keys": [],
-            "description": "Not Documented by AWS",
+            "condition_keys": [
+                "aws:ResourceTag/${TagKey}",
+                "ec2:Attribute",
+                "ec2:Attribute/${AttributeName}",
+                "ec2:CapacityReservationFleet",
+                "ec2:Region",
+                "ec2:ResourceTag/${TagKey}"
+            ],
+            "description": "Grants permission to modify a Capacity Reservation's capacity and the conditions under which it is to be released",
             "orphan": false,
-            "resources": []
+            "resources": [
+                "capacity-reservation"
+            ]
         },
         "ModifyCapacityReservationFleet": {
-            "access_level": "Undocumented",
+            "access_level": "Write",
             "action": "ModifyCapacityReservationFleet",
-            "condition_keys": [],
-            "description": "Not Documented by AWS",
+            "condition_keys": [
+                "aws:ResourceTag/${TagKey}",
+                "ec2:Attribute",
+                "ec2:Attribute/${AttributeName}",
+                "ec2:Region",
+                "ec2:ResourceTag/${TagKey}"
+            ],
+            "description": "Grants permission to modify a Capacity Reservation Fleet",
             "orphan": false,
-            "resources": []
+            "resources": [
+                "capacity-reservation-fleet"
+            ]
         },
         "ModifyClientVpnEndpoint": {
-            "access_level": "Undocumented",
+            "access_level": "Write",
             "action": "ModifyClientVpnEndpoint",
-            "condition_keys": [],
-            "description": "Not Documented by AWS",
-            "orphan": false,
-            "resources": []
+            "condition_keys": [
+                "aws:ResourceTag/${TagKey}",
+                "ec2:Attribute",
+                "ec2:Attribute/${AttributeName}",
+                "ec2:ClientRootCertificateChainArn",
+                "ec2:CloudwatchLogGroupArn",
+                "ec2:CloudwatchLogStreamArn",
+                "ec2:DirectoryArn",
+                "ec2:Region",
+                "ec2:ResourceTag/${TagKey}",
+                "ec2:SamlProviderArn",
+                "ec2:SecurityGroupID",
+                "ec2:ServerCertificateArn",
+                "ec2:VpcID"
+            ],
+            "description": "Grants permission to modify a Client VPN endpoint",
+            "orphan": false,
+            "resources": [
+                "client-vpn-endpoint",
+                "security-group",
+                "vpc"
+            ]
         },
         "ModifyDefaultCreditSpecification": {
-            "access_level": "Undocumented",
+            "access_level": "Write",
             "action": "ModifyDefaultCreditSpecification",
-            "condition_keys": [],
-            "description": "Not Documented by AWS",
+            "condition_keys": [
+                "ec2:Region"
+            ],
+            "description": "Grants permission to change the account level default credit option for CPU usage of burstable performance instances",
             "orphan": false,
             "resources": []
         },
         "ModifyEbsDefaultKmsKeyId": {
-            "access_level": "Undocumented",
+            "access_level": "Write",
             "action": "ModifyEbsDefaultKmsKeyId",
-            "condition_keys": [],
-            "description": "Not Documented by AWS",
+            "condition_keys": [
+                "ec2:Region"
+            ],
+            "description": "Grants permission to change the default customer master key (CMK) for EBS encryption by default for your account",
             "orphan": false,
             "resources": []
         },
         "ModifyFleet": {
-            "access_level": "Undocumented",
+            "access_level": "Write",
             "action": "ModifyFleet",
-            "condition_keys": [],
-            "description": "Not Documented by AWS",
+            "condition_keys": [
+                "aws:ResourceTag/${TagKey}",
+                "ec2:Attribute",
+                "ec2:Attribute/${AttributeName}",
+                "ec2:AvailabilityZone",
+                "ec2:ImageID",
+                "ec2:ImageType",
+                "ec2:KeyPairName",
+                "ec2:NetworkInterfaceID",
+                "ec2:Owner",
+                "ec2:ParentVolume",
+                "ec2:Public",
+                "ec2:Region",
+                "ec2:ResourceTag/${TagKey}",
+                "ec2:RootDeviceType",
+                "ec2:SecurityGroupID",
+                "ec2:SnapshotID",
+                "ec2:SnapshotTime",
+                "ec2:Subnet",
+                "ec2:SubnetID",
+                "ec2:VolumeSize",
+                "ec2:Vpc"
+            ],
+            "description": "Grants permission to modify an EC2 Fleet",
             "orphan": false,
-            "resources": []
+            "resources": [
+                "fleet",
+                "image",
+                "key-pair",
+                "launch-template",
+                "network-interface",
+                "security-group",
+                "snapshot",
+                "subnet"
+            ]
         },
         "ModifyFpgaImageAttribute": {
-            "access_level": "Undocumented",
+            "access_level": "Write",
             "action": "ModifyFpgaImageAttribute",
-            "condition_keys": [],
-            "description": "Not Documented by AWS",
+            "condition_keys": [
+                "aws:ResourceTag/${TagKey}",
+                "ec2:Attribute",
+                "ec2:Attribute/${AttributeName}",
+                "ec2:Owner",
+                "ec2:Public",
+                "ec2:Region",
+                "ec2:ResourceTag/${TagKey}"
+            ],
+            "description": "Grants permission to modify an attribute of an Amazon FPGA Image (AFI)",
             "orphan": false,
-            "resources": []
+            "resources": [
+                "fpga-image"
+            ]
         },
         "ModifyHosts": {
-            "access_level": "Undocumented",
+            "access_level": "Write",
             "action": "ModifyHosts",
-            "condition_keys": [],
-            "description": "Not Documented by AWS",
+            "condition_keys": [
+                "aws:ResourceTag/${TagKey}",
+                "ec2:Attribute",
+                "ec2:Attribute/${AttributeName}",
+                "ec2:Region",
+                "ec2:ResourceTag/${TagKey}"
+            ],
+            "description": "Grants permission to modify a Dedicated Host",
             "orphan": false,
-            "resources": []
+            "resources": [
+                "dedicated-host"
+            ]
         },
         "ModifyIdFormat": {
-            "access_level": "Undocumented",
+            "access_level": "Write",
             "action": "ModifyIdFormat",
-            "condition_keys": [],
-            "description": "Not Documented by AWS",
+            "condition_keys": [
+                "ec2:Region"
+            ],
+            "description": "Grants permission to modify the ID format for a resource",
             "orphan": false,
             "resources": []
         },
         "ModifyIdentityIdFormat": {
-            "access_level": "Undocumented",
+            "access_level": "Write",
             "action": "ModifyIdentityIdFormat",
-            "condition_keys": [],
-            "description": "Not Documented by AWS",
+            "condition_keys": [
+                "ec2:Region"
+            ],
+            "description": "Grants permission to modify the ID format of a resource for a specific principal in your account",
             "orphan": false,
             "resources": []
         },
         "ModifyImageAttribute": {
-            "access_level": "Undocumented",
+            "access_level": "Write",
             "action": "ModifyImageAttribute",
-            "condition_keys": [],
-            "description": "Not Documented by AWS",
+            "condition_keys": [
+                "aws:ResourceTag/${TagKey}",
+                "ec2:Attribute",
+                "ec2:Attribute/${AttributeName}",
+                "ec2:ImageID",
+                "ec2:ImageType",
+                "ec2:Owner",
+                "ec2:Public",
+                "ec2:Region",
+                "ec2:ResourceTag/${TagKey}",
+                "ec2:RootDeviceType"
+            ],
+            "description": "Grants permission to modify an attribute of an Amazon Machine Image (AMI)",
             "orphan": false,
-            "resources": []
+            "resources": [
+                "image"
+            ]
         },
         "ModifyInstanceAttribute": {
-            "access_level": "Undocumented",
+            "access_level": "Write",
             "action": "ModifyInstanceAttribute",
-            "condition_keys": [],
-            "description": "Not Documented by AWS",
+            "condition_keys": [
+                "aws:ResourceTag/${TagKey}",
+                "ec2:Attribute",
+                "ec2:Attribute/${AttributeName}",
+                "ec2:AvailabilityZone",
+                "ec2:EbsOptimized",
+                "ec2:Encrypted",
+                "ec2:InstanceAutoRecovery",
+                "ec2:InstanceID",
+                "ec2:InstanceMarketType",
+                "ec2:InstanceMetadataTags",
+                "ec2:InstanceProfile",
+                "ec2:InstanceType",
+                "ec2:MetadataHttpEndpoint",
+                "ec2:MetadataHttpPutResponseHopLimit",
+                "ec2:MetadataHttpTokens",
+                "ec2:ParentSnapshot",
+                "ec2:PlacementGroup",
+                "ec2:ProductCode",
+                "ec2:Region",
+                "ec2:ResourceTag/${TagKey}",
+                "ec2:RootDeviceType",
+                "ec2:SecurityGroupID",
+                "ec2:Tenancy",
+                "ec2:VolumeID",
+                "ec2:VolumeIops",
+                "ec2:VolumeSize",
+                "ec2:VolumeThroughput",
+                "ec2:VolumeType",
+                "ec2:Vpc"
+            ],
+            "description": "Grants permission to modify an attribute of an instance",
             "orphan": false,
-            "resources": []
+            "resources": [
+                "instance",
+                "security-group",
+                "volume"
+            ]
         },
         "ModifyInstanceCapacityReservationAttributes": {
-            "access_level": "Undocumented",
+            "access_level": "Write",
             "action": "ModifyInstanceCapacityReservationAttributes",
-            "condition_keys": [],
-            "description": "Not Documented by AWS",
+            "condition_keys": [
+                "aws:ResourceTag/${TagKey}",
+                "ec2:Attribute",
+                "ec2:Attribute/${AttributeName}",
+                "ec2:AvailabilityZone",
+                "ec2:EbsOptimized",
+                "ec2:InstanceAutoRecovery",
+                "ec2:InstanceID",
+                "ec2:InstanceMarketType",
+                "ec2:InstanceMetadataTags",
+                "ec2:InstanceProfile",
+                "ec2:InstanceType",
+                "ec2:MetadataHttpEndpoint",
+                "ec2:MetadataHttpPutResponseHopLimit",
+                "ec2:MetadataHttpTokens",
+                "ec2:PlacementGroup",
+                "ec2:ProductCode",
+                "ec2:Region",
+                "ec2:ResourceTag/${TagKey}",
+                "ec2:RootDeviceType",
+                "ec2:Tenancy"
+            ],
+            "description": "Grants permission to modify the Capacity Reservation settings for a stopped instance",
             "orphan": false,
-            "resources": []
+            "resources": [
+                "capacity-reservation",
+                "instance"
+            ]
         },
         "ModifyInstanceCreditSpecification": {
-            "access_level": "Undocumented",
+            "access_level": "Write",
             "action": "ModifyInstanceCreditSpecification",
-            "condition_keys": [],
-            "description": "Not Documented by AWS",
+            "condition_keys": [
+                "aws:ResourceTag/${TagKey}",
+                "ec2:Attribute",
+                "ec2:Attribute/${AttributeName}",
+                "ec2:AvailabilityZone",
+                "ec2:EbsOptimized",
+                "ec2:InstanceAutoRecovery",
+                "ec2:InstanceID",
+                "ec2:InstanceMarketType",
+                "ec2:InstanceMetadataTags",
+                "ec2:InstanceProfile",
+                "ec2:InstanceType",
+                "ec2:MetadataHttpEndpoint",
+                "ec2:MetadataHttpPutResponseHopLimit",
+                "ec2:MetadataHttpTokens",
+                "ec2:PlacementGroup",
+                "ec2:ProductCode",
+                "ec2:Region",
+                "ec2:ResourceTag/${TagKey}",
+                "ec2:RootDeviceType",
+                "ec2:Tenancy"
+            ],
+            "description": "Grants permission to modify the credit option for CPU usage on an instance",
             "orphan": false,
-            "resources": []
+            "resources": [
+                "instance"
+            ]
         },
         "ModifyInstanceEventStartTime": {
-            "access_level": "Undocumented",
+            "access_level": "Write",
             "action": "ModifyInstanceEventStartTime",
-            "condition_keys": [],
-            "description": "Not Documented by AWS",
+            "condition_keys": [
+                "aws:ResourceTag/${TagKey}",
+                "ec2:Attribute/${AttributeName}",
+                "ec2:InstanceID",
+                "ec2:Region",
+                "ec2:ResourceTag/${TagKey}"
+            ],
+            "description": "Grants permission to modify the start time for a scheduled EC2 instance event",
             "orphan": false,
-            "resources": []
+            "resources": [
+                "instance"
+            ]
         },
         "ModifyInstanceEventWindow": {
-            "access_level": "Undocumented",
+            "access_level": "Write",
             "action": "ModifyInstanceEventWindow",
-            "condition_keys": [],
-            "description": "Not Documented by AWS",
+            "condition_keys": [
+                "aws:ResourceTag/${TagKey}",
+                "ec2:Region",
+                "ec2:ResourceTag/${TagKey}"
+            ],
+            "description": "Grants permission to modify the specified event window",
             "orphan": false,
-            "resources": []
+            "resources": [
+                "instance-event-window"
+            ]
         },
         "ModifyInstanceMaintenanceOptions": {
-            "access_level": "Undocumented",
+            "access_level": "Write",
             "action": "ModifyInstanceMaintenanceOptions",
-            "condition_keys": [],
-            "description": "Not Documented by AWS",
+            "condition_keys": [
+                "aws:ResourceTag/${TagKey}",
+                "ec2:Attribute",
+                "ec2:Attribute/${AttributeName}",
+                "ec2:AvailabilityZone",
+                "ec2:EbsOptimized",
+                "ec2:InstanceAutoRecovery",
+                "ec2:InstanceID",
+                "ec2:InstanceMarketType",
+                "ec2:InstanceMetadataTags",
+                "ec2:InstanceProfile",
+                "ec2:InstanceType",
+                "ec2:MetadataHttpEndpoint",
+                "ec2:MetadataHttpPutResponseHopLimit",
+                "ec2:MetadataHttpTokens",
+                "ec2:PlacementGroup",
+                "ec2:ProductCode",
+                "ec2:Region",
+                "ec2:ResourceTag/${TagKey}",
+                "ec2:RootDeviceType",
+                "ec2:Tenancy"
+            ],
+            "description": "Grants permission to modify the recovery behaviour for an instance",
             "orphan": false,
-            "resources": []
+            "resources": [
+                "instance"
+            ]
         },
         "ModifyInstanceMetadataOptions": {
-            "access_level": "Undocumented",
+            "access_level": "Write",
             "action": "ModifyInstanceMetadataOptions",
-            "condition_keys": [],
-            "description": "Not Documented by AWS",
+            "condition_keys": [
+                "aws:ResourceTag/${TagKey}",
+                "ec2:Attribute",
+                "ec2:Attribute/${AttributeName}",
+                "ec2:AvailabilityZone",
+                "ec2:EbsOptimized",
+                "ec2:InstanceAutoRecovery",
+                "ec2:InstanceID",
+                "ec2:InstanceMarketType",
+                "ec2:InstanceMetadataTags",
+                "ec2:InstanceProfile",
+                "ec2:InstanceType",
+                "ec2:MetadataHttpEndpoint",
+                "ec2:MetadataHttpPutResponseHopLimit",
+                "ec2:MetadataHttpTokens",
+                "ec2:PlacementGroup",
+                "ec2:ProductCode",
+                "ec2:Region",
+                "ec2:ResourceTag/${TagKey}",
+                "ec2:RootDeviceType",
+                "ec2:Tenancy"
+            ],
+            "description": "Grants permission to modify the metadata options for an instance",
             "orphan": false,
-            "resources": []
+            "resources": [
+                "instance"
+            ]
         },
         "ModifyInstancePlacement": {
-            "access_level": "Undocumented",
+            "access_level": "Write",
             "action": "ModifyInstancePlacement",
-            "condition_keys": [],
-            "description": "Not Documented by AWS",
+            "condition_keys": [
+                "aws:ResourceTag/${TagKey}",
+                "ec2:Attribute",
+                "ec2:Attribute/${AttributeName}",
+                "ec2:AvailabilityZone",
+                "ec2:EbsOptimized",
+                "ec2:InstanceAutoRecovery",
+                "ec2:InstanceID",
+                "ec2:InstanceMarketType",
+                "ec2:InstanceMetadataTags",
+                "ec2:InstanceProfile",
+                "ec2:InstanceType",
+                "ec2:MetadataHttpEndpoint",
+                "ec2:MetadataHttpPutResponseHopLimit",
+                "ec2:MetadataHttpTokens",
+                "ec2:PlacementGroup",
+                "ec2:PlacementGroupName",
+                "ec2:PlacementGroupStrategy",
+                "ec2:ProductCode",
+                "ec2:Region",
+                "ec2:ResourceTag/${TagKey}",
+                "ec2:RootDeviceType",
+                "ec2:Tenancy"
+            ],
+            "description": "Grants permission to modify the placement attributes for an instance",
             "orphan": false,
-            "resources": []
+            "resources": [
+                "dedicated-host",
+                "instance",
+                "placement-group"
+            ]
         },
         "ModifyIpam": {
-            "access_level": "Undocumented",
+            "access_level": "Write",
             "action": "ModifyIpam",
-            "condition_keys": [],
-            "description": "Not Documented by AWS",
+            "condition_keys": [
+                "aws:ResourceTag/${TagKey}",
+                "ec2:Attribute",
+                "ec2:Attribute/${AttributeName}",
+                "ec2:Region",
+                "ec2:ResourceTag/${TagKey}"
+            ],
+            "description": "Grants permission to modify the configurations of an Amazon VPC IP Address Manager (IPAM)",
             "orphan": false,
-            "resources": []
+            "resources": [
+                "ipam"
+            ]
         },
         "ModifyIpamPool": {
-            "access_level": "Undocumented",
+            "access_level": "Write",
             "action": "ModifyIpamPool",
-            "condition_keys": [],
-            "description": "Not Documented by AWS",
+            "condition_keys": [
+                "aws:ResourceTag/${TagKey}",
+                "ec2:Attribute",
+                "ec2:Attribute/${AttributeName}",
+                "ec2:Region",
+                "ec2:ResourceTag/${TagKey}"
+            ],
+            "description": "Grants permission to modify the configurations of an Amazon VPC IP Address Manager (IPAM) pool",
             "orphan": false,
-            "resources": []
+            "resources": [
+                "ipam-pool"
+            ]
         },
         "ModifyIpamResourceCidr": {
-            "access_level": "Undocumented",
+            "access_level": "Write",
             "action": "ModifyIpamResourceCidr",
-            "condition_keys": [],
-            "description": "Not Documented by AWS",
+            "condition_keys": [
+                "aws:ResourceTag/${TagKey}",
+                "ec2:Attribute",
+                "ec2:Attribute/${AttributeName}",
+                "ec2:Region",
+                "ec2:ResourceTag/${TagKey}"
+            ],
+            "description": "Grants permission to modify the configurations of an Amazon VPC IP Address Manager (IPAM) resource CIDR",
             "orphan": false,
-            "resources": []
+            "resources": [
+                "ipam-scope"
+            ]
         },
         "ModifyIpamResourceDiscovery": {
-            "access_level": "Undocumented",
+            "access_level": "Write",
             "action": "ModifyIpamResourceDiscovery",
-            "condition_keys": [],
-            "description": "Not Documented by AWS",
+            "condition_keys": [
+                "aws:ResourceTag/${TagKey}",
+                "ec2:Region",
+                "ec2:ResourceTag/${TagKey}"
+            ],
+            "description": "Grants permission to modify a resource discovery",
             "orphan": false,
-            "resources": []
+            "resources": [
+                "ipam-resource-discovery"
+            ]
         },
         "ModifyIpamScope": {
-            "access_level": "Undocumented",
+            "access_level": "Write",
             "action": "ModifyIpamScope",
-            "condition_keys": [],
-            "description": "Not Documented by AWS",
+            "condition_keys": [
+                "aws:ResourceTag/${TagKey}",
+                "ec2:Attribute",
+                "ec2:Attribute/${AttributeName}",
+                "ec2:Region",
+                "ec2:ResourceTag/${TagKey}"
+            ],
+            "description": "Grants permission to modify the configurations of an Amazon VPC IP Address Manager (IPAM) scope",
             "orphan": false,
-            "resources": []
+            "resources": [
+                "ipam-scope"
+            ]
         },
         "ModifyLaunchTemplate": {
-            "access_level": "Undocumented",
+            "access_level": "Write",
             "action": "ModifyLaunchTemplate",
-            "condition_keys": [],
-            "description": "Not Documented by AWS",
+            "condition_keys": [
+                "aws:ResourceTag/${TagKey}",
+                "ec2:Attribute",
+                "ec2:Attribute/${AttributeName}",
+                "ec2:Region",
+                "ec2:ResourceTag/${TagKey}"
+            ],
+            "description": "Grants permission to modify a launch template",
             "orphan": false,
-            "resources": []
+            "resources": [
+                "launch-template"
+            ]
         },
         "ModifyLocalGatewayRoute": {
-            "access_level": "Undocumented",
+            "access_level": "Write",
             "action": "ModifyLocalGatewayRoute",
-            "condition_keys": [],
-            "description": "Not Documented by AWS",
-            "orphan": false,
-            "resources": []
+            "condition_keys": [
+                "aws:ResourceTag/${TagKey}",
+                "ec2:AuthorizedUser",
+                "ec2:AvailabilityZone",
+                "ec2:NetworkInterfaceID",
+                "ec2:Permission",
+                "ec2:Region",
+                "ec2:ResourceTag/${TagKey}",
+                "ec2:Subnet",
+                "ec2:Vpc"
+            ],
+            "description": "Grants permission to modify a local gateway route",
+            "orphan": false,
+            "resources": [
+                "local-gateway-route-table",
+                "local-gateway-virtual-interface-group",
+                "network-interface",
+                "prefix-list"
+            ]
         },
         "ModifyManagedPrefixList": {
-            "access_level": "Undocumented",
+            "access_level": "Write",
             "action": "ModifyManagedPrefixList",
-            "condition_keys": [],
-            "description": "Not Documented by AWS",
+            "condition_keys": [
+                "aws:ResourceTag/${TagKey}",
+                "ec2:Attribute",
+                "ec2:Attribute/${AttributeName}",
+                "ec2:Region",
+                "ec2:ResourceTag/${TagKey}"
+            ],
+            "description": "Grants permission to modify a managed prefix list",
             "orphan": false,
-            "resources": []
+            "resources": [
+                "prefix-list"
+            ]
         },
         "ModifyNetworkInterfaceAttribute": {
-            "access_level": "Undocumented",
+            "access_level": "Write",
             "action": "ModifyNetworkInterfaceAttribute",
-            "condition_keys": [],
-            "description": "Not Documented by AWS",
+            "condition_keys": [
+                "aws:ResourceTag/${TagKey}",
+                "ec2:Attribute",
+                "ec2:Attribute/${AttributeName}",
+                "ec2:AvailabilityZone",
+                "ec2:EbsOptimized",
+                "ec2:InstanceAutoRecovery",
+                "ec2:InstanceID",
+                "ec2:InstanceMarketType",
+                "ec2:InstanceMetadataTags",
+                "ec2:InstanceProfile",
+                "ec2:InstanceType",
+                "ec2:MetadataHttpEndpoint",
+                "ec2:MetadataHttpPutResponseHopLimit",
+                "ec2:MetadataHttpTokens",
+                "ec2:NetworkInterfaceID",
+                "ec2:PlacementGroup",
+                "ec2:ProductCode",
+                "ec2:Region",
+                "ec2:ResourceTag/${TagKey}",
+                "ec2:RootDeviceType",
+                "ec2:SecurityGroupID",
+                "ec2:Subnet",
+                "ec2:Tenancy",
+                "ec2:Vpc"
+            ],
+            "description": "Grants permission to modify an attribute of a network interface",
             "orphan": false,
-            "resources": []
+            "resources": [
+                "instance",
+                "network-interface",
+                "security-group"
+            ]
         },
         "ModifyPrivateDnsNameOptions": {
-            "access_level": "Undocumented",
+            "access_level": "Write",
             "action": "ModifyPrivateDnsNameOptions",
-            "condition_keys": [],
-            "description": "Not Documented by AWS",
+            "condition_keys": [
+                "aws:ResourceTag/${TagKey}",
+                "ec2:Attribute",
+                "ec2:Attribute/${AttributeName}",
+                "ec2:AvailabilityZone",
+                "ec2:EbsOptimized",
+                "ec2:InstanceAutoRecovery",
+                "ec2:InstanceID",
+                "ec2:InstanceMarketType",
+                "ec2:InstanceMetadataTags",
+                "ec2:InstanceProfile",
+                "ec2:InstanceType",
+                "ec2:MetadataHttpEndpoint",
+                "ec2:MetadataHttpPutResponseHopLimit",
+                "ec2:MetadataHttpTokens",
+                "ec2:NewInstanceProfile",
+                "ec2:PlacementGroup",
+                "ec2:ProductCode",
+                "ec2:Region",
+                "ec2:ResourceTag/${TagKey}",
+                "ec2:RootDeviceType",
+                "ec2:Tenancy"
+            ],
+            "description": "Grants permission to modify the options for instance hostnames for the specified instance",
             "orphan": false,
-            "resources": []
+            "resources": [
+                "instance"
+            ]
         },
         "ModifyReservedInstances": {
-            "access_level": "Undocumented",
+            "access_level": "Write",
             "action": "ModifyReservedInstances",
-            "condition_keys": [],
-            "description": "Not Documented by AWS",
+            "condition_keys": [
+                "aws:ResourceTag/${TagKey}",
+                "ec2:Attribute",
+                "ec2:Attribute/${AttributeName}",
+                "ec2:AvailabilityZone",
+                "ec2:InstanceType",
+                "ec2:Region",
+                "ec2:ReservedInstancesOfferingType",
+                "ec2:ResourceTag/${TagKey}",
+                "ec2:Tenancy"
+            ],
+            "description": "Grants permission to modify attributes of one or more Reserved Instances",
             "orphan": false,
-            "resources": []
+            "resources": [
+                "reserved-instances"
+            ]
         },
         "ModifySecurityGroupRules": {
-            "access_level": "Undocumented",
+            "access_level": "Write",
             "action": "ModifySecurityGroupRules",
-            "condition_keys": [],
-            "description": "Not Documented by AWS",
+            "condition_keys": [
+                "aws:ResourceTag/${TagKey}",
+                "ec2:Attribute",
+                "ec2:Attribute/${AttributeName}",
+                "ec2:Region",
+                "ec2:ResourceTag/${TagKey}",
+                "ec2:SecurityGroupID",
+                "ec2:Vpc"
+            ],
+            "description": "Grants permission to modify the rules of a security group",
             "orphan": false,
-            "resources": []
+            "resources": [
+                "prefix-list",
+                "security-group",
+                "security-group-rule"
+            ]
         },
         "ModifySnapshotAttribute": {
-            "access_level": "Undocumented",
+            "access_level": "Permissions management",
             "action": "ModifySnapshotAttribute",
-            "condition_keys": [],
-            "description": "Not Documented by AWS",
+            "condition_keys": [
+                "aws:ResourceTag/${TagKey}",
+                "ec2:Add/group",
+                "ec2:Add/userId",
+                "ec2:Attribute",
+                "ec2:Attribute/${AttributeName}",
+                "ec2:Owner",
+                "ec2:ParentVolume",
+                "ec2:Region",
+                "ec2:Remove/group",
+                "ec2:Remove/userId",
+                "ec2:ResourceTag/${TagKey}",
+                "ec2:SnapshotID",
+                "ec2:SnapshotTime",
+                "ec2:VolumeSize"
+            ],
+            "description": "Grants permission to add or remove permission settings for a snapshot",
             "orphan": false,
-            "resources": []
+            "resources": [
+                "snapshot"
+            ]
         },
         "ModifySnapshotTier": {
-            "access_level": "Undocumented",
+            "access_level": "Write",
             "action": "ModifySnapshotTier",
-            "condition_keys": [],
-            "description": "Not Documented by AWS",
+            "condition_keys": [
+                "aws:ResourceTag/${TagKey}",
+                "ec2:Attribute",
+                "ec2:Attribute/${AttributeName}",
+                "ec2:Encrypted",
+                "ec2:Owner",
+                "ec2:ParentVolume",
+                "ec2:Region",
+                "ec2:ResourceTag/${TagKey}",
+                "ec2:SnapshotID",
+                "ec2:SnapshotTime",
+                "ec2:VolumeSize"
+            ],
+            "description": "Grants permission to archive Amazon EBS snapshots",
             "orphan": false,
-            "resources": []
+            "resources": [
+                "snapshot"
+            ]
         },
         "ModifySpotFleetRequest": {
-            "access_level": "Undocumented",
+            "access_level": "Write",
             "action": "ModifySpotFleetRequest",
-            "condition_keys": [],
-            "description": "Not Documented by AWS",
+            "condition_keys": [
+                "aws:ResourceTag/${TagKey}",
+                "ec2:Attribute",
+                "ec2:Attribute/${AttributeName}",
+                "ec2:AvailabilityZone",
+                "ec2:Region",
+                "ec2:ResourceTag/${TagKey}",
+                "ec2:SubnetID",
+                "ec2:Vpc"
+            ],
+            "description": "Grants permission to modify a Spot Fleet request",
             "orphan": false,
-            "resources": []
+            "resources": [
+                "launch-template",
+                "spot-fleet-request",
+                "subnet"
+            ]
         },
         "ModifySubnetAttribute": {
-            "access_level": "Undocumented",
+            "access_level": "Write",
             "action": "ModifySubnetAttribute",
-            "condition_keys": [],
-            "description": "Not Documented by AWS",
+            "condition_keys": [
+                "aws:ResourceTag/${TagKey}",
+                "ec2:Attribute",
+                "ec2:Attribute/${AttributeName}",
+                "ec2:AvailabilityZone",
+                "ec2:Region",
+                "ec2:ResourceTag/${TagKey}",
+                "ec2:SubnetID",
+                "ec2:Vpc"
+            ],
+            "description": "Grants permission to modify an attribute of a subnet",
             "orphan": false,
-            "resources": []
+            "resources": [
+                "subnet"
+            ]
         },
         "ModifyTrafficMirrorFilterNetworkServices": {
-            "access_level": "Undocumented",
+            "access_level": "Write",
             "action": "ModifyTrafficMirrorFilterNetworkServices",
-            "condition_keys": [],
-            "description": "Not Documented by AWS",
+            "condition_keys": [
+                "aws:ResourceTag/${TagKey}",
+                "ec2:Attribute",
+                "ec2:Attribute/${AttributeName}",
+                "ec2:Region",
+                "ec2:ResourceTag/${TagKey}"
+            ],
+            "description": "Grants permission to allow or restrict mirroring network services",
             "orphan": false,
-            "resources": []
+            "resources": [
+                "traffic-mirror-filter"
+            ]
         },
         "ModifyTrafficMirrorFilterRule": {
-            "access_level": "Undocumented",
+            "access_level": "Write",
             "action": "ModifyTrafficMirrorFilterRule",
-            "condition_keys": [],
-            "description": "Not Documented by AWS",
+            "condition_keys": [
+                "aws:ResourceTag/${TagKey}",
+                "ec2:Attribute",
+                "ec2:Attribute/${AttributeName}",
+                "ec2:Region",
+                "ec2:ResourceTag/${TagKey}"
+            ],
+            "description": "Grants permission to modify a traffic mirror rule",
             "orphan": false,
-            "resources": []
+            "resources": [
+                "traffic-mirror-filter",
+                "traffic-mirror-filter-rule"
+            ]
         },
         "ModifyTrafficMirrorSession": {
-            "access_level": "Undocumented",
+            "access_level": "Write",
             "action": "ModifyTrafficMirrorSession",
-            "condition_keys": [],
-            "description": "Not Documented by AWS",
+            "condition_keys": [
+                "aws:ResourceTag/${TagKey}",
+                "ec2:Attribute",
+                "ec2:Attribute/${AttributeName}",
+                "ec2:Region",
+                "ec2:ResourceTag/${TagKey}"
+            ],
+            "description": "Grants permission to modify a traffic mirror session",
             "orphan": false,
-            "resources": []
+            "resources": [
+                "traffic-mirror-filter",
+                "traffic-mirror-session",
+                "traffic-mirror-target"
+            ]
         },
         "ModifyTransitGateway": {
-            "access_level": "Undocumented",
+            "access_level": "Write",
             "action": "ModifyTransitGateway",
-            "condition_keys": [],
-            "description": "Not Documented by AWS",
+            "condition_keys": [
+                "aws:ResourceTag/${TagKey}",
+                "ec2:Attribute",
+                "ec2:Attribute/${AttributeName}",
+                "ec2:Region",
+                "ec2:ResourceTag/${TagKey}"
+            ],
+            "description": "Grants permission to modify a transit gateway",
             "orphan": false,
-            "resources": []
+            "resources": [
+                "transit-gateway",
+                "transit-gateway-route-table"
+            ]
         },
         "ModifyTransitGatewayPrefixListReference": {
-            "access_level": "Undocumented",
+            "access_level": "Write",
             "action": "ModifyTransitGatewayPrefixListReference",
-            "condition_keys": [],
-            "description": "Not Documented by AWS",
+            "condition_keys": [
+                "aws:ResourceTag/${TagKey}",
+                "ec2:Attribute",
+                "ec2:Attribute/${AttributeName}",
+                "ec2:Region",
+                "ec2:ResourceTag/${TagKey}"
+            ],
+            "description": "Grants permission to modify a transit gateway prefix list reference",
             "orphan": false,
-            "resources": []
+            "resources": [
+                "prefix-list",
+                "transit-gateway-attachment",
+                "transit-gateway-route-table"
+            ]
         },
         "ModifyTransitGatewayVpcAttachment": {
-            "access_level": "Undocumented",
+            "access_level": "Write",
             "action": "ModifyTransitGatewayVpcAttachment",
-            "condition_keys": [],
-            "description": "Not Documented by AWS",
+            "condition_keys": [
+                "aws:ResourceTag/${TagKey}",
+                "ec2:Attribute",
+                "ec2:Attribute/${AttributeName}",
+                "ec2:Region",
+                "ec2:ResourceTag/${TagKey}",
+                "ec2:SubnetID"
+            ],
+            "description": "Grants permission to modify a VPC attachment on a transit gateway",
             "orphan": false,
-            "resources": []
+            "resources": [
+                "subnet",
+                "transit-gateway-attachment"
+            ]
         },
         "ModifyVerifiedAccessEndpoint": {
-            "access_level": "Undocumented",
+            "access_level": "Write",
             "action": "ModifyVerifiedAccessEndpoint",
-            "condition_keys": [],
-            "description": "Not Documented by AWS",
+            "condition_keys": [
+                "aws:ResourceTag/${TagKey}",
+                "ec2:AvailabilityZone",
+                "ec2:Region",
+                "ec2:ResourceTag/${TagKey}",
+                "ec2:SubnetID",
+                "ec2:Vpc"
+            ],
+            "description": "Grants permission to modify the configuration of a Verified Access endpoint",
             "orphan": false,
-            "resources": []
+            "resources": [
+                "subnet",
+                "verified-access-endpoint",
+                "verified-access-group"
+            ]
         },
         "ModifyVerifiedAccessEndpointPolicy": {
-            "access_level": "Undocumented",
+            "access_level": "Write",
             "action": "ModifyVerifiedAccessEndpointPolicy",
-            "condition_keys": [],
-            "description": "Not Documented by AWS",
+            "condition_keys": [
+                "aws:ResourceTag/${TagKey}",
+                "ec2:Region",
+                "ec2:ResourceTag/${TagKey}"
+            ],
+            "description": "Grants permission to modify the specified Verified Access endpoint policy",
             "orphan": false,
-            "resources": []
+            "resources": [
+                "verified-access-endpoint"
+            ]
         },
         "ModifyVerifiedAccessGroup": {
-            "access_level": "Undocumented",
+            "access_level": "Write",
             "action": "ModifyVerifiedAccessGroup",
-            "condition_keys": [],
-            "description": "Not Documented by AWS",
+            "condition_keys": [
+                "aws:ResourceTag/${TagKey}",
+                "ec2:Region",
+                "ec2:ResourceTag/${TagKey}"
+            ],
+            "description": "Grants permission to modify the specified Verified Access Group configuration",
             "orphan": false,
-            "resources": []
+            "resources": [
+                "verified-access-group",
+                "verified-access-instance"
+            ]
         },
         "ModifyVerifiedAccessGroupPolicy": {
-            "access_level": "Undocumented",
+            "access_level": "Write",
             "action": "ModifyVerifiedAccessGroupPolicy",
-            "condition_keys": [],
-            "description": "Not Documented by AWS",
+            "condition_keys": [
+                "aws:ResourceTag/${TagKey}",
+                "ec2:Region",
+                "ec2:ResourceTag/${TagKey}"
+            ],
+            "description": "Grants permission to modify the specified Verified Access group policy",
             "orphan": false,
-            "resources": []
+            "resources": [
+                "verified-access-group"
+            ]
         },
         "ModifyVerifiedAccessInstance": {
-            "access_level": "Undocumented",
+            "access_level": "Write",
             "action": "ModifyVerifiedAccessInstance",
-            "condition_keys": [],
-            "description": "Not Documented by AWS",
+            "condition_keys": [
+                "aws:ResourceTag/${TagKey}",
+                "ec2:Region",
+                "ec2:ResourceTag/${TagKey}"
+            ],
+            "description": "Grants permission to modify the configuration of the specified Verified Access instance",
             "orphan": false,
-            "resources": []
+            "resources": [
+                "verified-access-instance"
+            ]
         },
         "ModifyVerifiedAccessInstanceLoggingConfiguration": {
-            "access_level": "Undocumented",
+            "access_level": "Write",
             "action": "ModifyVerifiedAccessInstanceLoggingConfiguration",
-            "condition_keys": [],
-            "description": "Not Documented by AWS",
+            "condition_keys": [
+                "aws:ResourceTag/${TagKey}",
+                "ec2:Region",
+                "ec2:ResourceTag/${TagKey}"
+            ],
+            "description": "Grants permission to modify the logging configuration for the specified Verified Access instance",
             "orphan": false,
-            "resources": []
+            "resources": [
+                "verified-access-instance"
+            ]
         },
         "ModifyVerifiedAccessTrustProvider": {
-            "access_level": "Undocumented",
+            "access_level": "Write",
             "action": "ModifyVerifiedAccessTrustProvider",
-            "condition_keys": [],
-            "description": "Not Documented by AWS",
+            "condition_keys": [
+                "aws:ResourceTag/${TagKey}",
+                "ec2:Region",
+                "ec2:ResourceTag/${TagKey}"
+            ],
+            "description": "Grants permission to modify the configuration of the specified Verified Access trust provider",
             "orphan": false,
-            "resources": []
+            "resources": [
+                "verified-access-trust-provider"
+            ]
         },
         "ModifyVolume": {
-            "access_level": "Undocumented",
+            "access_level": "Write",
             "action": "ModifyVolume",
-            "condition_keys": [],
-            "description": "Not Documented by AWS",
+            "condition_keys": [
+                "aws:ResourceTag/${TagKey}",
+                "ec2:Attribute",
+                "ec2:Attribute/${AttributeName}",
+                "ec2:AvailabilityZone",
+                "ec2:Encrypted",
+                "ec2:ParentSnapshot",
+                "ec2:Region",
+                "ec2:ResourceTag/${TagKey}",
+                "ec2:VolumeID",
+                "ec2:VolumeIops",
+                "ec2:VolumeSize",
+                "ec2:VolumeThroughput",
+                "ec2:VolumeType"
+            ],
+            "description": "Grants permission to modify the parameters of an EBS volume",
             "orphan": false,
-            "resources": []
+            "resources": [
+                "volume"
+            ]
         },
         "ModifyVolumeAttribute": {
-            "access_level": "Undocumented",
+            "access_level": "Write",
             "action": "ModifyVolumeAttribute",
-            "condition_keys": [],
-            "description": "Not Documented by AWS",
+            "condition_keys": [
+                "aws:ResourceTag/${TagKey}",
+                "ec2:Attribute",
+                "ec2:Attribute/${AttributeName}",
+                "ec2:AvailabilityZone",
+                "ec2:Encrypted",
+                "ec2:ParentSnapshot",
+                "ec2:Region",
+                "ec2:ResourceTag/${TagKey}",
+                "ec2:VolumeID",
+                "ec2:VolumeIops",
+                "ec2:VolumeSize",
+                "ec2:VolumeThroughput",
+                "ec2:VolumeType"
+            ],
+            "description": "Grants permission to modify an attribute of a volume",
             "orphan": false,
-            "resources": []
+            "resources": [
+                "volume"
+            ]
         },
         "ModifyVpcAttribute": {
-            "access_level": "Undocumented",
+            "access_level": "Write",
             "action": "ModifyVpcAttribute",
-            "condition_keys": [],
-            "description": "Not Documented by AWS",
+            "condition_keys": [
+                "aws:ResourceTag/${TagKey}",
+                "ec2:Attribute",
+                "ec2:Attribute/${AttributeName}",
+                "ec2:Region",
+                "ec2:ResourceTag/${TagKey}",
+                "ec2:Tenancy",
+                "ec2:VpcID"
+            ],
+            "description": "Grants permission to modify an attribute of a VPC",
             "orphan": false,
-            "resources": []
+            "resources": [
+                "vpc"
+            ]
         },
         "ModifyVpcEndpoint": {
-            "access_level": "Undocumented",
+            "access_level": "Write",
             "action": "ModifyVpcEndpoint",
-            "condition_keys": [],
-            "description": "Not Documented by AWS",
+            "condition_keys": [
+                "aws:ResourceTag/${TagKey}",
+                "ec2:Attribute",
+                "ec2:Attribute/${AttributeName}",
+                "ec2:Region",
+                "ec2:ResourceTag/${TagKey}",
+                "ec2:RouteTableID",
+                "ec2:SecurityGroupID",
+                "ec2:SubnetID"
+            ],
+            "description": "Grants permission to modify an attribute of a VPC endpoint",
             "orphan": false,
-            "resources": []
+            "resources": [
+                "route-table",
+                "security-group",
+                "subnet",
+                "vpc-endpoint"
+            ]
         },
         "ModifyVpcEndpointConnectionNotification": {
-            "access_level": "Undocumented",
+            "access_level": "Write",
             "action": "ModifyVpcEndpointConnectionNotification",
-            "condition_keys": [],
-            "description": "Not Documented by AWS",
+            "condition_keys": [
+                "aws:ResourceTag/${TagKey}",
+                "ec2:Region",
+                "ec2:ResourceTag/${TagKey}"
+            ],
+            "description": "Grants permission to modify a connection notification for a VPC endpoint or VPC endpoint service",
             "orphan": false,
-            "resources": []
+            "resources": [
+                "vpc-endpoint",
+                "vpc-endpoint-service"
+            ]
         },
         "ModifyVpcEndpointServiceConfiguration": {
-            "access_level": "Undocumented",
+            "access_level": "Write",
             "action": "ModifyVpcEndpointServiceConfiguration",
-            "condition_keys": [],
-            "description": "Not Documented by AWS",
+            "condition_keys": [
+                "aws:ResourceTag/${TagKey}",
+                "ec2:Attribute",
+                "ec2:Attribute/${AttributeName}",
+                "ec2:Region",
+                "ec2:ResourceTag/${TagKey}",
+                "ec2:VpceServicePrivateDnsName"
+            ],
+            "description": "Grants permission to modify the attributes of a VPC endpoint service configuration",
             "orphan": false,
-            "resources": []
+            "resources": [
+                "vpc-endpoint-service"
+            ]
         },
         "ModifyVpcEndpointServicePayerResponsibility": {
-            "access_level": "Undocumented",
+            "access_level": "Write",
             "action": "ModifyVpcEndpointServicePayerResponsibility",
-            "condition_keys": [],
-            "description": "Not Documented by AWS",
+            "condition_keys": [
+                "aws:ResourceTag/${TagKey}",
+                "ec2:Attribute",
+                "ec2:Attribute/${AttributeName}",
+                "ec2:Region",
+                "ec2:ResourceTag/${TagKey}"
+            ],
+            "description": "Grants permission to modify the payer responsibility for a VPC endpoint service",
             "orphan": false,
-            "resources": []
+            "resources": [
+                "vpc-endpoint-service"
+            ]
         },
         "ModifyVpcEndpointServicePermissions": {
-            "access_level": "Undocumented",
+            "access_level": "Permissions management",
             "action": "ModifyVpcEndpointServicePermissions",
-            "condition_keys": [],
-            "description": "Not Documented by AWS",
+            "condition_keys": [
+                "aws:ResourceTag/${TagKey}",
+                "ec2:Attribute",
+                "ec2:Attribute/${AttributeName}",
+                "ec2:Region",
+                "ec2:ResourceTag/${TagKey}"
+            ],
+            "description": "Grants permission to modify the permissions for a VPC endpoint service",
             "orphan": false,
-            "resources": []
+            "resources": [
+                "vpc-endpoint-service"
+            ]
         },
         "ModifyVpcPeeringConnectionOptions": {
-            "access_level": "Undocumented",
+            "access_level": "Write",
             "action": "ModifyVpcPeeringConnectionOptions",
-            "condition_keys": [],
-            "description": "Not Documented by AWS",
+            "condition_keys": [
+                "aws:ResourceTag/${TagKey}",
+                "ec2:AccepterVpc",
+                "ec2:Attribute",
+                "ec2:Attribute/${AttributeName}",
+                "ec2:Region",
+                "ec2:RequesterVpc",
+                "ec2:ResourceTag/${TagKey}",
+                "ec2:VpcPeeringConnectionID"
+            ],
+            "description": "Grants permission to modify the VPC peering connection options on one side of a VPC peering connection",
             "orphan": false,
-            "resources": []
+            "resources": [
+                "vpc-peering-connection"
+            ]
         },
         "ModifyVpcTenancy": {
-            "access_level": "Undocumented",
+            "access_level": "Write",
             "action": "ModifyVpcTenancy",
-            "condition_keys": [],
-            "description": "Not Documented by AWS",
+            "condition_keys": [
+                "aws:ResourceTag/${TagKey}",
+                "ec2:Attribute",
+                "ec2:Attribute/${AttributeName}",
+                "ec2:Region",
+                "ec2:ResourceTag/${TagKey}",
+                "ec2:Tenancy",
+                "ec2:VpcID"
+            ],
+            "description": "Grants permission to modify the instance tenancy attribute of a VPC",
             "orphan": false,
-            "resources": []
+            "resources": [
+                "vpc"
+            ]
         },
         "ModifyVpnConnection": {
-            "access_level": "Undocumented",
+            "access_level": "Write",
             "action": "ModifyVpnConnection",
-            "condition_keys": [],
-            "description": "Not Documented by AWS",
+            "condition_keys": [
+                "aws:ResourceTag/${TagKey}",
+                "ec2:Attribute",
+                "ec2:Attribute/${AttributeName}",
+                "ec2:AuthenticationType",
+                "ec2:DPDTimeoutSeconds",
+                "ec2:GatewayType",
+                "ec2:IKEVersions",
+                "ec2:InsideTunnelCidr",
+                "ec2:InsideTunnelIpv6Cidr",
+                "ec2:Phase1DHGroup",
+                "ec2:Phase1EncryptionAlgorithms",
+                "ec2:Phase1IntegrityAlgorithms",
+                "ec2:Phase1LifetimeSeconds",
+                "ec2:Phase2DHGroup",
+                "ec2:Phase2EncryptionAlgorithms",
+                "ec2:Phase2IntegrityAlgorithms",
+                "ec2:Phase2LifetimeSeconds",
+                "ec2:PreSharedKeys",
+                "ec2:Region",
+                "ec2:RekeyFuzzPercentage",
+                "ec2:RekeyMarginTimeSeconds",
+                "ec2:ReplayWindowSizePackets",
+                "ec2:ResourceTag/${TagKey}",
+                "ec2:RoutingType"
+            ],
+            "description": "Grants permission to modify the target gateway of a Site-to-Site VPN connection",
             "orphan": false,
-            "resources": []
+            "resources": [
+                "vpn-connection"
+            ]
         },
         "ModifyVpnConnectionOptions": {
-            "access_level": "Undocumented",
+            "access_level": "Write",
             "action": "ModifyVpnConnectionOptions",
-            "condition_keys": [],
-            "description": "Not Documented by AWS",
+            "condition_keys": [
+                "aws:ResourceTag/${TagKey}",
+                "ec2:Attribute",
+                "ec2:Attribute/${AttributeName}",
+                "ec2:Region",
+                "ec2:ResourceTag/${TagKey}"
+            ],
+            "description": "Grants permission to modify the connection options for your Site-to-Site VPN connection",
             "orphan": false,
-            "resources": []
+            "resources": [
+                "vpn-connection"
+            ]
         },
         "ModifyVpnTunnelCertificate": {
-            "access_level": "Undocumented",
+            "access_level": "Write",
             "action": "ModifyVpnTunnelCertificate",
-            "condition_keys": [],
-            "description": "Not Documented by AWS",
+            "condition_keys": [
+                "aws:ResourceTag/${TagKey}",
+                "ec2:Attribute",
+                "ec2:Attribute/${AttributeName}",
+                "ec2:Region",
+                "ec2:ResourceTag/${TagKey}"
+            ],
+            "description": "Grants permission to modify the certificate for a Site-to-Site VPN connection",
             "orphan": false,
-            "resources": []
+            "resources": [
+                "vpn-connection"
+            ]
         },
         "ModifyVpnTunnelOptions": {
-            "access_level": "Undocumented",
+            "access_level": "Write",
             "action": "ModifyVpnTunnelOptions",
-            "condition_keys": [],
-            "description": "Not Documented by AWS",
+            "condition_keys": [
+                "aws:ResourceTag/${TagKey}",
+                "ec2:Attribute",
+                "ec2:Attribute/${AttributeName}",
+                "ec2:AuthenticationType",
+                "ec2:DPDTimeoutSeconds",
+                "ec2:GatewayType",
+                "ec2:IKEVersions",
+                "ec2:InsideTunnelCidr",
+                "ec2:InsideTunnelIpv6Cidr",
+                "ec2:Phase1DHGroup",
+                "ec2:Phase1EncryptionAlgorithms",
+                "ec2:Phase1IntegrityAlgorithms",
+                "ec2:Phase1LifetimeSeconds",
+                "ec2:Phase2DHGroup",
+                "ec2:Phase2EncryptionAlgorithms",
+                "ec2:Phase2IntegrityAlgorithms",
+                "ec2:Phase2LifetimeSeconds",
+                "ec2:PreSharedKeys",
+                "ec2:Region",
+                "ec2:RekeyFuzzPercentage",
+                "ec2:RekeyMarginTimeSeconds",
+                "ec2:ReplayWindowSizePackets",
+                "ec2:ResourceTag/${TagKey}",
+                "ec2:RoutingType"
+            ],
+            "description": "Grants permission to modify the options for a Site-to-Site VPN connection",
             "orphan": false,
-            "resources": []
+            "resources": [
+                "vpn-connection"
+            ]
         },
         "MonitorInstances": {
-            "access_level": "Undocumented",
+            "access_level": "Write",
             "action": "MonitorInstances",
-            "condition_keys": [],
-            "description": "Not Documented by AWS",
+            "condition_keys": [
+                "aws:ResourceTag/${TagKey}",
+                "ec2:AvailabilityZone",
+                "ec2:EbsOptimized",
+                "ec2:InstanceAutoRecovery",
+                "ec2:InstanceID",
+                "ec2:InstanceMarketType",
+                "ec2:InstanceMetadataTags",
+                "ec2:InstanceProfile",
+                "ec2:InstanceType",
+                "ec2:MetadataHttpEndpoint",
+                "ec2:MetadataHttpPutResponseHopLimit",
+                "ec2:MetadataHttpTokens",
+                "ec2:PlacementGroup",
+                "ec2:ProductCode",
+                "ec2:Region",
+                "ec2:ResourceTag/${TagKey}",
+                "ec2:RootDeviceType",
+                "ec2:Tenancy"
+            ],
+            "description": "Grants permission to enable detailed monitoring for a running instance",
             "orphan": false,
-            "resources": []
+            "resources": [
+                "instance"
+            ]
         },
         "MoveAddressToVpc": {
-            "access_level": "Undocumented",
+            "access_level": "Write",
             "action": "MoveAddressToVpc",
-            "condition_keys": [],
-            "description": "Not Documented by AWS",
+            "condition_keys": [
+                "ec2:Region"
+            ],
+            "description": "Grants permission to move an Elastic IP address from the EC2-Classic platform to the EC2-VPC platform",
             "orphan": false,
             "resources": []
         },
         "MoveByoipCidrToIpam": {
-            "access_level": "Undocumented",
+            "access_level": "Write",
             "action": "MoveByoipCidrToIpam",
-            "condition_keys": [],
-            "description": "Not Documented by AWS",
+            "condition_keys": [
+                "aws:ResourceTag/${TagKey}",
+                "ec2:Region",
+                "ec2:ResourceTag/${TagKey}"
+            ],
+            "description": "Grants permission to move a BYOIP IPv4 CIDR to Amazon VPC IP Address Manager (IPAM) from a public IPv4 pool",
             "orphan": false,
-            "resources": []
+            "resources": [
+                "ipam-pool"
+            ]
         },
         "PauseVolumeIO": {
-            "access_level": "Undocumented",
+            "access_level": "Write",
             "action": "PauseVolumeIO",
-            "condition_keys": [],
-            "description": "Not Documented by AWS",
+            "condition_keys": [
+                "aws:ResourceTag/${TagKey}",
+                "ec2:AvailabilityZone",
+                "ec2:EbsOptimized",
+                "ec2:Encrypted",
+                "ec2:InstanceAutoRecovery",
+                "ec2:InstanceID",
+                "ec2:InstanceMarketType",
+                "ec2:InstanceMetadataTags",
+                "ec2:InstanceProfile",
+                "ec2:InstanceType",
+                "ec2:MetadataHttpEndpoint",
+                "ec2:MetadataHttpPutResponseHopLimit",
+                "ec2:MetadataHttpTokens",
+                "ec2:ParentSnapshot",
+                "ec2:Region",
+                "ec2:ResourceTag/${TagKey}",
+                "ec2:RootDeviceType",
+                "ec2:Tenancy",
+                "ec2:VolumeID",
+                "ec2:VolumeIops",
+                "ec2:VolumeSize",
+                "ec2:VolumeThroughput",
+                "ec2:VolumeType"
+            ],
+            "description": "Grants permission to temporarily pause I/O operations for a target Amazon EBS volume",
             "orphan": false,
-            "resources": []
+            "resources": [
+                "instance",
+                "volume"
+            ]
         },
         "ProvisionByoipCidr": {
-            "access_level": "Undocumented",
+            "access_level": "Write",
             "action": "ProvisionByoipCidr",
-            "condition_keys": [],
-            "description": "Not Documented by AWS",
+            "condition_keys": [
+                "ec2:Region"
+            ],
+            "description": "Grants permission to provision an address range for use in AWS through bring your own IP addresses (BYOIP), and to create a corresponding address pool",
             "orphan": false,
             "resources": []
         },
         "ProvisionIpamPoolCidr": {
-            "access_level": "Undocumented",
+            "access_level": "Write",
             "action": "ProvisionIpamPoolCidr",
-            "condition_keys": [],
-            "description": "Not Documented by AWS",
+            "condition_keys": [
+                "aws:ResourceTag/${TagKey}",
+                "ec2:Region",
+                "ec2:ResourceTag/${TagKey}"
+            ],
+            "description": "Grants permission to provision a CIDR to an Amazon VPC IP Address Manager (IPAM) pool",
             "orphan": false,
-            "resources": []
+            "resources": [
+                "ipam-pool"
+            ]
         },
         "ProvisionPublicIpv4PoolCidr": {
-            "access_level": "Undocumented",
+            "access_level": "Write",
             "action": "ProvisionPublicIpv4PoolCidr",
-            "condition_keys": [],
-            "description": "Not Documented by AWS",
+            "condition_keys": [
+                "aws:ResourceTag/${TagKey}",
+                "ec2:Region",
+                "ec2:ResourceTag/${TagKey}"
+            ],
+            "description": "Grants permission to provision a CIDR to a public IPv4 pool",
             "orphan": false,
-            "resources": []
+            "resources": [
+                "ipam-pool",
+                "ipv4pool-ec2"
+            ]
         },
         "PurchaseHostReservation": {
-            "access_level": "Undocumented",
+            "access_level": "Write",
             "action": "PurchaseHostReservation",
-            "condition_keys": [],
-            "description": "Not Documented by AWS",
+            "condition_keys": [
+                "aws:ResourceTag/${TagKey}",
+                "ec2:Region",
+                "ec2:ResourceTag/${TagKey}"
+            ],
+            "description": "Grants permission to purchase a reservation with configurations that match those of a Dedicated Host",
             "orphan": false,
-            "resources": []
+            "resources": [
+                "dedicated-host"
+            ]
         },
         "PurchaseReservedInstancesOffering": {
-            "access_level": "Undocumented",
+            "access_level": "Write",
             "action": "PurchaseReservedInstancesOffering",
-            "condition_keys": [],
-            "description": "Not Documented by AWS",
+            "condition_keys": [
+                "ec2:Region"
+            ],
+            "description": "Grants permission to purchase a Reserved Instance offering",
             "orphan": false,
             "resources": []
         },
         "PurchaseScheduledInstances": {
-            "access_level": "Undocumented",
+            "access_level": "Write",
             "action": "PurchaseScheduledInstances",
-            "condition_keys": [],
-            "description": "Not Documented by AWS",
+            "condition_keys": [
+                "ec2:Region"
+            ],
+            "description": "Grants permission to purchase one or more Scheduled Instances with a specified schedule",
             "orphan": false,
             "resources": []
         },
         "PutResourcePolicy": {
-            "access_level": "Undocumented",
+            "access_level": "Write",
             "action": "PutResourcePolicy",
-            "condition_keys": [],
-            "description": "Not Documented by AWS",
+            "condition_keys": [
+                "aws:ResourceTag/${TagKey}",
+                "ec2:PlacementGroupName",
+                "ec2:PlacementGroupStrategy",
+                "ec2:Region",
+                "ec2:ResourceTag/${TagKey}"
+            ],
+            "description": "Grants permission to attach an IAM policy that enables cross-account sharing to a resource",
             "orphan": false,
-            "resources": []
+            "resources": [
+                "ipam-pool",
+                "placement-group",
+                "verified-access-group"
+            ]
         },
         "RebootInstances": {
-            "access_level": "Undocumented",
+            "access_level": "Write",
             "action": "RebootInstances",
-            "condition_keys": [],
-            "description": "Not Documented by AWS",
+            "condition_keys": [
+                "aws:ResourceTag/${TagKey}",
+                "ec2:AvailabilityZone",
+                "ec2:EbsOptimized",
+                "ec2:InstanceAutoRecovery",
+                "ec2:InstanceID",
+                "ec2:InstanceMarketType",
+                "ec2:InstanceMetadataTags",
+                "ec2:InstanceProfile",
+                "ec2:InstanceType",
+                "ec2:MetadataHttpEndpoint",
+                "ec2:MetadataHttpPutResponseHopLimit",
+                "ec2:MetadataHttpTokens",
+                "ec2:PlacementGroup",
+                "ec2:ProductCode",
+                "ec2:Region",
+                "ec2:ResourceTag/${TagKey}",
+                "ec2:RootDeviceType",
+                "ec2:Tenancy"
+            ],
+            "description": "Grants permission to request a reboot of one or more instances",
             "orphan": false,
-            "resources": []
+            "resources": [
+                "instance"
+            ]
         },
         "RegisterImage": {
-            "access_level": "Undocumented",
+            "access_level": "Write",
             "action": "RegisterImage",
-            "condition_keys": [],
-            "description": "Not Documented by AWS",
+            "condition_keys": [
+                "aws:ResourceTag/${TagKey}",
+                "ec2:ImageID",
+                "ec2:OutpostArn",
+                "ec2:Owner",
+                "ec2:ParentVolume",
+                "ec2:Region",
+                "ec2:ResourceTag/${TagKey}",
+                "ec2:SnapshotID",
+                "ec2:SnapshotTime",
+                "ec2:SourceOutpostArn",
+                "ec2:VolumeSize"
+            ],
+            "description": "Grants permission to register an Amazon Machine Image (AMI)",
             "orphan": false,
-            "resources": []
+            "resources": [
+                "image",
+                "snapshot"
+            ]
         },
         "RegisterInstanceEventNotificationAttributes": {
-            "access_level": "Undocumented",
+            "access_level": "Write",
             "action": "RegisterInstanceEventNotificationAttributes",
-            "condition_keys": [],
-            "description": "Not Documented by AWS",
+            "condition_keys": [
+                "ec2:Region"
+            ],
+            "description": "Grants permission to add tags to the set of tags to include in notifications about scheduled events for your instances",
             "orphan": false,
             "resources": []
         },
         "RegisterTransitGatewayMulticastGroupMembers": {
-            "access_level": "Undocumented",
+            "access_level": "Write",
             "action": "RegisterTransitGatewayMulticastGroupMembers",
-            "condition_keys": [],
-            "description": "Not Documented by AWS",
+            "condition_keys": [
+                "aws:ResourceTag/${TagKey}",
+                "ec2:AvailabilityZone",
+                "ec2:NetworkInterfaceID",
+                "ec2:Region",
+                "ec2:ResourceTag/${TagKey}",
+                "ec2:Subnet",
+                "ec2:Vpc"
+            ],
+            "description": "Grants permission to register one or more network interfaces as a member of a group IP address in a transit gateway multicast domain",
             "orphan": false,
-            "resources": []
+            "resources": [
+                "network-interface",
+                "transit-gateway-multicast-domain"
+            ]
         },
         "RegisterTransitGatewayMulticastGroupSources": {
-            "access_level": "Undocumented",
+            "access_level": "Write",
             "action": "RegisterTransitGatewayMulticastGroupSources",
-            "condition_keys": [],
-            "description": "Not Documented by AWS",
+            "condition_keys": [
+                "aws:ResourceTag/${TagKey}",
+                "ec2:AvailabilityZone",
+                "ec2:NetworkInterfaceID",
+                "ec2:Region",
+                "ec2:ResourceTag/${TagKey}",
+                "ec2:Subnet",
+                "ec2:Vpc"
+            ],
+            "description": "Grants permission to register one or more network interfaces as a source of a group IP address in a transit gateway multicast domain",
             "orphan": false,
-            "resources": []
+            "resources": [
+                "network-interface",
+                "transit-gateway-multicast-domain"
+            ]
         },
         "RejectTransitGatewayMulticastDomainAssociations": {
-            "access_level": "Undocumented",
+            "access_level": "Write",
             "action": "RejectTransitGatewayMulticastDomainAssociations",
-            "condition_keys": [],
-            "description": "Not Documented by AWS",
+            "condition_keys": [
+                "aws:ResourceTag/${TagKey}",
+                "ec2:Region",
+                "ec2:ResourceTag/${TagKey}"
+            ],
+            "description": "Grants permission to reject requests to associate cross-account subnets with a transit gateway multicast domain",
             "orphan": false,
-            "resources": []
+            "resources": [
+                "transit-gateway-attachment",
+                "transit-gateway-multicast-domain"
+            ]
         },
         "RejectTransitGatewayPeeringAttachment": {
-            "access_level": "Undocumented",
+            "access_level": "Write",
             "action": "RejectTransitGatewayPeeringAttachment",
-            "condition_keys": [],
-            "description": "Not Documented by AWS",
+            "condition_keys": [
+                "aws:ResourceTag/${TagKey}",
+                "ec2:Region",
+                "ec2:ResourceTag/${TagKey}"
+            ],
+            "description": "Grants permission to reject a transit gateway peering attachment request",
             "orphan": false,
-            "resources": []
+            "resources": [
+                "transit-gateway-attachment"
+            ]
         },
         "RejectTransitGatewayVpcAttachment": {
-            "access_level": "Undocumented",
+            "access_level": "Write",
             "action": "RejectTransitGatewayVpcAttachment",
-            "condition_keys": [],
-            "description": "Not Documented by AWS",
+            "condition_keys": [
+                "aws:ResourceTag/${TagKey}",
+                "ec2:Region",
+                "ec2:ResourceTag/${TagKey}"
+            ],
+            "description": "Grants permission to reject a request to attach a VPC to a transit gateway",
             "orphan": false,
-            "resources": []
+            "resources": [
+                "transit-gateway-attachment"
+            ]
         },
         "RejectVpcEndpointConnections": {
-            "access_level": "Undocumented",
+            "access_level": "Write",
             "action": "RejectVpcEndpointConnections",
-            "condition_keys": [],
-            "description": "Not Documented by AWS",
+            "condition_keys": [
+                "aws:ResourceTag/${TagKey}",
+                "ec2:Region",
+                "ec2:ResourceTag/${TagKey}"
+            ],
+            "description": "Grants permission to reject one or more VPC endpoint connection requests to a VPC endpoint service",
             "orphan": false,
-            "resources": []
+            "resources": [
+                "vpc-endpoint-service"
+            ]
         },
         "RejectVpcPeeringConnection": {
-            "access_level": "Undocumented",
+            "access_level": "Write",
             "action": "RejectVpcPeeringConnection",
-            "condition_keys": [],
-            "description": "Not Documented by AWS",
+            "condition_keys": [
+                "aws:ResourceTag/${TagKey}",
+                "ec2:AccepterVpc",
+                "ec2:Region",
+                "ec2:RequesterVpc",
+                "ec2:ResourceTag/${TagKey}",
+                "ec2:VpcPeeringConnectionID"
+            ],
+            "description": "Grants permission to reject a VPC peering connection request",
             "orphan": false,
-            "resources": []
+            "resources": [
+                "vpc-peering-connection"
+            ]
         },
         "ReleaseAddress": {
-            "access_level": "Undocumented",
+            "access_level": "Write",
             "action": "ReleaseAddress",
-            "condition_keys": [],
-            "description": "Not Documented by AWS",
+            "condition_keys": [
+                "aws:ResourceTag/${TagKey}",
+                "ec2:AllocationId",
+                "ec2:Domain",
+                "ec2:PublicIpAddress",
+                "ec2:Region",
+                "ec2:ResourceTag/${TagKey}"
+            ],
+            "description": "Grants permission to release an Elastic IP address",
             "orphan": false,
-            "resources": []
+            "resources": [
+                "elastic-ip"
+            ]
         },
         "ReleaseHosts": {
-            "access_level": "Undocumented",
+            "access_level": "Write",
             "action": "ReleaseHosts",
-            "condition_keys": [],
-            "description": "Not Documented by AWS",
+            "condition_keys": [
+                "aws:ResourceTag/${TagKey}",
+                "ec2:Region",
+                "ec2:ResourceTag/${TagKey}"
+            ],
+            "description": "Grants permission to release one or more On-Demand Dedicated Hosts",
             "orphan": false,
-            "resources": []
+            "resources": [
+                "dedicated-host"
+            ]
         },
         "ReleaseIpamPoolAllocation": {
-            "access_level": "Undocumented",
+            "access_level": "Write",
             "action": "ReleaseIpamPoolAllocation",
-            "condition_keys": [],
-            "description": "Not Documented by AWS",
+            "condition_keys": [
+                "aws:ResourceTag/${TagKey}",
+                "ec2:Region",
+                "ec2:ResourceTag/${TagKey}"
+            ],
+            "description": "Grants permission to release an allocation within an Amazon VPC IP Address Manager (IPAM) pool",
             "orphan": false,
-            "resources": []
+            "resources": [
+                "ipam-pool"
+            ]
         },
         "ReplaceIamInstanceProfileAssociation": {
-            "access_level": "Undocumented",
+            "access_level": "Write",
             "action": "ReplaceIamInstanceProfileAssociation",
-            "condition_keys": [],
-            "description": "Not Documented by AWS",
+            "condition_keys": [
+                "aws:ResourceTag/${TagKey}",
+                "ec2:AvailabilityZone",
+                "ec2:EbsOptimized",
+                "ec2:InstanceAutoRecovery",
+                "ec2:InstanceID",
+                "ec2:InstanceMarketType",
+                "ec2:InstanceMetadataTags",
+                "ec2:InstanceProfile",
+                "ec2:InstanceType",
+                "ec2:MetadataHttpEndpoint",
+                "ec2:MetadataHttpPutResponseHopLimit",
+                "ec2:MetadataHttpTokens",
+                "ec2:NewInstanceProfile",
+                "ec2:PlacementGroup",
+                "ec2:ProductCode",
+                "ec2:Region",
+                "ec2:ResourceTag/${TagKey}",
+                "ec2:RootDeviceType",
+                "ec2:Tenancy"
+            ],
+            "description": "Grants permission to replace an IAM instance profile for an instance",
             "orphan": false,
-            "resources": []
+            "resources": [
+                "instance"
+            ]
         },
         "ReplaceNetworkAclAssociation": {
-            "access_level": "Undocumented",
+            "access_level": "Write",
             "action": "ReplaceNetworkAclAssociation",
-            "condition_keys": [],
-            "description": "Not Documented by AWS",
+            "condition_keys": [
+                "aws:ResourceTag/${TagKey}",
+                "ec2:AvailabilityZone",
+                "ec2:NetworkAclID",
+                "ec2:Region",
+                "ec2:ResourceTag/${TagKey}",
+                "ec2:SubnetID",
+                "ec2:Vpc"
+            ],
+            "description": "Grants permission to change which network ACL a subnet is associated with",
             "orphan": false,
-            "resources": []
+            "resources": [
+                "network-acl",
+                "subnet"
+            ]
         },
         "ReplaceNetworkAclEntry": {
-            "access_level": "Undocumented",
+            "access_level": "Write",
             "action": "ReplaceNetworkAclEntry",
-            "condition_keys": [],
-            "description": "Not Documented by AWS",
+            "condition_keys": [
+                "aws:ResourceTag/${TagKey}",
+                "ec2:NetworkAclID",
+                "ec2:Region",
+                "ec2:ResourceTag/${TagKey}",
+                "ec2:Vpc"
+            ],
+            "description": "Grants permission to replace an entry (rule) in a network ACL",
             "orphan": false,
-            "resources": []
+            "resources": [
+                "network-acl"
+            ]
         },
         "ReplaceRoute": {
-            "access_level": "Undocumented",
+            "access_level": "Write",
             "action": "ReplaceRoute",
-            "condition_keys": [],
-            "description": "Not Documented by AWS",
+            "condition_keys": [
+                "aws:ResourceTag/${TagKey}",
+                "ec2:Region",
+                "ec2:ResourceTag/${TagKey}",
+                "ec2:RouteTableID",
+                "ec2:Vpc"
+            ],
+            "description": "Grants permission to replace a route within a route table in a VPC",
             "orphan": false,
-            "resources": []
+            "resources": [
+                "route-table"
+            ]
         },
         "ReplaceRouteTableAssociation": {
-            "access_level": "Undocumented",
+            "access_level": "Write",
             "action": "ReplaceRouteTableAssociation",
-            "condition_keys": [],
-            "description": "Not Documented by AWS",
-            "orphan": false,
-            "resources": []
+            "condition_keys": [
+                "aws:ResourceTag/${TagKey}",
+                "ec2:AvailabilityZone",
+                "ec2:InternetGatewayID",
+                "ec2:Region",
+                "ec2:ResourceTag/${TagKey}",
+                "ec2:RouteTableID",
+                "ec2:SubnetID",
+                "ec2:Vpc"
+            ],
+            "description": "Grants permission to change the route table that is associated with a subnet",
+            "orphan": false,
+            "resources": [
+                "internet-gateway",
+                "ipv4pool-ec2",
+                "ipv6pool-ec2",
+                "route-table",
+                "subnet"
+            ]
         },
         "ReplaceTransitGatewayRoute": {
-            "access_level": "Undocumented",
+            "access_level": "Write",
             "action": "ReplaceTransitGatewayRoute",
-            "condition_keys": [],
-            "description": "Not Documented by AWS",
+            "condition_keys": [
+                "aws:ResourceTag/${TagKey}",
+                "ec2:Region",
+                "ec2:ResourceTag/${TagKey}"
+            ],
+            "description": "Grants permission to replace a route in a transit gateway route table",
             "orphan": false,
-            "resources": []
+            "resources": [
+                "transit-gateway-attachment",
+                "transit-gateway-route-table"
+            ]
         },
         "ReplaceVpnTunnel": {
-            "access_level": "Undocumented",
+            "access_level": "Write",
             "action": "ReplaceVpnTunnel",
-            "condition_keys": [],
-            "description": "Not Documented by AWS",
+            "condition_keys": [
+                "aws:ResourceTag/${TagKey}",
+                "ec2:Region",
+                "ec2:ResourceTag/${TagKey}"
+            ],
+            "description": "Grants permission to replace a VPN tunnel",
             "orphan": false,
-            "resources": []
+            "resources": [
+                "vpn-connection"
+            ]
         },
         "ReportInstanceStatus": {
-            "access_level": "Undocumented",
+            "access_level": "Write",
             "action": "ReportInstanceStatus",
-            "condition_keys": [],
-            "description": "Not Documented by AWS",
+            "condition_keys": [
+                "ec2:Region"
+            ],
+            "description": "Grants permission to submit feedback about the status of an instance",
             "orphan": false,
             "resources": []
         },
         "RequestSpotFleet": {
-            "access_level": "Undocumented",
+            "access_level": "Write",
             "action": "RequestSpotFleet",
-            "condition_keys": [],
-            "description": "Not Documented by AWS",
+            "condition_keys": [
+                "aws:ResourceTag/${TagKey}",
+                "ec2:AvailabilityZone",
+                "ec2:ImageID",
+                "ec2:ImageType",
+                "ec2:KeyPairName",
+                "ec2:KeyPairType",
+                "ec2:OutpostArn",
+                "ec2:Owner",
+                "ec2:ParentVolume",
+                "ec2:PlacementGroupName",
+                "ec2:PlacementGroupStrategy",
+                "ec2:Public",
+                "ec2:Region",
+                "ec2:ResourceTag/${TagKey}",
+                "ec2:RootDeviceType",
+                "ec2:SecurityGroupID",
+                "ec2:SnapshotID",
+                "ec2:SnapshotTime",
+                "ec2:SourceOutpostArn",
+                "ec2:SubnetID",
+                "ec2:VolumeSize",
+                "ec2:Vpc"
+            ],
+            "description": "Grants permission to create a Spot Fleet request",
             "orphan": false,
-            "resources": []
+            "resources": [
+                "image",
+                "key-pair",
+                "launch-template",
+                "placement-group",
+                "security-group",
+                "snapshot",
+                "spot-fleet-request",
+                "subnet"
+            ]
         },
         "RequestSpotInstances": {
-            "access_level": "Undocumented",
+            "access_level": "Write",
             "action": "RequestSpotInstances",
-            "condition_keys": [],
-            "description": "Not Documented by AWS",
+            "condition_keys": [
+                "aws:RequestTag/${TagKey}",
+                "aws:ResourceTag/${TagKey}",
+                "aws:TagKeys",
+                "ec2:AuthorizedUser",
+                "ec2:AvailabilityZone",
+                "ec2:ImageID",
+                "ec2:ImageType",
+                "ec2:KeyPairName",
+                "ec2:KeyPairType",
+                "ec2:NetworkInterfaceID",
+                "ec2:OutpostArn",
+                "ec2:Owner",
+                "ec2:ParentVolume",
+                "ec2:Permission",
+                "ec2:PlacementGroupName",
+                "ec2:PlacementGroupStrategy",
+                "ec2:Public",
+                "ec2:Region",
+                "ec2:ResourceTag/${TagKey}",
+                "ec2:RootDeviceType",
+                "ec2:SecurityGroupID",
+                "ec2:SnapshotID",
+                "ec2:SnapshotTime",
+                "ec2:SourceOutpostArn",
+                "ec2:Subnet",
+                "ec2:SubnetID",
+                "ec2:VolumeSize",
+                "ec2:Vpc"
+            ],
+            "description": "Grants permission to create a Spot Instance request",
             "orphan": false,
-            "resources": []
+            "resources": [
+                "image",
+                "key-pair",
+                "network-interface",
+                "placement-group",
+                "security-group",
+                "snapshot",
+                "spot-instances-request",
+                "subnet"
+            ]
         },
         "ResetAddressAttribute": {
-            "access_level": "Undocumented",
+            "access_level": "Write",
             "action": "ResetAddressAttribute",
-            "condition_keys": [],
-            "description": "Not Documented by AWS",
+            "condition_keys": [
+                "aws:ResourceTag/${TagKey}",
+                "ec2:AllocationId",
+                "ec2:Attribute",
+                "ec2:Attribute/${AttributeName}",
+                "ec2:Domain",
+                "ec2:PublicIpAddress",
+                "ec2:Region",
+                "ec2:ResourceTag/${TagKey}"
+            ],
+            "description": "Grants permission to reset the attribute of the specified IP address",
             "orphan": false,
-            "resources": []
+            "resources": [
+                "elastic-ip"
+            ]
         },
         "ResetEbsDefaultKmsKeyId": {
-            "access_level": "Undocumented",
+            "access_level": "Write",
             "action": "ResetEbsDefaultKmsKeyId",
-            "condition_keys": [],
-            "description": "Not Documented by AWS",
+            "condition_keys": [
+                "ec2:Region"
+            ],
+            "description": "Grants permission to reset the default customer master key (CMK) for EBS encryption for your account to use the AWS-managed CMK for EBS",
             "orphan": false,
             "resources": []
         },
         "ResetFpgaImageAttribute": {
-            "access_level": "Undocumented",
+            "access_level": "Write",
             "action": "ResetFpgaImageAttribute",
-            "condition_keys": [],
-            "description": "Not Documented by AWS",
+            "condition_keys": [
+                "aws:ResourceTag/${TagKey}",
+                "ec2:Attribute",
+                "ec2:Attribute/${AttributeName}",
+                "ec2:Owner",
+                "ec2:Public",
+                "ec2:Region",
+                "ec2:ResourceTag/${TagKey}"
+            ],
+            "description": "Grants permission to reset an attribute of an Amazon FPGA Image (AFI) to its default value",
             "orphan": false,
-            "resources": []
+            "resources": [
+                "fpga-image"
+            ]
         },
         "ResetImageAttribute": {
-            "access_level": "Undocumented",
+            "access_level": "Write",
             "action": "ResetImageAttribute",
-            "condition_keys": [],
-            "description": "Not Documented by AWS",
+            "condition_keys": [
+                "aws:ResourceTag/${TagKey}",
+                "ec2:Attribute",
+                "ec2:Attribute/${AttributeName}",
+                "ec2:ImageID",
+                "ec2:ImageType",
+                "ec2:Owner",
+                "ec2:Public",
+                "ec2:Region",
+                "ec2:ResourceTag/${TagKey}",
+                "ec2:RootDeviceType"
+            ],
+            "description": "Grants permission to reset an attribute of an Amazon Machine Image (AMI) to its default value",
             "orphan": false,
-            "resources": []
+            "resources": [
+                "image"
+            ]
         },
         "ResetInstanceAttribute": {
-            "access_level": "Undocumented",
+            "access_level": "Write",
             "action": "ResetInstanceAttribute",
-            "condition_keys": [],
-            "description": "Not Documented by AWS",
+            "condition_keys": [
+                "aws:ResourceTag/${TagKey}",
+                "ec2:AvailabilityZone",
+                "ec2:EbsOptimized",
+                "ec2:InstanceID",
+                "ec2:InstanceMarketType",
+                "ec2:InstanceProfile",
+                "ec2:InstanceType",
+                "ec2:MetadataHttpEndpoint",
+                "ec2:MetadataHttpPutResponseHopLimit",
+                "ec2:MetadataHttpTokens",
+                "ec2:ProductCode",
+                "ec2:Region",
+                "ec2:ResourceTag/${TagKey}",
+                "ec2:RootDeviceType",
+                "ec2:Tenancy"
+            ],
+            "description": "Grants permission to reset an attribute of an instance to its default value",
             "orphan": false,
-            "resources": []
+            "resources": [
+                "instance"
+            ]
         },
         "ResetNetworkInterfaceAttribute": {
-            "access_level": "Undocumented",
+            "access_level": "Write",
             "action": "ResetNetworkInterfaceAttribute",
-            "condition_keys": [],
-            "description": "Not Documented by AWS",
+            "condition_keys": [
+                "aws:ResourceTag/${TagKey}",
+                "ec2:AvailabilityZone",
+                "ec2:NetworkInterfaceID",
+                "ec2:Region",
+                "ec2:ResourceTag/${TagKey}",
+                "ec2:Subnet",
+                "ec2:Vpc"
+            ],
+            "description": "Grants permission to reset an attribute of a network interface",
             "orphan": false,
-            "resources": []
+            "resources": [
+                "network-interface"
+            ]
         },
         "ResetSnapshotAttribute": {
-            "access_level": "Undocumented",
+            "access_level": "Permissions management",
             "action": "ResetSnapshotAttribute",
-            "condition_keys": [],
-            "description": "Not Documented by AWS",
+            "condition_keys": [
+                "aws:ResourceTag/${TagKey}",
+                "ec2:Attribute",
+                "ec2:Attribute/${AttributeName}",
+                "ec2:Owner",
+                "ec2:ParentVolume",
+                "ec2:Region",
+                "ec2:ResourceTag/${TagKey}",
+                "ec2:SnapshotID",
+                "ec2:SnapshotTime",
+                "ec2:VolumeSize"
+            ],
+            "description": "Grants permission to reset permission settings for a snapshot",
             "orphan": false,
-            "resources": []
+            "resources": [
+                "snapshot"
+            ]
         },
         "RestoreAddressToClassic": {
-            "access_level": "Undocumented",
+            "access_level": "Write",
             "action": "RestoreAddressToClassic",
-            "condition_keys": [],
-            "description": "Not Documented by AWS",
+            "condition_keys": [
+                "ec2:Region"
+            ],
+            "description": "Grants permission to restore an Elastic IP address that was previously moved to the EC2-VPC platform back to the EC2-Classic platform",
             "orphan": false,
             "resources": []
         },
         "RestoreImageFromRecycleBin": {
-            "access_level": "Undocumented",
+            "access_level": "Write",
             "action": "RestoreImageFromRecycleBin",
-            "condition_keys": [],
-            "description": "Not Documented by AWS",
+            "condition_keys": [
+                "aws:ResourceTag/${TagKey}",
+                "ec2:ImageID",
+                "ec2:ImageType",
+                "ec2:Owner",
+                "ec2:Public",
+                "ec2:Region",
+                "ec2:ResourceTag/${TagKey}",
+                "ec2:RootDeviceType"
+            ],
+            "description": "Grants permission to restore an Amazon Machine Image (AMI) from the Recycle Bin",
             "orphan": false,
-            "resources": []
+            "resources": [
+                "image"
+            ]
         },
         "RestoreManagedPrefixListVersion": {
-            "access_level": "Undocumented",
+            "access_level": "Write",
             "action": "RestoreManagedPrefixListVersion",
-            "condition_keys": [],
-            "description": "Not Documented by AWS",
+            "condition_keys": [
+                "aws:ResourceTag/${TagKey}",
+                "ec2:Region",
+                "ec2:ResourceTag/${TagKey}"
+            ],
+            "description": "Grants permission to restore the entries from a previous version of a managed prefix list to a new version of the prefix list",
             "orphan": false,
-            "resources": []
+            "resources": [
+                "prefix-list"
+            ]
         },
         "RestoreSnapshotFromRecycleBin": {
-            "access_level": "Undocumented",
+            "access_level": "Write",
             "action": "RestoreSnapshotFromRecycleBin",
-            "condition_keys": [],
-            "description": "Not Documented by AWS",
+            "condition_keys": [
+                "aws:ResourceTag/${TagKey}",
+                "ec2:Encrypted",
+                "ec2:Owner",
+                "ec2:ParentVolume",
+                "ec2:Region",
+                "ec2:ResourceTag/${TagKey}",
+                "ec2:SnapshotID",
+                "ec2:SnapshotTime",
+                "ec2:VolumeSize"
+            ],
+            "description": "Grants permission to restore an Amazon EBS snapshot from the Recycle Bin",
             "orphan": false,
-            "resources": []
+            "resources": [
+                "snapshot"
+            ]
         },
         "RestoreSnapshotTier": {
-            "access_level": "Undocumented",
+            "access_level": "Write",
             "action": "RestoreSnapshotTier",
-            "condition_keys": [],
-            "description": "Not Documented by AWS",
+            "condition_keys": [
+                "aws:ResourceTag/${TagKey}",
+                "ec2:Encrypted",
+                "ec2:Owner",
+                "ec2:ParentVolume",
+                "ec2:Region",
+                "ec2:ResourceTag/${TagKey}",
+                "ec2:SnapshotID",
+                "ec2:SnapshotTime",
+                "ec2:VolumeSize"
+            ],
+            "description": "Grants permission to restore an archived Amazon EBS snapshot for use temporarily or permanently, or modify the restore period or restore type for a snapshot that was previously temporarily restored",
             "orphan": false,
-            "resources": []
+            "resources": [
+                "snapshot"
+            ]
         },
         "RevokeClientVpnIngress": {
-            "access_level": "Undocumented",
+            "access_level": "Write",
             "action": "RevokeClientVpnIngress",
-            "condition_keys": [],
-            "description": "Not Documented by AWS",
+            "condition_keys": [
+                "aws:ResourceTag/${TagKey}",
+                "ec2:ClientRootCertificateChainArn",
+                "ec2:CloudwatchLogGroupArn",
+                "ec2:CloudwatchLogStreamArn",
+                "ec2:DirectoryArn",
+                "ec2:Region",
+                "ec2:ResourceTag/${TagKey}",
+                "ec2:SamlProviderArn",
+                "ec2:ServerCertificateArn"
+            ],
+            "description": "Grants permission to remove an inbound authorization rule from a Client VPN endpoint",
             "orphan": false,
-            "resources": []
+            "resources": [
+                "client-vpn-endpoint"
+            ]
         },
         "RevokeSecurityGroupEgress": {
-            "access_level": "Undocumented",
+            "access_level": "Write",
             "action": "RevokeSecurityGroupEgress",
-            "condition_keys": [],
-            "description": "Not Documented by AWS",
+            "condition_keys": [
+                "aws:ResourceTag/${TagKey}",
+                "ec2:Region",
+                "ec2:ResourceTag/${TagKey}",
+                "ec2:SecurityGroupID",
+                "ec2:Vpc"
+            ],
+            "description": "Grants permission to remove one or more outbound rules from a VPC security group",
             "orphan": false,
-            "resources": []
+            "resources": [
+                "security-group"
+            ]
         },
         "RevokeSecurityGroupIngress": {
-            "access_level": "Undocumented",
+            "access_level": "Write",
             "action": "RevokeSecurityGroupIngress",
-            "condition_keys": [],
-            "description": "Not Documented by AWS",
+            "condition_keys": [
+                "aws:ResourceTag/${TagKey}",
+                "ec2:Region",
+                "ec2:ResourceTag/${TagKey}",
+                "ec2:SecurityGroupID",
+                "ec2:Vpc"
+            ],
+            "description": "Grants permission to remove one or more inbound rules from a security group",
             "orphan": false,
-            "resources": []
+            "resources": [
+                "security-group"
+            ]
         },
         "RunInstances": {
-            "access_level": "Undocumented",
+            "access_level": "Write",
             "action": "RunInstances",
-            "condition_keys": [],
-            "description": "Not Documented by AWS",
-            "orphan": false,
-            "resources": []
+            "condition_keys": [
+                "aws:RequestTag/${TagKey}",
+                "aws:ResourceTag/${TagKey}",
+                "aws:TagKeys",
+                "ec2:AssociatePublicIpAddress",
+                "ec2:AuthorizedService",
+                "ec2:AvailabilityZone",
+                "ec2:EbsOptimized",
+                "ec2:ElasticGpuType",
+                "ec2:Encrypted",
+                "ec2:ImageID",
+                "ec2:ImageType",
+                "ec2:InstanceAutoRecovery",
+                "ec2:InstanceID",
+                "ec2:InstanceMarketType",
+                "ec2:InstanceMetadataTags",
+                "ec2:InstanceProfile",
+                "ec2:InstanceType",
+                "ec2:IsLaunchTemplateResource",
+                "ec2:KeyPairName",
+                "ec2:KeyPairType",
+                "ec2:LaunchTemplate",
+                "ec2:MetadataHttpEndpoint",
+                "ec2:MetadataHttpPutResponseHopLimit",
+                "ec2:MetadataHttpTokens",
+                "ec2:NetworkInterfaceID",
+                "ec2:Owner",
+                "ec2:ParentSnapshot",
+                "ec2:ParentVolume",
+                "ec2:PlacementGroup",
+                "ec2:PlacementGroupName",
+                "ec2:PlacementGroupStrategy",
+                "ec2:ProductCode",
+                "ec2:Public",
+                "ec2:Region",
+                "ec2:ResourceTag/${TagKey}",
+                "ec2:RootDeviceType",
+                "ec2:SecurityGroupID",
+                "ec2:SnapshotID",
+                "ec2:SnapshotTime",
+                "ec2:Subnet",
+                "ec2:SubnetID",
+                "ec2:Tenancy",
+                "ec2:VolumeID",
+                "ec2:VolumeIops",
+                "ec2:VolumeSize",
+                "ec2:VolumeThroughput",
+                "ec2:VolumeType",
+                "ec2:Vpc"
+            ],
+            "description": "Grants permission to launch one or more instances",
+            "orphan": false,
+            "resources": [
+                "capacity-reservation",
+                "elastic-gpu",
+                "elastic-inference",
+                "group",
+                "image",
+                "instance",
+                "key-pair",
+                "launch-template",
+                "license-configuration",
+                "network-interface",
+                "placement-group",
+                "security-group",
+                "snapshot",
+                "subnet",
+                "volume"
+            ]
         },
         "RunScheduledInstances": {
-            "access_level": "Undocumented",
+            "access_level": "Write",
             "action": "RunScheduledInstances",
-            "condition_keys": [],
-            "description": "Not Documented by AWS",
+            "condition_keys": [
+                "ec2:Region"
+            ],
+            "description": "Grants permission to launch one or more Scheduled Instances",
             "orphan": false,
             "resources": []
         },
         "SearchLocalGatewayRoutes": {
-            "access_level": "Undocumented",
+            "access_level": "List",
             "action": "SearchLocalGatewayRoutes",
-            "condition_keys": [],
-            "description": "Not Documented by AWS",
+            "condition_keys": [
+                "aws:ResourceTag/${TagKey}",
+                "ec2:Region",
+                "ec2:ResourceTag/${TagKey}"
+            ],
+            "description": "Grants permission to search for routes in a local gateway route table",
             "orphan": false,
-            "resources": []
+            "resources": [
+                "local-gateway-route-table"
+            ]
         },
         "SearchTransitGatewayMulticastGroups": {
-            "access_level": "Undocumented",
+            "access_level": "List",
             "action": "SearchTransitGatewayMulticastGroups",
-            "condition_keys": [],
-            "description": "Not Documented by AWS",
+            "condition_keys": [
+                "aws:ResourceTag/${TagKey}",
+                "ec2:Region",
+                "ec2:ResourceTag/${TagKey}"
+            ],
+            "description": "Grants permission to search for groups, sources, and members in a transit gateway multicast domain",
             "orphan": false,
-            "resources": []
+            "resources": [
+                "transit-gateway-multicast-domain"
+            ]
         },
         "SearchTransitGatewayRoutes": {
-            "access_level": "Undocumented",
+            "access_level": "List",
             "action": "SearchTransitGatewayRoutes",
-            "condition_keys": [],
-            "description": "Not Documented by AWS",
+            "condition_keys": [
+                "aws:ResourceTag/${TagKey}",
+                "ec2:Region",
+                "ec2:ResourceTag/${TagKey}"
+            ],
+            "description": "Grants permission to search for routes in a transit gateway route table",
             "orphan": false,
-            "resources": []
+            "resources": [
+                "transit-gateway-route-table"
+            ]
         },
         "SendDiagnosticInterrupt": {
-            "access_level": "Undocumented",
+            "access_level": "Write",
             "action": "SendDiagnosticInterrupt",
-            "condition_keys": [],
-            "description": "Not Documented by AWS",
+            "condition_keys": [
+                "aws:ResourceTag/${TagKey}",
+                "ec2:AvailabilityZone",
+                "ec2:EbsOptimized",
+                "ec2:InstanceAutoRecovery",
+                "ec2:InstanceID",
+                "ec2:InstanceMarketType",
+                "ec2:InstanceMetadataTags",
+                "ec2:InstanceProfile",
+                "ec2:InstanceType",
+                "ec2:MetadataHttpEndpoint",
+                "ec2:MetadataHttpPutResponseHopLimit",
+                "ec2:MetadataHttpTokens",
+                "ec2:Region",
+                "ec2:ResourceTag/${TagKey}",
+                "ec2:RootDeviceType",
+                "ec2:Tenancy"
+            ],
+            "description": "Grants permission to send a diagnostic interrupt to an Amazon EC2 instance",
             "orphan": false,
-            "resources": []
+            "resources": [
+                "instance"
+            ]
         },
         "SendSpotInstanceInterruptions": {
-            "access_level": "Undocumented",
+            "access_level": "Write",
             "action": "SendSpotInstanceInterruptions",
-            "condition_keys": [],
-            "description": "Not Documented by AWS",
+            "condition_keys": [
+                "aws:ResourceTag/${TagKey}",
+                "ec2:AvailabilityZone",
+                "ec2:EbsOptimized",
+                "ec2:InstanceAutoRecovery",
+                "ec2:InstanceID",
+                "ec2:InstanceMarketType",
+                "ec2:InstanceMetadataTags",
+                "ec2:InstanceProfile",
+                "ec2:InstanceType",
+                "ec2:MetadataHttpEndpoint",
+                "ec2:MetadataHttpPutResponseHopLimit",
+                "ec2:MetadataHttpTokens",
+                "ec2:Region",
+                "ec2:ResourceTag/${TagKey}",
+                "ec2:RootDeviceType",
+                "ec2:Tenancy"
+            ],
+            "description": "Grants permission to interrupt a Spot Instance",
             "orphan": false,
-            "resources": []
+            "resources": [
+                "instance"
+            ]
         },
         "StartInstances": {
-            "access_level": "Undocumented",
+            "access_level": "Write",
             "action": "StartInstances",
-            "condition_keys": [],
-            "description": "Not Documented by AWS",
+            "condition_keys": [
+                "aws:ResourceTag/${TagKey}",
+                "ec2:AvailabilityZone",
+                "ec2:EbsOptimized",
+                "ec2:InstanceID",
+                "ec2:InstanceMarketType",
+                "ec2:InstanceProfile",
+                "ec2:InstanceType",
+                "ec2:PlacementGroup",
+                "ec2:Region",
+                "ec2:ResourceTag/${TagKey}",
+                "ec2:RootDeviceType",
+                "ec2:Tenancy"
+            ],
+            "description": "Grants permission to start a stopped instance",
             "orphan": false,
-            "resources": []
+            "resources": [
+                "instance",
+                "license-configuration"
+            ]
         },
         "StartNetworkInsightsAccessScopeAnalysis": {
-            "access_level": "Undocumented",
+            "access_level": "Write",
             "action": "StartNetworkInsightsAccessScopeAnalysis",
-            "condition_keys": [],
-            "description": "Not Documented by AWS",
+            "condition_keys": [
+                "aws:RequestTag/${TagKey}",
+                "aws:ResourceTag/${TagKey}",
+                "aws:TagKeys",
+                "ec2:Region",
+                "ec2:ResourceTag/${TagKey}"
+            ],
+            "description": "Grants permission to start a Network Access Scope analysis",
             "orphan": false,
-            "resources": []
+            "resources": [
+                "network-insights-access-scope",
+                "network-insights-access-scope-analysis"
+            ]
         },
         "StartNetworkInsightsAnalysis": {
-            "access_level": "Undocumented",
+            "access_level": "Write",
             "action": "StartNetworkInsightsAnalysis",
-            "condition_keys": [],
-            "description": "Not Documented by AWS",
+            "condition_keys": [
+                "aws:RequestTag/${TagKey}",
+                "aws:ResourceTag/${TagKey}",
+                "aws:TagKeys",
+                "ec2:Region",
+                "ec2:ResourceTag/${TagKey}"
+            ],
+            "description": "Grants permission to start analyzing a specified path",
             "orphan": false,
-            "resources": []
+            "resources": [
+                "network-insights-analysis",
+                "network-insights-path"
+            ]
         },
         "StartVpcEndpointServicePrivateDnsVerification": {
-            "access_level": "Undocumented",
+            "access_level": "Write",
             "action": "StartVpcEndpointServicePrivateDnsVerification",
-            "condition_keys": [],
-            "description": "Not Documented by AWS",
+            "condition_keys": [
+                "aws:ResourceTag/${TagKey}",
+                "ec2:Region",
+                "ec2:ResourceTag/${TagKey}"
+            ],
+            "description": "Grants permission to start the private DNS verification process for a VPC endpoint service",
             "orphan": false,
-            "resources": []
+            "resources": [
+                "vpc-endpoint-service"
+            ]
         },
         "StopInstances": {
-            "access_level": "Undocumented",
+            "access_level": "Write",
             "action": "StopInstances",
-            "condition_keys": [],
-            "description": "Not Documented by AWS",
+            "condition_keys": [
+                "aws:ResourceTag/${TagKey}",
+                "ec2:AvailabilityZone",
+                "ec2:EbsOptimized",
+                "ec2:InstanceID",
+                "ec2:InstanceMarketType",
+                "ec2:InstanceProfile",
+                "ec2:InstanceType",
+                "ec2:PlacementGroup",
+                "ec2:Region",
+                "ec2:ResourceTag/${TagKey}",
+                "ec2:RootDeviceType",
+                "ec2:Tenancy"
+            ],
+            "description": "Grants permission to stop an Amazon EBS-backed instance",
             "orphan": false,
-            "resources": []
+            "resources": [
+                "instance"
+            ]
         },
         "TerminateClientVpnConnections": {
-            "access_level": "Undocumented",
+            "access_level": "Write",
             "action": "TerminateClientVpnConnections",
-            "condition_keys": [],
-            "description": "Not Documented by AWS",
+            "condition_keys": [
+                "aws:ResourceTag/${TagKey}",
+                "ec2:ClientRootCertificateChainArn",
+                "ec2:CloudwatchLogGroupArn",
+                "ec2:CloudwatchLogStreamArn",
+                "ec2:DirectoryArn",
+                "ec2:Region",
+                "ec2:ResourceTag/${TagKey}",
+                "ec2:SamlProviderArn",
+                "ec2:ServerCertificateArn"
+            ],
+            "description": "Grants permission to terminate active Client VPN endpoint connections",
             "orphan": false,
-            "resources": []
+            "resources": [
+                "client-vpn-endpoint"
+            ]
         },
         "TerminateInstances": {
-            "access_level": "Undocumented",
+            "access_level": "Write",
             "action": "TerminateInstances",
-            "condition_keys": [],
-            "description": "Not Documented by AWS",
+            "condition_keys": [
+                "aws:ResourceTag/${TagKey}",
+                "ec2:AvailabilityZone",
+                "ec2:EbsOptimized",
+                "ec2:InstanceID",
+                "ec2:InstanceMarketType",
+                "ec2:InstanceProfile",
+                "ec2:InstanceType",
+                "ec2:MetadataHttpEndpoint",
+                "ec2:MetadataHttpPutResponseHopLimit",
+                "ec2:MetadataHttpTokens",
+                "ec2:PlacementGroup",
+                "ec2:Region",
+                "ec2:ResourceTag/${TagKey}",
+                "ec2:RootDeviceType",
+                "ec2:Tenancy"
+            ],
+            "description": "Grants permission to shut down one or more instances",
             "orphan": false,
-            "resources": []
+            "resources": [
+                "instance"
+            ]
         },
         "UnassignIpv6Addresses": {
-            "access_level": "Undocumented",
+            "access_level": "Write",
             "action": "UnassignIpv6Addresses",
-            "condition_keys": [],
-            "description": "Not Documented by AWS",
+            "condition_keys": [
+                "aws:ResourceTag/${TagKey}",
+                "ec2:AvailabilityZone",
+                "ec2:NetworkInterfaceID",
+                "ec2:Region",
+                "ec2:ResourceTag/${TagKey}",
+                "ec2:Subnet",
+                "ec2:Vpc"
+            ],
+            "description": "Grants permission to unassign one or more IPv6 addresses from a network interface",
             "orphan": false,
-            "resources": []
+            "resources": [
+                "network-interface"
+            ]
         },
         "UnassignPrivateIpAddresses": {
-            "access_level": "Undocumented",
+            "access_level": "Write",
             "action": "UnassignPrivateIpAddresses",
-            "condition_keys": [],
-            "description": "Not Documented by AWS",
+            "condition_keys": [
+                "aws:ResourceTag/${TagKey}",
+                "ec2:AvailabilityZone",
+                "ec2:NetworkInterfaceID",
+                "ec2:Region",
+                "ec2:ResourceTag/${TagKey}",
+                "ec2:Subnet",
+                "ec2:Vpc"
+            ],
+            "description": "Grants permission to unassign one or more secondary private IP addresses from a network interface",
             "orphan": false,
-            "resources": []
+            "resources": [
+                "network-interface"
+            ]
         },
         "UnassignPrivateNatGatewayAddress": {
-            "access_level": "Undocumented",
+            "access_level": "Write",
             "action": "UnassignPrivateNatGatewayAddress",
-            "condition_keys": [],
-            "description": "Not Documented by AWS",
+            "condition_keys": [
+                "aws:ResourceTag/${TagKey}",
+                "ec2:Region",
+                "ec2:ResourceTag/${TagKey}"
+            ],
+            "description": "Grants permission to unassign secondary private IPv4 addresses from a private NAT gateway",
             "orphan": false,
-            "resources": []
+            "resources": [
+                "natgateway"
+            ]
         },
         "UnmonitorInstances": {
-            "access_level": "Undocumented",
+            "access_level": "Write",
             "action": "UnmonitorInstances",
-            "condition_keys": [],
-            "description": "Not Documented by AWS",
+            "condition_keys": [
+                "aws:ResourceTag/${TagKey}",
+                "ec2:AvailabilityZone",
+                "ec2:EbsOptimized",
+                "ec2:InstanceAutoRecovery",
+                "ec2:InstanceID",
+                "ec2:InstanceMarketType",
+                "ec2:InstanceMetadataTags",
+                "ec2:InstanceProfile",
+                "ec2:InstanceType",
+                "ec2:MetadataHttpEndpoint",
+                "ec2:MetadataHttpPutResponseHopLimit",
+                "ec2:MetadataHttpTokens",
+                "ec2:PlacementGroup",
+                "ec2:ProductCode",
+                "ec2:Region",
+                "ec2:ResourceTag/${TagKey}",
+                "ec2:RootDeviceType",
+                "ec2:Tenancy"
+            ],
+            "description": "Grants permission to disable detailed monitoring for a running instance",
             "orphan": false,
-            "resources": []
+            "resources": [
+                "instance"
+            ]
         },
         "UpdateSecurityGroupRuleDescriptionsEgress": {
-            "access_level": "Undocumented",
+            "access_level": "Write",
             "action": "UpdateSecurityGroupRuleDescriptionsEgress",
-            "condition_keys": [],
-            "description": "Not Documented by AWS",
+            "condition_keys": [
+                "aws:ResourceTag/${TagKey}",
+                "ec2:Region",
+                "ec2:ResourceTag/${TagKey}",
+                "ec2:SecurityGroupID",
+                "ec2:Vpc"
+            ],
+            "description": "Grants permission to update descriptions for one or more outbound rules in a VPC security group",
             "orphan": false,
-            "resources": []
+            "resources": [
+                "security-group"
+            ]
         },
         "UpdateSecurityGroupRuleDescriptionsIngress": {
-            "access_level": "Undocumented",
+            "access_level": "Write",
             "action": "UpdateSecurityGroupRuleDescriptionsIngress",
-            "condition_keys": [],
-            "description": "Not Documented by AWS",
+            "condition_keys": [
+                "aws:ResourceTag/${TagKey}",
+                "ec2:Region",
+                "ec2:ResourceTag/${TagKey}",
+                "ec2:SecurityGroupID",
+                "ec2:Vpc"
+            ],
+            "description": "Grants permission to update descriptions for one or more inbound rules in a security group",
             "orphan": false,
-            "resources": []
+            "resources": [
+                "security-group"
+            ]
         },
         "WithdrawByoipCidr": {
-            "access_level": "Undocumented",
+            "access_level": "Write",
             "action": "WithdrawByoipCidr",
-            "condition_keys": [],
-            "description": "Not Documented by AWS",
+            "condition_keys": [
+                "ec2:Region"
+            ],
+            "description": "Grants permission to stop advertising an address range that was provisioned for use in AWS through bring your own IP addresses (BYOIP)",
             "orphan": false,
             "resources": []
         }
     },
     "ec2-instance-connect": {
         "SendSSHPublicKey": {
             "access_level": "Write",
@@ -54994,27 +60058,75 @@
             "orphan": false,
             "resources": [
                 "execute-api-general"
             ]
         }
     },
     "finspace": {
+        "ConnectKxCluster": {
+            "access_level": "Undocumented",
+            "action": "ConnectKxCluster",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
+            "orphan": false,
+            "resources": []
+        },
         "CreateEnvironment": {
             "access_level": "Write",
             "action": "CreateEnvironment",
             "condition_keys": [
                 "aws:RequestTag/${TagKey}",
                 "aws:TagKeys"
             ],
             "description": "Grants permission to create a FinSpace environment",
             "orphan": false,
             "resources": [
                 "environment"
             ]
         },
+        "CreateKxChangeset": {
+            "access_level": "Undocumented",
+            "action": "CreateKxChangeset",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
+            "orphan": false,
+            "resources": []
+        },
+        "CreateKxCluster": {
+            "access_level": "Undocumented",
+            "action": "CreateKxCluster",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
+            "orphan": false,
+            "resources": []
+        },
+        "CreateKxDatabase": {
+            "access_level": "Undocumented",
+            "action": "CreateKxDatabase",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
+            "orphan": false,
+            "resources": []
+        },
+        "CreateKxEnvironment": {
+            "access_level": "Undocumented",
+            "action": "CreateKxEnvironment",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
+            "orphan": false,
+            "resources": []
+        },
+        "CreateKxUser": {
+            "access_level": "Undocumented",
+            "action": "CreateKxUser",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
+            "orphan": false,
+            "resources": []
+        },
         "CreateUser": {
             "access_level": "Write",
             "action": "CreateUser",
             "condition_keys": [
                 "aws:RequestTag/${TagKey}",
                 "aws:TagKeys"
             ],
@@ -55031,24 +60143,104 @@
             "condition_keys": [],
             "description": "Grants permission to delete a FinSpace environment",
             "orphan": false,
             "resources": [
                 "environment"
             ]
         },
+        "DeleteKxCluster": {
+            "access_level": "Undocumented",
+            "action": "DeleteKxCluster",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
+            "orphan": false,
+            "resources": []
+        },
+        "DeleteKxDatabase": {
+            "access_level": "Undocumented",
+            "action": "DeleteKxDatabase",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
+            "orphan": false,
+            "resources": []
+        },
+        "DeleteKxEnvironment": {
+            "access_level": "Undocumented",
+            "action": "DeleteKxEnvironment",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
+            "orphan": false,
+            "resources": []
+        },
+        "DeleteKxUser": {
+            "access_level": "Undocumented",
+            "action": "DeleteKxUser",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
+            "orphan": false,
+            "resources": []
+        },
         "GetEnvironment": {
             "access_level": "Read",
             "action": "GetEnvironment",
             "condition_keys": [],
             "description": "Grants permission to describe a FinSpace environment",
             "orphan": false,
             "resources": [
                 "environment"
             ]
         },
+        "GetKxChangeset": {
+            "access_level": "Undocumented",
+            "action": "GetKxChangeset",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
+            "orphan": false,
+            "resources": []
+        },
+        "GetKxCluster": {
+            "access_level": "Undocumented",
+            "action": "GetKxCluster",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
+            "orphan": false,
+            "resources": []
+        },
+        "GetKxConnectionString": {
+            "access_level": "Undocumented",
+            "action": "GetKxConnectionString",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
+            "orphan": false,
+            "resources": []
+        },
+        "GetKxDatabase": {
+            "access_level": "Undocumented",
+            "action": "GetKxDatabase",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
+            "orphan": false,
+            "resources": []
+        },
+        "GetKxEnvironment": {
+            "access_level": "Undocumented",
+            "action": "GetKxEnvironment",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
+            "orphan": false,
+            "resources": []
+        },
+        "GetKxUser": {
+            "access_level": "Undocumented",
+            "action": "GetKxUser",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
+            "orphan": false,
+            "resources": []
+        },
         "GetLoadSampleDataSetGroupIntoEnvironmentStatus": {
             "access_level": "Read",
             "action": "GetLoadSampleDataSetGroupIntoEnvironmentStatus",
             "condition_keys": [],
             "description": "Grants permission to request status of the loading of sample data bundle",
             "orphan": false,
             "resources": [
@@ -55072,14 +60264,62 @@
             "condition_keys": [],
             "description": "Grants permission to list FinSpace environments in the AWS account",
             "orphan": false,
             "resources": [
                 "environment"
             ]
         },
+        "ListKxChangesets": {
+            "access_level": "Undocumented",
+            "action": "ListKxChangesets",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
+            "orphan": false,
+            "resources": []
+        },
+        "ListKxClusterNodes": {
+            "access_level": "Undocumented",
+            "action": "ListKxClusterNodes",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
+            "orphan": false,
+            "resources": []
+        },
+        "ListKxClusters": {
+            "access_level": "Undocumented",
+            "action": "ListKxClusters",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
+            "orphan": false,
+            "resources": []
+        },
+        "ListKxDatabases": {
+            "access_level": "Undocumented",
+            "action": "ListKxDatabases",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
+            "orphan": false,
+            "resources": []
+        },
+        "ListKxEnvironments": {
+            "access_level": "Undocumented",
+            "action": "ListKxEnvironments",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
+            "orphan": false,
+            "resources": []
+        },
+        "ListKxUsers": {
+            "access_level": "Undocumented",
+            "action": "ListKxUsers",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
+            "orphan": false,
+            "resources": []
+        },
         "ListTagsForResource": {
             "access_level": "Read",
             "action": "ListTagsForResource",
             "condition_keys": [],
             "description": "Grants permission to return a list of tags for a resource",
             "orphan": false,
             "resources": [
@@ -55103,14 +60343,22 @@
             "condition_keys": [],
             "description": "Grants permission to load sample data bundle into your FinSpace environment",
             "orphan": false,
             "resources": [
                 "environment"
             ]
         },
+        "MountKxDatabase": {
+            "access_level": "Undocumented",
+            "action": "MountKxDatabase",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
+            "orphan": false,
+            "resources": []
+        },
         "ResetUserPassword": {
             "access_level": "Write",
             "action": "ResetUserPassword",
             "condition_keys": [],
             "description": "Grants permission to reset the password for a FinSpace user",
             "orphan": false,
             "resources": [
@@ -55144,14 +60392,54 @@
             "condition_keys": [],
             "description": "Grants permission to update a FinSpace environment",
             "orphan": false,
             "resources": [
                 "environment"
             ]
         },
+        "UpdateKxClusterDatabases": {
+            "access_level": "Undocumented",
+            "action": "UpdateKxClusterDatabases",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
+            "orphan": false,
+            "resources": []
+        },
+        "UpdateKxDatabase": {
+            "access_level": "Undocumented",
+            "action": "UpdateKxDatabase",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
+            "orphan": false,
+            "resources": []
+        },
+        "UpdateKxEnvironment": {
+            "access_level": "Undocumented",
+            "action": "UpdateKxEnvironment",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
+            "orphan": false,
+            "resources": []
+        },
+        "UpdateKxEnvironmentNetwork": {
+            "access_level": "Undocumented",
+            "action": "UpdateKxEnvironmentNetwork",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
+            "orphan": false,
+            "resources": []
+        },
+        "UpdateKxUser": {
+            "access_level": "Undocumented",
+            "action": "UpdateKxUser",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
+            "orphan": false,
+            "resources": []
+        },
         "UpdateUser": {
             "access_level": "Write",
             "action": "UpdateUser",
             "condition_keys": [],
             "description": "Grants permission to update a FinSpace user",
             "orphan": false,
             "resources": [
@@ -69782,14 +75070,30 @@
             ],
             "description": "Grants permission to create an OTA update job",
             "orphan": false,
             "resources": [
                 "otaupdate"
             ]
         },
+        "CreatePackage": {
+            "access_level": "Undocumented",
+            "action": "CreatePackage",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
+            "orphan": false,
+            "resources": []
+        },
+        "CreatePackageVersion": {
+            "access_level": "Undocumented",
+            "action": "CreatePackageVersion",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
+            "orphan": false,
+            "resources": []
+        },
         "CreatePolicy": {
             "access_level": "Write",
             "action": "CreatePolicy",
             "condition_keys": [
                 "aws:RequestTag/${TagKey}",
                 "aws:TagKeys"
             ],
@@ -70109,14 +75413,30 @@
             "condition_keys": [],
             "description": "Grants permission to delete an OTA update job",
             "orphan": false,
             "resources": [
                 "otaupdate"
             ]
         },
+        "DeletePackage": {
+            "access_level": "Undocumented",
+            "action": "DeletePackage",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
+            "orphan": false,
+            "resources": []
+        },
+        "DeletePackageVersion": {
+            "access_level": "Undocumented",
+            "action": "DeletePackageVersion",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
+            "orphan": false,
+            "resources": []
+        },
         "DeletePolicy": {
             "access_level": "Write",
             "action": "DeletePolicy",
             "condition_keys": [],
             "description": "Grants permission to delete the specified policy",
             "orphan": false,
             "resources": [
@@ -70736,14 +76056,38 @@
             "condition_keys": [],
             "description": "Grants permission to get the information about the OTA update job",
             "orphan": false,
             "resources": [
                 "otaupdate"
             ]
         },
+        "GetPackage": {
+            "access_level": "Undocumented",
+            "action": "GetPackage",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
+            "orphan": false,
+            "resources": []
+        },
+        "GetPackageConfiguration": {
+            "access_level": "Undocumented",
+            "action": "GetPackageConfiguration",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
+            "orphan": false,
+            "resources": []
+        },
+        "GetPackageVersion": {
+            "access_level": "Undocumented",
+            "action": "GetPackageVersion",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
+            "orphan": false,
+            "resources": []
+        },
         "GetPercentiles": {
             "access_level": "Read",
             "action": "GetPercentiles",
             "condition_keys": [],
             "description": "Grants permission to get percentiles for IoT fleet index",
             "orphan": false,
             "resources": [
@@ -71077,14 +76421,30 @@
             "access_level": "List",
             "action": "ListOutgoingCertificates",
             "condition_keys": [],
             "description": "Grants permission to list certificates that are being transfered but not yet accepted",
             "orphan": false,
             "resources": []
         },
+        "ListPackageVersions": {
+            "access_level": "Undocumented",
+            "action": "ListPackageVersions",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
+            "orphan": false,
+            "resources": []
+        },
+        "ListPackages": {
+            "access_level": "Undocumented",
+            "action": "ListPackages",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
+            "orphan": false,
+            "resources": []
+        },
         "ListPolicies": {
             "access_level": "List",
             "action": "ListPolicies",
             "condition_keys": [],
             "description": "Grants permission to list your policies",
             "orphan": false,
             "resources": []
@@ -71855,14 +77215,38 @@
             "condition_keys": [],
             "description": "Grants permission to update the definition for the specified mitigation action",
             "orphan": false,
             "resources": [
                 "mitigationaction"
             ]
         },
+        "UpdatePackage": {
+            "access_level": "Undocumented",
+            "action": "UpdatePackage",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
+            "orphan": false,
+            "resources": []
+        },
+        "UpdatePackageConfiguration": {
+            "access_level": "Undocumented",
+            "action": "UpdatePackageConfiguration",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
+            "orphan": false,
+            "resources": []
+        },
+        "UpdatePackageVersion": {
+            "access_level": "Undocumented",
+            "action": "UpdatePackageVersion",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
+            "orphan": false,
+            "resources": []
+        },
         "UpdateProvisioningTemplate": {
             "access_level": "Write",
             "action": "UpdateProvisioningTemplate",
             "condition_keys": [],
             "description": "Grants permission to update a fleet provisioning template",
             "orphan": false,
             "resources": [
@@ -80355,14 +85739,15 @@
             ]
         },
         "ScheduleKeyDeletion": {
             "access_level": "Write",
             "action": "ScheduleKeyDeletion",
             "condition_keys": [
                 "kms:CallerAccount",
+                "kms:ScheduleKeyDeletionPendingWindowInDays",
                 "kms:ViaService"
             ],
             "description": "Controls permission to schedule deletion of an AWS KMS key",
             "orphan": false,
             "resources": [
                 "key"
             ]
@@ -85476,24 +90861,40 @@
             "description": "Grants permission to create or update a subscription filter and associates it with the specified log group",
             "orphan": false,
             "resources": [
                 "destination",
                 "log-group"
             ]
         },
+        "StartLiveTail": {
+            "access_level": "Read",
+            "action": "StartLiveTail",
+            "condition_keys": [],
+            "description": "Grants permission to start a livetail session in CloudWatch Logs",
+            "orphan": false,
+            "resources": []
+        },
         "StartQuery": {
             "access_level": "Read",
             "action": "StartQuery",
             "condition_keys": [],
             "description": "Grants permission to schedule a query of a log group using CloudWatch Logs Insights",
             "orphan": false,
             "resources": [
                 "log-group"
             ]
         },
+        "StopLiveTail": {
+            "access_level": "Read",
+            "action": "StopLiveTail",
+            "condition_keys": [],
+            "description": "Grants permission to stop a CloudWatch Logs livetail session that is in progress",
+            "orphan": false,
+            "resources": []
+        },
         "StopQuery": {
             "access_level": "Read",
             "action": "StopQuery",
             "condition_keys": [],
             "description": "Grants permission to stop a CloudWatch Logs Insights query that is in progress",
             "orphan": false,
             "resources": []
@@ -129094,14 +134495,22 @@
             "condition_keys": [],
             "description": "Grants permission to return information about a specific Signing Job",
             "orphan": false,
             "resources": [
                 "signing-job"
             ]
         },
+        "GetRevocationStatus": {
+            "access_level": "Undocumented",
+            "action": "GetRevocationStatus",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
+            "orphan": false,
+            "resources": []
+        },
         "GetSigningPlatform": {
             "access_level": "Read",
             "action": "GetSigningPlatform",
             "condition_keys": [],
             "description": "Grants permission to return information about a specific Signing Platform",
             "orphan": false,
             "resources": []
@@ -129205,14 +134614,22 @@
             ],
             "description": "Grants permission to change the state of a Signing Profile to REVOKED",
             "orphan": false,
             "resources": [
                 "signing-profile"
             ]
         },
+        "SignPayload": {
+            "access_level": "Undocumented",
+            "action": "SignPayload",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
+            "orphan": false,
+            "resources": []
+        },
         "StartSigningJob": {
             "access_level": "Write",
             "action": "StartSigningJob",
             "condition_keys": [
                 "signer:ProfileVersion"
             ],
             "description": "Grants permission to initiate a Signing Job on the provided code",
@@ -143503,26 +148920,26 @@
             "description": "Grants permission to delete a WebACL",
             "orphan": false,
             "resources": [
                 "webacl"
             ]
         },
         "DescribeAllManagedProducts": {
-            "access_level": "Undocumented",
+            "access_level": "Read",
             "action": "DescribeAllManagedProducts",
             "condition_keys": [],
-            "description": "Not Documented by AWS",
+            "description": "Grants permission to retrieve product information for a managed rule group",
             "orphan": false,
             "resources": []
         },
         "DescribeManagedProductsByVendor": {
-            "access_level": "Undocumented",
+            "access_level": "Read",
             "action": "DescribeManagedProductsByVendor",
             "condition_keys": [],
-            "description": "Not Documented by AWS",
+            "description": "Grants permission to retrieve product information for a managed rule group by a given vendor",
             "orphan": false,
             "resources": []
         },
         "DescribeManagedRuleGroup": {
             "access_level": "Read",
             "action": "DescribeManagedRuleGroup",
             "condition_keys": [],
```

### Comparing `iam_actions-1.2.20230606/iam_actions/generate/action_map.py` & `iam_actions-1.2.20230607/iam_actions/generate/action_map.py`

 * *Files identical despite different names*

### Comparing `iam_actions-1.2.20230606/iam_actions/generate/aws_docs.py` & `iam_actions-1.2.20230607/iam_actions/generate/aws_docs.py`

 * *Files identical despite different names*

### Comparing `iam_actions-1.2.20230606/iam_actions/generate/generate.py` & `iam_actions-1.2.20230607/iam_actions/generate/generate.py`

 * *Files identical despite different names*

### Comparing `iam_actions-1.2.20230606/iam_actions/generate/notifier.py` & `iam_actions-1.2.20230607/iam_actions/generate/notifier.py`

 * *Files identical despite different names*

### Comparing `iam_actions-1.2.20230606/iam_actions/generate/resource_type.py` & `iam_actions-1.2.20230607/iam_actions/generate/resource_type.py`

 * *Files identical despite different names*

### Comparing `iam_actions-1.2.20230606/iam_actions/generate/services.py` & `iam_actions-1.2.20230607/iam_actions/generate/services.py`

 * *Files identical despite different names*

### Comparing `iam_actions-1.2.20230606/iam_actions/policies.json` & `iam_actions-1.2.20230607/iam_actions/policies.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9994616773980397%*

 * *Differences: {"'serviceMap'": "{'AWS IoT': {'Actions': {insert: [(32, 'CreatePackage'), (33, "*

 * *                 "'CreatePackageVersion'), (64, 'DeletePackage'), (65, 'DeletePackageVersion'), "*

 * *                 "(131, 'GetPackage'), (132, 'GetPackageConfiguration'), (133, "*

 * *                 "'GetPackageVersion'), (173, 'ListPackageVersions'), (174, 'ListPackages'), (252, "*

 * *                 "'UpdatePackage'), (253, 'UpdatePackageConfiguration'), (254, "*

 * *                 "'UpdatePackageVersion')]}}, 'AWS Signer': {'Actions […]*

```diff
@@ -4965,14 +4965,16 @@
                 "CreateDynamicThingGroup",
                 "CreateFleetMetric",
                 "CreateJob",
                 "CreateJobTemplate",
                 "CreateKeysAndCertificate",
                 "CreateMitigationAction",
                 "CreateOTAUpdate",
+                "CreatePackage",
+                "CreatePackageVersion",
                 "CreatePolicy",
                 "CreatePolicyVersion",
                 "CreateProvisioningClaim",
                 "CreateProvisioningTemplate",
                 "CreateProvisioningTemplateVersion",
                 "CreateRoleAlias",
                 "CreateScheduledAudit",
@@ -4995,14 +4997,16 @@
                 "DeleteDynamicThingGroup",
                 "DeleteFleetMetric",
                 "DeleteJob",
                 "DeleteJobExecution",
                 "DeleteJobTemplate",
                 "DeleteMitigationAction",
                 "DeleteOTAUpdate",
+                "DeletePackage",
+                "DeletePackageVersion",
                 "DeletePolicy",
                 "DeletePolicyVersion",
                 "DeleteProvisioningTemplate",
                 "DeleteProvisioningTemplateVersion",
                 "DeleteRegistrationCode",
                 "DeleteRoleAlias",
                 "DeleteScheduledAudit",
@@ -5060,14 +5064,17 @@
                 "GetBucketsAggregation",
                 "GetCardinality",
                 "GetEffectivePolicies",
                 "GetIndexingConfiguration",
                 "GetJobDocument",
                 "GetLoggingOptions",
                 "GetOTAUpdate",
+                "GetPackage",
+                "GetPackageConfiguration",
+                "GetPackageVersion",
                 "GetPercentiles",
                 "GetPolicy",
                 "GetPolicyVersion",
                 "GetRegistrationCode",
                 "GetRetainedMessage",
                 "GetStatistics",
                 "GetThingShadow",
@@ -5099,14 +5106,16 @@
                 "ListJobs",
                 "ListManagedJobTemplates",
                 "ListMetricValues",
                 "ListMitigationActions",
                 "ListNamedShadowsForThing",
                 "ListOTAUpdates",
                 "ListOutgoingCertificates",
+                "ListPackageVersions",
+                "ListPackages",
                 "ListPolicies",
                 "ListPolicyPrincipals",
                 "ListPolicyVersions",
                 "ListPrincipalPolicies",
                 "ListPrincipalThings",
                 "ListProvisioningTemplateVersions",
                 "ListProvisioningTemplates",
@@ -5176,14 +5185,17 @@
                 "UpdateDomainConfiguration",
                 "UpdateDynamicThingGroup",
                 "UpdateEventConfigurations",
                 "UpdateFleetMetric",
                 "UpdateIndexingConfiguration",
                 "UpdateJob",
                 "UpdateMitigationAction",
+                "UpdatePackage",
+                "UpdatePackageConfiguration",
+                "UpdatePackageVersion",
                 "UpdateProvisioningTemplate",
                 "UpdateRoleAlias",
                 "UpdateScheduledAudit",
                 "UpdateSecurityProfile",
                 "UpdateStream",
                 "UpdateThing",
                 "UpdateThingGroup",
@@ -8204,25 +8216,27 @@
         "AWS Signer": {
             "ARNFormat": "arn:aws:signer:${Region}:${Account}:/${ResourceType}/${ResourceIdentifier}",
             "ARNRegex": "^arn:aws:signer:.+",
             "Actions": [
                 "AddProfilePermission",
                 "CancelSigningProfile",
                 "DescribeSigningJob",
+                "GetRevocationStatus",
                 "GetSigningPlatform",
                 "GetSigningProfile",
                 "ListProfilePermissions",
                 "ListSigningJobs",
                 "ListSigningPlatforms",
                 "ListSigningProfiles",
                 "ListTagsForResource",
                 "PutSigningProfile",
                 "RemoveProfilePermission",
                 "RevokeSignature",
                 "RevokeSigningProfile",
+                "SignPayload",
                 "StartSigningJob",
                 "TagResource",
                 "UntagResource"
             ],
             "HasResource": true,
             "StringPrefix": "signer",
             "conditionKeys": [
@@ -10790,15 +10804,17 @@
                 "PutDestinationPolicy",
                 "PutLogEvents",
                 "PutMetricFilter",
                 "PutQueryDefinition",
                 "PutResourcePolicy",
                 "PutRetentionPolicy",
                 "PutSubscriptionFilter",
+                "StartLiveTail",
                 "StartQuery",
+                "StopLiveTail",
                 "StopQuery",
                 "TagLogGroup",
                 "TagResource",
                 "TestMetricFilter",
                 "Unmask",
                 "UntagLogGroup",
                 "UntagResource",
@@ -12043,376 +12059,15 @@
             ],
             "HasResource": true,
             "StringPrefix": "dax",
             "conditionKeys": [
                 "dax:EnclosingOperation"
             ]
         },
-        "Amazon EC2 Auto Scaling": {
-            "ARNFormat": "arn:aws:autoscaling:${Region}:${Account}:${RelativeId}",
-            "ARNRegex": "^arn:aws:autoscaling:.+:.+:.+",
-            "Actions": [
-                "AttachInstances",
-                "AttachLoadBalancerTargetGroups",
-                "AttachLoadBalancers",
-                "AttachTrafficSources",
-                "BatchDeleteScheduledAction",
-                "BatchPutScheduledUpdateGroupAction",
-                "CancelInstanceRefresh",
-                "CompleteLifecycleAction",
-                "CreateAutoScalingGroup",
-                "CreateLaunchConfiguration",
-                "CreateOrUpdateTags",
-                "DeleteAutoScalingGroup",
-                "DeleteLaunchConfiguration",
-                "DeleteLifecycleHook",
-                "DeleteNotificationConfiguration",
-                "DeletePolicy",
-                "DeleteScheduledAction",
-                "DeleteTags",
-                "DeleteWarmPool",
-                "DescribeAccountLimits",
-                "DescribeAdjustmentTypes",
-                "DescribeAutoScalingGroups",
-                "DescribeAutoScalingInstances",
-                "DescribeAutoScalingNotificationTypes",
-                "DescribeInstanceRefreshes",
-                "DescribeLaunchConfigurations",
-                "DescribeLifecycleHookTypes",
-                "DescribeLifecycleHooks",
-                "DescribeLoadBalancerTargetGroups",
-                "DescribeLoadBalancers",
-                "DescribeMetricCollectionTypes",
-                "DescribeNotificationConfigurations",
-                "DescribePolicies",
-                "DescribeScalingActivities",
-                "DescribeScalingProcessTypes",
-                "DescribeScheduledActions",
-                "DescribeTags",
-                "DescribeTerminationPolicyTypes",
-                "DescribeTrafficSources",
-                "DescribeWarmPool",
-                "DetachInstances",
-                "DetachLoadBalancerTargetGroups",
-                "DetachLoadBalancers",
-                "DetachTrafficSources",
-                "DisableMetricsCollection",
-                "EnableMetricsCollection",
-                "EnterStandby",
-                "ExecutePolicy",
-                "ExitStandby",
-                "GetPredictiveScalingForecast",
-                "PutLifecycleHook",
-                "PutNotificationConfiguration",
-                "PutScalingPolicy",
-                "PutScheduledUpdateGroupAction",
-                "PutWarmPool",
-                "RecordLifecycleActionHeartbeat",
-                "ResumeProcesses",
-                "RollbackInstanceRefresh",
-                "SetDesiredCapacity",
-                "SetInstanceHealth",
-                "SetInstanceProtection",
-                "StartInstanceRefresh",
-                "SuspendProcesses",
-                "TerminateInstanceInAutoScalingGroup",
-                "UpdateAutoScalingGroup"
-            ],
-            "HasResource": true,
-            "StringPrefix": "autoscaling",
-            "conditionKeys": [
-                "autoscaling:ImageId",
-                "autoscaling:InstanceType",
-                "autoscaling:InstanceTypes",
-                "autoscaling:LaunchConfigurationName",
-                "autoscaling:LaunchTemplateVersionSpecified",
-                "autoscaling:LoadBalancerNames",
-                "autoscaling:MaxSize",
-                "autoscaling:MetadataHttpEndpoint",
-                "autoscaling:MetadataHttpPutResponseHopLimit",
-                "autoscaling:MetadataHttpTokens",
-                "autoscaling:MinSize",
-                "autoscaling:ResourceTag/${TagKey}",
-                "autoscaling:SpotPrice",
-                "autoscaling:TargetGroupARNs",
-                "autoscaling:TrafficSourceIdentifiers",
-                "autoscaling:VPCZoneIdentifiers",
-                "aws:RequestTag/${TagKey}",
-                "aws:ResourceTag/${TagKey}",
-                "aws:TagKeys"
-            ]
-        },
-        "Amazon EC2 Image Builder": {
-            "ARNFormat": "arn:aws:imagebuilder:${Region}:${Account}:${ResourceType}/${ResourceName}",
-            "ARNRegex": "^arn:aws:imagebuilder:.+:.+:.+",
-            "Actions": [
-                "CancelImageCreation",
-                "CreateComponent",
-                "CreateContainerRecipe",
-                "CreateDistributionConfiguration",
-                "CreateImage",
-                "CreateImagePipeline",
-                "CreateImageRecipe",
-                "CreateInfrastructureConfiguration",
-                "DeleteComponent",
-                "DeleteContainerRecipe",
-                "DeleteDistributionConfiguration",
-                "DeleteImage",
-                "DeleteImagePipeline",
-                "DeleteImageRecipe",
-                "DeleteInfrastructureConfiguration",
-                "GetComponent",
-                "GetComponentPolicy",
-                "GetContainerRecipe",
-                "GetContainerRecipePolicy",
-                "GetDistributionConfiguration",
-                "GetImage",
-                "GetImagePipeline",
-                "GetImagePolicy",
-                "GetImageRecipe",
-                "GetImageRecipePolicy",
-                "GetInfrastructureConfiguration",
-                "GetWorkflowExecution",
-                "GetWorkflowStepExecution",
-                "ImportComponent",
-                "ImportVmImage",
-                "ListComponentBuildVersions",
-                "ListComponents",
-                "ListContainerRecipes",
-                "ListDistributionConfigurations",
-                "ListImageBuildVersions",
-                "ListImagePackages",
-                "ListImagePipelineImages",
-                "ListImagePipelines",
-                "ListImageRecipes",
-                "ListImageScanFindingAggregations",
-                "ListImageScanFindings",
-                "ListImages",
-                "ListInfrastructureConfigurations",
-                "ListTagsForResource",
-                "ListWorkflowExecutions",
-                "ListWorkflowStepExecutions",
-                "PutComponentPolicy",
-                "PutContainerRecipePolicy",
-                "PutImagePolicy",
-                "PutImageRecipePolicy",
-                "StartImagePipelineExecution",
-                "TagResource",
-                "UntagResource",
-                "UpdateDistributionConfiguration",
-                "UpdateImagePipeline",
-                "UpdateInfrastructureConfiguration"
-            ],
-            "HasResource": true,
-            "StringPrefix": "imagebuilder",
-            "conditionKeys": [
-                "aws:RequestTag/${TagKey}",
-                "aws:ResourceTag/${TagKey}",
-                "aws:TagKeys",
-                "imagebuilder:CreatedResourceTag/<key>",
-                "imagebuilder:CreatedResourceTagKeys",
-                "imagebuilder:Ec2MetadataHttpTokens",
-                "imagebuilder:StatusTopicArn"
-            ]
-        },
-        "Amazon EC2 Instance Connect": {
-            "ARNFormat": "arn:aws:ec2:${Region}:${Account}:${ResourceType}/${ResourcePath}",
-            "ARNRegex": "^arn:aws:ec2:.+",
-            "Actions": [
-                "SendSSHPublicKey",
-                "SendSerialConsoleSSHPublicKey"
-            ],
-            "HasResource": true,
-            "StringPrefix": "ec2-instance-connect",
-            "conditionKeys": [
-                "aws:ResourceTag/${TagKey}",
-                "ec2:ResourceTag/${TagKey}",
-                "ec2:osuser"
-            ]
-        },
-        "Amazon EMR Serverless": {
-            "ARNFormat": "arn:aws:emr-serverless:${Region}:${Account}:/${ResourceType}/${ResourcePath}",
-            "ARNRegex": "^arn:aws:emr-serverless:.+",
-            "Actions": [
-                "CancelJobRun",
-                "CreateApplication",
-                "DeleteApplication",
-                "GetApplication",
-                "GetDashboardForJobRun",
-                "GetJobRun",
-                "ListApplications",
-                "ListJobRuns",
-                "ListTagsForResource",
-                "StartApplication",
-                "StartJobRun",
-                "StopApplication",
-                "TagResource",
-                "UntagResource",
-                "UpdateApplication"
-            ],
-            "HasResource": true,
-            "StringPrefix": "emr-serverless",
-            "conditionKeys": [
-                "aws:RequestTag/${TagKey}",
-                "aws:ResourceTag/${TagKey}",
-                "aws:TagKeys"
-            ]
-        },
-        "Amazon EMR on EKS (EMR Containers)": {
-            "ARNFormat": "arn:aws:emr-containers:${Region}:${Account}:/${ResourceType}/${ResourcePath}",
-            "ARNRegex": "^arn:aws:emr-containers:.+",
-            "Actions": [
-                "CancelJobRun",
-                "CreateJobTemplate",
-                "CreateManagedEndpoint",
-                "CreateVirtualCluster",
-                "DeleteJobTemplate",
-                "DeleteManagedEndpoint",
-                "DeleteVirtualCluster",
-                "DescribeJobRun",
-                "DescribeJobTemplate",
-                "DescribeManagedEndpoint",
-                "DescribeVirtualCluster",
-                "GetManagedEndpointSessionCredentials",
-                "ListJobRuns",
-                "ListJobTemplates",
-                "ListManagedEndpoints",
-                "ListTagsForResource",
-                "ListVirtualClusters",
-                "StartJobRun",
-                "TagResource",
-                "UntagResource"
-            ],
-            "HasResource": true,
-            "StringPrefix": "emr-containers",
-            "conditionKeys": [
-                "aws:RequestTag/${TagKey}",
-                "aws:ResourceTag/${TagKey}",
-                "aws:TagKeys",
-                "emr-containers:ExecutionRoleArn",
-                "emr-containers:JobTemplateArn"
-            ]
-        },
-        "Amazon ElastiCache": {
-            "ARNFormat": "arn:aws:elasticache:${Region}:${Account}:${ResourceType}:${ResourceName}",
-            "ARNRegex": "^arn:aws:elasticache:.+:.+:.+",
-            "Actions": [
-                "AddTagsToResource",
-                "AuthorizeCacheSecurityGroupIngress",
-                "BatchApplyUpdateAction",
-                "BatchStopUpdateAction",
-                "CompleteMigration",
-                "Connect",
-                "CopySnapshot",
-                "CreateCacheCluster",
-                "CreateCacheParameterGroup",
-                "CreateCacheSecurityGroup",
-                "CreateCacheSubnetGroup",
-                "CreateGlobalReplicationGroup",
-                "CreateReplicationGroup",
-                "CreateSnapshot",
-                "CreateUser",
-                "CreateUserGroup",
-                "DecreaseNodeGroupsInGlobalReplicationGroup",
-                "DecreaseReplicaCount",
-                "DeleteCacheCluster",
-                "DeleteCacheParameterGroup",
-                "DeleteCacheSecurityGroup",
-                "DeleteCacheSubnetGroup",
-                "DeleteGlobalReplicationGroup",
-                "DeleteReplicationGroup",
-                "DeleteSnapshot",
-                "DeleteUser",
-                "DeleteUserGroup",
-                "DescribeCacheClusters",
-                "DescribeCacheEngineVersions",
-                "DescribeCacheParameterGroups",
-                "DescribeCacheParameters",
-                "DescribeCacheSecurityGroups",
-                "DescribeCacheSubnetGroups",
-                "DescribeEngineDefaultParameters",
-                "DescribeEvents",
-                "DescribeGlobalReplicationGroups",
-                "DescribeReplicationGroups",
-                "DescribeReservedCacheNodes",
-                "DescribeReservedCacheNodesOfferings",
-                "DescribeServiceUpdates",
-                "DescribeSnapshots",
-                "DescribeUpdateActions",
-                "DescribeUserGroups",
-                "DescribeUsers",
-                "DisassociateGlobalReplicationGroup",
-                "FailoverGlobalReplicationGroup",
-                "IncreaseNodeGroupsInGlobalReplicationGroup",
-                "IncreaseReplicaCount",
-                "ListAllowedNodeTypeModifications",
-                "ListTagsForResource",
-                "ModifyCacheCluster",
-                "ModifyCacheParameterGroup",
-                "ModifyCacheSubnetGroup",
-                "ModifyGlobalReplicationGroup",
-                "ModifyReplicationGroup",
-                "ModifyReplicationGroupShardConfiguration",
-                "ModifyUser",
-                "ModifyUserGroup",
-                "PurchaseReservedCacheNodesOffering",
-                "RebalanceSlotsInGlobalReplicationGroup",
-                "RebootCacheCluster",
-                "RemoveTagsFromResource",
-                "ResetCacheParameterGroup",
-                "RevokeCacheSecurityGroupIngress",
-                "StartMigration",
-                "TestFailover"
-            ],
-            "HasResource": true,
-            "StringPrefix": "elasticache",
-            "conditionKeys": [
-                "aws:RequestTag/${TagKey}",
-                "aws:ResourceTag/${TagKey}",
-                "aws:TagKeys",
-                "elasticache:AtRestEncryptionEnabled",
-                "elasticache:AuthTokenEnabled",
-                "elasticache:AutomaticFailoverEnabled",
-                "elasticache:CacheNodeType",
-                "elasticache:CacheParameterGroupName",
-                "elasticache:ClusterModeEnabled",
-                "elasticache:EngineType",
-                "elasticache:EngineVersion",
-                "elasticache:KmsKeyId",
-                "elasticache:MultiAZEnabled",
-                "elasticache:NumNodeGroups",
-                "elasticache:ReplicasPerNodeGroup",
-                "elasticache:SnapshotRetentionLimit",
-                "elasticache:TransitEncryptionEnabled",
-                "elasticache:UserAuthenticationMode"
-            ]
-        },
-        "Amazon Elastic Block Store": {
-            "ARNFormat": "arn:aws:ebs:${Region}:${Account}:${ResourceType}/${ResourcePath}",
-            "ARNRegex": "^arn:aws:ebs:.+",
-            "Actions": [
-                "CompleteSnapshot",
-                "GetSnapshotBlock",
-                "ListChangedBlocks",
-                "ListSnapshotBlocks",
-                "PutSnapshotBlock",
-                "StartSnapshot"
-            ],
-            "HasResource": true,
-            "StringPrefix": "ebs",
-            "conditionKeys": [
-                "aws:RequestTag/${TagKey}",
-                "aws:ResourceTag/${TagKey}",
-                "aws:TagKeys",
-                "ebs:Description",
-                "ebs:ParentSnapshot",
-                "ebs:VolumeSize"
-            ]
-        },
-        "Amazon Elastic Compute Cloud (EC2)": {
+        "Amazon EC2": {
             "ARNFormat": "arn:aws:ec2:${Region}:${Account}:${ResourceType}/${ResourcePath}",
             "ARNRegex": "^arn:aws:ec2:.+",
             "Actions": [
                 "AcceptAddressTransfer",
                 "AcceptReservedInstancesExchangeQuote",
                 "AcceptTransitGatewayMulticastDomainAssociations",
                 "AcceptTransitGatewayPeeringAttachment",
@@ -13129,14 +12784,375 @@
                 "ec2:VpcID",
                 "ec2:VpcPeeringConnectionID",
                 "ec2:VpceServiceName",
                 "ec2:VpceServiceOwner",
                 "ec2:VpceServicePrivateDnsName"
             ]
         },
+        "Amazon EC2 Auto Scaling": {
+            "ARNFormat": "arn:aws:autoscaling:${Region}:${Account}:${RelativeId}",
+            "ARNRegex": "^arn:aws:autoscaling:.+:.+:.+",
+            "Actions": [
+                "AttachInstances",
+                "AttachLoadBalancerTargetGroups",
+                "AttachLoadBalancers",
+                "AttachTrafficSources",
+                "BatchDeleteScheduledAction",
+                "BatchPutScheduledUpdateGroupAction",
+                "CancelInstanceRefresh",
+                "CompleteLifecycleAction",
+                "CreateAutoScalingGroup",
+                "CreateLaunchConfiguration",
+                "CreateOrUpdateTags",
+                "DeleteAutoScalingGroup",
+                "DeleteLaunchConfiguration",
+                "DeleteLifecycleHook",
+                "DeleteNotificationConfiguration",
+                "DeletePolicy",
+                "DeleteScheduledAction",
+                "DeleteTags",
+                "DeleteWarmPool",
+                "DescribeAccountLimits",
+                "DescribeAdjustmentTypes",
+                "DescribeAutoScalingGroups",
+                "DescribeAutoScalingInstances",
+                "DescribeAutoScalingNotificationTypes",
+                "DescribeInstanceRefreshes",
+                "DescribeLaunchConfigurations",
+                "DescribeLifecycleHookTypes",
+                "DescribeLifecycleHooks",
+                "DescribeLoadBalancerTargetGroups",
+                "DescribeLoadBalancers",
+                "DescribeMetricCollectionTypes",
+                "DescribeNotificationConfigurations",
+                "DescribePolicies",
+                "DescribeScalingActivities",
+                "DescribeScalingProcessTypes",
+                "DescribeScheduledActions",
+                "DescribeTags",
+                "DescribeTerminationPolicyTypes",
+                "DescribeTrafficSources",
+                "DescribeWarmPool",
+                "DetachInstances",
+                "DetachLoadBalancerTargetGroups",
+                "DetachLoadBalancers",
+                "DetachTrafficSources",
+                "DisableMetricsCollection",
+                "EnableMetricsCollection",
+                "EnterStandby",
+                "ExecutePolicy",
+                "ExitStandby",
+                "GetPredictiveScalingForecast",
+                "PutLifecycleHook",
+                "PutNotificationConfiguration",
+                "PutScalingPolicy",
+                "PutScheduledUpdateGroupAction",
+                "PutWarmPool",
+                "RecordLifecycleActionHeartbeat",
+                "ResumeProcesses",
+                "RollbackInstanceRefresh",
+                "SetDesiredCapacity",
+                "SetInstanceHealth",
+                "SetInstanceProtection",
+                "StartInstanceRefresh",
+                "SuspendProcesses",
+                "TerminateInstanceInAutoScalingGroup",
+                "UpdateAutoScalingGroup"
+            ],
+            "HasResource": true,
+            "StringPrefix": "autoscaling",
+            "conditionKeys": [
+                "autoscaling:ImageId",
+                "autoscaling:InstanceType",
+                "autoscaling:InstanceTypes",
+                "autoscaling:LaunchConfigurationName",
+                "autoscaling:LaunchTemplateVersionSpecified",
+                "autoscaling:LoadBalancerNames",
+                "autoscaling:MaxSize",
+                "autoscaling:MetadataHttpEndpoint",
+                "autoscaling:MetadataHttpPutResponseHopLimit",
+                "autoscaling:MetadataHttpTokens",
+                "autoscaling:MinSize",
+                "autoscaling:ResourceTag/${TagKey}",
+                "autoscaling:SpotPrice",
+                "autoscaling:TargetGroupARNs",
+                "autoscaling:TrafficSourceIdentifiers",
+                "autoscaling:VPCZoneIdentifiers",
+                "aws:RequestTag/${TagKey}",
+                "aws:ResourceTag/${TagKey}",
+                "aws:TagKeys"
+            ]
+        },
+        "Amazon EC2 Image Builder": {
+            "ARNFormat": "arn:aws:imagebuilder:${Region}:${Account}:${ResourceType}/${ResourceName}",
+            "ARNRegex": "^arn:aws:imagebuilder:.+:.+:.+",
+            "Actions": [
+                "CancelImageCreation",
+                "CreateComponent",
+                "CreateContainerRecipe",
+                "CreateDistributionConfiguration",
+                "CreateImage",
+                "CreateImagePipeline",
+                "CreateImageRecipe",
+                "CreateInfrastructureConfiguration",
+                "DeleteComponent",
+                "DeleteContainerRecipe",
+                "DeleteDistributionConfiguration",
+                "DeleteImage",
+                "DeleteImagePipeline",
+                "DeleteImageRecipe",
+                "DeleteInfrastructureConfiguration",
+                "GetComponent",
+                "GetComponentPolicy",
+                "GetContainerRecipe",
+                "GetContainerRecipePolicy",
+                "GetDistributionConfiguration",
+                "GetImage",
+                "GetImagePipeline",
+                "GetImagePolicy",
+                "GetImageRecipe",
+                "GetImageRecipePolicy",
+                "GetInfrastructureConfiguration",
+                "GetWorkflowExecution",
+                "GetWorkflowStepExecution",
+                "ImportComponent",
+                "ImportVmImage",
+                "ListComponentBuildVersions",
+                "ListComponents",
+                "ListContainerRecipes",
+                "ListDistributionConfigurations",
+                "ListImageBuildVersions",
+                "ListImagePackages",
+                "ListImagePipelineImages",
+                "ListImagePipelines",
+                "ListImageRecipes",
+                "ListImageScanFindingAggregations",
+                "ListImageScanFindings",
+                "ListImages",
+                "ListInfrastructureConfigurations",
+                "ListTagsForResource",
+                "ListWorkflowExecutions",
+                "ListWorkflowStepExecutions",
+                "PutComponentPolicy",
+                "PutContainerRecipePolicy",
+                "PutImagePolicy",
+                "PutImageRecipePolicy",
+                "StartImagePipelineExecution",
+                "TagResource",
+                "UntagResource",
+                "UpdateDistributionConfiguration",
+                "UpdateImagePipeline",
+                "UpdateInfrastructureConfiguration"
+            ],
+            "HasResource": true,
+            "StringPrefix": "imagebuilder",
+            "conditionKeys": [
+                "aws:RequestTag/${TagKey}",
+                "aws:ResourceTag/${TagKey}",
+                "aws:TagKeys",
+                "imagebuilder:CreatedResourceTag/<key>",
+                "imagebuilder:CreatedResourceTagKeys",
+                "imagebuilder:Ec2MetadataHttpTokens",
+                "imagebuilder:StatusTopicArn"
+            ]
+        },
+        "Amazon EC2 Instance Connect": {
+            "ARNFormat": "arn:aws:ec2:${Region}:${Account}:${ResourceType}/${ResourcePath}",
+            "ARNRegex": "^arn:aws:ec2:.+",
+            "Actions": [
+                "SendSSHPublicKey",
+                "SendSerialConsoleSSHPublicKey"
+            ],
+            "HasResource": true,
+            "StringPrefix": "ec2-instance-connect",
+            "conditionKeys": [
+                "aws:ResourceTag/${TagKey}",
+                "ec2:ResourceTag/${TagKey}",
+                "ec2:osuser"
+            ]
+        },
+        "Amazon EMR Serverless": {
+            "ARNFormat": "arn:aws:emr-serverless:${Region}:${Account}:/${ResourceType}/${ResourcePath}",
+            "ARNRegex": "^arn:aws:emr-serverless:.+",
+            "Actions": [
+                "CancelJobRun",
+                "CreateApplication",
+                "DeleteApplication",
+                "GetApplication",
+                "GetDashboardForJobRun",
+                "GetJobRun",
+                "ListApplications",
+                "ListJobRuns",
+                "ListTagsForResource",
+                "StartApplication",
+                "StartJobRun",
+                "StopApplication",
+                "TagResource",
+                "UntagResource",
+                "UpdateApplication"
+            ],
+            "HasResource": true,
+            "StringPrefix": "emr-serverless",
+            "conditionKeys": [
+                "aws:RequestTag/${TagKey}",
+                "aws:ResourceTag/${TagKey}",
+                "aws:TagKeys"
+            ]
+        },
+        "Amazon EMR on EKS (EMR Containers)": {
+            "ARNFormat": "arn:aws:emr-containers:${Region}:${Account}:/${ResourceType}/${ResourcePath}",
+            "ARNRegex": "^arn:aws:emr-containers:.+",
+            "Actions": [
+                "CancelJobRun",
+                "CreateJobTemplate",
+                "CreateManagedEndpoint",
+                "CreateVirtualCluster",
+                "DeleteJobTemplate",
+                "DeleteManagedEndpoint",
+                "DeleteVirtualCluster",
+                "DescribeJobRun",
+                "DescribeJobTemplate",
+                "DescribeManagedEndpoint",
+                "DescribeVirtualCluster",
+                "GetManagedEndpointSessionCredentials",
+                "ListJobRuns",
+                "ListJobTemplates",
+                "ListManagedEndpoints",
+                "ListTagsForResource",
+                "ListVirtualClusters",
+                "StartJobRun",
+                "TagResource",
+                "UntagResource"
+            ],
+            "HasResource": true,
+            "StringPrefix": "emr-containers",
+            "conditionKeys": [
+                "aws:RequestTag/${TagKey}",
+                "aws:ResourceTag/${TagKey}",
+                "aws:TagKeys",
+                "emr-containers:ExecutionRoleArn",
+                "emr-containers:JobTemplateArn"
+            ]
+        },
+        "Amazon ElastiCache": {
+            "ARNFormat": "arn:aws:elasticache:${Region}:${Account}:${ResourceType}:${ResourceName}",
+            "ARNRegex": "^arn:aws:elasticache:.+:.+:.+",
+            "Actions": [
+                "AddTagsToResource",
+                "AuthorizeCacheSecurityGroupIngress",
+                "BatchApplyUpdateAction",
+                "BatchStopUpdateAction",
+                "CompleteMigration",
+                "Connect",
+                "CopySnapshot",
+                "CreateCacheCluster",
+                "CreateCacheParameterGroup",
+                "CreateCacheSecurityGroup",
+                "CreateCacheSubnetGroup",
+                "CreateGlobalReplicationGroup",
+                "CreateReplicationGroup",
+                "CreateSnapshot",
+                "CreateUser",
+                "CreateUserGroup",
+                "DecreaseNodeGroupsInGlobalReplicationGroup",
+                "DecreaseReplicaCount",
+                "DeleteCacheCluster",
+                "DeleteCacheParameterGroup",
+                "DeleteCacheSecurityGroup",
+                "DeleteCacheSubnetGroup",
+                "DeleteGlobalReplicationGroup",
+                "DeleteReplicationGroup",
+                "DeleteSnapshot",
+                "DeleteUser",
+                "DeleteUserGroup",
+                "DescribeCacheClusters",
+                "DescribeCacheEngineVersions",
+                "DescribeCacheParameterGroups",
+                "DescribeCacheParameters",
+                "DescribeCacheSecurityGroups",
+                "DescribeCacheSubnetGroups",
+                "DescribeEngineDefaultParameters",
+                "DescribeEvents",
+                "DescribeGlobalReplicationGroups",
+                "DescribeReplicationGroups",
+                "DescribeReservedCacheNodes",
+                "DescribeReservedCacheNodesOfferings",
+                "DescribeServiceUpdates",
+                "DescribeSnapshots",
+                "DescribeUpdateActions",
+                "DescribeUserGroups",
+                "DescribeUsers",
+                "DisassociateGlobalReplicationGroup",
+                "FailoverGlobalReplicationGroup",
+                "IncreaseNodeGroupsInGlobalReplicationGroup",
+                "IncreaseReplicaCount",
+                "ListAllowedNodeTypeModifications",
+                "ListTagsForResource",
+                "ModifyCacheCluster",
+                "ModifyCacheParameterGroup",
+                "ModifyCacheSubnetGroup",
+                "ModifyGlobalReplicationGroup",
+                "ModifyReplicationGroup",
+                "ModifyReplicationGroupShardConfiguration",
+                "ModifyUser",
+                "ModifyUserGroup",
+                "PurchaseReservedCacheNodesOffering",
+                "RebalanceSlotsInGlobalReplicationGroup",
+                "RebootCacheCluster",
+                "RemoveTagsFromResource",
+                "ResetCacheParameterGroup",
+                "RevokeCacheSecurityGroupIngress",
+                "StartMigration",
+                "TestFailover"
+            ],
+            "HasResource": true,
+            "StringPrefix": "elasticache",
+            "conditionKeys": [
+                "aws:RequestTag/${TagKey}",
+                "aws:ResourceTag/${TagKey}",
+                "aws:TagKeys",
+                "elasticache:AtRestEncryptionEnabled",
+                "elasticache:AuthTokenEnabled",
+                "elasticache:AutomaticFailoverEnabled",
+                "elasticache:CacheNodeType",
+                "elasticache:CacheParameterGroupName",
+                "elasticache:ClusterModeEnabled",
+                "elasticache:EngineType",
+                "elasticache:EngineVersion",
+                "elasticache:KmsKeyId",
+                "elasticache:MultiAZEnabled",
+                "elasticache:NumNodeGroups",
+                "elasticache:ReplicasPerNodeGroup",
+                "elasticache:SnapshotRetentionLimit",
+                "elasticache:TransitEncryptionEnabled",
+                "elasticache:UserAuthenticationMode"
+            ]
+        },
+        "Amazon Elastic Block Store": {
+            "ARNFormat": "arn:aws:ebs:${Region}:${Account}:${ResourceType}/${ResourcePath}",
+            "ARNRegex": "^arn:aws:ebs:.+",
+            "Actions": [
+                "CompleteSnapshot",
+                "GetSnapshotBlock",
+                "ListChangedBlocks",
+                "ListSnapshotBlocks",
+                "PutSnapshotBlock",
+                "StartSnapshot"
+            ],
+            "HasResource": true,
+            "StringPrefix": "ebs",
+            "conditionKeys": [
+                "aws:RequestTag/${TagKey}",
+                "aws:ResourceTag/${TagKey}",
+                "aws:TagKeys",
+                "ebs:Description",
+                "ebs:ParentSnapshot",
+                "ebs:VolumeSize"
+            ]
+        },
         "Amazon Elastic Container Registry": {
             "ARNFormat": "arn:aws:ecr:${Region}:${Account}:repository/${RepositoryName}",
             "ARNRegex": "^arn:aws:ecr:.+",
             "Actions": [
                 "BatchCheckLayerAvailability",
                 "BatchDeleteImage",
                 "BatchGetImage",
@@ -13784,28 +13800,56 @@
                 "fsx:StorageVirtualMachineId"
             ]
         },
         "Amazon FinSpace": {
             "ARNFormat": "arn:aws:finspace:${Region}:${Account}:${ResourceType}/${ResourcePath}",
             "ARNRegex": "^arn:aws:finspace:.+",
             "Actions": [
+                "ConnectKxCluster",
                 "CreateEnvironment",
+                "CreateKxChangeset",
+                "CreateKxCluster",
+                "CreateKxDatabase",
+                "CreateKxEnvironment",
+                "CreateKxUser",
                 "CreateUser",
                 "DeleteEnvironment",
+                "DeleteKxCluster",
+                "DeleteKxDatabase",
+                "DeleteKxEnvironment",
+                "DeleteKxUser",
                 "GetEnvironment",
+                "GetKxChangeset",
+                "GetKxCluster",
+                "GetKxConnectionString",
+                "GetKxDatabase",
+                "GetKxEnvironment",
+                "GetKxUser",
                 "GetLoadSampleDataSetGroupIntoEnvironmentStatus",
                 "GetUser",
                 "ListEnvironments",
+                "ListKxChangesets",
+                "ListKxClusterNodes",
+                "ListKxClusters",
+                "ListKxDatabases",
+                "ListKxEnvironments",
+                "ListKxUsers",
                 "ListTagsForResource",
                 "ListUsers",
                 "LoadSampleDataSetGroupIntoEnvironment",
+                "MountKxDatabase",
                 "ResetUserPassword",
                 "TagResource",
                 "UntagResource",
                 "UpdateEnvironment",
+                "UpdateKxClusterDatabases",
+                "UpdateKxDatabase",
+                "UpdateKxEnvironment",
+                "UpdateKxEnvironmentNetwork",
+                "UpdateKxUser",
                 "UpdateUser"
             ],
             "HasResource": true,
             "StringPrefix": "finspace",
             "conditionKeys": [
                 "aws:RequestTag/${TagKey}",
                 "aws:ResourceTag/${TagKey}",
```

### Comparing `iam_actions-1.2.20230606/iam_actions/resourcetypes.json` & `iam_actions-1.2.20230607/iam_actions/resourcetypes.json`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9986111111111111%*

 * *Differences: {"'ec2'": "{replace: OrderedDict([('elastic-ip', OrderedDict([('arn_pattern', "*

 * *          "'arn:*:ec2:*:*:elastic-ip/*'), ('condition_keys', 'aws:RequestTag/${TagKey}')])), "*

 * *          "('capacity-reservation-fleet', OrderedDict([('arn_pattern', "*

 * *          "'arn:*:ec2:*:*:capacity-reservation-fleet/*'), ('condition_keys', "*

 * *          "'aws:RequestTag/${TagKey}')])), ('capacity-reservation', OrderedDict([('arn_pattern', "*

 * *          "'arn:*:ec2:*:*:capacity-reservation/*'), ('condition_keys', "*

 * *          "'a […]*

```diff
@@ -1891,15 +1891,368 @@
     },
     "ebs": {
         "snapshot": {
             "arn_pattern": "arn:*:ec2:*::snapshot/*",
             "condition_keys": "aws:RequestTag/${TagKey}"
         }
     },
-    "ec2": {},
+    "ec2": {
+        "capacity-reservation": {
+            "arn_pattern": "arn:*:ec2:*:*:capacity-reservation/*",
+            "condition_keys": "aws:RequestTag/${TagKey}"
+        },
+        "capacity-reservation-fleet": {
+            "arn_pattern": "arn:*:ec2:*:*:capacity-reservation-fleet/*",
+            "condition_keys": "aws:RequestTag/${TagKey}"
+        },
+        "carrier-gateway": {
+            "arn_pattern": "arn:*:ec2:*:*:carrier-gateway/*",
+            "condition_keys": "aws:RequestTag/${TagKey}"
+        },
+        "certificate": {
+            "arn_pattern": "arn:*:acm:*:*:certificate/*",
+            "condition_keys": null
+        },
+        "client-vpn-endpoint": {
+            "arn_pattern": "arn:*:ec2:*:*:client-vpn-endpoint/*",
+            "condition_keys": "aws:RequestTag/${TagKey}"
+        },
+        "coip-pool": {
+            "arn_pattern": "arn:*:ec2:*:*:coip-pool/*",
+            "condition_keys": "aws:RequestTag/${TagKey}"
+        },
+        "customer-gateway": {
+            "arn_pattern": "arn:*:ec2:*:*:customer-gateway/*",
+            "condition_keys": "aws:RequestTag/${TagKey}"
+        },
+        "dedicated-host": {
+            "arn_pattern": "arn:*:ec2:*:*:dedicated-host/*",
+            "condition_keys": "aws:RequestTag/${TagKey}"
+        },
+        "dhcp-options": {
+            "arn_pattern": "arn:*:ec2:*:*:dhcp-options/*",
+            "condition_keys": "aws:RequestTag/${TagKey}"
+        },
+        "egress-only-internet-gateway": {
+            "arn_pattern": "arn:*:ec2:*:*:egress-only-internet-gateway/*",
+            "condition_keys": "aws:RequestTag/${TagKey}"
+        },
+        "elastic-gpu": {
+            "arn_pattern": "arn:*:ec2:*:*:elastic-gpu/*",
+            "condition_keys": "aws:RequestTag/${TagKey}"
+        },
+        "elastic-inference": {
+            "arn_pattern": "arn:*:elastic-inference:*:*:elastic-inference-accelerator/*",
+            "condition_keys": null
+        },
+        "elastic-ip": {
+            "arn_pattern": "arn:*:ec2:*:*:elastic-ip/*",
+            "condition_keys": "aws:RequestTag/${TagKey}"
+        },
+        "export-image-task": {
+            "arn_pattern": "arn:*:ec2:*:*:export-image-task/*",
+            "condition_keys": "aws:RequestTag/${TagKey}"
+        },
+        "export-instance-task": {
+            "arn_pattern": "arn:*:ec2:*:*:export-instance-task/*",
+            "condition_keys": "aws:RequestTag/${TagKey}"
+        },
+        "fleet": {
+            "arn_pattern": "arn:*:ec2:*:*:fleet/*",
+            "condition_keys": "aws:RequestTag/${TagKey}"
+        },
+        "fpga-image": {
+            "arn_pattern": "arn:*:ec2:*:*:fpga-image/*",
+            "condition_keys": "aws:RequestTag/${TagKey}"
+        },
+        "group": {
+            "arn_pattern": "arn:*:resource-groups:*:*:group/*",
+            "condition_keys": null
+        },
+        "host-reservation": {
+            "arn_pattern": "arn:*:ec2:*:*:host-reservation/*",
+            "condition_keys": "aws:RequestTag/${TagKey}"
+        },
+        "image": {
+            "arn_pattern": "arn:*:ec2:*::image/*",
+            "condition_keys": "aws:RequestTag/${TagKey}"
+        },
+        "import-image-task": {
+            "arn_pattern": "arn:*:ec2:*:*:import-image-task/*",
+            "condition_keys": "aws:RequestTag/${TagKey}"
+        },
+        "import-snapshot-task": {
+            "arn_pattern": "arn:*:ec2:*:*:import-snapshot-task/*",
+            "condition_keys": "aws:RequestTag/${TagKey}"
+        },
+        "instance": {
+            "arn_pattern": "arn:*:ec2:*:*:instance/*",
+            "condition_keys": "aws:RequestTag/${TagKey}"
+        },
+        "instance-event-window": {
+            "arn_pattern": "arn:*:ec2:*:*:instance-event-window/*",
+            "condition_keys": "aws:RequestTag/${TagKey}"
+        },
+        "internet-gateway": {
+            "arn_pattern": "arn:*:ec2:*:*:internet-gateway/*",
+            "condition_keys": "aws:RequestTag/${TagKey}"
+        },
+        "ipam": {
+            "arn_pattern": "arn:*:ec2::*:ipam/*",
+            "condition_keys": "aws:RequestTag/${TagKey}"
+        },
+        "ipam-pool": {
+            "arn_pattern": "arn:*:ec2::*:ipam-pool/*",
+            "condition_keys": "aws:RequestTag/${TagKey}"
+        },
+        "ipam-resource-discovery": {
+            "arn_pattern": "arn:*:ec2::*:ipam-resource-discovery/*",
+            "condition_keys": "aws:RequestTag/${TagKey}"
+        },
+        "ipam-resource-discovery-association": {
+            "arn_pattern": "arn:*:ec2::*:ipam-resource-discovery-association/*",
+            "condition_keys": "aws:RequestTag/${TagKey}"
+        },
+        "ipam-scope": {
+            "arn_pattern": "arn:*:ec2::*:ipam-scope/*",
+            "condition_keys": "aws:RequestTag/${TagKey}"
+        },
+        "ipv4pool-ec2": {
+            "arn_pattern": "arn:*:ec2:*:*:ipv4pool-ec2/*",
+            "condition_keys": "aws:RequestTag/${TagKey}"
+        },
+        "ipv6pool-ec2": {
+            "arn_pattern": "arn:*:ec2:*:*:ipv6pool-ec2/*",
+            "condition_keys": "aws:RequestTag/${TagKey}"
+        },
+        "key-pair": {
+            "arn_pattern": "arn:*:ec2:*:*:key-pair/*",
+            "condition_keys": "aws:RequestTag/${TagKey}"
+        },
+        "launch-template": {
+            "arn_pattern": "arn:*:ec2:*:*:launch-template/*",
+            "condition_keys": "aws:RequestTag/${TagKey}"
+        },
+        "license-configuration": {
+            "arn_pattern": "arn:*:license-manager:*:*:license-configuration:*",
+            "condition_keys": null
+        },
+        "local-gateway": {
+            "arn_pattern": "arn:*:ec2:*:*:local-gateway/*",
+            "condition_keys": "aws:RequestTag/${TagKey}"
+        },
+        "local-gateway-route-table": {
+            "arn_pattern": "arn:*:ec2:*:*:local-gateway-route-table/*",
+            "condition_keys": "aws:RequestTag/${TagKey}"
+        },
+        "local-gateway-route-table-virtual-interface-group-association": {
+            "arn_pattern": "arn:*:ec2:*:*:local-gateway-route-table-virtual-interface-group-association/*",
+            "condition_keys": "aws:RequestTag/${TagKey}"
+        },
+        "local-gateway-route-table-vpc-association": {
+            "arn_pattern": "arn:*:ec2:*:*:local-gateway-route-table-vpc-association/*",
+            "condition_keys": "aws:RequestTag/${TagKey}"
+        },
+        "local-gateway-virtual-interface": {
+            "arn_pattern": "arn:*:ec2:*:*:local-gateway-virtual-interface/*",
+            "condition_keys": "aws:RequestTag/${TagKey}"
+        },
+        "local-gateway-virtual-interface-group": {
+            "arn_pattern": "arn:*:ec2:*:*:local-gateway-virtual-interface-group/*",
+            "condition_keys": "aws:RequestTag/${TagKey}"
+        },
+        "natgateway": {
+            "arn_pattern": "arn:*:ec2:*:*:natgateway/*",
+            "condition_keys": "aws:RequestTag/${TagKey}"
+        },
+        "network-acl": {
+            "arn_pattern": "arn:*:ec2:*:*:network-acl/*",
+            "condition_keys": "aws:RequestTag/${TagKey}"
+        },
+        "network-insights-access-scope": {
+            "arn_pattern": "arn:*:ec2:*:*:network-insights-access-scope/*",
+            "condition_keys": "aws:RequestTag/${TagKey}"
+        },
+        "network-insights-access-scope-analysis": {
+            "arn_pattern": "arn:*:ec2:*:*:network-insights-access-scope-analysis/*",
+            "condition_keys": "aws:RequestTag/${TagKey}"
+        },
+        "network-insights-analysis": {
+            "arn_pattern": "arn:*:ec2:*:*:network-insights-analysis/*",
+            "condition_keys": "aws:RequestTag/${TagKey}"
+        },
+        "network-insights-path": {
+            "arn_pattern": "arn:*:ec2:*:*:network-insights-path/*",
+            "condition_keys": "aws:RequestTag/${TagKey}"
+        },
+        "network-interface": {
+            "arn_pattern": "arn:*:ec2:*:*:network-interface/*",
+            "condition_keys": "aws:RequestTag/${TagKey}"
+        },
+        "placement-group": {
+            "arn_pattern": "arn:*:ec2:*:*:placement-group/*",
+            "condition_keys": "aws:RequestTag/${TagKey}"
+        },
+        "prefix-list": {
+            "arn_pattern": "arn:*:ec2:*:*:prefix-list/*",
+            "condition_keys": "aws:RequestTag/${TagKey}"
+        },
+        "replace-root-volume-task": {
+            "arn_pattern": "arn:*:ec2:*:*:replace-root-volume-task/*",
+            "condition_keys": "aws:RequestTag/${TagKey}"
+        },
+        "reserved-instances": {
+            "arn_pattern": "arn:*:ec2:*:*:reserved-instances/*",
+            "condition_keys": "aws:RequestTag/${TagKey}"
+        },
+        "role": {
+            "arn_pattern": "arn:*:iam::*:role/*",
+            "condition_keys": null
+        },
+        "route-table": {
+            "arn_pattern": "arn:*:ec2:*:*:route-table/*",
+            "condition_keys": "aws:RequestTag/${TagKey}"
+        },
+        "security-group": {
+            "arn_pattern": "arn:*:ec2:*:*:security-group/*",
+            "condition_keys": "aws:RequestTag/${TagKey}"
+        },
+        "security-group-rule": {
+            "arn_pattern": "arn:*:ec2:*:*:security-group-rule/*",
+            "condition_keys": "aws:RequestTag/${TagKey}"
+        },
+        "snapshot": {
+            "arn_pattern": "arn:*:ec2:*::snapshot/*",
+            "condition_keys": "aws:RequestTag/${TagKey}"
+        },
+        "spot-fleet-request": {
+            "arn_pattern": "arn:*:ec2:*:*:spot-fleet-request/*",
+            "condition_keys": "aws:RequestTag/${TagKey}"
+        },
+        "spot-instances-request": {
+            "arn_pattern": "arn:*:ec2:*:*:spot-instances-request/*",
+            "condition_keys": "aws:RequestTag/${TagKey}"
+        },
+        "subnet": {
+            "arn_pattern": "arn:*:ec2:*:*:subnet/*",
+            "condition_keys": "aws:RequestTag/${TagKey}"
+        },
+        "subnet-cidr-reservation": {
+            "arn_pattern": "arn:*:ec2:*:*:subnet-cidr-reservation/*",
+            "condition_keys": "aws:RequestTag/${TagKey}"
+        },
+        "traffic-mirror-filter": {
+            "arn_pattern": "arn:*:ec2:*:*:traffic-mirror-filter/*",
+            "condition_keys": "aws:RequestTag/${TagKey}"
+        },
+        "traffic-mirror-filter-rule": {
+            "arn_pattern": "arn:*:ec2:*:*:traffic-mirror-filter-rule/*",
+            "condition_keys": "ec2:Attribute"
+        },
+        "traffic-mirror-session": {
+            "arn_pattern": "arn:*:ec2:*:*:traffic-mirror-session/*",
+            "condition_keys": "aws:RequestTag/${TagKey}"
+        },
+        "traffic-mirror-target": {
+            "arn_pattern": "arn:*:ec2:*:*:traffic-mirror-target/*",
+            "condition_keys": "aws:RequestTag/${TagKey}"
+        },
+        "transit-gateway": {
+            "arn_pattern": "arn:*:ec2:*:*:transit-gateway/*",
+            "condition_keys": "aws:RequestTag/${TagKey}"
+        },
+        "transit-gateway-attachment": {
+            "arn_pattern": "arn:*:ec2:*:*:transit-gateway-attachment/*",
+            "condition_keys": "aws:RequestTag/${TagKey}"
+        },
+        "transit-gateway-connect-peer": {
+            "arn_pattern": "arn:*:ec2:*:*:transit-gateway-connect-peer/*",
+            "condition_keys": "aws:RequestTag/${TagKey}"
+        },
+        "transit-gateway-multicast-domain": {
+            "arn_pattern": "arn:*:ec2:*:*:transit-gateway-multicast-domain/*",
+            "condition_keys": "aws:RequestTag/${TagKey}"
+        },
+        "transit-gateway-policy-table": {
+            "arn_pattern": "arn:*:ec2:*:*:transit-gateway-policy-table/*",
+            "condition_keys": "aws:RequestTag/${TagKey}"
+        },
+        "transit-gateway-route-table": {
+            "arn_pattern": "arn:*:ec2:*:*:transit-gateway-route-table/*",
+            "condition_keys": "aws:RequestTag/${TagKey}"
+        },
+        "transit-gateway-route-table-announcement": {
+            "arn_pattern": "arn:*:ec2:*:*:transit-gateway-route-table-announcement/*",
+            "condition_keys": "aws:RequestTag/${TagKey}"
+        },
+        "verified-access-endpoint": {
+            "arn_pattern": "arn:*:ec2:*:*:verified-access-endpoint/*",
+            "condition_keys": "aws:RequestTag/${TagKey}"
+        },
+        "verified-access-group": {
+            "arn_pattern": "arn:*:ec2:*:*:verified-access-group/*",
+            "condition_keys": "aws:RequestTag/${TagKey}"
+        },
+        "verified-access-instance": {
+            "arn_pattern": "arn:*:ec2:*:*:verified-access-instance/*",
+            "condition_keys": "aws:RequestTag/${TagKey}"
+        },
+        "verified-access-policy": {
+            "arn_pattern": "arn:*:ec2:*:*:verified-access-policy/*",
+            "condition_keys": "aws:RequestTag/${TagKey}"
+        },
+        "verified-access-trust-provider": {
+            "arn_pattern": "arn:*:ec2:*:*:verified-access-trust-provider/*",
+            "condition_keys": "aws:RequestTag/${TagKey}"
+        },
+        "volume": {
+            "arn_pattern": "arn:*:ec2:*:*:volume/*",
+            "condition_keys": "aws:RequestTag/${TagKey}"
+        },
+        "vpc": {
+            "arn_pattern": "arn:*:ec2:*:*:vpc/*",
+            "condition_keys": "aws:RequestTag/${TagKey}"
+        },
+        "vpc-endpoint": {
+            "arn_pattern": "arn:*:ec2:*:*:vpc-endpoint/*",
+            "condition_keys": "aws:RequestTag/${TagKey}"
+        },
+        "vpc-endpoint-connection": {
+            "arn_pattern": "arn:*:ec2:*:*:vpc-endpoint-connection/*",
+            "condition_keys": "aws:RequestTag/${TagKey}"
+        },
+        "vpc-endpoint-service": {
+            "arn_pattern": "arn:*:ec2:*:*:vpc-endpoint-service/*",
+            "condition_keys": "aws:RequestTag/${TagKey}"
+        },
+        "vpc-endpoint-service-permission": {
+            "arn_pattern": "arn:*:ec2:*:*:vpc-endpoint-service-permission/*",
+            "condition_keys": "aws:RequestTag/${TagKey}"
+        },
+        "vpc-flow-log": {
+            "arn_pattern": "arn:*:ec2:*:*:vpc-flow-log/*",
+            "condition_keys": "aws:RequestTag/${TagKey}"
+        },
+        "vpc-peering-connection": {
+            "arn_pattern": "arn:*:ec2:*:*:vpc-peering-connection/*",
+            "condition_keys": "aws:RequestTag/${TagKey}"
+        },
+        "vpn-connection": {
+            "arn_pattern": "arn:*:ec2:*:*:vpn-connection/*",
+            "condition_keys": "aws:RequestTag/${TagKey}"
+        },
+        "vpn-connection-device-type": {
+            "arn_pattern": "arn:*:ec2:*:*:vpn-connection-device-type/*",
+            "condition_keys": "ec2:Region"
+        },
+        "vpn-gateway": {
+            "arn_pattern": "arn:*:ec2:*:*:vpn-gateway/*",
+            "condition_keys": "aws:RequestTag/${TagKey}"
+        }
+    },
     "ec2-instance-connect": {
         "instance": {
             "arn_pattern": "arn:*:ec2:*:*:instance/*",
             "condition_keys": "aws:ResourceTag/${TagKey}"
         }
     },
     "ec2messages": {},
```

### Comparing `iam_actions-1.2.20230606/iam_actions/services.json` & `iam_actions-1.2.20230607/iam_actions/services.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.999787427494231%*

 * *Differences: {"'ec2'": "{'ServiceNames': ['Amazon EC2']}",*

 * * "'finspace'": "{'Actions': {insert: [(0, 'ConnectKxCluster'), (2, 'CreateKxChangeset'), (3, "*

 * *               "'CreateKxCluster'), (4, 'CreateKxDatabase'), (5, 'CreateKxEnvironment'), (6, "*

 * *               "'CreateKxUser'), (9, 'DeleteKxCluster'), (10, 'DeleteKxDatabase'), (11, "*

 * *               "'DeleteKxEnvironment'), (12, 'DeleteKxUser'), (14, 'GetKxChangeset'), (15, "*

 * *               "'GetKxCluster'), (16, 'GetKxConnectionString'), (17, 'GetKxDatabase'), (18, " […]*

```diff
@@ -7012,15 +7012,15 @@
             "ec2:VpcPeeringConnectionID",
             "ec2:VpceServiceName",
             "ec2:VpceServiceOwner",
             "ec2:VpceServicePrivateDnsName"
         ],
         "HasResource": true,
         "ServiceNames": [
-            "Amazon Elastic Compute Cloud (EC2)"
+            "Amazon EC2"
         ]
     },
     "ec2-instance-connect": {
         "ARNFormats": [
             "arn:aws:ec2:${Region}:${Account}:${ResourceType}/${ResourcePath}"
         ],
         "ARNRegexes": [
@@ -8226,28 +8226,56 @@
         "ARNFormats": [
             "arn:aws:finspace:${Region}:${Account}:${ResourceType}/${ResourcePath}"
         ],
         "ARNRegexes": [
             "^arn:aws:finspace:.+"
         ],
         "Actions": [
+            "ConnectKxCluster",
             "CreateEnvironment",
+            "CreateKxChangeset",
+            "CreateKxCluster",
+            "CreateKxDatabase",
+            "CreateKxEnvironment",
+            "CreateKxUser",
             "CreateUser",
             "DeleteEnvironment",
+            "DeleteKxCluster",
+            "DeleteKxDatabase",
+            "DeleteKxEnvironment",
+            "DeleteKxUser",
             "GetEnvironment",
+            "GetKxChangeset",
+            "GetKxCluster",
+            "GetKxConnectionString",
+            "GetKxDatabase",
+            "GetKxEnvironment",
+            "GetKxUser",
             "GetLoadSampleDataSetGroupIntoEnvironmentStatus",
             "GetUser",
             "ListEnvironments",
+            "ListKxChangesets",
+            "ListKxClusterNodes",
+            "ListKxClusters",
+            "ListKxDatabases",
+            "ListKxEnvironments",
+            "ListKxUsers",
             "ListTagsForResource",
             "ListUsers",
             "LoadSampleDataSetGroupIntoEnvironment",
+            "MountKxDatabase",
             "ResetUserPassword",
             "TagResource",
             "UntagResource",
             "UpdateEnvironment",
+            "UpdateKxClusterDatabases",
+            "UpdateKxDatabase",
+            "UpdateKxEnvironment",
+            "UpdateKxEnvironmentNetwork",
+            "UpdateKxUser",
             "UpdateUser"
         ],
         "ConditionKeys": [
             "aws:RequestTag/${TagKey}",
             "aws:ResourceTag/${TagKey}",
             "aws:TagKeys"
         ],
@@ -10334,14 +10362,16 @@
             "CreateDynamicThingGroup",
             "CreateFleetMetric",
             "CreateJob",
             "CreateJobTemplate",
             "CreateKeysAndCertificate",
             "CreateMitigationAction",
             "CreateOTAUpdate",
+            "CreatePackage",
+            "CreatePackageVersion",
             "CreatePolicy",
             "CreatePolicyVersion",
             "CreateProvisioningClaim",
             "CreateProvisioningTemplate",
             "CreateProvisioningTemplateVersion",
             "CreateRoleAlias",
             "CreateScheduledAudit",
@@ -10364,14 +10394,16 @@
             "DeleteDynamicThingGroup",
             "DeleteFleetMetric",
             "DeleteJob",
             "DeleteJobExecution",
             "DeleteJobTemplate",
             "DeleteMitigationAction",
             "DeleteOTAUpdate",
+            "DeletePackage",
+            "DeletePackageVersion",
             "DeletePolicy",
             "DeletePolicyVersion",
             "DeleteProvisioningTemplate",
             "DeleteProvisioningTemplateVersion",
             "DeleteRegistrationCode",
             "DeleteRoleAlias",
             "DeleteScheduledAudit",
@@ -10429,14 +10461,17 @@
             "GetBucketsAggregation",
             "GetCardinality",
             "GetEffectivePolicies",
             "GetIndexingConfiguration",
             "GetJobDocument",
             "GetLoggingOptions",
             "GetOTAUpdate",
+            "GetPackage",
+            "GetPackageConfiguration",
+            "GetPackageVersion",
             "GetPercentiles",
             "GetPolicy",
             "GetPolicyVersion",
             "GetRegistrationCode",
             "GetRetainedMessage",
             "GetStatistics",
             "GetThingShadow",
@@ -10468,14 +10503,16 @@
             "ListJobs",
             "ListManagedJobTemplates",
             "ListMetricValues",
             "ListMitigationActions",
             "ListNamedShadowsForThing",
             "ListOTAUpdates",
             "ListOutgoingCertificates",
+            "ListPackageVersions",
+            "ListPackages",
             "ListPolicies",
             "ListPolicyPrincipals",
             "ListPolicyVersions",
             "ListPrincipalPolicies",
             "ListPrincipalThings",
             "ListProvisioningTemplateVersions",
             "ListProvisioningTemplates",
@@ -10545,14 +10582,17 @@
             "UpdateDomainConfiguration",
             "UpdateDynamicThingGroup",
             "UpdateEventConfigurations",
             "UpdateFleetMetric",
             "UpdateIndexingConfiguration",
             "UpdateJob",
             "UpdateMitigationAction",
+            "UpdatePackage",
+            "UpdatePackageConfiguration",
+            "UpdatePackageVersion",
             "UpdateProvisioningTemplate",
             "UpdateRoleAlias",
             "UpdateScheduledAudit",
             "UpdateSecurityProfile",
             "UpdateStream",
             "UpdateThing",
             "UpdateThingGroup",
@@ -12579,15 +12619,17 @@
             "PutDestinationPolicy",
             "PutLogEvents",
             "PutMetricFilter",
             "PutQueryDefinition",
             "PutResourcePolicy",
             "PutRetentionPolicy",
             "PutSubscriptionFilter",
+            "StartLiveTail",
             "StartQuery",
+            "StopLiveTail",
             "StopQuery",
             "TagLogGroup",
             "TagResource",
             "TestMetricFilter",
             "Unmask",
             "UntagLogGroup",
             "UntagResource",
@@ -18607,25 +18649,27 @@
         "ARNRegexes": [
             "^arn:aws:signer:.+"
         ],
         "Actions": [
             "AddProfilePermission",
             "CancelSigningProfile",
             "DescribeSigningJob",
+            "GetRevocationStatus",
             "GetSigningPlatform",
             "GetSigningProfile",
             "ListProfilePermissions",
             "ListSigningJobs",
             "ListSigningPlatforms",
             "ListSigningProfiles",
             "ListTagsForResource",
             "PutSigningProfile",
             "RemoveProfilePermission",
             "RevokeSignature",
             "RevokeSigningProfile",
+            "SignPayload",
             "StartSigningJob",
             "TagResource",
             "UntagResource"
         ],
         "ConditionKeys": [
             "aws:RequestTag/${TagKey}",
             "aws:ResourceTag/${TagKey}",
```

### Comparing `iam_actions-1.2.20230606/pyproject.toml` & `iam_actions-1.2.20230607/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "iam-actions"
-version = "1.2.20230606"
+version = "1.2.20230607"
 description = "JSON of AWS policy components"
 authors = ["Constable <info@constableapp.com>"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/constableapp/iam_actions"
 packages = [{include = "iam_actions"}]
```

### Comparing `iam_actions-1.2.20230606/setup.py` & `iam_actions-1.2.20230607/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 ['iam_actions', 'iam_actions.generate']
 
 package_data = \
 {'': ['*']}
 
 setup_kwargs = {
     'name': 'iam-actions',
-    'version': '1.2.20230606',
+    'version': '1.2.20230607',
     'description': 'JSON of AWS policy components',
     'long_description': '# iam_actions\n\n`iam_actions` is a python module which contains a dictionary of AWS IAM information. Ideally, it is a complete catalog of all AWS services, actions, and resource types. The information is scraped from the AWS documentation pages.\n\nNightly, the scraping service runs, and publishes a new version with the date appended. \n\nThe package is meant to be used as a consumable package, but it also contains the code to generate the definitions for packaging.\n\nThere are three "roots" that you can consume: actions, resource_types, and services. They all currently return as dict\'s. *However, in a future release, it will be returned as python data structures*\n\n## Actions\n\nActions is a listing of all the actions for a given service. The structure is as follows:\n```\n{\n    "service_name": {\n        "action_name: {\n            "access_level": access_level,\n            "action": action_name,\n            "condition_keys": [condition_key1, ...],\n            "description": description\n        }\n    }\n}\n```\n\nTherefore, you can find information about an action as follows\n\n```\n>>> iam_actions.actions[\'s3\'][\'GetObject\']\n{\'access_level\': \'Read\', \'action\': \'GetObject\', \'condition_keys\': [\'s3:AccessPointNetworkOrigin\', \'s3:DataAccessPointAccount\', \'s3:DataAccessPointArn\', \'s3:ExistingObjectTag/<key>\', \'s3:ResourceAccount\', \'s3:TlsVersion\', \'s3:authType\', \'s3:signatureAge\', \'s3:signatureversion\', \'s3:x-amz-content-sha256\'], \'description\': \'Grants permission to retrieve objects from Amazon S3\', \'orphan\': False, \'resources\': [\'object\']}\n```\n\n## Services\n\nServices list information about the service. The structure is as follows:\n\n```\n{\n    "service_name": {\n        "Actions": [action1, ...]\n        "ServiceNames": [service_name1, ...]\n        "ARNFormats": [arn_format1, ...]\n        "ConditionKeys": [condition_key1, ...]\n        "HasResource": bool\n    }\n}\n```\n\n## Resource Types\n\nResource Types list information about the resource types for the service. The structure is as follows:\n\n```\n{\n    "service_name": {\n        "resource_name": {\n            "arn_pattern": arn_pattern,\n            "condition_keys": [condition_key1, ...]\n        }\n    }\n}\n```\n\n## Usage\n\n```python\nimport iam_actions\n\nprint(item_actions.services)\nprint(item_actions.actions)\nprint(item_actions.resource_types)\n```\n',
     'author': 'Constable',
     'author_email': 'info@constableapp.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/constableapp/iam_actions',
```

### Comparing `iam_actions-1.2.20230606/PKG-INFO` & `iam_actions-1.2.20230607/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: iam-actions
-Version: 1.2.20230606
+Version: 1.2.20230607
 Summary: JSON of AWS policy components
 Home-page: https://github.com/constableapp/iam_actions
 License: MIT
 Author: Constable
 Author-email: info@constableapp.com
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
```

