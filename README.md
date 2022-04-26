# GolangVsCodeSetup

# click the extension symbol in the left hand side


![image](https://user-images.githubusercontent.com/80065996/165335078-97c5b38e-b05f-4eb0-8104-37e317beac1e.png)


# search for 'golang' you will get 'gopls' extension which is created by 'team at google', select that and install. with this 'gopls' server we are going to 
# use for our development 


# Press Ctrl + shift + p.  We have a pop up which gets opened. in that type 'go install' you will get one option in dropdown named 'go:Install/Update tools'
# and select all checkbox that selects all (everything) and install it.

# Once everything is installed, you will get message saying 'ready to go'

# next step, click 'ctl + shift + p' and select the 'settings.json' file and paste the below settings. There will be some setting exists by default. 
# along with that paste the below settings as well. 

     "go.useLanguageServer": true,
    "go.languageServerExperimentalFeatures":{
        "diagnostics": true,
        "documentLink": true,
        "format": true
    },
    "[go]": {
        "editor.CodeActionOnSave": {
            "editor.formatOnSave": false,
            "source.organizeImports": true,
        }
    },
    "gopls":{
        "completeUnimported": true,
        "deepCompletition": true,
    },
   
# whole 'settings.json' file

{
    "go.useLanguageServer": true,
    "go.languageServerExperimentalFeatures":{
        "diagnostics": true,
        "documentLink": true,
        "format": true
    },
    
    "[go]": {
        "editor.CodeActionOnSave": {
            "editor.formatOnSave": false,
            "source.organizeImports": true,
        }
    },
    "gopls":{
        "completeUnimported": true,
        "deepCompletition": true,
    },
    "explorer.confirmDelete": false,
    "git.autofetch": true,
    "go.toolsManagement.autoUpdate": true,
    "go.autocompleteUnimportedPackages": true,
    "gopls": {
    
        "completeUnimported": true,
        "usePlaceholders": true,
        "completionDocumentation": true,
        "hoverKind": "SynopsisDocumentation"
    },
    "go.toolsEnvVars": {
        "GO111MODULE": "on",
    },
    "window.zoomLevel": 1,
}

# That's it 'restart the visual studio code'. We are all set.

