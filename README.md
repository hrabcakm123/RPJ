## *SYSTÉM NA SPRÁVU UČEBNÝCH MATERIÁLOV ŠKOLY*

***Podrobnejšiu dokumentáciu projektu je možné nájsť pod názvom "RPJ_dokumentacia_Hrabcak_Demcak_4SB.pdf" v priečinku "Dokumentacia".***


#### Anotácia

> Táto práca slúži ako centrálne úložisko materiálov pre študentov a učiteľov školy. Poskytuje priestor pre nahrávanie súborov, ich sťahovanie a mazanie. Taktiež tento systém vie spravovať tieto materiály a nastavovať prístup k materiálom podľa roly užívateľa.
>
> Systém pracuje s databázou, kde sa dá nahrať celá hierarchia školy, učitelia, študenti, triedy, predmety, materiály a pod. Za ich správu je zodpovedný školský administrátor s prislúchajúcimi prístupovými právami. Aplikácie sú užívateľsky prívetivé a intuitívne. Databáza je zdieľaná medzi všetkými podporovanými aplikáciami, je vytvorená v jazyku MySQL vo vývojovom prostredí MySQL Workbench a nahratá na XAMPP serveri pomocou webovej aplikácie pre správu databáz phpMyAdmin.
>
> Systém pozostáva z troch aplikácií (webová, desktopová a mobilná). Webová aplikácia je vytvorená pomocou HTML, CSS, JavaScript a PHP v aplikácii PhpStorm a poskytuje možnosť úplnej správy systému administrátorom. Spolu s desktopovou aplikáciou umožňuje prihlásenie sa učiteľov, ktorí môžu spravovať nimi vytvorené materiály pre študentov, ktorých učia a prihlásenie sa študentov, ktorí si tieto materiály vedia prezerať a sťahovať. Každý učiteľ a študent má prístupný svoj vlastný ToDoList, kde si môže zaznamenávať svoje povinnosti.
>
> Desktopová aplikácia je zakonštruovaná v jazyku Java pre Model a Controller a FXML pre View. Ponúka možnosť kompletnej správy školy.
>
> Nakoniec mobilná aplikácia, zostrojená vo vývojovom prostredí Android Studio, v jazyku Java pre Model a Controller a XML pre View, umožňuje prihlásenie sa študentom, prezeranie si vytvorených štruktúr ich učiteľmi a správu vlastného ToDoListu.


#### Databáza

- Základ projektu, úložisko dát
- Je zložená z 15 tabuliek, rozdelená do 4 sekcií:
	1. sekcia: Informácie o účtoch (login, heslo, typ účtu)
	2. sekcia: Administrátorský panel a všetky informácie o škole
	3. sekcia: Ukladanie informácií o témach, podtémach a súboroch
	4. sekcia: Zabezpečenie ukladania dát do ToDoListu

**Použité technológie:**
- MySQL
- MySQL Workbench

**Tabuľky databázy:**
- Účet
- Administrátor
- Učiteľ
- Študent
- Škola
- Odbor
- Ročník
- Trieda
- Skupina
- Predmet
- Učiteľ_Predmet_Trieda
- Téma
- Podtéma
- Súbory
- ToDoList

**ER diagram:**

![1](README_Obrazky/1.png)


#### Desktopová aplikácia

- Ponúka plnú správu školy pomocou administrátorského panela
- Prihlasovanie učiteľov a študentov
- Učitelia môžu vytvárať témy, podtémy a súbory pre žiakov, ktorí si ich po zverejnení môžu prezerať a sťahovať súbory
- Každý z týchto účtov má aj svoj ToDoList

**Použité technológie:**
- IntelliJ IDEA
- Architektúra MVC
- Java (Model a Controller)
- FXML (View) – Scene Builder

**Časti:**
- Prihlasovací panel
- Panely pre obnovu hesla
- Panel pre školského administrátora
- Učiteľský panel
- Študentský panel

**Súborova štruktúra:**

![2](README_Obrazky/2.png)

**Prihlasovací panel:**

![3](README_Obrazky/3.png)

**Panely pre obnovu hesla:**

![4](README_Obrazky/4.png)
![5](README_Obrazky/5.png)
![6](README_Obrazky/6.png)

**Panely pre obnovu hesla - video:**

![1-video](https://raw.githubusercontent.com/hrabcakm123/RPJ/main/README_Videa/1.mp4)

**Administrátorský panel:**

![7](README_Obrazky/7.png)
![8](README_Obrazky/8.png)
![9](README_Obrazky/9.png)

**Administrátorský panel - všetky karty - video:**

![2-video](https://raw.githubusercontent.com/hrabcakm123/RPJ/main/README_Videa/2.mp4)

**Administrátorský panel - pridávanie učiteľa a študenta + odosielanie informačného emailu - video:**

![3-video](https://raw.githubusercontent.com/hrabcakm123/RPJ/main/README_Videa/3.mp4)

**Učiteľský panel:**

![10](README_Obrazky/10.png)
![11](README_Obrazky/11.png)
![12](README_Obrazky/12.png)
![13](README_Obrazky/13.png)

**Učiteľský panel - video:**

![4-video](https://raw.githubusercontent.com/hrabcakm123/RPJ/main/README_Videa/4.mp4)

**Študentský panel:**

![14](README_Obrazky/14.png)
![15](README_Obrazky/15.png)

**Študentský panel - video:**

![5-video](https://raw.githubusercontent.com/hrabcakm123/RPJ/main/README_Videa/5.mp4)


#### Mobilná aplikácia

- Len pre študentov
- MVC architektúra
- Android Studio
- Java (Model a Controller)
- XML (View)
- Študenti si môžu prezerať témy, podtémy a sťahovať súbory, ktoré im zverejní učieľ
- ToDoList

**Časti:**
- Prihlasovací panel
- Panely pre obnovu hesla
- Študentský panel

**Súborová štruktúra:**

![16](README_Obrazky/16.png)

**Prihlasovací panel:**

![17](README_Obrazky/17.png)

**Panely pre obnovu hesla:**

![18](README_Obrazky/18.png)
![19](README_Obrazky/19.png)
![20](README_Obrazky/20.png)

**Študentský panel:**

![21](README_Obrazky/21.png)
![22](README_Obrazky/22.png)
![23](README_Obrazky/23.png)
![24](README_Obrazky/24.png)

**Karta "Menu":**

![25](README_Obrazky/25.png)

**Karta "ToDo List":**

![26](README_Obrazky/26.png)
![27](README_Obrazky/27.png)
![28](README_Obrazky/28.png)

**Mobilná aplikácia - video:**

![6-video](https://raw.githubusercontent.com/hrabcakm123/RPJ/main/README_Videa/6.mp4)


#### Webová aplikácia

- Kompletná administrácia celého systému
- Administrátor systému vie pridávať a spravovať školy
- Školský administrátor vie spravovať svoju školu
- Učitelia vedia pridávať, mazať a zdieľať učebné materiály
- Študenti si môžu prezerať témy, podtémy a sťahovať súbory, ktoré im zverejní učiťeľ
- ToDoList

**Použité technológie:**
-  MVC architektúra
- PhpStorm
- PHP
- jQuery a AJAX

**Časti:**
- Prihlasovací panel
- Panely pre obnovu hesla
- Panel pre administrátora systému (pridanie školy, správa škôl)
- Panel pre školského administrátora
- Učiteľský panel
- Študentský panel

**Súborová štruktúra:**

![29](README_Obrazky/29.png)

**Prihlasovací panel:**

![30](README_Obrazky/30.png)

**Registrácia školy:**

![31](README_Obrazky/31.png)

**Panely pre obnovu hesla:**

![32](README_Obrazky/32.png)
![33](README_Obrazky/33.png)
![34](README_Obrazky/34.png)

**Administrátorský panel - pridanie školy:**

![35](README_Obrazky/35.png)

**Administrátorský panel - správa škôl:**

![36](README_Obrazky/36.png)

**Administrátorský panel - správa školy:**

![37](README_Obrazky/37.png)

**Administrátorský panel školy:**

![38](README_Obrazky/38.png)

**Učiteľský panel:**

![39](README_Obrazky/39.png)

**Študentský panel:**

![40](README_Obrazky/40.png)

**Koniec ...**
