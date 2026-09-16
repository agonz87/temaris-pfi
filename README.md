# Temaris de PFI · Institut de Lliçà

Programacions de teoria d'aula dels mòduls dels **Programes de Formació i Inserció**, en format
HTML autònom: es projecten a classe sense internet, sense instal·lar res i sense dependències externes.

**Lloc web:** https://USUARI.github.io/temaris-pfi/

> Substitueix `USUARI` pel teu nom d'usuari de GitHub quan tinguis Pages activat.

## Perfils

| Codi | Perfil professional | Família |
|------|--------------------|---------|
| **PFI EE01** | Auxiliar de muntatges d'instal·lacions electrotècniques en edificis | Electricitat i electrònica |
| **PFI HT06** | Auxiliar de serveis de restauració i cuina | Hoteleria i turisme |

## Mòduls

| Mòdul | Títol | Sessions | Perfils |
|-------|-------|---------:|---------|
| **3013** | Instalaciones eléctricas y domóticas | 33 | EE01 |
| **3014** | Instalaciones de telecomunicaciones | 33 | EE01 |
| **MPRL** | Prevención de riesgos laborales | 33 | EE01 + HT06 |
| **MFG4** | Incorporación al mundo profesional | 50 | EE01 + HT06 |

Total: **149 sessions** d'una hora. Els materials estan redactats en castellà.

## Contingut del repositori

```
index.html                      Portal d'entrada amb l'estat de cada mòdul
Temario_<codi>_Teoria.html      Temari complet de cada mòdul (un sol fitxer)
Banco_preguntas_<codi>_GIFT.txt Banc de preguntes per importar a Moodle
assets/logo.jpg                 Logo del centre
```

## Com s'usa un temari

Cada sessió està pensada per a 60 minuts i sempre té la mateixa estructura:

1. **Repàs** de la sessió anterior, amb preguntes clicables que es corregeixen soles
2. **Objectius** i desenvolupament teòric amb esquemes, per projectar
3. **Comprovació ràpida** a mitja sessió
4. **Per dictar a la llibreta**: les 6-8 frases que han de quedar escrites
5. **Exercici** de classe amb la solució desplegable per al professorat

La barra superior té tres modes de visualització: **dictat** (només el que s'ha de dictar),
**pràctica** (només els exercicis amb la solució) i, al MFG4, **avaluació** (només les proves
i les activitats avaluables amb les seves rúbriques).

## Seguiment de les sessions

A la portada de cada temari hi ha el panell **«Seguimiento del curso»**, on es tria l'última
sessió impartida. El portal (`index.html`) llegeix aquesta dada i mostra l'avenç dels quatre
mòduls i la propera classe de cadascun.

El progrés es desa al **navegador de cada persona** (`localStorage`), sense comptes ni servidor.
Qui obri el lloc des d'un altre equip o amb un altre navegador comença el comptador de zero.

## Bancs de preguntes

Els fitxers `Banco_preguntas_*.txt` estan en **format GIFT**. Per importar-los a Moodle:

> Banc de preguntes › Importa › Format GIFT › puja el fitxer

Cada fitxer crea les seves pròpies categories, una per bloc del temari. Les preguntes estan
redactades a partir de les frases dictades a classe.

## Manteniment

Hi ha dades que caduquen cada any i que cal revisar al setembre, marcades dins dels temaris
amb una caixa grisa **«Dato que caduca»**: el SMI, la quota d'autònoms, els tipus de cotització
i les taules salarials del conveni (sessions 31, 47, 48 i 49 del MFG4).
