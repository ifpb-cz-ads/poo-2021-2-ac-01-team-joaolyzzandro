## 2.03 Atividade Colaborativa

## João Alfredo Alves e Lyzzandro Dualamo

---

### **1) Explique qual a função da Máquina Virtual Java (JVM)**

A JVM (Java Virtual Machine) é um software capaz de interpretar os bytecodes e executá-los independentemente de qual sistema operacional em que esteja sendo usado. A JVM permite a portabilidade do código Java porque todo código Java é compilado para um formato intermediário, o bytecode. Esse formato é então interpretado pela JVM e existem diversas JVMs, cada uma delas destinada a um tipo de sistema operacional (Windows, Linux, Mac, etc.). Dessa forma, sendo o código de uma aplicação Java transformada em bytecode e interpretada pela JVM, podemos desenvolver uma aplicação sem nos preocuparmos onde ela será executada, pois uma vez que a JVM está instalada nossa aplicação irá executar sem nenhum envolvimento com o sistema operacional.

---

### **2) Qual a diferença entre JRE e JDK?**

O JRE (Java Runtime Environment) é um ambiente de execução Java. Ele fornece uma JVM, pacotes básicos Java e todos os outros requisitos para executar um programa Java.

Já o JDK (Java Development Kit) é um um Kit de desenvolvimento Java, que fornece aos desenvolvedores Java, ferramentas para o desenvolvimento de um programa. Ele contém um compilador, um depurador e o próprio JRE para a execução de programas.

---

### **3) Crie um programa Java que imprima o seguinte texto “Terminei a primeira aula com um programa Java!”.**

_O arquivo do programa criado está dentro desta pasta com o nome **ProgramaQ3.java**_

```
class ProgramaQ3 {
	public static void main(String[] args) {
		System.out.println(“Terminei a primeira aula com um programa Java!”);
	}
}
```

---

### **4) Compile o programa desenvolvido no exercício anterior. A seguir apague o arquivo .class gerado e tente executar o programa. O que aconteceu?**

Vai gerar um erro, já que o .class é o bytecode que a JVM usa para executar o programa.

---

### **5) Mude o nome do método “main” para “start”, compile e execute. O que aconteceu?**

O programa não foi compilado com sucesso, pois o main é o método que inicia as aplicações Java e quando solicitamos ao interpretador que execute uma determinada classe compilada, ele procura o método main e se esse método não existir, irá ser gerada uma exceção informando que o método não foi localizado.

- O erro apresentado foi:

     _Error: Main method not found in class Main, please define the main method as: public static void main(String[] args)_

---
