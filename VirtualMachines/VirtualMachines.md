# Virtual Machines

[Link de Acesso](https://azure.microsoft.com/en-us/products/virtual-machines/#overview)

## Objetivo do Produto

Implementar máquinas virtuais com até 416 vCPUs e 12 TB de memória. Obtenha até 3,7 milhões de IOPS de armazenamento local por VM. Tire partido de até 30 Gbps Ethernet e da primeira implantação de 200 Gbps InfiniBand na nuvem. Seleccione os processadores subjacentes - AMD, Ampere (baseados em braço), ou Intel - que melhor satisfazem os seus requisitos.

## Usos

* Construir e implementar aplicações para a cloud.
* Experimentar um novo sistema operativo (SO), incluindo versões beta.
* Criação de um novo ambiente para tornar mais simples e mais rápido o desenvolvimento de cenários de teste de desenvolvimento.
* Fazer o backup do seu sistema operativo atual.
* Aceder a dados infectados por vírus ou executar uma aplicação antiga através da instalação de um SO antigo.
* Executar software ou aplicações em sistemas operativos para os quais não estavam originalmente previstos.

## Benefícios

* Poupança de custos - a partir de uma só peça de infra-estrutura, é possível reduzir drasticamente a sua pegada física de infra-estrutura.
* Agilidade e rapidez - A instalação de um VM é relativamente fácil e rápida e é muito mais simples do que fornecer todo um novo ambiente para os seus criadores.
* Tempo de inactividade reduzido - as VM's são tão portáteis e fáceis de mover de um hipervisor para outro numa máquina diferente - isto significa que são uma óptima solução para backup, no caso do anfitrião descer inesperadamente.
* Benefícios de segurança - Porque as máquinas virtuais funcionam em múltiplos sistemas operativos, a utilização de um sistema operativo convidado numa VM permite-lhe executar aplicações de segurança questionável e protege o seu sistema operativo anfitrião.

## Tipos de VM's

* A-Series - Entry-level VMs for dev/test
* Bs-Series - Economical burstable VMs
* D-Series - General purpose compute
* E-Series - Optimised for in-memory applications
* F-Series - Compute optimised virtual machines
* G-Series - Memory and storage optimised virtual machines
* H-Series - High Performance Computing virtual machines
* Ls-Series - Storage optimised virtual machines
* M-Series - Memory optimised virtual machines
* Mv2-Series - Largest memory optimised virtual machines
* N-Series - GPU enabled virtual machines

### A-Series

VMs económicos de nível de entrada para desenvolvimento e teste
Estes são geralmente utilizados em pequenos destacamentos onde o custo da consciência é superior ao desempenho. Estes só devem ser utilizados em implementações raras com VMs não voltadas para o cliente.

#### Preços Windows

![Windows](./A-Series/Windows%20Pricing.png)

#### Preços Linux

![Linux](./A-Series//Linux%20Pricing.png)

### Bs-Series

São máquinas virtuais económicas que fornecem uma opção de baixo custo para cargas de trabalho que normalmente funcionam com uma utilização de base de CPU baixa a moderada, mas por vezes precisam de explodir para uma utilização significativamente mais elevada da CPU quando a procura aumenta. Em idle, a Bs-Series irá guardar os créditos e utilizá-los mais tarde quando a utilização da CPU precisar de ultrapassar a linha de base.  Quando reiniciada, a Bs-Series perderá os seus créditos que podem levar horas a reconstruir sem grande impacto. Quando reiniciada sem quaisquer créditos em 'banca', a Bs-Series só terá acesso para permitir uma pequena fracção da utilização total da CPU até que um banco de créditos possa ser construído.

#### Preços Windows

![Windows](./Bs-Series/Windows%20Pricing.png)

#### Preços Linux

![Linux](./Bs-Series/Linux%20Pricing.png)

### D-Series

D-series VMs apresentam CPUs rápidas e uma configuração óptima CPU-to-memory, tornando-as adequadas para a maioria das cargas de trabalho de produção. As instâncias da série DSv3 transportam CPUs mais potentes e as mesmas configurações de memória e disco que a série D.  No entanto, estes núcleos de CPU são hyper-threaded, o que significa que um único núcleo físico de CPU está por trás de cada dois núcleos de CPU numa VM Dsv3.

Ds2-64 v3 instances (ie. Ds4v3 – 4 core x 16GB RAM)  são a mais recente geração de instâncias de uso geral hyper-threaded e baseiam-se no processador Intel Xeon® E5-2673 v3 (Haswell) de 2,4 GHz ou no mais recente processador Intel XEON® E5-2673 v4 (Broadwell) de 2,3 GHz. Podem atingir velocidades mais elevadas com a tecnologia Intel Turbo Boost 2.0. A D-Series suporta armazenamento SSD Standard e Premium.  

O melhor uso da D-Serie será para o desempenho, pois emparelham-se bem com SSD premium - uma obrigação para soluções ou camadas de apresentação que são orientadas para o cliente.  Não há muita diferença no preço com as instâncias v3 (em oposição à v2), o que as torna ideais.  

Os exemplos de casos de utilização incluem muitas aplicações de nível empresarial, bases de dados relacionais, caching in-memory, e análises. As últimas gerações são ideais para aplicações que exigem CPUs mais rápidas, melhor desempenho do disco local ou memórias mais elevadas.  

### E-Series

A família E-series de VM's está optimizada para aplicações pesadas em memória, tais como SAP HANA. Estas VMs são criadas com altos rácios de memória para núcleo, o que as torna bem adequadas para servidores de bases de dados relacionais, com caches médios a grandes, e análises in-memory. As VMs série E variam de 2 a 64 vCPUs e 16-432 GiB RAM, respectivamente. A série E suporta SSDs Azure Premium.

O melhor uso da E-Series será para anfitriões de sessões e colecções onde a linha de aplicações empresariais consome uma pegada de memória superior à normal por utilizador.  O software que é optimizado para anfitriões de sessões multi-utilizador pode muitas vezes consumir grandes pegadas de memória.

Exemplos de casos de utilização incluem SAP HANA, SAP S/4 HANA, SQL Hekaton e outras grandes cargas de trabalho críticas para o negócio in-memory.

### F-Series

Esta nova série de VMs, denominada F-Series, baseia-se no processador Intel Xeon® E5-2673 v3 (Haswell) de 2,4 GHz, que pode atingir velocidades de relógio até 3,1 GHz com a tecnologia Intel Turbo Boost 2.0. Este é o mesmo desempenho de CPU que a série Dv2 de VMs com 2GB de memória por núcleo de CPU a um preço por hora mais baixo. Isto coloca a F-Series como o melhor valor numa posição de preço-desempenho em Azure com base no preço de lista da F-Series dividido pela Unidade de Cálculo Azure (ACU) por núcleo.

Os VMs da F-Series são uma excelente escolha para servidores de jogos, servidores web e processamento de lotes. Qualquer carga de trabalho que não necessite de tanta memória ou SSD local por núcleo de CPU irá beneficiar do valor da Série F. Os tamanhos da Série F variam de um a 16 núcleos de CPU com opções para tamanhos optimizados de armazenamento tanto standard como premium.

### G-Series

Os tamanhos da G-Series são construídos para fornecer a maior memória, o maior poder de processamento, e a maior quantidade de SSD local de qualquer tamanho de máquina virtual oferecida pelo Azure. Este desempenho extraordinário permitirá implementar aplicações empresariais de grande escala, tais como grandes servidores de bases de dados relacionais (SQL Server, MySQL, etc.) e grandes bases de dados NoSQL (MongoDB, Cloudera, Cassandra, etc.). A G-Series oferece até 32 vCPUs usando o mais recente processador Intel® Xeon® da família E5 V3, 448 GB de memória, e unidades SSD locais de 6,59 TB. Em parte, essas VMs estão a funcionar em hardware físico dedicado.

Grandes bases de dados, soluções ERP, aplicações SAP, armazenamento de dados, aplicações que requerem muita memória.

### H-Series

Os VMs da H-Series são optimizados para aplicações impulsionadas por altas frequências de CPU ou por grandes requisitos de memória por núcleo. As VMs H-Series apresentam 8 ou 16 núcleos de processador Intel Xeon E5 2667 v3, até 14 GB de RAM por núcleo de CPU, e sem hiperthreading. A série H apresenta 56 Gb/sec Mellanox FDR InfiniBand numa configuração de árvore de gordura não bloqueadora para um desempenho RDMA consistente. As VMs da série H não são actualmente compatíveis com SR-IOV e suportam Intel MPI 5.x e MS-MPI.

Utilizado para aplicações de alto desempenho,Citado de Azure: Dinâmica de fluidos, análise de elementos finitos, processamento sísmico, simulação de reservatórios, análise de risco, automatização de desenho electrónico, renderização, faísca, modelação meteorológica, simulação quântica, química computacional, simulação de transferência de calor.

### Ls-Series

As VMs da série Ls estão otimizadas para armazenamento e são ideais para aplicações que requerem baixa latência, débito elevado e grande armazenamento de disco local. Estas VMs são criadas com a tecnologia de processadores Intel Haswell, mais concretamente os processadores E5 Xeon v3 com tamanhos de VM de 4, 8, 16 e 32 núcleos. As VMs da série Ls suportam até 6 TB de SSD local e oferecem um desempenho de entrada/saída de armazenamento sem rival.

A série de VMs Lsv2 inclui elevado débito, baixa latência e armazenamento NVMe local mapeado diretamente. As VMs Lsv2 são executadas no processador AMD EPYC™ 7551 com uma potência de todos os núcleos de 2,55 GHz até 3,0 GHz de potência de núcleo único. As VMs da série Lsv2 oferecem até 80 vCPUs numa configuração hyper-threaded, com 8 GiB de memória por vCPU e até 19,2 TB (10x1,92 TB) disponíveis diretamente para a VM.

A série de VMs Lasv3 fornece capacidades semelhantes que caracterizam as VMs Lsv2 e são baseadas no processador AMD EPYC™ 7763v (Milan) de 3.ª Geração numa configuração hyper-threaded.

Por último, a série de VMs Lsv3 fornece configurações de dimensionamento comparáveis às VMs Lasv3 e baseiam-se no processador Intel® Xeon® Platinum 8370C (Ice Lake) de 3.ª Geração numa configuração hyper-threaded.

Bases de dados de alto desempenho, aplicações que requerem elevado rendimento para o armazenamento.

### M-Series

A família da série M de máquinas virtuais do Azure está otimizada para memória e é ideal para cargas de trabalho com consumo intensivo de memória, como SAP HANA. A série M oferece até 4 TB de RAM numa única VM. Além disso, estas VMs oferecem uma contagem de CPUs virtuais de até 128 vCPUs numa única VM, para permitir o processamento paralelo de elevado desempenho.

Os exemplos de cargas de trabalho incluem o SAP HANA, SAP S/4 HANA, SQL Hekaton e outras cargas de trabalho dentro da memória de grandes dimensões críticas para a empresa que necessitam de um poder de computação paralelo massivo.

### Mv2-Series

As máquinas virtuais da série Mv2 do Azure têm hyperthreading e incluem processadores Intel® Xeon® Platinum 8180M de 2,5 GHz (Skylake), que oferecem até 416 vCPU numa única VM e oferecem configurações de memória de 3 TB, 6 TB e 12 TB. Esta é de longe a máquina virtual com a memória maior oferecida pelo Azure e oferece um desempenho computacional sem paralelo para suportar bases de dados grandes dentro da memória.

Os exemplos de cargas de trabalho incluem o SAP HANA, SAP S/4 HANA, SQL Hekaton e outras cargas de trabalho dentro da memória de grandes dimensões críticas para a empresa que necessitam de um poder de computação paralelo massivo.

### N-Series

A série N é uma família de Máquinas Virtuais do Azure com capacidades GPU. As GPUs são ideais para cargas de trabalho de computação e repletas de gráficos, ajudando os clientes a inovarem-se através de cenários como visualização remota avançada, aprendizagem aprofundada e análise preditiva.

A série N tem três ofertas distintas destinadas a cargas de trabalho específicas:

* A série NC destina-se a cargas de trabalho de computação de alto desempenho e de aprendizagem automática. A versão mais recente, NCsv3, apresenta a GPU Tesla V100 da NVIDIA.
* A série NDs destina-se a cenários de preparação e inferência para aprendizagem profunda. Utiliza as GPUs NVIDIA Tesla P40. A versão mais recente, NDv2, apresenta as GPUs NVIDIA Tesla V100.
* A série NV permite a utilização de poderosas cargas de trabalho de visualização remota e outras aplicações repletas de gráficos apoiadas pelo GPU NVIDIA Tesla M60.

As VMs NCsv3, NCsv2, NC e NDs oferecem interconectividade InfiniBand opcional para permitir o desempenho de aumento vertical.

As cargas de trabalho de exemplo incluem simulação, aprendizagem aprofundada, composição de gráficos, edição de vídeo, jogos e visualização remota.
