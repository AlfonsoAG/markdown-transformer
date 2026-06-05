# MD Transformer

MD Transformer es un notebook de Google Colab para convertir documentos a Markdown limpio. Está pensado para transformar PDFs, imágenes escaneadas, documentos de Word y otros archivos de Office en texto estructurado que pueda usarse como contexto para herramientas de IA.

El problema que resuelve es simple: muchos documentos contienen información útil, pero vienen en formatos difíciles de consultar, fragmentar o reutilizar sin perder estructura. Markdown permite conservar títulos, tablas, páginas y bloques de texto en un formato legible, ligero y fácil de pasar a un modelo de lenguaje.

## Formatos soportados

El notebook puede procesar archivos como:

- PDF, incluyendo PDFs con texto y PDFs escaneados.
- Imágenes: PNG, JPG, JPEG, WEBP, TIFF y BMP.
- Word: DOCX y DOC.
- Excel y datos tabulares: XLSX, XLS y CSV.
- PowerPoint: PPTX y PPT.
- Otros formatos compatibles con MarkItDown, como HTML, TXT, JSON, XML, EPUB y ZIP.

## Librerías utilizadas

- **MarkItDown**: convierte archivos comunes de Office y otros formatos a Markdown.
- **pdfplumber**: extrae texto de PDFs cuando el documento ya contiene texto seleccionable.
- **PyMuPDF / pymupdf4llm**: convierte PDFs a Markdown y ayuda a detectar documentos escaneados.
- **pytesseract**: ejecuta OCR para extraer texto desde imágenes y PDFs escaneados.
- **Pillow**: abre y prepara imágenes para OCR.
- **pandas**: convierte hojas de cálculo y CSV a tablas en Markdown.
- **python-docx, python-pptx, openpyxl**: dan soporte adicional para documentos de Office.
- **rich y tqdm**: muestran progreso y resultados de procesamiento dentro de Colab.

## Uso

1. Abre el notebook en Colab desde el badge **Open in Colab**.
2. Carga uno o varios archivos en el entorno de Colab y ejecuta las celdas.
3. Descarga los archivos `.md` generados.

## Casos de uso

- Convertir contratos a Markdown para analizarlos con una IA sin perder secciones, cláusulas o tablas.
- Transformar documentos legales, políticas internas o expedientes en contexto reutilizable.
- Pasar reportes financieros, auditorías o presentaciones a texto estructurado.
- Extraer texto de PDFs escaneados o imágenes mediante OCR.
- Preparar archivos de soporte para sistemas RAG, asistentes internos o flujos de análisis documental.
- Convertir documentos largos en archivos `.md` más fáciles de versionar, revisar y resumir.

## Roadmap

- Procesamiento por lotes con empaquetado automático en ZIP.
- Integración con APIs para enviar el Markdown a modelos de IA o sistemas RAG.
- Mejor detección automática del mejor motor de conversión por tipo de archivo.
- Soporte ampliado para más formatos documentales.
- Limpieza avanzada de Markdown: encabezados, tablas, saltos de página y metadatos.
- Opciones configurables para idioma de OCR, nombres de salida y nivel de detalle.

## Licencia

Este proyecto se distribuye bajo licencia MIT.

## Autor

Creado por [Alfonso Aguilar Grimaldo](https://www.linkedin.com/in/aguilargrimaldo96/).
