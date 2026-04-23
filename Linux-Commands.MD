# 🐧 Guía Maestra de Comandos Linux
## Taller de Sistemas Operativos | Profr. Arturo Barajas

Esta guía contiene los comandos fundamentales para dominar la terminal de Linux, organizados por categorías funcionales.

---

## 📂 1. Gestión de Archivos y Directorios
| Comando | Descripción | Ejemplo |
| :--- | :--- | :--- |
| `ls` | Listar archivos y directorios. | `ls -la` |
| `cd` | Cambiar de directorio. | `cd /etc/network` |
| `pwd` | Mostrar la ruta del directorio actual. | `pwd` |
| `mkdir` | Crear un nuevo directorio. | `mkdir practicas_so` |
| `rm` | Eliminar archivos o directorios. | `rm -rf carpeta_old/` |
| `cp` | Copiar archivos o directorios. | `cp file.txt /tmp/` |
| `mv` | Mover o renombrar archivos/directorios. | `mv viejo.txt nuevo.txt` |
| `touch` | Crear un archivo vacío. | `touch sesion_1.txt` |

## 🔍 2. Visualización y Procesamiento de Texto
| Comando | Descripción | Ejemplo |
| :--- | :--- | :--- |
| `cat` | Muestra el contenido completo de un archivo. | `cat config.php` |
| `grep` | Busca un patrón de texto en archivos. | `grep "error" syslog` |
| `less` | Visualiza archivos de forma paginada. | `less logs.txt` |
| `head` | Muestra las primeras líneas de un archivo. | `head -n 15 data.csv` |
| `tail` | Muestra las últimas líneas de un archivo. | `tail -f access.log` |
| `wc` | Cuenta líneas, palabras y bytes. | `wc -l lista.txt` |
| `find` | Busca archivos en el sistema. | `find /home -name "*.sh"` |

## 🔐 3. Permisos y Administración (Seguridad)
| Comando | Descripción | Ejemplo |
| :--- | :--- | :--- |
| `chmod` | Cambia los permisos de archivos/directorios. | `chmod 755 script.sh` |
| `chown` | Cambia el propietario y grupo. | `sudo chown root:root file` |
| `sudo` | Ejecuta comandos con privilegios de root. | `sudo apt update` |
| `whoami` | Muestra el nombre del usuario actual. | `whoami` |
| `passwd` | Cambia la contraseña del usuario. | `passwd usuario` |

## ⚙️ 4. Procesos y Monitoreo del Sistema
| Comando | Descripción | Ejemplo |
| :--- | :--- | :--- |
| `top` / `htop` | Monitor interactivo de procesos. | `htop` |
| `ps` | Muestra instantánea de procesos actuales. | `ps aux` |
| `kill` | Termina un proceso por su ID (PID). | `kill -9 1234` |
| `df` | Espacio libre en el sistema de archivos. | `df -h` |
| `du` | Uso de disco por archivo/directorio. | `du -sh *` |
| `free` | Uso de memoria RAM y Swap. | `free -m` |

## 🌐 5. Redes y Conectividad
| Comando | Descripción | Ejemplo |
| :--- | :--- | :--- |
| `ping` | Prueba la conectividad con un host. | `ping 8.8.8.8` |
| `ip addr` | Muestra interfaces de red e IPs. | `ip addr show` |
| `ssh` | Conexión remota cifrada. | `ssh user@server.com` |
| `scp` | Copia archivos entre hosts por SSH. | `scp file.txt user@ip:/dir` |
| `curl` / `wget` | Descarga contenido de la web. | `wget http://site.com/iso` |
| `netstat` | Estadísticas de red y puertos. | `netstat -tulpn` |

## 📦 6. Archivos y Compresión
| Comando | Descripción | Ejemplo |
| :--- | :--- | :--- |
| `tar` | Empaqueta o extrae archivos .tar. | `tar -xzvf file.tar.gz` |
| `zip` / `unzip` | Comprime o extrae archivos .zip. | `unzip proyecto.zip` |
| `gzip` | Comprime archivos en formato .gz. | `gzip archivo.log` |

---

### 💡 Tips para el Taller:
1. **Autocompletado:** Presiona la tecla `Tab` después de escribir las primeras letras de un comando o ruta.
2. **Historial:** Usa las flechas `Arriba` y `Abajo` para navegar por comandos anteriores.
3. **Ayuda:** Si no sabes usar un comando, escribe `man <comando>` para leer el manual oficial.

---
*Documento generado para fines académicos en la materia de Sistemas Operativos.*
