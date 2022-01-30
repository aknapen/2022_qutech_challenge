# keytanglement

### MIT iQuHACK 2022
### QuTech Quantum Key Distribution Challenge

- Project at: [keytanglement.live](keytanglement.live)
- iQuHACK presentation [slides](https://docs.google.com/presentation/d/1JUC_5XKEcqWcx8vDHGJmTW_9klX04Cl1-xuXPzgNxpI/edit?usp=sharing)
- Jupyter Notebook in repo [link](https://github.com/JRice15/keytanglement/blob/main/jupyter_notebook/)
- Original repo - for all files/commits(https://github.com/JRice15/keytanglement)


Contributors 
- Julian Rice, Computer Science M.S. Candidate, Cal Pol SLO
- Alexander Knapen, Computer Engineering undergraduate, Cal Poly SLO
- Nayana Tiwari, Computer Engineering and Physics undergraduate, Cal Poly SLO

Technologies used:
- QuTech 26-qubit simulator
- Qiskit
- QuantumInspire
- Apache 2.0 / (very small) Ubuntu Webserver

### Project Description
Keytanglement is a web server that allows you to communicate over secure, encrypted messaging with a quantum key generated by a quantum computer. 
The server uses Bell states for Quantum Key Distribution (QKD) which has significant improvement over the simpler BB84 method. In Song and Chen's research paper
cited below, the hardware implementation of this method required only 11 qubits to detect an eavesdropper while BB84 requires 72 qubits for the same security level. 
We modified the implementation of the Bell state algorithm to abide by the modified architecture in the proposed challenge. Further explanation of the challenge,
our implementation, and its success can be found in the accompanying Jupyter notebook.

### Software Arch
#### Key Generation
![KeyArch](jupyter_notebook/SoftwareArch_KeyGeneration.png]

#### Secure Chat
![ChatArch](jupyter_notebook/SoftwareArch_SecureChat.png]

### Repository Organization:
- README.md [here]

Client scripts
- client.py
- encrypt_decrypt.py

QKD scripts
- quantum_computer.py
- key_generation.py
- tests/

Server backend
- flaskapp.py
- utils.py
- flaskapp.wsgi

Server frontend
- static/
- templates/


### Personal Experience at MIT iQuHACK 2022: 
- We learned a ton about web development and servers which none of us had ever worked with before. We also got to use some quantum computing in a very practical application which was rewarding and exciting. Overall, we had a lot of fun, even with the hard work and late night. We are excited to submit our project, Keytanglement!!

### Citations:
- Quantum Key Distribution using Bell States
  - D. Song and D. Chen, "Quantum Key Distribution Based on Random Grouping Bell State Measurement," in IEEE Communications Letters, vol. 24, no. 7, pp. 1496-1499, July 2020, doi: 10.1109/LCOMM.2020.2988380.
 - Tokyochat 
  - https://github.com/franciscop/tokyochat
