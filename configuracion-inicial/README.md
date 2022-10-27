# Configuracion Inicial

En este documento encontrara lo necesario para llevar a cabo este laboratorio

> ##### Se instalara virtualbox y Vagrant para llevar a cabo esta practica, crearemos maquinas virtuales personalizadas utilizando el fichero _vagrantfile_

 El siguiente manual esta basado en los recursos de mi computador personal

> Procesador: Intel core i5 11th

> RAM:16 GB

> Hard Disk: 480 GB SSD

> SO: Windows 10 Home

Puntos necesarios para instalar el entorno de este laboratorio

- [ ] [Install VirtualBox](#install-vb)
- [ ] [Install Vagrant](#install-v)
- [ ] [Iniciar maquina virtual personalizada(Vagrantfile)](#init)

<a name="install-vb"></a>
### Instalación de VirtualBox

VirtualBox es una aplicacion que sirve para virtualizar SO en un ambiente controlado, podemos virtualizar varios sistemas o uno en especifico el cual seria nuestro ambiente de trabajo. En este caso lo vamos a utilizar para instalar in ambiente asilado de nuestro sistema operativo principal.

1. Descargar e Instalar la última versión estable de **VirtualBox** para Windows [aqui](https://download.virtualbox.org/virtualbox/6.1.40/VirtualBox-6.1.40-154048-Win.exe)

> Este programa lo instalamos con todas las configuraciones por defecto

# Instalacion de Vagrant

Vagrant es una herramienta o aplicación de líneas de comando utilizada en el sector IT, especialmente por desarrolladores. Permite la creación de entornos de desarrollo virtualizados que pueden ser reproducidos y compartidos de una forma muy fácil.

1. Descargar e Instalar la última versión estable de **Vagrant** para Windows [aqui](https://releases.hashicorp.com/vagrant/2.3.2/vagrant_2.3.2_windows_i686.msi)

> Una vez descargado el programa procedemos a instalarlo con las configuraciones por defecto

2. Una vez terminada la instalacion nos solicitara reinicar nuestro equipo para que el PowerShell de windows pueda reconocer vagrant

3. Procedemos a abrir la linea de comandos "CLI" Powershell. Verificamos si el CLI powerShell detecta los comandos de vagrant
`vagrant`

```powershell
vagrant --help
```
<a name="init"></a>
### Iniciar máquina virtual personalizada

Utilizamos vagrantfile para crear nuestras maquinas virtuales personalizadas, si abrimos el archivo Vagrantfile podemos observar la cantidad de nodos,SO,recursos de cada una de ellas, es importante saber que vagrant está diseñado para trabajar con un Vagrantfile por proyecto.

El siguiente archivo Vagrantfile cuenta con las provisiones necesarias para llevar acabo nuestro laboratorio. Siga los siguentes pasos para crear su poyecto de vagrant personalizado.

1. Defimos un directorio para crear proyectos de Vagrant. En mi caso utilice `Documentos/laboratorios/ansible-install`

2. Dentro del directorio `Documentos/laboratorios/ansible-install`, copie el archivo `Vagrantfile` que se encuentra disponible en el ![repositorio](install-ansible/infraestructura/Vagrantfile)

3. Iniciamos el CLI de Windows PowerShell y nos dirigimos a nuestro directorio en donde esta alojado el archivo Vagrantfile `cd Documentos/laboratorios/ansible-install`

4. Una vez ubicados en el directorio correspondiente  iniciamos nuestra maquina personalizada con el siguiente comando:

```powershell
vagrant up
```
> Esto se estaria demorando dependiendo de los recursos de nuestro computador y la velocidad de nuestra conexion a internet