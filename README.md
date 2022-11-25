# Cadastro de Usuário
<html lang="pt-br">
<head>
<title>FORMs</title>

</head> 

<body>
    <form method="post" id="fContato" action="mailto:jefferson.moreira7@etec.sp.gov.br" oninput="calc_total();">

<fieldset id="usuario"><legend>Identificação do Usuário</legend>
    <p>Nome: <input type="text" name="tNome" id="cNome" size="20" maxlength="30" placeholder="Nome Completo"/></p>
    <p>Senha: <input type="password" name="tSenha" id="cSenha" size="15" maxlength="15" placeholder="Digite sua senha"/> </p>
    <p>E-mail: <input type="email" name="tEmail" id="cEmail" size="20" maxlength="40"/> </p>
        <fieldset id=sexo><legend>Sexo</legend>
            <input type="radio" name="tSexo" id="cMasc" checked/><label for="cMasc">Masculino</label>
            <input type="radio" name="tSexo" id="cFem"/><label for="cFem">Feminino</label> 
        </fieldset>
    <p>Data de Nascimento: <input type="date" name="tNasc" id="cNasc"/> </p>
</fieldset>

<fieldset id="endereco"><legend>Endereço do Usuário</legend>
    <p><label for="cRua"> Endereço</label> <input type="text" name="tRua" id="cRua" size="13" maxlength="80" placeholder="Rua, Av, Trav, ..."/></p>
    <p><label for="cNum"> Número: </label><input type="number" name="tNum" id="cNum" min="0" max="999"/></p>

    <p><label for="cEstado">Estado:</label>
        <select name="tEstado" id="cEstado">
            <optgroup label="Região Sudeste">
            <option value="RJ">Rio de Janeiro</option>
            <option value="SP">São Paulo</option>
            <option value="MG" selected>Minas Gerais</option>
        </optgroup>
        
        <optgroup label="Região Sul">
            <option value="PR">Paraná</option>
            <option value="SC">Santa Catarina</option>
            <option value="RS">Rio Grande do Sul</option>
        </optgroup>
        </select></p>

    <p><label for="cCidade">Cidade:</label>
        <p>Cidade: <input type="text" name="tCidade" id="cCidade" size="15" maxlength="15" placeholder="Digite sua cidade"/> </p>

            <datalist id="cidades">
                <option value="Rio de Janeiro"> </option>
                <option value="Niterói"></option>
                <option value="Nova Iguacú"></option>
                <option value="Belford Roxo"></option>
                <option value="Angra"></option>
            </datalist>
    </p>
</fieldset>

<fieldset id="mensagem"><legend>Mensagem do Usuário</legend>
    <p><label for="cUrg">Grau de Urgência: </label>
        Mín<input type="range" name="tUrg" id="cUrg" min="0" max="10" step="2"/>Máx
    </p>
    <p> <label for="cMsg">Mensagem</label>
        <textarea name="tMsg" id="cMsg" cols="45" rows="5" maxlength="150" placeholder="Digite aqui"></textarea> 
    </p>
    
</fieldset>


<input type="submit" value=""/>

</form>

</body>


</html>
