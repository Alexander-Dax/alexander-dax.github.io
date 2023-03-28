---
layout: publication
---
# On the Soundness of Infrastructure Adversaries



<h2> Abstract </h2>

Companies and network operators perform risk
assessment to inform policy-making, guide infrastructure investments
 or to comply with security standards such as ISO 27001.
Due to the size and complexity of these networks, risk assessment
techniques such as attack graphs or trees describe the attacker
with a finite set of rules. This characterization of the attacker can
easily miss attack vectors or overstate them, potentially leading
to incorrect risk estimation.

In this work, we propose the first methodology to justify a
rule-based attacker model. Conceptually, we add another layer
of abstraction on top of the symbolic model of cryptography,
which reasons about protocols and abstracts cryptographic primitives. 
This new layer reasons about Internet-scale networks and
abstracts protocols.

We show, in general, how the soundness and completeness of
a rule-based model can be ensured by verifying trace properties,
linking soundness to safety properties and completeness to liveness properties. 
We then demonstrate the approach for a recently
proposed threat model that quantifies the confidentiality of email
communication on the Internet, including DNS, DNSSEC, and
SMTP. Using off-the-shelf protocol verification tools, we discover
two flaws in their threat model. After fixing them, we show that
it provides symbolic soundness.

<h2> Co-Authors </h2>

<div class="coolcontainer">
{% include_relative _includes/kuennemann.md %}
</div>
<br>
<div class="publications">
<ol class="bibliography">

{% include_relative _includes/publication1.md %}
<br>
</ol>
</div>