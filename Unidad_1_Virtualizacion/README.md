# 📂 Unidad 1: Virtualización y Entornos Aislados
## Taller de Sistemas Operativos

Esta unidad se enfoca en la creación del "lienzo" sobre el cual construiremos nuestra infraestructura. El objetivo es dominar la abstracción de hardware para ejecutar múltiples sistemas operativos de forma simultánea y segura.

---

## 🎯 Objetivos de Aprendizaje
1. Diferenciar entre hipervisores de **Tipo 1 (Bare Metal)** y **Tipo 2 (Hosted)**.
2. Configurar entornos de red virtual (NAT, Bridge, Host-Only).
3. Gestionar recursos críticos: CPU (VT-x/AMD-V), RAM dinámica y VRAM.
4. Administrar instantáneas (Snapshots) para la recuperación de fallas.

---

## 💻 Herramientas del Laboratorio
En este curso utilizaremos principalmente:
* **Oracle VM VirtualBox:** Por su versatilidad y soporte multiplataforma.
* **VMware Workstation/Player:** Para entornos que requieran mayor aceleración de hardware.
* **ISO Images:** Preparación de medios de instalación para Windows Server y Debian.

---

## 🔧 Configuración Base de Red
Para el laboratorio híbrido, utilizaremos la siguiente convención de red:

| Modo de Red | Uso en el Taller |
| :--- | :--- |
| **NAT** | Acceso a Internet para descarga de paquetes y actualizaciones. |
| **Red Interna** | Comunicación privada entre el Controlador de Dominio (Win) y el Cliente (Linux). |
| **Adaptador Puente** | Para que el servidor sea visible en la red física del TecNM. |

---

## 📝 Actividades de la Unidad

### 1.1 Configuración del Hipervisor
* Habilitación de la virtualización en BIOS/UEFI.
* Instalación de *Guest Additions* o *VMware Tools*.

### 1.2 Creación de Plantillas (Templates)
* Configuración de hardware base para servidores:
  * RAM: 2GB (Mínimo para Server Core).
  * Disco: 40GB (Dinámicamente reservado).
  * Red: Doble adaptador (NAT e Interna).

### 1.3 Gestión de Snapshots
* Crear un punto de restauración "Limpio" antes de la promoción de dominios o instalaciones de servicios.
