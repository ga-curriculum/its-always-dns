<h1>
  <span class="headline">It's Always DNS</span>
  <span class="subhead">Fragility of Critical Protocols: Why They Fail</span>
</h1>

**Learning objective:** Identify vulnerabilities in DNS and BGP that create systemic risks to internet stability.

## Trust Issues: Legacy Design Weaknesses

Both DNS and BGP were designed in the early days of the internet when security wasn't a primary concern. They were built on a fundamental assumption of trust that doesn't align with today's threat landscape:

1. **DNS Trust Flaws**

- Originally had no authentication mechanisms
- No verification that responses came from legitimate servers
- No built-in encryption

2. **BGP Trust Flaws**

- No built-in route verification
- Networks announce routes and others accept them on faith
- No authentication requirements

These protocols were designed for a collegial, academic network—not the commercial, adversarial internet we have today.

## When DNS Goes Dark: Common Failure Points

DNS systems fail through multiple mechanisms:

1. **Cache Poisoning:** Injecting false records into DNS caches to redirect users

2. **DDoS Attacks:** Overwhelming DNS servers with traffic

3. **DNS Hijacking:** Compromising DNS settings at registrars

4. **DNS Amplification:** Using DNS servers to magnify attack traffic

5. **Configuration Errors:** Simple human mistakes in DNS settings

When major DNS providers experience outages, entire sections of the internet effectively disappear, despite the websites themselves functioning perfectly.

## BGP Gone Wild: Routing Disasters

BGP vulnerabilities manifest in several frightening ways:

1. **Route Leaks:** When an AS accidentally advertises incorrect routes

2. **Route Hijacking:** Deliberately announcing someone else's IP space

3. **Path Manipulation:** Altering the preferred path to intercept traffic

4. **Prefix Hijacking:** Announcing more specific routes to attract traffic

These failures aren't theoretical—they happen regularly and can redirect massive amounts of traffic, creating internet "black holes" or enabling sophisticated eavesdropping attacks.

