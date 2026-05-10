# BSM316 Gömülü Sistemler Ödev 3

Bu projede STM32F103C8T6 Bluepill kartı kullanılarak TIM2 interrupt ile PC13 üzerindeki dahili LED kontrol edilmiştir.

## Özellikler

- TIM2 saniyede 1 kez interrupt üretir.
- PC13 LED, `blink_count` değeri kadar yanıp söner.
- LED yanıp sönme döngüsünden sonra 5 saniye sönük bekler.
- PA0 buton girişi olarak kullanılmıştır.
- PA1 GPIO output olarak ayarlanmıştır ve program boyunca lojik 0 kalır.
- `blink_count` değeri 4 ile 7 arasında değişir.
- `blink_count` her değiştiğinde STM32 dahili Flash belleğine kaydedilir.
- Açılışta `blink_count` Flash bellekten okunur.
- Açılışta PA0 butonu en az 3 saniye basılı tutulursa fabrika ayarına dönülür ve `blink_count = 4` olur.

## Kullanılan Donanım

- STM32F103C8T6 Bluepill
- ST-Link
- PA0-A1 arası buton bağlantısı veya kısa devre teması
- PC13 dahili LED

## Video

Video linki: buraya YouTube linkini yaz
