---
swagger: "2.0"
x-collection-name: AWS EC2
x-complete: 1
info:
  title: AWS EC2 API
  version: 1.0.0
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /?Action=AssociateAddress:
    get:
      summary: Associate Address
      description: Associates an Elastic IP address with an instance or a network
        interface.
      operationId: associateaddress
      x-api-path-slug: actionassociateaddress-get
      parameters:
      - in: query
        name: AllocationId.N
        description: '[EC2-VPC] One or more allocation IDs'
        type: string
      - in: query
        name: DryRun
        description: Checks whether you have the required permissions for the action,
          without actually making the request,        and provides an error response
        type: string
      - in: query
        name: Filter.N
        description: One or more filters
        type: string
      - in: query
        name: PublicIp.N
        description: '[EC2-Classic] One or more Elastic IP addresses'
        type: string
      responses:
        200:
          description: OK
      tags:
      - IP Address
  /?Action=AssociateDhcpOptions:
    get:
      summary: Associate Dhcp Options
      description: Associates a set of DHCP options (that you've previously created)
        with the specified VPC, or associates no DHCP options with the VPC.
      operationId: associatedhcpoptions
      x-api-path-slug: actionassociatedhcpoptions-get
      parameters:
      - in: query
        name: DhcpConfiguration.N
        description: A DHCP configuration option
        type: string
      - in: query
        name: DryRun
        description: Checks whether you have the required permissions for the action,
          without actually making the request,        and provides an error response
        type: string
      responses:
        200:
          description: OK
      tags:
      - DHCP
  /?Action=AssociateRouteTable:
    get:
      summary: Associate Route Table
      description: Associates a subnet with a route table.
      operationId: associateroutetable
      x-api-path-slug: actionassociateroutetable-get
      parameters:
      - in: query
        name: DestinationCidrBlock
        description: The IPv4 CIDR address block used for the destination match
        type: string
      - in: query
        name: DestinationIpv6CidrBlock
        description: The IPv6 CIDR block used for the destination match
        type: string
      - in: query
        name: DryRun
        description: Checks whether you have the required permissions for the action,
          without actually making the request,        and provides an error response
        type: string
      - in: query
        name: EgressOnlyInternetGatewayId
        description: '[IPv6 traffic only] The ID of an egress-only Internet gateway'
        type: string
      - in: query
        name: GatewayId
        description: The ID of an Internet gateway or virtual private gateway attached
          to your VPC
        type: string
      - in: query
        name: InstanceId
        description: The ID of a NAT instance in your VPC
        type: string
      - in: query
        name: NatGatewayId
        description: '[IPv4 traffic only] The ID of a NAT gateway'
        type: string
      - in: query
        name: NetworkInterfaceId
        description: The ID of a network interface
        type: string
      - in: query
        name: RouteTableId
        description: The ID of the route table for the route
        type: string
      - in: query
        name: VpcPeeringConnectionId
        description: The ID of a VPC peering connection
        type: string
      responses:
        200:
          description: OK
      tags:
      - Route Table
  /?Action=AssociateSubnetCidrBlock:
    get:
      summary: Associate Subnet Cidr Block
      description: Associates a CIDR block with your subnet.
      operationId: associatesubnetcidrblock
      x-api-path-slug: actionassociatesubnetcidrblock-get
      parameters:
      - in: query
        name: AvailabilityZone
        description: The Availability Zone for the subnet
        type: string
      - in: query
        name: CidrBlock
        description: The IPv4 network range for the subnet, in CIDR notation
        type: string
      - in: query
        name: DryRun
        description: Checks whether you have the required permissions for the action,
          without actually making the request,        and provides an error response
        type: string
      - in: query
        name: Ipv6CidrBlock
        description: The IPv6 network range for the subnet, in CIDR notation
        type: string
      - in: query
        name: VpcId
        description: The ID of the VPC
        type: string
      responses:
        200:
          description: OK
      tags:
      - CIDR Block
  /?Action=AssociateVpcCidrBlock:
    get:
      summary: Associate Vpc Cidr Block
      description: Associates a CIDR block with your VPC.
      operationId: associatevpccidrblock
      x-api-path-slug: actionassociatevpccidrblock-get
      parameters:
      - in: query
        name: AmazonProvidedIpv6CidrBlock
        description: Requests an Amazon-provided IPv6 CIDR block with a /56 prefix
          length for the VPC
        type: string
      - in: query
        name: CidrBlock
        description: The IPv4 network range for the VPC, in CIDR notation
        type: string
      - in: query
        name: DryRun
        description: Checks whether you have the required permissions for the action,
          without actually making the request,        and provides an error response
        type: string
      - in: query
        name: InstanceTenancy
        description: The tenancy options for instances launched into the VPC
        type: string
      responses:
        200:
          description: OK
      tags:
      - CIDR Block
  /?Action=ReplaceNetworkAclAssociation:
    get:
      summary: Replace Network Acl Association
      description: Changes which network ACL a subnet is associated with.
      operationId: replacenetworkaclassociation
      x-api-path-slug: actionreplacenetworkaclassociation-get
      parameters:
      - in: query
        name: CidrBlock
        description: The IPv4 network range to allow or deny, in CIDR notation (for
          example                172
        type: string
      - in: query
        name: DryRun
        description: Checks whether you have the required permissions for the action,
          without actually making the request,        and provides an error response
        type: string
      - in: query
        name: Egress
        description: Indicates whether to replace the egress rule
        type: string
      - in: query
        name: Icmp
        description: 'ICMP protocol: The ICMP or ICMPv6 type and code'
        type: string
      - in: query
        name: Ipv6CidrBlock
        description: The IPv6 network range to allow or deny, in CIDR notation (for
          example                2001:bd8:1234:1a00::/64)
        type: string
      - in: query
        name: NetworkAclId
        description: The ID of the ACL
        type: string
      - in: query
        name: PortRange
        description: 'TCP or UDP protocols: The range of ports the rule applies to'
        type: string
      - in: query
        name: Protocol
        description: The IP protocol
        type: string
      - in: query
        name: RuleAction
        description: Indicates whether to allow or deny the traffic that matches the
          rule
        type: string
      - in: query
        name: RuleNumber
        description: The rule number of the entry to replace
        type: string
      responses:
        200:
          description: OK
      tags:
      - Network ACL
  /?Action=ReplaceRouteTableAssociation:
    get:
      summary: Replace Route Table Association
      description: Changes the route table associated with a given subnet in a VPC.
      operationId: replaceroutetableassociation
      x-api-path-slug: actionreplaceroutetableassociation-get
      responses:
        200:
          description: OK
      tags:
      - Route Table
---