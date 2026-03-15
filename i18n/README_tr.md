<!---
Copyright 2020 The HuggingFace Team. All rights reserved.

Licensed under the Apache License, Version 2.0 (the "License");
you may not use this file except in compliance with the License.
You may obtain a copy of the License at

    http://www.apache.org/licenses/LICENSE-2.0

Unless required by applicable law or agreed to in writing, software
distributed under the License is distributed on an "AS IS" BASIS,
WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
See the License for the specific language governing permissions and
limitations under the License.
-->

<p align="center">
  <picture>
    <source media="(prefers-color-scheme: dark)" srcset="https://huggingface.co/datasets/huggingface/documentation-images/raw/main/transformers-logo-dark.svg">
    <source media="(prefers-color-scheme: light)" srcset="https://huggingface.co/datasets/huggingface/documentation-images/raw/main/transformers-logo-light.svg">
    <img alt="Hugging Face Transformers Library" src="https://huggingface.co/datasets/huggingface/documentation-images/raw/main/transformers-logo-light.svg" width="352" height="59" style="max-width: 100%;">
  </picture>
  <br/>
  <br/>
</p>

<p align="center">
    <a href="https://huggingface.com/models"><img alt="Checkpoints on Hub" src="https://img.shields.io/endpoint?url=https://huggingface.co/api/shields/models&color=brightgreen"></a>
    <a href="https://circleci.com/gh/huggingface/transformers"><img alt="Build" src="https://img.shields.io/circleci/build/github/huggingface/transformers/main"></a>
    <a href="https://github.com/huggingface/transformers/blob/main/LICENSE"><img alt="GitHub" src="https://img.shields.io/github/license/huggingface/transformers.svg?color=blue"></a>
    <a href="https://huggingface.co/docs/transformers/index"><img alt="Documentation" src="https://img.shields.io/website/http/huggingface.co/docs/transformers/index.svg?down_color=red&down_message=offline&up_message=online"></a>
    <a href="https://github.com/huggingface/transformers/releases"><img alt="GitHub release" src="https://img.shields.io/github/release/huggingface/transformers.svg"></a>
    <a href="https://github.com/huggingface/transformers/blob/main/CODE_OF_CONDUCT.md"><img alt="Contributor Covenant" src="https://img.shields.io/badge/Contributor%20Covenant-v2.0%20adopted-ff69b4.svg"></a>
    <a href="https://zenodo.org/badge/latestdoi/155220641"><img src="https://zenodo.org/badge/155220641.svg" alt="DOI"></a>
</p>

<h4 align="center">
    <p>
        <a href="https://github.com/huggingface/transformers/blob/main/README.md">English</a> |
        <a href="https://github.com/huggingface/transformers/blob/main/i18n/README_zh-hans.md">简体中文</a> |
        <a href="https://github.com/huggingface/transformers/blob/main/i18n/README_zh-hant.md">繁體中文</a> |
        <a href="https://github.com/huggingface/transformers/blob/main/i18n/README_ko.md">한국어</a> |
        <a href="https://github.com/huggingface/transformers/blob/main/i18n/README_es.md">Español</a> |
        <a href="https://github.com/huggingface/transformers/blob/main/i18n/README_ja.md">日本語</a> |
        <a href="https://github.com/huggingface/transformers/blob/main/i18n/README_hd.md">हिन्दी</a> |
        <a href="https://github.com/huggingface/transformers/blob/main/i18n/README_ru.md">Русский</a> |
        <a href="https://github.com/huggingface/transformers/blob/main/i18n/README_pt-br.md">Português</a> |
        <a href="https://github.com/huggingface/transformers/blob/main/i18n/README_te.md">తెలుగు</a> |
        <a href="https://github.com/huggingface/transformers/blob/main/i18n/README_fr.md">Français</a> |
        <a href="https://github.com/huggingface/transformers/blob/main/i18n/README_de.md">Deutsch</a> |
        <a href="https://github.com/huggingface/transformers/blob/main/i18n/README_it.md">Italiano</a> |
        <a href="https://github.com/huggingface/transformers/blob/main/i18n/README_vi.md">Tiếng Việt</a> |
        <a href="https://github.com/huggingface/transformers/blob/main/i18n/README_ar.md">العربية</a> |
        <a href="https://github.com/huggingface/transformers/blob/main/i18n/README_ur.md">اردو</a> |
        <a href="https://github.com/huggingface/transformers/blob/main/i18n/README_bn.md">বাংলা</a> |
        <b>Türkçe</b>
    </p>
</h4>

<h3 align="center">
    <p>Çıkarım (inference) ve eğitim için son model eğitilmiş modeller</p>
</h3>

<h3 align="center">
    <img src="https://huggingface.co/datasets/huggingface/documentation-images/resolve/main/transformers/transformers_as_a_model_definition.png"/>
</h3>

Transformers; metin, görüntü işleme, ses, video ve çok modelli (multimodal) modeller için en son teknoloji makine öğrenmesi süreçlerinde, hem çıkarım (inference) hem de eğitim aşamalarında bir model tanımlama çerçevesi (framework) işlevi görür.

Transformers, model tanımlamasını merkezileştirerek bu tanımın tüm ekosistem genelinde üzerinde ortak bir standart halini alır. `transformers` farklı çalışma yapıları (frameworks) içerisinde merkezi bir konumdadır: Eğer model tanımlamasını destekliyorsa, Çoğu eğitim frameworkleri (Axolotl, Unsloth, DeepSpeed, FSDP, PyTorch-Lightning, ...), çıkarım motorları (inference engine) (vLLM, SGLang, TGI, ...) ve model tanımını transformers'tan alan modelleme kütüphaneleri (llama.cpp, mlx, ...) ile uyumlu çalışabilir.

Yeni ve en gelişmiş modelleri desteklemeye yardımcı olmayı ve model tanımlarının basit, özelleştirilebilir ve verimli olmasını sağlayarak bu modellerin kullanımını demokratikleştirmeyi vaat ediyoruz.

Hugging Face Hub'da kullanabileceğiniz 1M+'dan fazla Transformer [model checkpointi](https://huggingface.co/models?library=transformers&sort=trending) var.

Transformers'ı şu anda kullanmaya başlayacağın bir model bulmak için [Hub](https://huggingface.com/)'ı bugün keşfet.

## Kurulum

Transformers kütüphanesi Python 3.10+ ve [PyTorch](https://pytorch.org/get-started/locally/) 2.4+ sürümleriyle birlikte çalışır.

[venv](https://docs.python.org/3/library/venv.html) ya da [uv](https://docs.astral.sh/uv/) (Rust tabanlı Python paket ve proje yöneticisi) kullanarak bir sanal ortam (virtual environment) oluştur ve aktive et.

```py
# venv
python -m venv .my-env
source .my-env/bin/activate
# uv
uv venv .my-env
source .my-env/bin/activate
```

Transformers kütüphanesini sanal ortamına kur.

```py
# pip
pip install "transformers[torch]"

# uv
uv pip install "transformers[torch]"
```

Kütüphanedeki en son değişiklikleri kullanmak veya katkıda (contribution) bulunmak istiyorsanız Transformers'ı kaynak kodundan kurun. Ancak *en son* sürüm kararlı olmayabilir. Bir hatayla karşılaşırsanız çekinmeden bir [issue](https://github.com/huggingface/transformers/issues) açabilirsiniz.

```shell
git clone https://github.com/huggingface/transformers.git
cd transformers

# pip
pip install '.[torch]'

# uv
uv pip install '.[torch]'
```

## Hızlı Başlangıç

Transformers'ı kullanmaya [Pipeline](https://huggingface.co/docs/transformers/pipeline_tutorial) API'sini kullanarak başlayabilirsiniz. `Pipeline` high-level (insan diline daha yakın) bir çıkarım (inference) sınıfıdır. Pipeline metin, ses, görüntü ve multimodal görevleri destekler. Girdiyi (input) ön işleyip uygun çıktıyı (output) döndürür.

Bir pipeline oluşturalım ve metin üretimi için kullanılacak modeli belirleyelim. Önce model indirilir ve önbelleğe alınır, böylece daha sonra tekrar kolayca kullanabilirsiniz. Son olarak ise modeli tetiklemek (promptlamak) için bir miktar metin verelim.

```py
from transformers import pipeline

pipeline = pipeline(task="text-generation", model="Qwen/Qwen2.5-1.5B")
pipeline("the secret to baking a really good cake is ")
[{'generated_text': 'the secret to baking a really good cake is 1) to use the right ingredients and 2) to follow the recipe exactly. the recipe for the cake is as follows: 1 cup of sugar, 1 cup of flour, 1 cup of milk, 1 cup of butter, 1 cup of eggs, 1 cup of chocolate chips. if you want to make 2 cakes, how much sugar do you need? To make 2 cakes, you will need 2 cups of sugar.'}]
```

Model ile iletişim kurmak için ise kullanım şekli aynıdır. Tek fark, sistem ile sizin aranızda bir chat geçmişi kurmanız gerekmektedir (Pipeline'a gidecek input).

> [!TIP]
> [`transformers serve` çalıştığı](https://huggingface.co/docs/transformers/main/en/serving) sürece, komut istemi ile de direkt bir şekilde model ile iletişim kurabilirsiniz.
> ```shell
> transformers chat Qwen/Qwen2.5-0.5B-Instruct
> ```

```py
import torch
from transformers import pipeline

chat = [
    {"role": "system", "content": "You are a sassy, wise-cracking robot as imagined by Hollywood circa 1986."},
    {"role": "user", "content": "Hey, can you tell me any fun things to do in New York?"}
]

pipeline = pipeline(task="text-generation", model="meta-llama/Meta-Llama-3-8B-Instruct", dtype=torch.bfloat16, device_map="auto")
response = pipeline(chat, max_new_tokens=512)
print(response[0]["generated_text"][-1]["content"])
```

Aşağıdaki örnekleri genişleterek `Pipeline` API'sinin farklı görev ve modalitelerde nasıl kullanıldığını görebilirsiniz.

<details>
<summary>Otomatik konuşma tanıma (Automatic speech recognition)</summary>

```py
from transformers import pipeline

pipeline = pipeline(task="automatic-speech-recognition", model="openai/whisper-large-v3")
pipeline("https://huggingface.co/datasets/Narsil/asr_dummy/resolve/main/mlk.flac")
{'text': ' I have a dream that one day this nation will rise up and live out the true meaning of its creed.'}
```

</details>

<details>
<summary>Görüntü sınıflandırma (Image classification)</summary>

<h3 align="center">
    <a><img src="https://huggingface.co/datasets/Narsil/image_dummy/raw/main/parrots.png"></a>
</h3>

```py
from transformers import pipeline

pipeline = pipeline(task="image-classification", model="facebook/dinov2-small-imagenet1k-1-layer")
pipeline("https://huggingface.co/datasets/Narsil/image_dummy/raw/main/parrots.png")
[{'label': 'macaw', 'score': 0.997848391532898},
 {'label': 'sulphur-crested cockatoo, Kakatoe galerita, Cacatua galerita',
  'score': 0.0016551691805943847},
 {'label': 'lorikeet', 'score': 0.00018523589824326336},
 {'label': 'African grey, African gray, Psittacus erithacus',
  'score': 7.85409429227002e-05},
 {'label': 'quail', 'score': 5.502637941390276e-05}]
```

</details>

<details>
<summary>Görsel soru cevaplama (Visual question answering)</summary>

<h3 align="center">
    <a><img src="https://huggingface.co/datasets/huggingface/documentation-images/resolve/main/transformers/tasks/idefics-few-shot.jpg"></a>
</h3>

```py
from transformers import pipeline

pipeline = pipeline(task="visual-question-answering", model="Salesforce/blip-vqa-base")
pipeline(
    image="https://huggingface.co/datasets/huggingface/documentation-images/resolve/main/transformers/tasks/idefics-few-shot.jpg",
    question="What is in the image?",
)
[{'answer': 'statue of liberty'}]
```

</details>

## Neden Transformers kullanmalıyım?

1. Son modelleri kullanım kolaylığı:
    - Doğal dil anlama ve üretimi, bilgisayarlı görü, ses, video ve çoklu modal (multimodal) görevlerde yüksek performans.
    - Araştırmacılar, mühendisler ve geliştiriciler için düşük giriş engeli.
    - Öğrenilmesi gereken yalnızca üç sınıf ile az sayıda kullanıcıya yönelik soyutlama.
    - Tüm önceden eğitilmiş modelleri kullanmak için birleşik bir API.

1. Daha düşük hesaplama maliyeti, daha küçük karbon ayak izi:
    - Sıfırdan eğitmek yerine eğitilmiş modelleri paylaşma.
    - Hesaplama süresini ve üretim maliyetlerini azaltma.
    - Tüm modalitelerde 1 milyondan fazla önceden eğitilmiş checkpoint içeren onlarca model mimarisi.

1. Bir modelin yaşam döngüsünün her aşaması için doğru framework'ü seçme:
    - En gelişmiş modelleri 3 satır kod ile eğitme.
    - Tek bir modeli isteğe bağlı olarak PyTorch / JAX / TF2.0 framework'leri arasında taşıma.
    - Eğitim, değerlendirme ve üretim için en uygun framework'ü seçme.

1. Bir modeli veya örneği ihtiyaçlarınıza göre kolayca özelleştirme:
    - Her mimari için, orijinal yazarların yayımladığı sonuçları yeniden üretmeye yönelik örnekler sağlıyoruz.
    - Modelin iç yapısı mümkün olduğunca tutarlı şekilde erişilebilir durumdadır.
    - Model dosyaları, hızlı deneyler için kütüphaneden bağımsız olarak da kullanılabilir.

<a target="_blank" href="https://huggingface.co/enterprise">
    <img alt="Hugging Face Enterprise Hub" src="https://github.com/user-attachments/assets/247fb16d-d251-4583-96c4-d3d76dda4925">
</a><br>

## Neden Transformers kullanmamalıyım?

- Bu kütüphane, sinir ağları için modüler yapı taşlarından oluşan bir araç kutusu değildir. Model dosyalarındaki kod, araştırmacıların ek soyutlamalara/dosyalara dalmadan her bir model üzerinde hızla iterasyon yapabilmesi için bilerek ek soyutlamalarla yeniden düzenlenmemiştir.
- Eğitim API'si, Transformers tarafından sağlanan PyTorch modelleriyle çalışmak üzere optimize edilmiştir. Genel makine öğrenmesi döngüleri için [Accelerate](https://huggingface.co/docs/accelerate) gibi başka bir kütüphane kullanmalısınız.
- [Örnek script'ler](https://github.com/huggingface/transformers/tree/main/examples) yalnızca *örnek* niteliğindedir. Sizin özel kullanım durumunuzda birebir çalışmayabilir ve kodu kendi ihtiyaçlarınıza göre uyarlamanız gerekebilir.

## Transformers kullanan 100 proje

Transformers, yalnızca önceden eğitilmiş modelleri kullanmak için bir araç seti değil, aynı zamanda etrafında ve Hugging Face Hub'da oluşturulmuş bir proje topluluğudur. Transformers'ın geliştiricilerin, araştırmacıların, öğrencilerin, profesörlerin, mühendislerin ve herkesin hayallerindeki projeleri inşa etmesine olanak tanımasını istiyoruz.

Transformers'ın 100.000 yıldızını kutlamak için, Transformers ile oluşturulmuş 100 harika projeyi listeleyen [awesome-transformers](./awesome-transformers.md) sayfasıyla topluluğa dikkat çekmek istedik.

Listenin parçası olması gerektiğine inandığınız bir projeniz varsa veya kullanıyorsanız, lütfen eklemek için bir PR açın!

## Örnek modeller

Modellerimizin çoğunu doğrudan [Hub model sayfalarında](https://huggingface.co/models) test edebilirsiniz.

Çeşitli kullanım alanları için örnek modelleri görmek üzere aşağıdaki her bir modaliteyi genişletin.

<details>
<summary>Ses (Audio)</summary>

- [CLAP](https://huggingface.co/laion/clap-htsat-fused) ile ses sınıflandırma
- [Parakeet](https://huggingface.co/nvidia/parakeet-ctc-1.1b#transcribing-using-transformers-%F0%9F%A4%97), [Whisper](https://huggingface.co/openai/whisper-large-v3-turbo), [GLM-ASR](https://huggingface.co/zai-org/GLM-ASR-Nano-2512) ve [Moonshine-Streaming](https://huggingface.co/UsefulSensors/moonshine-streaming-medium) ile otomatik konuşma tanıma
- [Wav2Vec2](https://huggingface.co/superb/wav2vec2-base-superb-ks) ile anahtar kelime tespiti
- [Moshi](https://huggingface.co/kyutai/moshiko-pytorch-bf16) ile konuşmadan konuşmaya üretim
- [MusicGen](https://huggingface.co/facebook/musicgen-large) ile metinden sese dönüştürme
- [CSM](https://huggingface.co/sesame/csm-1b) ile metinden konuşmaya dönüştürme

</details>

<details>
<summary>Bilgisayarlı Görü (Computer Vision)</summary>

- [SAM](https://huggingface.co/facebook/sam-vit-base) ile otomatik maske oluşturma
- [DepthPro](https://huggingface.co/apple/DepthPro-hf) ile derinlik tahmini
- [DINO v2](https://huggingface.co/facebook/dinov2-base) ile görüntü sınıflandırma
- [SuperPoint](https://huggingface.co/magic-leap-community/superpoint) ile anahtar nokta tespiti
- [SuperGlue](https://huggingface.co/magic-leap-community/superglue_outdoor) ile anahtar nokta eşleştirme
- [RT-DETRv2](https://huggingface.co/PekingU/rtdetr_v2_r50vd) ile nesne tespiti
- [VitPose](https://huggingface.co/usyd-community/vitpose-base-simple) ile poz tahmini
- [OneFormer](https://huggingface.co/shi-labs/oneformer_ade20k_swin_large) ile evrensel segmentasyon
- [VideoMAE](https://huggingface.co/MCG-NJU/videomae-large) ile video sınıflandırma

</details>

<details>
<summary>Çoklu Modal (Multimodal)</summary>

- [Voxtral](https://huggingface.co/mistralai/Voxtral-Mini-3B-2507), [Audio Flamingo](https://huggingface.co/nvidia/audio-flamingo-3-hf) ile ses veya metinden metne dönüştürme
- [LayoutLMv3](https://huggingface.co/microsoft/layoutlmv3-base) ile doküman soru cevaplama
- [Qwen-VL](https://huggingface.co/Qwen/Qwen2.5-VL-3B-Instruct) ile görüntü veya metinden metne dönüştürme
- [BLIP-2](https://huggingface.co/Salesforce/blip2-opt-2.7b) ile görüntü açıklama (captioning)
- [GOT-OCR2](https://huggingface.co/stepfun-ai/GOT-OCR-2.0-hf) ile OCR tabanlı doküman anlama
- [TAPAS](https://huggingface.co/google/tapas-base) ile tablo soru cevaplama
- [Emu3](https://huggingface.co/BAAI/Emu3-Gen) ile birleşik çoklu modal anlama ve üretim
- [Llava-OneVision](https://huggingface.co/llava-hf/llava-onevision-qwen2-0.5b-ov-hf) ile görüntüden metne dönüştürme
- [Llava](https://huggingface.co/llava-hf/llava-1.5-7b-hf) ile görsel soru cevaplama
- [Kosmos-2](https://huggingface.co/microsoft/kosmos-2-patch14-224) ile görsel referans ifade segmentasyonu

</details>

<details>
<summary>Doğal Dil İşleme (NLP)</summary>

- [ModernBERT](https://huggingface.co/answerdotai/ModernBERT-base) ile maskeli kelime tamamlama
- [Gemma](https://huggingface.co/google/gemma-2-2b) ile adlandırılmış varlık tanıma (NER)
- [Mixtral](https://huggingface.co/mistralai/Mixtral-8x7B-v0.1) ile soru cevaplama
- [BART](https://huggingface.co/facebook/bart-large-cnn) ile özetleme
- [T5](https://huggingface.co/google-t5/t5-base) ile çeviri
- [Llama](https://huggingface.co/meta-llama/Llama-3.2-1B) ile metin üretimi
- [Qwen](https://huggingface.co/Qwen/Qwen2.5-0.5B) ile metin sınıflandırma

</details>

## Atıf (Citation)

Transformers kütüphanesi için atıf yapabileceğiniz bir [makalemiz](https://www.aclweb.org/anthology/2020.emnlp-demos.6/) bulunmaktadır:
```bibtex
@inproceedings{wolf-etal-2020-transformers,
    title = "Transformers: State-of-the-Art Natural Language Processing",
    author = "Thomas Wolf and Lysandre Debut and Victor Sanh and Julien Chaumond and Clement Delangue and Anthony Moi and Pierric Cistac and Tim Rault and Rémi Louf and Morgan Funtowicz and Joe Davison and Sam Shleifer and Patrick von Platen and Clara Ma and Yacine Jernite and Julien Plu and Canwen Xu and Teven Le Scao and Sylvain Gugger and Mariama Drame and Quentin Lhoest and Alexander M. Rush",
    booktitle = "Proceedings of the 2020 Conference on Empirical Methods in Natural Language Processing: System Demonstrations",
    month = oct,
    year = "2020",
    address = "Online",
    publisher = "Association for Computational Linguistics",
    url = "https://www.aclweb.org/anthology/2020.emnlp-demos.6",
    pages = "38--45"
}
```
