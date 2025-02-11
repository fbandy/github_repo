# Lépések, ha új remote repóra küldesz fel meglévő kódot

...
git clone https://github.com/fbandy/uj_projekt.git
# Helyezd át a fájljaidat a klónozott könyvtáradba.
git add -A
git commit -m "Másolja a meglévő fájlokat"
git push
...

# vagy

...
git remote add origin git@github.com:fbandy/uj_projekt.git
git branch -M main
git branch --set-upstream-to=origin/main main
git pull --rebase
git push
...