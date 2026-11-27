# Cyber Range y SOC Automatizado — Proyecto ASIR

Proyecto de 2º de ASIR basado en virtualización con **Proxmox VE**, segmentación de red, monitorización/respuesta con **Wazuh** y control de versiones en **GitHub**.

## Estado actual (Demo 1)

- **pfSense:** WAN en `vmbr0` y LAN estática en `192.168.20.1/24` (`vmbr2`).
- **Debian 12:** máquina virtual interna en `vmbr2` con IP estática `192.168.20.10/24`.
- **Conectividad base:** comprobación bidireccional con `0%` de pérdida de paquetes.
- **Kali Linux (`vmbr0`):** incidencias en el instalador tradicional (`kali-linux-2025.4-installer-amd64.iso`) durante la instalación de programas y `GRUB`, quedando el arranque en `Booting from Hard Disk...`; pendiente de arrancar desde imagen **Live** o completar `GRUB` para las pruebas controladas.
