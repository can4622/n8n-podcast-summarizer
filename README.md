🎙️ Podcast Özetleyici — n8n Workflow
Her gün 4 farklı podcastin RSS beslemesini otomatik çeken, yapay zeka ile Türkçe özetleyen ve Telegram'a gönderen otomasyon.
Ne Yapar?
Manuel dinleme gerekmeden, belirlenen saatte yeni bölümler otomatik özetlenerek Telegram'a düşer.
Takip Edilen Podcastler
PodcastKonuLex FridmanTeknoloji, bilim, felsefe söyleşileriMy First MillionGirişimcilik ve iş fikirleriHow I Built ThisKurucuların hikayesi (NPR)Tim FerrissVerimlilik, yatırım, yaşam tasarımı

Workflow Adımları

Zamanlama Tetikleyicisi — Günlük otomatik başlatır
JavaScript — 4 podcast RSS URL'sini hazırlar
HTTP İsteği — Her RSS beslemesinden yeni bölümü çeker
JavaScript — Ham XML'i parse eder, HTML taglarını temizler
AI Modeli — Bölümü Türkçe olarak özetler
Telegram — Özeti kanala/gruba iletir

Kurulum

workflow.json dosyasını n8n'e import edin
Ayarlar → Import workflow → workflow.json
Credential'ları tanımlayın:

Telegram Bot Token + Chat ID
OpenAI API anahtarı


Zamanlama node'unda saati ayarlayın
Workflow'u aktif edin

Gereksinimler

n8n (self-hosted veya cloud)
Telegram Bot
OpenAI veya uyumlu bir AI API anahtarı
