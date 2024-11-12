# Cifrado y Descifrado de Texto en Python

Este proyecto implementa un sistema de cifrado básico en Python que utiliza una clave numérica para transformar cada letra de un texto en caracteres encriptados. La clave de cifrado se genera mediante una fórmula matemática que permite obtener un valor único para encriptar el texto. A su vez, el mismo valor se utiliza para realizar la operación inversa y recuperar el mensaje original.

## Descripción del funcionamiento

El código toma un texto de entrada y, a través de operaciones matemáticas, transforma cada letra usando su valor ASCII y una clave de cifrado compleja. En la encriptación, cada letra se convierte en su valor ASCII, se le suma la clave, y luego se convierte de nuevo a un carácter. La desencriptación invierte el proceso: resta la clave al valor ASCII de cada letra encriptada, recuperando así el texto original.

Este método de cifrado es un ejemplo básico, sin embargo, muestra los principios fundamentales del cifrado mediante transformación de caracteres y puede ajustarse o extenderse para crear cifrados personalizados.

## Ejemplo de uso

1. **Texto original**: `Luis`
2. **Clave de cifrado**: se define con una fórmula matemática que produce un número complejo.
3. **Texto encriptado**: el código encripta el texto original, transformándolo en un conjunto de caracteres distintos e irreconocibles.
4. **Texto desencriptado**: al aplicar el proceso inverso, el texto encriptado se convierte de nuevo en el texto original (`Luis`), usando la misma clave.

Este tipo de cifrado no es de alta seguridad, pero es suficiente para entender los conceptos básicos de encriptación y desencriptación. Es importante utilizar la misma clave en ambos procesos, ya que de lo contrario no sería posible recuperar el texto original.

## **Aplicaciones en Ingeniería de Datos y Ciberseguridad**

**Este código puede ser útil en ingeniería de datos (Data Engineering) y ciberseguridad en diversos aspectos:**

- **Ingeniería de Datos**: En el procesamiento y manipulación de datos, muchas veces es necesario proteger datos sensibles (como nombres, direcciones, etc.) cuando se manejan grandes volúmenes de datos. Este tipo de cifrado puede implementarse como un paso preliminar en un pipeline de datos para enmascarar información antes de su procesamiento o almacenamiento. La encriptación simple es útil en el preprocesamiento y en la creación de pruebas de datos seguras.

- **Ciberseguridad**: El código introduce a los conceptos básicos de cifrado y es una excelente herramienta educativa para entender la importancia de proteger la información mediante encriptación. Aunque este cifrado es sencillo, proporciona una base para explorar cifrados más complejos y puede adaptarse para su uso en ambientes de prueba, donde se necesitan métodos de cifrado simplificados para experimentar y analizar datos sin comprometer la seguridad.

## Consideraciones

- **Clave constante**: Es crucial que la clave de cifrado/desencriptado sea la misma. De no ser así, el texto original no podrá ser recuperado correctamente.
- **Visibilidad de caracteres**: Si la clave produce caracteres fuera del rango ASCII imprimible, el texto encriptado puede contener símbolos inusuales o ilegibles, lo cual es normal en métodos de cifrado más complejos.
- **Seguridad**: Este método es un ejemplo básico y no debe usarse para proteger información altamente sensible en aplicaciones reales. Para esos casos, se recomienda emplear algoritmos de cifrado avanzados como AES o RSA.

