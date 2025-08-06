# Network Architecture Diagrams

This directory contains ASCII-based network architecture diagrams for AWS networking patterns and traffic flows. These diagrams document complex network topologies and support infrastructure design decisions.

## Contents

### AWS Direct Connect Diagrams
- **`aws-directconnect.txt`** - AWS Direct Connect traffic encryption options:
  - Site-to-Site VPN to Amazon VPC (Public VIF)
  - Site-to-Site VPN to Transit Gateway (Public VIF)
  - Traffic flow patterns and configuration steps

### DNS and Hybrid Environment
- **`aws-dns-hybridenv-r53`** - DNS configuration patterns for hybrid environments using Route 53

### VPC and Transit Gateway Patterns
- **`vpc-tgw-firewall-flow.txt`** - VPC Transit Gateway architecture with firewall integration:
  - Workload spoke VPCs
  - Transit Gateway routing
  - Gateway Load Balancer with firewall fleet
  - Traffic flow patterns

- **`vpc-tfw-perimetervpc-flow.txt`** - Perimeter VPC architecture with Transit Gateway:
  - Perimeter VPC design patterns
  - Traffic flow through security layers
  - Transit Gateway integration

## Purpose

These diagrams serve to:

- Document complex network topologies visually
- Support infrastructure planning and design
- Guide AWS networking component deployment
- Assist with traffic flow troubleshooting
- Provide reference for technical discussions

## Diagram Format

Diagrams use ASCII characters to visualize network topologies including:

- Network components (VPCs, subnets, EC2 instances, load balancers)
- Connectivity lines and directional arrows
- Traffic flow indicators
- Configuration details (route tables, CIDR blocks)
- Implementation steps where applicable

## Usage

### Viewing Diagrams
```bash
# View a specific diagram
cat diagrams/aws-directconnect.txt

# View with pager for large diagrams
less diagrams/vpc-tgw-firewall-flow.txt
```

### Contributing
When adding new diagrams:

1. Use consistent ASCII formatting
2. Include clear component labels
3. Add traffic flow indicators
4. Provide implementation steps
5. Update this README with new diagram descriptions

### Best Practices
- Focus on specific architectural patterns
- Include both high-level and detailed views where appropriate
- Use consistent symbols and formatting across diagrams
- Add explanatory text for complex flows
- Include relevant AWS service names and configurations

## Related Resources

These diagrams complement the Terraform modules in the parent directory and support:
- Infrastructure as Code implementations
- Architecture decision records (ADRs)
- Network design documentation
- Security and compliance documentation

## Notes

- Diagrams require monospace fonts for proper alignment
- Large diagrams may need appropriate terminal width for optimal viewing
- These are living documents that should be updated as architectures evolve