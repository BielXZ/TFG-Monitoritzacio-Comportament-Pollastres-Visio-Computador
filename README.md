# Monitorització del Comportament de Pollastres amb Visió per Computador

**Treball de Fi de Grau – UAB (2025/26)**
Autor: **Biel Ramon Polo**
Menció: **Computació**
Tutor: **Coen Antens**
Contacte: bielrp23@gmail.com

---

## Descripció

Aquest projecte desenvolupa un **sistema automatitzat de detecció, seguiment i anàlisi del comportament de pollastres** mitjançant **Visió per Computador i Deep Learning**, amb l’objectiu d’obtenir mètriques objectives relacionades amb el **benestar animal**.

El sistema treballa a partir de vídeos i permet analitzar:
- Patrons de moviment individuals i col·lectius
- Distribució espacial de l’activitat
- Trajectòries i consistència d’identitats al llarg del temps

---

## Tecnologies

- Python, OpenCV
- **YOLOv8 (segmentació)**
- **Norfair, DeepSORT, BoT-SORT, ByteTrack**
- Histogram of Oriented Gradients (HoG)
- Hungarian Algorithm
- Auto-Encoders convolucionals
- Google Colab
- CVAT

---

## Metodologia

1. **Tècniques clàssiques** (background subtraction, watershed)
2. **Associació d’objectes** amb HoG + Hungarian Algorithm
3. **Detecció amb YOLOv8-seg** entrenat amb dades anotades manualment
4. **Tracking multiobjecte** amb diversos algoritmes
5. **Extracció de mètriques** de moviment i comparació de mètodes MOT

S’ha desenvolupat també un **sistema híbrid propi** basat en Norfair + descriptors visuals per millorar l’estabilitat del seguiment amb baix cost computacional.

---

## Resultats

- Seguiment fiable de pollastres en entorns amb alta densitat i oclusions
- Extracció de mètriques com moviment total, velocitat i trajectòries
- **Norfair + HoG + Hungarian** ofereix un excel·lent equilibri entre precisió i eficiència
