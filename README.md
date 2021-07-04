# Configuracion para nvim

esta es mi configuracion para neo vim, yo uso este editor en windows asi que los siguientes pasos son para dicha plataforma. Recomiendo usar PowerSell desde _administrador_

## 1.- instalacion neo vim

utilisaremon chocolatey para esta tarea

```
choco install neovim -y
```

### 2.- instalacion de Plug

esta es el instalador de plugins que uso en mi configuracion

```
iwr -useb https://raw.githubusercontent.com/junegunn/vim-plug/master/plug.vim |`
    ni "$(@($env:XDG_DATA_HOME, $env:LOCALAPPDATA)[$null -eq $env:XDG_DATA_HOME])/nvim-data/site/autoload/plug.vim" -Force
```

### 3.- Ahora si configuramos

vamos a la direccion >C:\Users\@usuario\AppData\Local\nvim

alli pegamos esta carpeta, abrimos el archivo init.vim 
```
  nvim init.vim
```

corremos el siguiente comando desde neovim
```
  :PlugInstall
```

_ya esta luego creo un archivo indicando mis atajos de teclado_

