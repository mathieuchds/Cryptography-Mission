# Cryptographic Missions – Enigma & Sphynx Web Project

This project was carried out in collaboration with research professor **Pascal Lafourcade** during my second year of the integrated preparatory cycle at **ISIMA**, a French engineering school specialized in computer science.

The objective was to **design and develop an educational website** focused on the **Enigma** and **Sphynx** cipher machines. The platform allows users to explore the internal mechanisms of these historical encryption devices through **interactive and playful activities**.

The project was developed in a **two-person team** with **Benoît Dajoux**, and was intended for both classroom use and independent exploration.

> A **French version** of the project is available online at:  
> https://sancy.iut.uca.fr/~lafourcade/mission-cryptographie/enigma_sphinx/html/

---

## Features

- Interactive simulation of the **Enigma** and **Sphynx** cipher machines  
- Automatic generation of puzzles and cipher challenges  
- Manual decoding interface with drag-and-drop and band manipulation (Sphynx)  
- Educational mode for classroom activities  
- Import and export of puzzles via text files  
- Download of LaTeX/PDF puzzle sheets for print use  
- Adaptable difficulty through configurable strip counts (Sphynx)

---

## Puzzle Import Format

You can import a custom puzzle using a `.txt` file. This is especially useful in classroom settings where all participants need to work on the **same challenge**.

**File format:**

```
NumberOfStrips/SecretMessage/Key
```

**Key format:**

```
X,Y/X,Y/.../X,Y
```

- You must include **as many (X,Y) pairs** as the number of strips chosen.
- Each `X` must be **≤ 10** (upper strips), and each `Y` must be **> 10** (lower strips).
- `X` and `Y` refer to the original Sphynx strip numbers. For example, `Y = 11` corresponds to the strip **B, A, Z, ...**
- If the number of strips selected is **different from 10**, the input key may **not match the displayed key**, due to the reduction and reshuffling of available strips.

> See the puzzle interface for more details.  
> An example import file is available in this repository.

---

## Acknowledgments

I would like to warmly thank **Pascal Lafourcade** for his support and insightful guidance throughout the project. I am also grateful to the **teaching team working in collaboration with him** for their constructive feedback and ideas for improving the platform’s pedagogical use.

Finally, a special thanks to **Benoît Dajoux** for his valuable work and help, especially on the Enigma module of the project.
