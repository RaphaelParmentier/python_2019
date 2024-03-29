<!DOCTYPE html><html><head><meta charset="utf-8"><title>Etude du complexe sRNP.md</title><style></style></head><body id="preview">
<h1><a id="Etude_du_complexe_sRNP_0"></a>Etude du complexe sRNP</h1>
<h3><a id="Djabali_Yacine__Parmentier_Raphal_1"></a>Djabali Yacine &amp; Parmentier Raphaël</h3>
<h3><a id="M1_BIBS_2018_2019_2"></a>M1 BIBS 2018 -2019</h3>
<p>[<img src="https://hal.archives-ouvertes.fr/UNIV-PARIS-SACLAY/public/logo_UP_saclay_final.png" alt="Paris-Saclay">]</p>
<p><a href="https://travis-ci.org/joemccann/dillinger"><img src="https://travis-ci.org/joemccann/dillinger.svg?branch=master" alt="Build Status"></a></p>
<h1><a id="Objectif_8"></a>Objectif</h1>
<p>Le projet vise à essayer de comprendre l’impact de certaines mutations dans certains composants du complexe sRNP H/ACA, chez l’archaea: Pyrococcus abyssi. La structure 3D d’un complexe RNP H/ACA de ce type chez les eucaryotes n’étant pas connue, le système équivalent chez les archaea (procaryote) est donc utilisé comme modèle.<br>
Le complexe sRNP H/ACA, constituée de cinq domaines distincts, permet (catalyse) l’isomérisation de l’uridine en pseudo-uridine ψ (réaction d’addition NH).<br>
Au cours de cette étude, nous cherchons comprendre le rôle de chacun des domaines du complexe dans l’interaction avec l’ARN. En mesurant /comparant les temps de contact entre ces résidus dans la structure sauvage ainsi que la flexibilité des différents domaines de la protéine lors de l’interaction avec l’ARN.<br>
Afin de répondre à cette problématique nous disposons d’un outil puissant : Python.<br>
Ainsi qu’un fichier .pdb  disposant de 500 conformations (dont le formatage ne sera pas détaillé ici) du complexe afin de pouvoir suivre sa dynamique.</p>
<h1><a id="Organisation_du_code_16"></a>Organisation du code</h1>
<p>Nous avons conceptionné nos codes de façons a ce qu’ils soient modulaire et que nos fonctions soient les plus generiques possibles.<br>
Par consequent nous aurons 4 modules qui contiendra nos fonctions, ainsi que 6 scripts qui traiteras les inputs et sortiras les outputs.</p>
<h2><a id="Les_scripts_20"></a>Les scripts</h2>
<p>(A lancer dans l’ordre suivant pour garder la linearité de notre rapport)</p>
<ul>
<li>script_RMSDGLO.py&lt;USAGE : <a href="http://script.py">script.py</a> input.pdb output_brut.txt output_graphique.png&gt;//temps d’execution approximatif :250 sec</li>
<li>script_RMSDGLOREF.py&lt;USAGE : <a href="http://script.py">script.py</a> input.pdb output_brut.txt output_graphique.png&gt; //temps d’execution approximatif :30 sec</li>
<li>script_RMSDLOC.py &lt;USAGE : <a href="http://script.py">script.py</a> input.pdb output_brut.txt  //temps d’execution approximatif :250 sec</li>
<li>script_RMSDLOCREF.py&lt;USAGE: <a href="http://script.py">script.py</a> input.pdb output_brut.txt output_graphique.png&gt;//temps d’execution approximatif :30 sec</li>
<li>script_INTERFACEGLO.py&lt;USAGE:script.py input.pdb output_brut.txt output_graphique.png&gt;//temps d’execution approximatif :150 s</li>
<li>script_INTERFACELOC.py &lt;USAGE : <a href="http://script.py">script.py</a> input.pdb output_graphique.png&gt;//temps d’execution approximatif :150 sec</li>
</ul>
<p>ATTENTION : Bien mentionner les noms des outputs en arguments .txt pour les resultats brut et .png pour les resultats graphique</p>
<h2><a id="Les_modules_31"></a>Les modules</h2>
<ul>
<li>func_parse.py</li>
<li>func_DistMD.py</li>
<li>func_RMSD.py</li>
<li>func_interface.py</li>
</ul>
<h3><a id="Donne_41"></a>Donnée</h3>
<ul>
<li>pab21_500.pdb</li>
</ul>
<h2><a id="Usage"></a>Usage</h2>
<p>Télécharger le projet directement par l’interface graphique de GitHub ou en faisant un clone du projet avec la commande suivante :</p>
<p>git clone https://github.com/RaphaelParmentier/JAVA_2019.git</p>
<p>Ensuite exécutez diretement les fichier script_MEHTOD.py avec la commande :</p>
<p>python3 script_MEHTOD.py fichier.pdb nom_desire_output_brut.txt nom_desire_output_graphique.png</p>
<p>(voir la rubrique "Les Scripts" pour les usages spécifiques)</p>
</body></html>
