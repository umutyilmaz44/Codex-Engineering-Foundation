<div align="center">

# Codex Engineering Foundation

**Prepare any project for everyday agentic engineering.**  
**Her projeyi günlük agentic mühendislik çalışmasına hazırla.**

[v2.3 · Foundation](./FOUNDATION.md)

Choose your language below. · Aşağıdan dilini seç.

</div>

---

<details>
<summary><strong>English — What it is & how to use it</strong></summary>

You open a project. The code is there, but the context is scattered: an old README, rules from a previous session, a test command nobody has checked, decisions that only exist in a conversation.

**Codex Engineering Foundation is a reusable Markdown guide that helps Codex turn that starting point into a usable engineering environment.** It inspects what exists, fills the important gaps, checks the result, and leaves project-specific guidance for everyday work.

Here, *agentic engineering* means working with a coding agent that can inspect files, make changes and run checks. The Foundation establishes the context and working conditions that help it do that consistently.

```text
Your project as it is
        ↓
Discover → Prepare or repair → Verify → Hand off
        ↓
Daily work through the project's own instructions
```

## When would I use it?

| Your starting point | What the Foundation helps establish |
| :--- | :--- |
| A new project | Enough direction, setup and guidance to begin development. |
| Existing code with no agent guidance | A way to understand, change and verify the project. |
| Conflicting or outdated agent instructions | A coherent working environment that preserves useful existing material. |
| A rebuild or modernization | A clear distinction between current behavior and the intended target. |
| An unfamiliar project | Reliable orientation, with important unknowns made visible. |

It adapts to the project. There is no required stack, folder layout, skill collection or multi-agent setup.

## Start in three steps

1. **Open your target project in Codex.** For a new project, provide its purpose and the constraints you already know.
2. **Make [the v2.3 guide](./FOUNDATION.md) available to that session.** Download it and attach it, or give Codex its accessible local file path. It does not have to live inside your project.
3. **Send the request below.** Replace the bracketed parts with your own information.

```text
Apply the attached Codex Engineering Foundation v2.3 to this project.

Project: [target directory]
Purpose and constraints: [what the project does and what matters]

Inspect the current code, documentation, instructions and working setup.
Preserve existing work and useful structure. Establish or repair the
smallest sufficient agentic engineering environment.

Ask only for important information you cannot discover.
Validate navigation and relevant working conditions without implementing
a product feature or turning an example task into assigned work.

Finish with READY or NOT READY for a clearly stated scope, the evidence,
remaining limitations, and where daily work should begin.
```

For an existing project, a short description is enough to start discovery. You do not need to write a full specification or pick the next feature before using the guide.

## What should I get back?

A future session should be able to answer:

- What is this project trying to do?
- Which instructions apply?
- Where is the relevant code and knowledge?
- How do I work on it and check a change?
- What remains unknown or unavailable?
- Where do I record decisions so the next session can continue?

The result may include an `AGENTS.md`, corrected documentation links, setup commands and maintenance instructions. The exact files depend on what the project already has. File count is not a measure of success.

**READY** means the environment supports the stated scope of work, with limitations made explicit. **NOT READY** means a specific environment gap still prevents that work. Neither result is a claim that the application is bug-free.

## Where does it stop?

The Foundation's job ends at the handoff. It can establish a small generic scaffold when needed, but it does not build the first feature, finish a historical bug fix or execute live business operations to prove readiness.

Afterward, start daily tasks from the project's own instructions. Keep useful knowledge current as code changes. Revisit the Foundation when the environment needs substantial repair or the project's direction changes.

You can keep the guide outside the project. If you retain a project-local copy, treat it as a setup reference rather than something every session must reread.

## What's in this repository?

| File | Role |
| :--- | :--- |
| [FOUNDATION.md](./FOUNDATION.md) | The English source guide to give Codex. |
| [README.md](./README.md) | English and Turkish introduction and usage. |

No package installation is required to read or apply the guide. The target project still needs its own tools, dependencies and access.

## Status and feedback

Version 2.3 has been exercised on a new project, an existing project without agent instructions, and a project whose agentic environment needed repair. These exercises led to revisions; they do not certify every stack or scenario. Broader modernization and recovery cases still need real-project validation.

Useful feedback describes the starting situation, what the guide caused, and what general rule would improve it. Keep private project details out of public reports.

---

**A successful setup leaves the next session somewhere clear to begin.**

</details>

<details>
<summary><strong>Türkçe — Nedir, nasıl kullanılır?</strong></summary>

Bir projeyi açıyorsun. Kod yerinde, ama bağlam dağınık: eski bir README, önceki oturumdan kalma kurallar, çalıştığı kontrol edilmemiş bir test komutu, yalnızca bir konuşmada duran kararlar.

**Codex Engineering Foundation, Codex'in bu başlangıç durumunu kullanılabilir bir mühendislik ortamına dönüştürmesine rehberlik eden, tekrar kullanılabilir bir Markdown dosyasıdır.** Mevcut yapıyı inceler, önemli eksikleri giderir, sonucu kontrol eder ve günlük işler için projeye özel yönlendirme bırakır.

Burada *agentic engineering*, dosyaları inceleyebilen, değişiklik yapabilen ve kontrolleri çalıştırabilen bir kodlama ajanıyla çalışmak demek. Foundation, bu çalışmanın tutarlı biçimde sürdürülebilmesi için gerekli bağlamı ve çalışma koşullarını kurar.

```text
Projenin mevcut durumu
        ↓
Keşfet → Kur veya onar → Doğrula → Devret
        ↓
Projenin kendi talimatlarıyla günlük çalışma
```

## Ne zaman kullanırım?

| Başlangıç durumun | Foundation'ın oluşturulmasına yardımcı olduğu yapı |
| :--- | :--- |
| Sıfırdan bir proje | Geliştirmeye başlamak için yeterli yön, kurulum ve çalışma rehberi. |
| Kodu olan, ajan yönlendirmesi olmayan proje | Projeyi anlama, değiştirme ve doğrulama yolu. |
| Çelişen veya eskimiş ajan talimatları | Yararlı bilgileri koruyan, tutarlı bir çalışma ortamı. |
| Yeniden geliştirme veya modernizasyon | Mevcut davranış ile hedeflenen durumun açıkça ayrılması. |
| Tanımadığın bir proje | Önemli belirsizlikleri görünür kılan, güvenilir bir başlangıç noktası. |

Projeye uyum sağlar. Zorunlu bir teknoloji, klasör düzeni, skill koleksiyonu veya çoklu ajan yapısı dayatmaz.

## Üç adımda başla

1. **Hedef projeyi Codex'te aç.** Yeni bir projeyse amacını ve bildiğin kısıtları belirt.
2. **[v2.3 rehberini](./FOUNDATION.md) o oturumun erişimine aç.** Dosyayı indirip ekle veya Codex'e erişebildiği yerel dosya yolunu ver. Dosyanın projenin içinde bulunması şart değil.
3. **Aşağıdaki isteği gönder.** Köşeli parantezli alanları kendi bilgilerinle değiştir.

```text
Eklediğim Codex Engineering Foundation v2.3 rehberini bu projeye uygula.

Proje: [hedef dizin]
Amaç ve kısıtlar: [proje ne yapıyor, nelere dikkat edilmeli]

Mevcut kodu, belgeleri, talimatları ve çalışma koşullarını incele.
Mevcut çalışmaları ve yararlı yapıyı koru. Yeterli olan en küçük
agentic engineering ortamını kur veya onar.

Yalnızca keşfederek bulamadığın önemli bilgileri sor.
Ürün özelliği geliştirmeden ve örnek bir işi atanmış göreve çevirmeden,
bilgiye erişim yollarını ve ilgili çalışma koşullarını doğrula.

Sonunda kapsamı açık bir READY veya NOT READY değerlendirmesi,
kanıtlar, kalan sınırlamalar ve günlük işe nereden başlanacağını belirt.
```

Mevcut bir projede kısa bir açıklama keşfe başlamak için yeterli. Rehberi kullanmadan önce kapsamlı bir şartname hazırlaman veya sıradaki özelliği seçmen gerekmiyor.

## Sonunda ne elde ederim?

Yeni bir oturum şu soruları cevaplayabilmeli:

- Bu projenin amacı ne?
- Hangi talimatlar geçerli?
- İlgili kod ve bilgi nerede?
- Nasıl çalışırım, yaptığım değişikliği nasıl kontrol ederim?
- Neler hâlâ bilinmiyor veya kullanılamıyor?
- Sonraki oturumun devam edebilmesi için kararları nereye kaydederim?

Sonuçta bir `AGENTS.md`, düzeltilmiş belge bağlantıları, kurulum komutları ve bilgi güncelleme talimatları bulunabilir. Hangi dosyalara ihtiyaç olduğu, projede zaten ne bulunduğuna bağlıdır. Başarı, üretilen dosya sayısıyla ölçülmez.

**READY**, belirtilen çalışma kapsamının desteklendiğini ve sınırlamaların açık olduğunu söyler. **NOT READY**, o çalışmayı engelleyen belirli bir ortam eksikliği kaldığını söyler. İkisi de uygulamanın hatasız olduğuna ilişkin bir iddia değildir.

## Nerede durur?

Foundation'ın görevi ortamı devrettiğinde biter. Gerektiğinde küçük, genel bir proje iskeleti hazırlayabilir; ancak hazır olmayı kanıtlamak için ilk özelliği geliştirmez, eski bir hatanın çözümünü tamamlamaz veya canlı iş işlemleri yürütmez.

Sonrasında günlük görevlere projenin kendi talimatlarından başla. Kod değiştikçe yararlı bilgileri güncel tut. Ortam ciddi onarım gerektirirse veya projenin yönü değişirse Foundation'a yeniden başvur.

Rehberi proje dışında tutabilirsin. Projede bir kopyasını saklarsan her oturumda yeniden okunması gereken talimat olarak değil, kurulum referansı olarak kullan.

## Bu repoda ne var?

| Dosya | Görevi |
| :--- | :--- |
| [FOUNDATION.md](./FOUNDATION.md) | Codex'e vereceğin İngilizce kaynak rehber. |
| [README.md](./README.md) | İngilizce ve Türkçe tanıtım ve kullanım. |

Rehberi okumak veya uygulamak için paket kurulumu gerekmiyor. Hedef projenin kendi araçlarına, bağımlılıklarına ve erişimlerine yine ihtiyaç var.

## Durum ve geri bildirim

V2.3; sıfırdan bir projede, ajan talimatları olmayan mevcut bir projede ve agentic ortamı onarım gerektiren bir projede denendi. Bu denemeler metnin iyileştirilmesini sağladı; her teknoloji veya senaryonun doğrulandığı anlamına gelmiyor. Daha kapsamlı modernizasyon ve proje kurtarma senaryoları gerçek proje doğrulaması bekliyor.

Yararlı geri bildirim; başlangıç durumunu, rehberin hangi sonuca yol açtığını ve hangi genel kuralın iyileştirilebileceğini anlatır. Özel proje bilgilerini herkese açık bildirimlere ekleme.

---

**Başarılı bir kurulum, sonraki oturuma açık bir başlangıç noktası bırakır.**

</details>
