# ALKALOIDS
Un alkaloid est utilisé pour créer des types de données personnalisés dans Enzyme.

## EXAMPLES

### Example - Simple
Un **alkaloid** simple qui encapsule des champs de données. Les champs peuvent être partagés (publiques) ou secrets (privés).
```rust
alkaloid: Name {
    // CHAMPS PUBLIC WITH SHARE
    share first_name: String,
    // CHAMPS PRIVATE DEFAULT
    last_name: String,
}
```

### Example - Tuple
Un **alkaloid** tuple qui regroupe des valeurs sans nommer explicitement les champs. Utile pour des structures simple.
```rust
alkaloid: Name(type, type);
alkaloid: Name({ type | type | type | type });
```

### Example - Macros
```rust
#[derived()]
alkaloid: Name {}
```

### Example - Simple with lifetime 
```rust
alkaloid: Name#: 'lifetime {
  share first_name: String,
  share last_name: String,
}
```

### Example - Simple with lifetime and solvants
```rust
alkaloid: Name<{ /*SOLVANT*/ }>#: 'lifetime {
  share first_name: String,
  share last_name: String,
}
```

### Example - Simple with lifetime and macros
```rust
#[derived()]
alkaloid: Name<{ /*SOLVANT*/ }>#: 'lifetime {
  share first_name: String,
  share last_name: String,
}
```