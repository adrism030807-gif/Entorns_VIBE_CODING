⚔️ README: Microjoc d'Acció i Supervivència 3D
🔗 ENLLAÇ AL VÍDEO GAMEPLAY: https://docs.google.com/videos/d/1yVFRbYBxyr-SKrflJw3iBFJsBsKwJbYfI8NZBqn83x0/edit?usp=sharing

Document de presentació del projecte (README) per a la fase final de desenvolupament. Aquest projecte és un joc d'acció en 3D en temps real desenvolupat a Roblox Studio, on el jugador explora un entorn i combat enemics de forma directa.

📋 Índex
Visió General

Controls i Jugabilitat

Canvis en l'Abast del Projecte (Pivotatge)

Riscos i Viabilitat Tècnica

Planificació i Eines

1. Visió General
🎯 Tipus de microvideojoc
Joc d'acció en tercera persona (Hack and Slash / Exploració 3D) situat en un entorn tancat (una vila).

💡 Definició de la idea
Ets un aventurer que ha de sobreviure i netejar un poblat de l'aparició d'enemics (Zombis/Dummies). L'acció transcorre en temps real, aprofitant el motor físic de Roblox per al moviment i el combat cos a cos.

🏆 Objectiu del joc
Equipar-se l'arma, explorar l'entorn dissenyat i derrotar tots els enemics presents al mapa abans que ells redueixin la teva vida a zero.

2. Controls i Jugabilitat
🎮 Interacció del Jugador
El joc abandona els menús estàtics per oferir un control complet i fluid sobre l'avatar en un espai tridimensional.

⌨️ Controls de PC:

W, A, S, D: Moure el personatge.

Barra Espaiadora: Saltar.

Tecles Numèriques (1, 2...): Equipar o desequipar l'espasa de l'inventari.

Clic Esquerre del Ratolí: Atacar amb l'espasa.

Ratolí (Moure): Controlar la càmera i la direcció de la visió.

3. Canvis en l'Abast del Projecte (Pivotatge)
🔄 Adaptació del disseny original
La proposta inicial d'aquest projecte era un RPG per torns de captura de criatures. Durant la fase de desenvolupament (Fase 2: Backend), els scripts de control de torns i el sistema de combat van presentar errors greus d'estat (state machine).
Per garantir una entrega funcional i un producte jugable, s'ha pres la decisió de disseny (pivot) de transformar-lo en un joc d'acció en temps real.

🚫 Què NO inclou el joc (Out of Scope actual)

Sistema de torns i menús d'atac.

Reclutament d'enemics.

Sistema d'inventari complex (es simplifica a una arma principal).

4. Riscos i Viabilitat
⚠️ Resolució de Riscos Tècnics
El principal risc tecnològic era l'error en els Scripts de l'arma personalitzada (Weapon.Sword). La solució aplicada ha estat netejar el repositori (StarterPack i StarterPlayerScripts) i implementar la "Classic Sword" oficial de l'ecosistema Roblox, garantint així un 100% de fiabilitat en les caixes de col·lisió (hitboxes) i l'animació de dany (Humanoid Taking Damage).

🤖 Exploració amb IA
S'ha utilitzat IA (Gemini) en fase de troubleshooting (resolució de problemes) i debugging. La IA ha estat clau per:

Identificar per què els Scripts originals fallaven a l'hora de rebre els "Inputs" del jugador.

Aconsellar el pivotatge a la "Classic Sword" per complir amb el deadline de l'entrega.

Guiar en la neteja d'arxius residuals al motor de Roblox.

5. Planificació i Eines
🛠️ Eines Utilitzades

Roblox Studio: Motor 3D de desenvolupament principal, gestor d'entorn i físiques.

Roblox Toolbox: Ús de models estàndard (Zombies/Dummies i Espasa Clàssica) per agilitzar el desenvolupament de la jugabilitat.

Markdown: Per a l'estructuració d'aquesta documentació.

OBS / Eina de Captura: Per a la gravació del Gameplay final de demostració.
