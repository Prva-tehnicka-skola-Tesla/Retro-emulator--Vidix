# Upute za postavljanje popularnih igrica na Vidi x
Vidi X je mikroračunalo koje osmišljeno u Hrvatskoj i koristi ESP32 procesorom. Ima razvnovrsne koristi i primjena. Ovim uputama možete staviti emulator koji stavlja programe retro konzola na Vidi X.
## 1. Priprema
Kako bi započeli sa pripremanjem Vidi X-a za emulator prvo trebamo flashati procesor sa ovim programom: 

[flash_download_tools_v3.6.7_1.zip](https://github.com/user-attachments/files/18617109/flash_download_tools_v3.6.7_1.zip)

- Kada preuzmete program i otvorite ga, nađite opciju "ESP32 DownloadTool"
- Ovim alatom možemo brisati, zaustaviti i započeti preuzimanje na sami procesor.

## 2. Odroid-go firmware
Prvo preuzmite odroid go firmware:
https://github.com/VidiLAB-com/Vidi-X/blob/master/Alati-za-prvi-setup/odroid-go-firmware-20181001.img
1. Nakon što ste preuzeli odroid-go-firmware-20181001.img,  u prvom redu kliknite tri točkice (…). Nakon klika na tri točkice otvorit će se explorer s kojim morate navigirati do image-a. Kako bi mogli vidjeti image u donjem desnom kutu potrebno je odabarati „All files“ ili „Image“ opciju.

   ![image](https://github.com/user-attachments/assets/46f92ef8-5577-47a3-8ebb-8d16634c37d5)

2. Kada ste pronašli image kliknite na njega te ga otvorite. Nakon toga odmah pored prvog reda trebate upisati memorijsku lokaciju u kojoj će se učitati zadani image. To je 0x00. Ispred prvog reda treba biti kvačica kako bi prvi red pozelenio. Ako još niste, ukopčajte Vidi X u računalo pa izaberite COM: port sa padajuće liste (ako je više portova navedeno, odabire se onaj s većim brojem).

3. Nakon toga samo trebate postaviti sve parametre prema slici ispod.

   ![image](https://github.com/user-attachments/assets/89503bb9-e44e-4b95-bda6-4a8ca6d1e244)

5. Ako ste sve postavili prema slici, možete započeti sa flashanjem. Prvo ćete kliknuti na ERASE gumb te kada se pojavi FINISH na mjestu IDLE-a, možete kliknuti START. Kada program završi s preuzimanjem, gotovi ste sa flashanjem i možete ugasiti program.

## 3. Pripremanje SD kartice
Sada prelazimo na pripremanje SD kartice. SD karticu ćemo trebati formati na FAT32 format. Zatim na SD karticu otpakirajte .zip datoteku:
[sdcard_0907.zip](https://github.com/user-attachments/files/18617615/sdcard_0907.zip)

- Na SD kartici ćete imati dvije mape : odroid i roms
- U roms mapi će se nalaziti emulatori pod nazivom:

   - nes – Nintendo Entertainment System
   - gb – Nintento GameBoy
   - gbc – Nintendo GameBoy Color
   - sms – Sega Master System
   - gg – Sega Game Gear
   - col – ColecoVison

Kada pronađete rom igrice koje želite igrati možete ih staviti u mapu pripadajućeg emulatora. Npr. za Gameboy Color rom ćete staviti u mapu roms/gbc sa ekstenzijom  .gbc te tako i za ostale emulatore.

Ako ste točno pratili korake možete ugasiti i upaliti Vidi X te započeti sa igranjem retro igrica.
## 4. Gotovo 
- ....
     (slika)/(video)
## Dodatna opcije
  ### Bolji go play 
  Dodatno se može zamijeniti još boljim sistemom "Super Go play" koji nudi poboljšani zvuk i omogućava izmjenu boje zaslona.
  Emulator je dostupan na stranici: https://github.com/mattkj/super-go-play

  
  ### Dodatne igrice






