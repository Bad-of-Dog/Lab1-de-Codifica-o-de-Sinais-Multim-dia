# Processamento e Codificação de Sinais Multimédia

Este repositório contém o código desenvolvido para o Trabalho Prático 1 da unidade curricular de **Codificação de Sinais Multimédia**, integrada na **Licenciatura em Engenharia Informática e Multimédia** do **ISEL** (Instituto Superior de Engenharia de Lisboa) durante o 2º Semestre de 2025/2026.

## 📋 Descrição do Projeto

O objetivo deste trabalho é explorar as bases do processamento de imagem digital, compressão, difusão de erro (*dithering*) e controlo de erros em canais de transmissão ruidosos utilizando Python e a biblioteca OpenCV.

O projeto está dividido em várias etapas fundamentais:
1. **Manipulação Básica de Imagem:** Leitura, visualização e análise de propriedades estruturais (`shape` e `dtype`) com OpenCV.
2. **Compressão e Métricas de Qualidade:** Gravação de imagens em formato JPEG com diferentes níveis de qualidade (ex: 80 e 10) e cálculo da taxa de compressão, SNR (Signal-to-Noise Ratio) e PSNR (Peak Signal-to-Noise Ratio).
3. **Conversão de Espaço de Cor & Histogramas:** Transformação de imagens coloridas para tons de cinzento e análise da sua distribuição através de histogramas.
4. **Análise por Planos de Bits (Bit-Plane Slicing):** Separação e visualização individual dos 8 bits que compõem cada pixel da imagem.
5. **Dithering (Algoritmo de Floyd-Steinberg):** Implementação do algoritmo de difusão de erro para conversão fidedigna de tons de cinzento para preto e branco (binário).
6. **Simulação e Controlo de Erros em Canal Ruidoso:**
   - Simulação do efeito de um canal com probabilidade de erro (*bit flip*).
   - Implementação de técnicas de correção de erros através de **Códigos de Repetição ($R_N$)** com diferentes comprimentos ($N = 3, 5, 7, ...$).
   - Implementação de correção de erros através do **Código de Hamming $H(7,4)$** usando formulação matricial.
   - Análise estatística da taxa de erro de bit (BER) residual e discussão dos compromissos entre robustez ao ruído e taxa/razão de código.

## 🛠️ Tecnologias Utilizadas

* **Python 3**
* **OpenCV (`cv2`):** Para processamento de imagem.
* **NumPy:** Para manipulação matricial eficiente.
* **Matplotlib:** Para geração de gráficos, histogramas e exibição de múltiplos planos visuais.
* **Pillow (PIL):** Para renderização e exibição fidedigna de imagens binárias.
