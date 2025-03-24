# Custom VPC

- Regional Service - All AZs in a region
- Isolated network
- Nothing IN or OUT without explicit configuration
- Hybrid Networking - other cloud or on-premises
- Default or Dedicated Tenancy
- IPv4 Private CIDR Block & Public IPs
- 1 Primary Private IPv4 CIDR Block
- ...Min /28 (16 IPs) Max /16 (65,536 IPs)
- Optional Secondary IPv4 CIDR Blocks
- Optional single assigned IPv6 /56 CIDR Block

![Custom VPC](/09-VPC-Basics/02_custom_vpc/vpc_endstate.png)

## DNS in a VPC

- Provided by Amazon Route 53
- VPC Base IP + 2 Address
- `enableDnsHostnames` - gives instance DNS names
- `enableDnsSupport` - resolves public DNS names
