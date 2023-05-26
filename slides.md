---
# try also 'default' to start simple
theme: seriph
background: https://source.unsplash.com/N9jijWmF4dQ
# apply any windi css classes to the current slide
class: 'text-center'
# https://sli.dev/custom/highlighters.html
highlighter: shiki
transition: fade-out
---

# REST Easy

Les astuces pour concevoir simplement vos API REST.

---
transition: fade-out
---

# C'est quoi REST?

REpresentation State Transfert

Roy Fielding:
> "Style d'architecture pour les systmèmes distribué basés sur le réseau".

Les contraintes applicables sur une API REST:
- Client-Server
- Stateless
- Cache
- Uniform Interface
- Layered System

<br>

<p class="text-sm font-light pb-3">Pour plus d'informations voir <a href=https://www.ics.uci.edu/~fielding/pubs/dissertation/top.htm>Architectural Styles and the Design of Network based Software Architectures</a>
par Roy Fielding</p>

<!--
Blabla
-->

<style>
h1 {
  background-color: #2B90B6;
  background-image: linear-gradient(45deg, #4EC5D4 10%, #146b8c 20%);
  background-size: 100%;
  -webkit-background-clip: text;
  -moz-background-clip: text;
  -webkit-text-fill-color: transparent;
  -moz-text-fill-color: transparent;
}
blockquote {
  p {
    @apply text-teal-500 dark:text-teal-400;
  }
}
</style>

---
transition: fade-out
layout: two-cols
---
# Interface uniforme

## Contraintes d'interface uniforme

REST est défini par [quatre contraintes d'interface](https://www.ics.uci.edu/~fielding/pubs/dissertation/rest_arch_style.htm#sec_5_2) :
- identification des ressources
- manipulation des ressources via des représentations
- messages **auto-descriptifs**
- l'hyperlien comme moteur de l'état de l'application (HATEOAS)

::right::

<br>
<br>
<br>

## Messages REST

Le structure de message:
- identifiant
- representation de ressource
- metadonnées de representation de ressource
- données de contrôle


<!--
Identifiant sert à la fois identifier de manière unique un ressource dans le système ET exprimer la rélation avec d'autres ressources.
Exemple: un livre dans le bibliothèques, un livre preferé (qui peut être physiquement le même livre) d'une personne.

Données de contrôle - le but de message, l'action à effectuer
-->

---
transition: fade-out
---
# Representation de ressource

## Un nom 
Et pas un verbe

--> exemples ici

## L'ensemble des données identifiables

--> exemples ici

---
transition: fade-out
---
# Identifiant de ressource

---
layout: end
---

