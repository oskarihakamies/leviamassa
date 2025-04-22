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




## Yhteenveto 




# References 


Karvinen 2022: Cracking Passwords with Hashcat, https://terokarvinen.com/2022/cracking-passwords-with-hashcat/



Karvinen 2023: Crack File Password With John, https://terokarvinen.com/2023/crack-file-password-with-john/


Santos et al 2017: Security Penetration Testing - The Art of Hacking Series LiveLessons: Lesson 6: Hacking User Credentials, https://www.oreilly.com/videos/security-penetration-testing/9780134833989/9780134833989-sptt_00_06_00_00/


 Kennedy et al 2025: Metasploit: File-Format Exploits, https://www.oreilly.com/library/view/metasploit-2nd-edition/9798341620032/xhtml/chapter9.xhtml#:-:text=File-Format%20Exploits


 Singh 2025: The Ultimate Kali Linux Book: Understanding Active Directory, https://www.oreilly.com/library/view/the-ultimate-kali/9781835085806/Text/Chapter_12.xhtml#_idParaDest-272



