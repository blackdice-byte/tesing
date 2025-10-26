# tesing
ssh keys test
i wrote this line to test that i can push using another github account
 # step one
 navigate to any directory of your choice eg. cd documments/unknown
# step two
ssh-keygen -t rsa -b 4096 -C "eghoiazibapu@gmail.com" -f ~/.ssh/eghoi-key
# step three
ls ~/.ssh/
# step four
eval "$(ssh-agent -s)"
# step five
ssh-add ~/.ssh/eghoi-key
# step six
ssh-add -l
# step seven
cat ~/.ssh/eghoi-key.pub
# step eight
ssh -T -i ~/.ssh/eghoi-key git@github.com
# step nine
nano ~/.ssh/config
# step ten
ls ~/.ssh/
# step eleven
chmod 600 ~/.ssh/config
# step twelve
git clone git@eghoi:blackdice-byte/tesing.git
# step thirteen
cd tesing
# step fourteen
ls
# step fifteen
git config user.name "blackdice-byte"
# step sixteen
git config user.email "eghoiazibapu@gmail.com"
# step seventeen
git remote -v
# step eighteen
touch main.ts
# step nineteen
git add .
# step twenty
git commit -m "feat: added a new file..."
# step twenty one
git push
