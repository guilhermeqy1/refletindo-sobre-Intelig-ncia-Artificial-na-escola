<!DOCTYPE html>
<html lang="pt-br">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Você decide o futuro da IA</title>
    <style>
        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
        }

        body {
            font-family: 'Segoe UI', Arial, sans-serif;
            background: #0a0a0f;
            color: #fff;
            display: flex;
            justify-content: center;
            align-items: center;
            min-height: 100vh;
            padding: 20px;
        }

        .caixa-principal {
            background: #0d0d1a;
            padding: 50px 40px;
            border-radius: 16px;
            max-width: 700px;
            width: 100%;
            text-align: center;
            box-shadow: 0 0 40px rgba(0, 200, 255, 0.15);
        }

        h1 {
            font-size: 2.8rem;
            font-weight: 700;
            color: #00e5ff;
            line-height: 1.1;
            margin-bottom: 30px;
            text-shadow:
                0 0 10px #00e5ff,
                0 0 20px #00e5ff,
                0 0 40px #00b3cc;
            letter-spacing: 1px;
        }

        .tela-inicial p {
            font-size: 1.15rem;
            line-height: 1.7;
            color: #e0e0e0;
            margin-bottom: 40px;
            text-align: center;
        }

        .iniciar-btn,
        .novamente-btn,
        .caixa-alternativas button {
            background: #1c1c2e;
            color: #e0e0e0;
            border: 1px solid #2e2e44;
            padding: 14px 50px;
            border-radius: 999px;
            font-size: 1.1rem;
            cursor: pointer;
            transition: all 0.3s ease;
            box-shadow: 0 4px 15px rgba(0, 0, 0, 0.4);
        }

        .iniciar-btn:hover,
        .novamente-btn:hover,
        .caixa-alternativas button:hover {
            background: #00e5ff;
            color: #0a0a0f;
            box-shadow: 0 0 25px rgba(0, 229, 255, 0.8);
            transform: translateY(-2px);
        }

        .caixa-alternativas button {
            display: block;
            width: 100%;
            text-align: left;
            margin: 10px 0;
            padding: 14px 25px;
            font-size: 1rem;
        }

        .novamente-btn {
            margin-top: 15px;
        }

        .caixa-perguntas,
        .caixa-alternativas,
        .caixa-resultado {
            display: none;
        }

        .caixa-perguntas.mostrar,
        .caixa-alternativas.mostrar,
        .caixa-resultado.mostrar {
            display: block;
        }

        .caixa-perguntas {
            font-size: 1.3rem;
            margin-bottom: 20px;
            color: #00e5ff;
        }

        .texto-resultado {
            font-size: 1.1rem;
            line-height: 1.7;
            color: #e0e0e0;
        }
    </style>
</head>
<body>
    <div class="caixa-principal">
        <h1>Você decide o<br>futuro da IA</h1>

        <!-- TELA INICIAL -->
        <div class="tela-inicial">
            <p>
                Novembro de 2022, a humanidade se viu em uma realidade perturbadora.
                De repente, percebemos que as máquinas evoluíram para além do que imaginávamos.
                Agora, elas escrevem e falam de um jeito tão parecido com humanos que é quase impossível diferenciar quem foi que escreveu ou falou o que.
                Em meio a esse caos de identidade, uma missão surgiu.
                Nosso objetivo: explorar o impacto da Inteligência Artificial (IA) em nossas vidas e confrontar as possibilidades que o futuro nos reserva.
                O mundo nunca mais será o mesmo.
            </p>
            <button class="iniciar-btn">Iniciar</button>
        </div>

        <!-- CAIXAS DO JOGO -->
        <div class="caixa-perguntas"></div>
        <div class="caixa-alternativas"></div>

        <div class="caixa-resultado">
            <p class="texto-resultado"></p>
            <button class="novamente-btn">Jogar novamente</button>
        </div>
    </div>

    <script>
        // ===== PERGUNTAS =====
        const perguntas = [
            {
                enunciado: "Qual é o impacto da IA na sociedade?",
                alternativas: [
                    { texto: "Positivo", afirmacao: "Você acredita que a IA pode melhorar a vida das pessoas." },
                    { texto: "Negativo", afirmacao: "Você teme que a IA possa causar danos à sociedade." }
                ]
            },
            {
                enunciado: "Você confiaria em uma IA para tomar decisões importantes?",
                alternativas: [
                    { texto: "Sim", afirmacao: "Você confia na capacidade da IA." },
                    { texto: "Não", afirmacao: "Você prefere que humanos tomem decisões críticas." }
                ]
            },
            {
                enunciado: "Como você vê o futuro da IA?",
                alternativas: [
                    { texto: "Promissor", afirmacao: "Você está otimista com o futuro da IA." },
                    { texto: "Preocupante", afirmacao: "Você está preocupado com o rumo da IA." }
                ]
            }
        ];

        // ===== SELEÇÃO DE ELEMENTOS =====
        const caixaPerguntas = document.querySelector(".caixa-perguntas");
        const caixaAlternativas = document.querySelector(".caixa-alternativas");
        const caixaResultado = document.querySelector(".caixa-resultado");
        const textoResultado = document.querySelector(".texto-resultado");
        const botaoJogarNovamente = document.querySelector(".novamente-btn");
        const botaoIniciar = document.querySelector(".iniciar-btn");
        const telaInicial = document.querySelector(".tela-inicial");

        // ===== VARIÁVEIS DE ESTADO =====
        let atual = 0;
        let perguntaAtual;
        let historiaFinal = "";

        // ===== BOTÃO INICIAR =====
        botaoIniciar.addEventListener("click", iniciaJogo);

        function iniciaJogo() {
            atual = 0;
            historiaFinal = "";
            telaInicial.style.display = "none";

            caixaPerguntas.classList.remove("mostrar");
            caixaAlternativas.classList.remove("mostrar");
            caixaResultado.classList.remove("mostrar");

            mostraPergunta();
        }

        // ===== MOSTRA PERGUNTA =====
        function mostraPergunta() {
            if (atual >= perguntas.length) {
                mostraResultado();
                return;
            }

            perguntaAtual = perguntas[atual];
            caixaPerguntas.textContent = perguntaAtual.enunciado;
            caixaAlternativas.textContent = "";
            mostraAlternativas();

            caixaPerguntas.classList.add("mostrar");
            caixaAlternativas.classList.add("mostrar");
        }

        // ===== MOSTRA ALTERNATIVAS =====
        function mostraAlternativas() {
            for (const alternativa of perguntaAtual.alternativas) {
                const botaoAlternativa = document.createElement("button");
                botaoAlternativa.textContent = alternativa.texto;
                botaoAlternativa.addEventListener("click", () =>
                    respostaSelecionada(alternativa)
                );
                caixaAlternativas.appendChild(botaoAlternativa);
            }
        }

        // ===== PROCESSA RESPOSTA =====
        function respostaSelecionada(opcaoSelecionada) {
            historiaFinal += opcaoSelecionada.afirmacao + " ";
            atual++;
            mostraPergunta();
        }

        // ===== MOSTRA RESULTADO =====
        function mostraResultado() {
            caixaPerguntas.classList.remove("mostrar");
            caixaAlternativas.classList.remove("mostrar");
            caixaResultado.classList.add("mostrar");
            textoResultado.textContent = historiaFinal;
        }

        // ===== JOGAR NOVAMENTE =====
        botaoJogarNovamente.addEventListener("click", reiniciaJogo);

        function reiniciaJogo() {
            atual = 0;
            historiaFinal = "";
            caixaResultado.classList.remove("mostrar");
            telaInicial.style.display = "block";
        }
    </script>
</body>
</html>
