<h1>
  <span class="headline">It's Always DNS</span>
  <span class="subhead">A Real-World Example of a DNS Failure</span>
</h1>

**Learning objective:** Analyze how DNS vulnerabilities materialized in the 2016 Dyn DDoS attack that disrupted major internet services.

## The 2016 Dyn DDoS Attack: Internet Partially Paralyzed

On October 21, 2016, Dyn (a major DNS provider) became the target of one of the largest distributed denial-of-service (DDoS) attacks ever witnessed. The attack came in multiple waves, with traffic volumes reaching unprecedented levels.

**Attack Details:**

- **Weapon of Choice:** The Mirai botnet, comprising ~100,000 compromised IoT devices

- **Attack Method:** DNS flood (overwhelming DNS servers with queries)

- **Attack Volume:** Estimated 1.2 Tbps

- **Duration:** Multiple waves over approximately 24 hours

**Cascade of Failures:**
Dyn provided DNS services for numerous high-profile websites and services, including:

- Twitter
- Netflix
- Reddit
- GitHub
- Airbnb
- Spotify
- The New York Times

When Dyn's DNS infrastructure became unavailable, users couldn't resolve domain names to IP addresses for these services, rendering them effectively inaccessible.

**The Aftermath:**

- Millions of users experienced internet service disruptions

- Estimated economic impact in the hundreds of millions of dollars

- Highlighted the internet's dependency on centralized DNS providers

- Accelerated the adoption of DNS security measures

- Sparked conversations about IoT security standards

This single attack on one DNS provider managed to disable access to significant portions of the internet, demonstrating how the compromise of a seemingly invisible background service can have massive ripple effects.
