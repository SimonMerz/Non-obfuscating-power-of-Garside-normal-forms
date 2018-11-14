# Non-obfuscation-of-Garside-normal-form
This project contains the necessary parts of WalnutDSA and our attack on WalnutDSA implemented using MAGMA. Moreover, it contains our decomposition algorithm to solve some instances of the conjugacy search problem in braid groups.

In order to generate signatures, we defined the following functions: (in Walnut.txt)
1. encode_msg: the encoder of WalnutDSA taking a bit string and encoding it to a pure braid
2. generate_braid_with_perm: a generator for braids in B_N inducing a given permutation in S_N
3. generate_cloaking_elt: a generator of cloaking elements of the form as in Proposition 15 of the paper "On the (non) obfuscating power of  Garside normal forms".
4. generate_sig: the generator of WalnutDSA^TM signatures

For the cryptanalysis, we implemented: (in Attack.txt)
1. forge_sig: our attack that locates and replaces the encoding of a message in a signature
2. verify_forgery: a function that verifies whether our attack was successful.

Test.txt can be used to generate instances of WalnutDSA^TM, apply the attack on it and check whether we launched a successful universal forgery attack.

Conjugacysearch.txt contains a function applying the same decomposition algorithm that is used in "forge_sig" to solve instances of CSP in braid groups.  The success of the algorithm can be tested using TestCSP on randomly generated instances of braids. 
