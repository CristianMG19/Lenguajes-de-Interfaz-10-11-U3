# Prácticas de Unidad 3 - Lenguajes de Interfaz

Alumno: Medina González Cristian Roberto  
N. Control: 23170234  
Materia: Lenguajes de Interfaz - Unidad 3  
Docente: Ing. José Luis Medina Jiménez  
Horario: 10:00 - 11:00

Cinco prácticas independientes sobre procedimientos, registros, validación y macros. Cada una incluye el código ASM comentado, una solución de Visual Studio 2022, el proyecto y un README con su funcionamiento y comprobaciones.

## Prácticas incluidas

| Práctica | Tema | Resultado |
| --- | --- | --- |
| 01 | Llamadas a un procedimiento | Dos avisos entre los mensajes de inicio y fin |
| 02 | Registro EBX | 15, esperado por el código; ejecución bloqueada en este equipo |
| 03 | Cadena no vacía | Hola; la variante vacía mostró el mensaje correspondiente |
| 04 | Macro de multiplicación | 8 por 5 = 40 |
| 05 | Macro IMUL | 6 por 7 = 42 |


## Requisitos

- Windows y Visual Studio 2022 con Desarrollo para el escritorio con C++.
- Herramientas MSVC v143 para x86 y un SDK de Windows instalado.
- Irvine32.inc, SmallWin.inc, VirtualKeys.inc e Irvine32.lib en C:\Irvine, además de las bibliotecas de Windows utilizadas por Irvine.

Irvine32 es una dependencia externa y no se incluye como biblioteca en esta entrega. Si está en otra ubicación, cambiar IrvineDir en cada .vcxproj. No usar x64: estas prácticas utilizan Irvine32 y registros de 32 bits.

Compilar.cmd permite ensamblar y enlazar desde x86 Native Tools Command Prompt for VS 2022. Ejecutar.cmd abre el ejecutable generado y espera una tecla al terminar. Ambos archivos son auxiliares.

## Comprobaciones reales

Las cinco prácticas se ensamblaron y enlazaron correctamente con ML/LINK 14.44.35207 de Visual Studio 2022, para x86 y con símbolos de depuración. Las prácticas 01, 03, 04 y 05 se ejecutaron en consola y sus salidas coincidieron con las esperadas. También se ejecutó la variante vacía de la práctica 03.

Microsoft Defender detectó el ejecutable de la práctica 02 y lo puso en cuarentena al intentar ejecutarlo. Por esa razón su resultado 15 se identifica como esperado, no como observado. No se restauró la cuarentena, no se desactivó la protección y no se añadieron exclusiones. La entrega contiene fuentes y proyectos, sin ejecutables.

Se verificaron los archivos XML, los identificadores de proyecto y las rutas de las soluciones. La compilación comprobada se realizó directamente con ML/LINK. No se presenta como realizada una sesión de depuración desde la interfaz de Visual Studio.
