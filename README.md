# Tamarin-prover-PUF-Authentication-protocol
The code verifies multiple security properties of the authentication protocol proposed in:

Miroslav Mitev, Mahdi Shekiba-Herfeh, Arsenia Chorti, Martin Reed, "Multi-factor Physical Layer Security Authentication in Short Blocklength Communication" (https://arxiv.org/abs/2010.14457).

As showed in Figure 1 the protocol provides: aliveness, weak agreement, noninjective agreement injective agreement, message authentication, perfect forward secrecy. Rules **types** and **executable** are used to link the events in the protocol and the prove its executability, respectively.

Further, figure 2 shows that the protocol provides anonymity and untraceability. These are verified using observation equivalence. To prove that simply comment rules **Compromise_Alice** and **Compromise_Bob** and add **Out(diff(A_ID_new, ~Random_variable))** to the conclusion of rule **Alice_receives_sends2**.



| ![](</images/PropertyVerification.jpg>) | 
|:--:| 
|Figure 1:|


| ![](</images/Observation_equivalence.jpg>) |
|:--:|
|Figure 2:|
