# 01798/2024 – Mentor de Projetos e Pesquisa

Problema: 
Os equipamentos elétricos utilizados na transmissão e distribuição de energia falham principalmente devido a problemas de isolamento e isso ocorre devido a fraquezas, defeitos, impurezas e degradação do isolamento. Estudos anteriores revelaram que fraquezas ou defeitos no isolamento muitas vezes causam descargas elétricas
localizadas que conectam parcialmente o isolamento entre os condutores, um fenômeno conhecido como Descarga Parcial (PD). Como a PD é um fenômeno comum, sua análise provou ser uma ferramenta eficaz para monitorar a condição de diversos equipamentos elétricos. Além disso, a ocorrência sucessiva de PDs enfraquece gradualmente o isolamento, levando potencialmente ao colapso total do sistema.
Durante descargas parciais, a tensão do campo elétrico excede a constante de ruptura dielétrica local no meio isolante, liberando energia em diversas formas, como ondas acústicas, ondas eletromagnéticas na banda de Ultra Alta Frequência (UHF), banda de frequência óptica e calor. Vários estudos propuseram diferentes técnicas de medição de DP medindo qualquer uma ou uma combinação das várias formas de energia liberada.
Devido a dificuldade de acessos a esses equipamentos de alta tensão, abordagens utilizando algoritmos de inteligência artificial, tem se mostrado promissores. Você como Mentor de Projetos e Pesquisa em Inteligência Artificial, foi acionado para desenvolver um projeto envolvendo descargas parciais em unidades geradoras de energia elétrica.

Solução proposta: 
Algoritmo de classificação das descargas parciais registradas em categorias de descargas e monitoramento da fase, amplitude e número de descargas por evento, através de médias móveis.

Justificativa: 
O banco de dados conta com datas em formatos irregulares, o que impede uma abordagem completa que incorpore o tratamento das séries temporais sem, antes, diagnosticar a causa da inconsistência nos registros. Há registros como “31 de setembro”, um mês que possui apenas 30 dias, e registros do tipo “jan-2111”. Embora o primeiro caso possa ser resolvido ,corrigindo as datas desde a primeira inconsistência, sem ter conhecimento de quando foi, realmente, o primeiro evento, não é possível assumir que a menor data represente, de fato, aquele dia. 
Para contornar esta dificuldade, a média móvel será calculada não em função dos dias, mas em função dos eventos. Isto é, a janela para a média de cada uma das três métricas será de n eventos, em vez de n dias.

A figura abaixo apresenta o número de descargas parciais por evento, separadas por categoria de discarga. De modo geral, parece haver um crescimento no número de descargas por evento. Para algumas categorias, esse aumento é mais acentuado.  
![Número de Descargas Parciais por Evento](https://github.com/inacio-puntel/mentor_projetos_pesquisa/blob/main/nxevento.png)
![Número de Desgargas Parciais por Evento - Geral](https://github.com/inacio-puntel/mentor_projetos_pesquisa/blob/main/nxeventogeral.png)




