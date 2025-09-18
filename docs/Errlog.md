# ErrorLog
## p.70 cargo clipy
```sh
shu8cream@shupad:~/repo/wasabi$ cargo clippy
    Checking wasabi v0.1.0 (/home/shu8cream/repo/wasabi)
error: language item required, but not found: `eh_personality`
  |
  = note: this can occur when a binary crate with `#![no_std]` is compiled for a target where `eh_personality` is defined in the standard library
  = help: you may be able to compile for a target that doesn't need `eh_personality`, specify a target with `--target` or in `.cargo/config`

error: could not compile `wasabi` (bin "wasabi") due to 1 previous error
```

add .cargo/config.toml