# git branch -M main

Data: 21/06/2023
Empresa: Abstergo Industries
Responsável: Kassia ES

## Introdução
Este relatório apresenta o processo de implementação de ferramentas AWS na empresa Abstergo Industries, realizado por Kassia ES. O objetivo do projeto foi elencar 3 serviços AWS, com a finalidade de realizar diminuição de custos imediatos.

## Descrição do Projeto
O projeto de implementação de ferramentas foi dividido em 3 etapas, cada uma com seus objetivos específicos. A seguir, serão descritas as etapas do projeto:

Etapa 1: 
- EC2 - Elastic Compute Cloud
A principal finalidade do EC2 é oferecer uma plataforma flexível para executar aplicativos e cargas de trabalho em um ambiente de computação em nuvem. Ele permite que os usuários criem, configurem e dimensionem rapidamente instâncias de servidores virtuais conforme a demanda, sem a necessidade de investimentos antecipados em hardware físico.
- Eliminação de investimentos em hardware: Com o EC2, não há necessidade de adquirir e manter servidores físicos para executar os aplicativos da empresa. Isso reduz significativamente os custos iniciais de infraestrutura, como a compra de hardware, armazenamento e resfriamento.

- Escalabilidade sob demanda: O EC2 permite ajustar rapidamente a capacidade de computação conforme necessário. Em momentos de maior demanda, como durante períodos de pico ou lançamento de produtos, é possível aumentar temporariamente o número de instâncias EC2. Após o período de pico, é possível reduzir novamente a capacidade. Isso evita a necessidade de provisionar e manter recursos ociosos durante todo o tempo, resultando em economia de custos.

- Pague pelo uso real: Com o EC2, você paga apenas pelos recursos computacionais que utiliza. Os preços são baseados no tempo de execução das instâncias e na capacidade de computação utilizada. Isso permite uma alocação mais eficiente de recursos e redução de custos em comparação com a aquisição de servidores físicos que podem ter capacidade ociosa.

- Opções de instâncias otimizadas para custo: O EC2 oferece uma variedade de tipos de instâncias com diferentes níveis de desempenho e custo. É possível selecionar instâncias que atendam aos requisitos de desempenho do aplicativo, ao mesmo tempo em que otimizam os custos. Por exemplo, é possível escolher instâncias com uso mais eficiente de CPU, instâncias com armazenamento local para reduzir custos de armazenamento em outros serviços, ou instâncias spot para aproveitar preços reduzidos em períodos de baixa demanda.

- Gerenciamento simplificado: O EC2 oferece recursos de automação e gerenciamento simplificado por meio do uso de imagens de máquina virtual (AMI), scripts de inicialização, políticas de escalabilidade e integração com outras ferramentas da AWS. Isso ajuda a reduzir o esforço e o tempo gasto na configuração e manutenção dos servidores, resultando em economia de custos operacionais.

Etapa 2: 
- Amazon EC2 Auto Scaling
O principal foco do Amazon EC2 Auto Scaling é permitir que você dimensione automaticamente a capacidade do seu grupo de instâncias EC2 de acordo com a demanda. Ele ajuda a garantir que você tenha capacidade suficiente para lidar com o tráfego e a carga de trabalho, ao mesmo tempo em que evita a alocação excessiva de recursos ociosos.

- Redução de custos operacionais: Com o Auto Scaling, a empresa pode configurar políticas para aumentar ou diminuir automaticamente o número de instâncias do EC2 com base nas métricas de utilização, como a carga da CPU, o tráfego de rede ou outras métricas personalizadas. Isso permite que a capacidade seja ajustada sob demanda, evitando a necessidade de manter instâncias ociosas. Dessa forma, os custos operacionais são reduzidos, uma vez que a capacidade é dimensionada de acordo com a demanda real.

- Otimização de recursos: O Auto Scaling pode ajudar a otimizar o uso dos recursos disponíveis. Por exemplo, durante os períodos de baixa demanda, o número de instâncias pode ser reduzido automaticamente, economizando em custos de infraestrutura e energia. À medida que a demanda aumenta, o Auto Scaling adiciona automaticamente instâncias adicionais para lidar com o aumento da carga. Isso garante que a empresa esteja usando apenas os recursos necessários em cada momento, evitando desperdícios e reduzindo os custos associados.

- Flexibilidade de preços: A AWS oferece diferentes opções de instâncias do EC2 com preços variados. Com o Auto Scaling, a empresa pode usar instâncias com preços mais baixos durante períodos de baixa demanda e alternar para instâncias com maior capacidade durante períodos de pico. Essa flexibilidade permite aproveitar os preços sob demanda, instâncias reservadas ou instâncias spot, dependendo das necessidades específicas. Ao fazer uso eficiente das opções de preços, é possível obter economias significativas.

- Maior disponibilidade e escalabilidade: O Auto Scaling garante que a infraestrutura esteja dimensionada adequadamente para lidar com as variações de carga, garantindo a disponibilidade dos sistemas da empresa. Além disso, ele facilita a escalabilidade automática em resposta a eventos inesperados, como picos repentinos de demanda. Isso evita interrupções de serviço e perdas financeiras associadas a essas situações.


Etapa 3:
- CloudFront
O CloudFront é um serviço de entrega de conteúdo (CDN - Content Delivery Network). Ele é projetado para fornecer uma entrega de conteúdo de alta velocidade e baixa latência para usuários finais em todo o mundo.
O objetivo principal do CloudFront é reduzir a latência e melhorar o desempenho da entrega de conteúdo, como páginas da web, imagens, vídeos, arquivos de áudio e outros recursos estáticos e dinâmicos. Ele faz isso distribuindo esses recursos em servidores de borda localizados estrategicamente em vários locais ao redor do mundo.

- Redução de custos de infraestrutura: O CloudFront permite a distribuição eficiente de conteúdo estático, como imagens, documentos e outros recursos digitais. Ao utilizar o CloudFront, a indústria farmacêutica pode reduzir a carga nos servidores de origem, diminuindo a necessidade de investimentos em infraestrutura adicional para lidar com picos de tráfego. Isso pode resultar em economia de custos significativa, especialmente em momentos de alta demanda.

- Melhoria do desempenho: O CloudFront ajuda a melhorar o desempenho da entrega de conteúdo, reduzindo a latência e melhorando o tempo de resposta. Isso é especialmente importante para operações na indústria farmacêutica que dependem da transferência rápida de informações, como sistemas de gestão de inventário, compartilhamento de dados de pesquisa, colaboração entre equipes e acesso a documentos regulatórios. Com um melhor desempenho, os processos internos podem ser mais eficientes, resultando em economia de custos operacionais.

- Menor uso de largura de banda: Ao armazenar em cache o conteúdo em servidores de borda geograficamente distribuídos, o CloudFront reduz a quantidade de tráfego de dados que precisa ser transferido do servidor de origem para o usuário final. Isso resulta em uma redução no uso de largura de banda, o que pode levar a economias de custos em operações com altos volumes de transferência de dados, como o compartilhamento de grandes conjuntos de dados entre equipes de pesquisa ou o acesso a informações clínicas em várias localidades.Descrição de caso de uso

## Conclusão
A implementação de ferramentas AWS na empresa Abstergo Industries tem como esperado obter flexibilidade, escalabilidade, otimização do uso de recursos e redução dos custos operacionais, o que aumentará a eficiência e a produtividade da empresa. Recomenda-se a continuidade da utilização das ferramentas implementadas e a busca por novas tecnologias que possam melhorar ainda mais os processos da empresa.

## Anexos

[lista de anexos, como manuais, documentos, planilhas, entre outros]

Assinatura do Responsável pelo Projeto:

#### _Kaes_