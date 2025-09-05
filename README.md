Guía rápida para usar el proyecto:

0) Requisitos
Node.js (recomendado LTS 18+).
Git instalado.
Permitir ICMP/ping en la red (algunos firewalls lo bloquean y daría “FALLA” falso).

1) Clonar el repositorio
git clone https://github.com/mdduran9/monitoreo_conectividad.git
cd monitoreo_conectividad

2) Instalar dependencias
Si el repo ya trae package.json:
npm install

Si por algún motivo no existiera package.json, entonces:
npm init -y
npm i express cors ping

3) Configurar (opcional)
Por defecto escucha en el puerto 3000. Si quieres cambiarlo:

Windows (CMD/PowerShell):
set PORT=4000 && node server.js

Linux/Mac:
PORT=4000 node server.js

4) Ejecutar el servidor
npm start
ó
npm run start

Deberías ver algo como:

✅ Servidor corriendo en http://localhost:3000

5) Abrir el monitor en el navegador

Página principal: http://localhost:3000
API para ver el JSON: http://localhost:3000/status

6) Actualizar local con cambios del reposicion
   git pull origin main




