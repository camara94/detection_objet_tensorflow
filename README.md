# Detection Objet Tensorflow

Vous souhaitez commencer à créer vos propres modèles de détection d'objets d'apprentissage en profondeur ?  Besoin d'aide pour détecter des éléments pour votre cours, votre startup ou votre entreprise ?  Dans ce repos, vous apprendrez tout ce que vous devez savoir pour passer de débutant à praticien en matière de détection d'objets en Deep Learning avec Tensorflow. Ce cours tourne principalement autour de Python, mais il y a aussi un peu de Javascript lorsqu'il s'agit de créer une application Web dans le projet 2. Mais ne vous inquiétez pas, nous allons le faire étape par étape afin que vous puissiez prendre votre temps et travailler dessus.

## Plan de la Formation

1. Installer Tensorflow sur une machine locale et sur Colab
2. Collecter et étiqueter des images pour la détection d'objets à l'aide de LabelImg
3. Former des modèles de détection d'objets alimentés par Deep Learning à l'aide de Python et TFOD
4. Détecter des objets en temps réel à l'aide d'une webcam et à l'aide d'images
5. Ajustez les modèles de détection d'objets pour améliorer la précision et le rappel
6. Exportez votre modèle vers Tensorflow JS pour l'intégrer dans les applications Web React JS
7. Exportez votre modèle vers TFLite pour une utilisation sur un Raspberry Pi

## Objectif de la Formation

1. Détection de gestes - c'est le premier projet où vous pourrez créer un modèle qui détecte quatre gestes différents
2. Détection de défauts basée sur un microscope - ici, nous utiliserons un microscope USB pour détecter les défauts dans les LED et les PCB à l'aide de TFOD et Python
3. Détection de la direction Web - dans ce modèle, vous apprendrez à détecter les directions manuelles pour l'intégration dans une application Web React Js avec Tensorflow Js
4. Détection des émotions faciales - vous apprendrez ici comment estimer les émotions faciales à l'aide de la détection d'objets Tensorflow sur un Raspberry Pi avec TFLite

## Création d'environnement virtuel

pourquoi créer un environnement virtuel
1. on pourrait selection tous les packages et objets concernant une tâche spécifique. 
   Par exemple: dans ce cas les objet consernant la detection d'objets en **tensorflow** et **TFOD**
  pour enfin être sûr qu'il n'y a pas de conflit avec les autres packages
2. Ce que nous allons faire est de créer un nouvel environnement virtuel pour des
 eventuel conflit entre les packages
3. Cela nous assure qu'on a des packages principaux 

## Installation et Configuration

### Crée Environnement 

<pre>
<code> 
 	python -m venv tfod
</code>
</pre>

### Activation de l'Environnement sous (MacOS)

<pre>
<code> 
 	source tfod/bin/activate
</code>
</pre>

### Activation de l'Environnement sous (Windows)

<pre>
<code> 
 	.\tfod\Scripts\activate
</code>
</pre>
### Mise à Jour des Dépendances PIP

<pre>
<code> 
 	python -m pip install --upgrade pip
</code>
</pre>

### Ajout de it à Jupyter Kernel (Noyau)

Ce package nous permet de lier notre environnement virtuel à jupyter notebook

<pre>
<code> 
 	pip install ipykernel
	python -m ipykernel install --user --name tfod
</code>
</pre>

### Installer les outils de génération de Visual C++

* [https://visualstudio.microsoft.com/fr/vs/community/](https://visualstudio.microsoft.com/fr/vs/community/)

### Installer la version appropriée de CUDA et cuDNN

Alors ceuci ne sont pas obligatoire si vous n'avez pas un processeur graphique dedié, mais par contre si nous en avez cela va permettre d'acceler vos processus d'entrainement de modèle de **Deep Learning** 

* (**Linux et MacOS**): [https://www.tensorflow.org/install/source#ubuntu](https://www.tensorflow.org/install/source#ubuntu)

* (**Windows**): [https://www.tensorflow.org/install/source_windows](https://www.tensorflow.org/install/source_windows)