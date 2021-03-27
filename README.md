# VisagioHackthon: Combate a fake news
Hackthon2020: https://www.visagiotalentos.com/hackathon

Explicação dos arquivos no Github:

 1) Protótipo.7z:

Este arquivo está compactado a nossa entrega da competição. Basta descompactar a pasta zipada e rodar o arquivo FRONT.PY

PS: É necessários instalar todas as bibliotecas utilizadas antes de rodar o FRONT.PY e ter o chromedriver (disponível na pasta compactada: Protótipo) no mesmo diretório. Bibliotecas:

tensorflow
re
numpy
json
os
time
selenium
dash
dash.dependencies
dash_html_components
dash_core_components
dash_bootstrap_components
 

2) Modelo.ipynb

Este é o arquivo o qual treinamos o modelo com 256 palavras. Na pasta Protótipo.7z estão salvos 3 modelos treinados (Meu_modelo_80, Meu_modelo_160, Meu_modelo_256) e dependendo do input(texto), um modelo é carregado. A escolha do modelo é feita segundo a quantidade de palavras do input. Um input menor utilizamos o modelo que foi treinado com menos palavras (Meu_modelo_80). Vale ressaltar que, este arquivo não roda na ferramenta. Ele foi rodado paralelamente 3 vezes e os resultados de treinamento foram salvos e utilizados na FRONT.py

3)Banco_completo_utf8.csv

Banco utilizado para treinar o modelo. Este contém notícias de dois bancos de dados:

            3.1) https://github.com/roneysco/Fake.br-Corpus

            3.2)  https://chequeado.com/latamcoronavirusportugues/

 

O item 3.2 foi feito um código que acessava a página de cada notícia e selecionava o fake na íntegra. As páginas mais utilizadas foram: https://piaui.folha.uol.com.br/lupa e https://www.aosfatos.org/noticias

E como as fake são em sua maioria vinculadas pelo WhatsApp, decidimos juntar estes bancos com os tweets que possuem mais de 40 palavras que foram fornecidos no banco de dados da Visagio. Visto que, as mensagens através do aplicativo de mensagem não possuem um corpo muito grande.
