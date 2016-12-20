Empty project for learn to use travis in platformIO

Luego de subir el repositorio ir a la cuenta personal de travis-ci.org y activar
travis en el repositorio.

El archivo .travis.yml puede no subirse al repositorio ya que git lo ingnora si
simplemente ponemos "git add *" por lo que hay que ser específico y subirlo con
"git add .travis.yml"

Si el repositorio no aparece, al lado derecho hay un botón de "Sync account".

Luego de que travis fué activado pueden hacerse configuraciones adicionales

Para realizar un primer test solamente descomentar el "Template #1" y realizar
el commit y push al repositorio de github
