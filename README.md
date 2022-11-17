# Techcareer Network&Security Bootcamp Bitirme Projesi
Techcareer tarafından 17 Ekim-8 Kasım tarihleri arasında düzenlenen 45 saatlik Network&Security bootcampini başarılı bir şekilde tamamlamak için hazırlanmış bir projedir. Yapılandırılması istenen topoloji aşağıdaki gibidir.
![image](https://user-images.githubusercontent.com/50342974/202558093-025891be-52a2-4fc4-8a48-aabdcdf65034.png)
### Proje Ortamı
- Proje Cisco Packet Tracer uygulaması ile simülasyon ortamında geliştirilmiştir. 
- Projede 3 adet 2811 Router, 1 adet 3560 24PS MultiLayer Switch, 2 adet 2960-24TT Switch, 2 adet Server-PT, 1 adet Laptop-PT, 1 adet PC-PT kullanılmıştır.
- Projede farklı networklerde 3 bölge bulunmaktadır. 
    - AREA 1'de biri DNS diğeri WEB sunucu olmak üzere 2 adet sunucu bulunmaktadır.
    - AREA 2'de 1 adet PC son kullanıcısı yerleştirilmiştir.
    - AREA 3'de ise 1 adet laptop son kullanıcısı yerleştirilmiştir.
### Projenin Amacı
- 2. ve 3. bölgedeki end devicelardan, 1. bölgede bulunan DNS ve WEB sunucularına hem IPv4 hem de IPv6 protokolleri ile erişilmelidir. 
- Routerlar arasındaki iletişim IPv4 ve IPv6 için OSPF ile yapılandırılmalıdır.
- ACL kuralları kullanılarak sunucuların sadece ilgili servis portlarına erişilmesi ve geriye kalan tüm sunucu portlarının kapatılması gerekmektedir.
 ### Proje Çıktıları
 Aşağıdaki görselde AREA 3'de bulunan PC makinesinden DNS ve WEB sunucularına IPv4 protokolü ile ping erişimin sağlanamadığı görülmektedir.
 
 ![image](https://user-images.githubusercontent.com/50342974/202562911-13a4c95d-70e4-4261-9145-abd1d9b7ce6e.png)
 
 Buna karşılık AREA 3'de bulunan PC'nin tarayıcısı üzerinden "cisco4.com" WEB sunucusuna erişebildiği görülmektedir.  
 
 ![image](https://user-images.githubusercontent.com/50342974/202564219-c3556826-d557-4283-b27d-de866cd6d21c.png)
 
AREA 3'deki PC'nin IPv6 adresi üzerinden de DNS ve WEB sunucularına ping erişiminin olmadığı aşağıda görülmektedir.

![image](https://user-images.githubusercontent.com/50342974/202565350-861a973f-8cc9-41c6-b24f-56b3cec5da7c.png)

Web tarayıcısı üzerinden, bu sefer IPv6 adresleri için oluşturulmuş "cisco6.com" adresine erişim sağlayabildiği aşağıda görülmektedir.

![image](https://user-images.githubusercontent.com/50342974/202566039-c0fe6914-57ce-4c72-bd9e-e2a96e206003.png)

Aynı şekilde Area 2'deki laptopda DNS ve WEB sunucularına sadece ilgili portlardan erişebilmektedir.
Detaylı incelemek için dosyayı indirebilirsiniz.
