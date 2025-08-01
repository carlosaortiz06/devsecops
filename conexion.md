# Conexión Segura a un Servidor Remoto mediante SSH con Clave Privada

Este documento describe los pasos para establecer una conexión SSH segura hacia un servidor remoto utilizando una clave privada.

---

## ✅ Requisitos Previos

- Tener instalada una herramienta de cliente SSH (`ssh`) en tu sistema.
- Disponer de una clave privada válida (por ejemplo, `vm.pem` o `id_rsa`).
- Conocer la IP pública o el hostname del servidor remoto.
- Tener el nombre de usuario remoto con privilegios de acceso (por ejemplo, `ubuntu`, `ec2-user`, `azureuser`, etc.).

---

## 🔐 Asignar Permisos Correctos a la Clave Privada

Para que la conexión SSH sea segura, la clave privada debe tener los permisos correctos:


chmod 400 ruta/a/tu/clave_privada.pem

## Conectarse al servidor

ssh -i ~/.ssh/clave.pem azureuser@20.123.45.67



