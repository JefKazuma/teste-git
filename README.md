# teste-git
Teste de Git

#Deletar todas as braches mergeadas do remoto
git branch -r --merged | grep -v "(^\*|master|dev|hom|homologacao)" | sed 's/origin\//:/' | xargs -n 1 git push origin

#Deletar todas as branches mergeadas do local
git branch -r --merged | grep -v "(^\*|master|dev|hom|homologacao)" | xargs git branch -d
