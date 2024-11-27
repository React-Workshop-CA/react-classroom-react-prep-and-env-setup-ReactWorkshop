

## Step 1. Install Visual Studio Code

 [https://code.visualstudio.com/Download](https://code.visualstudio.com/Download)

## Step 2. Update Chrome Browser to the latest version

	 (Install Chrome Browser if not installed already)

 [https://www.google.com/chrome/update](https://www.google.com/chrome/update)

## Step 3. Install Node JS \[use LTS Version\]

	 Version: v22.11.0(LTS)

 [https://nodejs.org/en/download/prebuilt-installer](https://nodejs.org/en/download/prebuilt-installer)

## Step 4. Dev Tools

	Add "React Developer Tools" Extension for Chrome
	Open below link in Chrome Browser

[https://chromewebstore.google.com/detail/react-developer-tools/fmkadmapgofadopljbjfkapdkoienihi?hl=en](https://chromewebstore.google.com/detail/react-developer-tools/fmkadmapgofadopljbjfkapdkoienihi?hl=en)

## Step 5. Setup Visual Studio Code

 Open Visual Studio Code that we installed from Step 1

A. From the menu do

	 File > Enable "Auto Save"

B. From the menu do View ❯ Command Palette

	 Type "shell command” and find below to install

	 Shell Command: Install 'code' command in PATH command_

## Step 6. Verify Node/NPM

**A. Open a Command Prompt**


**Mac**: Terminal 
**Windows**: Powershell (as Administrator)
https://www.javatpoint.com/powershell-run-as-administrator

 **B. Type in below and enter and Check** that it prints \`v22.11.0\`

	 node -v

 **C. Type in below and enter and Check** that it prints should print \`10.9.0\`

	 npm -v

 **D. Type in below and enter**

	 npm install -g create-react-app@latest typescript@latest json-server@latest http-server@latest trash-cli@latest tree-cli@latest

 **E. Type in below and enter and Check** that it prints should print \`5.7.2\`

	 tsc --version

 **F. Copy paste all of below and run it** (if not working run it one by one)

	 code --install-extension blanu.vscode-styled-jsx
	 code --install-extension yoavbls.pretty-ts-errors
	 code --install-extension MariusAlchimavicius.json-to-ts
	 code --install-extension esbenp.prettier-vscode
	 code --install-extension formulahendry.auto-close-tag
	 code --install-extension vincaslt.highlight-matching-tag
	 code --install-extension christian-kohler.path-intellisense
		 
 **G. Create Folders**

**Mac: Go to ~ (cd ~) or wherever you want to do the project and issue**

	 mkdir react-class react-class/type-learn react-class/node-learn react-class/react-server react-class/react-learn

  **Windows: Go to C:/ or wherever you want to do the project and issue**

	  mkdir react-class && chdir react-class && mkdir type-learn && mkdir node-learn && mkdir react-server && mkdir react-learn

  **H. Type in below and enter and Check** that it prints the correct folder structure

	  tree --base react-class

  Output:

	   <your_root_folder>/react-class

		  	        ├── node-learn

		  	        ├── react-learn

		  	        ├── react-server
  
		  	        └── type-learn

## Step 7. Setup Data

 **A. Create two new files as below inside** **`react-server`** **Folder**

	db.json
	db-original.json

 **B. Copy the content below on to** **`both`** **files and save and close these files.**
 
	{
	  "albums": [
	    {
	      "name": "Mr. IQ",
	      "id": 1,
	      "artist": "illayaraja",
	      "upVotes": 10,
	      "downVotes": 4
	    },
	    {
	      "name": "Magneta",
	      "id": 2,
	      "artist": "AR Rahman",
	      "upVotes": 30,
	      "downVotes": 0
	    },
	    {
	      "name": "Bombasto",
	      "id": 3,
	      "artist": "DJ Snake",
	      "upVotes": 3,
	      "downVotes": 10
	    }
	  ],
	  "users": [
	    {
	      "userName": "admin",
	      "password": "admin"
	    }
	  ]
	}

 **C. Open Terminal and go to** &lt;your\_root\_folder&gt;/react-class/react-server

 Issue below command

	 json-server db.json

 **D. Open a browser and go to** http://localhost:3000 and see if it shows

	 /albums - 3 items

	 /users - 1 item
