# Proyecto Integrador 6CV1: Simulación Local de Phishing

Este repositorio contiene la documentación, evidencias y configuraciones del proyecto integrador de la materia Computer Security (Grupo 6CV1). El proyecto recorre el ciclo completo de la seguridad: ataque (Red Team), detección (Blue Team) y gobierno (Zero Trust).

## Entorno de Laboratorio y Reproducibilidad
El entorno utiliza infraestructura propia del equipo de forma local. Para levantar el entorno y reproducir el ejercicio, siga estos pasos exactos:

### Prerrequisitos
1. Máquina física (Windows/Linux/macOS) con Splunk Free instalado.
2. Hipervisor (VMware) instalado en la máquina física.
3. Una máquina virtual con Kali Linux (conectada en modo red NAT o Host-Only).

### Pasos para Ejecución (Demo en vivo)
1. **Atacante (Kali Linux):** Abrir la terminal y ejecutar `sudo setoolkit`. Seleccionar "Social-Engineering Attacks" -> "Website Attack Vectors" -> "Credential Harvester Attack Method" -> "Site Cloner".
2. **Defensa (Máquina Física):** Iniciar el servicio de Splunk Free y verificar que el reenvío de logs locales (puerto 80 / tráfico HTTP) esté activo.
3. **Simulación:** Desde el navegador de la máquina física, acceder a la IP de la máquina virtual Kali Linux e ingresar credenciales de prueba.
4. **Detección:** Revisar el panel de alertas de Splunk para confirmar la captura del evento de red.

## Bitácora de Trabajo
El registro de actividades de cada integrante se mantiene en el historial de commits de este repositorio.

| Fase | Tarea | Responsable(s) | Estado |
|------|-------|----------------|--------|
| Fase 0 | Registro, propuesta y creación del repositorio | Ulises Mota / Diego Silva | Completado |
| Fase 1 | Configuración de Kali, ataque SET y reporte técnico | Por asignar | Pendiente |
| Fase 2 | Instalación de Splunk, reglas de detección y plan de respuesta | Por asignar | Pendiente |
| Fase 3 | Programa de seguridad y arquitectura de Confianza Cero | Por asignar | Pendiente |
