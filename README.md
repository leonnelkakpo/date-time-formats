# Date Time Formats and interoperability in software systems

## What about date time, time zone and formats

- Date & Heure: coordonnées temporelles (pour le réperage dans le temps)

- Les **fuseaux horaires**: kesako ?  
  L'heure est une coordonnée temporelle d'un instant de la journée. Elle est normalement
relative à la position du soleil par rapport à l'emplacement (**heure solaire**).  

```
L'heure "vraie" (aussi appelée "heure solaire") est définie géométriquement de la façon suivante:
il est midi vrai (=12h00) lorsque le soleil est exactement situé dans le plan méridien du lieu
considéré.
```

- **Difficultés avec l'heure solaire à partir 19ième siècle (industrialisation, le tranpsort, le commerce):** multitude d'heures locales à travers une région (Amerique du Nord environs 300 heures locales)

- **Solutions**: proposer une "uniformisation" (choisir une référence, Greenwich, ... ) GMT --> UTC

## Time marks

### GMT

- Division de la terre en 24 zones de temps (--> +1 ; <--- -1);
- Référence: Greenwich

### UTC

- Temps Universel (TU)
- Temps Atomique International (TAI)

## What's the problem with software systems ?

## Standards

Les standards doivent permettre "d'uniformiser" la répresentation du temps sans ambiguité.

### RFC 3339

```
2019-10-12T07:20:50.52Z
```

- **T** est utilisé pour séparer la date de l'heure
- **T** peut être remplacé par un espace
- **Z** définit la zone de temps (fuseau horaire), Z: __Zulu__  
  `Z ==> UTC+0`

### ISO 8601

```
2019-10-12T07:20:50.52Z
```

### Timestamp

- C'est quoi l'**epoch** ? 
- Le timestamp ?
- Pourquoi ?
- Le timestamp peut-il être négatif ? :cowboy_hat_face:

## Bug 2038


## Conclusion

Vous êtes:

- RFC339 ?
- ISO8601 ?
- POSIX ?