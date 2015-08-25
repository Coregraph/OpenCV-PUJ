#Informe de ejecucion y puesta en marcha de Calibracion de Camara utilizando OpenCV#

##Consideraicones Iniciales##
Para la ejecicion de este proyecto se cuenta con unas restricciones de maquina:
* Camara iSight 1.3mp
* Macbook Pro core i5 4gb Ram

##Instalación##
En OSX el proceso de instalacion de OpenCV 3.0 es un poco diferente al proceso en otros sistemas Unix. La compilaicon manual de las librerias es un proceso que requiere muchos componentes adicionales que hay que instalar de antemano. Razon por la cual se procede a hacer la instalacion mediante un manejador de paquetes para Mac OSX que se llama "brew", la instalacion de openCV pasa a ser un proceso simple con un unico comando.

{code}brew install opencv3 --c++11 --with-cuda --with-contrib --with-tbb --with-qt5 --with-gstreamer --with-opengl --with-openni --with-contrib{code}

Esta linea de codigo descarga y configura OpenCV para ser usado como una libreria estatica en los proyectos siguientes.

Luego de esto se procede a configurar el metodo de compilacion para los proximos proyectos de OpenCV, este proceso se realiza mediante el uso de Cmake, el cual se encarga de compilar los codigos c++ que ejecuten OpenCV. Este proceso genera un archivo de configuracion CMakeList que realiza la compilacion correcta de un ejecutable con las librerias de OpenCV.

##Calibracion de Camara##

