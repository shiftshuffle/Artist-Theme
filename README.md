# math

git add .
git commit -m 'latextweak'
git push origin master

git checkout gh-pages
git rebase master
git push origin gh-pages
git checkout master
