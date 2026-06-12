# BlueHeaven: Automation & Infrastructure as Code - ISP

BlueHeaven es la continuacion del proyecto OuterHeaven, su finalidad es abarcar y mejorar ciertos aspectos de IT de mejor manera y mas avanzada

## Descripción del Proyecto

**BlueHeaven** es la continuacion, evolución y fase de optimización avanzada de un ISP simulado hecho anteriormente en el proyecto **OuterHeaven**. Tras haber finalizado la primera etapa una arquitectura basada en clústeres de **alta disponibilidad (HA)** y almacenamiento distribuido, esta nueva fase hemos decidido abordar la transición completa hacia la gestión moderna de operaciones, es decir, el objetivo central de **BlueHeaven** es eliminar la intervención manual en el ciclo de vida de la infraestructura. Para ello, se implementan metodologías de Infraestructura como **Código (IaC)** , gestión de **configuración automatizada** y flujos de integración continua **(CI/CD)**, garantizando un entorno escalable, replicable y mantenible por un único administrador.

### Objetivos Técnicos y Alcance

#### Aprovisionamiento Declarativo (IaC)

Migración del despliegue de máquinas virtuales y contenedores LXC en Proxmox VE hacia Terraform. Automatización integral de la creación, modificación y destrucción de recursos a través de código.

#### Gestión de Configuración y Orquestación: 

Expansión de las capacidades de Ansible para cubrir no solo las políticas de respaldo y snapshots, sino también el aprovisionamiento de software interno, la configuración de red de los servicios y el mantenimiento del sistema operativo.

#### Pipelines de CI/CD (Escala Menor): 

Implementación de flujos automatizados (ej. GitHub Actions / GitLab CI) enfocados en el aseguramiento de la calidad del código de infraestructura (linting, validación sintáctica) antes de su aplicación en el entorno real.

#### Refactorización y Endurecimiento (Hardening):

Pulido de la documentación técnica y diseño de playbooks específicos para la recuperación ante desastres (Troubleshooting avanzado).

#### Stack Tecnológico
Este es el planteamiento del stack que se utilizara, seguramente variara a lo largo de la trayectoria del proyecto
- Proxmox VE en cluster
- ZFS o Ceph ( por decidir)
- Kubernetes (K8s y K9s)
- NetData
- Zabbix
- Grafana o Prometheus
- Ansible
- Terraform
- Github Actions
- Mikrotik + Ubiquiti
- Veem Backup
- Proxmox PBS

Coming soon...

Plataforma de Virtualización: Proxmox VE (Clúster, HA, Ceph o ZFS)

IaC + Automatizacion + Configuracion: 
 - Terraform
 - Ansible
Control de Versiones y CI/CD: [GitHub / GitLab]
