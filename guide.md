> Install zsh.

		apt-get update
		apt-get install git man vim tree curl
		apt-get install zsh zsh-doc
			
> Create a single tree

		mkdir -p project/{app,dist,public,doc}/log
		mkdir -p project/public/{images,css}
		touch project/app/{index.js,index.html}
		touch project/dist/{bundle.js,index.html}
		touch project/public/images/logo.png project/public/css/styles.css
		
> Enter `zsh`

		ls project/**/*
		