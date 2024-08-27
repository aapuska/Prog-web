# Gabarito: Exercícios de Formulários HTML Básicos

## Exercício 1: Formulário de Login

```html
<!DOCTYPE html>
<html lang="pt-br">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Formulário de Login</title>
</head>
<body>
    <form action="/login" method="post">
        <label for="username">Nome de usuário:</label>
        <input type="text" id="username" name="username" required>
        
        <label for="password">Senha:</label>
        <input type="password" id="password" name="password" required>
        
        <button type="submit">Entrar</button>
    </form>
</body>
</html>
```

## Exercício 2: Formulário de Cadastro

```html
<!DOCTYPE html>
<html lang="pt-br">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Formulário de Cadastro</title>
</head>
<body>
    <form action="/cadastro" method="post">
        <label for="nome">Nome completo:</label>
        <input type="text" id="nome" name="nome" required>
        
        <label for="email">E-mail:</label>
        <input type="email" id="email" name="email" required>
        
        <label for="senha">Senha:</label>
        <input type="password" id="senha" name="senha" required>
        
        <label for="confirma-senha">Confirme a senha:</label>
        <input type="password" id="confirma-senha" name="confirma-senha" required>
        
        <label for="data-nascimento">Data de nascimento:</label>
        <input type="text" id="data-nascimento" name="data-nascimento" placeholder="DD/MM/AAAA" required>
        
        <fieldset>
            <legend>Gênero:</legend>
            <input type="radio" id="masculino" name="genero" value="masculino">
            <label for="masculino">Masculino</label>
            
            <input type="radio" id="feminino" name="genero" value="feminino">
            <label for="feminino">Feminino</label>
            
            <input type="radio" id="outro" name="genero" value="outro">
            <label for="outro">Outro</label>
        </fieldset>
        
        <button type="submit">Cadastrar</button>
    </form>
</body>
</html>
```

## Exercício 3: Formulário de Pesquisa

```html
<!DOCTYPE html>
<html lang="pt-br">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Pesquisa de Satisfação</title>
</head>
<body>
    <form action="/pesquisa" method="post">
        <label for="nome">Nome:</label>
        <input type="text" id="nome" name="nome" required>
        
        <label for="idade">Idade:</label>
        <input type="number" id="idade" name="idade" required>
        
        <label for="satisfacao">Satisfação geral:</label>
        <select id="satisfacao" name="satisfacao" required>
            <option value="">Selecione uma opção</option>
            <option value="muito-satisfeito">Muito Satisfeito</option>
            <option value="satisfeito">Satisfeito</option>
            <option value="neutro">Neutro</option>
            <option value="insatisfeito">Insatisfeito</option>
            <option value="muito-insatisfeito">Muito Insatisfeito</option>
        </select>
        
        <fieldset>
            <legend>Áreas de melhoria:</legend>
            <input type="checkbox" id="atendimento" name="melhoria" value="atendimento">
            <label for="atendimento">Atendimento</label>
            
            <input type="checkbox" id="produto" name="melhoria" value="produto">
            <label for="produto">Produto</label>
            
            <input type="checkbox" id="preco" name="melhoria" value="preco">
            <label for="preco">Preço</label>
            
            <input type="checkbox" id="entrega" name="melhoria" value="entrega">
            <label for="entrega">Entrega</label>
        </fieldset>
        
        <label for="comentarios">Comentários adicionais:</label>
        <textarea id="comentarios" name="comentarios" rows="4" cols="50"></textarea>
        
        <button type="submit">Enviar Pesquisa</button>
    </form>
</body>
</html>
```

## Exercício 4: Formulário de Pedido

```html
<!DOCTYPE html>
<html lang="pt-br">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Formulário de Pedido</title>
</head>
<body>
    <form action="/pedido" method="post">
        <fieldset>
            <legend>Informações do Cliente</legend>
            <label for="nome">Nome do cliente:</label>
            <input type="text" id="nome" name="nome" required>
            
            <label for="endereco">Endereço de entrega:</label>
            <textarea id="endereco" name="endereco" rows="3" required></textarea>
        </fieldset>
        
        <fieldset>
            <legend>Detalhes do Pedido</legend>
            <label for="produto">Produto:</label>
            <select id="produto" name="produto" required>
                <option value="">Selecione um produto</option>
                <option value="produto1">Produto 1</option>
                <option value="produto2">Produto 2</option>
                <option value="produto3">Produto 3</option>
            </select>
            
            <label for="quantidade">Quantidade:</label>
            <input type="number" id="quantidade" name="quantidade" min="1" required>
        </fieldset>
        
        <fieldset>
            <legend>Método de Pagamento</legend>
            <input type="radio" id="cartao" name="pagamento" value="cartao" required>
            <label for="cartao">Cartão de Crédito</label>
            
            <input type="radio" id="boleto" name="pagamento" value="boleto">
            <label for="boleto">Boleto</label>
            
            <input type="radio" id="transferencia" name="pagamento" value="transferencia">
            <label for="transferencia">Transferência</label>
        </fieldset>
        
        <input type="checkbox" id="termos" name="termos" required>
        <label for="termos">Aceito os termos e condições</label>
        
        <button type="submit">Enviar Pedido</button>
        <button type="reset">Limpar Formulário</button>
    </form>
</body>
</html>
```

## Exercício 5: Formulário de Contato

```html
<!DOCTYPE html>
<html lang="pt-br">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Formulário de Contato</title>
</head>
<body>
    <form action="/contato" method="post">
        <label for="nome">Nome:</label>
        <input type="text" id="nome" name="nome" required>
        
        <label for="email">E-mail:</label>
        <input type="email" id="email" name="email" required>
        
        <label for="assunto">Assunto:</label>
        <select id="assunto" name="assunto" required>
            <option value="">Selecione um assunto</option>
            <option value="duvida">Dúvida</option>
            <option value="sugestao">Sugestão</option>
            <option value="reclamacao">Reclamação</option>
            <option value="outro">Outro</option>
        </select>
        
        <label for="mensagem">Mensagem:</label>
        <textarea i