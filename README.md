# TELEVISION-MECANIQUE---REGROUPEMENT-VIDEO-COMPOSITE--SYNCHRO-LED-PUISSANCE-DFTA126 https://youtu.be/EH3WCfFm2zc
Ce schéma a pour rôle de venir commander le groupement de LEDs de puissance à l'arrière du disque de Nipkow. 
U7 vient retrancher une tension continue équivalente au niveau max du signal de synchro au signal de video composite, de manière à n'envoyer vers le driver de LEDs que le signal de luminance 0 - 100%.
Ce soustracteur réalise une différence sans gain entre VideoComposite et BlackLevel sous conditions que R24=R25=R21=R22.
BlackLevel étant le résultat du diviseur potentiomètrique RP9 (10K), ces 4 résistances ne peuvent être trop faibles vis à vis du potentiomètre sous peine de perturber significativement son rapport de division. C'est pourquoi j'ai choisi des valeurs de 56K.
C3  a pour fonction de filtrer la remontée du signal sur e-. Sa valeur devra probablement être ajustée en pratique en tenant compte du signal VideoComposite.
C4 a été rajouté suite à des adaptations pratiques (ce qu'on appelle un avis ingénieur).
U6, Q4 et les 4 résistances de source de 15 ohms constituent un driver en courant dont lavaleur est égale e+ de Q6 divisé par la résistance équivalente de source (Actuellement 4 résistances de 15 ohms 1W chacune soit 3.75 ohms 4W).
RP10 et R29 apportent une petite correction de manière à bénéficier d'un certain ajustement en contraste. Ici j'entends par contraste l'écart entre le 100% blanc et le noir absolu, tout en gardant le même niveau de lumière.
R27 servira ultérieurement dans le cas d'un rajout d'une éventuelle protection contre une surintensité accidentelle dans les LEDs.
R23 également doit sa présence par avis ingénieur (ici atténuer d'éventuelles petites oscillations parasites).
Des ajustements de niveau seront sans doute nécessaires pour une version définitive.

