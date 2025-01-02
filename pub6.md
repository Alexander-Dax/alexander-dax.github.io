---
layout: publication
---

# Breaking and Provably Restoring Authentication: A Formal Analysis of SPDM 1.2 including Cross-Protocol Attacks

<h2> Abstract </h2>

The SPDM (Security Protocol and Data Model) protocol is a standard under development by the DMTF consortium, and
supported by major industry players including Broadcom, Cisco, Dell, Google, HP, IBM, Intel, and NVIDIA. SPDM 1.2
is a complex protocol that aims to provide platform security, for example for communicating hardware components or
cloud computing scenarios.

In this work, we provide the first holistic, formal analysis of SPDM 1.2: we model the full protocol flow of SPDM
considering all of its modes – especially the complex interaction between its different key-exchange modes – in the
framework of the Tamarin prover, making our resulting model one of the most complex Tamarin models to date. To our
surprise, Tamarin finds a cross-protocol attack that allows a network attacker to completely break authentication
of the pre-shared key mode. We implemented our attack on the SPDM reference implementation, and reported the issue
to the SPDM developers. DMTF registered our attack as a CVE with CVSS rating 9 (critical).

We propose a fix and develop the first formal symbolic proof using the Tamarin prover for the fixed SPDM 1.2 protocol
as a whole. The resulting model of the main modes and their interactions is highly complex, and we develop supporting
lemmas to enable proving properties in the Tamarin prover, including the absence of all cross-protocol attacks. Our
fix has been incorporated into both the reference implementation and the newest version of the standard. Our results
highlight the need for a holistic analysis of other internet standards and the importance of providing generalized
security guarantees across entire protocols.

<h2> Co-Authors </h2>

<div class="coolcontainer">
{% include_relative _includes/cas.md %}
{% include_relative _includes/aurora.md %}
</div>
<br>
<div class="publications">
<ol class="bibliography">

{% include_relative _includes/publication6.md %}
<br>

</ol>
</div>
