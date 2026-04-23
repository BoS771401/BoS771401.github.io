---
title: "opdracht 2 vrije ruimte"
author: "Bo Steinschuld"
date: "2026-04-23"
output: html_document
---

# Vrije opdracht

## Introductie

Voor mijn vrije opdracht kies ik ervoor om een nieuwe Data Science for Biology skill te leren die aansluit bij mijn toekomstige stage en mijn interesse in AI‑gestuurde bioinformatica workflows. Ik ga mij verdiepen in het bouwen van een doorzoekbare bioinformatica tool registry voor RNA‑seq workflows, gecombineerd met een deep dive in Model Context Protocol (MCP) en de AI‑frameworks LangChain en LangGraph.

Het doel is om te begrijpen hoe moderne AI‑agents tools kunnen aanroepen, workflows kunnen structureren en beslissingen kunnen nemen op basis van context. Door een registry te koppelen aan MCP en vervolgens te gebruiken binnen LangChain/LangGraph, kan ik een fundament leggen voor een intelligente RNA‑seq workflow die automatisch de juiste tools selecteert op basis van input, metadata en workflow‑stappen.

Deze skill sluit direct aan op mijn toekomstplan: tijdens mijn stage ga ik werken aan het automatiseren van RNA‑seq analyses. Door nu al te leren hoe tool‑registries, metadata‑structuren en AI‑workflow‑systemen werken, kan ik beter voorbereid starten en sneller waarde toevoegen.



## Doel van de opdracht

- Een tool registry opzetten met metadata over RNA‑seq tools (bijv. FastQC, STAR, Salmon, DESeq2).  
- Begrijpen hoe Model Context Protocol (MCP) werkt om tools toegankelijk te maken voor AI‑agents.  
- Leren hoe LangChain reasoning‑ketens bouwt die tools kunnen aanroepen.  
- Leren hoe LangGraph workflows structureert als grafen met nodes en edges.  
- Een conceptuele koppeling maken tussen registry → MCP → LangChain → LangGraph → RNA‑seq workflow.

De daadwerkelijke uitwerking volgt later; deze fase richt zich op oriëntatie en planning.



## Planning (32 uur)

### Fase 1: Oriëntatie en literatuur (6 uur; 4 mei 2026)
Doelen:
- begrijpen wat MCP is en hoe het tools beschikbaar maakt  
- basisconcepten van LangChain en LangGraph leren  
- voorbeelden van bioinformatica registries bestuderen (Bioconda, BioContainers, Bioconductor)

Activiteiten:
- documentatie lezen van MCP, LangChain en LangGraph  
- RNA‑seq tools inventariseren  
- bepalen welke metadata nodig is voor een registry  



### Fase 2: Opzetten van een basis registry (8 uur; 7 mei 2026)
Doelen:
- dataset maken met RNA‑seq tools en metadata  
- registry opslaan in CSV of JSON  
- nadenken over hoe MCP deze tools kan “exposen” aan een AI‑agent

Activiteiten:
- minimaal 15 tools verzamelen  
- metadata toevoegen (functie, inputtype, outputtype, installatie, workflow‑stap)  
- eerste versie van registry opslaan  



### Fase 3: Integratieconcept met MCP + LangChain (8 uur; 10 mei 2026)
Doelen:
- begrijpen hoe een AI‑agent tools kan aanroepen via MCP  
- prototype‑scripts schrijven die registry‑items kunnen worden opgevraagd  
- eenvoudige zoekfunctie bouwen in R of Python

Activiteiten:
- MCP‑voorbeeldprojecten bestuderen  
- simpele tool‑call structuur opzetten  
- zoekfunctie bouwen (bijv. “geef alle tools die FASTQ als input gebruiken”)  



### Fase 4: Workflow‑structuur met LangGraph (6 uur; 11 mei 2026)
Doelen:
- begrijpen hoe LangGraph workflows moduleert  
- schets maken van een RNA‑seq workflow als graph  
- registry koppelen aan workflow‑stappen

Activiteiten:
- nodes definiëren (QC → alignment → quantification → DGE)  
- registry‑tools koppelen aan nodes  
- mini‑prototype van een graph workflow  



### Fase 5: Rapportage en afronding (4 uur; 21 mei 2026)
Doelen:
- documenteren wat ik geleerd heb  
- reflecteren op de skill  
- voorbereiden op de uiteindelijke uitwerking

Activiteiten:
- RMarkdown‑verslag schrijven  
- planning + motivatie afronden  
- ideeën noteren voor de uiteindelijke code‑uitwerking  



## Eindproduct 

Zal bestaan uit:

- een registry dataset (CSV/JSON)  
- een zoekfunctie  
- een MCP‑compatible toolstructuur  
- een LangChain/LangGraph workflowconcept  
- een reflectieverslag  
