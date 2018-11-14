# Non-obfuscation-of-Garside-normal-form
This project contains the necessary parts of WalnutDSA^TM and our attack on WalnutDSA implemented using MAGMA. Moreover, it contains our decomposition algorithm to solve some instances of the conjugacy search problem in braid groups.

The necessary parts of WalnutDSA^TM to generate signatures can be found in Walnut.txt. Our attack on the signature scheme is implemented in Attack.txt as well as a function to verify whether our universal forgery attack was successful. 
Test.txt can be used to generate instances of WalnutDSA^TM, apply the attack on it and check whether we launched a successful universal forgery attack.

Conjugacysearch.txt contains a function applying the same decomposition algorithm used to forge Walnut signatures to solve instances of CSP in braid groups.  The success of the algorithm can be tested using TestCSP on randomly generated instances of braids. 
