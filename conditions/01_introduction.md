# Introduction aux conditions - if, else et else if

Voici ci-dessous comment s'écrivent les conditions de base en Java.

```java
if (condition) {...}
else {...}
```
**/!\ Le `else` est obligatoirement précédé par un `if`**

Voici la signification de ces deux mots-clés de condition en français.
```properties
if = si
else = sinon
```

L'imbrication de conditions dans les blocs de code d'autres conditions est, bien entendu, tout à fait possible:
```java
if (condition1) {
  if (condition2) {...}
  else {...}
} else {
  if (condition3) {...}
  else {...}
}
```

Certains cas se prêtent cependant à l'utilisation du `else if`, c'est-à-dire un `else` et `if` *collés* ensemble. "Sinon si", en français.
```java
else if (condition) {...}
```

Cette structure permet donc d'avoir une suite de conditions infinie, comme ci-dessous.
```java
if (condition1) {...}
else if (condition2) {...}
else if (condition3) {...}
else if (condition4) {...}
else if (condition5) {...}
[...]
else {...}
```
A noter cependant que ce genre de situation pourrait préférablement être remplacé par un `switch`, que nous étudierons plus tard, et ce pour faciliter la compréhension du code.
