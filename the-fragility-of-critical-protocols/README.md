<h1>
  <span class="headline">It's Always DNS</span>
  <span class="subhead">The Fragility of Critical Protocols</span>
</h1>

**Learning objective:** By the end of this lesson, students will be able to identify vulnerabilities in DNS and BGP that create systemic risks to internet stability.

## Trust issues: Legacy design weaknesses

Both DNS and BGP were designed in the early days of the internet when security wasn't a primary concern. They were built on a fundamental assumption of trust that doesn't align with today's threat landscape:

1. **DNS trust flaws**

   - Originally had no authentication mechanisms.
   - No verification that responses came from legitimate servers.
   - No built-in encryption.

2. **BGP trust flaws**

   - No built-in route verification.
   - Networks announce routes and others accept them on faith.
   - No authentication requirements.

These protocols were designed for a collegial, academic network — not the commercial, adversarial internet we have today.

## When DNS goes dark: Common failure points

DNS systems fail through multiple mechanisms:

1. **Cache poisoning:** Injecting false records into DNS caches to redirect users.

2. **DDoS attacks:** Overwhelming DNS servers with traffic.

3. **DNS hijacking:** Compromising DNS settings at registrars.

4. **DNS amplification:** Using DNS servers to magnify attack traffic.

5. **Configuration errors:** Simple human mistakes in DNS settings.

When major DNS providers experience outages, entire sections of the internet effectively disappear, despite the websites themselves functioning perfectly.

## BGP gone wild: Routing disasters

BGP vulnerabilities manifest in several frightening ways:

1. **Route leaks:** When an AS accidentally advertises incorrect routes.

2. **Route hijacking:** Deliberately announcing someone else's IP space.

3. **Path manipulation:** Altering the preferred path to intercept traffic.

4. **Prefix hijacking:** Announcing more specific routes to attract traffic.

These failures aren't theoretical — they happen regularly and can redirect massive amounts of traffic, creating internet "black holes" or enabling sophisticated eavesdropping attacks.

Amplifying this risk is that BGP servers are hosted by various organizations across the globe, each with their own policies, security measures, and even political motivations.

This decentralized nature means that a single misconfigured router can have global consequences. While organizations have some individual control over their choice in a DNS provider, most have relatively little control over the BGP routing paths their data takes.
