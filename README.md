# robotframework-linux
Tutorial: Configurando um Ambiente Virtual e Instalando o Robot Framework no Linux


# Instalação do Robot Framework Linux

### **Passo 1: Verifique a Instalação do Python e Pip**

Certifique-se de ter o Python 3.x e o pip instalados no seu sistema. Verifique as versões com os comandos:

```bash
bashCopy 

code
python3 --version
pip3 --version

sudo apt install python3-pip

sudo apt install python3

```

### **Passo 2: Criar um Ambiente Virtual**

Abra o terminal e navegue para a pasta onde deseja criar o ambiente virtual:

```bash
bashCopy code
cd caminho/para/sua/pasta
```

Crie um ambiente virtual chamado "robot-env":

```bash
bashCopy code
python3 -m venv robot-env

```

### **Passo 3: Ativar o Ambiente Virtual**

Ative o ambiente virtual para isolar suas instalações Python:

```bash
bashCopy code
source robot-env/bin/activate
```

Você verá o nome do ambiente no prompt, indicando que você está dentro do ambiente virtual.

### **Passo 4: Instalar o Robot Framework e Bibliotecas Adicionais**

Dentro do ambiente virtual, instale o Robot Framework e bibliotecas adicionais (se necessário):

```bash
bashCopy code
pip install robotframework
pip install robotframework-seleniumlibrary  # Exemplo de biblioteca adicional
pip install --upgrade RESTinstance
```

### **Passo 5: Criar e Executar Testes do Robot Framework**

Agora você pode criar e executar seus testes do Robot Framework dentro deste ambiente virtual. Crie um arquivo de teste **`meu_teste.robot`**:

```
robotCopy code
*** Settings ***
Documentation  Exemplo de teste Robot Framework

*** Test Cases ***
Meu Primeiro Teste
    Log  Olá, Mundo!
```

Execute o teste usando o comando **`robot`**:

```bash
bashCopy code
robot meu_teste.robot
```

### **Passo 6: Desativar o Ambiente Virtual**

Quando terminar, saia do ambiente virtual:

```bash
bashCopy code
deactivate
```

### **Conclusão**

Ao seguir este tutorial, você aprendeu a criar e gerenciar ambientes virtuais no Linux usando o Python **`venv`**. Isso permite que você isole seus projetos e instalações Python, tornando mais fácil gerenciar pacotes e dependências específicos para cada projeto. Além disso, você instalou o Robot Framework em um ambiente virtual e criou um teste simples para demonstração.

Lembre-se de ativar o ambiente virtual sempre que estiver trabalhando em um projeto específico e desativá-lo quando terminar. Isso ajudará a manter suas instalações Python organizadas e evitar conflitos de pacotes entre diferentes projetos.
