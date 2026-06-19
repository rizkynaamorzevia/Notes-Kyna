download blackbird amanda
download rufus
sambungkan flashdisk, buka rufus, format amanda ke flashdisk
restart laptop 
masuk ke BIOS
jadikan linux boot paling atas
masuk linux
cek partisi : lsblk
sambungin wifi : iwctl > device list > station wlan0 scan > station wlan0 get-networks > station wlan0 connect NAMA_WIFI > exit
partisi disk : cfdisk /dev/nvme0n1
pilih disk yg dipake buat linux, select, enter
nanti dipojok tulisannya jadi partition size : 30G
abis itu enter aja, tulisan di atas yang partisi linux nya nanti jadi 30G sampingnya ada tulisan linux filesystem
yang menu dibawah geser ke menu WRITE terus nanti ada pertanyaan, tulis aja yes, abis itu keluar dengan geser lagi ke menu quit
buat partisi linux baru : mkfs.ext4 /dev/nvme0n1p6 (SETIAP LAPTOP BEDA" HARAP DI CEK KEMBALI, lokasi file linux)

