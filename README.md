## Como utilizar nosso projeto


### 1. Clonar o Repositório

```bash
git clone git@github.com:nearform/node-clinic-doctor-examples.git

```

Este comando clona o repositório  `node-clinic-doctor-examples`  do GitHub para o seu ambiente local. Isso cria uma cópia completa do repositório, incluindo todos os arquivos e histórico de commits.

### 2. Navegar para o Diretório do Repositório

```bash
cd node-clinic-doctor-examples

```

Este comando muda o diretório atual para o diretório  `node-clinic-doctor-examples`, que foi criado ao clonar o repositório. Isso permite que você trabalhe dentro do repositório clonado.

### 3. Instalar as Dependências do Projeto

```bash
npm install

```

Este comando instala todas as dependências listadas no arquivo  `package.json`  do projeto. Essas dependências são necessárias para que os exemplos funcionem corretamente.

### 4. Instalar o  `clinic`  Globalmente

```bash
npm install -g clinic

```

Este comando instala o pacote  `clinic`  globalmente no seu sistema. O  `clinic`  é uma ferramenta de diagnóstico de desempenho para aplicações Node.js.

### 5. Instalar o  `autocannon`  Globalmente

```bash
npm install -g autocannon

```

Este comando instala o  `autocannon`  globalmente. O  `autocannon`  é uma ferramenta de benchmarking HTTP que será usada para gerar carga nas aplicações durante os testes.

## Exemplos

### Event Loop

```bash
clinic doctor --autocannon [ / ] -- node slow-event-loop

```

 Este comando executa o  `clinic doctor`  com o  `autocannon`  para testar a aplicação  `slow-event-loop`. O  `clinic doctor`  analisa o desempenho da aplicação, enquanto o  `autocannon`  gera carga HTTP.

### Garbage Collection (GC)

```bash
clinic doctor --autocannon [ -c 2500 / ] -- node slow-gc

```

Este comando é semelhante ao anterior, mas testa a aplicação  `slow-gc`, que simula problemas de coleta de lixo (Garbage Collection). O parâmetro  `-c 2500`  especifica o número de conexões simultâneas que o  `autocannon`  deve usar.

### I/O

```bash
clinic doctor --autocannon [ / ] -- node slow-io

```

Este comando testa a aplicação  `slow-io`, que simula problemas de entrada/saída (I/O). O  `clinic doctor`  ajuda a identificar gargalos de desempenho relacionados a operações de I/O.

### I/O Síncrono

```bash
clinic doctor --autocannon [ / ] -- node sync-io

```

Este comando testa a aplicação  `sync-io`, que simula problemas de I/O síncrono. O  `clinic doctor`  analisa como operações de I/O síncrono podem afetar o desempenho da aplicação.

## Licença

[Apache 2.0](<https://tldrlegal.com/license/apache-license-2.0-(apache-2.0)>)
