# quiz-biblico
App Quiz Bíblico para Lives.
Localização,Potencial Erro/Melhoria,Ação Necessária
Tags de Imagem,As imagens da logo e do QR Code (logo-mz.png e qrcode-pix.png) estão com nomes genéricos.,"Ação: Certifique-se de que os arquivos de imagem que você colocar na pasta tenham exatamente esses nomes, ou ajuste o HTML para os nomes reais dos seus arquivos."
Rodapé PIX,O rodapé (credits-footer) está dentro do quiz-container.,"Melhoria: Para o formato vertical de lives, esse rodapé pode ocupar muito espaço na tela. Sugiro colocá-lo fora do quiz-container se você quiser um layout menor e mais focado no jogo. Vamos mantê-lo assim por enquanto, mas fique atento ao tamanho em lives."
Localização,Potencial Erro/Melhoria,Ação Necessária
Formato Vertical,O código usa max-width: 450px e max-height: 900px (relação 9:16).,"Verificação: Durante o uso no OBS/Streamlabs, defina as dimensões da ""Fonte do Navegador"" exatamente para essa proporção (ex: 450 x 800) para garantir o melhor encaixe no formato vertical."
Cores,As cores são genéricas (var(--color-primary): #FFD700;).,"Ação Crítica: Você deve substituir os valores hexadecimais (#FFD700, #0077B6, etc.) no bloco :root no início do style.css pelas cores exatas da logo da Web Rádio MZ para personalização."
Localização,Potencial Erro/Melhoria,Ação Necessária
Seleção de Perguntas,"A função getProximaPergunta seleciona perguntas de forma totalmente aleatória, sem priorizar os níveis (Fácil, Médio, Difícil) em ordem.","Melhoria: Para um quiz com progressão tipo ""Jogo do Milhão"", o ideal seria forçar, por exemplo: 3 fáceis, 3 médias, 3 difíceis. A lógica atual garante que nunca repete, o que é ótimo, mas não força a progressão de dificuldade."
Bônus Cálculo,"O cálculo do bônus (calcularBonus) funciona corretamente, dando mais pontos para respostas rápidas.","Verificação: O sistema usa: PONTOS_BONUS_MAX = 5 (rápido) e PONTOS_BONUS_MIN = 3 (lento). Se você quer bônus entre 3 e 5 pontos, isso está correto."
