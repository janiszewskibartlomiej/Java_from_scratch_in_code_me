```yaml
Java course in codeme:

Komputer - istotne elementy:
*Procesor
*Ram pamiec podreczna - tyczasowa
*Dysk twardy -pamiec dlugotrwala


kompilacja to zamiana jezyka zrozumialego dla nas na kodz rozumialy dla procesora

nr 1 to przenoszalonsc Javy, jest odporna na wirusy, szybkosc wykonania aplikacji. 
Wszystko co naisalismy jest ladowane do RAM. Aplikacji sa bardzo szybkie, uruchomieni jest dluzsze.

GIT jest super wazny i sedzi wersje dnaego pliku + mamy lokalne repo w git

maven to narzedzie, uzywane jest do trzymania bibliotek w swoim repo. Maven to jest repo do zarzadzania bibliotek.

JDK = JRE[java virtual machine] + JIT  + JAVAC

JRE musi byc zaintalowany na komie aby odpalac aplikacje java to jest virtualna maszyna.

Jast In Time >> to elemnt wirtualnej maszyny nie jako czyta napisany kod.

Javac zienia kod na bajtkod [czesciowo to kod zrozumialy dla maszyny]

eclipse >> noew project maven project.  

Mamy wiele mozliwosci koncowych wersji aplikacji i ni epotrzebujemy obecnei - wiec zazanaczamy bez archetypow

maven ma plik pom.xml sa tam - grupa [np zwierzw], artefakt [malpa], versja [1.0], 
packaging  te elemny to unikatowy projekt maiwenowy. bedziemy uzwaz POM czyli parentem projektu ktpry bedzie mial w sobie np 2 JAR

versje sa okreslane 3 elementami 1 duze zmiany, 2 versja, 3 bugfixy-snapshot to wersja wstepna 
```

![](https://github.com/janiszewskibartlomiej/Java_from_scratch_in_code_me/blob/master/2020-09-16_11h53_43.png "linux command")
![](https://github.com/janiszewskibartlomiej/Java_from_scratch_in_code_me/blob/master/2020-09-16_12h05_34.png "linux command 2")

```
dodawnie modółów >> overview >> Modules

JAR - to standardowy efekt >> wynik koncowym pracy .

struktura projektu jest narzucona przez maven
src/main/java >> nasz kody
src/main/resorces >> wszytsko co nei jest kodem np pliki tekstowe itd
targer/ nasz finalny plik jar

-------

public static void main(String[] args) {
		// TODO Auto-generated method stub

	}  >> umożliwia to ze plik jest uruchamialny

typy zmiennych

Najczesciej uzuwa sie INT - java uzywa int default oraz DOUBLE float prawie si enie uzywa

char do kodó ASCII sie uzywa


ctrl + shift + F  = autoforatowanie kodu

skrut do pisania System.out.println >> syso + enter  a jak "crtl + spacjamozn zobaczyc skruty

rzutowanei - zminana jednego typu na drug; mamy rzutowanie nei jawnne i jawne 

---

laczenie naszego katalogu z repo zdalnym

wchodzimy do katalogu i git init 


Existing folder
cd existing_folder
git init
git remote add origin ssh://git@git.codeme.pl:2244/jse-base/javase-ez1/Bartlomiej-Janiszewski/javase-workshop.git
vi .gitignore
git add .
git commit -m "Initial commit"
git push -u origin master


21-09-2020

Maven umozliwia budowanie kolejnych wersji aplikacji

git pull origin master  >> warto wpisywac poniewaz bedzei domyslnie sciagal wszytsko

w java mamy funkcje i procedury 

funkcja zwraca wynik  a procedura wykouje kod ale nie zwraca nic.

typ funkcji to np void -- dedykowany funkcji i nic nie zwraca czyli jest to procedura.

return mozn auzywac nawet w proceduze czyli tam gdzi ejest void

instrukcje warunkowe to podstawa programowania.


arytmetyka boola >> 

and >> && jezeli ktoray kolwiek jest false czyli 0 to wynik bedzie 0 czyli false
or ||  jezeli jeden z nich jest true to wynik bedzie true
xor czyli ^ roznica czyli jezeli jeden z nich jest rozny od drugiego to daje true czyli 1

if (warunek logiczny) {blok kodu >> wykonany jak warunke jest true
} else if (warunek) {
} else { blok kodu else jezeli warunke logiczny jest false
}

porownianei ==
rozny !=


rekurencja >> wywwolywanie sie tej samej fukcji

Programowanie obiektowe


klasa auto   a cechy np moc, pojemnosc it nazwya sie polami  a funkcje nazywa sie metodami
klasa to jest typ; obiekty moga w sobie zawierac obiekty
klasa to hermetyzacja[odcinamy bloki kodu] lub enkapsulacja[robimy n kapsulek]

klasa jest tylko informacją jak ma wygladac a obiekt to fizyczne stwonie danego obiektu na bazie projektu czyli klasy

kwalifikator dostepu sluzy do informowania czy jest publiczne czy nie jset publiczna i dostepna dane pola

== ni edzila przy typach obiektowych   obiekty poronujemy .equals

bez kawalifikatora to dostepna jest ta klasa dla wszytskich w danym pakieciei nazwywa sie kwalifikatorem pakietowy, a jak robimy public to mozeby uzywac w szedzie w kazdym pakieciei

wzorzec bina >> kazde pole robi sie prywatene a do pobierania i ustawiani robimy getery i setery

konstrukto to metoda wywywolywana przy uzyciu slowa new.

konstruktor nie zwarac typu i nazywa sie t samo jak klasa

this reprezentuje to wszytsko co storzylismy

przeciazenei np metod to w jednej klasie zdeklarowanie metody o tej samej nazwie ale roznia parametrami  >> jest to ustawiane bo java nie ma defaltowej wartosci

skrut myslowy do zapisywania ilosci parametró np public int getWiek(Czlowiek...ludz)  >>> w tym wypadku mozna wrzucac duza ilosc danych tegi samegotypu   ... == tablica o n elementach wiec podajemy np Czlowie(pierwszy, drugi trzeci)


rekurencje warto uzywac gdy nie wiemy ile razy petli mamy uzyc leprza jest petla

01/10/2020

programowanie obiektowe, dziedziczenie

Dziedziczenie >> zeby nie powelac kodu to robimy dziedziczenie poniewaz np ciezarowka dzidziczy po aucie np pojemnosc, kolor metode start i stop

this odnosi sie do nas samych a super odnosi sie do dziedziczonej klasy
kazda klasa moze dziedziczyc tylko po jednej klasie, natomiast mozemy miec dluga liste przodkow
.
super odwoluje sie do tylko jednego przodka

nazwa zmiennej nagminie nazywa sie  tak jak stworzona klasa !

wszytskie obiekty w java dziedzicza po Object !!!

obiekty nie sa rowne poniewaz zajmuja zupelnie inne miejsce w pamieci


dodatkowe zmiene w konstruktorze dopiero po super()

wrzystki dane liczbowe rymitywne sa domyslnie 0
zienne lokalne uzywa sie int a w obiektach uzywa sie Integer


jezlei pole jest private to nie ma dostepu do niego w parencie czy dziedziczeniu

jezeli zrobimy pole protected to bedzie dostepne w kazdym pokoleniu, protekted jest widoczne wewnatrz naszego obiektu


przyslanianie > w klasie ktora dzidziczy metody nadpisujemy je / przysłaniamy poprzez identyczna nazwe metody i parametrow
to jest doprecyzowywanie metod w danej klasie

referencja - sposubb przekazywania poprzez adres w oamieci >> wskaznik
a przy typach prymitywnych wartosc przekazujemy
