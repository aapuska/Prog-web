# Tutorial: Criando um Formulário de Cadastro com Git, GitHub e VS Code

## Objetivo
Criar um formulário de cadastro HTML básico, utilizando Git para controle de versão, GitHub para hospedagem do repositório, e VS Code como editor de código.

## Passo 1: Configuração Inicial

1. Abra o VS Code
2. Abra um novo terminal no VS Code (Terminal > New Terminal)
3. Navegue até o diretório onde você deseja criar o projeto:
   ```
   cd caminho/para/seus/projetos
   ```
4. Crie uma nova pasta para o projeto:
   ```
   mkdir formulario-cadastro
   cd formulario-cadastro
   ```

## Passo 2: Inicialização do Git

1. Inicialize um novo repositório Git:
   ```
   git init
   ```
2. Crie um arquivo .gitignore:
   ```
   echo "# Arquivos a serem ignorados pelo Git" > .gitignore
   ```
3. Adicione o .gitignore ao staging:
   ```
   git add .gitignore
   ```
4. Faça o primeiro commit:
   ```
   git commit -m "Inicialização do projeto e adição do .gitignore"
   ```

## Passo 3: Criação do Arquivo HTML

1. No VS Code, crie um novo arquivo chamado `index.html`
2. Adicione a estrutura básica HTML5:

```html
<!DOCTYPE html>
<html lang="pt-br">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Formulário de Cadastro</title>
</head>
<body>
    <h1>Formulário de Cadastro</h1>
    <form action="#" method="post">
        <!-- Aqui adicionaremos os campos do formulário -->
    </form>
</body>
</html>
```

3. Salve o arquivo

## Passo 4: Adicionando Campos ao Formulário

Vamos adicionar os campos solicitados no exercício dentro da tag `<form>`:

```html
<label for="nome">Nome completo:</label>
<input type="text" id="nome" name="nome" required>

<label for="email">E-mail:</label>
<input type="email" id="email" name="email" required>

<label for="senha">Senha:</label>
<input type="password" id="senha" name="senha" required>

<label for="confirma-senha">Confirmação de senha:</label>
<input type="password" id="confirma-senha" name="confirma-senha" required>

<label for="data-nascimento">Data de nascimento:</label>
<input type="date" id="data-nascimento" name="data-nascimento" required>

<fieldset>
    <legend>Gênero:</legend>
    <input type="radio" id="masculino" name="genero" value="masculino">
    <label for="masculino">Masculino</label>
    <input type="radio" id="feminino" name="genero" value="feminino">
    <label for="feminino">Feminino</label>
    <input type="radio" id="outro" name="genero" value="outro">
    <label for="outro">Outro</label>
</fieldset>

<button type="submit">Enviar</button>
```

## Passo 5: Commit das Alterações

1. Verifique o status das alterações:
   ```
   git status
   ```
2. Adicione o arquivo index.html ao staging:
   ```
   git add index.html
   ```
3. Faça o commit das alterações:
   ```
   git commit -m "Adiciona estrutura básica do formulário de cadastro"
   ```

## Passo 6: Criação do Repositório no GitHub

1. Acesse https://github.com e faça login
2. Clique em "New" para criar um novo repositório
3. Nomeie o repositório como "formulario-cadastro"
4. Deixe-o público e não inicialize com README
5. Clique em "Create repository"

## Passo 7: Conexão do Repositório Local com o GitHub

1. No terminal do VS Code, adicione o repositório remoto:
   ```
   git remote add origin https://github.com/seu-usuario/formulario-cadastro.git
   ```
2. Faça o push do seu código para o GitHub:
   ```
   git push -u origin master
   ```

## Passo 8: Visualização e Teste

1. No VS Code, instale a extensão "Live Server" se ainda não tiver
2. Clique com o botão direito no arquivo index.html no explorador de arquivos do VS Code
3. Selecione "Open with Live Server"
4. Seu navegador padrão abrirá mostrando o formulário

## Passo 9: Refinamentos e Melhorias

1. Teste o formulário, preenchendo os campos e tentando enviar
2. Faça ajustes no HTML conforme necessário
3. Após cada conjunto de alterações significativas, repita os passos de commit:
   ```
   git add index.html
   git commit -m "Descrição das alterações feitas"
   git push
   ```

## Conclusão

Parabéns! Você criou um formulário de cadastro básico usando HTML, o versionou com Git, e o hospedou no GitHub, tudo isso usando o VS Code como sua ferramenta principal de desenvolvimento. Este fluxo de trabalho é uma excelente base para projetos de desenvolvimento web mais complexos.

Próximos passos sugeridos:
1. Adicione estilos CSS para melhorar a aparência do formulário
2. Implemente validação de formulário usando JavaScript
3. Explore como processar os dados do formulário no lado do servidor

Lembre-se de continuar praticando e experimentando com diferentes elementos de formulário e estruturas HTML!
