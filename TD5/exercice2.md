## Exercice 2

	joaobrilhante@GlaDOS:~$ netcat -l 1234

	GET /?var=Hello%2C+world+%21 HTTP/1.1
	Host: localhost:1234
	Connection: keep-alive
	Upgrade-Insecure-Requests: 1
	User-Agent: Mozilla/5.0 (X11; Linux x86_64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/70.0.3538.110 Safari/537.36
	Accept: text/html,application/xhtml+xml,application/xml;q=0.9,image/webp,image/apng,*/*;q=0.8
	Accept-Encoding: gzip, deflate, br
	Accept-Language: fr-FR,fr;q=0.9,en-US;q=0.8,en;q=0.7

	HTTP/1.1 200 OK
	Date: Mon, 26 Nov 2018 12:09:20 GMT
	Content-Type: text/plain; charset=utf-8

  Hello, world !

Nous envoyons alors une réponse à la requête du client. Nous commençons par lui indiquer que sa requête a bien été prise en code à l'aide d'un code `200`. Enfin, nous lui envoyons une date et un contenu en précisant qu'il s'agit d'un texte clair.