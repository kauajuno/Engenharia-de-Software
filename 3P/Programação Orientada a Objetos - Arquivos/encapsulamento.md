# Encapsulamento
O encapsulamento é um conceito em OOP que consiste em ocultar detalhes do funcionamento interno de um objeto, de forma que o usuário tenha que lidar apenas com aspectos que de fato lhe interessem ao interagir com este.

## Modificadores de acesso
O controle de acesso é realizado pelos modificadores de acesso. Em Java, tem-se 4 modificadores:
- public
- private
- protected
- default

### public
O public indica que um atributo ou método pode ser acessado por objetos de outra classe.

### private
O private indica que apenas métodos daquela classe e o próprio objeto instanciado dessa classe pode acessar o atributo/método em questão.

### protected
O protected permite o acesso às classes filhas.

### default
Indica que o atributo ou método pode ser acessado por objetos do mesmo pacote.

---

## Boas práticas de programação
O encapsulamento oferece boas práticas de programação em OOP, que consiste em esconder os dados e as implementações, bem como publicar as operações criando uma interface de classe amigável ao usuário que precisar acessar.

![Modelo de Interface de uma classe](interface_da_classe.png)

>class Cliente{
>	private String nome;
>	private String endereco;
>	private String cpf;
>	private Date dataNasc;
>	private int idade;
>	
>	Cliente(String nome, String cpf){
>		this.nome = nome;
>		this.cpf = cpf;
>	}
>	
>	public void attIdade(int ano){
>		int idade;
>		//calcula a idade
>		this.idade = idade;
>	}
>}

Nem todo método precisa ser público:

>class Cliente{
>	private String nome;
>	private String endereco;
>	private String cpf;
>	private Date dataNasc;
>	private int idade;
>	
>	Cliente(String nome, String cpf){
>		this.nome = nome;
>		this.cpf = cpf;
>	}
>	
>	public void attIdade(int ano){
>		int idade;
>		//calcula a idade
>		this.idade = idade;
>	}
>	
>	public void mudaCPF(String cpf){
>		if(verificaCPF(cpf)){
>			this.cpf = cpf;
>		}
>	}
>	
>	private void verificaCPF(String cpf){
>		//bloco de código, retorna true se válido, do contrário false
>	}
>}

## Como acessar atributos com modificador private
Para acessar atributos privados de uma classe, é necessário criar métodos para isso, os quais chamamos de métodos GET e SET

### GET
Get é um método que será criado para retornar o valor de um atributo, a nomenclatura desse método é padronizada para getNomeDoAtributo.

### SET
Set é um método que será criado para alterar o valor de um atributo, a nomenclatura desse método é padronizada para setNomeDoAtributo.

>class Conta{
>	private double saldo;
>	private double limite;
>	
>	public double getSaldo(){
>		return this.saldo;
>	}
>	
>	public setLimite(double limite){
>		this.limite = limite
>	}
>}

...

>class Programa{
>	public static void main(String[] args){
>		Conta conta = new Conta();
>		~~System.out.println(conta.saldo);~~
>		System.out.println(conta.getSaldo());
>		~~conta.limite = 1000;~~
>		conta.setLimite(1000);
>	}
>}

## Atributos final
Atributos com o modificador final são atributos que, uma vez instanciados, não poderão mais ter seu valor alterado. Um exemplo built-in disso em Java é o atributo PI da classe Math.

## Variáveis de classe e de instância
Quando criamos uma classe com alguns atributos e instanciamos alguns objetos dela, cada um desses objetos possuirá seus próprios atributos, que podem ser alterados independentemente das outras instâncias. Esses atributos são conhecidos como variáveis de instância.
Entretanto, também é possível que vários objetos diferentes de uma mesma classe compartilhem de uma variável em comum, que será igual para todos os objetos a qualquer momento da execução, isto é, qualquer alteração realizada nessa variável é válida para todas as instâncias daquela classe. Chamamos esse tipo de variável de variável de classe.
Para criar uma variável de classe, basta adicionar o modificador static ao inicializá-la.

### static
O modificador static é o diretor por trás das variáveis de classe. Ao inicializar uma variável da seguinte forma:

>Class bola{
>	static String cor = "Azul";
>}

E escrevermos o seguinte código na main:

>Class programa{
>	public static void main(String[] args){
>		Bola bola1 = new Bola();
>		Bola bola2 = new Bola();
>		bola1.cor = "Verde";
>		System.out.println(bola1.cor);
>		System.out.println(bola2.cor);
>	}
>}

Será printado no console:

>Verde
>Verde

Isso acontece pois, quando foi alterada em uma das instâncias (bola1), por ser um atributo do tipo static, esse atributo foi alterado em todas as instâncias daquele objeto. Vale ressaltar que atributos static não dependem de instâncias para serem acessados, podendo ser acessados diretamente pela própria classe, sendo válidos comandos tais como:

>Bola.cor = "Rosa";
>System.out.println(Bola.cor);

Visto esse aspecto, também é útil utilizar o modificador static em métodos de alguma classe para determinadas situações:

>class Conta{
>	private static int numeroDeContas;
>	
>	public static int getTotalContas(){
>		return Conta.numeroDeContas;
>	}
>}