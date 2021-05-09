# Pi-Hole + Unbound on Docker - For Use in Networks with Unraid Servers  


###Modified to allow Unraid SSL Certificates and DNS Resolution

### Use Docker to run [Pi-Hole](https://pi-hole.net) with an upstream [Unbound](https://nlnetlabs.nl/projects/unbound/about/) resolver.

Install Unbound directly into the Pi-Hole container
  - This configuration contacts the DNS root servers directly, please read the Pi-Hole docs on [Pi-hole as All-Around DNS Solution](https://docs.pi-hole.net/guides/unbound/) to understand what this means.
  - With this approach, we can also simply our networking since `macvlan` is no longer necessary.

