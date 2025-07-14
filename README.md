steps to install Web3 modules in Termux.

1. Install Rust dan Binutils

```bash
pkg install -y rust binutils
````

2. Install Maturin

```bash
CARGO_BUILD_TARGET="$(rustc -Vv | grep "host" | awk '{print $2}')" pip install maturin
```

3. Install Web3

```bash
pip install web3
```

4. Install all Modules requirements.txt

```bash
pip install -r requirements.txt
```

