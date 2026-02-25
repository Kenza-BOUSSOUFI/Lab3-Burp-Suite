# Lab3-Burp-Suite
Étape 1 — Préparer Burp Suite
1- On Lance Burp Suite, puis on crée un projet temporaire.
2- Ensuite, dans l’onglet Proxy.On vérifir que la page “Intercept” est visible et que l’état Intercept is off apparaît:
Étape 2 — Vérifier le Proxy Listener (adresse et port)
1- Dans proxy -> proxy settings:
On vérifie qu’un listener est actif
2- On modifie le Proxy listener pour passer de loop back only à All Interfaces sur le port 8080, pour permettre a l'emulateur android de joindre le proxy via l'IP du PC.
Étape 3 — Identifier l’adresse réseau de la machine hôte
1- On doit identifier l'adresse IP de la machine local, ou utiliser l’adresse réseau de la machine hôte accessible depuis l’émulateur Android qui est 10.0.2.2.
Étape 4 — Configurer le proxy côté Android Emulator
1- J'ai utilisé l'émulateur pixel 6 ( API 36) d'Android studio.
2- Pour configurer la liaison entre l'emulateur et Burp suite, on doit accedé à: Settings > Network & Internet > Internet > Proxy (Choisis Manual).
