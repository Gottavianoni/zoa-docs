**************
WS - Pdf 2 Txt
**************

Presentation
************

This service take a documents in input (doc, docx, pdf ...) and return the text into your documents in a json result

You have the possiblity to call just the ws by using a Curl post request.

Call the standalone WS
**********************

Curl POST parameters 

* url : http://localhost:5001
* file : { "file" : "path/to/your/file" }

Example with a Python POST Requests ::

	import requests, json
	url = "http://localhost:5001/pdf2txt"
	files = {'file': open(text, 'rb')}
	res = requests.post(url)
	json_done = res.json()

Sources
*******

* Web Service `pdf2txt <https://github.com/Gottavianoni/zoa-ws-pdf2txt>`_

Dependances
***********

========== ========
 Python    3.6   
========== ========
 Flask     0.10.1  
 Requests  2.6.0
========== ========

========== ========
 Tika App  1.18    
========== ========