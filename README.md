# Tamarin-prover-PUF-Authentication-protocol
The code verifies multiple security properties of the authentication protocol proposed in:

Miroslav Mitev, Mahdi Shekiba-Herfeh, Arsenia Chorti, Martin Reed, "Multi-factor Physical Layer Security Authentication in Short Blocklength Communication" (https://arxiv.org/abs/2010.14457).

As showed in Figure 1 the protocol provides: aliveness, weak agreement, noninjective agreement injective agreement, message authentication, perfect forward secrecy. Rules  Further, figure 2 shows that the protocol provides anonymity and untraceability. These are verified using observation equivalence: simply comment rules Compromise_Alice and Compromise_Bob 



| ![](</images/PropertyVerification.jpg>) | 
|:--:| 
|Figure 1:|


| ![](</images/Observation_equivalence.jpg>) |
|:--:|
|Figure 2:|
