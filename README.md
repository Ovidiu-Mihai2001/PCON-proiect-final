# Sintetizator Algoritmic
Acest proiect presupiune dezvoltarea un sintetizator algoritmic în Max MSP care generează automat secvențe muzicale pe baza unei transformări numerice. Utilizatorul introduce un număr pozitiv, iar sintetizatorul aplică următorul algoritm iterativ:

- dacă numărul este par, este împărțit la 2;
- dacă este impar, este înmulțit cu 3, se adaugă 1, apoi se împarte la 2;
- procesul continuă până când se ajunge la valoarea 1.

Opțional, se poate alege ca notele generate să fie cuantizate într-o gamă muzicală la legere (de exemplu Do Major, La minor etc...), sau se poate lăsa sintetizatorul să genereze notele liber, fără restricții.

## Instalare
Cerințe sistem:
- MAX/MSP versiunea 8 sau mai recentă (recomandat MAX 8.5+);
- Opțional, MDID controller.

Descărcare și organizare fișiere
- Creează un folder dedicat, de exemplu: Proiect_MAX;
- Copiază toate fișierele .maxpat în acel folder.

## (Utilizare)
Lansare și rulare:
- Deschide MAX/MSP;
- Deschide mai întâi patch-ul ProiectMax_Algoritm.maxpat;
- Deschide patch-ul ProiectMax_MIDI.maxpat;
- Patch-urile vor comunica între ele prin obiecte send/receive, poly~, sau noteout/notein.

![](Schema.jpg)

Redare și interacțiune:
- Selectează o gamă apăsând pe unul dintre butoanele gamei muzicale;
- Setează tempo-ul introducând o valoare în numărul conectat la [metro];
- Folosește claviatura virtuală (kslider) sau un controller MIDI extern pentru a genera note pe baza algoritmului implementat.

## (Istoric)

(15.05) Implementarea algoritmului de genarare a notelor muzicale.

(27.05) Adaugarea posibilității de generare pe anumite game muzicale la alegere, crearea unei interfețe usor de utilizat(Presentation Mode).

(X.06) ...

## (Link-uri)
...

# Dezvoltarea proiectului

Pentru început:

1. Creează-ți cont pe Github
2. Download și install [Github Desktop](https://desktop.github.com/)
3. Citește [acest ghid](https://charlesmartin.com.au/blog/2020/08/09/student-project-repository) și ține la îndemână [Markdown Cheat Sheet](https://www.markdownguide.org/cheat-sheet).

Apoi, procesul este următorul (inspirat de [aici](https://cs.anu.edu.au/courses/comp1720/deliverables/05-major-project/#submission-process)):

1. *fork* al acestui template către propriul tău cont de Github

![](assets/fork.gif)

_(dacă preferi cumva ca repo-ul să nu fie vizibil de către public, îl poți seta ca Private din Settings - "Change visibility". Atunci trebuie să mă adaugi drept colaborator, ca eu să am acces.)_

2. *clone* al repo-ului din Github Desktop pentru a-l downloada local

![](assets/clone.gif)

3. *commit* și *push* pe măsură ce lucrezi la proiect. Ultima versiune push-ată pe server înainte de deadline va conta pentru evaluare.

![](assets/commit.gif)

## Elemente obligatorii

1. Acest readme completat. Titlu, descriere, mod de utilizare, istoric, link-uri utile.

   Poți include și imagini și chiar [gif-uri animate](https://www.screentogif.com/), sau link-uri către materiale audio/video.
   
   Vezi [aici](https://charlesmartin.com.au/blog/2020/08/09/student-project-repository) mai multe sugestii.

2. [Declarația de originalitate](statement-of-originality.yml) completată. Tot ce nu este inclus acolo va fi considerat 100% contribuție proprie.

    *(formatul este adaptat de [aici](https://gitlab.cecs.anu.edu.au/comp1720/2018/comp1720-2018-major-project/-/blob/master/statement-of-originality.yml). Da, este un pic ironic să refolosim un doc [de altundeva](https://cs.anu.edu.au/courses/comp1720/resources/faq/#how-do-i-fill-out-my-statement-of-originality), dar menționăm sursa deci nu este plagiat!)*

3. Proiectul în sine. Tot codul trebuie să fie prezent, proiectul trebuie să poată rula conform instrucțiunilor din readme. Dacă e nevoie de asset-uri mari (sunete, video etc), [folosește Git LFS](https://git-lfs.github.com/) sau include link de download în instrucțiunile de instalare.

