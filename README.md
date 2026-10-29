# SE Primer

SE Primer, sağlık randevu sistemi krizi üzerinden mimari, test ve KVKK kararlarını öğreten kişiselleştirilmiş mobil web oyunudur.

## Çalıştırma

```bash
npm run dev
```

Tarayıcıda `http://localhost:5173` adresini açın. Uygulamanın çalışması için yalnızca Node.js gerekir; Cypress testleri için ayrıca `npm install` çalıştırılmalıdır.

## Test ve derleme

```bash
npm run build
npm run test:e2e
```

Cypress; kişiselleştirme zorunluluğunu, iyi sonu, KVKK ihlalini, testsiz yayın sonucunu ve yeniden başlatmayı test eder. Test videosu koşu sonunda `cypress/videos/` altında üretilir.

## Teslim kanıtları

- Ürün spesifikasyonu ve kabul örnekleri: [`spec.md`](./spec.md)
- Tasarım sistemi ve Stitch istemi: [`DESIGN.md`](./DESIGN.md)
- 20 cevaplık tutor değerlendirmesi: [`eval/tutor-eval.md`](./eval/tutor-eval.md)
- Cypress E2E senaryoları: [`cypress/e2e/game.cy.js`](./cypress/e2e/game.cy.js)
- Çalışan uygulama: `src/main.js` ve `src/styles.css`
- 60 saniyelik demo: [`docs/se-primer-demo-60s.gif`](./docs/se-primer-demo-60s.gif)
- Teslim özeti: [`TESLIM.md`](./TESLIM.md)

## Bilinçli olarak yapılmayan üç özellik

1. **Kullanıcı hesabı:** Bir haftalık eğitim prototipinde öğrenme akışına katkısı olmadığı için yapılmadı.
2. **İkinci vaka:** Üç kararın sonuçlarını ve tutor kalitesini derinlemesine sınamak için kapsam tek sağlık vakasıyla tutuldu.
3. **Gerçek hasta verisi:** Mahremiyet ve güvenlik nedeniyle yalnızca tamamen kurgusal içerik kullanıldı.

## Kişiselleştirme

Seviye, rol ve öğrenme hedefi tutor metinlerini değiştirir. Başlangıç seviyesinde açıklayıcı destek; DevOps rolünde dağıtım ve geri dönüş; test hedefinde kritik akış; güvenlik hedefinde veri minimizasyonu öne çıkar.

## Yayınlama kontrol listesi

- [ ] Repoyu GitHub'a gönder ve bağlantıyı Classroom'a ekle.
- [ ] Uygulamayı Google AI Studio'ya aktar/yayınla ve bağlantıyı ekle.
- [ ] Stitch istemiyle ekranları üretip bağlantıyı ve ekran görüntülerini `DESIGN.md`ye ekle.
- [ ] `npm run test:e2e` videosundan yaklaşık 60 saniyelik demo hazırla ve bağlantıyı ekle.

Hesap yetkisi gerektiren bu dört yayınlama işlemi yerel proje oluşturulurken otomatik yapılmamıştır; uygulama, belgeler ve test kanıtı hazırdır.
