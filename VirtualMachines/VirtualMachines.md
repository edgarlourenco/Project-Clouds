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

**Preços Windows**
![Windows](./A-Series/Windows%20Pricing.png)

**Preços Linux**
![Linux](./A-Series//Linux%20Pricing.png)

### Bs-Series

São máquinas virtuais económicas que fornecem uma opção de baixo custo para cargas de trabalho que normalmente funcionam com uma utilização de base de CPU baixa a moderada, mas por vezes precisam de explodir para uma utilização significativamente mais elevada da CPU quando a procura aumenta. Em idle, a Bs-Series irá guardar os créditos e utilizá-los mais tarde quando a utilização da CPU precisar de ultrapassar a linha de base.  Quando reiniciada, a Bs-Series perderá os seus créditos que podem levar horas a reconstruir sem grande impacto. Quando reiniciada sem quaisquer créditos em 'banca', a Bs-Series só terá acesso para permitir uma pequena fracção da utilização total da CPU até que um banco de créditos possa ser construído.

**Preços Windows**
![Windows](./Bs-Series/Windows%20Pricing.png)

**Preços Linux**
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

### G-Series

### H-Series

### Ls-Series

### M-Series

### Mv2-Series

### N-Series
