# Mathéo Glessmer
**Élève-ingénieur à l'ENSIIE** (Évry) · Spécialisation HPC, Systèmes & Bas Niveau  
En recherche d'un **stage de 3 à 4 mois** en **Cybersécurité offensive** (Exploitation binaire / Sécurité système) ou **Ingénierie Bas Niveau & HPC**.

---

### À propos

Étudiant en filière Calcul Haute Performance à l'ENSIIE[cite: 1, 3], j'ai choisi cette formation pour sa proximité avec le matériel, l'architecture des processeurs et le fonctionnement interne du noyau Linux[cite: 5, 11].

J'oriente aujourd'hui mes compétences en **C, C++, assembleur x86-64 et systèmes d'exploitation** vers la **cybersécurité offensive**[cite: 11] :
- **Exploitation binaire & mémoire** : compréhension des corruptions de mémoire (pile/tas), des mécanismes d'allocation et du contournement des protections système[cite: 4, 11].
- **Sécurité noyau & OS** : étude approfondie de l'ordonnanceur Linux 4.9 (gestion des verrous, routines de changement de contexte x86-64, préemption)[cite: 6, 8, 10, 11].
- **Calcul scientifique & Optimisation** : analyse vectorielle, mémoïsation TLB/cache et utilisation de routines BLAS/LAPACK[cite: 1, 14].

---

### Projets phares

* **[ipsdev — Simulation & Optimisation de Densité Nucléaire](https://github.com/MatheoGlessmer/ipsdev)**  
  Modélisation en C++ de densité nucléaire sur base d'oscillateur harmonique cylindrique[cite: 14]. Travail d'accélération matérielle et algorithmique (optimisation de cache/TLB, factorisation de Cholesky, algèbre linéaire BLAS 3 / DGEMM) permettant d'atteindre un gain de performance de **×160** par rapport à l'implémentation naïve[cite: 14]. Interface et wrapper natif Python[cite: 14].

* **[hp-allocator — Allocateur mémoire Huge Pages](https://github.com/MatheoGlessmer/hp-allocator)**  
  Conception en C d'un allocateur mémoire en espace utilisateur réservant des Huge Pages (2 Mo)[cite: 4]. Mise en place d'un benchmark mesurant le gain de performance et la réduction des défauts de TLB face à un allocateur classique sous forte charge[cite: 4].

* **[tipe-economie — Simulation de flux discrets en C](https://github.com/MatheoGlessmer/tipe-economie)**  
  Simulateur de dynamiques de marchés discrets écrit en C[cite: 1]. Calcul en virgule fixe ($10^{-6}$), modularité via pointeurs de fonctions, sérialisation personnalisée, calcul de jacobien et analyse de stabilité spectrale avec LAPACK[cite: 1].

* **[linux-sched-study — Analyse du noyau Linux 4.9](https://github.com/MatheoGlessmer/ensiie_tp)**  
  Étude technique du code source de l'ordonnanceur (`kernel/sched/`)[cite: 5] : analyse de l'appel système `sched_yield`[cite: 6], synchronisation par verrous de runqueue[cite: 8], bascule de contexte en assembleur x86-64[cite: 10] et gestion de l'arbre rouge-noir dans l'ordonnanceur CFS[cite: 12, 13].

---

### Compétences techniques

* **Langages :** C (C99/C11), C++ (C++17), Assembleur x86-64, Python, Bash
* **Systèmes & Bas niveau :** GNU/Linux, structures internes du noyau, pagination mémoire (TLB, Huge Pages)[cite: 4, 6]
* **Outils & Profiling :** Make, GDB, Perf, Valgrind, Doxygen, Git[cite: 1, 14]
* **Mathématiques & Calcul :** Algèbre linéaire, Armadillo, BLAS, LAPACK[cite: 1, 14]

---

### Contact

- **Email :** [matheo.glessmer@proton.me](mailto:matheo.glessmer@proton.me)[cite: 3]
- **LinkedIn :** [pas encore disponible](https://www.linkedin.com)