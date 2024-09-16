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
ssh-keygen -t rsa -b 4096 -C "tucorreo@gmail.com"
```
Se generar 2 keys SSH `id_rsa` *key privada* y `id_rsa.pub` *key publica*, las cuales quedan guardadas en la carpeta .ssh

- Opcion alternativa NO Usar
```css
ssh-keygen -t ed25519 -C "tucorreo@gmail.com"
```

3. Correr Agente-ssh en GitBash
- $ eval "$(ssh-agent -s)"

4. Agregar key privada en GitBash
- $ ssh-add ~/.ssh/id_rsa
