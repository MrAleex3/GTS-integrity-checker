# 📡 GTS Integrity check

**GTS Integrity check** es una herramienta permite verificar la integridad de archivos `clave` en múltiples dispositivos GTS mediante conexión LAN. Diseñada para entornos de producción, automatiza la detección de modificaciones no autorizadas y envía alertas por correo electrónico.

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
- 📋 Registro de actividad

## 🧰 Requisitos del Sistema

- Python 3.7 o superior
- Bibliotecas requeridas:
  ```
  tkinter
  pillow
  telnetlib
  smtplib
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
