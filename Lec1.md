- NP Proofs => Efficiently verifiable proofs
- P Proofs => Efficiently solvable proofs

   **b=1** checks if the randomness is generated according to protocol.  
   **b=0** check if the prover knows x assuming the randomness generated according to the protocol.  
   So half of the time we check if the randomness is generated fairly (it is crucial for the second part) half of the time we check x. Both of the steps are important.  

![image](https://user-images.githubusercontent.com/37501487/223778812-c1e6e57c-69a2-424e-850a-17759e7f4bcb.png)

Properties of a ZKP:
- Completeness: The claims that are true always have proof, preferably short proofs.
- Soundness: The claims that are false never have proofs.
- Zero-knowledge: There is no information leaked or made public.

![image](https://user-images.githubusercontent.com/37501487/223881276-a55ddbaa-c697-4e45-be6e-d161acfb1751.png)

To prove without actually revealing any information, **Interaction** & **Randomness** come into the picture.
Incase of interaction, the verifier may have a non-trivial interaction with the prover.
Incase of randomness, there may be a small probability of an error in the acceptance/rejectance.

![IMG_3381](https://user-images.githubusercontent.com/37501487/224408474-baa84ddc-f02d-4f25-a715-bffd09de6e73.jpeg)


![image](https://user-images.githubusercontent.com/37501487/223883352-267de075-b044-41b5-a29d-bde68f29d183.png)

![image](https://user-images.githubusercontent.com/37501487/223883888-d67d4be0-f96b-4fca-a6fc-5b01453fa068.png)

![image](https://user-images.githubusercontent.com/37501487/223885676-640e82c8-5b4e-440f-92a9-6b2143fbeff3.png)

![image](https://user-images.githubusercontent.com/37501487/223886116-fc538c2e-377f-48d7-86b3-912bbc7d68eb.png)

![image](https://user-images.githubusercontent.com/37501487/223886323-79691c6c-d43c-468c-ab68-ba0cbe2eed33.png)

![image](https://user-images.githubusercontent.com/37501487/223886700-c6fac85b-0fde-482d-829a-7e21e9bcd5af.png)

Some Takeaways:
- Legacy, common proofs:
  - **Completeness**: Theorem is true: Verifier is definitely convinced: P[Verifier is convinced] = 1
  - **Soundness**: Theorem is false: Verifier cannot be convinced: P[Verifier is convinced] = 0

- Interactive Proof:
  - **Completeness**: Statement is true: P[Verifier is convinced] > 1/2
  - **Soundness**: Statement is false: P[Verifier is convinced] < 1/2

![image](https://user-images.githubusercontent.com/37501487/224381582-b219ef75-c377-45cd-8a04-6f654aad6168.png)
