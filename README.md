test
====
0705:
add script tarball. with encrypt : scripts_0705.tar.bz2.pwd.bey.old.one.for.all

encrypt:
tar jcv Fterm | openssl des3 -salt > Fterm.tar.bz2
decrypt:
cat ../Fterm.tar.bz2 | openssl des3 -d -salt | tar jxv


====
write repo:
git push https://github.com/jwu26/test.git master


====
doc





====
OpenBox Setting
1.tint2
对应文件是~/.config/tint2/tint2rc

2.conky
将rings-v1.2.1.lua放到~/conky/目录下（没有就新建）
将.conkyrc放到~目录

3.openbox主题
放到/usr/share/themes/目录下（如果该目录下有同名主题，可以覆盖，如果怕出问题，先备份）

4.字体
放到~/.fonts/目录下，然后fc-cache更新一下即可。

5.Wallpaper
feh  --bg-scale '/home/jkwu/Pictures/1348666078970.jpg'
cat /etc/xdg/openbox/autostart
eval `cat $HOME/.fehbg` &

6.Config Openbox
1. ~/.config/openbox/menu.xml , config menu on right click.
2. rc.xml, keybind etc.

7.Obconf
select theme as "Numix"

8.Guake : drop down terminal

9.wBar: dock

10. screenlets

11. scrot: screensnapshot

12. zsh: agonster
#git checkout d6a36b1 agnoster.zsh-theme
