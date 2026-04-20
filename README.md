[![Review Assignment Due Date](https://classroom.github.com/assets/deadline-readme-button-22041afd0340ce965d47ae6ef1cefeee28c7c493a6346c4f15d667ab976d596c.svg)](https://classroom.github.com/a/0V8i2zWk)
[![Open in Visual Studio Code](https://classroom.github.com/assets/open-in-vscode-2e0aaae1b6195c2367325f4f02e2d04e9abb55f0b24a779b69b11b9e10269abc.svg)](https://classroom.github.com/online_ide?assignment_repo_id=23618646&assignment_repo_type=AssignmentRepo)
# Laboratorio 04: Visualización de Datos en Raspberry Pi con Node-RED

## Integrantes

| Campo | Detalle |
|---|---|
| Integrante 1 | David Santiago Guarin |
| Integrante 2 | Juan David Jiménez |
| Integrante 3 | Santiago Montaño Suárez |
| Carrera | Ingeniería Electrónica |
| Fecha | Abril de 2026 |

---

## 1. Introducción

Este repositorio contiene la solución al Laboratorio 04, enfocado en el uso de **Node-RED** para el diseño de flujos de datos. El objetivo principal es la integración de nodos de interfaz de usuario (Dashboard), procesamiento lógico mediante JavaScript y la gestión de almacenamiento local para el registro de eventos.

---

## 2. Descripción del Procedimiento

Para la realización de esta práctica, se diseñó un flujo que permite la interacción en tiempo real y el almacenamiento de datos. El procedimiento se dividió en las siguientes etapas:

### 2.1 Configuración del Entorno

Se instalaron las dependencias necesarias de `node-red-dashboard` para habilitar los nodos de interfaz gráfica.

### 2.2 Implementación del Flujo

Se arrastraron y conectaron los siguientes nodos según el esquema técnico solicitado:

- **Color Picker:** Actúa como el nodo de entrada principal, permitiendo al usuario seleccionar un color.
- **Debug:** Configurado para monitorear las salidas en la consola de depuración y validar que el `msg.payload` contenga el valor esperado.
- **Function:** Nodo intermedio donde se aplica lógica personalizada (por ejemplo, añadir una estampa de tiempo o formatear el mensaje).
- **Text Input:** Utilizado para visualizar la entrada procesada directamente en el Dashboard.
- **Write File:** Configurado para escribir los datos recibidos en un archivo local, asegurando la persistencia de la información.

---

## 3. Documentación

<!-- Incluir diagramas y adjuntar al repositorio, en una carpeta src, el flujo que crearon -->

### 3.1 Diagrama del Flujo Principal

> _Adjuntar diagrama del flujo Node-RED aquí_

### 3.2 Capturas del Dashboard

> _Adjuntar capturas de pantalla del Dashboard aquí_

> **Nota:** Los archivos `.json` del flujo exportado se encuentran en la carpeta `src/` del repositorio.

---

## 4. Resultados Obtenidos

1. **Interconectividad:** Se logró una comunicación fluida entre el selector de color y los actuadores virtuales (texto y archivo).
2. **Validación de Datos:** Mediante el nodo Debug, se confirmó que los valores hexadecimales/RGB se transmiten correctamente al nodo de función.
3. **Almacenamiento Local:** Se verificó la creación de un archivo en el sistema de archivos local, donde cada interacción con el selector de color queda registrada de manera secuencial.

---

## 5. Conclusiones

La práctica demuestra la eficiencia de Node-RED para el prototipado rápido de sistemas de control. La capacidad de integrar lógica de programación en nodos de función junto con nodos de entrada/salida físicos o virtuales (como el guardado de archivos) es fundamental para desarrollar soluciones robustas en el ámbito de la automatización y el monitoreo de datos.

<!-- Espacio para conclusiones adicionales del equipo -->

---

*David Santiago Guarin • Juan David Jiménez • Santiago Montaño Suárez*  
*Ingeniería Electrónica • Abril 2026*