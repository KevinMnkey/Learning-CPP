# Roadmap Definitivo: De C++ a Arquitectura de Motores de Videojuegos

Este documento traza el camino desde los fundamentos absolutos del lenguaje hasta la programación de bajo nivel de un motor gráfico personalizado. 

---

## FASE 1: Fundamentos de Programación (La Base)
*Objetivo: Dominar la sintaxis básica y la lógica de control.*

- [ ] **01. Configuración del Entorno:** Instalar un compilador (GCC/Clang) y un IDE o editor (VS Code, Neovim). Entender el proceso de compilación y enlazado.
- [ ] **02. Variables y Tipos de Datos:** `int`, `float`, `double`, `char`, `bool`. Entender la gestión de bytes y tamaño en memoria.
- [ ] **03. Operadores:** Aritméticos, lógicos (`&&`, `||`, `!`) y de comparación.
- [ ] **04. Estructuras de Control:** Condicionales (`if`, `switch`) y Bucles (`for`, `while`, `do-while`).
- [ ] **05. Funciones:** Declaración, definición, ámbito (scope), y la diferencia vital entre pasar argumentos por valor y por referencia (`&`).

## FASE 2: Estructuras de Datos Básicas y Memoria (El ADN de C++)
*Objetivo: Entender el hardware real y cómo C++ gestiona la memoria RAM.*

- [ ] **06. Arreglos Estáticos (Arrays):** Vectores unidimensionales y matrices bidimensionales (como tableros de 3x3).
- [ ] **07. Punteros (Pointers):** Operadores de dirección (`&`) y desreferencia (`*`). Aritmética de punteros.
- [ ] **08. Memoria Dinámica:** Stack (rápida/automática) vs Heap (manual). Uso de `new`, `delete` y `delete[]`.
- [ ] **09. Estructuras Personalizadas:** Uso de `struct` y `enum` para agrupar datos complejos (ej. Vectores matemáticos).

## FASE 3: Programación Orientada a Objetos - POO (Arquitectura)
*Objetivo: Modelar sistemas complejos de software.*

- [ ] **10. Clases y Objetos:** Abstracción, separación de archivos `.h` (headers) y `.cpp` (implementación).
- [ ] **11. Encapsulamiento:** Modificadores de acceso `public`, `private` y `protected`.
- [ ] **12. Ciclo de Vida del Objeto:** Constructores, Destructores y el principio RAII (Resource Acquisition Is Initialization).
- [ ] **13. Herencia y Polimorfismo:** Clases abstractas, métodos virtuales (`virtual`, `override`).
- [ ] **14. Sobrecarga de Operadores:** Definir cómo interactúan los objetos (ej. sumar dos objetos `Vector3`).

## FASE 4: C++ Moderno y la STL (El Estándar Profesional)
*Objetivo: Escribir código seguro y eficiente de nivel industrial (C++11 a C++20).*

- [ ] **15. Programación Genérica (Templates):** Funciones y clases adaptables a cualquier tipo de dato.
- [ ] **16. La STL (Standard Template Library):** Contenedores (`std::vector`, `std::map`), Iteradores y Algoritmos (`std::sort`, `std::find`).
- [ ] **17. Punteros Inteligentes:** `std::unique_ptr` y `std::shared_ptr` para gestión automática de memoria y evitar memory leaks.
- [ ] **18. Manejo de Excepciones:** Bloques `try`, `catch`, `throw`.
- [ ] **19. I/O Streams:** Lectura y escritura de archivos en disco (`std::ifstream`, `std::ofstream`).

---

## FASE 5: Matemáticas para Videojuegos (El Núcleo)
*Objetivo: Traducir álgebra y geometría a código ejecutable.*

- [ ] **20. Álgebra Lineal 2D/3D:** Vectores, Producto Punto (Dot Product) y Producto Cruz (Cross Product).
- [ ] **21. Matrices de Transformación:** Matrices 3x3 y 4x4 para Traslación, Rotación y Escala.
- [ ] **22. Cuaterniones (Quaternions):** Rotaciones 3D avanzadas sin bloqueo de cardán (Gimbal Lock).

## FASE 6: APIs Gráficas (Hablando con la GPU)
*Objetivo: Renderizado y control de píxeles por hardware.*

- [ ] **23. Creación de Ventanas y Contexto:** Uso de librerías base (SDL2 o GLFW).
- [ ] **24. El Pipeline Gráfico:** Entender el viaje desde un vértice hasta el píxel final.
- [ ] **25. Renderizado Básico:** Integración de OpenGL o Vulkan. Dibujar el primer triángulo.
- [ ] **26. Programación de Shaders:** Escribir código GLSL para el Vertex Shader y Fragment Shader.

## FASE 7: Arquitectura Central del Motor (Game Engine Core)
*Objetivo: Estructurar el motor para máxima eficiencia y 60+ FPS.*

- [ ] **27. El Game Loop:** Patrón de inicialización, actualización de lógica (`Update`) y renderizado (`Render`).
- [ ] **28. Gestión de Tiempo:** Cálculo de Delta Time para sincronizar la física sin importar el framerate.
- [ ] **29. Patrón ECS (Entity-Component-System):** Desacoplar datos de la lógica para optimizar el uso de la memoria caché.
- [ ] **30. Allocators Personalizados:** Crear gestores propios de memoria (Memory Pools, Stack Allocators) para rendimiento extremo.

## FASE 8: Subsistemas y Herramientas
*Objetivo: Darle vida y utilidad al motor gráfico.*

- [ ] **31. Input System:** Detección unificada de teclado, ratón y gamepad.
- [ ] **32. Detección de Colisiones:** Implementación de AABB (Axis-Aligned Bounding Box) y Raycasting.
- [ ] **33. UI de Desarrollo:** Integración de Dear ImGui para crear el panel de control y ventanas de depuración del motor.
