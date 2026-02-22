# NIH-Plug-VST3

Please see [the original repo](https://github.com/robbert-vdh/nih-plug) for more information.

This is a fork of a fork of a fork (no joke) to merge a branch to master that adds support for the [vst3](https://crates.io/crates/vst3) crate that is licensed under the MIT license. This eliminates preexisting GPL contamination of built plugins using the otherwise ISC-licensed framework. This is all possible because the VST3 SDK was [relicensed](https://ocl-steinberg-live.steinberg.net/_storage/asset/819253/storage/master/Press%20Release%20-%202025-10-29%20-%20VST%203.8%20-%20EN.pdf) to the MIT license. The [old VST3 crate](https://micahrj.github.io/posts/vst3/) was also licensed under GPL to remain compliant, but the new version of the crate was updated to reflect the license change to MIT. **So, in short, this repo allows you to build VST3 plugins without having to employ the GPL license for built binaries (or source code, if applicable).**

You can use this version of NIH-Plug like so:

```toml
[dependencies]
nih_plug = { git = "https://github.com/EuphoricPenguin/nih-plug-vst3", features = ["vst3"] }
```
