![Neovim logo](https://upload.wikimedia.org/wikipedia/commons/thumb/4/4f/Neovim-logo.svg/2560px-Neovim-logo.svg.png "Neovim logo")

# Configuracion para nvim

esta es mi configuracion para neo vim, yo uso este editor en windows asi que los siguientes pasos son para dicha plataforma. Recomiendo usar PowerSell desde _administrador_

## Antes de ir con neovim

para usar neovim en windows yo uso la app de terminal de su tienda y una guente que me gusta en lo personal
para la fuente hay que bajarla desde
```
https://github.com/ryanoasis/nerd-fonts
```
esta me gusta en especial
```
https://github.com/ryanoasis/nerd-fonts/tree/master/patched-fonts/FiraCode
```

y se instala con un simple click

mi configuracion de windows terminal es

```
 "profiles":
    {
        "defaults":
        {
            // Put settings here that you want to apply to all profiles.
            "useAcrylic": true,
            "acrylicOpacity": 0.70,
            "fontFace" : "Fira Code"
```

##  instalacion neo vim

utilisaremon chocolatey para esta tarea

```
choco install neovim -y
```

### instalacion de Plug

esta es el instalador de plugins que uso en mi configuracion

```
iwr -useb https://raw.githubusercontent.com/junegunn/vim-plug/master/plug.vim |`
    ni "$(@($env:XDG_DATA_HOME, $env:LOCALAPPDATA)[$null -eq $env:XDG_DATA_HOME])/nvim-data/site/autoload/plug.vim" -Force
```
### Antes de configurar instalamos esto
```
pip2 install pynvim
pip3 install pynvim
npm install -g neovim
```
### Ahora si configuramos

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

