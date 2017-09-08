# Corrigir erro 12514/12505 no Oracle Ubuntu

1. Entre no SQLPlus
```
alter system set LOCAL_LISTENER='(ADDRESS=(PROTOCOL=TCP)(HOST=localhost)(PORT=1521))' scope=both;

alter system register;

show parameter local_listener

exit
```
2. Execute o comando abaixo no console
```lsnrctl services orcl```
