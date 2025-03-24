<h1>
  <span class="headline">It's Always DNS</span>
  <span class="subhead">A Real-World Example of a DNS Failure</span>
</h1>

**Learning objective:** By the end of this lesson students will be able to analyze how DNS vulnerabilities materialized in the 2016 Dyn DDoS attack that disrupted major internet services.

## The 2016 Dyn DDoS attack: Internet partially paralyzed

On October 21, 2016, Dyn (a large DNS provider) became the target of one of the largest distributed denial-of-service (DDoS) attacks ever witnessed. The attack came in multiple waves, with traffic volumes reaching unprecedented levels. Let's review the details of the attack:

- **Weapon of choice:** The Mirai botnet, made up of ~100,000 compromised IoT devices.

- **Attack method:** DNS flood (overwhelming DNS servers with queries).

- **Attack volume:** Estimated 1.2 Tbps.

- **Duration:** Multiple waves over approximately 24 hours.

### Cascade of failures

Dyn provided DNS services for numerous high-profile websites and services, including:

- Twitter
- Netflix
- Reddit
- GitHub
- Airbnb
- Spotify
- The New York Times

When Dyn's DNS infrastructure became unavailable, users couldn't resolve domain names to IP addresses for these services, rendering them effectively inaccessible.

### The aftermath

The attack had far-reaching consequences:

- Millions of users experienced internet service disruptions.

- Estimated economic impact in the hundreds of millions of dollars.

- The attack highlighted the internet's dependency on centralized DNS providers.

- It caused an acceleration in the adoption of DNS security measures.

- The use of the Mirai botnet in the attack sparked conversations about IoT security standards.

## Takeaways

This single attack on one DNS provider restricted access to significant portions of the internet. The attack demonstrated how compromising a seemingly invisible background service can have massive ripple effects.

The lack of resilience in the DNS infrastructure is a common theme in many of the most significant internet outages. The Dyn incident presented here is just one of the contributors to a common phrase in the industry: "It's always DNS." There are even haikus about it!

![A haiku about DNS: "It's not DNS" / "There's no way it's DNS" / "It was DNS"](./assets/haiku-resized.jpeg)

Don't worry, though; despite the ubiquity of the phrase, the rest of your career won't be all about fixing DNS issues. As you've seen in this course, and even just this lesson, there are many other critical points of failure in the internet's infrastructure - DNS is just one of the most notorious.

<div class="activity solo-exercise">
  <h2 class="title">Research another DNS outage or attack</h2>
  <span class="minutes">5 min</span>
</div>

Take a few minutes to research another DNS outage or attack online. What was the cause of the outage? How did it affect users? What were the lessons learned?
