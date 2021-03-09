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
