# Welkom bij D

Welkom bij de interactieve rondleiding door de *D Programmeer taal*.

{{#dmanmobile}}

De rondleiding biedt een overzicht van deze __krachtige__ en __expressieve__
taal, die rechtstreeks wordt gecompileerd naar __efficiënte__, __native__ machinecode.

{{/dmanmobile}}

### Wat is D?

D is het resultaat van _tientallen jaren ervaring met het ontwikkelen van compilers_
voor tal van verschillende programmeertalen en beschikt over een unieke reeks functies:

{{#dmandesktop}}

- _high level_ constructies voor uitstekende modelleringsmogelijkheden
- _hoge prestaties_, gecompileerde taal
- statische types
- directe koppeling met de API’s van het besturingssysteem en de hardware
- zeer snelle compilatietijden
- geheugenveilige subset (SafeD)
- _onderhoudbare_, _makkelijk te begrijpen_ code
- een geleidelijke leercurve (C-achtige syntax, vergelijkbaar met Java en andere talen)
- compatibel met de binaire interface voor C-toepassingen
- beperkte compatibiliteit met de binaire interface van C++-toepassingen
- veelzijdig (imperatief, gestructureerd, objectgeoriënteerd, generiek, functioneel programmeren, en zelfs assembleertaal)
- ingebouwde foutdetectie (contracten, unit-tests)

... en nog veel meer [functionaliteiten](http://dlang.org/overview.html).

{{/dmandesktop}}

### Over de rondleiding

Elk hoofdstuk bevat een voorbeeld broncode dat kan worden aangepast en gebruikt
om te experimenteren met de taalfuncties van D.
Klik op de ‘run’ knop (of druk op `Ctrl-Enter`) om het programma te compileren en uit te voeren.

Om door deze rondleiding te navigeren, gebruik de "`<` vorige" en de "`>` volgende" knoppen die beneden te vinden zijn op het scherm (of gebruik de linker- en rechterpijltoets). Of ga meteen naar een specifiek hoofdstuk met behulp van het menu bovenaan.

### Contributing

Deze rondleiding is [open source](https://github.com/dlang-tour)
en we staan open voor pull requests om deze rondleiding te verbeteren.

## {SourceCode}

```d
import std.stdio;
import std.algorithm;
import std.range;

void main()
{
    // Let's get going!
    writeln("Hello World!");

    // An example for experienced programmers:
    // Take three arrays, and without allocating
    // any new memory, sort across all the
    // arrays inplace
    int[] arr1 = [4, 9, 7];
    int[] arr2 = [5, 2, 1, 10];
    int[] arr3 = [6, 8, 3];
    sort(chain(arr1, arr2, arr3));
    writefln("%s\n%s\n%s\n", arr1, arr2, arr3);
    // To learn more about this example, see the
    // "Range algorithms" page under "Gems"
}
```
