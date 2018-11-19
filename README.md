# teste-git
Teste de Git

# Deletar todas as braches mergeadas do remoto
´´´
git branch -r --merged | egrep -v "(^\*|\/master|\/dev|\/develop|\/hom|\/homologacao)$" | grep origin | sed "s/\s*origin\///" | xargs -n 1 git push origin --delete
´´´
