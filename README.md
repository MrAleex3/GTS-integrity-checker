# 📡 GTS Checksum Verifier

**GTS Checksum Verifier** es una herramienta desarrollada en Python con Tkinter que permite verificar la integridad de archivos `autorun.sh` en múltiples dispositivos GTS mediante conexión LAN. Diseñada para entornos de producción, automatiza la detección de modificaciones no autorizadas y envía alertas por correo electrónico.

<img width="827" height="671" alt="image" src="https://github.com/user-attachments/assets/b5cde1a9-f150-47ee-ab19-8d7766124529" />


## ✅ Características Principales

- 🔍 Verificación masiva de checksums SHA1 en dispositivos GTS
- 📧 Notificación por correo electrónico cuando se detectan alteraciones
- 📊 Panel de resultados con contadores visuales
- ⏱ Programación de verificaciones periódicas
- 📝 Registro detallado de actividad

## 🚀 Funcionalidades Clave

### Verificación Automatizada
- Conexión automatizada a múltiples dispositivos
- Comparación de checksums contra valor de referencia
- Detección de archivos alterados o corruptos

### Sistema de Alertas
- 📨 Envío de correos electrónicos a múltiples destinatarios
- 📋 Reporte detallado con IPs de dispositivos afectados
- 📈 Resumen estadístico de verificaciones

### Interfaz Intuitiva
- 🎨 Diseño moderno
- 📊 Barra de progreso visual
- 🌐 Visualización de resultados en tiempo real
- 📋 Registro de actividad con timestamp

## 🧰 Requisitos del Sistema

- Python 3.7 o superior
- Bibliotecas requeridas:
  ```
  tkinter
  pillow
  telnetlib
  smtplib
  ```
- Acceso de red a los dispositivos GTS
- Credenciales SMTP para envío de alertas

## 🛠️ Configuración

1. **Archivo de configuración**:
   - Crear `checksum.txt` con una IP por línea
   - Configurar parámetros SMTP en el código:
     ```python
     self.smtp_config = {
         'server': 'smtp.office365.com',
         'port': 587,
         'email': 'tu_correo@empresa.com',
         'password': 'tu_contraseña',
         'recipients': ['destinatario1@empresa.com', 'destinatario2@empresa.com']
     }
     ```

2. **Checksum de referencia**:
   - Modificar `self.correct_checksum` con el valor SHA1 correcto

## 📦 Estructura del Proyecto

```
GTS-Checksum-Verifier/
├── checksum.txt          # Lista de IPs a verificar
├── logo.png              # Logo de la aplicación (opcional)
├── main.py               # Script principal
├── requirements.txt      # Dependencias
└── README.md             # Este archivo
```

## ⚙️ Ejecución

1. Instalar dependencias:
   ```
   pip install -r requirements.txt
   ```

2. Ejecutar la aplicación:
   ```
   python main.py
   ```

## 📝 Licencia

Este proyecto está bajo la Licencia MIT.

## 🙋 Autor

**Jose Espinoza**  
Foxconn México · Herramienta desarrollada para el departamento de TI

---

### 📌 Notas Adicionales

- La herramienta es compatible con cualquier dispositivo que permita conexión Telnet
- Se recomienda ejecutar en entornos seguros debido al manejo de credenciales
- El intervalo mínimo recomendado entre verificaciones es de 60 segundos

### 🔄 Historial de Versiones

**v1.1** (Actual)
- Soporte para múltiples destinatarios
- Mejoras en el manejo de timeouts
- Interfaz más responsiva

**v1.0**
- Lanzamiento inicial
- Verificación básica de checksums
- Notificaciones por correo electrónico
