# Tamarin-prover-PUF-Authentication-protocol
The code *PUF_Authentication_protocol.spthy* verifies multiple security properties of the authentication protocol proposed in:

Miroslav Mitev, Mahdi Shekiba-Herfeh, Arsenia Chorti, Martin Reed, "Multi-factor Physical Layer Security Authentication in Short Blocklength Communication" (https://arxiv.org/abs/2010.14457).

The protocol provides: aliveness, weak agreement, noninjective agreement injective agreement, message authentication, perfect forward secrecy. The full security proofs are given in the file: Proof_of_security_properties.spthy. Figure 1 illustates the conclusion from the proofs, i.e., all properties are verified. Note that, rules **types** and **executable** are used to link the events in the protocol and to prove its executability, respectively.

Further, Figure 2 shows that the protocol provides anonymity and untraceability. These are verified using observation equivalence, i.e., an adversary cannot distinguish between two instances of the protocol. The example in Figure 2 assumes the following two instances: i) Alice sends her one-time alias ID; ii) Alice sends a random variable. These are then observed by an adversary. As shown in the figure, regardless of which parameter is observed the final result is equality, i.e., the one-time alias ID cannot be distinguished from a random variable, therefore, Alice's privacy is preserved. To implement this example simply comment rules **Compromise_Alice** and **Compromise_Bob** and add **Out(diff(A_ID_new, ~Random_variable))** to the conclusion of rule **Alice_receives_sends2**.

| ![](</images/PropertyVerification.jpg>) | 
|:--:| 
|Figure 1: Verification of the security properties of the authentication protocol|


| ![](</images/Observation_equivalence.jpg>) |
|:--:|
|Figure 2: Proof for observational equivalence. The adversary is not able distinguish between Alice's one-time alias ID and a random varible. This proves that the protocol preserve Alice's privacy.|
