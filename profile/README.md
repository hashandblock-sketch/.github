<!--
  README de la portada de Hash and Block en GitHub.
  Va en el repositorio .github, en profile/README.md. Las imágenes van en profile/assets/.
  Si cambias el nombre de la organización, reemplaza "hashandblock-sketch" en las direcciones de las imágenes.
-->

<div align="center">

<a href="https://wwwhashandblock.com/"><img src="https://raw.githubusercontent.com/hashandblock-sketch/.github/main/profile/assets/hero.svg" alt="Hash and Block, notaría digital. Demuestra que tu documento no ha cambiado." width="100%"></a>

<br><br>

<a href="https://wwwhashandblock.com/"><img alt="Sitio web: wwwhashandblock.com" src="https://img.shields.io/badge/Sitio%20web-wwwhashandblock.com-D4AF37?style=for-the-badge&labelColor=0B0B0C"></a>
<img alt="Estado: MVP en construcción" src="https://img.shields.io/badge/Estado-MVP%20en%20construcci%C3%B3n-D4AF37?style=for-the-badge&labelColor=0B0B0C">
<img alt="Huella: SHA-256" src="https://img.shields.io/badge/Huella-SHA--256-D4AF37?style=for-the-badge&labelColor=0B0B0C">
<img alt="Verificar: Siempre gratis" src="https://img.shields.io/badge/Verificar-Siempre%20gratis-D4AF37?style=for-the-badge&labelColor=0B0B0C">
<img alt="Hecho en: Ecuador" src="https://img.shields.io/badge/Hecho%20en-Ecuador-D4AF37?style=for-the-badge&labelColor=0B0B0C">

<br><br>

<b>Registramos la huella digital de tus documentos y la sellamos en el tiempo.</b><br>
Así demuestras después que un archivo no cambió, sin subir nunca su contenido.

<br><br>

<img src="https://raw.githubusercontent.com/hashandblock-sketch/.github/main/profile/assets/divider.svg" alt="" width="100%">

<img src="https://raw.githubusercontent.com/hashandblock-sketch/.github/main/profile/assets/que-hacemos.svg" alt="Qué hacemos: huella SHA-256, sello de tiempo verificable y certificado." width="100%">

<br><br>

<a href="https://wwwhashandblock.com/"><img src="https://raw.githubusercontent.com/hashandblock-sketch/.github/main/profile/assets/demo.svg" alt="Demostración: cambiar 1.000 por 1,000 en un contrato produce una huella SHA-256 totalmente distinta." width="100%"></a>

<sub>👆 Pruébalo con tus propios archivos en <a href="https://wwwhashandblock.com/"><b>wwwhashandblock.com</b></a>. La huella se calcula en tu navegador.</sub>

<br><br>

<img src="https://raw.githubusercontent.com/hashandblock-sketch/.github/main/profile/assets/como-funciona.svg" alt="Cómo funciona en 4 pasos: eliges el archivo, se calcula la huella, se registra con sello de tiempo y cualquiera verifica gratis." width="100%">

</div>

<br>

<h3 align="center">🔍 Compruébalo tú mismo, sin depender de nosotros</h3>
<p align="center">Cualquier computadora puede calcular la huella de un archivo. Abre tu sistema y compara el resultado con el certificado.</p>

<details>
<summary><b>&nbsp;🪟&nbsp; Windows</b> · PowerShell</summary>

```powershell
Get-FileHash .\contrato.pdf -Algorithm SHA256
```
</details>

<details>
<summary><b>&nbsp;🍎&nbsp; macOS</b> · Terminal</summary>

```bash
shasum -a 256 contrato.pdf
```
</details>

<details>
<summary><b>&nbsp;🐧&nbsp; Linux</b> · Terminal</summary>

```bash
sha256sum contrato.pdf
```
</details>

<details>
<summary><b>&nbsp;⚡&nbsp; JavaScript</b> · en el navegador, como lo hace nuestra web</summary>

```js
async function sha256(file) {
  const buf = await crypto.subtle.digest('SHA-256', await file.arrayBuffer());
  return [...new Uint8Array(buf)].map(b => b.toString(16).padStart(2, '0')).join('');
}
```
</details>

<br>

<div align="center">

<img src="https://raw.githubusercontent.com/hashandblock-sketch/.github/main/profile/assets/divider.svg" alt="" width="100%">

<img src="https://raw.githubusercontent.com/hashandblock-sketch/.github/main/profile/assets/que-demuestra.svg" alt="Qué demuestra una huella y qué no." width="100%">

<br><br>

<img src="https://raw.githubusercontent.com/hashandblock-sketch/.github/main/profile/assets/hoja-de-ruta.svg" alt="Hoja de ruta en 5 etapas; la etapa 1 está en curso." width="100%">

<sub><b>Hoy existe:</b> la <a href="https://wwwhashandblock.com/">página web</a>, que calcula y compara huellas SHA-256 en tu navegador. Los registros y certificados llegan en las próximas etapas.</sub>

<br><br>

<img src="https://raw.githubusercontent.com/hashandblock-sketch/.github/main/profile/assets/equipo.svg" alt="Equipo de Hash and Block." width="100%">

<br><br>

<a href="https://mail.google.com/mail/?view=cm&fs=1&to=hashandblock@wwwhashandblock.com&su=Quiero%20ser%20empresa%20piloto"><img src="https://raw.githubusercontent.com/hashandblock-sketch/.github/main/profile/assets/piloto.svg" alt="Quiero ser empresa piloto. Escríbenos." width="100%"></a>

<sub>¿No usas Gmail? Escríbenos a <b>hashandblock@wwwhashandblock.com</b></sub>

<br><br>

<img src="https://raw.githubusercontent.com/hashandblock-sketch/.github/main/profile/assets/divider.svg" alt="" width="100%">

<sub>
Hash and Block ofrece pruebas técnicas de integridad y registro temporal de archivos.<br>
No sustituye a un notario público ni a una firma electrónica, y no acredita la identidad de los firmantes ni la validez jurídica de un documento.<br><br>
© 2026 Hash and Block · Ecuador
</sub>

</div>
