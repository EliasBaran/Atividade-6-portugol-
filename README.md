# Atividade-6-portugol-

1. Faça um programa que imprima na tela os números de 1 a 20, um abaixo do outro.”
a. Use a estrutura de repetição “enquanto”;
b. Use a estrutura de repetição “para”;

programa {
	funcao inicio() {
		
	inteiro N = 1
	
	 enquanto (N <= 20) {escreva (N+ "\n") N++} 
	 
	 escreva ("\n fim do exercicio a. \n\n\n")
	 
 	 para (inteiro I = 1; I <= 20; I++) { escreva (I+ "\n")}
 	 
 	 escreva ("\n fim do exerciccio b. ")
	 
}
}





2. Faça um programa que imprima na tela os números de 20 a 1, um abaixo do outro.

programa {
	funcao inicio() {
		
		para (inteiro I = 20; I >=0; I--) {escreva (I+ "\n")}
	}
}





3. Faça uma cópia do exercício anterior e o modifique o para mostrar os números um
ao lado do outro.

programa {
	funcao inicio() {
		
			para (inteiro I = 20; I >=0; I--) {escreva (I+ ", ")}
	}
}





4. Faça um programa que imprima na tela apenas os números ímpares entre 1 e 50.

programa {
	funcao inicio() {
		
		
	    inteiro N = 1
	    
	
	 enquanto (N <= 50) {escreva (N , "\n") N = N + 2} 
	 
	}
}





5. Faça um programa, utilizando “para”, que:
a. Peça para o usuário inserir um número N;
b. Escreva na tela todos os números de 1 até N e pule 3 linhas;
c. Escreva na tela todos os números de N até 1;

programa {
	funcao inicio() {
		
		inteiro N
		
		escreva ("informe um numero: ")
		leia (N)
		
		para (inteiro C = 1; C <= N; C++) {escreva (C , "\n")}
		
		escreva ("\n\n\n")
		
		para(inteiro I = 1; I <= N; N--) {escreva (N , "\n")}
	}
}





6. Faça um programa que receba dois números inteiros e gere os números inteiros que
estão no intervalo compreendido por eles.

programa {
	funcao inicio() {
		
		inteiro A
		inteiro B
		
		escreva ("informe um numero: ")
		leia (A)
		
		escreva ("informe outro numero: ")
		leia (B)
		
		enquanto(A > B) {A = A - 1 escreva (A, "\n")}
		
		enquanto(A < B) {A = A + 1 escreva (A, "\n")}
		
	}
}





7. Faça um programa que peça ao usuário uma nota, entre zero e dez. Mostre uma
mensagem caso o valor seja inválido e continue pedindo até que o usuário informe
um valor válido.

programa {
	funcao inicio() {
		
		inteiro N = 7
		inteiro V
		
		escreva ("digite a senha: ")
	    leia (V)
	    
	    se (N == V) {escreva ("acesso permitido")}
	    
	    senao  {escreva ("senha incorreta")}
}
}





8. Faça um programa que leia uma senha do usuário. Seu programa não deve aceitar
senhas iguais a:
• “12345”
• “admin”
• “senha”
• “xuxa”
Caso esse padrão seja informado, seu programa deve informar
uma mensagem de “senha insegura” e pedir outra senha
novamente.

programa {
	funcao inicio() {
		
		cadeia S
		
		escreva ("digite sua nova senha: ")
		leia (S)
		
		se (S == "12345") {escreva ("senha insegura")}
		
	    senao se (S == "admin") {escreva ("senha insegura")} 
	    
		senao se (S == "senha") {escreva ("senha insegura")}
		
	    senao se (S == "xuxa") {escreva ("senha insegura")}
	    
	    senao {escreva ("senha aprovada")}
		
}
}





9. Similar ao exercício anterior, faça um programa que leia e valide as seguintes
informações:
• Nome: maior que 3 caracteres;
• Idade: entre 0 e 150;
• Salário: maior que zero;

programa {
	funcao inicio() {
		
		cadeia N
		inteiro L , I, S
		
		escreva ("Qual seu nome? ")
		leia (N)
		limpa()
		
		escreva ("Quantas letras tem seu nome? ")
		leia (L)
        limpa()
        
		escreva ("Qual sua idade? ")
		leia (I)
        limpa()
        
		escreva ("Qual seu salario? ")
		leia (S)
		limpa()

		se (L > 3 e I >= 0 e S > 0) {escreva("Informaçoes validas")} 
			
		senao {escreva("Informaçoes invalidas")}
		
	}
}





10. Supondo que a população de um país A seja da
ordem de 80000 habitantes com uma taxa
anual de crescimento de 3% e que a população
de B seja 200000 habitantes com uma taxa de
crescimento de 1.5%.
Faça um programa que calcule e escreva o número de anos necessários para que a
população do país A ultrapasse ou iguale a população do país B, mantidas as taxas
de crescimento.

programa {
	funcao inicio() {
		
		inteiro A = 80000 
		inteiro B = 200000  

		inteiro anos = 0

		enquanto(A < B) {
	    A = A + (A * 0.03)
	    B = B + (B * 0.015)
        anos++}

		escreva("numero de habitante pais A: ", paisA, "\n")
		escreva("numero de habitante pais B: ", paisB, "\n")

		escreva("foram necessários ", anos, " anos para o pais A ter a maior populacão")
		
	}
}





11. Altere o programa anterior permitindo ao usuário informar as populações e as taxas
de crescimento iniciais. Valide a entrada e permita repetir a operação.

programa {
	funcao inicio() {
		
		inteiro P1
		inteiro P2
		inteiro anos = 0
        real t1
        real t2

		escreva ("Informe a popoulaçao do pais 1: ")
		leia (P1)
		escreva ("Informe a populaçao do pais 2: ")
		leia (P2)

		escreva ("Informe a taxa de crescimento do pais 1: ")
		leia (t1)
		escreva ("Informe a taxa de crescimento do pais 2: ")
		leia (t2)

		enquanto (P1 < P2) {P1 = P1 + (P1 * t1) P2 = P2 + (P2 * t2) anos++}
			
		enquanto (P1 > P2) {P1 = P1 + (P1 * t1) P2 = P2 + (P2 * t2) anos++}

		escreva("A populaçao do pais 1 chegou à: ", P1, "\n")
		escreva("A populaçao do pais 2 chegou à: ", P2, "\n")

		se (P1 > P2) {escreva("O pais 1 levou ", anos, " anos para ultrapassar a populaçao do pais 2")}
		
		senao {escreva("O pais 2 levou ", anos, " anos para ultrapassar a populaçao do pais 1")}
		
	}
}





12. Faça um programa que leia 5 números e informe o maior número.

programa {
	funcao inicio() {
		
		inteiro num1
		inteiro num2
		inteiro num3
		inteiro num4
		inteiro num5

		escreva("Qual o valor do primeiro valor: ")
		leia(num1)
		escreva("Qual o valor do segundo valor: ")
		leia(num2)
		escreva("Qual o valor do terceiro valor: ")
		leia(num3)
		escreva("Qual o valor do quarto valor: ")
		leia(num4)
		escreva("Qual o valor do quinto valor: ")
		leia(num5)

		se(num1 > num2 e num1 > num3 e num1 > num4 e num1 > num5){
			escreva("O maior numero é: ", num1)
		}

		se(num1 < num2 e num1 > num3 e num1 > num4 e num1 > num5){
			escreva("O maior numero é: ", num2)
		}

		se(num1 > num2 e num1 < num3 e num1 > num4 e num1 > num5){
			escreva("O maior numero é: ", num3)
		}

		se(num1 > num2 e num1 > num3 e num1 < num4 e num1 > num5){
			escreva("O maior numero é: ", num4)
		}

		se(num1 > num2 e num1 > num3 e num1 > num4 e num1 < num5){
			escreva("O maior numero é: ", num5)
		}
		
	}
}





13. Faça um programa que leia 5 números e informe a soma e a média dos números.

programa {
	funcao inicio() {
		
		inteiro num1
		inteiro num2
		inteiro num3
		inteiro num4
		inteiro num5

		escreva("Informe o Primeiro numero: ")
		leia(num1)
		escreva("Informe o Segundo numero: ")
		leia(num2)
		escreva("Informe o Terceiro numero: ")
		leia(num3)
		escreva("Informe o Quarto numero: ")
		leia(num4)
		escreva("Informe o Quinto numero: ")
		leia(num5)

		inteiro soma = num1 + num2 + num3 + num4 + num5
		escreva("A soma desses numeros é: ", soma, "\n")

		
		real media = soma / 5
		escreva("A media desses numeros é: ", media, "\n")
		
	}
}





14. Desenvolva um gerador de tabuada, capaz de gerar a tabuada de qualquer número
inteiro entre 1 a 10. O usuário deve informar de qual numero ele deseja ver a tabuada.
A saída deve ser conforme o exemplo abaixo:

programa {
	funcao inicio() {
		
		inteiro ex

		escreva("Informe um numero: ")
		leia(ex)
 
		escreva("A tabuada de ", ex, " é: ", "\n")
		
		escreva(ex," x 1 = ", ex * 1, "\n")
		escreva(ex, " x 2 = ", ex * 2, "\n")
		escreva(ex, " x 3 = ", ex * 3, "\n")
		escreva(ex, " x 4 = ", ex * 4, "\n")
		escreva(ex, " x 5 = ", ex * 5, "\n")
		escreva(ex, " x 6 = ", ex * 6, "\n")
		escreva(ex, " x 7 = ", ex * 7, "\n")
		escreva(ex, " x 8 = ", ex * 8, "\n")
		escreva(ex, " x 8 = ", ex * 9, "\n")
		escreva(ex, " x 10 = ", ex * 10, "\n")
		
	}
}
