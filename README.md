justaCausa = input("Foi demitido por justa causa? ").lower()
if (justaCausa == "não"):
    trabalhadorFormal = input("Você trabalha formalmente? ").lower()
    domestico = input("Trabalhador domestico? ").lower()
    pescador = input("Trabalha com pesca? ").lower()
    escravo = input("Trabalho em codições semelhantes a escravo? ").lower()
    # desempregado = input("Está desempregado? Ou não possui renda suficiente para sustentar a familia? ")
    # beneficio = input("Recebe beneficio previdenciário? ")
    # numeroSolicitacao = input("Quantas vezes ja solicitou o seguro? ")
    tempo = int(input("Quantos meses foram trabalhados? "))
    if ( domestico == "sim"):

            beneficio = input("Recebe beneficio previdenciário? ou qualquer tipo de beneficio sem ser auxilio acidente ou pensão por morte").lower()
            desempregado = input("Está desempregado? Ou não possui renda suficiente para sustentar a familia? ").lower()
            tempoDesempregado = int(input("A quantos meses está desempregado? "))
            if (tempo >= 15 & tempoDesempregado <= 15 and beneficio == "não"):
                desempregado = input("Está desempregado? Ou não possui renda suficiente para sustentar a familia? ").lower()
                if (desempregado == "sim"):
                    print("Voce tem direito a um salario minimo o equivalente a R$1620,00 com limite até 3 parcelas")
                
            
            
        
    elif(pescador == "sim"):
            pescaIninterrupta = input("exerce pesca ininterrupta? ").lower()
            inscricaoInss = input("possui inscrição no INSS como segurado especial? ").lower()
            comprovacao = input("Possui comprovação de venda do pescado a adquirente pessoa jurídica ou cooperativa, no periodo correspondente aos últimos 12 meses que o antecederam ao inicio do defeso? ").lower()
            if(pescaIninterrupta == "sim" and inscricaoInss == "sim" and comprovacao == "sim"):
                beneficio = input("Recebe beneficio previdenciário, ou qualquer tipo de beneficio sem ser auxilio acidente ou pensão por morte? ").lower()
                pescadorRaiz = input("Trabalha unicamente com a pesca? ").lower()
                cadastroUnico = input("Possui inscrição no cadastro único? ").lower()
                if( beneficio == "não" and pescadorRaiz == "sim" and cadastroUnico == "sim"):
                     print("Você tem direito a receber um salário minimo por mês equivalente a R$1620 pelo periodo de interrupção da atividade.")
                     
    elif(escravo == "sim"):
        resgate = input("Foi resgatado em situção de trabalho forçado").lower()
        beneficio = input("Recebe beneficio previdenciário, ou qualquer tipo de beneficio sem ser auxilio acidente ou pensão por morte? ").lower()
        desempregado = input("Está desempregado? Ou não possui renda suficiente para sustentar a familia? ").lower()
        if(resgate =="sim" and beneficio == "não" and desempregado == "sim"):
             print("Você possui direito a 6 parcelas de um salário de um salario minimo o equivalente a R$1620")


    elif(trabalhadorFormal == "sim"):
        desempregado = input("Está desempregado? Ou não possui renda suficiente para sustentar a familia? ").lower()
        beneficio = input("Recebe beneficio previdenciário, ou qualquer tipo de beneficio sem ser auxilio acidente ou pensão por morte? ").lower()

        if(desempregado == "sim" and beneficio == "sim"):
            numSolitacao = int (input("Você já pediu seguro desemprego? Quantas vezes? "))

            if(numSolitacao == 0):
                mesesTrabalho = int(input("Quantos meses você trabalhou nessa empresa? "))
                mesesDesempregado = int(input("Quantos meses você está desempregado? "))

                if(mesesTrabalho >= 12 and mesesTrabalho <= 23 and mesesDesempregado <= 36):

                
                elif(mesesTrabalho >= 24 and mesesDesempregado <= 36):

            elif(numSolitacao == 1):
                mesesTrabalho = int(input("Quantos meses você trabalhou nessa empresa? "))
                mesesDesempregado = int(input("Quantos meses você está desempregado? "))

                if(mesesTrabalho >= 9 and mesesTrabalho <= 11 and mesesDesempregado <= 36):
                                    
                
                elif(mesesTrabalho >= 12 and mesesTrabalho <= 23 and mesesDesempregado <= 36):

                elif(mesesTrabalho >= 24 and mesesDesempregado <= 36):

            elif(numSolitacao >= 2):
                mesesTrabalho = int(input("Quantos meses você trabalhou nessa empresa? "))
                mesesDesempregado = int(input("Quantos meses você está desempregado? "))

                if(mesesTrabalho >= 6 and mesesTrabalho <= 11 and mesesDesempregado <= 36):
                                    
                elif(mesesTrabalho >= 12 and mesesTrabalho <= 23 and mesesDesempregado <= 36):
                
                elif(mesesTrabalho >= 24 and mesesDesempregado <= 36):
