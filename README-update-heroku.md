# Einmalig zum Einrichten 

Siehe:
- https://f-a.nz/dev/update-deploy-to-heroku-app/
- https://dashboard.heroku.com/apps/librelinkup-steph/deploy/heroku-git

Kommandos:

	heroku login
	heroku git:clone -a librelinkup-steph 	
	cd librelinkup-steph 	
	git remote add origin https://github.com/he99/nightscout-librelink-up.git

	:: Jetzt müsste git remote zwei remotes zeigen: heroku und origin
	
# Neuen code einchecken und heroku neu starten

	git pull origin main
	git add . 
	git commit -am "pre-heroku"
	git push heroku master

