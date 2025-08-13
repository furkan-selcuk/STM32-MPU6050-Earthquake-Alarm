# STM32 MPU6050 Earthquake Alarm

Bu proje, **STM32 mikrodenetleyici** kullanarak **MPU6050 ivmeölçer/jyroskop sensörü** ile deprem algılama ve buzzer ile alarm verme sistemidir.  
Ayrıca UART üzerinden bilgisayara anlık **Ax, Ay, Az** ivme verilerini gönderir, böylece terminalde veya Live Expressions ile takip edilebilir.

## 🚀 Özellikler
- **MPU6050** ile 3 eksende ivme ölçümü
- **I2C** haberleşme
- **Buzzer** ile deprem alarmı
- Eşik değer bazlı titreşim algılama
- STM32CubeIDE ile geliştirilmiş örnek proje

## 🛠 Donanım Gereksinimleri
- STM32 (ör. STM32F4, STM32F1 serisi)
- MPU6050 sensörü (GY-521 modülü)
- Buzzer (aktif veya pasif)
- Bağlantı kabloları
- USB üzerinden programlama bağlantısı

## ⚙ Bağlantı Şeması
| STM32 Pin | MPU6050 Pin | Açıklama |
|-----------|-------------|----------|
| 3.3V      | VCC         | Güç      |
| GND       | GND         | Toprak   |
| PB6       | SCL         | I2C Clock|
| PB7       | SDA         | I2C Data |
| PA0       | Buzzer      | Alarm çıkışı |

## 📦 Kullanım
1. STM32CubeMX ile `I2C1`  yapılandırın.
2. Projeyi **STM32CubeIDE** ile açın.
3. Kodu kartınıza yükleyin.
4. Ax, Ay, Az değerlerini takip edin ve eşik değeri geçtiğinde buzzer çalışacaktır.

## 📷 Görseller
![WhatsApp Image 2025-08-13 at 19 07 41_ba8e5e07](https://github.com/user-attachments/assets/9cc9b7d1-57ec-4e36-9e69-577e23ecc456)


## 📄 Lisans
Bu proje **MIT** lisansı ile paylaşılmıştır. Özgürce kullanılabilir, değiştirilebilir ve dağıtılabilir.
