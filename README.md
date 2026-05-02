# Exercice 6 : Champs Static en Java

## But du projet
Illustrer la différence entre un attribut static (partagé par toutes les instances) et un attribut non‑static (propre à chaque objet) grâce à une classe Personne.

---

## Organisation

- Personne.java : contient un compteur static et un compteur non‑static.
- Main.java : crée plusieurs objets Personne et affiche les valeurs des compteurs.

---

## Pré-requis

- JDK 21 installé
- IntelliJ IDEA ou autre IDE
- Git disponible sur la machine

---

## Mise en place

1. Cloner le dépôt :
   git clone https://github.com/cmoussa07/StaticFieldsTest.git
2. Ouvrir le projet dans IntelliJ.
3. Vérifier que le JDK configuré est bien la version 21.
4. Lancer la classe Main.

---

## Logique du programme

- 4 objets Personne sont créés.
- À chaque instanciation, le constructeur incrémente les deux compteurs.
- nbInstances (static) augmente à chaque création car il est partagé.
- nbLocal (non‑static) repart de zéro pour chaque objet, donc vaut toujours 1.

---

## Résultat attendu

(1,4)

- 1 = compteur local de la 4e personne.
- 4 = compteur global partagé par toutes les instances.

---

## Notions clés

- Attribut static : une seule copie en mémoire, commune à tous les objets.
- Attribut non‑static : chaque objet possède sa propre copie.
- Constructeur : utilisé pour incrémenter les compteurs lors de la création.
