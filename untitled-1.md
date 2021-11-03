# Rollback

O Rollback é utilizado para desfazer o comando que você realizou, como um UPDATE ou DELETE.

Exemplo:

```sql
BEGIN TRANSACTION -- RODAR JUNTO COM O SCRIPT QUE PRECISA GARANTIR O ROLLBACK
	DROP TABLE Vendas

ROLLBACK TRANSACTION -- PARA DESFAZER O COMANDO FEITO PELO BEGIN
COMMIT TRANSACTION -- PARA ENCERRAR A TRANSAÇÂO SALVANDO OS DADOS
```
