<h1 align="center"> Sui Devnet Node Kurulumu </h1> 

Not: Türkçeye çevrilmiştir, alıntıdır.
![image](https://user-images.githubusercontent.com/101149671/178116806-26715fca-3ff8-43d5-ae1e-cee3926828de.png)

# Telegram kanalı: https://t.me/SuiTurkish

# Gereksinimler (minimum) (ekip tavsiyesi 8 ram):
```
2 CPU
4 RAM
50 SSD
```
Node kurduktan sonra sonda söyleyeceğim işlemleri yapmayı unutmayın!!

# Bir screen oluşturalım:
```
screen -S sui
```

# Full nodeumuzu yükleyelim (15-20dk sürebilir)
```
wget -O sui.sh https://raw.githubusercontent.com/kj89/testnet_manuals/main/sui/sui.sh && chmod +x sui.sh && ./sui.sh
```

# Node başarılı çalıştıktan sonra karşınıza şu şekilde bir görsel çıkacak:

![image](https://user-images.githubusercontent.com/101149671/178118226-8ea930d4-a9d5-4bb3-be75-e682b0aac0ea.png)

# Daha sonra discorda giriyoruz ve şu şekilde mesaj atıyoruz #node-ip-application kanalına: https://discord.gg/GUeN8TY7xD

![image](https://user-images.githubusercontent.com/101149671/178118265-a2463048-f656-4382-87cf-faaef1d032d0.png)

Not: #pick-a-role role kanalından da rol alabilirsiniz isterseniz emojilere tıklayarak.

# Nodeunuzu kontrol etmek için: https://node.sui.zvalid.com/

![image](https://user-images.githubusercontent.com/101149671/178118300-29d6bf7e-c78a-40b0-97fd-26bd89d22b05.png)

<h1 align="center"> Yararlı komutlar </h1> 

# Loglar: 
```
journalctl -u suid -f -o cat
```

# Node silmek için:
```
sudo systemctl stop suid
sudo systemctl disable suid
sudo rm -rf ~/sui /var/sui/
sudo rm /etc/systemd/system/suid.service
```

# Node durumunu kontrol:
```
service suid status
```
![image](https://user-images.githubusercontent.com/101149671/178118339-82da6b52-bdb9-425a-af8d-832a671141aa.png)

# Node reset atma:
```
sudo systemctl restart suid
```

# Node durdurma: 
```
sudo systemctl stop suid
```
<img src="https://github-readme-stats.vercel.app/api?username=kebapTest&show_icons=true&theme=highcontrast" align="left" width="450" height="350" >




