FFTPACK 5.1 GPL Version

## Get Start
```bash
git clone https://github.com/fortran-fans/fftpack5.1-GPL.git
cd fftpack5.1-GPL
```
### Supported Compilers
The following combinations are tested on the default branch of `fftpack`:  
|Name|Vesrion|Platform|Architecture|  
|---|---|---|---|  
|GCC Fortran(MSYS2)|10.3|Windows 10|x86_64|

## Build with FPM
You can build using provided `fpm.toml`: 
```
fpm build --flag "-fallow-argument-mismatch"
fpm test --flag "-fallow-argument-mismatch"
```
You can use this package in your fpm porject, notice it is **with a GPL License**.  
Add the following to your fpm project `fpm.toml`.
```toml
[dependencies]
fftpack = { git="https://github.com/fortran-fans/fftpack5.1-GPL.git" }
```