# Ewolucyjne wnioskowanie gramatyczne

## Roadmap
[Strona domowa]() | [Okładka](#okładka) | [Streszczenie](#streszczenie) | [Abstract](#abstract) | [Spis treści](#spis-treści) | [PDF](#pdf) | [Errata](#errata)

## Okładka
<img src="files/ewg_unold.jpg" alt="Alt Text" style="width:50%; height:auto;">

## Streszczenie
W monografii została podjęta ważna i płodna zarówno teoretycznie, jak i praktycznie tematyka wnioskowania gramatycznego (maszynowego uczenia gramatyk). Zaproponowano nowy model ewolucyjnego wnioskowania gramatycznego, którego zasadniczym przeznaczeniem jest indukcja gramatyki bezkontekstowej. Konstrukcja nowego modelu ewolucyjnego wykorzystuje mechanizm uczenia stosowany w uczących się systemach klasyfikujących. W modelu klasyfikatorami są produkcje gramatyki bezkontekstowej podane w postaci normalnej Chomskyego, natomiast otoczeniem, do którego adaptuje się system, jest zbiór uczący składający się z przykładowych zdań opatrzonych etykietą, określającą przynależność lub brak przynależności zdania do poszukiwanego języka. Celem uczenia jest poprawna klasyfikacja zdań uczących. Ponieważ zbiór klasyfikatorów tworzy zestaw produkcji gramatyki, to poprawna klasyfikacja etykietowanych zdań oznacza wyindukowanie poszukiwanej gramatyki języka. Model śledzi produkcje użyte podczas analizy zbioru uczącego i po jej zakończeniu oblicza funkcję dopasowania każdej produkcji. Nowe produkcje gramatyki są odkrywane podczas procesu indukcji przez mechanizm pokrycia oraz algorytm genetyczny. W pracy można wyodrębnić dwie części.

Pierwsza część pracy wprowadza w tematykę wnioskowania gramatycznego, ewolucyjnego przetwarzania oraz uczących się systemów klasyfikujących. W szczególności zaprezentowano aktualny stan badań w zakresie indukcji gramatyki bezkontekstowej,  nowy sposób kategoryzacji uczących się systemów klasyfikujących oraz ich podstawowe modele w jednolitym ujęciu.

W drugiej części pracy zaproponowano oryginalny model ewolucyjnego wnioskowania gramatycznego, dedykowany indukcji gramatyki bezkontekstowej. Architekturę i działanie nowego modelu opisano posługując się kategoriami uczącego się systemu klasyfikującego. Wprowadzono tzw. mechanizm płodności produkcji, który wraz z mechanizmem ścisku oraz operatorem genetycznym inwersji ma przeciwdziałać wysokiej epistazie populacji produkcji modelu. Zdefiniowano nowe operatory pokrycia dostosowane do zastosowanej metody parsowania oraz estymatory dokładności i kosztu indukcji. Przeprowadzono indukcję języków regularnych z tzw. zbioru Tomity, wybranych formalnych języków bezkontekstowych, a także obszernych korpusów językowych. Eksperymenty wykazały, że model uzyskuje dla każdej z badanych klas języka wyniki porównywalne z najlepszymi ze znanych w literaturze przedmiotu i to nie tylko wśród metod ewolucyjnych, a w wielu wypadkach lepsze. Przeprowadzono badania symulacyjne modelu, których celem było eksperymentalne stwierdzenie własności proponowanego modelu ewolucyjnego. Poza wnioskami szczegółowymi osiągnięto również interesujące wyniki dotyczące ogólnych mechanizmów ewolucyjnych, jak wpływ selekcji turniejowej i ścisku na nacisk selektywny, czy rola nowego operatora pokrycia pełnego w procesie ewolucji populacji uczącego się systemu klasyfikującego. Wskazano na jedno z możliwych praktycznych zastosowań modelu, poza badanym już w monografii obszarem inżynierii lingwistycznej, jakim jest genomika obliczeniowa. Rozpatrywano zadanie rozpoznawania sekwencji telomerowej u człowieka oraz poszukiwania regionu promotorowego u bakterii E. coli. Model w obecnej implementacji może być zastosowany na wysokim poziomie estymatora swoistości do rozpoznawania regionów nienależących do sekwencji promotorowych.

## Abstract
### EVOLUTIONARY GRAMMATICAL INFERENCE

The monograph takes up an important and prolific, both theoretically and practically, subject of grammatical inference (grammar induction). A new model of evolutionary grammatical inference has been proposed, and its main purpose is context-free grammar induction. The structure of the new evolutionary model utilizes a learning mechanism applied in learning classifier systems. Here the classifiers are productions of context-free grammar presented in the Chomsky normal form, and the environment to which the system adapts is a learning set composed of the exemplary sentences. These sentences are labeled to distinguish a collocation or lack thereof to the searched language. The purpose of learning is a correct classification of learning sentences. Since the set of classifiers constitutes a grammar production unit, the correct classification of labeled sentences denotes inducing a grammar. The model monitors the productions used during the learning set analysis and after the analysis calculates a fitness function of each production. New grammar productions are discovered during the induction by a covering and a genetic algorithm.

The thesis is divided into two parts. The first part introduces into the area of grammatical inference, evolutionary processing, and learning classifier systems. In particular, the state of the art in the research in context-free grammar induction has been presented, a new categorization method of learning classifier systems has been proposed, and their generic models have been introduced in a uniform depiction.

The second part proposes an original model of evolutionary grammatical inference, dedicated to context-free grammar induction. The architecture and operation of the new model have been described with the use of the categories of a learning classifier system. So called “production fertility mechanism” has been introduced, which together with a crowding mechanism and inversion operator is supposed to counteract the high epistasis in production population. New covering operators adapted to the applied parsing method and estimators of induction accuracy and cost have been defined. The conducted induction includes regular languages from the Tomita set, chosen formal context-free languages, and large natural language corpora. These experiments showed that for each class of the examined language the model obtains results which are comparable with, and in some cases even better than, the best known in the literature of the subject, and not only among the evolutionary methods. Computer simulations have been conducted to experimentally identify qualities of the proposed evolutionary model. In addition to detailed conclusions, interesting results concerning general evolutionary mechanisms have been obtained, including an influence of tournament selection and of crowding on selective pressure, or the role of a new full covering operator in the evolution process of the population of a learning classifier system. Except for the examined in this thesis area of linguistic engineering, one of the potential applications of the model has been pointed to, which is computational genomics. The issues of an identification of human telomer sequence and of searching for a E. coli promoter region have also been investigated. The model in its current implementation can be applied at a high level of the specificity estimator to recognize regions not belonging to promotor sequences.

## Spis treści
	
Wstęp ...................................................................................................................................... 5

1.   Wnioskowanie gramatyczne ........................................................................................... 10

      1.1.   Wprowadzenie ....................................................................................................... 10

      1.2.   Obszary zastosowań ............................................................................................. 11

      1.3.   Wybrane pojęcia z teorii automatów i języków .................................................... 14

      1.4.   Paradygmaty uczenia ............................................................................................. 18

               1.4.1.   Identyfikacja w granicy .............................................................................. 18

               1.4.2.   Model PAC ................................................................................................ 19

               1.4.3.   Minimalna długość kodu ............................................................................ 20

               1.4.4.   Uczenie się na podstawie zapytań ............................................................ 21

      1.5.   Indukcja gramatyk bezkontekstowych .................................................................. 21

               1.5.1.   Indukcja na podstawie tekstu .................................................................... 23

               1.5.2.   Indukcja z danych strukturalnych ............................................................. 23

               1.5.3.   Indukcja podklas gramatyk bezkontekstowych ........................................ 25

               1.5.4.   Indukcja alternatywnych reprezentacji gramatyk bezkontekstowych ...... 26

               1.5.5.   Indukcja stochastycznych gramatyk bezkontekstowych .......................... 26

               1.5.6.   Indukcja z zastosowaniem metod sztucznej inteligencji ............................ 27

               1.5.7.   Algorytm CYK .......................................................................................... 35

2.   Metody ewolucyjne ....................................................................................................... 39

      2.1.   Programowanie ewolucyjne ................................................................................... 41

      2.2.   Strategie ewolucyjne .............................................................................................. 42

      2.3.   Algorytmy genetyczne .......................................................................................... 43

      2.4.   Programowanie genetyczne .................................................................................... 44

3.   Uczący się system klasyfikujący ................................................................................... 46

      3.1.   Architektura ........................................................................................................... 46

      3.2.   Klasyfikacja ........................................................................................................... 48

               3.2.1.   Kryterium zasięgu chromosomu ................................................................ 49

               3.2.2.   Kryterium miary użyteczności klasyfikatora ............................................ 50

               3.2.3.   Kryterium metody reprezentacji klasyfikatora ......................................... 51

               3.2.4.   Kryterium mechanizmu stosowanego w module odkrywczym ................ 52

               3.2.5.   Kryterium pamięci systemu ...................................................................... 53

      3.3.   Wybrane modele .................................................................................................... 55

               3.3.1.   LCS ............................................................................................................ 57

               3.3.2.   ZCS ............................................................................................................ 60

               3.3.3.   XCS ............................................................................................................ 63

               3.3.4.   ACS ............................................................................................................ 69

      3.4.   Zastosowania ......................................................................................................... 74

4.   Model GCS ..................................................................................................................... 76

      4.1.   Zadanie klasyfikacji ............................................................................................... 76

      4.2.   Werbalny opis modelu .......................................................................................... 78

      4.3.   Klasyfikator .......................................................................................................... 80

                4.3.1.    Definicja .................................................................................................... 80

                4.3.2.    Płodność ................................................................................................... 80

                4.3.3.    Przystosowanie ........................................................................................ 81

      4.4.   Gramatyka ............................................................................................................. 83

      4.5.   Architektura .......................................................................................................... 84

      4.6.   Pokrycie ................................................................................................................ 86

      4.7.   Ścisk ...................................................................................................................... 87

      4.8.   Algorytm genetyczny............................................................................................ 88

                4.8.1.    Schemat działania ...................................................................................... 88

                4.8.2.    Metody selekcji ........................................................................................ 89

                4.8.3.    Operatory genetyczne .............................................................................. 90

        4.9. Korekcja ................................................................................................................ 91

      4.10. Parametry .............................................................................................................. 92

      4.11. Algorytmiczny opis modelu ................................................................................. 93

                4.11.1.  Główna pętla programu ............................................................................ 93

                4.11.2.  Indukcja gramatyki ................................................................................... 94

                4.11.3.  Parsowanie zdania .................................................................................... 95

                4.11.4.  Ścisk .......................................................................................................... 97

                4.11.5.  Operatory pokrycia .................................................................................. 98

                4.11.6.  Algorytm genetyczny ............................................................................. 100

                4.11.7.  Korekcja .................................................................................................. 102

      4.12. Opis programu GCS ............................................................................................ 104

5.   Badania symulacyjne modelu GCS ............................................................................... 116

      5.1.   Estymatory symulacji ......................................................................................... 117

                5.1.1.    Dokładność indukcji ............................................................................... 117

                5.1.2.    Koszt indukcji ........................................................................................ 119

                5.1.3.    Dokładność generalizacji ......................................................................... 119

      5.2.   Zbiory uczące ...................................................................................................... 120

                5.2.1.    Wyrażenia regularne ............................................................................... 121

                5.2.2.    Języki bezkontekstowe .......................................................................... 122

                5.2.3.    Gramatyka dzięcięca ............................................................................... 123

                5.2.4.    Korpusy językowe ................................................................................. 123

      5.3.   Indukcja wybranych języków regularnych ......................................................... 126

      5.4.   Indukcja wybranych języków bezkontekstowych ............................................. 133

      5.5.   Indukcja języka naturalnego ................................................................................ 142

      5.6.   Badanie symulacyjne ........................................................................................... 145

                5.6.1.    Metody selekcji ...................................................................................... 146

                5.6.2.    Selekcja turniejowa ................................................................................. 147

                5.6.3.    Ścisk ........................................................................................................ 153

                5.6.4.    Operatory pokrycia ................................................................................ 156

                5.6.5.    Liczba początkowych produkcji nieterminalnych ................................. 164

                5.6.6.    Wielkość elity ......................................................................................... 167

                5.6.7.    Krzyżowanie i mutacja ........................................................................... 168

                5.6.8.    Inwersja .................................................................................................. 171

                5.6.9.    Liczba symboli nieterminalnych ............................................................. 172

                5.6.10.  Płodność ................................................................................................. 174

                5.6.11.  Wagi funkcji dopasowania produkcji ...................................................... 176

6.   Zastosowanie modelu GCS w genomice ....................................................................... 179

      6.1.   Rozpoznawanie sekwencji telomerowej ............................................................. 179

                6.1.1.    Preliminaria biologiczne .......................................................................... 179

                6.1.2.    Indukcja gramatyki „telomerowej” ......................................................... 181

      6.2.   Poszukiwanie regionów promotorowych ........................................................... 182

               6.2.1.    Preliminaria biologiczne .......................................................................... 182

                6.2.2.    Indukcja gramatyki „promotorowej” ...................................................... 184

7.   Podsumowanie .............................................................................................................. 187

Załącznik A ......................................................................................................................... 192

Załącznik B ......................................................................................................................... 194

Załącznik C ......................................................................................................................... 198

Bibliografia .......................................................................................................................... 199

Skorowidz ........................................................................................................................... 220

Spis rysunków .................................................................................................................... 223

Spis tabel ............................................................................................................................. 226

Streszczenie w języku angielskim ....................................................................................... 227
## PDF

## Errata
