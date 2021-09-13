# Experimental realization of quantum cheque using a 
# five qubit quantum computer

> https://github.com/anonymousr007/Quantum-Research-Papers/blob/main/Research-Papers/behera2017.pdf

## Table of Content

* Abstract
* Introduction
* Designing gates and some protocols on IBM Quantum Experience (QE)
* Quantum Cheque
  * The quantum cheque scheme
* Implementation of quantum cheque at IBM Quantum Experience (QE)
* Quantum state tomography
* Conclusions
* References

## Abstract

* Quantum cheques could be a forgery-free way to make transaction in a quantum networked banking system with perfect security against any no-signalling adversary,
* Here, we demonstrated the implementation of quantum cheque, proposed by Moulick and Panigrahi, using the five qubit IBM quantum computer.
* Appropriate single qubit, CNOT and fredkin gates are used in an optimized configuration.
* The accuracy of implementation is checked  and verified through quantum state tomography by comparing results from the theoretical and experimental density matrices.

## Introduction

* Currency bonds, when printed on textile or rag paper, can be counterfeited by any adversary party if it gets access to unlimited computational sources. 
* The quantum analog of the same is physically impossible to copy due to the **“No Cloning Theorem”**[1].
* Wiesner’s quantum money [2,3] has led to development of a quantum key distribution scheme, known as BB84 protocol [4], to send messages with perfect security.
* Wiesner’s original scheme was later broken [5–7]. However, Aaronson showed its existence by proposing a quantum copy protection scheme [8], which again was
broken by Lutomirski et al. [9]. New versions were then introduced by Farhi et al. [10] and Aaronson et al. [11]. Subsequently, a scheme of quantum coins was developed by Mosca and Stebila [12], based on blind quantum computation requiring a communicating bank for verification purposes.

The idea of quantum cheques was put forward by Moulick and Panigrahi [13],
which utilized quantum states to fabricate currency bonds. The proposed scheme was
perfectly secure against any no-signalling adversary based on fundamental laws of
quantum information. The quantum cheque involved a trusted bank providing every
account holder with a valid quantum cheque book to issue cheques that can be verified
by the main bank or any of its acting branches.

Establishing long distance quantum communication networks [14,15] is an active
area of research, where a quantum cheque scheme can be potentially used as an alternate for e-Payment Gateways in the field of e-commerce. It can also be considered
as the quantum analog of Electronic Data Interchange (EDI) [16]. In this scheme,
efficient transactions can be performed by storing quantum states in computers or
smart cards, equipped with quantum memories [17,18]. Without quantum memory,
the transactions can be streamed over the quantum internet [19,20]. The protocol can
run in real time, where the account holder physically goes to the Bank, collects a quantum cheque book and then prepares a quantum cheque and issues to a vendor. The
vendor then communicates the quantum cheque to the Bank and withdraws money
after a successful verification of the cheque. Recently, practical unforgeable quantum
money has found experimental verification [21,22]. The experimental demonstration
therefore paves the way for designing of physical devices for this purpose.

Here, we make use of the free web-based interface, IBM Quantum Experience (IBM
QE) [23], to experimentally demonstrate the quantum cheque transaction [13]. The
platform uses Python Application Programming Interface (API) and Software Development Kit (SDK) [24], which has enabled easy writing of codes and running them
on quantum processors. With fast access to the results of an experiment, the IBM QE
users can communicate and discuss results with IBM community. It permits a user
easy connectivity to this cloud [25] based 5-qubit quantum computer, using which a
number of quantum algorithms [26–29] and quantum computational tasks [30] have
already been performed. Test of Leggett–Garg [31] and Mermin inequality [32], quantum teleportation of an unknown single qubit [33] and two-qubit state [34] have been
reported. Entanglement-assisted invariance [35], non-Abelian braiding of surface code
defects [36], and entropic uncertainty and measurement reversibility [37] have been
illustrated. A comparison between two architectures for quantum computation [38]
and nondestructive discrimination of Bell states [39] have also been experimentally
performed. In this note, we explicate experimental realization of quantum cheque
transaction by implementing the scheme on IBM interface and find the accuracy of
quantum state preparation through quantum state tomography

## References

1. Wooters, W., Zurek, W.: Quantum no-cloning theorem. Nature 299, 802 (1982).
2. Wiesner, S.: Conjugate coding. ACM Sigact News 15(1), 78–88 (1983).
3. Bennett, C.H., Brassard, G., Breidbart, S., Wiesner, S.: Quantum cryptography, or unforgeable subway tokens. In: Chaum, D., Rivest, R.L., Sherman, A.T. (eds.) Advances in Cryptology, pp. 267–275.Springer (1983)
4. Bennett, C.H., Brassard, G.: Quantum cryptography: public key distribution and coin tossing. In: Proceedings of IEEE International Conference on Computers, Systems, and Signal Processing, pp. 175–179. Bangalore, India (1984)
5. Lutomirski, A.: An online attack against Wiesner’s quantum money. arXiv:1010.0256 (2010).
6. Molina, A., Vidick, T., Watrous, J.: Optimal counterfeiting attacks and generalizations for Wiesners quantum money. In: Theory of Quantum Computation, Communication, and Cryptography, 2012, pp.45–64. Springer (2013)
7. Brodutch, A., Nagaj, D., Sattath, O., Unruh, D.: An adaptive attack on Wiesner’s quantum money. arXiv:1404.1507 (2014)
8. Aaronson, S.: Quantum copy-protection and quantum money. In: Proceedings of 24th Annual IEEE Conference on Computational Complexity (CCC), 2009, pp. 229–242. IEEE (2009).
9. Lutomirski, A., Aaronson, S., Farhi, E., Gosset, D., Hassidim, A., Kelner, J., Shor, P.: Breaking and making quantum money: toward a new quantum cryptographic protocol. arXiv:0912.3825 (2009)
10. Farhi, E., Gosset, D., Hassidim, A., Lutomirski, A., Shor, P.: Quantum money from knots. In: Proceedings of the 3rd Innovations in Theoretical Computer Science Conference, pp. 276–289. ACM (2012)
11. Aaronson, S., Christiano, P.: Quantum money from hidden subspaces. In: Proceedings of the 44th Annual ACM Symposium on Theory of Computing, pp. 41–60. ACM (2012)
12. Mosca, M., Stebila, D.: Quantum coins. Error Correct. Codes Finite Geom. Cryptogr. 523, 35–47 (2010)
13. Moulick, S.R., Panigrahi, P.K.: Quantum cheques. Quantum Inf. Process. 15, 2475–2486 (2016)
14. Biham, E., Huttner, B., Mor, T.: Quantum cryptographic network based on quantum memories. Phys. Rev. A 54, 2651 (1996)
15. Duan, L.M., Monroe, C.: Quantum networks with trapped ions. Rev. Mod. Phys. 82, 1209 (2010)
16. Anderson, R.: Security Engineering. Wiley, New York (2008)
17. Trugenberger, C.A.: Probabilistic quantum memories. Phys. Rev. Lett. 87, 067901 (2001)
18. Simon, C., Afzelius, M., Appel, J., Boyer de la Giroday, A., Dewhurst, S., Gisin, N., Hu, C., Jelezko, F., Kröll, S., Müller, J., et al.: Quantum memories. Eur. Phys. J. D 58, 1–22 (2010)
19. Munro, W., Stephens, A., Devitt, S., Harrison, K., Nemoto, K.: Quantum communication without the necessity of quantum memories. Nat. Photonics 6, 777–781 (2012)
20. Kimble, H.: The quantum internet. Nature 453(7198), 1023–1030 (2008)
21. Bartkiewicz, K.,Cernoch, A., Chimczak, G., Lemr, K., Miranowicz, A., Nori, F.: Experimental quantum forgery of quantum optical money. npj Quantum Inf. 3(1), 7 (2017)
22. Bozzio, M., Orieux, A., Vidarte, L.T., Zaquine, I., Kerenidis, I., Diamanti, E.: Experimental demonstration of practical unforgeable quantum money. arXiv:1705.01428 (2017)
23. IBM Quantum Experience. https://www.research.ibm.com/ibm-q/.
24. Quantum computing gets an API and SDK. https://developer.ibm.com/dwblog/2017/quantumcomputing-api-sdk-david-lubensky/.
25. Castelvecchi, D.: IBM’s quantum cloud computer goes commercial. Nat. News 543, 159 (2017)
26. Shor, P.: Algorithms for quantum computation: discrete logarithms and factoring. In: Proceeding SFCS ’94 Proceedings of the 35th Annual Symposium on Foundations of Computer Science, pp. 124–134. IEEE (1994)
27. Grover, L.K.: A fast quantum mechanical algorithm for database search. In: Proceeding STOC ’96 Proceedings of the Twenty-Eighth Annual ACM Symposium on Theory of Computing, pp. 212–219. ACM (1996)
28. Ambainis, A.: Quantum search algorithms. In: Fenner, S. (ed.) Newsletter ACM SIGACT News, vol.35 (2), pp. 22–35. ACM (2004)
29. Mosca, M.: Quantum algorithms. In: Meyers, R.A. (ed.) Computational Complexity, pp. 2303–2333. Springer, New York (2012)
30. Devitt, S.J.: Performing quantum computing experiments in the cloud. Phys. Rev. A 94(3), 032329 (2016)
31. Huffman, E., Mizel, A.: Violation of noninvasive macrorealism by a superconducting qubit: implementation of a Leggett–Garg test that addresses the clumsiness loophole. Phys. Rev. A 95(3), 032131 (2017)
32. Alsina, D., Latorre, J.I.: Experimental test of Mermin inequalities on a five-qubit quantum computer. Phys. Rev. A 94(1), 012314 (2016)
33. Fedortchenko, S.: A quantum teleportation experiment for undergraduate students. arXiv:1607.02398 (2016)
34. Sisodia, M., Shukla, A., Thapliyal, K., Pathak, A.: Design and experimental realization of an optimal scheme for teleportion of an n-qubit quantum state. arXiv:1704.05294 (2017)
35. Deffner, S.: Demonstration of entanglement assisted invariance on IBM’s quantum experience. arXiv:1609.07459 (2017)
36. Wootton, J.R.: Demonstrating non-Abelian braiding of surface code defects in a five qubit experiment. Quantum Sci. Technol. 2(1), 015006 (2017)
37. Berta, M., Wehner, S., Wilde, M.M.: Entropic uncertainty and measurement reversibility. New J. Phys. 18(7), 073004 (2016)
38. Linke, N.M., Maslov, D., Roetteler, M., Debnath, S., Figgatt, C., Landsman, K.A., Wright, K., Monroe, C.: Experimental comparison of two quantum computing architectures. Proc. Natl. Acad. Sci. 114(13), 3305–3310 (2017)
39. Sisodia, M., Shukla, A., Pathak, A.: Experimental realization of nondestructive discrimination of Bell states using a five-qubit quantum computer. arXiv:1705.00670 (2017)
40. Gottesman, D., Chuang, I.: Quantum digital signatures. arXiv:quant-ph/0105032 (2001)
41. Chuang, I., Gottesman, D.: Quantum digital signatures. US Patent 7,246,240, 17 July 2007
42. Hillery, M., Bužek, V., Berthiaume, A.: Quantum secret sharing. Phys. Rev. A 59(3), 1829 (1999)
