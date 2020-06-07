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