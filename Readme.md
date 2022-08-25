# BULKOR

The source codes of BULKOR

## Requirements

Ubuntu 18.04, Intel SGX SDK 2.14, and Rust toolchain

## Compilation and Run


```
cd server
```

### For 1024B block evaluation

```
./execute.sh
```

### For 64B block evaluation 

```
git apply 1024B_to_64B.patch
./execute.sh
```
