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
- Sans état (Stateless)
- **Interface Uniforme**
- Cache
- Système en couches (Layered System)

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
---
# Interface uniforme


<div class="grid grid-cols-2 gap-4">
<div>

## Concepts de base des elements de données

**Ressource**: toute information qui peut être --nommée--; une correspondance conceptuelle à un ensemble d'entités **à un moment particulier dans le temps**.
 <!-- Demonstration du concept de temps pour un ressource: livre preferé de l'utilisateur -->

**Indentifiant**: un identifiant permettant d'identifier la ressource spécifique impliquée dans une interaction entre composants.

**Representation**: capture de **l'état** actuel ou prévu d'une ressource; message constitué d'une séquence d'octets, accompagnée de métadonnées pour décrire ces octets. 

</div>
<div>

... image ...
</div>
</div>



> The trade-off, though, is that a uniform interface **degrades efficiency**, since information is transferred in a standardized form rather than one which is specific to an application's needs.
<!--
Identifiant sert à la fois identifier de manière unique un ressource dans le système ET exprimer la rélation avec d'autres ressources.
Exemple: un livre dans le bibliothèques, un livre preferé (qui peut être physiquement le même livre) d'une personne.

Données de contrôle - le but de message, l'action à effectuer
-->

---
transition: fade-out
---

<div class="grid grid-cols-2 gap-4">
<div>

## Contraintes d'interface uniforme
REST est défini par [quatre contraintes d'interface](https://www.ics.uci.edu/~fielding/pubs/dissertation/rest_arch_style.htm#sec_5_2) :
- identification des ressources
- manipulation des ressources via des représentations(messages)
- messages **auto-descriptifs**
- l'hyperlien comme moteur de l'état de l'application (HATEOAS)
</div>
<div>

## Messages REST

Le structure de message:
- identifiant
- representation de ressource (données)
- metadonnées de representation de ressource
- données de contrôle (décrivant le but du message)




</div>
</div>
---
transition: fade-out
---
# Conventions

Representation de ressource:
- un nom  (pas un verbe) en pluriel
- dans l'ordre hierarchique d'appartenance
- en kebab case

--> exemples ici

## L'ensemble des données identifiables

--> exemples ici

---
transition: fade-out
---
# Identifiant de ressource

---
transition: fade-out
---
# References

---
layout: end
---

