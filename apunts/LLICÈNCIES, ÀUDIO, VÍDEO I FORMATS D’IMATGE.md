# APUNTS PER A DAW2: LLICÈNCIES, ÀUDIO, VÍDEO I FORMATS D’IMATGE

## Introducció
Aquest document presenta diferents aspectes essencials per al desenvolupament web i multimèdia en l’àmbit de DAW2: **les llicències i els drets d’autor**, el **funcionament bàsic dels fitxers d’àudio i vídeo**, la **classificació i selecció de formats** (imatge, àudio i vídeo) i recomanacions sobre com integrar contingut multimèdia en una pàgina web.

## Índex de continguts
1. [Llicències i drets d’autor en l’ús de continguts multimèdia](#1-llicències-i-drets-dautor-en-lús-de-continguts-multimèdia)
2. [Arxius d’àudio i vídeo: definició, compressió i còdecs](#2-arxius-dàudio-i-vídeo-definició-compressió-i-còdecs)
3. [Formats d’imatge: classificació i exemples](#3-formats-dimatge-classificació-i-exemples)
4. [Formats d’àudio](#4-formats-dàudio)
5. [Formats de vídeo](#5-formats-de-vídeo)
6. [Taula comparativa de formats](#6-taula-comparativa-de-formats)
7. [Recomanacions generals](#7-recomanacions-generals)
8. [Casos pràctics: integració de contingut multimèdia en una pàgina web](#8-casos-pràctics-integració-de-contingut-multimèdia-en-una-pàgina-web)
9. [Conclusió](#9-conclusió)
10. [Nous formats emergents](#10-nous-formats-emergents)

---

## 1. Llicències i drets d’autor en l’ús de continguts multimèdia

### 1.1. Concepte de drets d’autor
- **Drets d’autor (copyright)**: Conjunt de drets que la llei atorga als creadors d’obres originals (text, imatges, música, vídeos, programari, etc.) per protegir-ne l’ús, la distribució i l’explotació econòmica.
- **Domini públic**: Quan una obra passa a domini públic, significa que pot ser utilitzada lliurement per qualsevol persona sense necessitat de permís o pagament de drets. Normalment això succeeix quan han passat uns anys determinats després de la mort de l’autor (varia segons la legislació de cada país).

### 1.2. Tipus de llicències més comuns
1. **Copyright tradicional**  
   - L’autor conserva tots els drets sobre la seva obra.
   - Qualsevol ús requereix un permís explícit.
   - Sol ser la protecció per defecte.

2. **Creative Commons (CC)**  
   - Llicències que afavoreixen la compartició i reutilització de continguts.
   - Es basen en quatre condicions bàsiques:
     - **BY** (Reconeixement): Cal mencionar l’autor.
     - **NC** (No Comercial): Prohibeix l’ús comercial.
     - **ND** (No Derivatives): No es permeten obres derivades.
     - **SA** (Share Alike): Les obres derivades s’han de llicenciar de la mateixa manera.
   - Les combinacions d’aquestes condicions generen llicències com **CC BY**, **CC BY-SA**, **CC BY-NC-SA**, etc.

![image](https://github.com/user-attachments/assets/ca0116ae-6526-4ae1-b2f9-da985512b9ec)


3. **Llicències de programari lliure i codi obert**  
   - **GPL (General Public License)**: Permet utilitzar, copiar, modificar i redistribuir el codi, sempre que la versió resultant conservi la mateixa llicència.
   - **MIT**: Permet un ús molt ampli; cal conservar l’avís de copyright original.
   - **Apache**, **BSD**, etc.: Tenen condicions similars d’ús, modificació i redistribució, amb diferències en qüestions tècniques.

### 1.3. Què cal tenir en compte quan fem servir continguts de tercers?
- **Verificar la llicència**: Abans de descarregar i utilitzar un recurs, convé comprovar sota quina llicència es publica.
- **Donar crèdit a l’autor**: Si la llicència ho exigeix (p. ex., CC BY), cal esmentar l’autor i la font.
- **Respectar les restriccions**: Si la llicència és No Comercial (NC), no es pot fer servir el recurs amb finalitats lucratives.
- **Sol·licitar permís**: Si no està clar l’ús permès o hi ha restriccions, cal contactar amb l’autor o propietari dels drets.

---

## 2. Arxius d’àudio i vídeo: definició, compressió i còdecs

### 2.1. Què és un arxiu d’àudio o de vídeo?
Un **arxiu multimèdia** (d’àudio, vídeo o tots dos) és un fitxer que pot contenir fluxos d’informació com so, imatges en moviment, subtítols i metadades. Generalment, inclou:
1. **Contenidor**: El format que agrupa tots els fluxos (vídeo, àudio, subtítols, metadades) en un sol fitxer (p. ex. MP4, MKV, AVI). En àudio, poden ser WAV o AIFF.
2. **Flux d’àudio**: El so, codificat amb un còdec (MP3, AAC, FLAC, etc.).
3. **Flux de vídeo**: La seqüència d’imatges, amb un còdec específic (H.264, H.265, VP9, etc.).
4. **Subtítols** (opcional): Pistes de text que poden integrar-se en el mateix contenidor.
5. **Metadades**: Informació addicional (resolució, títol, autor, etc.).

### 2.2. Com es comprimeixen l’àudio i el vídeo?
- **Compressió**: Redueix la mida d’un fitxer per millorar-ne l’emmagatzematge i la transmissió.
  - **Sense pèrdua (lossless)**: No es perd informació. L’arxiu resultant és més gran, però la qualitat es manté intacta (p. ex. FLAC en àudio).
  - **Amb pèrdua (lossy)**: El còdec elimina part de la informació considerada menys rellevant (segons la psicoacústica o la percepció visual). Ofereix fitxers més petits, però la qualitat no pot restaurar-se completament (MP3, AAC, H.264, etc.).

### 2.3. Què són els còdecs?
- **Còdec (codificador/descodificador)**: Algorisme que comprimeix i descomprimeix un flux d’àudio o vídeo. Cada còdec utilitza un mètode de compressió específic.
- **Còdecs d’àudio**: MP3, AAC, Vorbis, Opus, FLAC, ALAC...
- **Còdecs de vídeo**: H.264 (AVC), H.265 (HEVC), VP9, AV1...

---

## 3. Formats d’imatge: classificació i exemples

### 3.1. Classificació: mapa de bits vs. vectorials
- **Imatges de mapa de bits (raster)**: Estan formades per píxels que contenen informació de color. S’utilitzen habitualment per a fotografies o imatges amb molts degradats (JPEG, PNG, GIF).
- **Imatges vectorials**: Es basen en formes geomètriques definides matemàticament. Es poden redimensionar sense perdre qualitat (SVG).

### 3.2. Formats d’imatge més comuns
1. **JPEG (Joint Photographic Experts Group)**
   - **Tipus**: Mapa de bits amb compressió amb pèrdua.
   - **Ús habitual**: Fotografies i imatges riques en color.
   - **Avantatge**: Mida reduïda.
   - **Inconvenient**: Possibles artefactes a compressions altes.

2. **PNG (Portable Network Graphics)**
   - **Tipus**: Mapa de bits amb compressió sense pèrdua.
   - **Ús habitual**: Logotips, icones, imatges amb transparència.
   - **Avantatge**: Manté qualitat original i admet transparència.
   - **Inconvenient**: Mida de fitxer més gran que JPEG.

3. **GIF (Graphics Interchange Format)**
   - **Tipus**: Mapa de bits, compressió sense pèrdua, però amb paleta de 256 colors.
   - **Ús habitual**: Animacions simples o imatges amb pocs colors.
   - **Avantatge**: Suporta animacions.
   - **Inconvenient**: Paleta de colors molt limitada.

4. **SVG (Scalable Vector Graphics)**
   - **Tipus**: Vectorial.
   - **Ús habitual**: Gràfics, logotips i icones escalables.
   - **Avantatge**: No perd qualitat en redimensionar.
   - **Inconvenient**: Poc idoni per a fotografies o imatges fotorealistes.

---

## 4. Formats d’àudio
1. **MP3 (MPEG-1 Audio Layer III)**
   - **Característiques**: Compressió amb pèrdua, àmpliament compatible.
   - **Avantatge**: Bona relació qualitat/mida.
   - **Inconvenient**: Pèrdua de qualitat en altes compressions.

2. **WAV (Waveform Audio File Format)**
   - **Característiques**: Sense compressió.
   - **Avantatge**: Qualitat màxima.
   - **Inconvenient**: Fitxers molt grans.

3. **FLAC (Free Lossless Audio Codec)**
   - **Característiques**: Sense pèrdua (lossless), amb certa compressió.
   - **Avantatge**: Manté la qualitat original.
   - **Inconvenient**: Més gran que MP3 (tot i que més petit que WAV).

4. **OGG Vorbis**
   - **Característiques**: Compressió amb pèrdua.
   - **Avantatge**: Format lliure, bona qualitat.
   - **Inconvenient**: Menys suport que MP3 en alguns dispositius.

---

## 5. Formats de vídeo
1. **MP4 (MPEG-4 Part 14)**
   - **Característiques**: Contenidor molt popular, admet còdecs com H.264, H.265.
   - **Avantatge**: Bona qualitat i compatibilitat àmplia.
   - **Inconvenient**: Alguns còdecs poden requerir llicències.

2. **WEBM**
   - **Característiques**: Desenvolupat per Google, usa còdecs VP8/VP9.
   - **Avantatge**: Ideal per streaming en HTML5, gratuït i obert.
   - **Inconvenient**: Compatibilitat limitada en dispositius antics.

3. **AVI (Audio Video Interleave)**
   - **Característiques**: Antic contenidor de Microsoft.
   - **Avantatge**: Molt reconegut, encara que vell.
   - **Inconvenient**: Menys eficient que altres formats moderns.

4. **MKV (Matroska Video)**
   - **Característiques**: Contenidor obert que suporta múltiples pistes de vídeo, àudio, subtítols.
   - **Avantatge**: Gran flexibilitat i suport per a molts còdecs.
   - **Inconvenient**: No sempre és el format predeterminat en entorns mòbils.

---

## 6. Taula comparativa de formats

| **Format** | **Tipus**                | **Compressió**        | **Usos Habituals**               | **Avantatges**                                       | **Inconvenients**                                     |
|------------|--------------------------|-----------------------|----------------------------------|------------------------------------------------------|-------------------------------------------------------|
| **JPEG**   | Imatge (raster)         | Amb pèrdua (lossy)    | Fotografies, imatges riques en color | Reducció de mida significativa                     | Possible pèrdua de qualitat amb compressió alta       |
| **PNG**    | Imatge (raster)         | Sense pèrdua (lossless) | Logotips, icones, transparència     | Manté qualitat i permet transparència              | Fitxers més grans que JPEG                            |
| **SVG**    | Imatge (vectorial)      | — (vector)            | Gràfics escalables, icones        | Escalat infinit sense pèrdua                       | No apte per a fotografies complexes                   |
| **MP3**    | Àudio                   | Amb pèrdua (lossy)    | Música en general, podcasts       | Molt compatible, fitxers petits                    | Pèrdua de qualitat                                   |
| **FLAC**   | Àudio                   | Sense pèrdua (lossless) | Àudio d’alta fidelitat              | Qualitat idèntica a l’original                     | Més gran que MP3                                    |
| **MP4**    | Vídeo (contenidor)      | Amb pèrdua (en general) | Vídeos per a web i dispositius       | Molt compatible                                   | Alguns còdecs són propietaris                        |
| **WEBM**   | Vídeo (contenidor)      | Amb pèrdua (VP8/VP9)  | Streaming web, HTML5               | Format lliure i obert                             | Suport irregular en dispositius antics               |
| **MKV**    | Vídeo (contenidor)      | Variable              | Múltiples pistes de vídeo/àudio    | Molt flexible i gratuït                            | No sempre per defecte en entorns mòbils              |
| **AVI**    | Vídeo (contenidor)      | Variable              | Arxius de vídeo històrics          | Compatibilitat "clàssica"                         | Més gran si s’usen còdecs antics                     |

---

## 7. Recomanacions generals
- **Compatibilitat**: Tria el format segons els dispositius i navegadors del públic objectiu. MP4 (H.264 o H.265) i WebM són bones opcions per a la web.
- **Qualitat vs. mida**: Cal equilibrar la qualitat i el pes del fitxer, especialment en entorns web on la velocitat de càrrega és rellevant.
- **Contingut editable**: Per elements que necessiten actualitzacions constants (com logotips), val la pena utilitzar formats sense pèrdua (PNG, SVG) o àudio sense pèrdua per preservar la qualitat.
- **Ús legal**: Verifica la llicència de totes les imatges, pistes d’àudio o vídeos per assegurar-ne l’ús legítim.

---

## 8. Casos pràctics: integració de contingut multimèdia en una pàgina web
1. **Pàgina web d’empresa amb continguts audiovisuals**:
   - **Imatges corporatives**: PNG (si cal transparència) o SVG (icones, vectors).
   - **Fotografies de productes**: JPEG, per la seva relació qualitat/mida.
   - **Vídeos promocionals**: MP4 (H.264), amb versió en WebM si cal.
   - **Àudio de fons**: MP3, tot i que s’ha de permetre desactivar-lo.

2. **Web d’aprenentatge en línia (e-learning)**:
   - **Vídeos educatius**: MP4 (H.264) i subtítols VTT o MKV.
   - **Podcasts**: MP3 per a descàrregues ràpides, OGG Vorbis com a opció lliure.
   - **Presentacions i gràfics**: SVG per a continguts interactius.

3. **Aplicació web amb galeria d’imatges**:
   - **Miniatures (thumbnails)**: JPEG amb compressió moderada.
   - **Imatges en alta resolució**: JPEG d’alta qualitat o PNG si cal màxima fidelitat.
   - **Iconografia**: Preferiblement SVG per eficiència i escalabilitat.

---

## 9. Conclusió
- **Llicències i drets d’autor**: Conèixer les diferents llicències (Creative Commons, GPL, etc.) i les seves implicacions és crucial per a l’ús responsable de continguts.
- **Fitxers multimèdia**: Saber com funcionen els contenidors, els còdecs i la compressió (amb o sense pèrdua) facilita una elecció encertada.
- **Formats d’imatge**: Distingir entre mapa de bits i vectorial ajuda a triar el format més adequat.
- **Pràctica recomanada**: Emprar formats estàndard i oberts, respectar llicències i assegurar la millor experiència d’usuari.

### Taula final de formats recomanats per a la web
| **Tipus de contingut** | **Format recomanat**                             | **Motiu**                                                                   |
|------------------------|--------------------------------------------------|-----------------------------------------------------------------------------|
| **Imatge**            | **JPEG** (fotos), **PNG** (transparència), **SVG** (icones) | Bon equilibri entre qualitat, mida i compatibilitat                         |
| **Àudio**             | **MP3** o **OGG Vorbis**                          | Compressió amb pèrdua, mida petita, bona compatibilitat                     |
| **Vídeo**             | **MP4** (H.264) o **WebM** (VP8/VP9)              | Molt compatibles amb navegadors moderns i dispositius diversos              |

Aquests coneixements són fonamentals en el dia a dia de l’àmbit de desenvolupament web i multimèdia, on cal triar recursos i formats òptims, tot respectant la legalitat.

---

## 10. Nous formats emergents
Malgrat que els formats anteriors són molt utilitzats, n’estan sorgint de nous amb l’objectiu de millorar la compressió i la qualitat, sobretot en entorns web i mòbils:

- **AVIF (AV1 Image File Format)**: Derivat del còdec de vídeo AV1, ofereix compressió amb pèrdua o sense pèrdua més eficient que JPEG o WebP. El suport encara no és universal, però creix gradualment.
- **HEIC (High Efficiency Image File Format)**: Basat en el còdec HEVC (H.265). Permet reduir la mida de les imatges amb més qualitat que JPEG, però presenta limitacions de compatibilitat en alguns navegadors.
- **AV1 (AOMedia Video 1)**: Còdec de vídeo obert i gratuït, amb millor compressió que H.264 i VP9. L’adopció encara és limitada a causa dels requeriments de potència i compatibilitat.
- **Opus**: Còdec d’àudio lliure, òptim per a transmissions de veu i música en temps real. Millora la qualitat de Vorbis o MP3 amb taxes de bits similars, però el suport no és universal.

Aquests formats poden resultar idonis en projectes on la mida i la qualitat siguin fonamentals, especialment en aplicacions mòbils o de streaming. Tanmateix, s’ha de valorar la compatibilitat amb els dispositius abans d’implantar-los en un entorn de producció.

