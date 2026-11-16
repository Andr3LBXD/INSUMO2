# Timbre: el registro de atrasos que también cuida al estudiante

## Problema
En muchos colegios, el control de atrasos y faltas se lleva a mano en cuadernos u hojas sueltas. El inspector debe contar manualmente cuántas veces llegó tarde cada estudiante, lo que facilita perder registros o contar mal, y hace que el representante se entere tarde. Para el estudiante el proceso es opaco: no sabe cuántos atrasos lleva ni cuántos le faltan para una sanción, y un atraso con motivo válido (salud o transporte) puede quedar sin justificar. Aunque existen plataformas escolares, estas se enfocan en tareas y mensajes, dejando sin resolver este control diario.

## Solución
La aplicación móvil Timbre automatizará el registro de atrasos y faltas con un toque, guardando fecha y hora automáticas. Llevará un semáforo mensual por estudiante y, al tercer atraso injustificado, generará un aviso listo para copiar y enviar al representante. Además, incluye una vista para el estudiante donde puede consultar su historial, justificar atrasos con motivo válido (sin que afecten su conteo) y ganar la insignia «Puntual» al cumplir 10 días sin atrasos.

## Objetivos
- Automatizar el registro de atrasos y faltas con fecha y hora automáticas para ahorrar tiempo al inspector.
- Implementar un sistema de conteo mensual con semáforo que genere un aviso listo para enviar al representante al tercer atraso injustificado.
- Brindar transparencia al estudiante mediante una vista de historial donde consulte sus registros, justifique atrasos válidos y reciba reconocimientos por puntualidad.

## Habilidades
- React Native con Expo y TypeScript (entorno configurado)
- Componentes reutilizables y props tipadas
- Estado local, useState y custom hooks con AsyncStorage
- Navegación entre pantallas con Expo Router
- Estilos, temas claro/oscuro y diseño adaptable

## Alcance inicial
En esta primera versión (MVP) ambos modos funcionarán en un mismo celular con entorno Expo Go ya configurado y almacenamiento local validado con AsyncStorage. Incluirá una lista de estudiantes con buscador (cargada con datos de ejemplo), registro rápido de atrasos y faltas con fecha y hora automáticas, opción para justificar con motivo (salud o transporte), conteo mensual con semáforo (verde: 0-1, amarillo: 2, rojo: 3 o más atrasos injustificados), generador de mensaje de aviso listo para copiar, vista de historial del estudiante con contador de días sin atrasos e insignia a los 10 días, y soporte para tema claro y oscuro.

## Restricciones
- Entorno Expo CLI y TypeScript ya instalado y proyecto base inicializado con éxito.
- Lectura y escritura básica de AsyncStorage ya probada con datos simulados de ejemplo.
- No incluirá cuentas de usuario, servidor ni sincronización entre distintos dispositivos.
- No realizará envíos automáticos de mensajes a los representantes (el aviso se copia manualmente).
- No contará con lectura de carnés, códigos QR ni conexión con la plataforma institucional del colegio.
- No incluirá generación de reportes avanzados ni funciones de inteligencia artificial.
