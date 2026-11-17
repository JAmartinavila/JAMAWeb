JAMAWeb — actualización de la sección Divulgación
=================================================

Este parche está pensado para el repositorio JAMAWeb que ya tiene publicada
la pestaña Divulgación/Outreach de la entrega anterior.

ARCHIVOS QUE DEBES COPIAR:
  - Outreach.qmd  (reemplazar)
  - styles.css    (reemplazar)

PASOS:
1. En GitHub Desktop, elige CURRENT REPOSITORY: JAMAWeb.
2. Repository > Show in Explorer.
3. Haz una copia de los dos archivos actuales antes de sobrescribirlos.
4. Pega Outreach.qmd y styles.css en la raíz del repositorio JAMAWeb.
   NO borres la carpeta .git ni sustituyas otras carpetas.
5. Verifica Changes; escribe un commit como "Add outreach media links".
6. Commit to main > Push origin.
7. En GitHub > Actions, comprueba Quarto Publish.
8. En la web publicada, abre la pestaña Divulgación y prueba los enlaces.

QUÉ SE INCLUYE:
- Cárabos: historia personal, cámaras SEO/BirdLife y anillamiento 2025.
- iVoox Cascando de Ciencia, reportaje Labranza de TVG y entrevista de RNE.
- Gciencia, Faro de Vigo, madri+d y prensa de la UAH.
- FameLab: elDiario.es, elEconomista, entrevista UAH y nota de FECYT.
- Charla de 2022 en el Aula Apícola del Jardín Botánico UAH.
- Nós Diario figura como investigación relacionada de otro equipo.

NOTAS:
- Este parche no toca index.qmd, _quarto.yml, los archivos R ni la foto.
- En algunos sitios la página externa puede ser de acceso restringido o
  no accesible desde determinados países; los enlaces siguen siendo externos.
- No hay que copiar el archivo README_ENLACES.txt al repositorio.
- El ZIP incluye URLs facilitadas por el usuario y otras dos fuentes públicas
  (entrevista UAH y RNE). No se incrusta material con copyright ajeno.
