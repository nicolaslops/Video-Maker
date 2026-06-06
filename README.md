# VIDEO-MAKER

## Sobre o Projeto

Este projeto consiste em um script de automação e manipulação de mídia focado na criação procedural de arquivos de vídeo a partir de sequências estáticas. Desenvolvido em Python, o script `CreateVideo.py` acessa automaticamente o diretório de imagens do sistema operacional, faz a leitura dos arquivos visuais disponíveis e os compila de forma sequencial para gerar um arquivo de vídeo contínuo.

O grande diferencial da lógica deste programa está no tratamento da linha do tempo: ele inverte a ordem natural de leitura dos arquivos. Dessa forma, a última imagem salva na pasta torna-se o primeiro frame a aparecer na tela, criando um efeito reverso e juntando todas as mídias da pasta em uma composição fluida de transição temporal.

---

## Funcionalidades

* Integração e leitura automatizada da pasta de imagens nativa do sistema operacional.
* Algoritmo de ordenação reversa que estrutura os elementos visuais de trás para frente.
* Processamento e junção de imagens em lote de maneira sequencial.
* Renderização e exportação direta do compilado final em formato de vídeo estável.

---

## Tecnologias Utilizadas

* **Python 3**
* Biblioteca principal: `OpenCV` (representada no código pelo módulo importável `cv2`)
* Bibliotecas nativas auxiliares: `os`

---

## Objetivo

O principal objetivo deste projeto é explorar o tratamento de matrizes de imagens e fluxos de mídia digital utilizando a biblioteca de visão computacional OpenCV. O foco técnico está em compreender os parâmetros de codificação de vídeo, como a definição de codecs (ex: FourCC), taxas de quadros por segundo (FPS) e dimensões de resolução, além da correta manipulação de caminhos do sistema para agrupamento e leitura lógica de arquivos.

---

## Aprendizados

Durante o desenvolvimento deste projeto, foram aplicados conceitos como:

* Utilização da biblioteca `os` para mapear de forma multiplataforma o caminho absoluto da pasta de imagens do usuário.
* Uso de técnicas de manipulação de listas em Python (fatiamento ou métodos de reversão) para inverter a ordem cronológica de leitura dos arquivos locais.
* Manipulação do objeto `cv2.VideoWriter` do OpenCV para configurar as propriedades estruturais e escrever os frames sequenciais no contêiner de vídeo.
* Gerenciamento de memória e I/O de mídia, aplicando métodos adequados de fechamento e liberação de arquivos (`video.release()`) após a conclusão do processo de renderização.

---

## Como Executar

1. Certifique-se de ter o Python instalado em sua máquina.
2. Instale a dependência do OpenCV através do terminal:
```bash
pip install opencv-python
```

3. Acesse a pasta do projeto:

```bash
cd VIDEO-MAKER
```

4. Execute o script principal para gerar o seu vídeo:

```bash
python CreateVideo.py
```

--- 

## Estrutura do Projeto
```text
VIDEO-MAKER/
│
├── CreateVideo.py
└── README.md
```

--- 

## Licença
Este projeto foi desenvolvido exclusivamente para fins educacionais e de aprendizado.

Desenvolvido como prática de automação multimídia e visão computacional com Python, combinando manipulação estruturada de arquivos do sistema operacional e compilação de vídeo reverso utilizando OpenCV (cv2).
