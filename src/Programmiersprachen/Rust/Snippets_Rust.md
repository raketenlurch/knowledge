# Snippets
Code-Schnipsel zum Wiederverwenden.

## Command-line
### Parse command-line arguments
**Numbers**
```Rust
fn get_number() -> usize {
    let mut buffer = String::new();
    let stdin = std::io::stdin();

    stdin.read_line(&mut buffer).expect("BROKEN STDIN");

    let input = buffer.trim();

    input.parse().expect("Peng")
}
```

**Strings**
```Rust
fn get_string() -> String {
    let mut buffer = String::new();
    let stdin = std::io::stdin();

    stdin.read_line(&mut buffer).expect("BROKEN STDIN");

    let input = buffer.trim();

    input.parse().expect("Peng")
}
```

## Strings
**Reverse String**
```Rust
fn reverse(input: &str) -> String {
    let reversed_string = input.chars().rev().collect();

    reversed_string
}
```