# GIT y GITHUB Referencia rapida

## Configuracion Inicial
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
---
## Configuracion SSH
### Configuracion en mi maquina

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
```css
eval "$(ssh-agent -s)"
```

4. Agregar key privada en GitBash
```css
ssh-add ~/.ssh/id_rsa
```
### Configuracion en mi Github

1. Copiar el contenido de la key publica `id_rsa.pub` al portapapeles
```css
clip < ~/.ssh/id_rsa.pub
```
2. Entrar a nuestra cuenta de Github he ir a:
   
[1]Setting --> [2]SSH and GPG Keys --> [3]New SSH Key

   ![screenssh00](https://github.com/rimardev/referencia-frontend/blob/main/img/set-github-ssh00.jpg)

3. En este formulario llenar con lo siguiente:
   - [4]Poner un Titulo Identificatorio
   - [5]Copiar el contenido del portapapeles
   - [6]Hacer click en `Add SSH Key`

   ![screenssh01](https://github.com/rimardev/referencia-frontend/blob/main/img/set-github-ssh01.jpg)

### Verificar conexion entre Repositorio Local y Remoto
1. En Gitbach ejecutar el comando
```css
git remote -v
/*resultado
origin  git@github.com:rimardev/referencia-frontend.git (fetch)
origin  git@github.com:rimardev/referencia-frontend.git (push)
*/
```
2. Comparar en Github si es la misma url

![screenssh02](https://github.com/rimardev/referencia-frontend/blob/main/img/set-github-ssh02.jpg)
