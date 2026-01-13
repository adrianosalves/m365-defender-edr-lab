
**Stack**: Microsoft Defender for Endpoint  
**SO**: MACOS (Lab)  
**Política aplicada**: [Ex.: ASR Rules, Tamper Protection ON]

![Detecção da macro maliciosa](https://raw.githubusercontent.com/adrianosalves/m365-defender-edr-lab/main/case-01-macro-malicioso/screenshots/detection01.png)

![Detecção da macro maliciosa](https://github.com/adrianosalves/m365-defender-edr-lab/blob/main/case-01-macro-malicioso/screenshots/detection02.png)

O arquivo exela_irestore do ReiBoot foi provavelmente marcado como falso positivo pelo antivírus, pois o programa usa métodos de baixo nível para reparar dispositivos iOS — técnicas que se assemelham a exploits reais (como o LimeRain). O usuário instalou o ReiBoot do site oficial, o risco é baixo, mas, como é um software não notarizado pela Apple, ainda representa uma possível vulnerabilidade. Se não está usando, remova-o para manter o sistema mais seguro e evitar alertas.

---

## 1) Detecção
- Alerta: LimeRain' exploit malware was detected
- Severidade: Low
- Origem: /Applications/ReiBoot.app/Contents/Frameworks/ToolsFrameworks/exela_irestore

  

---

## 2) Evidências
- Árvore de processos: N/A
- IOC genérico (
-   hash: 69199a5c3f2efe80b95646eb8af019fb90fe2c96,
-   comando: N/A,
-   URL: N/A)

---

## 3) Ações
- Isolamento do endpoint: N/A
- Bloqueio de hash: N/A
- Quarentena do arquivo: N/A

---

## 4) Lições aprendidas
- Ajustes de política: N/A
- Recomendações para prevenção: N/A











