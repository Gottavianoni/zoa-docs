*************
WS : Txt 2 PN
*************

Presentation
************

This service search some P/N pattern into a text input and returns the pattern found and the corresponding number of occurence

You have the possiblity to call just the ws by using a Curl post request.

Call the standalone WS
**********************

* url : http://localhost:5002
* headers : {'content-type': 'application/json','charset' : 'utf-8'}
* data : { text : "Your Text" }


Example in python ::

	import requests, json
	textarea = "Try to find this PN"
	url = "http://192.168.99.100:5002/txt2pn"
	inpt = json.dumps({'text': textarea})
	head = {'content-type': 'application/json','charset' : 'utf-8'}
	res = requests.post(url, data = inpt,headers = head)
	json_done = res.json()

Sources
*******

* Web Service `txt2pn <https://github.com/Gottavianoni/txt2pn>`_

Dependances
***********

========== ========
 Python    3.6    
========== ========
 Flask     0.10.1  
 Numpy     1.13.3
========== ========

========== ========
 PN List   0.1    
========== ========
