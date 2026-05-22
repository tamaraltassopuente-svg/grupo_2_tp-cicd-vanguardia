# 📋 Pasos para subir a GitHub

## Antes de empezar: instalar Git
1. Ir a https://git-scm.com/download/win
2. Descargar el instalador y ejecutarlo (siguiente, siguiente, finalizar)
3. Reiniciar VS Code después de instalarlo

---

## Paso 1: Abrir esta carpeta en VS Code
- Abrí VS Code
- Archivo → Abrir Carpeta → buscá esta carpeta: `grupo_2_tp-cicd-vanguardia`

## Paso 2: Abrir la terminal en VS Code
- Apretá `Ctrl + `` ` (la tecla debajo de Escape)
- Se abre una terminal negra abajo

## Paso 3: Configurar Git (solo la primera vez)
Escribí estos dos comandos (uno por uno, apretando Enter después de cada uno):

```
git config --global user.name "Tu Nombre"
git config --global user.email "tu-email@gmail.com"
```

## Paso 4: Inicializar Git en la carpeta
```
git init
git add .
git commit -m "Primer commit del proyecto"
```

## Paso 5: Conectar con GitHub y subir
```
git branch -M main
git remote add origin https://github.com/TU_USUARIO_GITHUB/grupo_2_tp-cicd-vanguardia.git
git push -u origin main
```
⚠️ Reemplazá TU_USUARIO_GITHUB con tu usuario de GitHub

## Paso 6: Ver el workflow en GitHub
1. Entrá a tu repo en github.com
2. Hacé clic en la pestaña "Actions"
3. Vas a ver el workflow corriendo → tiene que aparecer ✅ verde

## Paso 7: Para la Actividad 7 (hacer un cambio y verificar)
Modificá una línea del README.md, guardá, y ejecutá:
```
git add .
git commit -m "Prueba pipeline CI/CD"
git push
```
Volvé a la pestaña Actions en GitHub y vas a ver que se disparó solo.
