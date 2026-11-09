You can install Rust directly through **Homebrew** on macOS.

### 1. Install Rust

Open Terminal:

```bash
brew install rust
```

### 2. Verify installation

```bash
rustc --version
cargo --version
```

### 3. Check Rust installation path

```bash
which rustc
which cargo
```

### 4. Create a Rust project

```bash
cargo new shopping_calculator
cd shopping_calculator
```

### 5. Compile and run

```bash
cargo build
cargo run
```

### 6. Build optimized executable

```bash
cargo build --release
```

Run:

```bash
./target/release/shopping_calculator
```

### 7. Update Rust

```bash
brew update
brew upgrade rust
```

### Add these instructions to the top of your Rust file

```rust
/*
=========================================================
           RUST INSTALLATION - HOMEBREW
=========================================================

INSTALL HOMEBREW:
https://brew.sh

INSTALL RUST:
brew install rust

VERIFY:
rustc --version
cargo --version

CHECK PATH:
which rustc
which cargo

CREATE PROJECT:
cargo new shopping_calculator
cd shopping_calculator

COMPILE:
cargo build

OPTIMIZED COMPILE:
cargo build --release

RUN:
cargo run

RUN RELEASE:
cargo run --release

EXECUTE:
./target/release/shopping_calculator

UPDATE:
brew update
brew upgrade rust

=========================================================
*/
```

**Official resources:**
-  [oai_citation:0‡brew.sh](https://brew.sh/?utm_source=chatgpt.com)
-  [oai_citation:1‡rust-lang.org](https://www.rust-lang.org/?utm_source=chatgpt.com)

Would you like to use **Homebrew exclusively** for managing your Rust toolchain, or install `rustup` alongside it?

This means Homebrew installed Rust, but your system is currently using **rustup**, which doesn't have a default Rust toolchain configured.

### 1. Fix the error

Run this in Terminal:

```bash
rustup default stable
```

This downloads and configures the latest stable Rust toolchain.

### 2. Verify installation

```bash
rustc --version
cargo --version
rustup show
```

### 3. Test compilation

Create a test file:

```bash
nano hello.rs
```

Paste:

```rust
fn main() {
    println!("Rust is working!");
}
```

Compile:

```bash
rustc hello.rs -o hello
```

Execute:

```bash
./hello
```

Expected output:

```text
Rust is working!
```

### 4. Check which Rust installation you're using

```bash
which rustc
which cargo
which rustup
```

**My recommendation:** Since rustup is already installed and being invoked, use it to manage Rust versions. You can still use Homebrew for other development tools.

Official documentation:  [oai_citation:0‡rust-lang.github.io](https://rust-lang.github.io/rustup/?utm_source=chatgpt.com)

**What would you prefer next?**


