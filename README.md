# 🤖 Akıllı Asistan (Smart Assistant)

Modern web teknolojileri kullanılarak geliştirilmiş, sesle ve metinle etkileşime girebilen kural tabanlı bir sanal asistan arayüzüdür. Tamamen tarayıcı üzerinde, ekstra bir sunucu veya API bağlantısına ihtiyaç duymadan çalışır.

## ✨ Özellikler

- **🎙️ Sesli Komut (Speech Recognition):** Mikrofonunuzu kullanarak asistana doğrudan sesli olarak soru sorabilir veya komut verebilirsiniz.
- **🔊 Sesli Yanıt (Text-to-Speech):** Asistan, verdiği cevapları tarayıcının yerleşik ses sentezleyicisi ile size sesli olarak okur.
- **😮 Dinamik Yüz Animasyonu:** Asistan konuşurken ağız hareketleri sese uygun olarak senkronize edilir (titrer), konuşma bittiğinde eski haline döner.
- **🧠 Kural Tabanlı Chatbot:** Önceden belirlenmiş anahtar kelimelere (merhaba, nasılsın, kimsin vb.) mantıklı ve eğlenceli cevaplar verir. Bilmediği kelimelerde rastgele akıllıca varsayılan yanıtlar üretir.
- **💎 Modern Arayüz:** "Glassmorphism" (buzlu cam) tasarımı ve arka planda animasyonlu renk geçişleriyle (CSS Animations) premium bir görsel deneyim sunar.

## 🚀 Kurulum ve Kullanım

Herhangi bir sunucu kurulumuna veya paket yüklemesine gerek yoktur!

1. Bu projeyi bilgisayarınıza indirin veya klonlayın:
   ```bash
   git clone <repo-url>
   ```
2. Klasörün içindeki `index.html` dosyasını modern bir web tarayıcısında açın.
   *(Not: Mikrofon özelliklerinin sorunsuz çalışması için **Google Chrome** kullanılması tavsiye edilir.)*
3. Kutucuğa bir şeyler yazıp "Gönder" butonuna basın veya **Mikrofon (🎙️)** ikonuna tıklayıp konuşun.

## 🛠️ Kullanılan Teknolojiler

- **HTML5:** Sayfa iskeleti.
- **CSS3:** Animasyonlar, saydamlık (backdrop-filter), modern renk paletleri.
- **Vanilla JavaScript:** Mantıksal işlemler, olay dinleyicileri.
- **Web Speech API:** Tarayıcının kendi `SpeechSynthesis` (Metin Okuma) ve `SpeechRecognition` (Sesi Metne Çevirme) özellikleri.

## 👨‍💻 Özelleştirme

Asistanın verdiği cevapları değiştirmek veya yenilerini eklemek çok kolaydır. Sadece `index.html` dosyası içindeki JavaScript bölümünde yer alan `dictionary` nesnesini düzenlemeniz yeterlidir:

```javascript
const dictionary = {
  "merhaba": "Merhaba! Sana nasıl yardımcı olabilirim?",
  "yeni kelime": "İşte buraya cevabı yazabilirsin."
};
```

## 📝 Planlanan Geliştirmeler (TODO)

- [ ] İlerleyen aşamalarda gerçek bir AI / LLM API (Örn. Gemini API) bağlantısı kurmak.
- [ ] Kullanıcının seçebileceği farklı yüz / avatar seçenekleri.
- [ ] Gece / Gündüz modu butonu.
