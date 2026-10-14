---
layout: post
title: "Águila: programar en español suena hermoso, pero la historia completa importa"
---

Casi todo el que aprende a programar en Latinoamérica choca con el mismo muro antes de escribir su primera línea de código: el inglés. `if`, `while`, `function`, `print`, `true`, `false`... La lógica es universal, pero el vocabulario no. Por eso cada cierto tiempo aparece alguien con la misma idea hermosa: ¿y si el lenguaje hablara nuestro idioma?

El intento más reciente se llama **Águila**, y merece que lo miremos con lupa: con la ilusión que despierta y con la honestidad que exige.

## Qué es Águila

Águila es un lenguaje de programación con sintaxis 100% en español, creado por Emerson Espinoza, ingeniero de sistemas y docente que publica contenido como "CompilandoCode". Nació a finales de 2025 como proyecto personal —sin universidad ni empresa detrás— y sigue activo en 2026, con su sitio, documentación y comunidad pequeña pero real.

La propuesta se entiende en diez segundos:

```aguila
# Hola mundo
imprimir("¡Hola, mundo!")

si edad >= 18 {
    imprimir("Mayor de edad")
} sino {
    imprimir("Menor de edad")
}

funcion sumar(a, b) {
    retornar a + b
}
```

`si`, `mientras`, `funcion`, `imprimir`, `verdadero`, `falso`, `intentar`/`capturar`... Todo en español. Y no es solo un diccionario de sinónimos: según su documentación es multiparadigma (imperativo, orientación a objetos con `clase` y `yo`, lambdas, hilos, `asincrono`/`esperar`), con tipado dinámico, REPL, extensión para VS Code, un IDE web para programar sin instalar nada y una biblioteca estándar que cubre HTTP, JSON, bases de datos y hasta bots de Telegram. Se instala con un comando de npm y la documentación está toda en español, incluyendo una guía pensada para quienes vienen de Python.

Hasta aquí, todo bien. Es una idea con corazón: bajar la barrera del idioma para que más gente entre a programar. Incluso tiene un diferencial poco común y valioso: mensajes de error pensados para lectores de pantalla.

## Lo que no te cuentan en el video

Aquí es donde hay que ponerse serios, porque el marketing de Águila corre más rápido que sus hechos.

**El núcleo es cerrado.** El repositorio público tiene licencia MIT y usar el lenguaje es gratis, pero el propio README admite que el núcleo del compilador se desarrolla en un repositorio *privado*. Eso significa que las afirmaciones más ambiciosas —núcleo escrito en Rust, máquina virtual, compilación JIT— no las puede auditar nadie. "Open source" aplica al envoltorio, no al motor.

**"El primer lenguaje profesional de Latinoamérica": falso.** Existe **Latino** desde 2015, con objetivos casi idénticos, código 100% abierto y una comunidad diez veces mayor. Y en educación, **PSeInt** lleva desde 2003 enseñando a programar en español en universidades de toda Hispanoamérica. Águila no inventó la categoría; la continúa.

**"Compila a binario nativo": matizable.** Lo documentado hoy es un intérprete con JIT y un compilador *a JavaScript*, no emisión de binarios nativos. Y el benchmark que presume —"20x más rápido que Python"— es un Fibonacci recursivo publicado por el propio autor en su canal: el benchmark más débil y clásico que existe, sin réplica independiente.

**Es un proyecto de una sola persona.** 54 estrellas en GitHub, unos dos mil y pico de descargas, cero paquetes de terceros. Si el autor lo abandona, no hay comunidad que lo continúe —y la base cerrada lo hace imposible de rescatar.

Nada de esto lo hace un mal proyecto. Lo hace un proyecto **joven al que hay que exigirle transparencia**, no aplausos automáticos.

## ¿Y la educación en Latinoamérica?

La narrativa de Águila habla de soberanía tecnológica y de futuro educativo de Hispanoamérica. La realidad medible, hoy: **cero adopción documentada en escuelas o universidades**. Lo que existe es la iniciativa del propio autor —cursos en video, un IDE web usable en clase y una campaña para conseguir 1.000 "pioneros" (van 179). Es una apuesta personal con tracción en redes, no un movimiento educativo.

## Lo que me llevo

La idea de Águila es correcta y necesaria: el inglés no debería ser un peaje para aprender a programar. Pero las buenas intenciones no compilan. Un lenguaje que aspira a ser infraestructura educativa de un continente no puede construirse sobre un núcleo cerrado, con marketing que exagera y sin comunidad que lo sostenga.

Si Águila quiere volar de verdad, el camino es claro: abrir el núcleo, publicar benchmarks replicables y dejar que la comunidad —no un video— hable por él. Mientras tanto, lo miro con cariño y con escepticismo, que es como hay que mirar todo lo que promete cambiar el mundo.

*Fuentes: repositorio oficial (github.com/emersonxinay/aguila), sitio aguila.compilandocode.com, paquete npm aguila-lang, documentación del proyecto, y comparativa con Latino y PSeInt.*
