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

### For fully in-enclave evaluation

change the value of `TREETOP_CACHING_THRESHOLD_LOG2` in `server/enclave/src/oram_storage/mod.rs` from `24` to `24u32-1u32.log2()`
then `./execute.sh`

