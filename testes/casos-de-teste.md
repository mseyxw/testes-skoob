▶︎**Casos de Teste**

| ID | Funcionalidade | Entrada / Passos | Resultado Esperado | Resultado Obtido | Status |
| :--- | :--- | :--- | :--- | :--- | :---: |
| CT01 | Busca | 1. No campo de busca, escrever `"Memórias do Subsolo"`<br>2. Clicar na lupa | O sistema deve exibir o livro correto desse autor. | O sistema encontrou corretamente o livro que foi pesquisado. | PASS |
| CT02 | Busca | 1. No campo de busca, escrever caracteres aleatórios<br>2. Clicar na lupa | O sistema deve exibir uma mensagem informando que nenhum livro foi encontrado. | O sistema exibiu uma mensagem informando que não obteve nenhum resultado. | PASS |
| CT03 | Estante Virtual | 1. Entrar na página de um livro<br>2. Clicar em `"Adicionar à estante"`<br>3. Escolher o status `"Quero ler"` | O ícone deve atualizar para `"Quero ler"` e o livro deve aparecer instantaneamente na estante virtual. | O sistema atualizou o status para `"Quero ler"` e adicionou o livro à estante. | PASS |
| CT04 | Estante Virtual | 1. Entrar na página de um livro<br>2. Escolher o status `"Abandonei"` | O ícone deve atualizar para `"Abandonei"` e o livro deve ser movido para a aba `"Abandonei"`. | O sistema atualizou o status para `"Abandonei"` e moveu o livro para a aba correspondente. | PASS |
| CT05 | Avaliação | 1. Entrar na página de um livro<br>2. Clicar em `"Avaliação"`<br>3. Avaliar o livro com 5 estrelas | As estrelas devem ser preenchidas e a avaliação do usuário deve ser salva. | O sistema salvou a avaliação do usuário corretamente. | PASS |
| CT06 | Resenha | 1. Entrar na página de um livro<br>2. Clicar em `"Resenha"`<br>3. Não escrever nenhum caractere | O sistema deve desabilitar o botão de publicar resenha. | O sistema desabilitou o botão de publicar resenha. | PASS |
| CT07 | Resenha | 1. Entrar na página de um livro<br>2. Clicar em `"Resenha"`<br>3. Colar um lorem ipsum com +15.000 caracteres | O sistema deve deixar que a resenha seja publicável. | O sistema deixou a resenha ser publicada. | PASS |
| CT08 | Resenha | 1. Entrar na página de um livro<br>2. Clicar em `"Resenha"`<br>3. Escrever uma resenha<br>4. Marcar `"Contém Spoilers"` | A publicação deve aparecer no feed oculta e com uma mensagem de alerta. | A publicação foi postada oculta e com a mensagem de alerta de spoilers. | PASS |
| CT09 | Sincronização | 1. Entrar no perfil do usuário<br>2. Atualizar a imagem de perfil | A imagem deve ser atualizada tanto no mobile quanto na web, independente de onde foi alterada. | A imagem não foi atualizada na versão web, permanecendo a imagem padrão. | FAIL |
