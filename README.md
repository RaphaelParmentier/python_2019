<title>Etude du complexe sRNP.md</title><style></style>
Etude du complexe sRNP
Djabali Yacine & Parmentier Raphaël
M1 BIBS 2018 -2019
[Paris-Saclay]

Build Status

Objectif
Le projet vise à essayer de comprendre l’impact de certaines mutations dans certains composants du complexe sRNP H/ACA, chez l’archaea: Pyrococcus abyssi. La structure 3D d’un complexe RNP H/ACA de ce type chez les eucaryotes n’étant pas connue, le système équivalent chez les archaea (procaryote) est donc utilisé comme modèle.
Le complexe sRNP H/ACA, constituée de cinq domaines distincts, permet (catalyse) l’isomérisation de l’uridine en pseudo-uridine ψ (réaction d’addition NH).
Au cours de cette étude, nous cherchons comprendre le rôle de chacun des domaines du complexe dans l’interaction avec l’ARN. En mesurant /comparant les temps de contact entre ces résidus dans la structure sauvage ainsi que la flexibilité des différents domaines de la protéine lors de l’interaction avec l’ARN.
Afin de répondre à cette problématique nous disposons d’un outil puissant : Python.
Ainsi qu’un fichier .pdb disposant de 500 conformations (dont le formatage ne sera pas détaillé ici) du complexe afin de pouvoir suivre sa dynamique.

Organisation du code
Nous avons conceptionné nos codes de façons a ce qu’ils soient modulaire et que nos fonctions soient les plus generiques possibles.
Par consequent nous aurons 4 modules qui contiendra nos fonctions, ainsi que 6 scripts qui traiteras les inputs et sortiras les outputs.

Les scripts
(A lancer dans l’ordre suivant pour garder la linearité de notre rapport)

script_RMSDGLO.py<USAGE : script.py input.pdb output_brut.txt output_graphique.png>//temps d’execution approximatif :250 sec
script_RMSDGLOREF.py<USAGE : script.py input.pdb output_brut.txt output_graphique.png> //temps d’execution approximatif :30 sec
script_RMSDLOC.py <USAGE : script.py input.pdb output_brut.txt //temps d’execution approximatif :250 sec
script_RMSDLOCREF.py<USAGE: script.py input.pdb output_brut.txt output_graphique.png>//temps d’execution approximatif :30 sec
script_INTERFACEGLO.py<USAGE:script.py input.pdb output_brut.txt output_graphique.png>//temps d’execution approximatif :150 s
script_INTERFACELOC.py <USAGE : script.py input.pdb output_graphique.png>//temps d’execution approximatif :150 sec
ATTENTION : Bien mentionner les noms des outputs en arguments .txt pour les resultats brut et .png pour les resultats graphique

Les modules
func_parse.py
func_DistMD.py
func_RMSD.py
func_interface.py
Donnée
pab21_500.pdb
Usage
Télécharger le projet directement par l’interface graphique de GitHub ou en faisant un clone du projet avec la commande suivante :

git clone https://github.com/RaphaelParmentier/JAVA_2019.git

Ensuite exécutez diretement les fichier script_MEHTOD.py avec la commande :

python3 script_MEHTOD.py fichier.pdb nom_desire_output_brut.txt nom_desire_output_graphique.png

(voir la rubrique "Les Scripts" pour les usages spécifiques)
