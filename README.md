# Validador de Series de Billetes - Bolivia (No Oficial) 🇧🇴

Esta es una Aplicación Web Progresiva (PWA) diseñada como una herramienta de ayuda social para la verificación rápida de series de billetes del Estado Plurinacional de Bolivia. Utiliza la cámara del dispositivo y reconocimiento óptico de caracteres (OCR) mediante Inteligencia Artificial para extraer el número de serie de un billete y compararlo contra una base de datos de series reportadas.

**Desarrollado por:** Hugo Velarde - Fullstack Developer

---

## 🚀 Características Principales

* **Reconocimiento local (Privacidad):** Todo el procesamiento de la imagen (OCR) se realiza directamente en el navegador del dispositivo del usuario. Ninguna imagen o dato es enviado a servidores externos.
* **Inteligencia Artificial:** Implementa `Tesseract.js` para extraer con precisión cadenas alfanuméricas (9 dígitos + Letra A/B) del papel moneda.
* **Instalable (PWA):** Puede ser instalada en la pantalla de inicio de dispositivos móviles Android e iOS para funcionar como una aplicación nativa.
* **Interfaz Responsiva:** Construida con HTML5, Vanilla JavaScript y Tailwind CSS para una experiencia fluida y moderna.

---

## 📱 Guía de Uso (Tutorial)

Para obtener los mejores resultados y evitar errores de lectura, sigue estos pasos:

1. **Selecciona la Denominación:** En la pantalla principal, presiona el botón correspondiente al billete que deseas verificar (10 Bs., 20 Bs., o 50 Bs.).
2. **Concede Permisos:** Si el navegador lo solicita, permite el acceso a la cámara.
3. **Encuadre Correcto:** * Coloca el billete en una superficie plana y bien iluminada.
   * Evita sombras directas o reflejos de luz sobre el papel.
   * Alinea **exclusivamente el número de serie y la letra final (A o B)** dentro del recuadro rojo que aparece en pantalla.
   * No acerques demasiado el celular; permite que la cámara enfoque correctamente los números.
4. **Captura:** Mantén el pulso firme y presiona "CAPTURAR SERIE".
5. **Resultado:** La IA procesará la imagen y te indicará si la serie se encuentra en la base de datos de billetes observados (INVÁLIDO) o si no está reportada (VÁLIDO).

---

## ⚖️ Descargo de Responsabilidades (Disclaimer Legal)

**LEER ATENTAMENTE ANTES DE UTILIZAR ESTE SOFTWARE.**

Al utilizar esta aplicación ("Validador de Series de Billetes"), el usuario acepta incondicionalmente los siguientes términos:

1. **Naturaleza del Software:** Esta aplicación es un proyecto de desarrollo de software independiente creado con fines estrictamente educativos, informativos y de ayuda social. **NO ES UNA APLICACIÓN OFICIAL** y no tiene ningún tipo de afiliación, patrocinio, ni respaldo por parte del Banco Central de Bolivia (BCB), ni de ninguna otra entidad gubernamental o financiera.
2. **Precisión de los Datos:** La base de datos de rangos de series invalidas incrustada en el código fuente de esta aplicación fue recopilada a partir de reportes públicos en un momento específico en el tiempo. El desarrollador **NO GARANTIZA** que esta información esté completa, actualizada o libre de errores. El BCB puede actualizar sus listas en cualquier momento sin que esto se refleje de forma inmediata en esta aplicación.
3. **Limitaciones Tecnológicas:** El reconocimiento óptico de caracteres (OCR) depende de factores externos fuera del control del software, tales como la calidad de la cámara del dispositivo del usuario, la iluminación ambiental, el desgaste físico del billete y el enfoque. Por tanto, el software puede arrojar **FALSOS POSITIVOS** o **FALSOS NEGATIVOS**.
4. **Exención Total de Responsabilidad:** El resultado arrojado por esta aplicación ("VÁLIDO" o "INVÁLIDO") debe tomarse **ÚNICAMENTE COMO UNA REFERENCIA PREVENTIVA**. El usuario es el único y absoluto responsable de las decisiones financieras o comerciales que tome basándose en el uso de esta herramienta.
5. **Indemnización:** Hugo Velarde (el desarrollador), los colaboradores del repositorio y los proveedores de hosting renuncian expresamente a cualquier tipo de responsabilidad legal, civil, penal o económica derivada del uso, mal uso, o incapacidad de uso de esta aplicación. En ningún caso el desarrollador será responsable por daños directos, indirectos, incidentales, lucro cesante o pérdidas financieras que pudieran resultar de la aceptación o rechazo de papel moneda tras el uso de este software.

**El usuario asume el 100% del riesgo al emplear esta herramienta.**

---

## 🛠️ Tecnologías y Dependencias

* [HTML5 / Vanilla JS] - Estructura y lógica del cliente.
* [Tailwind CSS](https://tailwindcss.com/) - Framework de estilos y diseño UI.
* [Tesseract.js](https://tesseract.projectnaptha.com/) - Motor OCR (Optical Character Recognition) en WebAssembly.