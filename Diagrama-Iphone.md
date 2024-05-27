```mermaid
classDiagram
    class ReprodutorMusical {
        <<interface>>
        +tocar()void*
        +pausar()void*
        +selecionarMusica(String musicaEscolhida)void*
    }

    class AparelhoTelefonico {
        <<interface>>
        +ligar(String numero)void*
        +atender()void*
        +iniciarCorreioVoz()void*
    }

    class NavegadorInternet {
        <<interface>>
        +exibirPagina(String url)void*
        +adicionarNovaAba()void*
        +atualizarPagina()void*
    }

    class IPhone {
        List~string~ musica
        int musica
        +ligar(String numero)void
        +atender()void
        +iniciarCorreioVoz()void
        +exibirPagina(String url)void
        +adicionarNovaAba()void
        +atualizarPagina()void
        +tocar()void
        +pausar()void
        +selecionarMusica(String musicaEscolhida)void
    }
    class Usuario{
    }

    IPhone --> ReprodutorMusical
    IPhone --> AparelhoTelefonico
    IPhone --> NavegadorInternet
    Usuario --o IPhone : Aggregation
    
```
