
---

# Handling differents development environments

---

## context

---

## context

- project A: Java 8 + maven 3.3 

---

## context
- project A: Java 8 + maven 3.3 
- project B: Java 11 + maven 3.3 

---

## context
- project A: Java 8 + maven 3.3 
- project B: Java 11 + maven 3.3 
- project C: Scala 12.11 
- project D: Rust 1.67.0
- project E: Python 3.11 

---

## context
- project A: Java 8 + maven 3.3 
- project B: Java 11 + maven 3.3 
- project C: Scala 12.11 
- project D: Rust 1.67.0
- project E: Python 3.11 
<br><br>
- how to handle this ?

---

## workaround

---

## workaround
- install everything on my machine

---

## workaround
- install everything on my machine


```bash
echo $PATH
```

---

## workaround
- install everything on my machine


```bash
echo $PATH
```

- 💥 

---

## workaround
- yolo ! install everything on my machine ❌
- use one environment per project: 

---

## workaround
- yolo ! install everything on my machine ❌
- use one environment per project: 
    - [Sdkman](https://sdkman.io/)
    - [Pyenv](https://github.com/pyenv/pyenv)
    - ...

---

## tools

---

## tools
### direnv

[](https://direnv.net/)

direnv is an extension for your shell. It augments existing shells with a new feature that can load and unload environment variables depending on the current directory.

---

## tools
### direnv

[](https://direnv.net/)

direnv is an extension for your shell. It augments existing shells with a new feature that can load and unload environment variables depending on the current directory.

```bash
mkdir ~/my-project && cd ~/my-project/ && echo ${FOO-nope}
```
---

## tools
### direnv
- direnv improves the developer workflow 👍

---

## tools
### direnv
- direnv improves the developer workflow 👍
- different versions of the same sdks need to be installed 👎 

---

## tools
### nix

---

## tools
### nix-direnv
