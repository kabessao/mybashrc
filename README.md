# mybashrc
meu bashrc

h2. Descrições 

h3. procurar

wrap no grep para pesquisar arquivos que contem o conteudo descrito.

    procurar "brerp.residuos"
    find | grep pom.xml | procurar "tycho"
    procurar -i VIEW | while read line ; do ... done ; 

h3. dbgo

cd para a workspace

h3. mvn_core

mvn -U veryfy para o core brerp

h3. mvn_cliente 

mvn verify no cliente

h3. code monitor 

procura na home por arquivos migra*.sql, abrindo no vc code quando achar um

h3. db_count

mostra a quantidade de bancos e memoria usada por prefixo. Ex.: hs_

h3. exec_db

wrap para executar comandos no banco de dados 

    echo migracao.sql | exec_db
    exec_db << EOF
    select * from ad_org
    EOF
    exec_db "select * from ad_org"

h3. script_migracao

mostra quantos migra*.sql tem na pasta home, se tiver
