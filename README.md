# Modul-3-I11
I Putu Arya Prawira Wiwekananda-5025211065<br>
Hanifi Abrar Setiawan-5025211066<br>
Muhammad Fadhlan Asila Harashta-5025211068<br>

### Question
1. Lakukan konfigurasi sesuai dengan peta yang sudah diberikan.<br>
2. Client yang melalui Switch3 mendapatkan range IP dari [prefix IP].3.16 - [prefix IP].3.32 dan [prefix IP].3.64 - [prefix IP].3.80 <br>
3. Client yang melalui Switch4 mendapatkan range IP dari [prefix IP].4.12 - [prefix IP].4.20 dan [prefix IP].4.160 - [prefix IP].4.168<br>
4. Client mendapatkan DNS dari Heiter dan dapat terhubung dengan internet melalui DNS tersebut<br>
5. Lama waktu DHCP server meminjamkan alamat IP kepada Client yang melalui Switch3 selama 3 menit sedangkan pada client yang melalui Switch4 selama 12 menit. Dengan waktu maksimal dialokasikan untuk peminjaman alamat IP selama 96 menit
Pada masing-masing worker PHP, lakukan konfigurasi virtual host untuk website berikut dengan menggunakan php 7.3.<br>

### Answer
#### Number 1
Topology
![topology](https://cdn.discordapp.com/attachments/934661338934943774/1175794901376565329/image.png?ex=656c8755&is=655a1255&hm=705243fb164b159a110a4f19859ed67322c4bea393755d7848bddbf2ca3d236e&)
#### Number 2
Inside etc/dhcp/dhcpd.conf write as follows
![dhcpno2](https://cdn.discordapp.com/attachments/934661338934943774/1175800588697616486/image.png?ex=656c8ca1&is=655a17a1&hm=c07bd2f8dfa72e360418feb0d2f5e1121a99f4077ce2b873407290231424fca4&)
After that in terminal write
![test2](https://cdn.discordapp.com/attachments/934661338934943774/1175800936866779157/image.png?ex=656c8cf4&is=655a17f4&hm=4cde988ad9166b1746a3f43f4db7aeff16f983974c8ce3bb0aa952b5c8c3417b&)
#### Number 3
Inside etc/dhcp/dhcpd.conf write as follows
![dhcpno3](https://cdn.discordapp.com/attachments/934661338934943774/1175801197693784155/image.png?ex=656c8d32&is=655a1832&hm=f419b4fbe797f8a95f2e359e5133d3a392d0803ff4fc8fa1116a855e1fafa35e&)
After that in terminal write
![test2](https://cdn.discordapp.com/attachments/934661338934943774/1175801455601528954/image.png?ex=656c8d70&is=655a1870&hm=d1bcd0a33880934a518621e765f26d46a7f35ab0b13314b873d041312c12a5dd&)
#### Number 4
Install Bind 9 by using ```apt-get install bind9 -y```
And then edit the file in /etc/bind/named.conf.local as follows
![soal4](https://cdn.discordapp.com/attachments/934661338934943774/1175802098210832384/image.png?ex=656c8e09&is=655a1909&hm=2d30cd43b50d44f7a53385d9dd5373a567e7655184ae3d4ed7669faac1f637a6&)
And then edit the file in /etc/bind/named.conf.options
![option4](https://cdn.discordapp.com/attachments/934661338934943774/1175802374653231214/image.png?ex=656c8e4b&is=655a194b&hm=1747fc16e57b2befc96a9b4c45cb95ad981c6053f095ac185634888879d183e0&)
Next edit /etc/bind/riegel/canyon.i11.com as follows
![canyon4](https://cdn.discordapp.com/attachments/934661338934943774/1175802823754137731/image.png?ex=656c8eb6&is=655a19b6&hm=7aa803953af884ab816b4e0ca803c9f2f7d5160093291df149056a2b7c1587e7&)
Test the internet in the client such as sein, stark, etc
![test4](https://cdn.discordapp.com/attachments/934661338934943774/1175803299304312862/image.png?ex=656c8f27&is=655a1a27&hm=801ef1779c34b7cbd0d992f488061882f6d55d8bd2ca75e642adbbab3f847916&)
#### Number 5
For number 5, do the same thing as no 2 and 3 just change the default-lease-time for switch3 and switch4
Switch3
![switch3](https://cdn.discordapp.com/attachments/934661338934943774/1175803686316937317/image.png?ex=656c8f84&is=655a1a84&hm=d733c59ed711d950c58433b7474c7743c3631017424f658ffa47b8cb80a73e1d&)
Switch4
![switch3](https://cdn.discordapp.com/attachments/934661338934943774/1175804006493327511/image.png?ex=656c8fd0&is=655a1ad0&hm=e2e4ea108d04453c58bfd01ba5576ef77ae4b9649a4e378d75bbb631d2d78b08&)
### Number 6
First install wget
```apt install wget```
Next install unzip
```apt install unzip```
Next write
```wget -O filename.zip "drive download link"```
(Make sure to put the download link not the drive link)<br>
And then unzip the file by using
```unzip filename.zip```
The folder should be called modul-3 and it will contains the following files
![folder6](https://cdn.discordapp.com/attachments/934661338934943774/1175804245132443729/image.png?ex=656c9009&is=655a1b09&hm=2e0a479e3eb0d8023a5aef09cbc0bc1b80c5f8bb15e4c2d8c0535d470d67fe53&)
