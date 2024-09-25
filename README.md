## Como utilizar nosso projeto


### 1. Clonar o Repositório

```bash
git clone git@github.com:BrenoMartinsdoEirado/Seminario-BackEnd-Otimiza-o-de-Desempenho-em-aplica-es-Node.Js--T-cnicas-e-Ferramentas.git

```

Este comando clona o repositório  `Seminario-BackEnd-Otimiza-o-de-Desempenho-em-aplica-es-Node.Js--T-cnicas-e-Ferramentas`  do GitHub para o seu ambiente local. Isso cria uma cópia completa do repositório, incluindo todos os arquivos e histórico de commits.

### 2. Navegar para o Diretório do Repositório

```bash
cd node-Seminario-BackEnd-Otimiza-o-de-Desempenho-em-aplica-es-Node.Js--T-cnicas-e-Ferramentas

```

Este comando muda o diretório atual para o diretório  `node-Seminario-BackEnd-Otimiza-o-de-Desempenho-em-aplica-es-Node.Js--T-cnicas-e-Ferramentas`, que foi criado ao clonar o repositório. Isso permite que você trabalhe dentro do repositório clonado.

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

### Como rodar o codigo

```bash
npx autocannon http://localhost:3000

```
### Para testar utilize o comando abaixo junto com a pasta onde se encontra seu arquivo .js. No exemplo abaixo o arquivo está dentro da página `slow-event-loop`
```bash
clinic doctor --on-port 'autocannon localhost:$PORT' -- node slow-event-loop

```

 

## Licença

[Apache 2.0](<https://tldrlegal.com/license/apache-license-2.0-(apache-2.0)>)
