# **README - Projet STM32 Nucleo-L476RG**

## **Objectif du Projet**
Ce projet vise à allumer une **LED** connectée à **PA5** lorsque l'on appuie sur un **bouton poussoir** connecté à **PB3** sur une carte **STM32 Nucleo-L476RG**.

---

## **Configuration sous STM32CubeMX**
1. **Créer un nouveau projet** pour la carte **Nucleo-L476RG**.
2. **Configurer les GPIOs depuis CubeMX**  
Il faut chercher la référence de la carte sur internet récuperer la datasheet et regarder quel pin correspond à quelle LED et bouton poussoir.  
Sur ce petit projet nous utiliserons les pin suivant:
   - **PA5** : Mode **Output Push-Pull** (LED intégrée à la carte)
   - **PB3** : Mode **Input** avec **Pull-down** (Bouton poussoir)
3. **Configurer l’horloge** :
   - Laisser la configuration par défaut.
4. **Générer le projet** en sélectionnant **STM32CubeIDE** comme outil de compilation depuis le project manager ATTENTION il faut bien verifier que les repertoirs sont bon.

---

## **Compilation et Flashage avec STM32CubeIDE**
1. **Ouvrir le projet** généré avec STM32CubeIDE.
2. **Compiler** (`Ctrl + B` ou bouton "Build").
3. **Flasher la carte** en cliquant sur **Run > Debug (F11)**.

---



