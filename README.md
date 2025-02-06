# pwnhash

A Bash script or set of functions for your `.bashrc` or `.zshrc` to crack hashes using the [ntlm.pw API](https://ntlm.pw/docs).

## Usage
```
pwnhash <hash_type> (<hash_value> | -f <hash_file>)
````
### Parameters:
- `<hash_type>`: Specify the type of hash you want to crack. Supported hash types are:
  - nt
  - lm
  - md5
  - sha1
  - sha256

- `<hash_value>`: Provide the hash value directly to attempt cracking it.

- `-f <hash_file>`: Use this option to specify a file containing a list of hashes (one per line) to be processed.

## Install in bashrc
To integrate the `pwnhash` function into your terminal session, run he following:

```bashrc```
```
wget -qO- https://raw.githubusercontent.com/Cyb3rGh0st-Team/pwnhash/refs/heads/main/pwnhash_bashrc_function | tee -a ~/.bashrc && source ~/.bashrc
```

```zshrc```
```
wget -qO- https://raw.githubusercontent.com/Cyb3rGh0st-Team/pwnhash/refs/heads/main/pwnhash_bashrc_function | tee -a ~/.zshrc && source ~/.zshrc
```
