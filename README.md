

# AWS | EC2 



Repositório organizado contendo anotações e insights adquiridos durante a prática. Com o tema "Gerenciamento de instâncias EC2 na AWS". Desafio do curso [DIO - Santander Code Girls - 2025](https://web.dio.me/track/santander-code-girls-2025).



## Elastic Compute Cloud - EC2 

- [Documentação AWS - O que é a Amazon EC2?](https://docs.aws.amazon.com/pt_br/AWSEC2/latest/UserGuide/concepts.html)

A Amazon EC2, oferece a plataforma de computação mais ampla e profunda. Com mais de 750 instâncias e opções de processamento, armazenamento, redes, sistemas operacionais, e outros. No modelo Cloud, uma EC2 é um tipo IaaS.

A Amazon EC2, fornece os seguintes recursos:
- Instâncias: servidores virtuais;
- AMIs (Amazon Machine Images): modelos pré-configurados para instâncias;
- Tipos de instâncias;
- Volumes do Amazon EBS: volumes de armazenamento persistentes para seus dados usando EBS;
- Volumes de Armazenamento de Instâncias: Volumes de armazenamento para dados temporários;
- Pares de Chaves: Projeta informações de login de suas instâncias;
- Grupos de Segurança: um firewall da Amazon.

## Instâncias 
Uma instâncias do EC2 é um serviço virtual na nuvem AWS. O tipo de instância que você especifica determina o hardware disponível para a sua instância.  
Escolher a instância correta na AWS é crucial para garantir eficiência, estabilidade e econimia nos gastos com a nuvem. E para isso, precisamos entender as necessidades de sua aplicação.  
Cada tipo de instância oferece diferentes recursos de computação.

Instance Types:
- General Purpose: A1, T4g, T3, ...
- Compute Optmized: C6g, C5, C5a, ...
- Memory Optmized: R6g, R5, R5a, ...
- Storage Optmized: I3, I3en, D2, ...
- Accelerated Computing: P3, P2,...  

É possivel adicionar capacidade (aumentar a escala verticalmente), dependendo da demanda. Como também é possivel diminuir a capacidade.

## Otimizando Recursos na AWS

- Desligando instâncias não utilizadas;
- Removendo recursos ociosos ou não utilizados;
- Escalando recursos (Horizontalmente ou Verticalmente)

## Gerenciamento de Instâncias EC2
- [Documentação AWS - Gerenciando EC2 instâncias da Amazon](https://docs.aws.amazon.com/pt_br/toolkit-for-visual-studio/latest/user-guide/tkv-ec2-ami.html)

### Criação e uso de imagem AMI (Amazon Machine Image)
No Amazon EC2, uma AMI é uma imagem de máquina virtual pré-configurada, que inclui as informações necessárias para iniciar uma instância.  

AMIs: 
- As AMIs podem ser criadas a partir de instâncias paradas ou em execução. Permitindo capturar uma instância do seu ambiente configurado.
- Temos AMIs que são públicas ou privadas.
- É possivel personalizar uma instância e criar uma AMI a partir dessa instância. Facilitando a replicação do seu ambiente.
- Para executar instâncias no EC2, seleciona uma AMI, que irá fornecer as informações necessárias para iniciar a instância.
- Existem diferentes tipos de AMIs

### Snapshots EBS (Elastic Block Store)
É um serviço de backup nativo da AWS que faz backup dos volumes do EBS. Sendo possivel configurar a frequencia com que são feitos os backup.

No Amazon EC2, uma imagem de máquina da Amazon (AMI) faz o backup de um servidor interno, incluindo todos os volumes EBS anexadas. Já o Snapshot é uma cópia pontual de um determinado volume, armazenadas na Amazon A3.

## Referências
- [Documentação AWS - Gerenciando EC2 instâncias da Amazon](https://docs.aws.amazon.com/pt_br/toolkit-for-visual-studio/latest/user-guide/tkv-ec2-ami.html)
- [Documentação AWS - O que é a Amazon EC2?](https://docs.aws.amazon.com/pt_br/AWSEC2/latest/UserGuide/concepts.html)
- [Aulas do Curso da DIO - Santander Code Girls](https://web.dio.me/track/santander-code-girls-2025) 
