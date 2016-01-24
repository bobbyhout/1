Libopenshot is the new video framework of the Openshot Video Editor done by developpers of this project. But you can use it independently.
Libopenshot is composed of libopenshot-audio and libopenshot. 

You MUST INSTALL Libopenshot-audio in FIRST. AFTER, you can install/compile libopenshot.

You get a document about how to get Libopenshot, to have dependencies on the three system (i.e LInux, Mac and Window) and how to compile them here : https://docs.google.com/document/d/1V6nq-IuS9zxqO1-OSt8iTS_cw_HMCpsUNofHLYtUNjM/pub and here https://launchpad.net/~openshot.developers/+archive/ubuntu/libopenshot-daily.

There are the same.

Basically, you can compile them of the same way i.e :
mkdir build
cd build
cmake ../
make 
sudo make install

After you get the last version of openshot-qt here : 
https://launchpad.net/openshot/2.0

Go to the src folder, open a console and type :
python launch.py

That's all.

Another way easiest than the compilation is to use this ppa if you are on Ubuntu or an derivative like Linux Mint, Elementary Os,...

https://launchpad.net/~openshot.developers/+archive/ubuntu/libopenshot-daily

Libopenshot  est le nouveau framework video du projet Openshot Video Editor créer par les developpeurs de ce meme projet. Mais vous pouvez l'utiliser independament.


Libopenshot est composé de libopenshot-audio et de libopenshot.

Vous DEVEZ installer libopenshot-audio en premier. Après, vous pouvez installer libopenshot.

Vous avez un document qui vous explique comment obtenir Libopenshot, avoir les dependances pour les 3 systemes (cad Linux, Mac et Windows) et comment les compiler ici https://docs.google.com/document/d/1V6nq-IuS9zxqO1-OSt8iTS_cw_HMCpsUNofHLYtUNjM/pub et ici https://launchpad.net/~openshot.developers/+archive/ubuntu/libopenshot-daily.  

Ils sont identiques.

Basiquement, vous pouvez les compiler de la même manière : 
mkdir build
cd build
cmake ../
make 
sudo make install

Après, vous obtenez la version d'openshot-qt ici : 
https://launchpad.net/openshot/2.0

Allez dans le dossier src, ouvrez une console et tapez :
python launch.py

C'est tout.

Un autre moyen, plus facile que la compilation est d'utiliser le ppa disponible sur cette page pour Ubuntu et derivé comme Linux Mint, Elementary OS, ....:
https://launchpad.net/~openshot.developers/+archive/ubuntu/libopenshot-daily