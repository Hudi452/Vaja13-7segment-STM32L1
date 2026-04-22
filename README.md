# Vaja13-7segment-STM32L1

PINOUT KONFIGURACIJA:\
![konfig](https://github.com/Hudi452/Vaja13-7segment-STM32L1/blob/main/Pinout_konfiguracija.png)

2. b)\
Segment a: PA0\
Segment b: PA1\
Segment c: PA2\
Segment d: PA3\
Segment e: PA4\
Segment f: PA5\
Segment g: PA6\
c) Prikazovalnik ima skupno katodo.\
e) Pravilnostna tabela:\
Števka--a-b-c-d-e-f-g--PA15-PA14-PA13-PA12-PA11-PA10-PA9-PA8-PA7-PA6-PA5-PA4-PA3-PA2-PA1-PA0--HEX\
---0-----1-1-1-1-1-1-0---0----0----0----0----0----0----0---0---0---0---1---1---1---1---1---1----0X003F\
---1-----0-1-1-0-0-0-0---0----0----0----0----0----0----0---0---0---0---0---0---0---1---1---0----0X0006\
---2-----1-1-0-1-1-0-1---0----0----0----0----0----0----0---0---0---1---0---1---1---0---1---1----0X005B\
---3-----1-1-1-1-0-0-1---0----0----0----0----0----0----0---0---0---1---0---0---1---1---1---1----0X004F\
---4-----0-1-1-0-0-1-1---0----0----0----0----0----0----0---0---0---1---1---0---0---1---1---0----0X0066\
---5-----1-0-1-1-0-1-1---0----0----0----0----0----0----0---0---0---1---1---0---1---1---0---1----0X006D\
---6-----1-0-1-1-1-1-1---0----0----0----0----0----0----0---0---0---1---1---1---1---1---0---1----0X007D\
---7-----1-1-1-0-0-0-0---0----0----0----0----0----0----0---0---0---0---0---0---0---1---1---1----0X0007\
---8-----1-1-1-1-1-1-1---0----0----0----0----0----0----0---0---0---1---1---1---1---1---1---1----0X007F\
---9-----1-1-1-1-0-1-1---0----0----0----0----0----0----0---0---0---1---1---0---1---1---1---1----0X006F\
3. e) ODR pomeni Output Data Register (register izhodnih podatkov). To je 16-bitni register, ki neposredno določa stanje (napetost) na pinih določenega porta (v tem primeru porta A). Če v določen bit registra vstavimo 1, pin nastavimo na napetost 3,3 V, če pa bit nastavimo na 0, ta pin nastavimo na napetost 0 V.\
4.  e) Ko pritisnemo črno tipko na STM32, se STM32 resetira, kar pomeni, da se program začne izvajati od začetka. Na 7-segmentnem displayu se ponovno začne štetje od 0 do 9, ko pritisnemo na tipko reset.

Komentar na delovanje:\
Projekt deluje po pričakovanjih. 7-segmentni display šteje od 0 do 9. To se ves čas, ko je STM32 priključen na napajanje ponavlja. 
