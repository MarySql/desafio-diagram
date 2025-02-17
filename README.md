```mermaid
classDiagram
    class iPhone {
        +reprodutorMusical: ReprodutorMusical
        +aparelhoTelefonico: AparelhoTelefonico
        +navegadorInternet: NavegadorInternet
    }
    interface ReprodutorMusical {
        +tocar()
        +pausar()
        +selecionarMusica(String musica)
    }
    interface AparelhoTelefonico {
        +ligar(String numero)
        +atender()
        +iniciarCorreioVoz()
    }
    interface NavegadorInternet {
        +exibirPagina(String url)
        +adicionarNovaAba()
        +atualizarPagina()
    }
    iPhone ..> ReprodutorMusical
    iPhone ..> AparelhoTelefonico
    iPhone ..> NavegadorInternet
