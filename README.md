# Laboratorio de Redes.
    Tp, practicas y apuntes de materia Laboratorio de redes. IFTS 2023

# Instrucciones.
    Para poder ejecutar el documento 5.pk se debe descargar e instalar SiscoPacketTracer en alguna de sus versiones.

# Datos del Laboratorio
    
    # Red 1 Gerencial 
    172.168.1.0 - CLASE B:
    255.255.0.0 - Mask 
    172.168.1.1 - Gateway
    172.168.1.20 > Nodos en adelante.
    --------------- 
    172.168.1.10 - DHCP
    172.168.1.11 - DNS
    172.168.1.12 - WebServer 
    
    # Red 2 Ventas 
    192.160.1.0 - CLASE C
    255.255.255.0 - Mask
    192.160.1.1 - Gateway
    192.160.1.10 > Nodos en adelante.

    # Red VLan (Ventas1)
    Puertos de F0/1-5
    uno de los nodos con conexion Trunk a puertos F0/24 en ambos switch.
    
    # 172.168.1.12 - WebServer
    Con dos paginas accesibles a todos los nodods de la red excepto Vlan (Ventas1). 
    www.grupo5.com
    
    # 172.168.1.10 - DHCP
    Asignacion automatica de direcciones IP a los nodos de la red (Gerencia)
    Ip fijas en las red (Lan Ventas) y red (VLan ventas1) 
    
    # 172.168.1.11 - DNS
    DNS en la red LAN (Administracion) que resuelve www.grupo5.com
    
    # Segurridad
    Los switch de ambas redes tienen configurada password y user para permitir acceso.
    User: grupo5
    pass:grupo5
    
    El router tiene configurada pass para permitir acceso.
    Pass: grupo5
    
  
# Notas del Laboratorio.

    Usando CISCO Packet Tracer (versión 5.3.2 en adelante) diseñar una red con las siguientes
    características:
    
    1. 1 Router que enrute 2 redes diferentes de 2 Switches, en las cuales:
    a. 1 Switch con una red CLASE C (que NO sea el rango del ej. en clase)
    b. 1 Switch con una red CLASE B (que NO sea el rango del ej. en clase)
    c. Configurar Default Gateway para que el Router pueda enrutar datos entre las
    2 redes.
    
    2. A un switch configurar:
    a. 1 Servidor DHCP
    b. 1 Servidor DNS
    c. 1 Servidor WEB (Con una IP fija y que el DNS convierta su nombre y pueda
    verse la web en esa subred)
    
    3. Al otro switch (o al mismo) configurar:
    a. 1 VLAN con 3 nodos/computadoras cada uno (elegir el número y nombre de
    VLAN que quieran y los rangos de puertos que deseen)
    b. Conectar otro Switch (Switch a Switch) en modo Trunk con 2
    nodos/computadoras que sean de alguna de las otras 2 VLANs del otro
    Switch.
    Aclaración: En este caso, como no se pide configurar servidor DHCP, queda
    a elección si quieren igualmente agregarlo, o si prefieren configurarlo con IPs
    estáticas.

    4. Seguridad: Ponerle password a los switches y al router. OPTATIVO
    REQUISITOS:
    - Hacer ping entre nodos/computadoras entre una red a otra.
    - Acceder a la WEB del servidor en otros nodos/computadoras tanto con IP como con
    DNS.
    - Funcionamiento del servidor DHCP para asignar IP, Máscara, DHCP y DNS.
    - Poner labels con información importante (IPs, nombres de servidores, interfaces,
    etc)
    - ¡Todo aquello adicional que prueben y quieran agregar es optativo y bienvenido!

    PREGUNTAS PARA INTEGRANTES DEL GRUPO
    - ¿Cómo configuraron el Switch?
    - ¿Qué clases usaron entre las dos diferentes redes? ¿Qué rango de IPs?
    - ¿Qué clases usaron en esos rangos de IPs?
    - ¿Cómo configuraron el router?
    - ¿Cómo configuraron la VLAN?
    - ¿Hicieron Trunk entre VLANs? ¿Para qué sirve?
    - Probar Ping de 2 nodos entre una red a otra.
    - Modo simulación probar enviar un paquete simple.
    - ¿Cómo configuraron el DNS? ¿Para qué sirve?
    - ¿Cómo configuraron el DHCP? ¿Para qué sirve?
    - ¿Cómo configuraron el DNS? ¿Para qué sirve?
    - ¿Cómo configuraron el WEB Server? ¿Para qué sirve?
    - ¿Le pusieron seguridad? ¿Cómo pusieron password al router y/o switch? OPTATIVO
    - ¿Pusieron Labels? ¿Usaron algún tipo de procedimiento/políticas para los nombres,
    rangos de IP, etc?
