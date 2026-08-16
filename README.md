# Biblioteca de Leyes de Nicaragua

Repositorio de referencias legales nicaragüenses (texto extraído + metadata estructurada), organizado por categoría, como fuente de datos para herramientas de análisis fiscal y legal con IA.

## Estructura

Cada ley/decreto vive en su propia carpeta con dos archivos:

- `texto-extraido.md` — texto completo extraído del PDF original, con marcadores de página para trazabilidad.
- `metadata.yaml` — ficha con categoría, número de páginas, artículos detectados, estado de vigencia y fecha de última verificación.

## Categorías

### civil-comercial (2 documentos)
- Código Civil de Nicaragua -2019
- Código de Comercio de Nicaragua

### competencia (1 documentos)
- Texto Consolidado, Ley N°. 601, Ley de Promoción de la Competencia

### consumidor (2 documentos)
- Ley de Reformas y Adición a la Ley N°. 842, Ley de Protección de los Derechos de las Personas Consumidoras y Usuarios
- Texto Consolidado, Ley Nº. 842, Ley de Protección de los Derechos de las Personas Consumidoras y Usuarias

### financiero (3 documentos)
- Ley Nº. 977, Ley Contra el Lavado de Activos
- Normativa de Registro de Sujetos Obligados ante la Unidad de Análisis Financiero
- Ley 1215 de Reformas y Adiciones a La Ley 977

### inversion-extranjera (2 documentos)
- Ley de Inversiones Extranjeras - Ley 1240
- Reglamento Ley 1240

### municipal (3 documentos)
- Decreto-10-91-Plan-de-Arbitrios-del-Municipio-de-Managua
- Decreto-3-95-Impuesto-de-Bienes-Inmuebles
- Decreto-455-Plan-de-Arbitrios-Municipal

### regulatorio (8 documentos)
- 09_Ley_No_587_Ley_de_Mercado_de_Capiltales
- Decreto Ejecutivo N°. 15-2018, Reglamento de la Ley N°. 977
- Decreto-No.-49-92-Reforma-a-la-Ley-Organica-del-Instituto-Nicaraguense-de-Telecomunicaciones-y-Correos-Telcor
- Ley General de Telecomunicaciones Convergentes
- Ley General de Turismo
- Ley de Reforma al Decreto-Ley N°. 1053, Ley Orgánica del Instituto Nicaragüense de Telecomunicaciones y Correo (TELCOR)
- Reglamento de la Ley N°. 1210, Ley General de Turismo
- “Normativa de Cánones y Tarifas por Trámites Administrativos y Regulatorios de Telecomunicaciones”

### tributario (1 documentos)
- Código tributario Con reformas

### zonas-francas (2 documentos)
- Ley 917 Ley de Zonas Francas
- Reglamento de la Ley N°. 917 Ley de Zonas Francas de Exportación

## Pendientes de OCR

Estos archivos tienen muy poco o ningún texto extraíble (probablemente escaneados como imagen) y requieren OCR antes de poder usarse en el pipeline de IA:

- Ley N 1003, Ley del Digesto Jurídico Nicaragüense de la Materia Telecomunicaciones y Servicios Postales.pdf (regulatorio)
- Empresas Inactivas y en Suspensión Temporal ZF.pdf (zonas-francas)

## Estado de vigencia

Cada ley se verifica manualmente antes de incluirse en el repositorio. La fecha de esa verificación queda registrada en `metadata.yaml` (`fecha_verificacion`). **Nota:** los campos `numero`, `fecha_publicacion` y `reformas` en varios metadata.yaml quedaron como plantilla — deben completarse manualmente por ser datos legales que no se pueden inferir de forma confiable desde el texto.

## Próximos pasos sugeridos

- Completar campos legales pendientes en metadata.yaml (número de ley, gaceta, fecha de publicación, reformas).
- Aplicar OCR a los documentos escaneados.
- Automatizar verificación periódica de vigencia (cruce con publicaciones nuevas en La Gaceta).

### comparativos (1 documentos, agregado después)
- Ley 987 LCT 822 COMPARATIVO 2019-1_ EJCE 1 (subido manualmente por el usuario tras fallo de descarga)
