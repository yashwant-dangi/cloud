Domain Registrar - Amazon Router 53, GoDaddy

### Record Types

- A - maps a hostname to IPv4
- AAAA - maps a hostname to IPv6
- CNAME - maps a host to another hostname
  - The target is a domain name which must have A or AAAA record
  - can't create a CNAME record
  - you can't create for example.com but you can create for www.example.com
- NS - Name Servers for the hosted zones

- Public Hosted Zone - For Public Internet (Public IP)
- Private Hosted Zone - For VPC (Private IP)
