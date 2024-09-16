# GIT y GITHUB Referencia rapida

### Configuracion Inicial
``` css
git config --global user.name "tunombre"
git config --global user.email tucorreo
git config --global core.editor "code --wait"
git config --global core.autocrlf true
```
### Verificar configuracion
``` css
git config --list
```

## Configuracion SSH

1. Verificar si existe un ssh
```css
ls -al ~/.ssh
```

2. Generar una key ssh
```css
ssh-keygen -t ed25519 -C "rimar.basaa@gmail.com"
```

- $ ssh-keygen -t rsa -b 4096 -C "rimar.basaa@gmail.com"
// id_rsa: key privada (mia)
// id_rsa.pub: key publica

3. Correr Agente-ssh en GitBash
- $ eval "$(ssh-agent -s)"

4. Agregar key privada en GitBash
- $ ssh-add ~/.ssh/id_rsa
