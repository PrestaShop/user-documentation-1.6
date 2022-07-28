# Uwagi ogólne

## Uwagi ogólne <a href="#uwagiogolne-uwagiogolne" id="uwagiogolne-uwagiogolne"></a>

W celu uniknięcia nieporozumień odnośnie zarządzania zapasami w wersji 1.4 a możliwością zaawansowanego zarządzania magazynami, którą proponuje wersja 1.5 koniecznym staje się przedstawienie dwóch odrębnych pojęć jakimi są zapasy fizyczne i ilości produktów dostępnych do sprzedaży.

### Ilości produktów dostępnych do sprzedaży <a href="#uwagiogolne-ilosciproduktowdostepnychdosprzedazy" id="uwagiogolne-ilosciproduktowdostepnychdosprzedazy"></a>

Odnosi się to do zarządzania zapasami w PrestaShop 1.4.x. Chodzi o ilości, które są wyświetlane w sklepie dla każdego produktu i odmian produktu. Jest to ilość, która definiuje czy dany produkt może zostać zamówiony lub nie (chyba, że opcja "Zezwól na zamawianie produktów, których nie ma na stanie" jest aktywowana). Ta opcja może być zdefiniowana ręcznie dla każdego produktu i każdej odmiany produktu.

W PrestaShop 1.5.x ilość produktów dostępnych do sprzedaży może zostać automatycznie zdefiniowana w zależności od rzeczywistych zapasów danego produktu. W przypadku posiadania wielu sklepów ilość ta musi zostać zdefiniowana dla każdego z nich.

W rezultacie to co w wersji PrestaShop 1.4.x nazywaliśmy “magazynem” w wersji PrestaShop 1.5.x. zostało nazwane “Ilością produktów dostępnych do sprzedaży”.

### Produkty magazynowane (fizycznie przechowywane) <a href="#uwagiogolne-produktymagazynowane-fizycznieprzechowywane" id="uwagiogolne-produktymagazynowane-fizycznieprzechowywane"></a>

Odnosi się to do zarządzania produktami fizycznie magazynowanymi w jednym lub w wielu miejscach. Po wprowadzeniu tej nowej funkcji do PrestaShop 1.5.x nosi ona nazwę "Magazyn".

Nowe zarządzanie magazynami uwzględnia ruch magazynowy, aktualne pokrycie stanu, stany magazynowe, integrację z trybem “Multisklep” oraz dostawę zamówień.

Nowe zarządzanie magazynami umożliwia również uwzględnienie pojęcia rzeczywistego magazynu. W określonym czasie dany produkt może być dostępny w magazynie fizycznym, lecz niedostępny w sprzedaży z racji dokonanych zamówień (oczekujących już na przesyłkę). Ten sam produkt może również stanowić przedmiot dostawy zamówienia (innymi słowy być w trakcie realizacji dostawy), a zatem produkt ten nie został jeszcze odnotowanym w magazynie fizycznym.

Magazyn rzeczywisty składa się z zapasów fizycznie obecnych w składzie (magazynie fizycznym), do których dodajemy ilość produktów obecnie zamówioną u dostawcy, oraz od której odejmujemy ilość produktów aktualnie zamówionych przez klientów, lecz jeszcze nie wysłanych.

## Korzystanie z nowego zarządzania magazynem <a href="#uwagiogolne-korzystanieznowegozarzadzaniamagazynem" id="uwagiogolne-korzystanieznowegozarzadzaniamagazynem"></a>

### Czy korzystanie z nowego zarządzania magazynem jest obowiązkowe? <a href="#uwagiogolne-czykorzystanieznowegozarzadzaniamagazynemjestobowiazkowe" id="uwagiogolne-czykorzystanieznowegozarzadzaniamagazynemjestobowiazkowe"></a>

Zarówno korzystanie z nowego zarządzania magazynem jak i zarządzania liczbą produktów dostępnych do sprzedaży nie jest obowiązkowe.

Aktywacja zarządzania ilościami dostępnymi do sprzedaży oraz zarządzania magazynem znajduje się w ustawieniach strony “Produkty”. Przewiń w dół do sekcji "Stan Produktów” i wybierz "Tak" dla dwóch opcji zarządzania magazynem. Aby móc aktywować zaawansowane zarządzanie zapasami najpierw musisz aktywować zarządzanie magazynem.

Zarówno Zaawansowana funkcja zarządzania magazynem, jak i standardowa oraz Twoje magazyny są niezależne od funkcji Multistore. W związku z tym, bez względu na to, którym sklepem zarządzasz z poziomu back-office PrestaShop używając menu “Magazyn” zawsze zarządzasz zapasami w sposób globalny.

### Jak nie dokonywać żadnych zmian na PrestaShop 1.4.x/1.5.x ? Co powinienem zrobić? <a href="#uwagiogolne-jakniedokonywaczadnychzmiannaprestashop1.4.x-1.5.x-copowinienemzrobic" id="uwagiogolne-jakniedokonywaczadnychzmiannaprestashop1.4.x-1.5.x-copowinienemzrobic"></a>

Jeśli nie chcesz skorzystać z zaawansowanego zarządzania zapasami w PrestaShop 1.5 i chcesz pozostać przy “klasycznym” funkcjonowaniu zarządzania ilością produktów, z którego jesteś w pełni zadowolony przejdź do strony preferencji “Produkty”. Następnie przewiń aż do sekcji “Stan Produktów” i wybierz “Tak” dla opcji “Włącz zarządzanie magazynem” oraz pozostaw “Nie” przy opcji “Włącz zaawansowane zarządzanie magazynem”.

Funkcja “Ilości dostępnych do sprzedaży” jest od tej pory scentralizowana w zakładce “Ilości” w karcie produktu: stwórz nowy produkt lub edytuj już istniejący. Zakładka pojawia się pomiędzy innymi po lewej stronie ekranu.

### Czy nowe zarządzanie magazynami znajdzie zastosowanie w moim przypadku? <a href="#uwagiogolne-czynowezarzadzaniemagazynamiznajdziezastosowaniewmoimprzypadku" id="uwagiogolne-czynowezarzadzaniemagazynamiznajdziezastosowaniewmoimprzypadku"></a>

Nowe zarządzanie magazynem pozwala na zarządzanie w sposób zaawansowany. Ta funkcjonalność ma zastosowanie jeśli:

* Zarządzasz magazynem z produktami w sprzedaży w Twoim sklepie/sklepach.
* Korzystasz przynajmniej z jednego miejsca (składu lub hurtowni), którym zarządzasz samodzielnie.
* Zamawiasz część lub wszystkie produkty u jednego lub wielu dostawców.
* Potrzebujesz statystyk dotyczących stanu Twojego magazynu lub hurtowni.

Ta funkcjonalność nie znajdzie zastosowania w przypadku, gdy:

* Nie zarządzasz magazynem z produktami w sprzedaży w Twoim sklepie/sklepach.
* Posiadasz już system zarządzający magazynem i chcesz z niego nadal korzystać bez dokonywania zmian.
