# Aulas-Orienta--o-a-Objeto-Faculdade
algumas atividades do professor Célio
package Program;

import java.util.Locale;
import java.util.Scanner;

public class Application {
	
	int numeroEscolhido;
	static int i;
	
	public void tabuada() {
		while(i <= 10) {
			System.out.println(numeroEscolhido + " X " + i + " = " + numeroEscolhido * i);
			i++;
		}
	}
	
	public static void main(String[] args) {
		Locale.setDefault(Locale.US);
		Scanner sc = new Scanner (System.in);
		Application calc = new Application();
		
		System.out.println("Escolha um número");
		calc.numeroEscolhido = sc.nextInt();
		i = 0;
		calc.tabuada();

	}

}
