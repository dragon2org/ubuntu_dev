方法一
安装fcitx输入法，在terminal中，root权限运行#apt install fcitx   
已安装的直接执行
sudo vim /etc/defautl/im-config

更改(#号后面是原文内容) 

IM_CONFIG_DEFAULT_MODE=fcitx #auto

IM_CONFIG_DEFAULT_MODE=fcitx #cjkv




 sudo vim /opt/PhpStorm-162.2380.11/bin/phpstorm.sh
 
 在最后一几行 exec前面加上
 
 export GTK_IM_MODULE=fcitx
 export QT_IM_MODULE=fcitx
 export XMODIFIERS="@im=fcitx"
 
 重启phpstrom
 
 方法二.
 
 # ------需要加入的代码begin-----------
 XMODIFIERS="@im=fcitx"
 export XMODIFIERS
 # ------需要加入的代码end----  一定要在 # Run the IDE. 的前面的如何地方  -------
 # ---------------------------------------------------------------------
 # Run the IDE.
 # ---------------------------------------------------------------------
 # 省略原来的代码

 