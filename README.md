# Shredder en Assembler x86_64

<p align="center">
  <img width="1000" src="https://github.com/user-attachments/assets/e59d3161-4cc1-4103-b741-7e789cbbe41b" alt="jeanjass-honolulu"/>
</p>

`L'effaceur` est un programme asm qui permet d'écraser un fichier en le rendant illisible avant de supprimer son contenu.  
Il est conçu pour assurer que les données supprimées sont irrécupérables, même avec des outils d'analyse forensics.

---

## PREREQUIS

- **Système d'exploitation :** Linux (x86_64).
- **Assembleur :** NASM (Netwide Assembler).
- **Linker :** ld (GNU linker).

---

## INSTALLATION

1. Clonez ce dépôt :
   ```bash
   git clone https://github.com/B1J1M11/Shredder.git
   cd file-shredder

2. Compiler lee dépôt :
   ```bash
   nasm -f elf64 shredder.asm -o shredder.o
   ld shredder.o -o shredder

3. Executer le code :
   ```bash
   ./shredder

---

## AXE D'AMELIORATION :

- Rajouter une barre de progression pour les fichiers qui sont volumineux.
- Demander combien de fois l'utilisateur veux overwrite.
