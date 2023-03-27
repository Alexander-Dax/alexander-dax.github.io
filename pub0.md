---
layout: publication
---
# How To Wrap It Up - A Formally Verified Proposal for the use of Authenticated Wrapping in PKCS#11

## Abstract
Being the most widely used and comprehensive standard for hardware security modules, cryptographic tokens and smart cards,
PKCS#11 has been the subject of academic study for years. PKCS#11 provides a key store that is separate from the application, so
that, ideally, an application never sees a key in the clear. Again and again, researchers have pointed out the need for an import/export
mechanism that ensures the integrity of the permissions associated to a key. With version 2.40, for the first time, the standard included
authenticated deterministic encryption schemes. The interface to this operation is insecure, however, so that an application can get the
key in the clear, subverting the purpose of using a hardware security module.
This work proposes a formal model for the secure use of authenticated deterministic encryption in PKCS#11, including concrete
API changes to allow for secure policies to be implemented. Owing to the authenticated encryption mechanism, the policy we propose
provides more functionality than any policy proposed so far and can be implemented without access to a random number generator. Our
results cover modes of operation that rely on unique initialisation vectors (IVs), like GCM or CCM, but also modes that generate synthetic
IVs. We furthermore provide a proof for the deduction soundness of our modelling of deterministic encryption in Böhl et. al.’s composable
deduction soundness framework.

<div class="publications">
<ol class="bibliography">

{% include_relative _includes/publication0.md %}
<br>
</ol>
</div>