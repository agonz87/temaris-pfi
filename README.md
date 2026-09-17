# Temaris de PFI · Institut de Lliçà

Programacions de teoria d'aula dels mòduls dels **Programes de Formació i Inserció**, en format
HTML autònom: es projecten a classe sense internet, sense instal·lar res i sense dependències externes.

**Lloc web:** https://USUARI.github.io/temaris-pfi/

> Substitueix `USUARI` pel teu nom d'usuari de GitHub quan tinguis Pages activat.

## Accés

El portal i cada temari demanen una **contrasenya** la primera vegada que s'obren en un navegador,
i tot seguit amb quin **perfil** es treballa. Les dues coses es recorden en aquell navegador.

> ⚠️ La contrasenya **no és una protecció real**: el codi és visible dins del fitxer HTML i qualsevol
> que en sàpiga una mica la pot trobar. Serveix només perquè l'alumnat no entri al material per
> curiositat. Per bloquejar-lo un altre cop hi ha l'opció **«Bloqueja el temari»** al menú del perfil.

## Perfils

| Codi | Perfil professional | Família |
|------|--------------------|---------|
| **PFI EE01** | Auxiliar de muntatges d'instal·lacions electrotècniques en edificis | Electricitat i electrònica |
| **PFI HT06** | Auxiliar de serveis de restauració i cuina | Hoteleria i turisme |

Els mòduls de formació general s'imparteixen als dos perfils. Per això **el seguiment de les
sessions es desa per separat per a cada perfil**: el mateix temari porta dos comptadors
independents i es canvia d'un a l'altre amb el botó del perfil de la barra superior (o des del
portal). Els mòduls professionals 3013 i 3014 només són de l'EE01 i apareixen atenuats quan el
perfil actiu és l'HT06.

## Mòduls

| Mòdul | Títol (nom oficial del currículum) | Sessions | Durada | Perfils |
|-------|-----------------------------------|---------:|--------|---------|
| **3013** | Instal·lacions elèctriques i domòtiques | 33 | 1 h | EE01 |
| **3014** | Instal·lacions de telecomunicacions | 33 | 1 h | EE01 |
| **MFG1** | Estratègies i eines de comunicació | 55 | 2 h | EE01 + HT06 |
| **MPRL** | Formació bàsica en prevenció de riscos laborals | 33 | 1 h | EE01 + HT06 |
| **MFG4** | Incorporació al món professional | 50 | 1 h | EE01 + HT06 |

Total: **204 sessions**. El contingut de les sessions està redactat **en castellà**; els menús
d'accés, el portal i la pantalla de contrasenya són **en català**, i els noms dels mòduls es fan
servir tal com apareixen al currículum oficial.

**Excepció del MFG1:** és un mòdul de llengües i les seves sessions van en tres idiomes, marcats
amb un distintiu a la capçalera de cada sessió: **ES** (majoria), **CA** (les deu sessions en què
el contingut *és* la llengua catalana: 4, 11, 22, 31, 32, 33, 34, 42, 43 i 44) i **EN** (els tres
blocs d'anglès, amb l'explicació en castellà i tota la producció de l'alumnat en anglès fàcil).

## Contingut del repositori

```
index.html                      Portal d'entrada amb l'estat de cada mòdul
Temario_<codi>_Teoria.html      Temari complet de cada mòdul (un sol fitxer)
Banco_preguntas_<codi>_GIFT.txt Banc de preguntes per importar a Moodle
assets/logo.jpg                 Logo del centre
```

## Com s'usa un temari

Cada sessió sempre té la mateixa estructura:

1. **Repàs** de la sessió anterior, amb preguntes clicables que es corregeixen soles
2. **Objectius** i desenvolupament teòric amb esquemes, per projectar
3. **Comprovació ràpida** a mitja sessió
4. **Per dictar a la llibreta**: les frases que han de quedar escrites
5. **Exercici o taller** de classe amb la solució desplegable per al professorat
6. Quan toca, l'**activitat avaluable** amb la seva rúbrica tancada

Els mòduls 3013, 3014, MPRL i MFG4 fan **sessions de 60 minuts**. El **MFG1 fa sessions de 2 hores**,
perquè el seu horari real són dues classes de 2 h la setmana i perquè en un mòdul de comunicació el
taller *és* la classe: 110 h = 55 sessions ≈ 28 setmanes.

La barra superior té tres modes de visualització: **dictat** (només el que s'ha de dictar),
**pràctica** (només els exercicis amb la solució) i, al MFG1 i al MFG4, **avaluació** (només les
proves i les activitats avaluables amb les seves rúbriques).

## Avaluació

| Mòdul | Per trimestre | Pesos |
|-------|---------------|-------|
| **MFG1** | 2 proves + 2 treballs de grup + 5 activitats individuals | 40 % / 20 % / 40 % |
| **MFG4** | 2 proves + 1 treball de grup + 3 activitats individuals | 50 % / 20 % / 30 % |

A tots dos, les activitats individuals es fan i es lliuren **dins de la sessió**, i els treballs de
grup es preparen al taller de les sessions anteriors: així no cal enviar res a casa.

## Seguiment de les sessions

A la portada de cada temari hi ha el panell **«Seguimiento del curso»**, on es tria l'última
sessió impartida. El portal (`index.html`) llegeix aquesta dada i mostra l'avenç dels cinc
mòduls i la propera classe de cadascun, **per al perfil actiu**.

El progrés es desa al **navegador de cada persona** (`localStorage`), sense comptes ni servidor,
amb la clau `temaris.v1.<CODI>.<PERFIL>`. Qui obri el lloc des d'un altre equip o amb un altre
navegador comença el comptador de zero.

## Bancs de preguntes

Els fitxers `Banco_preguntas_*.txt` estan en **format GIFT**. Per importar-los a Moodle:

> Banc de preguntes › Importa › Format GIFT › puja el fitxer

Cada fitxer crea les seves pròpies categories, una per bloc del temari. Les preguntes estan
redactades a partir de les frases dictades a classe: *si et saps la llibreta, aproves*.

## Manteniment

Hi ha dades i materials que caduquen i que cal revisar al setembre:

- **Dades econòmiques del MFG4**, marcades dins del temari amb una caixa grisa **«Dato que caduca»**:
  el SMI, la quota d'autònoms, els tipus de cotització i les taules salarials del conveni
  (sessions 31, 47, 48 i 49).
- **Materials d'actualitat del MFG1**: les notícies del bloc 4, els bulos de la sessió 27 i les
  campanyes de la sessió 52 s'han de buscar cada curs; les adreces de les webs oficials de la
  sessió 47 canvien.
