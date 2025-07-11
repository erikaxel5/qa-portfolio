# 🧪 Test Cases – renfe.com – Formato Profesional
**Aplicación:** https://www.renfe.com  
**Tester:** Axel Spina  
**Fecha:** 2025-07-11  
**Dispositivo:** MacBook Pro (13", 2016)  
**Navegador:** Google Chrome 115.0.5790.102  
**Sistema operativo:** macOS Catalina 10.15.7  

---

## ✅ TC-001 – Búsqueda de trayecto válida

- **Tipo de prueba:** Funcional – Positiva  
- **Prioridad:** Alta  
- **Estado del test:** ✔️ Pasó  

**Pasos:**
1. Acceder a https://www.renfe.com  
2. Seleccionar origen: "Valencia Joaquín Sorolla"  
3. Seleccionar destino: "Madrid Puerta de Atocha"  
4. Elegir una fecha válida  
5. Pulsar "Buscar"

**Resultado esperado:**  
Se muestra una lista de trenes disponibles para la ruta y fecha elegidas.

**Resultado real:**  
La búsqueda funciona correctamente y se muestran los resultados.

---

## ❌ TC-002 – Búsqueda sin rellenar campos

- **Tipo de prueba:** Funcional – Negativa  
- **Prioridad:** Alta  
- **Estado del test:** ✔️ Pasó  

**Pasos:**
1. Acceder a https://www.renfe.com  
2. No seleccionar origen ni destino  
3. Pulsar "Buscar"

**Resultado esperado:**  
El sistema debe mostrar un mensaje de error indicando que faltan campos obligatorios.

**Resultado real:**  
Correcto, el sistema avisa de que se deben seleccionar origen y destino.

---

## ✅ TC-003 – Cambio de idioma a inglés

- **Tipo de prueba:** UI / Funcionalidad  
- **Prioridad:** Media  
- **Estado del test:** ✔️ Pasó  

**Pasos:**
1. Acceder a https://www.renfe.com  
2. Pulsar en el icono de idioma y seleccionar "English"

**Resultado esperado:**  
La web recarga y se muestra en idioma inglés.

**Resultado real:**  
Correcto, la web cambia al idioma inglés sin errores.

---

## ✅ TC-004 – Prueba de diseño responsive (modo móvil)

- **Tipo de prueba:** UI / Responsive  
- **Prioridad:** Media  
- **Estado del test:** ✔️ Pasó  

**Pasos:**
1. Acceder a https://www.renfe.com  
2. Simular resolución de móvil (modo responsive del navegador)  
3. Verificar si los elementos se adaptan correctamente

**Resultado esperado:**  
La web se adapta correctamente al formato móvil, sin solapamientos ni errores visuales.

**Resultado real:**  
Correcto, aunque algunas animaciones tardan en cargar, la estructura se adapta bien.

---

## ❌ TC-005 – Error visual: sección Renfe +

- **Tipo de prueba:** UI – Exploratorio  
- **Prioridad:** Baja  
- **Estado del test:** ⚠️ Bug visual detectado  

**Pasos:**
1. Acceder a https://www.renfe.com  
2. Ir a la sección “Renfe+” desde el menú principal  
3. Observar el comportamiento al hacer scroll

**Resultado esperado:**  
Se carga correctamente la página y el contenido se adapta a la vista

**Resultado real:**  
La imagen superior se desplaza mal en algunos navegadores y el texto se solapa con el fondo.  
🔴 **Bug visual: layout inconsistente en scroll**

---
