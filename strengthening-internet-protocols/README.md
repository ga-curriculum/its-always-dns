<h1>
  <span class="headline">It's Always DNS</span>
  <span class="subhead">Strengthening Internet Protocols</span>
</h1>

**Learning objective:** By the end of this lesson, students will be able to formulate strategies to enhance the security and resilience of critical internet infrastructure.

## Hardening DNS: Trust but verify

Modern DNS security enhancements address many of the protocol's original vulnerabilities:

1. **DNSSEC (DNS Security Extensions):**

   - Adds digital signatures to DNS records.
   - Verifies DNS data authenticity and integrity.
   - Prevents cache poisoning attacks.

2. **DNS over HTTPS (DoH) and DNS over TLS (DoT):**

   - Encrypts DNS queries and responses.
   - Prevents eavesdropping and manipulation.
   - Enhances privacy by hiding DNS traffic.

3. **DNS resilience strategies:**

   - Multiple DNS providers.
   - Anycast DNS deployment.
   - Monitoring and anomaly detection.
   - Rate limiting and filtering.

## Securing BGP: Building trust into routing

BGP security initiatives aim to verify routing information:

1. **Resource Public Key Infrastructure (RPKI):**

   - Cryptographic framework to validate route origins.
   - Allows networks to verify who owns IP address blocks.
   - This is the most basic form of BGP security. Organizations like Cloudflare [use the implementation of RPKI to measure the safety of the BGP protocol as a whole](https://isbgpsafeyet.com/).

2. **BGPsec:**

   - Extends RPKI to validate the entire path.
   - Creates a chain of signatures for route announcements.

3. **[MANRS](https://manrs.org/) (Mutually Agreed Norms for Routing Security):**

   - Community-driven initiative for routing security.
   - Filtering, anti-spoofing, coordination, and validation.

## Organizational best practices

Beyond protocol improvements, organizations should:

1. **Implement DNS redundancy:**

   - Use multiple DNS providers.
   - Set appropriate TTL values.
   - Maintain backup DNS configurations.

2. **Deploy monitoring and alerting:**

   - Monitor DNS and BGP for anomalies.
   - Set up alerting for unexpected changes.
   - Participate in threat intelligence sharing.

3. **Prepare incident response:**

   - Develop playbooks for DNS/BGP incidents.
   - Conduct tabletop exercises.
   - Maintain offline contact information for key providers.

4. **Follow defense in depth:**

   - Don't rely solely on DNS/BGP security.
   - Implement application-level security controls.
   - Educate teams about infrastructure vulnerabilities.

The internet's core protocols may remain inherently fragile. However, we can significantly reduce their vulnerability to accidental failures and malicious attacks through layered defenses and continued protocol evolution.

## Key takeaways

DNS and BGP are critical but inherently fragile internet infrastructures. These protocols were designed with limited security considerations.

Because of how these critical systems were designed, we're left to contend with their downsides. Major outages can and do occur, affecting large portions of the internet. Implementing security enhancements like DNSSEC and encryption in your organization is essential.

It also means that as an IT professional, you should advocate for security measures such as RPKI, BGPsec, and MANRS in the industry. While you might not be able to implement these measures directly, you can still push your organization to work with vendors and providers that do.
