🔎 Laboratório de Threat Hunting – Análise de IOC com FireEye Redline
📌 Visão Geral

Este projeto documenta um laboratório prático de Threat Hunting utilizando o FireEye Redline para investigação baseada em Indicadores de Compromisso (IOC) em ambiente controlado.

O objetivo foi gerar um IOC Search Collector, executar auditoria em um diretório suspeito e analisar o relatório .mans gerado para identificar artefatos maliciosos.

🛠 Ferramentas Utilizadas

FireEye Redline

Windows 10 (Ambiente Virtualizado – VirtualBox)

IOC Search Collector

Análise de Hash MD5

🎯 Cenário

Foi realizada auditoria no diretório:

TARGETDIRECTORY

Após execução do coletor, foi gerado um relatório de IOC contendo arquivos que acionaram indicadores de comprometimento.

A investigação exigiu:

Identificação de arquivos por hash MD5

Validação de tamanhos específicos

Identificação de caminhos completos

Interpretação do IOC Report

🔍 Processo de Investigação

Criação do IOC Search Collector

Execução do coletor no diretório alvo

Geração da sessão .mans

Abertura do IOC Report

Análise de:

Hash MD5

Tamanho do arquivo

Caminho completo

Metadados de criação/modificação

📊 Principais Resultados

1 Indicador de Compromisso acionado

Múltiplos arquivos analisados

Executável identificado por hash malicioso

Arquivo de tamanho específico validado

Evidências confirmadas diretamente no relatório IOC

🧠 Competências Demonstradas

Análise baseada em IOC

Validação de Hash (MD5)

Triage de artefatos

Interpretação de relatórios forenses

Processo investigativo em ambiente SOC

🚀 Objetivo

Simular fluxo real de investigação em ambiente SOC, validando indicadores e confirmando possíveis comprometimentos através de análise estruturada.

👤 Autor

José Gomes
Estudante de Cibersegurança
Foco em SOC | Blue Team | Threat Detection
