+++
date = '2025-09-02T11:11:08-03:00'
draft = true
title = '3 Anos Em TI'
+++
#3 anos em TI
## Começo

Primeiramente, eu não tenho exatamente 3 anos de TI, oficialmente é isso, mas eu comecei muito antes.
Em 2009-2010, quem jogou algum MMO provavelmente conheceu Ragnarok Online. Na cena brasileira, poucos eram aqueles afortunados que conseguiam pagar o bRO da LevelUp!, muitos conheceram por servidores "privates", alguns mais atualizados do que o bRO!

Eu sempre fui muito curioso, lembro que meu primeiro contato com desenvolvimento foi ver meu pai tentar quebrar a cabeça com o FrontPage, um programa da Microsoft para edição de sites. Era um software muito visual, pouco editor de código pelo que eu lembro.
Eu sabia que não era possível um "bom site" naquela época utilizar aquele programa, ele era muito limitado. Aos poucos fui descobrindo HTML, CSS e JavaScript.

Com essa cabeça curiosa, me aventurei em fóruns de desenvolvimento de emuladores de servidores de Ragnarok (saudosos eAthena e Cronus Emulator). A curiosidade de conseguir subir um servidor private desses me fez aprender Linux, scripting básico e até PHP para mexer no portal de cadastro do CeresCP!

Então, muito antes de atuar com TI, eu já era um moleque de 14-15 anos que provavelmente tinha mais conhecimento de redes e infra do que eu deveria pra começar um estágio...
Quando fui fazer a faculdade, fiquei entre duas escolhas: Sistemas e Mídias Digitais na UFC ou Jogos Digitais na Estácio... Pois é, se alguém conseguir voltar no tempo, dá um tapa nesse Rodrigo pra ele não seguir o sonho dele e ir pra SMD...
Na Estácio não aprendi nada, levei com a barriga, na época não precisava me preocupar com nada, meus pais só falavam pra focar nos estudos e me formar e fui fazendo isso, até que me formei, sem estágio, praticamente sem chances de entrar no mercado, me sentindo um inútil. Acabei entrando em depressão, quase 10 anos parado praticamente, até que com 27 anos consegui um emprego como Auxiliar de Infraestrutura e aí... aí nós começamos de verdade.

## Primeiro emprego

Primeira experiência vai te ensinar muito, se você tiver muita liberdade do que fazer, então você vai aprender de verdade, pode cometer erros e aprender com eles (preferencialmente), testar novas tecnologias e praticar soft skills.

Duas coisas importantes eu aprendi nessa época: a me comunicar — eu era praticamente um ogro socialmente, não falava a menos que falassem comigo.
A segunda, que eu era muito mais esperto do que eu achava. Não é questão de ser melhor que os outros, mas eu era realmente bom no que eu fazia.
A ansiedade do emprego novo no primeiro mês praticamente morreu, minhas métricas eram ótimas! Não tinha problema que eu não resolvesse, a não ser quando envolvia desenvolvimento, aí já não era comigo.
Mas ninguém me ensinou que, às vezes, você tem um colega que pode até parecer ter mais experiência, mas na verdade... não é bem assim...

### E

Vamos chamar esse colega de "E". E tinha 10 anos, segundo ele, de experiência com TI.
E era mais velho que eu, "mais experiente", porém cometia alguns erros... um tanto incomuns para 10 anos de TI e, principalmente, 10 anos de experiência em TI e ainda era Auxiliar (??)!

Mas vamos lá a um dos problemas pra exibir o porquê era incomum a experiência dele com os erros.
Nós tínhamos um servidor virtualizado em um VMware, nosso AD. Nessa época trabalhava de 14h às 22h, 6x1. Desde a manhã cedo eu estava acompanhando o chat da TI falando que nosso AD estava travando a cada 20min, reiniciavam e 20min depois travava.
E estava reiniciando o AD a cada 20min. Das 6h às 14h, esse servidor estava sendo reiniciado.
Acho que aqui vocês conseguem ver um dos problemas de E, certo? Em vez de diagnosticar, ele tentava pular o problema.

14h eu chego, abro o servidor, disco alto, ok...
Abro o VMware, snapshot rodando, ok... só esperar, certo? Errado. E, na hora que vê, vai meter o dedo no servidor...
Ok, entendi o problema, esperei o E sair, meu chefe já estava puto com a situação, chamou até pessoal de fora.
Fiz meu jogo de cintura, expliquei pra equipe que chegou que eu já estava resolvendo, 2h depois de deixar o servidor quieto, snapshot feito, problema resolvido!
Documentação de diagnóstico feita, eu lembro exatamente as seguintes linhas:

Diagnóstico de problema no AD xx/xx/2022
Analisar velocidade de disco, verificar utilização por usuários no Monitor de Recursos, caso utilização do servidor esteja baixa mas latência alta, verificar utilização do VMware.
Em caso de Snapshot, esperar finalizar o processo.
Em caso de falta de utilização, verificar Logs do VMware para análise de possível falha no disco.

Entreguei para o meu chefe, expliquei o processo, ele riu e pronto. Essa documentação deixei impressa e salva no computador que nós dois dividíamos, expliquei para E no dia seguinte.
Adivinha o que ele fez 2 meses depois quando o mesmo problema aconteceu?!

Aprendi muito nesse emprego, coloquei Veeam como solução de backup, Zabbix, Grafana para monitoramento. Pouco menos de um ano depois recebemos um analista de infra. Aprendi pra caralho!
Um dos melhores profissionais que conheci, não tinha problema em ensinar, acabou virando um grande amigo. Me deu muita liberdade para fazer testes, rodar projetos pra melhorar rede, implementamos um PiHole na rede pra melhorar utilização (e evitar o pessoal da madrugada acessar sites +18 na rede...).
Enfim, um ano e meio nesse emprego, já estava fazendo muita coisa, mas ainda recebendo pouco mais de um salário mínimo. Estava na hora de sair, eu sabia que já estava em um nível acima de auxiliar, aproveitei as férias, preparei o currículo e, 2 meses depois, aprovado para uma vaga de Analista de Sistemas Jr!

Não vou entrar muito nessa vaga, não fiz muita coisa, aprendi bastante SQL, mas não tinha muito o que fazer na real. Era um ERP baseado em SQL, poucas modificações eram necessárias.
O máximo que eu fiz foi um script com Python pra automatizar um processo desgraçado que levava 6h por semana para baixar notas fiscais. Reduzi isso pra 15min por semana, fizemos uns dashboards, lindos comparados ao BI que era em um Excel. Eu juro pra vocês, é real essa.

6 meses depois... Meu antigo chefe me chama de volta, o dobro do que eu ganhava antigamente, mais perto de casa, sem pegar ônibus, setor de suporte todo meu, mas todas as responsabilidades também seriam todas minhas. Não pensei duas vezes e fui, não aguentava mais ônibus.

## Dias atuais

Depois de um ano como Analista de Suporte, eu estava cansado. A liberdade toda que eu tinha me fez acabar pegando projetos para ajudar o desenvolvimento. Eu era suporte, infra, DevOps. Eu gostava, mas era muita coisa pra uma pessoa só.
Arrisquei começar a aplicar para vagas fora do Brasil.
Lembra a época que eu estava aprendendo a subir servidores de Ragnarok? Pois é, nessa época eu tive que aprender inglês para me virar, imersão durante um ano que fiquei preso em casa. Não assistia nada fora do YouTube americano. Pratiquei um pouco e... Passei! Engenheiro de Suporte, mais uma vez salário dobrado e, melhor de tudo, home office!

Aqui eu já tinha alguns diferenciais: ferramenta parceira principal deles era o Veeam, que eu já conhecia bastante, e AWS, que eles também usavam com tecnologias compatíveis. Então sim, uma certificação como a AWS ainda faz diferença, principalmente quando você está no final de um processo seletivo.
Se você está na dúvida de investir em um certificado desses, vale sim o investimento.

É isso, um pouco da minha trajetoria, vou tentar trazer algumas cronicas dos empregos passados, algumas que hoje da pra rir em vez de chorar, talvez as que só dê pra chorar também!
