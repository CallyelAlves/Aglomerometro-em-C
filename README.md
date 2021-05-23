# Aglomerômetro

### Área de atuação

A nossa proposta tende a ser flexível em várias áreas. Pode ser aplicada em qualquer local público ou estabelecimentos nos quais seja observada a necessidade de um maior controle do fluxo de pessoas. Alguns exemplos principais são na área de educação, comércio e lazer.

### Problema

Devido ao vírus Covid-19 ter alto risco de contaminação, é bem acertado que deve-se evitar aglomeração em locais públicos e privados. é necessário que haja algum tipo de controle de entrada e saída de pessoas nesses locais, a fim de evitar aglomerações.
	
### Proposta

	Desenvolver uma aplicação que controle a quantidade ideal de pessoas de acordo com a capacidade espacial de um determinado ambiente. Em posse das informações de câmeras de segurança ou sensores infravermelhos para contabilizar a quantidade de pessoas, considerando a área do local para classificar os níveis de aglomeração.  

### Cálculo Considerado: 
	
Mínimo de distanciamento recomendado = 1 m  (Segundo a O.M.S.);
NAG = Area / Pessoas * 2,25.

De acordo com a recomendação da OMS é recomendado manter 1 metro de distância das demais pessoas, a fim de diminuir as chances de contágio do covid-19. Com isso, a base de cálculo de 1m de distância em todas as direções - 1m para esquerda, 1m para direita, 1m para frente e 1m para trás - resulta em uma área de 4m² por pessoa, para que assim haja o devido distanciamento. Porém, considerando as irregularidades(colunas, escadas, paredes...) e móveis dos estabelecimentos, que por si só já causam o distanciamento entre as pessoas, também o fato de que geralmente pessoas da mesma família frequentam juntos esses locais, sendo assim não há a necessidade obrigatória de distanciamento entre elas. Tendo esses pontos em vista, deliberou-se por uma base de distanciamento de 0,75m em todas as direções por pessoa, levando ao valor de 2,25m² por pessoa.	     


### Níveis de aglomeração:

nag = 1 -> aglomeração máxima aceitável;
nag > 1 -> aglomeração baixa;
nag < 1 -> aglomeração extrapolante.

### Estrutura dos dados:

área do local;
dados dos sensores.

Entrada/Saída;
Quantidade pessoas

Dados atuais(total de pessoas presentes no local)

Empregados;
Visitantes;


### Estrutura do programa

ler dados dos sensores;
manipular dados atuais;
calcular o nível de aglomeração;
quantidade de pessoas aceitáveis atual;
emitir alerta(seguranças);
oferecer dados através de site ou app (opcional);
