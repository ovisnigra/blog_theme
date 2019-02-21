---
layout: post
title: "apuntes git"
comments: false
description: "apuntes git"
keywords: "apuntes, git"
---

# instalar git (Debian based systems)

`sudo apt-get install git-all`

configurar

```
git config --global user.name "nombre_usuario"
git config --global user.email "correo-e"
```

# clonar repositorio

`git clone http…`

```
git config --global alias.s "status -s -b"
git config --global alias.lo "log --all --graph --decorate --oneline"
```

consultar/leer config
`git config --global -l`
