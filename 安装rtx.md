    sudo add-apt-repository ppa:wine/wine-builds
    sudo apt-get update
    sudo apt-get install wine-devel
    下载最新 winetricks
    （https://raw.githubusercontent.com/Winetricks/winetricks/master/src/winetricks）

安装依赖
为防止 32 位、64 位可能出现不兼容，执行命令的时候配置 WINEARCH 为 win32。
    WINEARCH=win32 WINEPREFIX=~/.wine winetricks msxml3 gdiplus riched20 riched30 ie6 vcrun6 vcrun2005sp1 allfonts

安装 rtx2015
    WINEARCH=win32 WINEPREFIX=~/.wine wine Downloads/rtxclient2015formal.exe