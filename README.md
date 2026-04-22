# Entorns_VIBE_CODING
# 🧙‍♂️ README: Microjoc RPG (Màgia i Captura)

> **Document de presentació del projecte (README)** elaborat per a la fase inicial de desenvolupament. Aquest projecte és un RPG tàctic per torns desenvolupat a **Roblox Studio**.

---

## 📋 Índex
1. [Visió General](#1-visió-general)
2. [Jugabilitat i Regles](#2-jugabilitat-i-regles)
3. [Abast i Límits del Projecte](#3-abast-i-límits-del-projecte)
4. [Riscos i Viabilitat](#4-riscos-i-viabilitat)
5. [Planificació i Eines](#5-planificació-i-eines)

---

## 1. Visió General

### 🎯 Tipus de microvideojoc
Joc de combat tàctic per torns amb col·leccionisme lleuger i estructura lineal (Boss Rush / Seqüencial).

### 💡 Definició de la idea
Ets un jove mag que avança per una història lineal superant combats. Hi ha dos tipus d'enfrontaments:
* **Mini-batalles:** Contra criatures màgiques. En derrotar-les, pots "capturar-les" perquè s'uneixin al teu equip (màxim 1 criatura invocada alhora).
* **Batalles de Cap (Bosses):** Enemics més poderosos lligats a la història que **no** es poden capturar.

### 🏆 Objectiu del joc
Superar la seqüència completa de la història, gestionant estratègicament els atacs del teu mag i reclutant la criatura adequada en les mini-batalles prèvies per poder derrotar els Caps.

---

## 2. Jugabilitat i Regles

### 🎮 Rol del jugador
El jugador controla el seu **Mag principal** i la seva **Criatura aliada** (si en té una). A cada torn, mitjançant la interfície gràfica (GUI), decidirà quins atacs o curacions utilitzar. En finalitzar una mini-batalla amb èxit, prendrà la decisió de si vol reclutar la criatura vençuda (substituint l'anterior).

### ⚖️ Regles i Condicions
* **Sistema de Torns:** Combat per torns estrictes. Si tens una criatura, tant el mag com la criatura actuen en el mateix torn abans que l'enemic.
* **Immunitat:** Els Caps Finals són immunes a la captura.
* **Condició de Victòria:** Reduir a `0` la vida (HP) de l'enemic per avançar.
* **Condició de Derrota:** La vida del teu Mag principal arriba a `0` (independentment de si la teva criatura continua viva).

### 🔄 Bucle Principal (Core Loop)
1. Lectura d'un fragment d'història.
2. Inici d'una **mini-batalla** contra una criatura.
3. Decisió de captura en guanyar.
4. Avanç de la història.
5. Inici de la **batalla contra el Cap** (Boss).
6. Es repeteix el cicle o s'acaba el joc.

---

## 3. Abast i Límits del Projecte

### 🧠 Repte principal i Dificultat
El repte recau en la **planificació tàctica**: el jugador haurà de deduir quina criatura reclutar en les mini-batalles per tenir un avantatge estratègic contra el Cap següent. Nivell de dificultat: **Mitjà**.

### 🚫 Què NO inclourà el joc (Out of Scope)
Per mantenir la viabilitat tècnica i complir amb els terminis, s'exclou explícitament:
- **No** hi haurà exploració de món obert (l'avanç és mitjançant menús i escenes tancades).
- **No** es poden capturar els Caps (Bosses).
- **No** hi haurà inventari d'objectes complex ni evolucions de les criatures.

---

## 4. Riscos i Viabilitat

### ⚠️ Riscos Tècnics Reals
1. **Lògica de Torns Múltiples:** Programar correctament la màquina d'estats a Roblox per gestionar escenaris 2v1 (Mag + Criatura vs Boss) sense bloquejos.
2. **Sistema de "Tags" (Etiquetes):** Diferenciar programàticament un "Enemic Normal" (mostra botó de captura) d'un "Boss" (avança la història).
3. **Gestió del Reclutament (Persistència):** Aconseguir que el sistema de dades guardi quina criatura has escollit perquè aparegui correctament al següent combat.

### 🤖 Exploració amb IA
S'ha utilitzat IA en fase de *brainstorming* i estructuració:
* *Prompt 1:* "Voy a hacer un proyecto nuevo en Roblox Studio, quiero hacer un combate por turnos o una historia, yo haré lo visual y necesito ayuda."
* *Prompt 2:* "Ayúdame a completar el documento. Voy a hacer una mezcla entre Pokémon y Harry Potter, quiero que los boss no sean capturables, hacer mini batallas por la historia donde puedas reclutar."

### ✅ Justificació de Viabilitat
Aquest disseny és viable perquè utilitza un sistema de progressió lineal. En eliminar l'exploració lliure i l'inventari, l'esforç de programació es destina al 100% a aplicar **Clean Code** i dissenyar una arquitectura sòlida per al sistema de combat i interfícies.

---

## 5. Planificació i Eines

### 🗺️ Mini Pla de Fases
- [x] **Fase 1:** Disseny i aprovació d'aquest README.
- [ ] **Fase 2:** Programació Backend (Arquitectura de Dades, Classes de Lluita).
- [ ] **Fase 3:** Disseny Frontend (GUI de combat, barres de vida, botons).
- [ ] **Fase 4:** Integració del Core Loop i Debugging.

### 🛠️ Eines Previstes
* **Roblox Studio:** Motor de desenvolupament principal i gestor de GUI.
* **Luau:** Llenguatge de programació per a la lògica de servidor (Backend) i client (Frontend).
* **IA Assistida (Gemini):** Com a eina de suport per planificar l'arquitectura del codi i refactorització.
