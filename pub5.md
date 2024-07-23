---
layout: publication
---
# Keeping Up with the KEMs: Stronger Security Notions for KEMs and Automated Analysis of KEM-based Protocols


<h2> Abstract </h2>

Key Encapsulation Mechanisms (KEMs) are a critical building block for hybrid encryption and modern security protocols, notably in the post-quantum setting. Given the asymmetric public key of a recipient, the primitive establishes a shared secret key between sender and recipient. In recent years, a large number of abstract designs and concrete implementations of KEMs have been proposed, e.g., in the context of the NIST process for post-quantum primitives. In this work, we (i) establish stronger security notions for KEMs, and (ii) develop a symbolic analysis method to analyze security protocols that use KEMs. First, we generalize existing security notions for KEMs in the computational setting, introduce several stronger security notions and prove their relations. Our new properties formalize in which sense outputs of the KEM uniquely determine, i.e., bind, other values. Our new binding properties can be used, e.g., to prove the absence of attacks that were not captured by prior security notions. Among these, we identify a new class of attacks that we coin re-encapsulation attacks. Second, we develop a family of fine-grained symbolic models that correspond to our hierarchy of computational security notions, and are suitable for the automated analysis of KEM-based security protocols. We encode our models as a library in the framework of the Tamarin prover. Given a KEM-based protocol, our approach can automatically derive the minimal binding properties required from the KEM; or, if also given a concrete KEM, can analyze if the protocol meets its security goals. In case studies, Tamarin automatically discovers, e.g., that the key exchange protocol proposed in the original Kyber paper requires stronger properties from the KEM than the authors have proven.

<h2> Co-Authors </h2>

<div class="coolcontainer">
{% include_relative _includes/cas.md %}
{% include_relative _includes/niklas.md %}
</div>
<br>
<div class="publications">
<ol class="bibliography">

{% include_relative _includes/publication5.md %}
<br>
</ol>
</div>
