#Proyecto vacío para aprender como utilizar Travis CI en PlatformIO [![Build Status](https://travis-ci.org/wifixcort/travis_test.svg?branch=master)](https://travis-ci.org/wifixcort/travis_test)

Todo lo estoy haciendo desde PlatformIO, por lo que esté prepara el archivo de Travis
de antemano junto con algunas configuraciones útiles.

Para empezar créo un archivo main.cpp e incluyo la librería de arduido junto con
el setup y el loop que deben estar en cualquier sketch de arduino

Luego de subir el repositorio ir a la cuenta personal de travis-ci.org y activar
travis en el repositorio.

El archivo .travis.yml puede no subirse al repositorio ya que git lo ignora, si
sucede simplemente ponemos "git add .travis.yml"

Si el repositorio no aparece, al lado derecho hay un botón de "Sync account".

Luego de que travis fué activado pueden hacerse configuraciones adicionales

Para realizar un primer test solamente descomentar el "Template #1" y realizar
el commit y push al repositorio de github

Aunque el template #1 especifíca que los archivos deberían ser de python, cuando travis
encuentre el main.cpp lo va a compilar como debe sin problemas(Recordar que platformio
  preparó algunas cosas por nosotros).

Para añadir el icono al repositorio del estado del mismo, en la plataforma de Travis
hacer click en la imagen de "build|passing" (Si ya logramos hacer que pasara correctamente),
nos aparecerá un "Pop-Up" con la palabra "Status Image", elegimos el branche al que
se lo queremos aplicar y nos genera el link que necesitamos.

Copiamos y pegamos ese link junto al titulo del readme.md como aparece en este repositorio
