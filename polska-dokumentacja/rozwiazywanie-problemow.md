# Rozwiązywanie problemów

**Spis treści**

* [Rozwiązywanie problemów](rozwiazywanie-problemow.md#Rozwiązywanieproblemów-Rozwiązywanieproblemów)
  * [Wyłączanie komunikatu o błędach wyświetlania w przypadku nieoczekiwanych pustych stron](rozwiazywanie-problemow.md#Rozwiązywanieproblemów-Wyłączaniekomunikatuobłędachwyświetlaniawprzypadkunieoczekiwanychpustychstron)
  * [Hostowanie na1&1: Rozwiązywanie problemu pamięci alokacji](rozwiazywanie-problemow.md#Rozwiązywanieproblemów-Hostowaniena1&1:Rozwiązywanieproblemupamięcialokacji)
  * [Jest niemożliwe aby podłączyć więcej](rozwiazywanie-problemow.md#Rozwiązywanieproblemów-Jestniemożliweabypodłączyćwięcej)
  * [Regeneracja hasła ręcznie](rozwiazywanie-problemow.md#Rozwiązywanieproblemów-Regeneracjahasłaręcznie)
  * [PrestaShop nie wysyła mi mojego nowego hasła](rozwiazywanie-problemow.md#Rozwiązywanieproblemów-PrestaShopniewysyłamimojegonowegohasła)
  * [Omyłkowe usunięcie domyślnego pakietu językowego po zalogowaniu](rozwiazywanie-problemow.md#Rozwiązywanieproblemów-Omyłkoweusunięciedomyślnegopakietujęzykowegopozalogowaniu)

## Rozwiązywanie problemów <a href="#rozwiazywanieproblemow-rozwiazywanieproblemow" id="rozwiazywanieproblemow-rozwiazywanieproblemow"></a>

### Wyłączanie komunikatu o błędach wyświetlania w przypadku nieoczekiwanych pustych stron <a href="#rozwiazywanieproblemow-wylaczaniekomunikatuobledachwyswietlaniawprzypadkunieoczekiwanychpustychstron" id="rozwiazywanieproblemow-wylaczaniekomunikatuobledachwyswietlaniawprzypadkunieoczekiwanychpustychstron"></a>

Module

Dla PrestaShop 1.6 i wyższych możesz użyć modułu: [https://www.prestashop.com/forums/index.php?setlanguage=1\&cal\_id=\&langid=11\&k=880ea6a14ea49e853634fbdc5015a024](https://www.prestashop.com/forums/index.php?setlanguage=1\&cal\_id=\&langid=11\&k=880ea6a14ea49e853634fbdc5015a024)

Jeśli panel administracyjny i/albo strona główna wyświetla regulanie pustą albo niekompletną stronę bez żadnego komunikatu o błędzie. Koniecznie jest włączenie wyświetlania błędów PHP w celu zrozumienia problemu.

Odbywa się to w pliku instalacji PrestaShop `/config/defines.inc.php`.  Należy zmodyfikować nastepującą linię:

```
define('_PS_MODE_DEV_', false);
```

...i zmienić na:

```
define('_PS_MODE_DEV_', true);
```

Przejrzyj swoją stronę sklepu ponownie. PrestaShop wyświetli wszystkie komunikaty o błędach (jeśli są jakieś), co powinno pomóc w rozwiązaniu problemu.

Gdy problem został rozwiązany, należy cofnąc wprowadzone zmiany, edytuj plik `/config/defines.inc.php` jeszcze raz i umieść wstecz fałszywą wartośc `_PS_MODE_DEV_` constant.

### Hostowanie na1&1: Rozwiązywanie problemu pamięci alokacji <a href="#rozwiazywanieproblemow-hostowaniena1-and-1-rozwiazywanieproblemupamiecialokacji" id="rozwiazywanieproblemow-hostowaniena1-and-1-rozwiazywanieproblemupamiecialokacji"></a>

Niektórzy ludzie mogą napotkać problemy z alokacją pamięci, zwłaszcza gdy panel administracyjny próbuje wyświetlić obrazy na dysku które są całkiem duże (ponad 800 Kb). Powinieneś wiedzieć, że nawet jeśli ręcznie zwiększysz limit pamięci hostingu do 128 Mb, to niektóre hostingi, takie jak 1&1, będą ograniczone do limitu 32 Mb. Zobacz sekcje FAQ od 1&1:[http://faq.oneandone.co.uk/scripting/php/10.html](http://faq.oneandone.co.uk/scripting/php/10.html).

Są tylko dwa rozwiązania, i obydwa są drastyczne:

* Zmniejsz rozmiar pikseli swoich zdjęć, i zmniejsz ich rozmiar na dysku. To powinno także prawdopodobnie poprawić ogólną wydajność.
* Zmień hosting na taki który obsługuje rozszerzenie pamięci.

### Jest niemożliwe aby podłączyć więcej <a href="#rozwiazywanieproblemow-jestniemozliweabypodlaczycwiecej" id="rozwiazywanieproblemow-jestniemozliweabypodlaczycwiecej"></a>

Istnieją przypadki kiedy PrestaShop nie rozpozna e-maila albo hasła użytkownika, co uniemożliwia podłączenie zarówno panelu administracyjnego jak i strony głównej. Użytkownik jest odesłany do widoku logowania. Niektóre raporty wskazują na to, że IE10 jest jedyną przeglądarką w której się to dzieje.

To jest najprawdopodobnie problem z plikami cookies w przeglądarce użytkownika sklepu: gdy użytkownik loguje się wielokrotnie w sklepie, klucze szyfrowania plików cookies mogą się mieszać.

W każdym razie jest, jeden prosty sposób żeby rozwiązać ten problem i aby się ponownie zalogować, jest to wyczyszczenie pamici podręcznej i plików cookies. Oto strona która wyjaśnia jak to zrobić, w zależności od przeglądarki: [https://support.google.com/accounts/answer/32050?hl=pl\&rd=1](https://support.google.com/accounts/answer/32050?hl=pl\&rd=1).

### Regeneracja hasła ręcznie <a href="#rozwiazywanieproblemow-regeneracjahaslarecznie" id="rozwiazywanieproblemow-regeneracjahaslarecznie"></a>

Są sytuacje kiedy nic się nie dzieje, kiedy poprosisz o nowe hasło, i to nie działa. Może być wiele powodów dla których się to stało , ale ważne jest, aby być sie w stanie zalogować ponownie.

To będzie wymagało uzyskania dostepu do bazy używając na przykład phpMyAdmin.

Będziesz musiał wykonać nastepującą procedurę:

1. Otwórz plik `/config/settings.inc.php`, bezpośrednio z root twojego sklepu. Znajdź linię zawierającą "`_COOKIE_KEY`\_". Skopiuj zawartość pliku cookie (bez cudzysłowiów): To jest MD5 do twojego orginalnego hasła.
2. Teraz trzeba wygenerować dla hasła nowy hash MD5.\

   1. Przejdź do [http://www.miraclesalad.com/webtools/md5.php](http://www.miraclesalad.com/webtools/md5.php).
   2. Wklej wartość "`_COOKIE_KEY`\_" w polu tekstowym, a zaraz po nim, dodaj żądane hasło. Na przykład. xykxB41JrEacRIoZxDioPNRmKeuO3ixCLygNxBAkeOkAHf2YUVESuT9jMYPASSWORD, gdzie pliki cookie kończy się T9j, a pożądane hasło to MYPASSWORD (to może być wszystko co chcesz)
   3. Kliknij przycisk "md5": to stworzy MD5 hash zawartości tekstowej pola. Skopiuj go.
3. Teraz należy przenieść ten hash do bazy danych: You now need to put this hash into your database:
   1. Otwórz bazę danych swojego sklepu używając phpMyAdmin. Jeśli nie wiesz jak użyć phpMyAdmin, zapytaj swojego webmastera, albo swojego dostawcę hostingu.
   2. Otwórz tabele `pw_employee`, znajdź wiersz odpowiadający twojemu kontu (powinien odpowiadać twojemu mieniu, nazwisku i adresowi e-mail) i kliknij przycisk "Edytuj".
   3. Znajdź pole `passwd`, i wklej w MD5 który właśnie wygenerowałeś.
4. Zaloguj się ponownie do swojego panelu adminstracyjnego z listy e-mail w tej samej tabeli, a następnie na żądane hasło które zostało użyte (MYPASSWORD). To wygeneruje nowy klucz plików cookie.

Jeśli to nadal nie działa, użyj phpMyAdmin do dostepu tabeli  `ps_shop_url` i sprawdź wartość głównego sklepu które jest `id` 1. Powinna ona zawierać ścieżkę do pliku sklepu:

* Jeśli twój sklep jest na root serwera, to ta zmienna powinna zawierać "`/`".
* Jeśli twój sklep jest na podkatalogu, Powinien zawierać Na przykład, tak jest w  "[http://www.mywebsite/shop/](http://www.mywebsite/shop/)", następnie zmienna powinna zawierać "/shop/".

Jeśli wszystko zawiedzie skontaktuj się z zespołem wsparcia PrestaShop na [http://addons.prestashop.com/pl/35-wsparcie](http://addons.prestashop.com/pl/35-wsparcie).

### PrestaShop nie wysyła mi mojego nowego hasła <a href="#rozwiazywanieproblemow-prestashopniewysylamimojegonowegohasla" id="rozwiazywanieproblemow-prestashopniewysylamimojegonowegohasla"></a>

Żądanie aby zresetować hasło działa tylko wtedy jeśli serwer SMTP został skonfigurowany tak, że to PrestaShop jest wstanie wysyłać emaile.

Są zaprezetowane Tobie dwa rozwiązania:

1. **Skonfigurować serwer SMTP do wysyłania emaili:**\

   1. Zdobądź informacje od swojego dostawcy hostingu na temat połączeń SMTP
   2. Przejdź do swojego panelu administracyjnego (użykownik albo adminstrator który nadal jest zalogowany) Strona "E-maile" w menu "Parametry zaawansowane".
   3. Wybierz opcje "Użyj moich własnych ustawień SMTP". Pojawi się formularz: wypełnij go informacjami podanymi przez twój hosting.
   4. Zachowaj swoje zmiany.
   5. Poproś o nowe hasło ponownie Należy je zachować.
2. **Postepuj zgodnie z krokami:**\

   1. Wybierz nowe hasło. W naszym przykładzie, "\$$$rabbit$159\$$$".
   2. Użyj swojego FTP, otwórz plik `login.php`, zlokalizowany w folderze adminstracyjnym online (nazwa zależy od twojej instalacji).\
      &#x20;Na dole pliku, dodaj nastepującą linię:\
      &#x20;`echo md5( PSQL( _COOKIE_KEY_ . 'newpassword' ) );`\
      &#x20;Tak więc nasze przykładowe hasło:\
      &#x20;`echo md5( PSQL( _COOKIE_KEY_ . '$$$rabbit$159$$$' ) );`\
      &#x20;Pamiętaj aby umieścić swoje nowe hasło!
3. Przejdź do strony logowania w panelu administracyjnym, jeśli chcesz się zalogować, i skopiować tekst który się pojawia na dole strony (np: a0ee884b507dd4624ce51968cfbb19a9).
4. Przejdź do bazy danych PrestaShop, na przykład używając phpMyAdmin. W tabeli `ps_employee`, zastąp istniejącą wartość w kolumnie `passwd` dla pracownika któremu chcesz zmienić hasło z wartością otrzymaną w poprzednim kroku. Zachowaj zmiany.
5. Teraz można połączyć się zwykłym loginem i nowym hasłem.

### Omyłkowe usunięcie domyślnego pakietu językowego po zalogowaniu <a href="#rozwiazywanieproblemow-omylkoweusunieciedomyslnegopakietujezykowegopozalogowaniu" id="rozwiazywanieproblemow-omylkoweusunieciedomyslnegopakietujezykowegopozalogowaniu"></a>

W przypadku gdy usunięto przy instalacji domyślny pakiet językowy ze swojego sklepu, możesz mieć problemy z ponownym połączeniem z panelem adminstracyjnym.

Oto jak rozwiązać ten problem jeśli domyślnym językiem był angielski:

1. Przejdź do phpMyAdmin. Jeśli nie można uzyskac do niego dostępu, należy zwrócić się do swojego dostawcy hostingu aby wykonał tą czynność.
2. Wybierz bazę danych swojego sklepu, i wybierz tabelę `ps_lang`.
3. Kliknij przycisk "Wstaw" na górze, i utwórz nowy wpis z tych wartości:
   * `id_lang` -> 1
   * ```
     name -> english
     ```
   * `active` -> 1
   * `iso_code` -> en
   * `language_code` -> en
   * `date_format_lite` -> Y-m-d
   * `date_format_full` -> Y-m-d H:i:s
   * `is_rtl` -> 0
4. Wykonaj kwerendę.

Powinieneś być w stanie zalogować się jeszcze raz.
