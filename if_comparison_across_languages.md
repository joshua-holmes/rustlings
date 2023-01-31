# `if` Comparison Across Languages

## Using normal if control flow
### JavaScript
```
let message = "";
if (is_success) {
    message = "HOORAY";
} else {
    message = "OOPS;
}
```

### Python
```
message = ""
if is_success:
    message = "HOORAY"
else:
    message = "OOPS"
```

### Rust
```
let mut message = "";
if is_success {
    message = "HOORAY";
} else {
    message = "OOPS";
}
```


## Using ternary operator so it can fit on one line
### JavaScript
```
const message = is_success ? "HOORAY" : "OOPS";
```

### Python
```
message = "HOORAY" if is_success else "OOPS"
```

### Rust
```
let message = if is_success { "HOORAY" } else { "OOPS" };
```

## In Rust, `if` is an expression, not a statement, which means it returns a value. So this works in Rust:
### Rust only
```
let message = if is_success {
    message = "HOORAY"
} else {
    message = "OOPS"
};
```
