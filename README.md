# 3.1-Simulador-picoW

<pre>

	<p align=center>

Tecnológico Nacional de México
Instituto Tecnológico de Tijuana

Departamento de Sistemas y Computación
Ingeniería en Sistemas Computacionales

Semestre:
Agosto - Diciembre 2023

Materia:
Lenguajes de interfaz

Docente:
M.C. Rene Solis Reyes 

Unidad:
3

Título del trabajo:
3.1 Simulador PicoW

Estudiante:
Marquez Santillan Jose Eduardo 21210395

	</p>

</pre>

<pre>

	<p align=left>

/*
 * Nombre del Archivo: Simulador PicoW
 * Autor:   Marquez Santillan Jose Eduardo
 * Correo:  l21210395@tectijuana.edu.mx
 * Fecha:   24/10/2023
 * Curso:   Lenguajes de Interfaz, TECNM Campus ITT
 * 
 * Objetivo:
 * Este programa fue creado para adentrarse al como un Raspberry Pi pico W realiza un hola mundo con blink.
 *
 * Historial de Revisiones:
 * 23/10/2023        Marquez Santillan Jose Eduardo
 *
 */
		
//-------------------------------------------------------------------------------------------------------------------------------------------------
		
// La función de configuración se ejecuta una vez cuando presionas el botón de reinicio o enciendes la placa.
void setup() {
  // Inicializa el pin digital LED_BUILTIN como una salida.
  pinMode(LED_BUILTIN, OUTPUT);
}

// La función de bucle se ejecuta una y otra vez infinitamente.
void loop() {
  digitalWrite(LED_BUILTIN, HIGH);  // enciende el LED (HIGH es el nivel de voltaje)
  delay(1000);                      // espera durante un segundo
  digitalWrite(LED_BUILTIN, LOW);   // apaga el LED al establecer el voltaje en LOW
  delay(1000);                      // espera durante un segundo
}
