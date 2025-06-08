# Desafio POO - Modelando um iPhone com Java

Projeto desenvolvido para o Desafio de Programação Orientada a Objetos do bootcamp de Java da DIO. O objetivo foi modelar e implementar as funcionalidades de um iPhone, aplicando conceitos de Abstração, Encapsulação, Polimorfismo e o uso de Interfaces.

---

## Diagrama de classe 

```mermaid
classDiagram
    class ReprodutorMusical {
        +tocar(): void
        +pausar(): void
        +selecionarMusica(musica: String): void
    }

    class AparelhoTelefonico {
        +ligar(numero: String): void
        +atender(): void
        +iniciarCorreioVoz(): void
    }

    class NavegadorInternet {
        +exibirPagina(url: String): void
        +adicionarNovaAba(): void
        +atualizarPagina(): void
    }

    class iPhone {
          + musica: String
          + url: String
          + numero String
    }

    iPhone ..|> ReprodutorMusical
    iPhone ..|> AparelhoTelefonico
    iPhone ..|> NavegadorInternet
```
