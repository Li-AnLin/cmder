## Cmder 設定教學

1. 把此路徑設至於環境變數 `PATH` 中。
2. 安裝 `.\fonts\AnonymousPro` 中的 `Anonymice Powerline.ttf`。
3. 若有使用 `windows terminal`。請於它的 `setting.json` 中，新增以下至 `list`
    
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
## Powershell 設定教學

1. 打開 `powershell`，輸入

    ```powershell
    Install-Module posh-git -Scope CurrentUser
    Install-Module oh-my-posh -Scope CurrentUser
    ```

2. 找到 `$profile` 位置 (例如: `D:\documents\WindowsPowerShell`)，並新建 `Microsoft.PowerShell_profile.ps1` 檔案，裡面內容為

    ```powershell
    Import-Module posh-git
    Import-Module oh-my-posh
    Set-Theme Agnoster
    ```

3. 若有使用 `windows terminal`。請於它的 `setting.json` 中，新增以下至 `list`

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