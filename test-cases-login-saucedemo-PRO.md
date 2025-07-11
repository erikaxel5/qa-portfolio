# 🧪 Casos de Prueba – Login (SauceDemo) – Formato Profesional
**URL de prueba:** https://www.saucedemo.com  
**Tester:** Axel Spina  
**Fecha:** 2025-07-11  

---

## ✅ TC-001 – Login exitoso con usuario válido

- **Tipo de prueba:** Funcional – Positiva  
- **Prioridad:** Alta  
- **Severidad (si falla):** Alta  
- **Estado del test:** ✔️ Pasó  
- **Dispositivo:** MacBook Pro (13", 2016)  
- **Navegador:** Google Chrome 115.0.5790.102  
- **Sistema operativo:** macOS Catalina 10.15.7  

**Pasos:**
1. Acceder a https://www.saucedemo.com  
2. Introducir usuario: `standard_user`  
3. Introducir contraseña: `secret_sauce`  
4. Pulsar el botón “Login”

**Resultado esperado:**  
Redirige a /inventory.html y carga la lista de productos

**Resultado real:**  
Correcto. Página de productos cargada con éxito

---

## ❌ TC-002 – Bug real: usuario bloqueado no puede entrar

- **Tipo de prueba:** Funcional – Negativa  
- **Prioridad:** Alta  
- **Severidad:** Alta  
- **Estado del test:** ❌ Falló  
- **Dispositivo:** MacBook Pro (13", 2016)  
- **Navegador:** Google Chrome 115.0.5790.102  
- **Sistema operativo:** macOS Catalina 10.15.7  

**Pasos:**
1. Acceder a https://www.saucedemo.com  
2. Usuario: `locked_out_user`  
3. Contraseña: `secret_sauce`  
4. Pulsar el botón “Login”

**Resultado esperado:**  
Mostrar mensaje de error visible con información clara sobre bloqueo del usuario

**Resultado real:**  
Mensaje confuso: `"Epic sadface: Sorry, this user has been locked out."`  
Además, icono de error se superpone con el campo password (mala alineación visual)  
🔴 **Bug visual + texto poco claro para usuarios no técnicos**

---

## ❌ TC-003 – Campos vacíos

- **Tipo de prueba:** Negativa  
- **Prioridad:** Alta  
- **Severidad:** Alta  
- **Estado del test:** ✔️ Pasó  
- **Dispositivo:** MacBook Pro (13", 2016)  
- **Navegador:** Google Chrome 115.0.5790.102  
- **Sistema operativo:** macOS Catalina 10.15.7  

**Pasos:**
1. Acceder a https://www.saucedemo.com  
2. Dejar usuario y contraseña vacíos  
3. Pulsar “Login”

**Resultado esperado:**  
Mensaje: `"Username is required"`

**Resultado real:**  
Correcto, mensaje aparece y desaparece tras recargar

---

## ✅ TC-004 – Contraseña vacía

- **Tipo de prueba:** Negativa  
- **Prioridad:** Alta  
- **Severidad:** Media  
- **Estado del test:** ✔️ Pasó  
- **Dispositivo:** MacBook Pro (13", 2016)  
- **Navegador:** Google Chrome 115.0.5790.102  
- **Sistema operativo:** macOS Catalina 10.15.7  

**Pasos:**
1. Introducir `standard_user` como usuario  
2. Dejar contraseña vacía  
3. Pulsar “Login”

**Resultado esperado:**  
Mensaje: `"Password is required"`

**Resultado real:**  
Correcto

---

## 🟡 TC-005 – Login con espacios extra

- **Tipo de prueba:** Exploratoria  
- **Prioridad:** Baja  
- **Severidad:** Media  
- **Estado del test:** ✔️ Pasó  
- **Dispositivo:** MacBook Pro (13", 2016)  
- **Navegador:** Google Chrome 115.0.5790.102  
- **Sistema operativo:** macOS Catalina 10.15.7  

**Pasos:**
1. Usuario: `" standard_user "` (con espacios al principio y final)  
2. Contraseña: `" secret_sauce "`  
3. Pulsar “Login”

**Resultado esperado:**  
Sistema debería eliminar espacios o mostrar error

**Resultado real:**  
Login funciona igual → el sistema **recorta espacios automáticamente**  
🔍 No es un bug, pero comportamiento confirmado

---
