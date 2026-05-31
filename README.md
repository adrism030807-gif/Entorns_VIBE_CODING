🧙‍♂️ README: Microjoc d'Acció i Supervivència 3D

🔗 ENLLAÇ AL VÍDEO GAMEPLAY: https://docs.google.com/videos/d/1yVFRbYBxyr-SKrflJw3iBFJsBsKwJbYfI8NZBqn83x0/edit?usp=sharing

Document de presentació del projecte (README) elaborat per a la fase final de desenvolupament. Aquest projecte és un joc d'acció en 3D en temps real desenvolupat a Roblox Studio.

📋 Índex

Visió General
Jugabilitat i Regles
Abast i Límits del Projecte
Riscos i Viabilitat
Planificació i Eines

1. Visió General

🎯 Tipus de microvideojoc

Joc d'acció en tercera persona situat en un entorn tancat (una vila).

💡 Definició de la idea

Ets un aventurer que ha de sobreviure i netejar un poblat de l'aparició d'enemics (Zombis/Dummies). L'acció transcorre en temps real, aprofitant el motor físic de Roblox per al moviment i el combat cos a cos.

🏆 Objectiu del joc

Equipar-se l'arma, explorar l'entorn dissenyat i derrotar tots els enemics presents al mapa abans que ells redueixin la teva vida a zero.

2. Jugabilitat i Regles

🎮 Rol del jugador

El jugador controla el seu avatar en un espai tridimensional. L'exploració i el combat es fan en temps real, movent-se lliurement pel mapa per atacar i esquivar.

⌨️ Controls del Joc

W, A, S, D: Moure el personatge.

Barra Espaiadora: Saltar.

Tecles Numèriques (1, 2...): Equipar o desequipar l'espasa de l'inventari.

Clic Esquerre del Ratolí: Atacar amb l'espasa.

Ratolí (Moure): Controlar la càmera i la direcció de la visió.

3. Abast i Límits del Projecte

🔄 Canvis en el disseny (Pivotatge)

La proposta inicial d'aquest projecte era un RPG per torns de captura de criatures. Durant la fase de desenvolupament, els scripts de control de combat van presentar errors greus. Per garantir una entrega funcional i un producte jugable en el termini marcat, s'ha pres la decisió de disseny (pivot) de transformar-lo en un joc d'acció en temps real.

🚫 Què NO inclourà el joc (Out of Scope)

Per mantenir la viabilitat tècnica, s'exclou explícitament:

No hi haurà sistema de torns ni menús d'atac.

No es poden capturar els enemics.

No hi haurà inventari d'objectes complex (es simplifica a una arma principal).

4. Riscos i Viabilitat

⚠️ Riscos Tècnics Reals

L'error de l'arma personalitzada: El principal risc tecnològic era l'error en els Scripts de la primera espasa (Weapon.Sword). La solució aplicada ha estat netejar el repositori i implementar la "Classic Sword" oficial de l'ecosistema Roblox, garantint així un 100% de fiabilitat en el dany i les col·lisions.

🤖 Exploració amb IA

S'ha utilitzat IA (Gemini) en fase de resolució de problemes i debugging:

Identificar per què els Scripts originals fallaven.

Aconsellar el pivotatge a la "Classic Sword" per salvar el projecte i complir amb el deadline.

Guiar en la neteja d'arxius residuals al motor de Roblox.

5. Planificació i Eines

🛠️ Eines Previstes i Utilitzades

Roblox Studio: Motor 3D de desenvolupament principal, gestor d'entorn i físiques.

Roblox Toolbox: Ús de models estàndard (Zombies/Dummies i Espasa Clàssica) per agilitzar el desenvolupament.

OBS Studio: Per a la gravació del vídeo Gameplay final de demostració.
