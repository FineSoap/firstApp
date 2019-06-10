1. Obliczanie rozmiaru bitmapy, np.   
    Rozmiar = 10cm x 5 cm -> 4i x 2i.  
    Jakosc = 300dpi.  
    Kolor = grayscale = 8b = 1B.  
    dlugosc * jakosc * wysokosc * jakosc * kolor = 4 * 300 * 2 * 300 * 8b = 5 760 000b = 720 000 ~ 703 KB.
2. Co to jest ( podstawowe definicje ):
    - w oku preciki -> receptory jasnosci( fotopowe ) i czopki -> receptory barw ( skotopowe )
    - OpenGl -> Biblioteka Graficzna ( Graphic Library )
    - jednostka swiatlosci -> kandela (cd.)
    - piksel -> najmniejszy jednolity (przedstawiający konkretny kolor) element obrazu 
    - rozdzielczosc -> parametr określający liczbę pikseli obrazu wyświetlanych na ekranie ( szerokoc x wysokosc )
    - bitmaping -> mapowanie jakis wartosci ( zazwyczaj wartosci pikseli ) na bity
    - histogram -> rozklad empiryczny cechy ( wykres ile czegos jest - zapewne chodzi o rozklad kolorow )
    - gamut -> jakis okreslony zbior kolorow, np. zakres barw danego urzadzenia
    - punkt bieli w modelu CIE XYZ -> punkt o jednakowych wspolrzednych X Y Z ( wykres chromatycznosci )
    - barwa dominujaca (barwa czysta dla jakiegos punktu) i dopelniajaca -> jakies cos z wykresu XYZ
3. Modele odbicia oswietlenia lokalnego:
    - Phong -> 
    - Cook-Torrence -> 
4. Modele oswietlenia globalnego:
    - sledzenie promieni (ray tracing) ->
    - oswietlenie rozproszone (ambient occlusion) ->
5. Prawa Grassmanna
    - trójchromatyczności -> Każda dowolnie wybrana barwa może być określona za pomocą trzech liniowo niezależnych barw.
    - ciągłości -> Stopniowa zmiana barwy jednego składnika w mieszaninie złożonej z dwóch barw powoduje stopniową zmianę barwy mieszanej.
    - addytywnosci -> Barwa mieszaniny zależy jedynie od barw jej składników, a nie od ich składu widmowego.
6. Prawo Webera-Fechnera ->  prawo wyrażające relację pomiędzy fizyczną miarą bodźca a reakcją zmysłów, np. wzroku, słuchu, węchu czy poczucia temperatury (siła wrażenia).
7. Zjawisko hamowania obocznego -> Na granicy kolorow (bialy i czarny), bialy wydaje sie bardziej bialy a czarny wydaje sie bardziej czarny. Spowodowane budowa oka.
8. Klasy algorytmow przyspieszajacych sledzenie promieni (wymienic):
    - dzielenie przestrzeni ->
    - hierarchia bryl otaczajacych ->
    - maszyny rownolegle ->
9. BRDF = Dwukierunkowa Funkcja Rozkladu Odbicia -> proporcja swiatla docierajacego do swiatla odbijanego
10. Formaty plikow
    - wektorowe -> SVG EPS
    - rastrowe -> JPG GIF PNG MPEG4
11. Dwa rodzaje kompresji bezstratnej w grafice (wymien) -> LZW, RLE, DEFLATE
12. Kolejnosc operacji w formacie JPG:
    1. Konwersja RGB do Luminancja (jasnosc) + 2 kanaly Chrominancji (barwa)
    2. Czesciowe odrzucanie pikseli Chrominancji
    3. Dzielenie kanalow na bloki 8x8
    4. Na blokach robi sie DCT - Dyskretna Transformante Cosinusowa
    5. Zastapienie srednich wartosci blokow przez roznice wobec poprzednich DPCM
    6. Kwantyzacja - zamiana zmiennoprzecinkowych na calkowite
    7. Wspolczynniki DCT sa uporzadkowywane zygzakowato, aby zera byly obok siebie (?)
    8. Wspolczynniki niezerowe sa kompresowane algorytmem Huffmana
13. Rzeczywiste odbicie swiatla jest suma trzech skladowych -> kierunkowe + rozproszone + powrotne
14. Kontruktywna geometria bryl (CGS) -> jest oparta na logicznych operacjach na brylach
15. Systemy barw:
    - addytywne -> polegaja na dodawaniu kolorow skladowych i daza do bieli, np:
        - RGB -> Red Green Blue - (Czerwony Zielony Niebieski)
        - HSL -> Hue Saturation Lightness - (Barwa Nasycenie Jasnosc)
        - system Munsella -> Color Value Chroma - (Kolor Jasnosc Czystosc koloru)
        - CIE XYZ -> trzy skladowe trojchromatyczne
    - subtraktywne -> polegaja na odejmowaniu kolorow skladowych i daza do czerni, np:
        - RYB -> Red Yellow Blue - (Czerwony Zolty Niebieski)
        - CMY(K) -> Cyan Magenta Yellow (blacK) - (xD)
16. Atrybuty barwy -> nasycenie, jasnosc, odcien
17. Macierz do napisania -> odbicia lub filtry