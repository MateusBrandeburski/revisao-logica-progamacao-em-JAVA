import java.util.Locale;
import java.util.Scanner;

public class Main {

	public static void main(String[] args) {
		
		Locale.setDefault(Locale.US);
		
		Scanner sc = new Scanner(System.in);
		
		int id, horas;
		double valor, receber;
		
		id = sc.nextInt();
		horas = sc.nextInt();
		valor = sc.nextDouble();
		receber = horas * valor;
		
		System.out.printf("NUMBER = %d%n", id);
		System.out.printf("SALARY = U$ %.2f%n ", receber);
		
			sc.close();
