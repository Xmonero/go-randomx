# go-randomx

## Build

### Windows

Firstly download and install the msys2, then open and install the following components:

Take msys2's pacman for example

```bash
pacman -Syu
pacman -S git mingw64/mingw-w64-x86_64-go mingw64/mingw-w64-x86_64-gcc mingw64/mingw-w64-x86_64-cmake mingw64/mingw-w64-x86_64-make
```

Secondly clone this repo to your project folder
```
cd MyProject
git clone https://github.com/maoxs2/go-randomx
```

And then run `go generate` to auto compile official random-x code 
```bash
go generate # will clone and compile RandomX source code into librandomx
```

Finally you can using the package as your internal one. 

Directly using it with `import "github.com/MyProject/go-randomx"` and then `randomx.AllocCache()` etc.

### Linux

Take Ubuntu for example 

Download the latest go from [here](https://golang.org/dl/) and then install it following [this instruction](https://golang.org/doc/install#tarball)
```bash
sudo apt update && sudo apt upgrade 
sudo apt install git cmake make gcc build-essential
```

Secondly clone this repo to your project folder
```
cd MyProject
git clone https://github.com/maoxs2/go-randomx
```

And then run `go generate` to auto compile official random-x code 
```bash
go generate # will clone and compile RandomX source code into librandomx
```

Finally you can using the package as your internal one. 

Directly using it with `import "github.com/MyProject/go-randomx"` and then `randomx.AllocCache()` etc.
