# caf-power-platform

graph TD
    A[Inicio] --> B[Formulario en Power Pages]
    B --> C{Validación Automática de Datos}
    C -->|Datos Correctos| D[Envía Correo Automático]
    C -->|Datos Incorrectos| E[Notifica al Usuario para Corrección]
    E --> B
    D --> F[Revisión por Administradores]
    F --> G{Validación por Otras Áreas}
    G -->|Aprobada| H[Creación de Cuenta]
    G -->|Rechazada| I[Notificar al Usuario]
    I --> B
    H --> J[Correo de Confirmación]
    J --> K[Fin]
