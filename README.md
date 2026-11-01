# Mathéo Glessmer

**Élève-ingénieur à l'ENSIIE** (Évry) · Filière Calcul haute performance (HPC) · Systèmes & bas niveau

À la recherche d'un **stage de 3 à 4 mois** à partir de mai, en Île-de-France, en **sécurité des systèmes et du logiciel** (sécurité offensive, reverse engineering, noyau et cloud) ou en **HPC / calcul scientifique**.

---

### À propos

J'ai choisi la filière HPC pour sa proximité avec le matériel, l'architecture des processeurs et le fonctionnement interne du noyau Linux. J'oriente mes compétences en **C, C++ et systèmes d'exploitation** vers la **sécurité des systèmes**, où comprendre ce qui se passe sous le capot est essentiel :

- **Mémoire** : allocateur en espace utilisateur (blocs, liste de blocs libres, huge pages), pagination, TLB et caches.
- **Noyau & OS** : étude du code de l'ordonnanceur Linux 4.9 (verrou de la run queue, préemption, changement de contexte en assembleur x86-64).
- **Calcul scientifique & optimisation** : mesure de performances, optimisation mémoire et cache, BLAS niveau 3, LAPACK.

---

### Projets

* **[ipsdev — densité nucléaire](https://github.com/MatheoGlessmer/ipsdev)** *(projet d'équipe, 3 personnes)*
* 
  Modélisation en C++ de la densité nucléaire locale sur base d'oscillateur harmonique cylindrique (polynômes d'Hermite et de Laguerre, base tronquée), avec Armadillo et tests CxxTest. Comparaison de plusieurs algorithmes de calcul, du naïf aux produits matriciels par blocs (BLAS niveau 3) : jusqu'à **×160** sur une grille 100×100, avec des écarts de l'ordre de 10⁻¹⁵ par rapport à la référence. Wrapper Python pour la visualisation.

  Ma part : 
    1. Makefile
    2. Test des fonctions polynome
    3. Wrapper Python
    4. Algorithme et optimisation

* **[hp-allocator — allocateur mémoire sur huge pages](https://github.com/MatheoGlessmer/hp-allocator)**
* 
  Allocateur en C en espace utilisateur sur une zone de huge pages (2 Mo) : en-têtes de blocs, liste chaînée de blocs libres, alignement. Mesure de l'impact des huge pages avec le benchmark du TD : temps de lecture stable (≈ 0,02 s) au-delà d'environ 1,4 million de doubles, contre une hausse jusqu'à ≈ 0,035 s avec des pages standards (défauts de TLB). Limites documentées : pas de fusion des blocs libres, bibliothèque dynamique non terminée.

* **[TIPE — simulation de flux monétaires en C](https://github.com/MatheoGlessmer/tipe-economie)** 
* 
  Simulateur de dynamiques de marchés discrets (TIPE 2026, candidat libre) : arithmétique en virgule fixe (10⁻⁶), pointeurs de fonctions, sérialisation de marchés, suite de tests unitaires, calcul du jacobien et outil d'analyse de ses valeurs propres avec LAPACK pour étudier la stabilité locale. Exploitation des résultats en cours.

* **[Étude de l'ordonnanceur Linux 4.9](https://github.com/MatheoGlessmer/ensiie_tp/tree/main/ordonnanceur_linux)**
* 
  Étude du code de `kernel/sched/` en lecture seule : chemin de `sched_yield` jusqu'à `context_switch`, verrou de la run queue, changement de contexte x86-64, CFS (arbre rouge-noir). Rapport PDF.

---

### Compétences techniques

* **Langages :** C, C++, assembleur (RISC-V ; lecture de x86-64), Python, Bash 
* **Systèmes & bas niveau :** GNU/Linux, structures internes du noyau, pagination mémoire (TLB, huge pages)
* **Outils :** Make, Git, Valgrind, perf, AddressSanitizer, Doxygen, CxxTest 
* **Calcul :** algèbre linéaire, Armadillo, BLAS, LAPACK

---

### Contact

- **E-mail :** [matheo.glessmer@proton.me](mailto:matheo.glessmer@proton.me)