<h1>
  <span class="headline">It's Always DNS</span>
  <span class="subhead">Mitigating Risks: Strengthening Internet Protocols</span>
</h1>

**Learning objective:** Formulate strategies to enhance the security and resilience of critical internet infrastructure.

## Hardening DNS: Trust but Verify

Modern DNS security enhancements address many of the protocol's original vulnerabilities:

1. **DNSSEC (DNS Security Extensions):**

- Adds digital signatures to DNS records
- Verifies DNS data authenticity and integrity
- Prevents cache poisoning attacks

2. **DNS over HTTPS (DoH) and DNS over TLS (DoT):**

- Encrypts DNS queries and responses
- Prevents eavesdropping and manipulation
- Enhances privacy by hiding DNS traffic

3. **DNS Resilience Strategies:**

- Multiple DNS providers
- Anycast DNS deployment
- Monitoring and anomaly detection
- Rate limiting and filtering

## Securing BGP: Building Trust into Routing

BGP security initiatives aim to verify routing information:

1. **Resource Public Key Infrastructure (RPKI):**

- Cryptographic framework to validate route origins
- Allows networks to verify who owns IP address blocks

2. **BGPsec:**

- Extends RPKI to validate the entire path
- Creates a chain of signatures for route announcements

3. **MANRS (Mutually Agreed Norms for Routing Security):**

- Community-driven initiative for routing security
- Filtering, anti-spoofing, coordination, and validation

## Organizational Best Practices

Beyond protocol improvements, organizations should:

1. **Implement DNS Redundancy:**

- Use multiple DNS providers
- Set appropriate TTL values
- Maintain backup DNS configurations

2. **Deploy Monitoring and Alerting:**

- Monitor DNS and BGP for anomalies
- Set up alerting for unexpected changes
- Participate in threat intelligence sharing

3. **Prepare Incident Response:**

- Develop playbooks for DNS/BGP incidents
- Conduct tabletop exercises
- Maintain offline contact information for key providers

4. **Follow Defense-in-Depth:**

- Don't rely solely on DNS/BGP security
- Implement application-level security controls
- Educate teams about infrastructure vulnerabilities

The internet's core protocols may remain inherently fragile, but through layered defenses and continued protocol evolution, we can significantly reduce their vulnerability to both accidental failures and malicious attacks.

## Key Takeaways

- DNS and BGP are critical but inherently fragile internet infrastructures
- These protocols were designed with limited security considerations
- Major outages can and do occur, affecting large portions of the internet
- Security enhancements like DNSSEC, RPKI, and encryption are essential
- Defense-in-depth and redundancy are crucial organizational strategies
