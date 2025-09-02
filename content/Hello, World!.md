
Recentemente voltei a usar AI para preencher lacunas no meu código e notei o quanto eu estava com a lógica falha.

Passei a depender tanto de IA para preencher lacunas no meu código que até o basico fui perdendo, vejam bem, eu 
não sou desenvolvedor, não me considero como um, sempre que precisei programar foi para resolver alguma coisa para mim mesmo. Porém recentemnete voltei a estudar programação começando por Java e agora Go, Java por questões
de mercado, C# e Java ainda são muito fortes para quem está querendo entrar no mercado, eu não tenho foco desenvolvimento, então fui estudar apenas por curiosidade.

E olhem só, eu que sempre desdenhei Java acabei gostando, ainda me confundo um pouco com Maven, mas é ok, isso eu deixo na mão da IA mesmo e só me preocupo com o código. Mas retornando ao assunto principal, decidi estudar Go pela relevancia que estou vendo em vagas DevOps, onde eu quero focar. Porém Go tem suas peculiaridades comparadas as Java, acho que a mais fácil de mencionar seriam ``` structs ```, Go não tem classes e sim estruturas.

```
type Estrutura struct{
  Nome string // Classes começando com letras maiusculas são públicas! 
  idade int // Classes começando com letras minusculas são privadas!

}

```
```

```
Outra coisa é como definir variaveis:
```
var Data int

```
Ou :

``` data := 10 ```

``` := ```

Go já permite você declarar o tipo da varivael ou assumir o tipo dela de acordo com o valor, é uma forma de economizar tempo, mas para quem ta iniciando as vezes fica confuso, querendo ou não é questão de pratica, ainda estou no primeiro projeto que devo postar em breve, relativamente simples, mas passos iniciais de qualquer Jr.

Além disso parsing em Go é muito divertido com structs:
Para fins simples um exemplo do json:
nome.json:
```
```
```
```
```
```
{
  "nome":{
    "Nome1",
    "Nome2"
}
} 
```
```

```
```
type Data struct {
  nome []string `json:"nome"`
}
```
```




