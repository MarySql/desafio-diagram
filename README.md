## Desafio diagramação de classes do iphone

```mermaid
classDiagram
    class iPhone {
        +reprodutorMusical: ReprodutorMusical
        +aparelhoTelefonico: AparelhoTelefonico
        +navegadorInternet: NavegadorInternet
    }
    class ReprodutorMusical {
        <<interface>>
        +tocar()
        +pausar()
        +selecionarMusica(String musica)
    }
    class AparelhoTelefonico {
        <<interface>>
        +ligar(String numero)
        +atender()
        +iniciarCorreioVoz()
    }
    class NavegadorInternet {
        <<interface>>
        +exibirPagina(String url)
        +adicionarNovaAba()
        +atualizarPagina()
    }
    iPhone --|> ReprodutorMusical
    iPhone --|> AparelhoTelefonico
    iPhone --|> NavegadorInternet
