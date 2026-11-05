
# ARCHI POS & ERP Empresarial

> Sistema Integral de Punto de Venta, Inteligencia de Inventario Multi-Sucursal y Asesor Financiero Automatizado para Retail (Régimen Pro Pyme 14 D3 - SII Chile).

[![Python Version](https://img.shields.io/badge/Python-3.11+-3776AB?style=flat&logo=python&logoColor=white)](https://www.python.org/)
[![Framework](https://img.shields.io/badge/Backend-Flask%20Modular-000000?style=flat&logo=flask&logoColor=white)](https://flask.palletsprojects.com/)
[![Database](https://img.shields.io/badge/Database-SQLite%20%7C%20MySQL-4479A1?style=flat&logo=sqlite&logoColor=white)](https://www.sqlite.org/)
[![AI Vision](https://img.shields.io/badge/AI%20Engine-Google%20Gemini%20Vision-4285F4?style=flat&logo=google&logoColor=white)](https://ai.google.dev/)
[![Frontend](https://img.shields.io/badge/Frontend-Vanilla%20ES6%20%2B%20CSS3%20(No%20Frameworks)-F7DF1E?style=flat&logo=javascript&logoColor=black)](https://developer.mozilla.org/)
[![UI Target](https://img.shields.io/badge/Target-Touch%20Tablets%209.7%22-10B981?style=flat)](https://github.com/)
[![Test Suite](https://img.shields.io/badge/Tests-79%20Passing-success?style=flat)](https://github.com/)
[![License](https://img.shields.io/badge/License-Proprietary-red?style=flat)](LICENSE)

---

## 1. Propuesta de Valor y Enfoque Comercial

### El Problema del Retail y las Pymes en Chile
La mayoría de los sistemas de punto de venta (POS) tradicionales se limitan a ser calculadoras de caja registradoras con emisión de tickets. Los dueños de negocios en Chile enfrentan tres problemas críticos que destruyen su rentabilidad:
1. **Ceguera Tributaria:** Incapacidad de prever el pago mensual de impuestos (Formulario 29: IVA neto + PPM), lo que provoca multas por mora ante el SII y crisis repentinas de liquidez al día 20 de cada mes.
2. **Capital Atrapado en Bodega:** Carencia de visibilidad sobre qué productos concentran el 80% de las ventas frente a aquellos que representan capital inmovilizado y obsolescencia.
3. **Desorden en la Tesorería:** Mezcla constante de los ingresos operativos con el sueldo del dueño, los arriendos y el dinero de reinversión en stock.

### La Solución: ARCHI POS & ERP
ARCHI no es solo un software de facturación; es un **asesor financiero y operativo automatizado**. Transforma cada venta en datos estratégicos en tiempo real, permitiendo a empresas del **Régimen Pro Pyme (Art. 14 D3)** tomar decisiones basadas en números precisos.

### Retorno de Inversión (ROI) Comprobado
- **Reducción del 85% en tiempo de cuadratura:** Cierre de caja en menos de 2 minutos mediante conciliación asistida por visión artificial (OCR multimodal de vouchers de tarjetas).
- **Disminución del 40% en quiebres de inventario:** Monitoreo dinámico del ritmo de venta diaria (Run Rate) y alertas automáticas de reposición antes de agotar existencias.
- **Previsibilidad Tributaria Total (F29):** Cálculo automático del IVA débito vs. crédito fiscal y cálculo exacto del PPM a reservar, evitando sorpresas al cierre contable.
- **Disciplinamiento Financiero Automático:** División algorítmica de la recaudación mediante la regla de los 4 Fondos de Capital.

---

## 2. Core Features (Capacidades Principales)

### A. Punto de Venta Touch de Ultra Baja Latencia
- **Diseño Ergonómico para Tablets de 9.7":** Interfaz táctil de alto contraste (estética Tesla/Orion) construida en Vanilla JavaScript sin sobrecarga de frameworks, garantizando 60 FPS estables y cero latencia de toque.
- **Soporte Multi-Método de Pago:** Débito, Crédito, Efectivo (con cálculo de vuelto dinámico), Transferencias Bancarias y Pagos Divididos/Mixtos en una sola transacción.
- **Gestión Avanzada de Variantes:** Matriz completa de tallas y atributos por producto con selector modal touch-friendly de toque completo.
- **Cuadratura y Cierre de Caja con IA:** Captura fotográfica directa de los vouchers emitidos por terminales de pago (Transbank, Getnet, Redelcom, Mercado Pago) con extracción automática de totales mediante Google Gemini Vision OCR.

### B. Inteligencia Financiera y Motor Tributario (SII Chile)
- **Simulador en Tiempo Real del Formulario 29 (F29):** Proyección mensual de la obligación tributaria neta considerando el débito fiscal de ventas y el crédito fiscal de compras a proveedores.
- **Gestión de Tratamientos Tributarios:** Clasificación estricta de egresos en:
  - *Factura Afecta (Recupera IVA 19%)*
  - *Factura Exenta / Boleta de Honorarios (Gasto Renta)*
  - *Gastos Rechazados*
- **Tasa de PPM Parametrizable:** Cálculo del Pago Provisional Mensual según los regímenes tributarios vigentes en Chile.
- **Escudo Fiscal y Simulador de Medios de Pago:** Proyección del costo financiero y tributario derivado de comisiones de adquirencia versus pago en efectivo o transferencia.

### C. Asignación de Capital: Metodología de los 4 Fondos
El sistema distribuye algorítmicamente la tesorería acumulada para garantizar solvencia perpetua:
1. **Fondo de Remuneraciones:** Reserva programada para sueldos del personal y retiro del emprendedor.
2. **Fondo de Reinversión de Stock:** Capital protegido exclusivamente para la recompra de mercadería crítica.
3. **Fondo de Gastos Fijos (Colchón Operativo):** Acumulación prorrateada para arriendos, gastos comunes, energía y conectividad.
4. **Fondo de Reserva / Imprevistos:** Fondo de seguridad para contingencias operacionales.
- **Conciliación de Pozo Bancario:** Arqueo periódico de cuentas bancarias contrastando el saldo real con los saldos teóricos del sistema.

### D. Inteligencia de Inventario Multi-Sucursal
- **Análisis ABC (Pareto 80/20):** Clasificación algorítmica del catálogo en productos Clase A (alto impacto), Clase B (rotación media) y Clase C (bajo impacto/riesgo de obsolescencia).
- **Detección de Capital Inmovilizado:** Identificación de stock sin rotación para liquidación estratégica.
- **Plan MRP de Reabastecimiento Inter-Sucursales:**
  - Cálculo de la velocidad de consumo diario (Run Rate).
  - Cálculo de días de cobertura restante.
  - Punto de Reorden (ROP) y Stock de Seguridad ajustado al tiempo de entrega (Lead Time) del proveedor.
- **Generación Vectorial de Códigos EAN-13 GS1:** Generador de etiquetas PDF en formato Carta/A4 a 300 DPI (24 etiquetas por hoja) con prefijo oficial de Chile (780), legibles con lectores ópticos láser y de cámara.

---

## 3. Arquitectura Técnica

### Stack Tecnológico

| Capa | Tecnología | Justificación Técnica |
| :--- | :--- | :--- |
| **Frontend** | HTML5 Semántico, CSS3 Vanilla, JavaScript Modular (ES6+) | Eliminación de bundle overhead. Latencia cero en renderizado de componentes touch para tablets de recursos moderados. |
| **Backend** | Python 3.11+, Flask Framework (Blueprints) | Arquitectura modular desacoplada por dominios de negocio. Mantenimiento y extensibilidad simplificados. |
| **Base de Datos** | SQLite (Modo WAL) / MySQL 8.0+ | Transacciones ACID atómicas con bloqueos optimistas para evitar condiciones de carrera en ventas e inventario. |
| **Visión / IA** | Google Gemini 1.5 / 2.0 Flash Vision API | Extracción multimodal estructurada de comprobantes térmicos de pago con tolerancia a arrugas y baja luz. |
| **Reportes / PDF** | ReportLab 4.x Vectorial | Generación nativa de PDFs (etiquetas de código de barras 300 DPI y reportes financieros) sin dependencias headless. |
| **Servidor WSGI** | Waitress (Producción Windows/Linux) | Servidor HTTP WSGI multihilo puro de alto rendimiento sin requerir Nginx inverso obligatorio para despliegues locales. |

### Diagrama de Arquitectura de la Solución

```mermaid
graph TD
    subgraph Clientes_Touch [Terminales Touch y Tablets 9.7 Pulgadas]
        A[Tablet Mostrador - POS Touch]
        B[Smartphone - Toma de Inventario]
        C[PC Administrador - ERP & Finanzas]
    end

    subgraph Red_Segura [Capa de Red & Acceso]
        D[Tailscale VPN / DuckDNS HTTPS]
    end

    subgraph Servidor_Local [Servidor Local ARCHI WSGI]
        E[Waitress WSGI Server :5000]
        F[Flask Application Core]
        
        subgraph Modulos_Blueprints [Modulos de Negocio]
            F1[POS & Ventas]
            F2[Inventario & Variantes]
            F3[Gastos & Proveedores]
            F4[Tesorería & 4 Fondos]
            F5[Motor Tributario F29]
            F6[Motor OCR Gemini Vision]
            F7[Backup & Restauracion]
        end
    end

    subgraph Datos_Persistencia [Capa de Datos y Almacenamiento]
        G[(Base de Datos SQLite / MySQL)]
        H[Backups Locales Rotativos]
        I[Google Drive Cifrado Cloud]
    end

    Clientes_Touch -->|HTTP/JSON Seguro| D
    D --> E
    E --> F
    F --> F1 & F2 & F3 & F4 & F5 & F6 & F7
    F1 & F2 & F3 & F4 & F5 & F7 --> G
    F7 --> H
    F7 --> I
    F6 -.->|API REST Multimodal| J[Google Gemini Cloud AI]
```

### Principales Endpoints de la API REST

| Método | Endpoint | Descripción | Perfil Requerido |
| :--- | :--- | :--- | :--- |
| `POST` | `/api/sales` | Registra una nueva transacción de venta con desglose de pago | Cajero / Admin |
| `GET` | `/api/sales/daily-summary` | Obtiene el total consolidado del día y arqueo de caja | Cajero / Admin |
| `GET` | `/api/products` | Consulta el catálogo con variantes y stock por sucursal | Cajero / Admin |
| `POST` | `/api/products` | Crea o actualiza un producto y sus variantes | Administrador |
| `POST` | `/api/transfers` | Registra un traspaso atómico de stock entre sucursales | Administrador |
| `GET` | `/api/suppliers/expenses` | Consulta los gastos operativos del mes por categoría | Administrador |
| `POST` | `/api/suppliers/expenses` | Registra un egreso operacional o compra de stock | Administrador |
| `GET` | `/api/taxes/f29-summary` | Obtiene la simulación tributaria del F29 del periodo | Administrador |
| `POST` | `/api/ocr/analyze-voucher` | Procesa voucher de pago con IA para cuadratura de caja | Cajero / Admin |
| `POST` | `/api/backup/create` | Genera copia de seguridad física de la base de datos | Administrador |

---

## 4. Instalación y Puesta en Marcha

### Prerrequisitos de Sistema
- **Sistema Operativo:** Linux (Ubuntu 22.04+ LTS recomendado), Windows 10/11 o macOS.
- **Python:** Versión **3.11** o superior.
- **Hardware Mínimo Recomendado:** 4 GB de RAM, Procesador Dual-Core 2.0 GHz, 10 GB de almacenamiento SSD.
- **Terminales:** Cualquier tablet con navegador web moderno (Safari en iOS 14+, Chrome en Android 10+).

### 1. Clonar el Repositorio y Configurar Entorno Virtual
```bash
# Clonar repositorio
git clone https://github.com/tu-organizacion/gestion-pos.git
cd gestion-pos

# Crear entorno virtual
python -m venv venv

# Activar entorno virtual
# En Windows:
venv\Scripts\activate
# En Linux/macOS:
source venv/bin/activate

# Instalar dependencias
pip install -r requirements.txt
```

### 2. Configuración de Variables de Entorno (`.env`)
Crear un archivo `.env` en la raíz del proyecto tomando como referencia la siguiente plantilla:

| Variable | Tipo | Valor por Defecto | Descripción |
| :--- | :--- | :--- | :--- |
| `FLASK_ENV` | String | `production` | Modo de ejecución (`development` o `production`) |
| `FLASK_SECRET_KEY` | String | *(Generar aleatorio)* | Llave criptográfica para firmas de sesión de usuario |
| `PORT` | Entero | `5000` | Puerto TCP de escucha del servidor |
| `DB_TYPE` | String | `sqlite` | Motor de base de datos (`sqlite` o `mysql`) |
| `DB_PATH` | String | `inventory_sales.db` | Ruta del archivo de base de datos SQLite |
| `DB_HOST` | String | `localhost` | Host de conexión MySQL (si `DB_TYPE=mysql`) |
| `DB_PORT` | Entero | `3306` | Puerto de conexión MySQL |
| `DB_USER` | String | `archi_user` | Usuario de base de datos MySQL |
| `DB_PASSWORD` | String | `tu_password` | Contraseña de usuario MySQL |
| `DB_NAME` | String | `archi_db` | Nombre del esquema en MySQL |
| `GEMINI_API_KEY` | String | *(Opcional)* | Clave de API de Google Gemini para módulo OCR |
| `ADMIN_INITIAL_USERNAME` | String | `admin` | Usuario administrador creado en el primer inicio |
| `ADMIN_INITIAL_PASSWORD` | String | `Admin2026!` | Contraseña inicial (obligatorio cambiar tras login) |

### 3. Ejecutar el Servidor de Aplicación

#### En Entorno Windows:
Hacer doble clic en `run.bat` o ejecutar:
```cmd
run.bat
```

#### En Entorno Linux / Servidor Local:
```bash
python app.py
```
El servidor inicializará las 14 migraciones relacionales automáticamente y quedará disponible en `http://localhost:5000`.

### 4. Configuración para Tablets (PWA)
1. Conectar la tablet a la misma red local Wi-Fi o mediante VPN segura (**Tailscale**).
2. Abrir el navegador en la tablet e ingresar la IP local del servidor (ejemplo: `http://192.168.1.100:5000`).
3. Instalar como aplicación web nativa de pantalla completa:
   - **En iPad (Safari):** Pulsar botón Compartir > **"Agregar a pantalla de inicio"**.
   - **En Android (Chrome):** Menú de opciones (tres puntos) > **"Instalar aplicación"**.

---

### Modelo De Soporte Para Tablet En 3D

---

<img width="569" height="448" alt="3d" src="https://github.com/user-attachments/assets/01491150-1109-4096-ba9a-e93d1400b17a" />

---

## 5. Capturas de Pantalla del Sistema

Las siguientes vistas representan los módulos clave de la interfaz táctil:



---

### Terminal Punto de Venta Touch (POS)

---
<img width="1307" height="713" alt="image" src="https://github.com/user-attachments/assets/a9d581be-e2ab-481f-aeec-6e4169fccf48" />

---
<img width="1036" height="758" alt="pos3" src="https://github.com/user-attachments/assets/80eb175d-7135-44cf-8140-01903a811a01" />

---
<img width="1026" height="770" alt="pos" src="https://github.com/user-attachments/assets/6c097383-644d-4787-ad9a-989abb632854" />

---
<img width="1023" height="766" alt="pos2" src="https://github.com/user-attachments/assets/c7b503b3-55a1-42e8-9ad8-067c7aa52a1d" />

---

### Dashboard Financiero y Asignación de 4 Fondos
---

<img width="1890" height="915" alt="7" src="https://github.com/user-attachments/assets/9b6c169d-19a4-4429-8c27-1acba1330c28" />

---
<img width="1648" height="906" alt="Captura de pantalla 2026-10-22 021811" src="https://github.com/user-attachments/assets/1111ebe8-a073-47bd-84b7-7f547e069b9e" />

---
### Analisis & Metricas

---

<img width="1651" height="911" alt="Captura de pantalla 2026-10-22 022723" src="https://github.com/user-attachments/assets/c245d553-4298-4c49-b05a-cf5524fb465a" />

---

<img width="1644" height="920" alt="Captura de pantalla 2026-10-22 022746" src="https://github.com/user-attachments/assets/5a63e89d-e89d-40c1-aa86-9a2e63937ba4" />

---

<img width="1659" height="908" alt="Captura de pantalla 2026-10-22 022610" src="https://github.com/user-attachments/assets/c74e58af-477c-4d02-9565-2d822ed84c6b" />

---

<img width="1878" height="888" alt="15" src="https://github.com/user-attachments/assets/ddfdd030-669b-4f58-bc4a-c78162da1e52" />


---

<img width="1899" height="907" alt="13" src="https://github.com/user-attachments/assets/5bf4e3a1-498e-48bb-ac31-db262388d09d" />

---

<img width="1805" height="905" alt="14" src="https://github.com/user-attachments/assets/c6052fd0-1d8c-4643-ad50-72037e2fa31d" />

---


### Inteligencia de Inventario y Matriz ABC (Pareto)
---
<img width="1646" height="900" alt="Captura de pantalla 2026-10-22 021954" src="https://github.com/user-attachments/assets/c9e4d680-55a3-46d1-bf20-bc5dfd4a9700" />

---
<img width="1642" height="901" alt="Captura de pantalla 2026-10-22 022046" src="https://github.com/user-attachments/assets/f2c65596-b7a3-4f04-86e3-56f885a79b7a" />

---

### Control de Gastos y Visión Semestral
<img width="1023" height="768" alt="Captura de pantalla 2026-10-22 021215" src="https://github.com/user-attachments/assets/1fa1df14-a696-4d0b-abf7-ad9389cf44da" />

---

<img width="1653" height="902" alt="Captura de pantalla 2026-10-22 022429" src="https://github.com/user-attachments/assets/e3ad36f7-1e20-444f-8f4c-bbe8554ef576" />

---

<img width="1638" height="914" alt="Captura de pantalla 2026-10-22 022230" src="https://github.com/user-attachments/assets/a59cb5db-4bb4-4409-884d-ef4bad8535fd" />


---

<img width="1901" height="912" alt="11" src="https://github.com/user-attachments/assets/7074f58d-24ae-4b0a-90f5-36a4335ba411" />

---

<img width="1894" height="922" alt="12" src="https://github.com/user-attachments/assets/44330380-e5fd-4664-8d19-26c16545e33d" />

---
### Impuestos & F29

---

<img width="1913" height="925" alt="8" src="https://github.com/user-attachments/assets/286ca4bb-cab3-4f92-9866-e7b5b5bb4d78" />

---

<img width="1845" height="907" alt="9" src="https://github.com/user-attachments/assets/a6edcd8b-166c-4d96-ae57-351083e03179" />

---

<img width="1851" height="900" alt="10" src="https://github.com/user-attachments/assets/c00517d2-b3b4-42c2-bf96-eb4c7ed9a7b1" />


---
### Configuración del Sistema

---

<img width="1838" height="913" alt="a1" src="https://github.com/user-attachments/assets/87cdc877-ad2a-4b82-8416-78d33ce38724" />


---

<img width="1908" height="887" alt="a2" src="https://github.com/user-attachments/assets/8ec1b669-2d18-46a0-9549-b0ae840deaa4" />



---

## 6. Seguridad y Estándares Defensivos (OWASP & NIST)

El sistema implementa arquitectura de seguridad por capas en conformidad con **OWASP Top 10**:
- **Almacenamiento de Credenciales:** Hashing seguro mediante **PBKDF2-HMAC-SHA256 con 600.000 iteraciones** y salt criptográfico único de 16 bytes por cuenta.
- **Protección contra Inyecciones SQL:** 100% de consultas parametrizadas mediante Prepared Statements.
- **Mitigación de Ataques de Fuerza Bruta:** Limitador de tasa de peticiones (Rate Limiter) en memoria por dirección IP y cuenta de acceso.
- **Control de Acceso Basado en Roles (RBAC):** Segregación estricta de funciones entre perfiles de Administrador y Cajero. Los cajeros no tienen visibilidad de márgenes comerciales, costos ni tesorería.
- **Inspección Criptográfica de Archivos:** Validación de Magic Bytes en subida de imágenes y eliminación completa de metadatos EXIF.
- **Auditoría Inmutable:** Registro continuo de todas las operaciones sensibles en la tabla `audit_logs`.

---

## 7. Pruebas Automatizadas y Calidad de Código

El repositorio incluye una suite automatizada de pruebas unitarias y de integración que validan la lógica de negocio, consistencia transaccional y motores tributarios:

```bash
# Ejecutar suite de pruebas
python -m unittest test_system.py
```

Resultado verificado:
```text
Ran 79 tests in 33.911s
OK
```

---

## 8. Roadmap de Desarrollo

- [x] Motor de matriz de variantes y códigos de barra EAN-13 GS1.
- [x] Simulación y proyección del Formulario 29 (IVA + PPM).
- [x] Cuadratura de caja mediante visión artificial Google Gemini OCR.
- [x] Metodología de tesorería y regla de los 4 Fondos.
- [x] Arquitectura responsiva optimizada para tablets de 9.7 pulgadas.
- [ ] Integración directa con boleta electrónica del Servicio de Impuestos Internos (SII DTE vía API Bhe/Bhe-Boleta).
- [ ] Sincronización bidireccional con plataformas de e-commerce (Shopify / WooCommerce).
- [ ] Notificaciones automáticas de stock crítico y metas diarias a través de Webhook de WhatsApp Business.

---

## 9. Licencia y Contacto

### Licencia
Este proyecto es software privado y propietario. Todos los derechos reservados. El uso, distribución o modificación no autorizada está estrictamente prohibido bajo las leyes de propiedad intelectual de la República de Chile y tratados internacionales.

### Contacto y Soporte Corporativo
- **Organización:** ARCHI Gestión Comercial
- **Departamento de Ingeniería:** Tech Lead & Product Team
- **Sitio Web:** [https://archi-pos.com](https://archi-pos.com)
- **Consultas Comerciales e Inversión:** `contacto@archi-pos.com`
