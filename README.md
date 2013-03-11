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
