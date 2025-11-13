# Sistema de Facturación Electrónica - SUNAT

Sistema completo de facturación electrónica integrado con los servicios de SUNAT para ACUÑA LOLY DIKSON YAMPIER.

## Características

### Generación de Facturas
- Generación de facturas electrónicas
- Cálculo automático de IGV (18%)
- Exportación a PDF
- Generación de XML UBL 2.1

### Integración con SUNAT
- **Control CPE** (`/v1/contribuyente/controlcpe`): Verifica el estado de comprobantes electrónicos
- **MIGE IGV** (`/v1/contribuyente/migeigv`): Gestión de libros electrónicos (RCE y RVIE)
- **GRE Emisión** (`/v1/contribuyente/gem`): Emisión de comprobantes electrónicos
- **Control Mensajes** (`/v1/contribuyente/controlmsg`): Consulta de alertas y errores de SUNAT
- **SSPP Receptor** (`/v1/contribuyente/enviossp`): Envío de XML para procesamiento

## Uso

1. Abre el archivo `index.html` en tu navegador o visita la página en GitHub Pages
2. Ve a la pestaña "Configuración" e ingresa tus credenciales SOL de SUNAT
3. Usa las diferentes pestañas para gestionar tus comprobantes electrónicos

## Servicios SUNAT Implementados

| Servicio | Endpoint | Función |
|----------|----------|---------|
| Control CPE | `/v1/contribuyente/controlcpe` | Verificar estado de facturas, boletas, notas |
| MIGE IGV | `/v1/contribuyente/migeigv` | Enviar/consultar libros electrónicos |
| GRE Emisión | `/v1/contribuyente/gem` | Emitir comprobantes electrónicos |
| Control Mensajes | `/v1/contribuyente/controlmsg` | Gestionar alertas y errores |
| SSPP Receptor | `/v1/contribuyente/enviossp` | Enviar XML para procesamiento |

## Tecnologías

- HTML5
- CSS3
- JavaScript (ES6+)
- jsPDF
- html2canvas
- Fetch API para integración con SUNAT

## Notas Importantes

- Requiere credenciales SOL (Sistema de Operaciones en Línea) de SUNAT
- La configuración se guarda localmente en el navegador
- Los XML generados siguen el estándar UBL 2.1 de SUNAT
- Para producción, asegúrate de usar el entorno correcto de la API de SUNAT

