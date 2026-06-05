Tips and tricks
- From powershell ssh to synology
	ehman@ds218play:/usr$ sudo /usr/syno/bin/synopkg restart homeassistant
	Password:
	restart package [homeassistant] successfully

- Git from powershell
	Add and commit
		git status to list files that are modified
		git add to add files to be committed
		git commit -m "Added foo to the bar"
		git push
    Merge 
		
	
	Squash
		cd "\\ds218play\homeassistant_config" && git branch -d feature/correct_pricing && git push origin --delete feature/correct_pricing

Todo list
- feature/correct_pricing
	get correct import (you buy) and correct export (you sell) price

