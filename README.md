# leviamassa


x)

Karvinen 2022: Cracking Passwords with Hashcat

- Lyhyt johdanne esimerkkien kanssa, miten salasanoja murretaan Hashcatin avulla.
- Esimerkki miten hash-tyyppi tunnetaan.
- Hyviä esimerkkejä a-kohtaan avuksi. 




Karvinen 2023: Crack File Password With John

- Puhutaan John the Ripper ohjelmasta, joka on tarkoitettu tiedostosalasanojen purkamiseen tarkemmin sanottuja ZIP.
- Pystyy purkamaan useita tiedostoja iTunesista telegrammiin.
- Itse en ollut aiemmin kuullut tästä, vaikka hauska nimileikki on keksitty.





Santos et al 2017: Security Penetration Testing - The Art of Hacking Series LiveLessons: Lesson 6: Hacking User Credentials 



- Puhuttiin salasanojen säilyttämisestä, niiden heikkouksista ja salasanoihin kohdistuvista hyökkäyksistä.
- Painotettiin MFA käyttöä.
- Alussa myös näytettiin millä brute-force työkaluilla voi päästä "purkamaan" salasanakantoja (medusa, wfuzz etc.) Näytettiin myös hashcatin toimintaa. 


Kennedy et al 2025: Metasploit: File-Format Exploits 


- File-format-haavoittuvuudet ovat hyväksikäytettäviä virheitä tiedostojen lukijoissa kuten Abode Readerissa. Hyökkäys tapahtuu kun uhri avaa tiedoston.
- Tärkeää on tiedonhankinta kohteesta ja tarkka kohdentaminen, jotta hyökkäys onnistuu.
- Loppukappaleessa puhuttiin hyvin, miten jos kohdistaa hyökkäyksiä ei niin teknillisiin yrityskomponentteihin, niin mahdollisuus onnistua kasvaa. 



Singh 2025: The Ultimate Kali Linux Book: Understanding Active Directory


- Active Directory mahdollistaa käyttäjien, laitteiden ja sääntöjen keskitetyn hallinnan Windows-verkoissa IT- ammattilaisten puolesta.
- Domaini on vain keräys eri organizational uniteista, jota käytetään organisoimaan objekteja. (näytetään kolmio-esimerkki)
- Domainien välillä voi olla eri luottamussuhteita, jotka määrittävät resurssien jakamisen. Kutsutaan kappaleessa nimellä trust models. 



a) 

Asensin hash catin aluksi annetuilla kommenoilla sudo apt-get update
ja  sudo apt-get -y install hashid hashcat wget


<img width="483" alt="image" src="https://github.com/user-attachments/assets/8ab08619-4f1a-4c70-ad2d-a16f216feae1" />


Vaihdoin luotuani ensin itseni hashed directoryyn. Wgetilla latasin ison kirjaston eri sanoja. 


<img width="491" alt="image" src="https://github.com/user-attachments/assets/23250eef-c11d-4ec7-b936-2b4772f7160b" />


Tämän jälkeen purin sen tar - komennolla. 


<img width="220" alt="image" src="https://github.com/user-attachments/assets/4e32e2c8-1eea-48e3-861f-50fa9172930b" />



headerinkin näin, jotta sisälle pääsin katsomaan erilaisia sanoja. Pääsin myös katsomaan erilaisia esimerkki hasheja. 


<img width="411" alt="image" src="https://github.com/user-attachments/assets/0794c56b-7cec-4854-bafc-f60ca5b9e11c" />




Sitten lähdin testaamaan juuri sitä esimerkkisalasanaa. 




<img width="484" alt="image" src="https://github.com/user-attachments/assets/93988247-224a-405a-8a01-42fe27d40cc4" />






<img width="387" alt="image" src="https://github.com/user-attachments/assets/ae839011-0b1d-40a7-9444-e2fdf86938dc" />



Ja näin se ratkesi. 




b)

Latasin ja käänsin John the Ripperin aluksi kaliin. 


<img width="410" alt="image" src="https://github.com/user-attachments/assets/d5195338-9ec7-4592-a784-6b7d161a9328" />





John saatiin compilattua. 


<img width="480" alt="image" src="https://github.com/user-attachments/assets/8f8738a8-7fcc-491b-bbaa-fbddedcb942f" />


run/ löysi myös näitä scriptejä. 


<img width="295" alt="image" src="https://github.com/user-attachments/assets/2aa4c8a3-716d-4f6d-b45d-8fd0d2ad8eb0" />




<img width="364" alt="image" src="https://github.com/user-attachments/assets/6747df27-9b42-43b7-9ac3-e729de1249bf" />



john tulosti näin 


<img width="479" alt="image" src="https://github.com/user-attachments/assets/6f6200b5-4677-41dd-9c98-96424db2a2f1" />


Testasin eri salasanoja ja en päässyt. 


<img width="352" alt="image" src="https://github.com/user-attachments/assets/dd19953b-ce8a-4f9a-872b-5d50902928b7" />









## Yhteenveto 




# References 



Karvinen 2022: Cracking Passwords with Hashcat, https://terokarvinen.com/2022/cracking-passwords-with-hashcat/




Karvinen 2023: Crack File Password With John, https://terokarvinen.com/2023/crack-file-password-with-john/




Santos et al 2017: Security Penetration Testing - The Art of Hacking Series LiveLessons: Lesson 6: Hacking User Credentials, https://www.oreilly.com/videos/security-penetration-testing/9780134833989/9780134833989-sptt_00_06_00_00/




 Kennedy et al 2025: Metasploit: File-Format Exploits, https://www.oreilly.com/library/view/metasploit-2nd-edition/9798341620032/xhtml/chapter9.xhtml#:-:text=File-Format%20Exploits




 Singh 2025: The Ultimate Kali Linux Book: Understanding Active Directory, https://www.oreilly.com/library/view/the-ultimate-kali/9781835085806/Text/Chapter_12.xhtml#_idParaDest-272




GeeksForGeeks 2024: How to use John the Ripper in Kali Linux, https://www.geeksforgeeks.org/how-to-use-john-the-ripper-in-kali-linux/
