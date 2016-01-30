# Plataforma Quilombo

O sistema é um CMS conhecido, Drupal, para colocar o sistema em funcionamento é necessário algumas dependencias

- Apache2
- PHP
- MySQL

Com tudo isso basta colocar os arquivos na pasta www, httpd ou outro nome que foi utilizado em seu sistema operacional.

Em seguida faça a importação do banco de dados para o MySQL. Você pode fazer isso pela linha de comando:

`mysql -u usuario_administrador -p < base.sql`

Digite a senha do usuário do banco de dados.

Por ultimo entre na pasta sites/default e abra o arquivo settings.php e modifique as seguintes linhas com o nome do usuário e a senha do banco de dados, lembre que o nome do banco de dados continua o mesmo, pois o arquivo de importação é quem cria o banco de dados.
```
      'database' => 'nome banco de dados',
      'username' => 'usuario admin db',
      'password' => 'senha',
```
Nesse momento pode visualizar o site por meio de um navegador.
