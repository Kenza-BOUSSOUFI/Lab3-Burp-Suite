# Lab3-Burp-Suite

Étape 1 — Préparer Burp Suite

1- On Lance Burp Suite, puis on crée un projet temporaire.

<img width="942" height="705" alt="1" src="https://github.com/user-attachments/assets/2ca13c25-39dc-4a76-8782-4fdd42fac318" />

<img width="948" height="705" alt="2" src="https://github.com/user-attachments/assets/7fcb3f33-0295-45cc-a42e-a6aa05ea60fa" />

2- Ensuite, dans l’onglet Proxy.On vérifir que la page “Intercept” est visible et que l’état Intercept is off apparaît:

<img width="1908" height="1021" alt="3" src="https://github.com/user-attachments/assets/9195dfbb-dbd3-463e-bb3c-fb62df673d5c" />

Étape 2 — Vérifier le Proxy Listener (adresse et port)

1- Dans proxy -> proxy settings:
On vérifie qu’un listener est actif:
Port proxy : 8080
Adresse d’écoute : 172.0.0.1 -> loop back only

<img width="1920" height="1034" alt="5" src="https://github.com/user-attachments/assets/8322a5de-b9f6-4b9e-ab59-f4482381598d" />

2- On modifie le Proxy listener pour passer de loop back only à All Interfaces sur le port 8080, pour permettre a l'emulateur android de joindre le proxy via l'IP du PC.

<img width="1144" height="715" alt="6" src="https://github.com/user-attachments/assets/aae96988-7a4e-4d8d-a954-278a1652af36" />
 
<img width="1459" height="380" alt="7" src="https://github.com/user-attachments/assets/1ef26ec5-107b-4a7f-a0fd-2c027ad5a0a3" />

Étape 3 — Identifier l’adresse réseau de la machine hôte
1- On doit identifier l'adresse IP de la machine local, ou utiliser l’adresse réseau de la machine hôte accessible depuis l’émulateur Android qui est 10.0.2.2.
Étape 4 — Configurer le proxy côté Android Emulator
1- J'ai utilisé l'émulateur pixel 6 ( API 36) d'Android studio.
2- Pour configurer la liaison entre l'emulateur et Burp suite, on doit accedé à: Settings > Network & Internet > Internet > Proxy (Choisis Manual).
