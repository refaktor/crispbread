# Crispbread

This is a minimal, practical and simple web/app/api server for Rye language.

# Plan for version 0.01

* crispbread will sit behind nginx (or similar), so nginx should serve all static files
* crispbread is for now only an API server, exposing API-s behind one or multiple routes
* some api-s are public, others are protected behind a sessions (webapp), third via API tokens (API)

## Plan of work

* we take example server from Rye and:
	* we test the basic code and make it more solid
	* we start making website for pushbox/share to it
	* we add support for sessions
	* we add support for API tokens
	* we add standard signup / validate / signin / signout / get-api-token
	* it would be good to support static file support for development purposes
	* we add support for reloading of resources / scripts

## Pushbox/share

* enables you to upload a file via webpage or API (document, json, text, ...) 
* you get a link and or QR kode or a token to download it
* the data can be enctypted by the client, in this case client would send the dectyption data to reciever
* we will use it for one of our mobile apps, so users will be able to move certs to them for example (enctypted)
