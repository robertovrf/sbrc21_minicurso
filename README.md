# Minicurso SBRC'21

Welcome to our SBRC shortcourse. For now, we only make available the files we used during our short course presentation. We will make available the practical exercises for the book chapter soon.

This repository currently contains: 

1. A dana code example (located in shortcourse_practicals/dana_example);
2. The InteractiveEmergentSys tool (located in shortcourse_practicals/emergent_web_server);
3. Emergent Web Server (located in emergent_web_server);

First, please download all the content we added to this repository. After that, go to https://projectdana.com, download the latest available version of the language for your system (we currently support: MacOS, Ubuntu, Windows and Raspberry pi). For installation instructions, please visit: http://www.projectdana.com/dana/guide/installation

After installing and testing the recently installed Dana version, to execute the Emegent Web Server using the InteractiveEmergentSys tool follow the steps below:

1. Go to shortcourse_practicals/emergent_web_server directory on your system's terminal;
2. Compile the pal folder:
2.1. Go to /pal directory;
2.2. Type: "dnc . -sp ../repository".
3. Then compile the repository folder:
3.1. Go to /repository directory;
3.2. Type: "dnc .".
4. Go to /pal directory;
5. Execute the InteractiveEmergentSys tool:
5.1 Type: "dana -sp ../repository InteractiveEmergentSys.o ../repository/TCPNetwork.o"

Now you have an instance of the InteractiveEmergentSys running executing an instance of the Emergent Web Server.

To test the web serve, go to a web browser and acess: http://localhost:2012. You should get see the index.html page located in shortcourse_practicals/emergent_web_server/repository/htdocs.

To see the type of commands you can execute using the IntractiveEmergentSys, type "help" into the terminal.

To add a monitoring proxy to collect data from the executing web server, type into the terminal:

add_proxy |../pal/monitoring/proxies/HTTPProxy.o|*(*:http.handler.GET.HTTPGET[0]:*)|

Any questions? Please get in contact!

