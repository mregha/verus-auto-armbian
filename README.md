Script Autorun miner verush coin in Armbian

How to install

1.Buka terminal armbiannya.
2.Masukkan perintah dibawah
3.wget -L https://raw.githubusercontent.com/iwanmartinsetiawan/verus-auto-armbian/main/miner.sh
4.edit file miner.sh yang telah didownload sebelumnya.
nano miner.sh
wallet = ganti dengan wallet address verus kalian
workername = nama worker yang akan digunakan. Contoh : node-01
5.Save and quit. Dengan cara tekan tombol CTRL+X, tekan tombol Y dan enter.
6.ketik command dibawah di terminal, untuk edit crontab
crontab -e
7.Tambahkan script dibawah
@reboot bash /root/miner.sh > /root/miner.log 2>&1
Save dan quit. Dengan cara tekan tombol CTRL+X, tekan tombol Y dan enter.
