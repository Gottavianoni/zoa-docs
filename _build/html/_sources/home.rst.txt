**************
Service - Home
**************

Presentation
************

This service is a simple Flask web interface which allows to call some web services by the standard use of the site :

=> By using the Web buttons on the url

Each fonctionnaly you will use, call a WS to serve you the corresponding result

ie : To proceed a call to pdf2txt service :

* You upload the file
* The app call the standalone pdf2txt web service
* The ws return a json result to the app
* The app display you the request results 

Sources
*******

* Service `Home <https://github.com/Gottavianoni/zoa-ws-home>`_

Dependances
***********
========== ========
 Python    3.6    
========== ========
 Flask     0.10.1  
 Requests  2.6.0
========== ========

