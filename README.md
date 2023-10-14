# BTCData
Conjunto de Dados Utilizado para Averiguar o Uso de Técnicas de Engenharia de Tráfego em Prefixos da Rede Bitcoin 

## Dados BGP

Os dados da rede e do BGP definimos a especificidade dos an ́uncios, o uso de prepending e a conectividade do ASes. Assim  ́e poss ́ıvel definir quais fatores relacionados a engenharia de tr ́afego podem facilitar ataques de sequestro de prefixo contra a rede Bitcoin, sejam eles com o intuito de particionar ou atrasar a rede. Os dados de roteamento utilizados são do dia 31 de Agosto de 2022 as 22:00 horas e do dia 1 de Agosto as 4:00 horas, ambos do coletor de São Paulo, disponibilizado em https://archive.routeviews.org/route-views2.saopaulo/bgpdata/.  Os dados compactados podem ser acessados utilizando a ferramenta BGPScanner: https://gitlab.com/Isolario/bgpscanner

### Exemplo dos Dados

```
=|23.94.207.0/24|57695 60068 174 36352|187.16.220.159|i|||174:21001 174:22013 57695:13000 60068:202 60068:2000 60068:2010 60068:7280|187.16.220.159 57695|1661550506|1
=|23.94.207.0/24|52694 174 36352|187.16.216.13|i||||187.16.216.13 52694|1661437924|1
=|23.94.207.0/24|264479 3356 1299 36352|187.16.222.156|i||||187.16.222.156 264479|1661431636|1
=|23.94.207.0/24|263009 174 36352|187.16.222.221|i|||1000:174|187.16.222.221 263009|1660888737|1
=|23.94.207.0/24|61573 1299 36352|187.16.221.27|i|||1299:35000|187.16.221.27 61573|1660714880|1
=|23.94.207.0/24|61595 174 36352|187.16.210.50|i||||187.16.210.50 61595|1660032364|1
```

## Bitnodes

Os dados utilizados do API do BitNodes s ̃ao os disponibilizados as 22:03 horas do dia 31 de Agosto de 2022 e do dia 1 de Agosto de 2023 às 3:01 horas, onde os campos extra ́ıdos foram o IP do no e o AS ao qual ele pertence, o qual o ultimo e identificado pela sigla AS seguida pelo numero do mesmo.

### Exemplo dos Dados

```
"nodes": {
        "135.181.56.49:8333": [
            70016,
            "/Satoshi:24.0.1/",
            1684328018,
            1033,
            796635,
            "static.49.56.181.135.clients.your-server.de",
            null,
            "FI",
            60.1717,
            24.9349,
            "Europe/Helsinki",
            "AS24940",
            "Hetzner Online GmbH"
        ],
        "34.91.195.229:8333": [
            70015,
            "/Satoshi:0.20.1/",
            1688176245,
            1037,
            796635,
            "229.195.91.34.bc.googleusercontent.com",
            "Groningen",
            "NL",
            53.2157,
            6.5765,
            "Europe/Amsterdam",
            "AS396982",
            "GOOGLE-CLOUD-PLATFORM"
        ],
```
