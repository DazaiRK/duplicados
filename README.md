# Detección de Duplicados en Tickets

Este repositorio contiene un archivo con **dos funciones** relacionadas con la validación y detección de duplicados en tickets digitales.

El objetivo principal es **modificar y optimizar la segunda función** siguiendo las pautas que se detallan a continuación.

---

## 📌 Tareas a realizar

1. **Agregar un disparador (trigger)**  
   - La segunda función debe incorporar un disparador igual al que ya existe en la primera función.  
   - Esto asegura que la función se ejecute de manera automática bajo las mismas condiciones.

2. **Optimizar la lógica de detección de duplicados**  
   La función debe evaluar los tickets según los siguientes criterios:

   - **Coincidencia exacta de campos claves**  
     - Si todos los campos claves son **iguales en un 100%**, el ticket debe marcarse como **duplicado** inmediatamente.

   - **Coincidencia parcial de campos claves (≥ 85%)**  
     - Si los campos claves son **similares** (superan un 85% de coincidencia), entonces:
       1. **Comparar el total**  
          - Si el total es **exactamente igual**, se considera **el mismo ticket**.  
       2. **Si el total difiere**, revisar los **productos**:  
          - Si los productos son equivalentes (según la lógica definida), se considera duplicado.  
          - Si no, se descarta como duplicado.

3. **Mejorar performance y legibilidad**  
   - Optimizar los cálculos de similitud para que la función sea más eficiente.  
   - Asegurar que el código tenga **comentarios claros** y sea fácil de mantener.

---

## ⚙️ Estructura del repositorio

