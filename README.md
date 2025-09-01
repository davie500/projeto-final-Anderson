README dos seguintes elementos >  Admin/Cliente, Diagrama(explicação da ligação das tabelas), Figma, JS, CSS, Postgres, Node, JSON, React, Front, Back.

v Admin/Cliente v

Nosso projeto possui dois sistemas de login: um para cliente e outro para administrador (adm).
Cada um tem sua própria página de login e redireciona para uma área específica após o login bem-sucedido.

Login do Cliente

Arquivo: login_cliente.html

Campos: Usuário e Senha

Processo:
O formulário envia os dados via fetch para /login-cliente.
Se o login for válido (response.ok), o usuário é redirecionado para home_cliente.html.
Se inválido, aparece um alerta.

Login do Administrador
Arquivo: login_adm.html
Campos: Usuário e Senha

Processo:
O formulário envia os dados via fetch para /login-adm.
Se o login for válido (response.ok), o usuário é redirecionado para /home-adm.html.
Se inválido, aparece um alerta.

Funcionamento geral

Cada tipo de usuário tem sua própria tela de login e área restrita.
O backend precisa validar os dados recebidos e responder corretamente.
Sem banco de dados, os logins não funcionam de verdade, pois não há onde verificar ou armazenar usuários e senhas.

Resumo:
Seu projeto separa clientes e administradores, cada um com login e área própria, mas depende de um backend e banco de dados para funcionar corretamente.

--------------------------------------------------------------------------------------------------------------------------------------------------------

Diagrama(explicação da ligação das tabelas).
