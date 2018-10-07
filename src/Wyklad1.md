# Organizacyjnie
* 2 kolokwia po 15 punktow
* zadanie domowe po punkcie, razem 15
* egzamin pisemny pozwala potencjalnie uzupełnić punkty
* dalej egzamin ustny
* "dobrze jest mieć (na ustnym) 45 punktów, polecam państwu, wtedy nasza rozmowa staje się coraz przyjemniejsza"

Konsultacje - pokój 527 czwartki 14:00-15:30

## Literatura
1. Nieśmiertelny Landau Lifszyc, Fizyka Statystyczna
2. Nieśmiertelny Huang - Statistical Mechanics
3. M. Kardar, dwa tomy, I + II, będzie w tytule coś statystycznego na pewno
4. F. Schwabl
5. R. Pathna
6. Callen - termodynamika

# Termodynamika

Makroskopowy opis makroskopowych obiektów makroskopowymi parametrami w *stanach równowagi*

* $d/dt = 0$
* brak systematycznych przepływów

Z doświadczeń wiemy, że do stanów równowagi wystarczy kilka makroskopowych parametrów.  
Dla *prostych* (jednorodnych, izotropowych, bez własności elektrycznych i magnetycznych, bez reakcji) układów termodynamicznych wystarczą:

* Energia wewnętrzna $U$
* Objętość $V$
* Liczba cząstek danego składnika $N_i$

Mamy układ, który oddziałowuje przez **ścianki** wyodrębniające go ze świata i ustalające, jakie oddziaływania są dozwolone.

* Dla oddziaływań materialnych mamy ścianki
    * przepuszczalne (układ otwarty)
    * półprzepuszczalne (w przypadku wielu składników, przepuszczają niektóre)
    * nieprzepuszczalne (układ zamknięty - na tych się skupimy - stała ilość materii w układzie)
* Dla oddziaływań mechanicznych (układ wymienia energię z otoczeniem przez **mierzalną** pracę mechaniczną)
    * Jakbyśmy mieli np. dipole magnetyczne, praca byłaby też przy magnetyzacji składników - zakładamy że jest kontrolowalna
    * Na razie założymy, że uwzględniamy jedynie zmianę objętości
* Dla oddziaływań termicznych mamy ścianki
    * adiabatyczne - dające jedynie oddziaływania mechaniczne
    * diatermiczne - przepuszczające jakieś "ciepło"

## Zerowa zasada termodynamiki

**Wzajemna równowaga termiczna** - jeśli z termodynamicznie równowagowych ciał (A, B, C) (A, B) są w
równowadze i (B, C) są w równowadze przy oddziaływaniu przez nieruchomą,
nieprzepuszczalną, **diatermiczną** ściankę, to (A, C) też są - *przechodniość relacji*.

Istnieje więc równoważność między wszystkimi ciałami w równowadze (należą do
wspólnej "klasy abstrakcji"?) - więc można przyporządkować skalar - temperaturę
empiryczną.

## Pierwsza zasada termodynamiki

"Zasada zachowania energii dla układów termodynamicznych" - ale nie wiemy czym jest ciepło i energia wewnętrzna, więc definiujemy ją tak:

* mamy układ polegający przemianie od stanu równowagi $A \to B$.
* Ścianki są adiabatyczne.

Praca mechaniczna $W^{adiabatyczne}_{A,B}$ zależy *tylko* od stanów $A, B$. Ale jeśli po drodze wstawimy stan $P$:

$$A \to P \to B$$

to

$$ W_{A,B}^{ad} = W_{A,P}^{ad} + W_{P,B}^{ad}$$

Więc istnieje **funkcja stanu** $U$ (**energia wewnętrzna**) zależna od parametrów i definiująca stan układu przez

$$W_{A,P}^{ad} = U_P - U_A$$

A teraz usuwamy założenie o adiabatyczności, układ idzie $a \to b$ po jakiejś
niekoniecznie adiabatycznej drodze z mierzalnym $W_{a,b}$ - ale możemy też przejść po tej
adiabatycznej z $W_{a,b}^ad = U_b - U_a = \Delta U$. Stąd definiujemy
**ciepło** $Q_{a,b} = W_{a,b}^{ad} - W_{a,b} = \delta U - W_{a,b}$ poprzez różnicę prac między dwoma
drogami.

$$ \Delta U = U_b - U_a = Q_{a,b} + W_{a,b} $$

> Z własności z prac dla przejść adiabatycznych wywnioskowujemy istnienie energii wewnętrznej, a z rozluźnienia warunku na przejścia adiabatyczne - ciepło.

## Formy Pfaffa

Dla małych przejść

$$ dU = \dj Q + \dj W $$

Gdzie $ \dj Q , \dj W $ to formy Pfaffa - nie są różniczkami zupełnymi bo zależy od drogi, w przeciwieństwie do $ dU $.

## Procesy kwazistatyczne

Układ przechodzi $a \to b$ przez ciąg stanów równowagi. Hong-Kong przed i po
tajfunie nie przechodzi przez ciąg stanów równowagi, więc to jest mocne
ograniczenie.

Tak naprawdę to jest definicja procesu *pseudostatycznego*.

> Nie chcę tu państwa zamęczać, ale... Chwila udręki...

Kwazistatyczny jest taki, gdzie praca wykonywana nad układem jest wykonywana tylko przez siły zachowujące układ w stanie równowagi.

Przykład - naczynie z wodą i z wiatraczkiem, którym to wiatraczkiem kręcimy
zewnątrz (wykonując pracę mechaniczną). Proces jest pseudostatyczny, bo
działamy wbrew siłom tarcia, które nie utrzymują stanu w równowadze! Raczej
sprowadzają go do niej.

## Zmiana objętości w naczyniu z płynem

Żeby proces był kwazistatyczny, ciśnienie musi być w nim identyczne jak ciśnienie zewnętrzne.  
Ale tak naprawdę nie mamy 
$$ \dj W \neq - p dV $$
, ale $$ \dj W = -p^{zew} dV $$ - siła razy
przesunięcie. I wtedy dopiero z przyrównania ciśnień wychodzi $$ - p dV $$ i to
by była forma Pfaffa, nie ogólna forma różniczkowa. Wstawiając tam bezpośrednio $p^{zew}$ mamy zależność stanu układu z wszechświatem.

I wtedy dopiero mamy znane

$$ dU = \dj Q - p dV $$

$p^{zew}$ zależy od zmiennych innych niż stan układu, ale na przykład humor ściskacza.

Tak naprawdę powinniśmy pisać na ogólne formy różniczkowe zależące od reszty świata

$$ DW = - p^{zew} (\text{nie tylko parametry układu}) $$

W ten sposób mamy formę Pfaffa:

$$ \dj W = -p (\text{tylko od parametrów układu}) $$

## Magnetyki
Dla magnetycznych właściwości mamy całkowity dipolowy moment układu $\vec{M}$,
a zmiana właściwości układu związana z nim to 
$$ DW_{mag} = \vec{B} \cdot \vec{M}$$
gdzie B to indukcja zewnętrznego pola magnetycznego, i trzeba by napisać $DW_{mag}$.
Jakbyśmy wyrazili $\vec{B}$ przez parametry układu (może temperaturę), 

Dla właściwości elektrycznych
$$ DW_{el} = \vec{E} \cdot \vec{P} $$



## Matematycznie formy Pfaffa
Niech $x_1, .... x_n$ - parametry określające stan układu. Wtedy forma Pfaffa to

$$ \Sigma_{i=1}^n X_i(x_1, ..., x_n) dx_i $$

## Druga zasada termodynamiki w duchu neo-gibbsowskim
Istnienie entropii $S = S(U, V, N)$, co do której postulujemy:

> Entropia przybiera wartość maksymalną w stanach równowagowych.

Weźmy układ izolowany złożony z dwóch podukładów. Stan równowagowy zdefiniowany przez ścianki.

Teraz uwalniamy *więzy* - pozwalamy ściance wewnętrznej się ruszać, umożliwiamy
przepływ ciepła... - wtedy układ dąży do nowego stanu równowagi. Jakiego? Na to odpowiada drugi postulat:

> Stan równowagi osiągnięty pod nieobecność więzów maksymalizuje entropię na zbiorze stanów równowagi z więzami (dotyczy układu izolowanego).

1. Układ z więzami. Stan równowagi.
2. Zwalniamy więzy.
3. Pytamy jaki jest stan równowagi teraz?
4. Nowy stan równowagi odpowiada maksymalnej entropii wybranej na wszystkich
możliwych stanach równowagi z więzami. Znajdujemy maksimum entropii, i to nam daje
parametry (U, V, N) stanu układu.

Postulujemy też, że

$$ (\frac{\partial S}{\partial U})_{V, N} > 0 $$

Postulujemy też addytywność entropii - entropia sumy układów jest równa sumie entropii poszczególnych podukładów.


## Temperatura termodynamiczna T

*W wielu wzorach w tym fragmencie N-ek powinno być wiele.*

Bierzemy $S = S(U, V, N_1, ..., N_r)$.

$$ dS = 
 (\frac{\partial S}{\partial U})_{V, N} dU
+ (\frac{\partial S}{\partial V})_{U, N} dV
+ \Sigma_{i=1}^n
 (\frac{\partial S}{\partial N_i})_{U, V, N \neq N_i} dN_i $$

Bierzemy też

$$ dU = 
 (\frac{\partial U}{\partial S})_{V, N} dS
+ (\frac{\partial U}{\partial V})_{S, N} dV
+ \Sigma_{i=1}^n
 (\frac{\partial U}{\partial N_i})_{S, V, N \neq N_i} dN_i $$

To są parametry ekstensywne.  Definiujemy parametry intensywne: 

$$ T =   (\frac{\partial U}{\partial S})_{V, N} $$
$$ p = - (\frac{\partial U}{\partial V})_{S, N} $$
$$ \mu_i =   (\frac{\partial U}{\partial N_i})_{S, V} $$

Więc możemy napisać

$$ dU = T dS - p dV + \Sigma_{i=1}^r \mu_i dN_i $$

W układzie zamkniętym $$ dN_i = 0 $$
więc $$ dU = T dS - p dV $$

Z drugiej strony w procesie kwazistatycznym

 $$ dU = \dj Q + \dj W = \dj Q - p dV $$

Więc

$$ \dj Q = T dS $$

Zatem
$$ dS = \frac{\dj Q}{T} $$
jest różniczką zupełną i funkcją stanu.

> *"Energia wszechświata jest stała; entropia wszechświata osiąga maksimum"* - Clausius z Koszalina, twórca entropii (lubimy go za to)


### Związek podstawowy reprezentacji energii wewnętrznej

$$ U = U(S, V, N) $$
$$ dU = TdS - pdV + \mu dN $$

Możemy też napisać...

### Związek podstawowy reprezentacji entropii
> *Od autora notatek: przechodzę na notację z indeksami bo mam dość - indeks oznacza różniczkowanie, po czym nie różniczkujemy to ustalone.*

$$ S = S(U, V, N) $$


$$ dS = S_U dU + S_V dV + S_N dN $$



$$ S_V = - U_V / U_S = P / T $$


$$ S_N = - U_N / U_S = - \mu / T $$

Warto pamiętać: 

> W wersji z entropią dS parametry intensywne są funkcjami parametrów ekstensywnych, w wersji z dU odwrotnie

## Trzecia Zasada Termodynamiki

Obowiązuje gdy $T \to 0$.

### Wersja W. Nernsta

Jeśli mamy entropię (funkcję T i jakichś parametrów, które oznaczamy X)

$$ T = \text{const}, X_1 \to X_2: \lim_{ T \to 0} [ S( T, X_2) - S(T, X_1) ] = 0 $$

### Wersja M. Plancka

Jeśli mamy entropię (funkcję T i jakichś parametrów), to granica tych parametrów $T \to 0$ jest stała (on zaproponował zero, ale w kondensatach.... chyba nie).
