O site deseja que eu escreva uma consulta SQL para identificar as Páginas do Facebook que não possuem nenhum "like". Para isso, realizei uma junção entre as tabelas `pages` e `page_likes` usando a cláusula `LEFT JOIN`, garantindo que todas as páginas sejam retornadas, mesmo aquelas sem registros na tabela `page_likes`.

Após a junção, agrupei os resultados pelo `page_id` da tabela `pages` e, em seguida, filtrei para mostrar apenas as páginas onde o número de likes é igual a zero, usando a cláusula `HAVING COUNT(page_likes.page_id) = 0`. Por fim, a consulta será ordenada de forma crescente pelo `page_id`, garantindo que os resultados apareçam na ordem correta.

<H1> Exemplos de saída e as tabelas</H1>

![image](https://github.com/user-attachments/assets/19adb7ec-8973-49eb-b19d-5c40a712c574)
