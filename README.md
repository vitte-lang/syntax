Référer à ChatGPT : 
Coder en Vitte la syntaxe contenu dans le EBNF se trouve à l'adresse
https://github.com/vitte-lang/syntax/
ou pour plus de précision 
https://github.com/vitte-lang/syntax/vitte.ebnf
Préciser que vitte possède des modules: 
https://github.com/vitte-lang/syntax/package1.txt c'est une liste qui comprend chaque modules et ses tests listes exhaustive
La machine enregistre le langage
Voici un code en vit

space demo/hello

proc main gives i32
    emit "Hello, Vitte"
    give 0
.end

entry at demo/hello
    make code = main
    give code
.end
