# 🧪 Test Cases – Login Functionality (SauceDemo)
**Aplicación:** https://www.saucedemo.com  
**Módulo:** Login  
**Fecha de creación:** 2025-07-11  
**Tester:** Axel Spina  
---

## 📋 Lista de Casos de Prueba

| ID       | Título                                             | Tipo         | Prioridad | Resultado Esperado                                           |
|----------|----------------------------------------------------|--------------|-----------|--------------------------------------------------------------|
| TC-001   | Login exitoso con usuario válido                   | Positivo     | Alta      | Accede a /inventory.html                                     |
| TC-002   | Login con usuario bloqueado                        | Positivo     | Alta      | Muestra mensaje de error de usuario bloqueado               |
| TC-003   | Login con usuario problemático                     | Positivo     | Media     | Accede con errores visuales                                  |
| TC-004   | Login con usuario lento (performance)              | Positivo     | Media     | Accede con retardo                                           |
| TC-005   | Usuario válido, contraseña incorrecta              | Negativo     | Alta      | Muestra mensaje de error de credenciales                     |
| TC-006   | Usuario incorrecto, contraseña válida              | Negativo     | Alta      | Muestra mensaje de error de credenciales                     |
| TC-007   | Usuario y contraseña incorrectos                   | Negativo     | Alta      | Muestra mensaje de error de credenciales                     |
| TC-008   | Usuario y contraseña vacíos                        | Negativo     | Alta      | Muestra error: Username is required                          |
| TC-009   | Usuario vacío, contraseña válida                   | Negativo     | Alta      | Muestra error: Username is required                          |
| TC-010   | Usuario válido, contraseña vacía                   | Negativo     | Alta      | Muestra error: Password is required                          |
| TC-011   | Verificar visibilidad de campos login              | UI/Visual    | Media     | Campos username y password visibles                          |
| TC-012   | Verificar botón login habilitado                   | UI/Visual    | Media     | Botón habilitado tras ingresar datos                         |
| TC-013   | Verificar comportamiento del mensaje de error      | UI/Visual    | Media     | Mensaje visible y desaparece tras recargar                   |
| TC-014   | Verificar funcionalidad del botón cerrar error     | UI/Visual    | Media     | Botón (X) cierra mensaje de error                            |
| TC-015   | Login con espacios extra en credenciales           | Exploratorio | Baja      | El sistema debe limpiar espacios o mostrar error             |
| TC-016   | Login con caracteres especiales                    | Exploratorio | Media     | Muestra mensaje de error                                     |
| TC-017   | Navegación con teclado (Tab y Enter)               | Exploratorio | Media     | Se puede navegar y hacer login sin usar el ratón             |

---

**Nota:** Puedes ejecutar y documentar estos casos manualmente e ir marcando los resultados reales, capturas de pantalla o bugs detectados en un archivo adicional de reporte.
