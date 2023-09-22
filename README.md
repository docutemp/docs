# docs.docutemp.com

### Rozwiązanie:
+ szyfrowanie i przechowywanie dokumentów projektu w jednym dokumencie html


### Cel:
+ do wymiany danych w formie zaszyfrowanej
+ do realizacja usług w sposób asynchroniczny

  
### Zastosowanie:
+ Wymiana danych z księgowym, faktur, raportów, danych medycznych, pracowników
+ Podpisywanie i monitorowanie realizacji umów asyncrhoczninie (i syncrhonicznie na serwerze)
+ Archiwizajca danych, np. przenoszenie między PC i USB danych w formie zaszyfrowanej
+ mozliwosc korzystania z mniej bezpiecznych kanalow komunikacji wysyłając dane wrażliwe w postaci zaszyfrowanej

  
### Korzyści
+ jeden przenośny dokument jako portfel dla wielu dokumentów
+ bez centralnego serwera przechowującego dane i hasła
+ Kontrola zmian, danych
+ działa na każdego platformie i przeglądarce
+ edycja danych bezpośrednio w przeglądarce internetowej bez zewnętrznej aplikacji

  
### Specyfikacja:

+ dokument w formacie HTML, dlatego nie wymaga zewnętrznej aplikacji
+ aktywne elementy i szyfrowanie obsługiwane po stronie przeglądarki w języku JavaScript
+ możliwość synchronizacji z zewnętrznymi i lokalnymi usługami na serwerze, komputerze użytkownik, np. w celu aktualizacji statusu kontraktu
+ możliwość załączenia i uruchomienia w komunikatorze do przeglądu lub edycji w prywatnym oknie




## Bezpieczna wymiana dokumentów

Szyfrowanie kanałów komunikacji to minimum do którego przywykliśmy.
Niestety nie zawsze to wystarczy, zwłaszcza gdy możemy stać się ofiarą luki w oprogramowaniu, np. backdoory czy ciągłej infiltracji ze strony rządu polegającej na archiwizownaiu wiadomości przez providerów usług komunikacji.

Przechowywanie danych na prywatnym urządzeniu pc, smartphone czy pendrive z podaniem hasła dostępu do całego systemu czy dysku może nie być wystarczające, jeśli dostęp do urządzenia ma strona trzecia poprzez celowo pozostawione luki w systemie.

To co może pomóc w takich skrajnych, ale zdarzających się sytuacjach, to pozostawianie danych w formie zaszyfrowanej na dysku, nawet wtedy gdy system jest zabezpieczony hasłem.

W sytuacji zagrożenia życia, takie różnice pomagają w zachowaniu życiua swojego i innych osób narażonych na wyciek danych.

Na co dzień jednak nie chcemy aby the luki bezpieczeństwa pozwalałby na dostęp konkurencji, czy grup posuwających się do przestępstwa i łamania tajemnicy korespondencji gwarantowanej nam w konstytucji.


## Oferta

FinOfficer to narzędzie do transparentnej dla obu stron komunikacji a zarazem szyfrowanej dla osób postronnych.
Komunikacja może odbywać się za pomocą dowolnego medium, ale sama treść wiadomości i załączników może zostać zaszyfrowana.

Taka forma komunikacja wymaga prostego narzędzia dlatego korzystamy z narzędzia DocuTemp do tworzenia dokumentów w locie z szyfrowaniem.
   
Plik który przesyłamy w koresponendcji jest formacie HTML a do otwarcia wymaga tylko przeglądarki i hasła, po  realizacji zdalnych usług


+ Szyfrowanie to tylko warstwa niezalezna od kanalu komunikacji
+ Plik HTML to typ MIME multipart z plikami wbudowanymi do html


## Zastosowanie

+ tworzenie umów pod customizowane pod klienta usługi online/offline
+ Wbudowana checklista kolejnych kroków, potwierdzanych przez zlecającego wykonanie usług
+ Potem edycja i ponowne zapisanie, zaszyfrowanie i wyslanie zmian
+ Możliwość przechowywania zaszyfrowanego pliku w jednorazowym sejfie

HTML multipart zawiera wbudowanych w html dowolne pliki projektu potrzebnego do realizacji usługi: png, doc, png, md, ...

Chodzi o to by na dysku nie bylo sladu po sourcode, zeby te wazne pliki byly wbudowane wewnatrz html w sposob zaszyfrowany i tylko otworzenie dokumentu w przegladarce pozwoli na zobaczenie co tam jest po podaniu hasla
Taki dokument zaszyfrowany html ma miec tez niezaszyfrowane dane jak status do umowy
Czyli Ty mi wysylasz zlecenie, umowe w formacie html z checklista, ja odbieram i poprzrz wygenerowany klucz otwieram dodaje pliki poprzez funcke upload i wysylam Tobie zaznaczajac zmiane statusu i rozpoczecie kolejnego etapu
Ty odbierasz html z zalacznikami w nim i po otrzymaniu klucza otwierasz i potwierdzasz lub nie ten etap, zalaczasz jakies wskazowki i plik znowu wraca do mnie, na koniec jak wszystkie checkbosy statusu zlecenia beda zaznaczone i potwierdzone jako zweryfikowane automatycznie wysylasz kase z depozytu
Chodzi o to by kontrolowac przebieg prac nad projektem i nie zmieniac kryteriow wykonania w trakcie, aby byla to transparenta umowa dla obu stron
Ta checklista aktualnie zapisuje sie w cookies i jesli jest dostepny na zdalnym serwerze, ale sam dokument nie jest przechowywany na serwerze
Jedynie template
A co pomiedzy sie w nim zmiesci nie jest nikomu znane Oprocz dwom stronom umowy

# Use Case

## Kontrakt

Chodzi o mozliwosc korzystania z mniej bezpiecznych komunikacji informacji do celow zawierania umów i rozliczania, bez udzialu strony trzeciej, ktora udostepnia templates i hash do aktualizacji statusu, bez ktorego nie mozna samowolnie przejsc do nastepnego etapu
Osoba ktore zleca odpowiada za weryfikacje prac dlatego ona potwierdza checkliste i decyduje o wyplacie dlatego mozna tez zrobic umowe z wyplata zaliczek po zmianie kolejnych statusow
W tej chwili zakladam dwie strony umowy ale moze bedzie potrzebna rozbudowa
To moze dzialac online ale w skrajnosci musi byc mozliwosc pracowania na pliku offline bez dostepu do danych na urzadzeniu

## Fiverr

Korzystam z fiverr i tam jest chat, ja bym chcial aby to bylo w formie offline bez chatu a po prostu spakowana paczka na wszystko co da sie zdalnie wykonac

## Księgowość, wymiana dokumentów

To samo z moim ksiegowym
Nie chce by posiadal moje dokumenty na dysku w formie niezaszyfrowanej
Dlatego chce mu wysylac taka paczke do pobrania np z jednorazowego linku
Żebym tez mial informacje czy pobral w statusie dokumentu jaki mam u siebie
Wiec jesli bede chcial mu wyslac wiele dokumentow to bedzie mogl sobie to pobrac z linku i otworzyc na kompie a potem pokasować jak juz wprowadzi do systemu
Bo jak widze z jakich oni korzystaja klientow poczty
Np. o2, wp,...


## Usługa Sejf

+ Możliwość przechowywania zaszyfrowanego pliku w jednorazowym sejfie
to znaczy, że można zaszyfrowany dokument upload-ować aby druga osoba po podaniu hasła mogła go pobrać
Skrytka w tym momencie zostaje usunięta z serwera.
a dokument pozostaje u nadającego i odbierającego.
Nikt inny nie ma dostępu, nawet po włamaniu na komputer w trakcie działania przeglądarki plik pozostaje zaszyfrowany, a hasło do otworzenia posiadają dwie strony kontraktu
