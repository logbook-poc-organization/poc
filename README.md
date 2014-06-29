Proof Of Concept
===
Offrir un journal de bord collaboratif simple, intuitif, rapide.

Il y a deux aspects fondamentaux:
* enregistrer une entrée aisement
* retrouver une liste d'entrées suivant plusieurs critères

Features
========

* authentification par SSO
* différenciation backend / frontend nette
** capacité à décliner le frontal par préférence

Backend
-------
Résolument une base NoSQL type document (mongoDB par exemple)
Chaque document doit comprendre
```javascript
{
  __id:  '110E8400-E29B-11D4-A716-446655440000',
  author: { mail: 'jean.gabin@nowhere', idp: 'monidp'},
  times : { start: ..., end: ... }
  object_tags : [ 'server0', 'application1', 'database2'],
  category_tags : ['update','sql'],
  data : {
    html_content: { "...." },
    binaries : {
      ...  
    }
  }
}
```
La liste des propriétés doit répondre à 
* qui ?
* quand ?
* où ?
* quoi ?

