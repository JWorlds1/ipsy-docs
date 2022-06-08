VNC on Linux/MacOS/Windows (with Putty) 
********

Download VNC Viewer to the device you want to control.

Make sure you have downloaded VNC® Connect to the computer you want to control.

Download VNC Viewer and VNC Connect, for Linux/MacOS/Windows,  and more ...

https://www.realvnc.com/de/connect/download/viewer/macos/

VNC on MacOS
*********

.. figure:: ./dokumentation_ipsy/bilder_vnc/Bar.png
    :name: bar.png
    :alt:  bar.png
    :align: center
    :width: 20%
    
    Finde in der Menueleiste die Systemeinstellungen 
    
.. figure:: ./dokumentation_ipsy/bilder_vnc/settings.png
    :name: settings.png
    :alt:  settings.png
    :align: center
    :width: 20%
    
    Finde in den Systemeinstellungen die Freigaben 
    
.. figure:: ./dokumentation_ipsy/bilder_vnc/settings1.png
    :name: settings1.png
    :alt:  settings1.png
    :align: center
    :width: 20%
    
    Finde in den Freigaben die entfernte Anmeldung 
    
.. figure:: ./dokumentation_ipsy/bilder_vnc/settings2.png
    :name: settings2.png
    :alt:  settings2.png
    :align: center
    :width: 20%
    
    Gebe dein Passwort von deinem Benutzer ein und schalte den Zugang auf entferne Geraete sowohl bei dir als auch bei anderen System per ssh frei
    
.. figure:: ./dokumentation_ipsy/bilder_vnc/settings3.png
    :name: settings3.png
    :alt:  settings3.png
    :align: center
    :width: 20%
    
    Jetzt muesste es moeglich sein vnc Viewer & Connect zu nutzen! 

.. figure:: ./dokumentation_ipsy/bilder_vnc/controlled.png
    :name: controlled.png
    :alt:  controlled.png
    :align: center
    :width: 20%

 Test to controll !
 
.. figure:: ./dokumentation_ipsy/bilder_vnc/becontrolled.png
    :name: becontrolled.png
    :alt: becontrolled.png
    :align: center
    :width: 20%

Test to be controlled !






VNC on Linux
****
Text 



VNC on Windows
**********



Putty on Windows/Linux/MacOS
**********
All pages and steps found detailed here: 

https://www.ssh.com/academy/ssh/putty/windows

And short here: 

Putty on Windows
**********

Download Putty. 
https://www.chiark.greenend.org.uk/~sgtatham/putty/latest.html




Putty on Linux
**********




Putty on MacOS
**********
PuTTY is an SSH telnet client which, with a VNC Viewer, connects to the GUI. The steps after downloading PuTTY is as follows:

      1. Specify host name as your medusa login (name@medusa.ovgu.de) and Port 22
      2. On the right hand side, click on the + next to SSH and then click Tunnels.
      3. Type 59 + your session number for Source port (e.g. if your session number is 8 type 5908).
      4. Type localhost:59(session number) as Destination then click Add. (e.g. localhost:5908)
      5. Go back to session and you can save this session so you don’t have to repeat these steps each time you want to connect.
      6. Load and open session and connect to medusa and start the VNC Server (after setting up your password)
      7. Open a VNC Viewer, type localhost:59(session number) and connect.
      8. You will be required to enter your VNC password, afterwards you will have access to the GUI.


Config & Settings 
******
Killen von Prozessen auf dem Medusa Server, notwendig bei mehrfacher Anwendung von dem starten von vnc Servern: 

.. code::

ps aux | grep Benutzer | grep vnc

.. code::

vncserver -kill :9

.. code::

pkill -u Benutzer



----

Important to know: 
links for more understanding: 
