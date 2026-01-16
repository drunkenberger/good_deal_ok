# CHANGE_LOG.md

## Registro de Cambios Exitosos

[2026-01-14] Corregido cálculo de PI para aplicarse sobre utilidad neta | Archivos: propuesta-alianza-dashboard.html | Estado: ✅ Exitoso
- Modificada función `calculateProfit()` para calcular PI después de descontar gastos
- Actualizado HTML del "Resumen de Utilidad" mostrando flujo correcto: Valor total → Gastos → Utilidad bruta → PI → Utilidad neta

[2026-01-14] Agregado módulo de Venta de Licencias | Archivos: propuesta-alianza-dashboard.html | Estado: ✅ Exitoso
- Nueva sección "Venta de Licencias" con badge "Nuevo"
- Formulario para agregar productos (nombre, precio, tipo de licencia, costo por unidad)
- Tabla dinámica con cálculo automático de ingresos, utilidad bruta y PI
- Tarjetas de resumen: Ingresos Totales, Costos Totales, Utilidad Bruta, Tu Participación
- Proyección de ventas con tasa de crecimiento mensual
- Integración con cálculos principales (updateAllCalculations)
- Sincronización con cambios en el porcentaje de PI global
- Icono 🎫 agregado en la navegación lateral

[2026-01-14] Mejorado diseño del módulo de Licencias | Archivos: propuesta-alianza-dashboard.html | Estado: ✅ Exitoso
- Nuevo estilo `.cost-section.licenses` con gradiente amarillo/dorado coherente con tema de ingresos
- Botones preset rápidos para productos comunes (Chatbot IA, SaaS Tool, Plugin, API, Template, Curso)
- Formulario rediseñado con grid responsive y labels descriptivos
- Botón "Agregar" con estilo `.btn.btn-success` (verde) consistente con la app
- Badges de tipo de licencia con colores distintivos (azul=único, verde=mensual, dorado=anual)
- Input de cantidad vendidas estilizado con focus dorado
- Botón eliminar con estilo consistente (× rojo con hover)
- Mensaje de estado vacío mejorado con emoji y texto descriptivo
- Sección de proyección con contenedor estilizado (fondo dorado sutil)
- Responsive design para móvil (grid adaptativo en 3 breakpoints)
- Función `addPresetLicense()` para agregar productos con un click

[2026-01-15] Agregado sistema de exportación HTML y JSON | Archivos: index.html | Estado: ✅ Exitoso
- Nueva función `exportToHTML()` para descargar propuesta como archivo HTML standalone
- Nueva función `exportToJSON()` para exportar configuración completa en formato JSON
- Nueva función `handleJSONImport()` para importar configuración desde archivo JSON
- Botones de exportación: 🌐 Descargar HTML, 📦 Exportar JSON, 📥 Importar JSON
- JSON incluye: configuración base, proyectos con gastos, referidos, licencias, equity, breakeven
- Permite compartir configuración con otras personas para cargarla en otro host
- Corregidos IDs de elementos: projectsData.projects, state.referrals, licenseProducts
- Integración con funciones existentes: renderProjectSelector(), updateReferralsTable(), renderLicensesTable()
