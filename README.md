# Nmap Cheat Sheet - Guía Profesional

Guía de referencia rápida y profesional sobre el uso de Nmap para tareas de escaneo, enumeración, evasión y generación de reportes. Diseñada para pentesters, analistas de seguridad y administradores de red.

---

## Estructura del Repositorio
Nmap-Cheat-Sheet/
├── README.md           # Guía principal
├── ejemplos/           # Salidas reales de escaneos
├── scripts/            # Scripts NSE destacados o personalizados
├── resultados/         # Reportes generados en distintos formatos
└── recursos.md         # Enlaces útiles y documentación externa


---

## Introducción a Nmap

Nmap (Network Mapper) es una herramienta de código abierto para exploración de redes y auditorías de seguridad. Permite descubrir hosts activos, servicios, versiones, sistemas operativos y posibles vulnerabilidades.

Instalación:

`bash
sudo apt install nmap       # En distribuciones Debian/Ubuntu
brew install nmap           # En macOS con Homebrew

COMANDOS BASICOS
nmap 192.168.1.1            # Escaneo simple por IP
nmap -v 192.168.1.1         # Escaneo detallado (verbose)
nmap scanme.nmap.org        # Escaneo por nombre de dominio
