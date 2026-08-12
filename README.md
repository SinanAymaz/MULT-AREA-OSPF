# Multi-Area OSPF – Cisco Packet Tracer

##  Proje Hakkında

Bu proje, **Cisco Packet Tracer** kullanılarak **Multi-Area OSPF** yapılandırmasını göstermektedir.

Proje içerisinde **Area 0 (Backbone)**, **Area 1** ve **Area 2** kullanılarak farklı ağlar arasında dinamik yönlendirme sağlanmıştır.

##  Proje Yapısı

* **3 Router**
* **3 Switch**
* Her router'a bağlı istemci cihazlar
* **Area 1**
* **Area 0 (Backbone)**
* **Area 2**
* Routerlar arasında **Serial bağlantılar**

##  IP Planı

| Bölge  | Network           |
| ------ | ----------------- |
| Area 1 | `192.168.10.0/24` |
| Area 0 | `192.168.20.0/24` |
| Area 2 | `192.168.30.0/24` |

Routerlar arasındaki Serial bağlantılarda `10.0.0.0` ağı kullanılmaktadır.

##  OSPF Yapısı

Topolojide **Area 0**, backbone bölgesi olarak görev yapmaktadır.

```text
        Area 1
           |
        Router
           |
        Area 0
           |
        Router
           |
        Area 2
```

**Multi-Area OSPF** sayesinde farklı bölgelerde bulunan ağların routing bilgileri dinamik olarak paylaşılır.

Bu yapı sayesinde **Area 1 ile Area 2 arasında iletişim** sağlanmaktadır.

##  Kullanılan Teknolojiler

* Cisco Packet Tracer
* OSPF
* Multi-Area OSPF
* Area 0 Backbone
* Area 1
* Area 2
* Serial bağlantılar
* IPv4
* Dynamic Routing

##  Test ve Doğrulama

OSPF komşuluklarını kontrol etmek için:

```text
show ip ospf neighbor
```

Routing tablosunu kontrol etmek için:

```text
show ip route
```

OSPF yapılandırmasını kontrol etmek için:

```text
show ip protocols
```

Bağlantıyı test etmek için:

```text
ping 192.168.30.x
```

komutu kullanılabilir.

##  Projenin Amacı

Bu proje ile aşağıdaki konularda pratik yapılmıştır:

* Multi-Area OSPF yapılandırması
* Area 0 Backbone yapısı
* Area 1 ve Area 2 yapılandırması
* OSPF komşuluklarının oluşturulması
* Routerlar arası dinamik yönlendirme
* Serial bağlantıların yapılandırılması
* Routing table kontrolü
* Farklı ağlar arasında iletişim testi


**Cisco Packet Tracer | Networking Lab | Multi-Area OSPF**
