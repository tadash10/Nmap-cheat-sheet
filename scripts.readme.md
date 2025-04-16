# Scripts Personalizados de Nmap

Este directorio contiene una colección de **scripts NSE** (Nmap Scripting Engine) que pueden ser utilizados para realizar auditorías de seguridad más específicas y detalladas. Los scripts están diseñados para probar vulnerabilidades comunes en servicios específicos, como HTTP, SMB, entre otros.

## Scripts en este Repositorio

### 1. `http-vuln.nse`
Este script está diseñado para identificar vulnerabilidades comunes en servidores web. Realiza pruebas de seguridad básicas en aplicaciones web, como la detección de vulnerabilidades de inyección SQL, XSS (Cross-Site Scripting), y más.

- **Uso**:
    ```bash
    nmap --script=http-vuln.nse <IP>
    ```
- **Descripción**: Escanea los servidores HTTP en busca de configuraciones inseguras y vulnerabilidades conocidas.

### 2. `smb-vuln.nse`
Este script escanea servicios SMB (Server Message Block) para detectar vulnerabilidades comunes como la explotación de la vulnerabilidad **MS17-010** (EternalBlue), y otros problemas relacionados con la configuración de SMB.

- **Uso**:
    ```bash
    nmap --script=smb-vuln.nse <IP>
    ```
- **Descripción**: Busca vulnerabilidades en el protocolo SMB que podrían permitir la ejecución remota de código o la obtención de información sensible.

## ¿Cómo Ejecutar los Scripts?

Para ejecutar cualquiera de estos scripts, utiliza el siguiente comando de Nmap, especificando el script que deseas ejecutar:

``bash
nmap --script=<nombre_del_script> <IP>

# Scripts NSE Personalizados

| Script          | Descripción                                        | Uso recomendado                        |
|-----------------|----------------------------------------------------|----------------------------------------|
| http-vuln.nse   | Detecta posibles vulnerabilidades HTTP (XSS)       | Sitios web HTTP/HTTPS                  |
| smb-vuln.nse    | Verifica si está habilitado el protocolo SMBv1     | Equipos Windows o servicios Samba (445)|

