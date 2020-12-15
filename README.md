## Cmder Setting Tutorial

1. Set this path to the environment variable `PATH`.
2. Install `Anonymice Powerline.ttf` from `.\fonts\AnonymousPro`.
3. If you use `windows terminal`, please add the following to `list` in its `setting.json`.
    
    ```json
    {
    	"guid": "{5b4ef9a8-4506-4ac9-930a-5eb1fd0ebf20}",
    	"name": "cmder",
    	"commandline": "cmd.exe /k D:/cmder/vendor/init.bat",
    	"icon" : "D:/cmder/icons/cmder.ico",
    	"hidden": false,
    	"startingDirectory" : "%USERPROFILE%",
    	"fontFace" : "Anonymous Pro for Powerline",
    	"fontSize": 11,
    	"background": "#272822",
    	"useAcrylic" : true,
    	"acrylicOpacity" : 0.9
    }
    ```
## Powershell Setting Tutorial

1. Open `powershell` typing

    ```powershell
    Install-Module posh-git -Scope CurrentUser
    Install-Module oh-my-posh -Scope CurrentUser
    ```

2. Find your `$profile` path (ex: `D:\documents\WindowsPowerShell`), and create a file named `Microsoft.PowerShell_profile.ps1`. The content is

    ```powershell
    Import-Module posh-git
    Import-Module oh-my-posh
    Set-Theme Agnoster
    ```

3. If you use `windows terminal`, please add the following to `list` in its `setting.json`.

    ```json
    {
        "guid": "{61c54bbd-c2c6-5271-96e7-009a87ff44bf}",
        "name": "Windows PowerShell",
        "commandline": "powershell.exe",
        "closeOnExit": true,
        "colorScheme": "Campbell",
        "cursorShape": "filledBox",
        "fontFace" : "Anonymous Pro for Powerline",
        "hidden": false
    }
    ```

## vscode Setting Tutorial

1. add the following into `settings.json`

    ```json
    {
        "terminal.integrated.fontFamily": "Anonymous Pro for Powerline",

        // for cmder
        "terminal.integrated.shell.windows": "cmd.exe",
        "terminal.integrated.env.windows": {
            "CMDER_ROOT": "D:\\cmder"
        },
        "terminal.integrated.shellArgs.windows": [
            "/k",
            "D:\\cmder\\vendor\\init.bat"
        ]
    }
    ```