- Introdução
    - O objetivo do curso é apresentar as regras essenciais para a construção de códigos com base na linguagem Java.

Aula 1 - Anatomia das Classes

Etapa 1 - Anatomia das Classes 1

- Dicas
    - A escrita de código de um programa é feito através da composição de palavras pré-definidas pela linguagem com as expressões que utilizamos para determinar o nome dos nossos arquivos, classes, atributos e métodos.
    - É muito comum mesclarmos expressões no idioma americano com o nosso vocabulário. Existem projetos que recomendam que toda a implementação do seu programa seja escrita na língua inglesa.

- Sintaxe de declaração de uma nova classe:
    - public class MinhaClass {
        - // SEU CÓDIGO AQUI
        
        } 
        
- Criando um [projeto.Java](http://projeto.Java) no vsCode
    - Todos os arquivo que eu gerar, sempre começar com letra maiúscula e palavras complementares também, exemplo : MinhaClasse
    - Se a “MinhaClasse” for executável, ela tem um método principal “main”, ele possui um padrão, que seria :
        - public statis void(significa que só vai executar não irá retornar nada) main (String [] args) {}
            - {} → é o corpo, sempre abrir e fechar, , sempre iremos controlar e separar adequadamente, lembrar de potes, tudo dentro do pote”{}” pertence ao pote, então no código terei diversos potes (lembrar de uma boneca russa)
            - args → argumentos, parâmetros
- Classes
    - Todas classes precisa existir dentro da pasta src do nosso projeto, disponibiliza um bloco geral de códigos.

Etapa 2 - Anatomia das Classes 2

- Padrão de nomenclatura
    - Quando se trata de escrever códigos na linguagem Java, é recomendado seguir algumas convenções de escrita. Esses padões estão expressos nos itens abaixo:
        - Arquivo .java: Todo arquivo .java deve começar com a letra MAIÚSCULA. Se a palavra for composta, a segunda palavra também deve ser maiúscula, exemplo:
            
            Calculadora.java, CalculadoraCientifica.java
            
        - Nome da classe no arquivo: A classe deve possuir o mesmo nome do arquivo.java, exemplo:
            
            public class “nome do arquivo”
            
        - Nome de variável: Toda variável deve ser escrita com letra minúscula, porém se a palavra for composta, a primeira letra da segunda palavra deverá ser MAIÚSCULA, exemplo: ano e anoFabricacao. O nome dessa prática para nomear variáveis dessa forma se chama “camelCase”
        - Obs: Existe uma regra adicional para variáveis quando na mesma queremos identificar que ela não sofrerá alteração de valor, exemplo: queremos determinar que uma variável de nome “br” sempre representará “Brasil” e nunca mudará o seu valor, logo, determinamos como escrita o código abaixo:
            
            1 “final” String BR = “Brasil”
            
            2 double PI = 3.14
            
            3 int ESTADOS_BRASILEIRO = 27
            
            4 int ANO_2000 = 2000
            
        - Para declarar uma variável nós podemos utilizar caracteres, números e símbolos, porém devemos seguir algumas regras da linguagem.
            - Deve conter apenas letras, _ , $ ou os números de 0 a 9
            - Deve obrigatoriamente se inicial por uma letra (preferencialmente), _ ou $, jamais com um número
            - Deve iniciar com uma letra minúscula (boa prática - ver abaixo)
            - Não pode conter espaços
            - Não podemos usar palavras-chave da linguagem
            - O nome deve ser único dentro de um escopo
            

Etapa 3 - Anatomia das Classes 3

- Declarando variáveis e métodos
- Como identificar entre declarações de variáveis e métodos em nosso programa? Existe uma estrutura comum para ambas as finalidades, exemplo:
    - Decalarar uma variável em Java segue sempre a seguinte estrutura:
        
        ```java
        // Estrutura
            Tipo NomeBemDefinido = Atribuição (Opcional em alguns casos)
        
        //Exemplo
        
            int idade = 23;
            double altura = 1.62
            Dog Spike;
        // Observe que a várial Dog Spike não possui atribução/valor
        ```
        
- Declarando métodos em Java segue uma estrutura bem simples:
    - 
    
    ```
    //Estrutura
    
        TipoRetorno NomeObjetivoNoInfinitivo Parametro()
    
    //Exemplo
    
        int somar (int numeroUm, int numero2)
    
        String formatarCep (long cep)
    ```
    

Etapa 4 - Anatomia das Classes 4

- Identação
    - Basicamente indentar é o termo utilizado para escrever o código do programa de forma hierárquica, facilitando assim a visualização e o entendimento do programa.

Etapa 5 - Anatomia das Classes 5

- Organizando arquivos
    - A medida que nosso sistema vai evoluindo, surgem novos arquivos (código fonte) em nossa estrutura de arquivos do projeto. Isso exige que seja realizado uma organização desses arquivos através dos pacotes (packges)

Etapa 6 - Anatomia das Classes 6

- Java Beans
    - Uma das maiores dificuldades na programação é escrever algoritmos legíveis a níveis que sejam compreendidos por todo seu time ou por você mesmo no futuro. Para isso a linguagem Java sugere, através de convenções, formas de escrita universal para nossas classes, atributos, métodos e pacotes.
- Variáveis
    - Mais cedo já aprendemos algumas regras de declaração de variáveis, mas agora iremos conhecer algumas sugestões de nomenclatura.
        - Uma variável deve ser clara, sem abreviações ou definição sem sentido;
        - Uma variável é sempre no singular, exceto quando se referir a um array ou coleção
        - Defina um idioma único para suas variáveis. Se você for declarar variáveis em inglês, defina todas em inglês

Aula 2 - Variáveis

Etapa 1 - Variáveis 1 e 2

- Ensinando como vincular e utilizar o repositório direto da GITHUB

Etapa 2 - Variáveis 3

- Tipos e Variáveis
    - Tipos e dados
        - No Java, existem algumas palavras reservadas para a representação dos tipos de dados básicos que precisam ser manipulados para a construção de programas. Estes tipos de dados são conhecidos como tipos primitivos (Primitive Types)
    - Os oito tipos primitivos em Java são:
        - int, byte, short, long, float, double, boolean e char
            - Estes tipos não são considerados objetos e portanto representam valores brutos.
                
                Eles são armazenados diretamente na pilha de memória. (Memory stack)
                
        
        - Byte - Low - 1 byte - 128
        - Short - Middle Low - 2 bytes - 32.768
        - Int - Middle - 4 bytes - 2.147.483.648
        - Long - High - 8 bytes - 9.223.372.036.854.775.808
        
    - Os tipos primitivos que podem conter partes fracinárias podem ser representador por dois tipos:
        - Float - 4 bytes - 3,4028E + 38
        - Double - 8 bytes - 17976 + 308
    
    - Apesar do tipo float ocupar metade da memória consumida do que um tipo double, ele é menos utilizado. Ele sofre uma limitação que compromete seu uso em determinadas situações: somente mantém uma precisão decimal entre 6 e 7 dígitos.
    - Atualmente, com os computadores modernos, se tornou desnecessário utilizar os tipos short e byte, pois nao precisamos nos preocupar tanto assim com o espaço de memória reduzido.
    - Da mesma forma, dificilmente utilizaremos o tipo long, pois não é tão comum trabalharmos com valores tão grandes.
    - Portanto, para representar números, na grande maioria das vezes utilizamos o tipo int para representar números inteiros ou double para representar números fracionados.
    - O ponto mais relevante em compreender a definição dos tipos de dados é o momentos da definição do tipo para uma variável. Qual tipo de dados eu utilizaria para determinar a idade de uma pessoa ou o salário de um funcionário?

- Declaração de Variáveis
    - Variável é uma identificação de um espaço em memória utilizado pelo nosso programa. Seguindo as convenções em linguagem de programação, toda variável é composta por: tipo de dados + identificação + valor atribuído.
        
        A estrutura padrão para se declarar uma variável sempre é:
        
        <Tipo> <nomeVariavel> <atribuicaoDeValorOpcional>
        
        Exemplos abaixo:
        
        ```java
        int idade; //Tipo "int", nome "idade", com nenhum valor atribuído
        int anoFabricacao = 2021; //tipo "int", nome "anoFabricacao" com valor 2021.
        double salarioMinimo = 2500; // tipo "double", nome "salarioMinimo" valor 2.500
        ```
        
        Atenção: existe algumas peculiaridades a trabalhar com alguns tipos específicos. Observe no exemplo abaixo:
        
        ```java
        public class TipoDados {
            public static void main(String[] args) {
                byte idade = 123;
                short ano = 2023;
                int cep = 12234809; // se começar com zero, talvez tenha que ser outro tipo
                long cpf = 98765432109L; // se começar com zero, talvez tenha que ser outro tipo
                float pi = 3.14F; // Se for tipo float precisa terminar com "F" se nã ele julgara que é um tipo double
                double salario = 1275.33;
           }
        }
        ```
        

Etapa 4 - Variáveis 4

- Variáveis e Constantes
    - Uma variável é uma área de memória, associada a um nome, que pode armazenar valores de um determinado tipo. Um tipo de dado define um conjunto de valores e um conjunto de operações. Java é uma linguagem com rigidez de tipos, diferente de linguagens como JavaScript, onde declarar o tipo da variável não é obrigatório.
    - No Java utilizamos identificadores que representam uma referência (ponteiro) a um valor em memória, e esta referência pode ser redirecionada a outro valor, sendo portanto esta a causa do nome “variável”, pois o valor pode variar.
    - Já as CONSTANTES são valores armazenados em memória que não podem ser modificados depois de declarados. Em Java, esses valores são representados pela palavra reservada final, seguida do tipo.
        
        Por convenção, CONSTANTES são sempre escritas em CAIXA ALTA
        
        Abaixo temos um exemplo explicativo sobre o uso:
        
        ```java
        public class TiposVariaveis {
            public static void main(String[] args) throws Exception {
                //tipo primitivos
                //estudar a classe String que representa  texto na aplicação
        
                String meuNome = "Julio Antonel"
                
                
                double salarioMinimo = 2500;
        
                short numeroCurto = 1;
                int numeroNormal = numeroCurto;
                short numeroCurto2 = (short) numeroNormal;
        
                int numero = 5;
        
                numero = 10;
        
                System.out.println(numero);
        
            }
        }
        ```
        
    

Aula 3 - Operadores

- Símbolos especiais que tem um significado próprio para a linguagem e estão associados a determinadas operações
    - Simbologia
        - **=** → Operador de atribuição, é utilizado para definir o valor inicial ou sobrescrever o valor de uma variável em Java definimos um tipo, nome e opcionalmente atribuímos um valor à variável através do operador de atribuição.
        - + → Além da adição, quando utilizado em variáveis do tipo texto, realizará a “concatenação de textos”(Que é pegar uma palavra e juntar com outra).
- Unários
    - Esses operadores são aplicados juntamente com um outro operador aritmético. Eles realizam alguns trabalhos básicos como incrementar, decrementar, inverter valores numéricos e booleanos.
        - ++ → incremento de valor em 1 unidade
        - - - → decrementa o valor em 1 unidade
        - ! → operador de negação, nega valor de uma expressão booleana

- Ternário
    - O operador de condição ternária é uma forma resumida para definir uma condição e escolher por um dentre dois valores. Você deve pensar numa condição e escolher por um dentre dois valores. Você deve pensar numa condição ternária como se fosse uma condição IF normal, porém, de uma forma em que toda a sua estrutura estará escrita numa única linha.
    - É representado pelos símbolos **“ ?: “**
    - Utilizados na seguinte sintaxe :
    - <Expressão Condicional> ? <Caso condição seja true> : <Caso condição seja false>

- Relacionais
    - Os operadores relacionais avaliam a relação entre duas variáveis ou expressões. Neste caso, mais precisamente, definem se o operando à esquerda é igual, diferente, menor, menor ou igual, maior ou maior ou igual ao da direita, retornando um valor booleano como resultado.
        - == → Quando desejamos verificar se uma variável é IGUAL a outro
        - ! = → Verificar se é DIFERENTE
        - > → Verificar se é MAIOR QUE
        - > = → Verificar se é MAIOR OU IGUAL
        - < → Verificar se é MENOR QUE
        - < = → Verificar se é MENOR OU IGUAL

- Lógicos
    - Os operadores lógicos representam o recurso que nos permite criar expressões lógicas maiores a partir da junção de duas ou mais expressões.
        - && Operador Lógico “E”
        - |  | - Operador Lógico “OU”
        

Aula 4 - Métodos

- Uma classe é definida por atributos e métodos. Já vimos que atributos são, em sua grande maioria variáveis de diferentes tipo e valores. Os métodos, por sua vez, correspondem a funções ou sub-rotinas disponíveis dentro de nossas classes.

- Critério de nomeação de Métodos
    - Deve ser nomeado como verbo
    - Seguir o padrão CamelCase (Todas as letras minúsculas com a exceção da primeira letra da segunda palavra). Exemplo:
        - abrirConexao
        - concluirPorcessamento

- Atenção
    - Não existe em Java o conceito de métodos globais. Todos os métodos devem SEMPRE ser definidos dentro de uma classe.
    
- Critério de definição de métodos
    
    Para chegar a essa conclusão, utilizar a convenção estrutural para todos os métodos. Essa convenção é determinada pelos aspectos abaixo:
    
    - Qual a proposta principal do método?
        - Você deve se perguntar constantemente até compreender a real finalidade do mesmo.
    - Qual o tipo de retorno esperado após executar o método?
        - Você deve analisar se o método será responsável por retornar algum valor ou não.
    - OBS: Caso o método não retorne nenhum valor, ele será representado pela palavra-chave **void**
    
    - Quais os parâmetros serão necessários para execução do métodos?
        - Os métodos as vezes precisão de argumentos como critérios para a execução
    - O Método possui o risco de apresentar alguma exceção ?
        - Exceções são comuns na execução de métodos, as vezes é necessário prever e tratar a possível existência de uma exceção.
    - Qual a visibilidade do método?
        - Será necessário que o método seja visível a toda aplicação, somente em mesmo pacotes, através de herança ou somente a nível a própria classe.
  - Exemplos:
    - 
        
        ```java
        public class MyClass {
        
        public double somar(int num1, int num2){
        	//LOGICA - FINALIDADE DO MÉTODO
        	return ... ;
        }
        
        public void imprimir(String texto){
        	//LOGICA - FINALIDADE DO MÉTODO
        	//AQUI NÃO PRECISA DO RETURN
        	//POIS NÃO SERÁ RETORNADO NENHUM RESULTADO
        }
        // throws Exception : indica que o método ao ser utilizado
        // poderá gerar uma exceção
        public double dividir(int dividendo, int divisor) throws Exception{}
        
        // este método não pode ser visto por outras classes no projeto
        private void metodoPrivado(){}
        
        //alguns equívocos estruturais
        public void validar(){
        	//este método deveria retornar algum valor
        	//no caso boolean (true ou false)
        }
        public void calcularEnviar(){
        	//um método deve representar uma única responsabilidade
        }
        public void gravarCliente(String nome, String cpf, Integer telefone, ....){
        	//este método tem a finalidade de gravar
        	//informações de um cliente, por que não criar
        	//um objeto cliente e passar como parâmetro ?
        	//veja abaixo
        }
        public void gravarCliente(Cliente cliente){}
        //ou
        public void gravar(Cliente cliente){}
        
        }
        ```
        
    
- Exercitando
    - Exemplo de uma classe para representar uma SmartTV onde:
        - Ela tenha as características: ligada (boolean), canal (int) e volume (int)
        - Nossa TV poderá ligar e desligar e assim mudar o estado ligada
        - Nossa TV aumentará e diminuirá o volume sempre em +1 ou -1
        - Nossa TV poderá mudar de canal de 1 em 1 ou definindo o número correspondente.
    
    - Código sub:
        - 
            
            ```java
            public class SmartTv {
                boolean ligada=false;
                int canal=1;
                int volume = 25;
            
                public void mudarCanal (int novoCanal){
                    canal = novoCanal;        
                }
            
                public void mudarCanal (){
                    canal++;
                }
            
                public void voltarCanal (){
                    canal--;
                }
            
                public void aumentarVolume(){
                    volume++;
                    System.out.println("Aumentando o volume para: " + volume);
                    //volume = volume + 1;
                    
                }
                
                public void diminuirVolume(){
                    volume--;
                    System.out.println("Diminuindo o volume para: " + volume);
                    //volume = volume - 1;
                    
                
                }
                
                public void ligar (){
                    ligada=true;
                }
                public void desligar(){
                    ligada=false;
            
                }
            
            }
            ```
            
        
    - Código main:
        - 
            
            ```java
            public class Usuario {
                public static void main(String[] args) throws Exception {
                    
                    SmartTv smartTv = new SmartTv();
            
                    smartTv.diminuirVolume();
                    smartTv.diminuirVolume();
                    smartTv.diminuirVolume();
                    smartTv.aumentarVolume();
            
                    System.out.println("Canal Atual? : " + smartTv.canal);
                    smartTv.mudarCanal(13);
                    System.out.println("Canal Atual? : " + smartTv.canal);
            
                    System.out.println("Volume Atual : ");
            
                    System.out.println("TV Ligada ? : " + smartTv.ligada);
                    System.out.println("Volume Atual? : " + smartTv.volume);
            
                    smartTv.ligar ();
                    System.out.println("Novo status -> TV Ligada ? : " + smartTv.ligada);
                }
            
            }
            ```
            

Aula 5 - Escopo

- O escopo pode ser entendido como ,o ambiente onde uma variável pode ser acessada. Em Java, o escopo de variáveis **vai de acordo com o bloco onde ela foi declarada**.
    - A variável é criada no primeiro acesso à ela, se tornando inacessível após o interpretador sair do bloco de execução, ao qual ela pertence. Portanto, esta variável não pode ser lida ou manipulada por rotinas e códigos que estão fora do seu bloco de declaração, ou seja, fora do escopo da variável.
    - Em uma Classe, podemos visualizar a diferença de escopos. Os atributos (variáveis) são declarados no corpo principal da Classe, sendo portanto, acessíveis por todos os métodos.
    - Caso você declare uma variável DENTRO DE UM MÉTODO, o escopo dessa variável está limitado apenas ao corpo desse método, ou seja, dentro das chaves que limitam o método.
    - Uma parte fundamental na elaboração de algoritmos simples ou complexos é determinar a localização do código em questão. Sem um domínio sobre escopo de códigos, seu projeto tende a conter falhas estruturais e comprometer a proposta principal da aplicação.
    
    ```
    public class Conta {
    //variavel da classe conta
    double saldo=10.0;
    
    public void sacar(Double valor) {
    	//variavel local de método
    	double novoSaldo = saldo - valor;
    }
    public void imprimirSaldo(){
    	//disponível em toda classe
    	System.out.println(saldo);
    	//somente o método sacar conhece esta variavel
    	System.out.println(novoSaldo);
    
    }
    public double calcularDividaExponencial(){
    	//variável local de método
    	double valorParcela = 50.0;
    	double valorMontante = 0.0; // começando a variável com valor zero
    	for(int x=1; x<=5; x++) {//x variável de escopo de fluxo
    		//esta variável será reiniciada a cada execução for
    		double valorCalculado = valorParcela * x;
    		valorMontante = valorMontante + valorCalculado;
    	}
    	//escopo de fluxo
    	//x e valorCalculado nunca estarão disponíveis fora do for
    
    	return valorMontante;
    }
    
    ```
    
    }
    

Aula 6 - Palavras Chaves

Palavras reservadas, são identificadores de uma linguagem que já possuem uma finalidade específica, portanto, não podem ser utilizados para nomear variáveis, classes, métodos ou atributos.

A linguagem Java possui 52 palavras reservadas. Todas essas palavras são classificadas em grupos e escritas com letra minúscula, sendo identificadas com uma cor especial pela maioria das IDE's. Abaixo temos a lista de palavras agrupadas por suas finalidades.

![Untitled](https://s3-us-west-2.amazonaws.com/secure.notion-static.com/00727950-a739-4fce-93b7-e265790693db/Untitled.png)

- Controle de pacotes
    - **import:** importa pacotes ou classes para dentro do código;
    - **package:** especifica a que pacote, todas as classes de um arquivo pertencem.

- Modificador de acess
    - **public:** acesso de qualquer classe;
    - **private:** acesso apenas dentro da classe;
    - **protected:** acesso por classes no mesmo pacote e subclasses.

- Primitivos
    - **boolean:** um valor indicando verdadeiro ou falso;
    - **byte:** um inteiro de 8 bits (signed);
    - **char:** um character unicode (16-bit unsigned);
    - **double:** um número de ponto flutuante de 64 bits (signed);
    - **float:** um número de ponto flutuante de 32 bits (signed);
    - **int:** um inteiro de 32 bits (signed);
    - **long:** um inteiro de 64 bits (signed);
    - **short:** um inteiro de 32 bits (signed);
    - **void:** indica que o método não tem retorno **de valor.**

- Modificadores de classes, variáveis ou métodos
    - **abstract:** classe que não pode ser instanciada ou método que precisa ser implementado, por uma subclasse não abstrata;
    - **class:** especifica uma classe;
    - **extends:** indica a superclasse que a subclasse está estendendo;
    - **final:** impossibilita que uma classe seja estendida, que um método seja sobrescrito ou que uma variável seja reinicializada;
    - **implements:** indica as interfaces que uma classe irá implementar;
    - **interface:** especifica uma interface;
    - **native:** indica que um método está escrito em uma linguagem dependente de plataforma, como o C;
    - **new:** instancia um novo objeto, chamando seu construtor;
    - **static:** faz um método ou variável pertencer à classe ao invés de às instâncias;
    - **strictfp:** usado em frente a um método ou classe para indicar que os números de ponto flutuante seguirão as regras de ponto flutuante, em todas as expressões;
    - **synchronized:** indica que um método só pode ser acessado por uma thread de cada vez
    - **transient:** impede a serialização de campos;
    - **volatile:** indica que uma variável pode ser alterada durante o uso de threads.;

- Tratamento de erros
    - **assert:** testa uma expressão condicional, para verificar uma suposição do programador;
    - **catch:** declara o bloco de código usado para tratar uma exceção;
    - **finally:** bloco de código, após um try-catch, que é executado independentemente do fluxo de programa seguido ao lidar com uma exceção;
    - **throw:** usado para passar uma exceção para o método que o chamou;
    - **throws:** indica que um método pode passar uma exceção para o método que o chamou;
    - **try:** bloco de código que tentará ser executado, mas que pode causar uma exceção.
    
- Variáveis de referência
    - **super:** refere-se a superclasse imediata;
    - **this:** refere-se a instância atual do objeto.
    
- Palavras reservadas não utilizadas
    - **const:** Não utilize para declarar constantes; use public static final;
    - **goto:** não implementada na linguagem Java, por ser considerada prejudicial.

- Literais reservados
    
    De acordo com a Java Language Specification, **null**, **true** e **false** são tecnicamente chamados de valores literais, e não keywords. Se você tentar criar algum identificador com estes valores, você também terá um erro de compilação.
    

- **Escopo de uso**

| Uso | Palavras | Observação |
| --- | --- | --- |
| Arquivo | package, import, static. |  |
| Classe | public ou protected ou private + final ou abstract + extends ou implements. | private (em caso de classe interna), final ou abstract |
| Método | public ou protected ou private + static ou final ou abstract + void e return. | void em caso de não ter retorno ou return se houver |
| Atributo | public ou protected ou private + static ou final + tipo primitivo. | **** |
- **Palavras "opostas"**

Assim como nas classificações gramaticais da língua portuguesa, existem algumas palavras que são completamente opostas (antônimas) na linguagem Java conforme tabela abaixo:

| Palavra | Palavra | Explicação |
| --- | --- | --- |
| package | import | Enquanto package determina o diretório real da classe, o import informa de onde será importada a classe. Isso porque, podemos ter classes de mesmo nome. |
| extends | implements | enquanto extends determina que uma classe estende outra classe, implements determina que uma classe implementa uma interface, porém nunca o contrário. |
| final | abstract | enquanto final determina fim de alteração de valor ou lógica comportamental, abstract em métodos, exige que sub-classes precisarão definir comportamento e um método abstrato. NOTA: Se uma classe contém um único método abstrato, toda classe precisa ser. |
| throws | throw | Esta é uma das situações mais complicadas, de compreensão destas duas palavras. Enquanto a throws determina que um método pode lançar uma exceção, throw é a implementação que dispara a exceção**. Vamos conhecer mais sobre este conceito no assunto Exceções.** |

Aula 7 - Documentação

- Documentação
    - Uma das maiores características da linguagem Java é que, desde suas primeiras versões, tínhamos em nossas mãos, uma documentação rica e detalhada dos recursos da linguagem.
    - Conforme site oficial, podemos compreender e explorar, todos os recursos organizados por pacotes e classes bem específicas, sem nem mesmo escrever uma linha de código.
    - Hoje, costuma-se afirmar que, para se tornar um desenvolvedor nível avançado, é um requisito imprescindível adquirir a habilidade de compreender, a documentação oficial da linguagem e dos frameworks que são incorporados nos projetos atuais.

- Tag
    - Mas e quais as informações, que obtemos através de classes documentadas, na linguagem ? Java
    - Documentation é composto por tags que, representam dados relevantes para a compreensão da proposta de uma classe e os conjuntos de seus métodos e atributos conforme tabela abaixo:
        
        
        | Tag | Descrição |
        | --- | --- |
        | @autor | Autor / Criador |
        | @version | Versão do recurso disponibilizado |
        | @since | Versão / Data de início da disponibilização do recurso |
        | @param | Descrição dos parâmetros dos métodos criados |
        | @return | Definição do tipo de retorno de um método |
        | @throws | Se o método lança alguma exceção |
    - Abaixo, iremos ilustrar a classe Calculadora com um exemplo de documentação, destacando as **tags** mais utilizadas:
        
        - 
        
        /**
        
        - <h1>Calculadora</h1>
        - A Calculadora realiza operações matemáticas entre números inteiros
        - <p>
        - <b>Note:</b> Leia atentamente a documentação desta classes
        - para desfrutar dos recursos oferecidos pelo autor
        - 
        - @author Gleyson Sampaio
        - @version 1.0
        - @since 01/01/2022
        */
        public class Calculadora {
        /*
            - Este método é utilizado para somar dois números inteiros
            - @param numeroUm este é o primeiro parâmetro do método
            - @param numeroDois este é o segundo parâmetro do método
            - @return int o resultado deste método é a soma dos dois números.
            */
            public int somar(int numeroUm, int numeroDois) {
            return numeroUm + numeroDois;
            }
            }
            
    - Tipos de comentarios
        - One Line
        - Multi Line
        - Documentation
        
        - Subsequentimente:
        
        ```
        public class Comentarios {
            public static void main(String[] args) {
                // Olá, eu sou um comentário em uma única linha
        
                /* Olá,
         * Eu sou um comentario
         * que posso ser mais detalhadod
         * quando necessário
         */
        
            }
            /** 
         * Estas duas estrelinhas acima
         * é para identificar que você
         * pretende elaborar um comentário
         * a nível de documentação.
         * Que incrível !!!
         */
            public void metodo(){
        
            }
        
        }
        ```
        
- Javadoc
    - **Javadoc** é um gerador de documentação criado pela Sun Microsystems , para documentar a API dos programas em Java, a partir do código-fonte. O resultado é expresso em HTML. É constituído, basicamente, por algumas marcações muitos simples, inseridas nos comentários do programa.
        
        Este sistema, é o padrão de documentação de classes em Java, onde muitas das IDEs desta linguagem irão automaticamente gerar um Javadoc em HTML.
        
- Aula 8 - Terminal e Argumentos.
    - Terminal
        - Nem sempre executamos nosso programa Java pela IDE, já pensou, nossos clientes tendo que instalar o Eclipse ou VsCode para rodar o sistema em sua empresa ?
        - Com a JVM devidamente configurada, nós podemos criar um executável do nosso programa e disponibilizar o instalador para qualquer sistema operacional.
        - No nosso caso, iremos aprender como executar um programa Java via terminal, como MS - DOS ou terminal do VsCode.
        
    - Argumentos
        - Quando executamos uma classe, que contenha o método main, o mesmo permite que passemos um array `[]`
         de argumentos, do tipo String. Logo, podemos após a definição da classe a ser executada, informar estes parâmetros, exemplo:
            - java MinhaClasse agumentoUm argumentoDois
            
    - Scanners
        - Nos exemplos anteriores, percebemos que podemos receber, dados digitados pelo usuário do nosso sistema, porém, tudo precisa estar em uma linha e também é necessário informar os valores nas posições correspondentes.
        - Esta abordagem pode deixar margens de execução, com erro do nosso programa. Para isso, com a finalidade de deixar as nossas entradas de dados mais seguras, agora vamos receber estes dados via **Scanner**.
        - A classe **Scanner,** permite que o usuário tenha, uma interação mais assertiva com o nosso programa, veja como vamos mudar o nosso programa **`AboutMe`** para deixar mais intuitivo aos usuários:
