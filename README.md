# 🔎 IOC-Based Threat Hunting Lab | FireEye Redline

## 📌 Visão Geral

Este projeto documenta um laboratório prático de Threat Hunting utilizando o **FireEye Redline** para investigação baseada em Indicadores de Compromisso (IOCs) em ambiente controlado Windows.

O objetivo foi simular um fluxo real de investigação SOC, aplicando coleta direcionada, validação de hashes e análise de artefatos suspeitos dentro de um diretório monitorado.

---

## 🎯 Objetivos do Laboratório

- Criar e configurar um IOC Search Collector
- Definir escopo adequado de varredura
- Executar auditoria direcionada em diretório suspeito
- Gerar sessão de análise (.mans)
- Identificar artefatos acionados por IOC
- Validar hashes MD5
- Documentar evidências encontradas

---

## 🛠 Ambiente e Ferramentas Utilizadas

- FireEye Redline
- Windows 10 (VirtualBox)
- IOC Search Collector
- Análise de Hash MD5
- Estrutura de diretório simulando ambiente comprometido

---

## 🚨 Contexto do Incidente (Simulado)

Durante monitoramento em ambiente controlado, foi identificado um diretório contendo arquivos potencialmente suspeitos (`TARGETDIRECTORY`).

Foi iniciada investigação baseada em IOC com o objetivo de:

- Detectar arquivos associados a hashes conhecidos
- Identificar artefatos maliciosos
- Confirmar presença de indicadores de comprometimento
- Documentar evidências técnicas

---

## 🔎 Metodologia de Investigação

1. Criação do IOC Search Collector
2. Definição do escopo de varredura (File Enumeration Path direcionado)
3. Execução do coletor
4. Geração da sessão de análise (.mans)
5. Abertura do IOC Report
6. Análise de:
   - Hash MD5
   - Tamanho do arquivo
   - Caminho completo
   - Metadados
7. Validação manual dos artefatos identificados

A investigação foi conduzida simulando fluxo operacional de um SOC N1.

---

## 📊 Principais Resultados

- 1 Indicador de Compromisso acionado
- Múltiplos arquivos identificados no relatório
- Executável detectado por hash malicioso
- Arquivo com tamanho específico (144557 bytes) validado
- Evidências confirmadas diretamente no IOC Report

---

## 📁 Artefatos Identificados

| Nome do Arquivo | Tamanho | Observação |
|-----------------|----------|------------|
| k3y09g3m2.exe | 81 bytes | Executável com hash associado a IOC |
| young_golden_retriever_1504846_638x426.jpg | 144557 bytes | Tamanho acionado por indicador |
| Weekly Meeting Notes.docx | 273 bytes | Arquivo relacionado a IOC específico |

---

## ⚠️ Classificação do Risco (Ambiente Simulado)

Com base na análise dos artefatos:

- Executável identificado via hash malicioso
- Evidências confirmadas no diretório monitorado
- Correspondência com indicadores previamente definidos

Classificação: **Médio a Alto Risco (ambiente controlado)**

Recomendação simulada:
- Isolamento do diretório
- Análise complementar do executável
- Validação adicional em sandbox

---

## 🎯 Possível Mapeamento MITRE ATT&CK

- Tactic: Execution
- Technique: T1204 – User Execution
- Technique: T1059 – Command and Scripting Interpreter (potencial)

---

## 🧠 Competências Demonstradas

- Investigação baseada em IOC
- Validação de hash (MD5)
- Triage de artefatos
- Interpretação de relatório forense (.mans)
- Definição de escopo de coleta
- Processo investigativo estruturado
- Mentalidade analítica aplicada a SOC

---

## 🔮 Possíveis Evoluções

- Automatizar validação de hashes via Python
- Integrar consulta em bases públicas de malware (ambiente controlado)
- Simular múltiplos IOCs em diferentes diretórios
- Expandir análise para resposta a incidente

---

## 🧾 Conclusão

Este laboratório reforçou a importância de:

- Definição correta de escopo de coleta
- Validação técnica de indicadores
- Correlação entre hash, tamanho e caminho do arquivo
- Documentação estruturada de evidências

A prática simulou um cenário real de triagem SOC, fortalecendo habilidades técnicas voltadas para detecção e análise de ameaças.

---

## 👤 Autor

José Gomes  
Estudante de Cibersegurança  
Foco em SOC | Blue Team | Threat Detection
