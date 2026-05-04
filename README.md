# Azərbaycan Dili üçün Nitq Tanıma Sistemi

## Layihənin qısa izahatı
Bu layihədə Mozilla Common Voice datasetindən istifadə edərək Azərbaycan dili üçün avtomatik nitq tanıma (STT) sistemi qurulmuşdur.
[https://commonvoice.mozilla.org/az](https://mozilladatacollective.com/datasets/cmn29hqvk015ko107fblsr5ay)

## İstifadə olunan model və parametrlər
- Model: openai/whisper-small
- Dil: Azerbaijani (az)
- Task: Transcribe

## WER/CER nəticələri
Aşağıdakı cədvəldə modelin həm baza, həm də fine-tuning nəticələri göstərilmişdir:

| Model              |   WER   |   CER   |
| Base Whisper       | 0.6011  | 0.1689  |
| Fine-tuned Whisper | 0.0883  | 0.0221  |

## 🚀 Kodu işə salmaq üçün addımlar
 Notebook-ları part_a/ və part_b/ qovluqlarından ardıcıllıqla işə salın.

## 🔄 Fine-tuning nəticəsinin müqayisəsi
WER-də böyük yaxşılaşma var 60% → 8.8%
yəni model artıq sözlərin çoxunu düzgün tanıyır (təxminən 7 dəfə yaxşılaşıb)
CER də ciddi azalıb 16.8% → 2.2%
bu da göstərir ki, model təkcə sözləri yox, hərf səviyyəsində də çox daha dəqiqdir
