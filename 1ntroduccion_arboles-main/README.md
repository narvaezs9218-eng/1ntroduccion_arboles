# 01-introduccion_arboles
# Guía 1: De lo lineal a lo jerárquico
**Asignatura:** Estructura de Datos II  
**Programa:** Ingeniería de Software (IV Semestre)  

---

## 1. Clasificación de Escenarios

1. **Sistema de archivos:** *Jerárquico*. Presenta una raíz central y carpetas anidadas que contienen archivos e hijas sin relaciones cruzadas.
2. **Organigrama:** *Jerárquico*. Define niveles claros de autoridad desde la gerencia hacia cargos operativos.
3. **Menú de aplicación:** *Jerárquico*. Mantiene categorías principales que despliegan submódulos específicos.
4. **Árbol genealógico:** *Mixto / Grafo*. Es jerárquico al analizar el linaje descendente directo, pero funciona como un Grafo Acíclico Dirigido (DAG) en el origen biológico al coexistir múltiples padres.

---

## 2. Reflexión Técnica

Las estructuras de datos lineales como las listas, pilas y colas resultan insuficientes cuando los datos del mundo real poseen dependencias multinivel o jerárquicas. Representar un organigrama o un sistema de archivos mediante una lista implícitamente destruye las relaciones de pertenencia, exigiendo variables auxiliares o índices complejos para simular la jerarquía. 

Al adoptar un modelo no lineal como el Árbol General, la relación padre-hijo queda modelada de forma explícita mediante referencias entre nodos. Esto no solo facilita la lectura conceptual del problema, sino que optimiza el recorrido algorítmico al permitir aislar y procesar subramas específicas sin necesidad de inspeccionar toda la colección de datos. Asimismo, la flexibilidad que otorga la Programación Orientada a Objetos en Java mediante tipos genéricos `T` y colecciones dinámicas como `List<NodoGeneral<T>>` permite construir estructuras adaptables a cualquier volumen de datos. En conclusión, dar el paso de lo lineal a lo jerárquico es indispensable para abordar el diseño de software donde la información se organiza naturalmente por niveles de abstracción o subordinación.

---

## 3. Diagrama de la Estructura
El diagrama correspondiente se encuentra disponible en el archivo `diagrama.drawio` de este repositorio.
