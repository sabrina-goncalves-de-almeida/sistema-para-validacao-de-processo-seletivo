# dio-trilha-java-basico-controle-de-fluxo

## Desafio
Criar um projeto cahamado `DesafioControleFluxo`, com as classes `Contador` e `ParametrosInvalidosException`.

A classe `Contador` receberá dois parametros inteiros `parametroUm` e `parametroDois`, e os subtrairá, para obter o valor de iterações para um laço for.

Temos nessa classe uma regra de negócio onde, quando o `parametroDois` for MENOR que o `parametroUm` ocorrerá uma excessão do tipo `ParametrosInvalidosException`, pois teriemos um numero negativo de iterações.

## Exemplos de Entradas e Saídas
| Entradas | Saídas|
|:---------:|--------|
|12 e 15 | Imprimindo o número 1 <br/> Imprimindo o número 2 <br/> Imprimindo o número 3|
|30 e 10 | ParametrosInvalidosException: O segundo parâmetro deve ser maior que o primeiro|

## Código original do desafio
O desafio conta com um código pronto que deve ser completado.

```java
public class Contador {
	public static void main(String[] args) {
		Scanner terminal = new Scanner(System.in);
		System.out.println("Digite o primeiro parâmetro");
		int parametroUm = terminal.??;
		System.out.println("Digite o segundo parâmetro");
		int parametroDois = terminal.??;
		
		try {
			//chamando o método contendo a lógica de contagem
			contar(parametroUm, parametroDois);
		
		}catch (? exception) {
			//imprimir a mensagem: O segundo parâmetro deve ser maior que o primeiro
		}
		
	}
	static void contar(int parametroUm, int parametroDois ) throws ParametrosInvalidosException {
		//validar se parametroUm é MAIOR que parametroDois e lançar a exceção
		
		int contagem = parametroDois - parametroUm;
		//realizar o for para imprimir os números com base na variável contagem
	}
}

```
