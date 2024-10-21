# Enzyme - Operators

## Braces "{}"

Les accolades `{}` servent de délimiteurs polyvalents dans Enzyme. Voici les principales utilisations :

1. **Délimiteurs de Blocs de Code** : Les accolades délimitent les blocs de code, telles que les corps de fonctions, de boucles, de conditions, et plus encore.
2. **Définition de Alkaloids** : Les accolades définissent les champs à l'intérieur d'un alkaloid.
3. **Expressions en Blocs** : Les accolades peuvent encapsuler des expressions dans un bloc, permettant des déclarations multiples avant de retourner une valeur.
4. **Formatage** : Les accolades `{}` sont utilisées dans les macros de formatage pour insérer des valeurs dans des chaînes.

## Examples

### EXAMPLE - REACTION
Les accolades délimitent le corps d'une ***reaction***.
```enzyme
async reaction: name() {
    // Corps de la reaction (function)
}
```

### EXAMPLE - ARGUMENTS
Les accolades délimitent les arguments passés à une ***reaction***.
```enzyme
async reaction: name({ argument1: Type, argument2: Type }) {
    // Corps de la reaction (function)
}
```

### EXAMPLE - ALKALOID
Les accolades délimitent les champs d'un alkaloid.
```enzyme
alkaloid: Name {
    // Champs de l'alkaloid
}
```

### EXAMPLE - EXPRESSIONS EN BLOCS
Les accolades délimitent les expressions de blocs
```enzyme
result = {
    let a = 1;
    let b = 2;
    a + b // La valeur de l'expression est retournée
};
```

### EXAMPLE - CONDITIONS 
Les accolades délimitent le corps des conditions.
```enzyme
if (condition) {
    // Code à exécuter si la condition est vraie
} else {
    // Code à exécuter si la condition est fausse
}
```
