<div align="center">

# Codex Engineering Foundation

**Prepare any project for everyday agentic engineering.**  
**Her projeyi günlük agentic mühendislik çalışmasına hazırla.**

[v2.3 · FOUNDATION.md](./FOUNDATION.md)

Choose your language. · Dilini seç.

</div>

---

<details>
<summary><strong>English — Overview, scenarios & copy-ready prompts</strong></summary>

## What is it?

**One Markdown guide for establishing or repairing the environment a coding agent needs to work on your project.** Give it to Codex in the target project. It helps Codex discover the code and intent, resolve important gaps, establish working instructions, check relevant tools, and hand daily work over to project-local guidance.

An *agentic engineering environment* is the combination of instructions, accessible project knowledge, tools, verification paths and continuity between sessions. The Foundation adapts these to your project; it does not require a particular stack or folder template.

```text
Inspect the project → Establish or repair the environment → Verify → Hand off
```

**The deliverable is a usable working environment.** Product development starts afterward. Setup may include a small generic scaffold, but does not implement a feature or complete a bug fix as proof of readiness.

## Before you start

1. Open the **target project** in Codex, rather than this guide's repository. For a new project, use its intended directory.
2. Download or attach [FOUNDATION.md](./FOUNDATION.md), or provide its accessible local path. No package installation is needed for the guide.
3. Choose the matching scenario below. Replace the bracketed fields and remove examples that do not apply. Each prompt is standalone.

You do not need a full specification or a selected backlog item. State what you know; leave unknowns visible. Examples below are illustrative, not required technologies or project structures.

## Choose your starting point

| Situation | Use |
| :--- | :--- |
| No implementation yet | **1 · New project** |
| Existing code, no agent guidance | **2 · Establish an environment** |
| Guidance exists but is unreliable | **3 · Repair an environment** |
| Rebuilding or changing the system's direction | **4 · Modernization** |
| Taking over a project with little reliable context | **5 · Project recovery** |
| Environment already works; you want to check it | **6 · Readiness check** |

### 1 · New project

**Example:** A booking application whose users and platform are known, but whose code has not been written.

**Steps:** Provide the project purpose and known constraints → let Codex resolve setup-critical questions → review the environment handoff before assigning implementation.

```text
Apply the attached FOUNDATION.md (v2.3) to a new project.
Target directory: [path]
Purpose and users: [e.g. bookings for a small service business]
Known constraints: [platform, stack if chosen, data or delivery constraints]
Undecided: [important choices still open]

Establish the smallest environment needed to begin engineering.
Ask only for missing decisions that affect setup. Prepare generic
scaffolding only where needed; do not implement the first feature.
Validate context navigation and applicable working conditions.
Report READY or NOT READY, scope, evidence, limits and the daily entry point.
```

**Expected handoff:** Project direction, working instructions, initial setup/verification paths, and visible decisions still needed for later tasks.

### 2 · Existing code, no agent guidance

**Example:** A backend already used by a team, with a short README and undocumented working practices.

**Steps:** Provide the repository and a short purpose → let Codex discover code, configuration and existing checks → review the guidance and execution limits it leaves behind.

```text
Apply the attached FOUNDATION.md (v2.3) to this existing project.
Repository: [path]
Purpose: [what the system does]
Known operating constraints: [if any]

Inspect code, documentation, configuration and existing checks before
asking questions. Establish missing project-local instructions,
context navigation, verification guidance and knowledge maintenance.
Preserve existing structure and uncommitted work. Use a relevant
existing workflow as a navigation example, not an assigned product task.
Inspect command side effects before running appropriate basic checks.
Do not fix application bugs or migrate business data during setup.
Report READY or NOT READY, evidence, limits and where daily work begins.
```

**Expected handoff:** A discoverable path from instructions to relevant code and checks, with observed behavior distinguished from accepted requirements.

### 3 · Existing environment needs repair

**Example:** AGENTS.md conflicts with another guide, links point to removed files, or every session loads too much context.

**Steps:** Describe symptoms you have noticed → let Codex compare instructions with their scope and evidence → review focused repairs and what was preserved.

```text
Apply the attached FOUNDATION.md (v2.3) to repair this agentic environment.
Repository: [path]
Symptoms: [e.g. conflicting instructions, stale paths, repeated discovery]
Preferences to preserve: [known working agreements, if any]

Audit existing instructions, context documents, skills and verification
routes. Identify concrete conflicts and gaps before changing them.
Preserve useful structure and user preferences; do not create a parallel
instruction system. Mark obsolete guidance clearly and preserve useful
history. Repair only justified environment issues, not product code.
Validate task navigation and appropriate working conditions.
Report repairs, preserved material, evidence and scoped READY/NOT READY.
```

**Expected handoff:** Clear authority, working references and coherent daily guidance within the existing structure.

### 4 · Rebuild or modernization

**Example:** Replacing a desktop application with a web application while preserving selected business workflows.

**Steps:** Identify current and target locations → explain why change is needed and what must be preserved → resolve material target gaps before environment setup is declared complete.

```text
Apply the attached FOUNDATION.md (v2.3) for modernization setup.
Current system: [path or accessible sources]
Target project: [path; may be the same repository]
Reason for change: [why]
Target direction: [what should change]
Must preserve: [workflows, contracts or compatibility]
Migration and operating constraints: [known limits or unknowns]

Distinguish current implementation from accepted target intent.
Do not assume every legacy behavior must be copied or discarded.
Resolve missing target decisions only where they block environment
readiness. Establish target guidance, reference navigation and verification
paths. Do not implement the rewrite or execute a data migration.
Report READY or NOT READY with evidence, unresolved decisions and handoff.
```

**Expected handoff:** A usable target environment with explicit preservation/change decisions and links to relevant legacy evidence.

### 5 · Unfamiliar project or missing context

**Example:** An inherited repository with old documents and no reliable setup explanation.

**Steps:** Share available sources and known facts → let Codex recover minimum reliable context → review confirmed findings, uncertainties and any access blockers.

```text
Apply the attached FOUNDATION.md (v2.3) to recover this project's context.
Repository: [path]
What I know: [brief facts, or unknown]
Other available sources: [documents or references, if any]

Recover enough reliable understanding to establish an engineering
environment. Distinguish observed facts, inferences and unknowns.
Do not invent requirements or treat old documentation as current truth.
Preserve existing work. Build the smallest useful navigation and working
guidance; inspect execution side effects before basic checks.
Do not redesign the system or start a product task.
Report scoped READY/NOT READY, evidence and remaining information needs.
```

**Expected handoff:** Reliable orientation and a clear account of what remains unknown, rather than a fabricated specification.

### 6 · Already prepared: check readiness

**Example:** A project has maintained instructions and checks; you want to know whether anything important is missing.

**Steps:** Identify the daily-work scope → request an inspection-only assessment → decide separately whether reported gaps need repair.

```text
Use the attached FOUNDATION.md (v2.3) to assess this environment.
Repository: [path]
Intended daily-work scope: [what engineers need to do]

Inspect existing guidance and walk through a relevant task's context
and verification route. Run only appropriate non-destructive basic checks
within existing permissions. Do not edit project files or generate a new
instruction structure. Report READY or NOT READY with concrete evidence,
limits and the smallest repairs needed, if any.
```

**Expected handoff:** A supported readiness conclusion. An already adequate environment does not need new files.

## How to read the result

| Result | Meaning | Your next step |
| :--- | :--- | :--- |
| **READY** | The stated engineering scope is supported; limits are explicit. | Start a daily task from the project's own instructions. |
| **NOT READY** | A specific environment gap prevents that scope. | Resolve the named prerequisite or decision, then reassess the affected capability. |

Look for evidence: instructions can be found, code and knowledge are reachable, applicable checks have actual outcomes, and future sessions know where decisions belong. File creation alone is not success. A passing build is not product acceptance; an untested future integration is not automatically a setup blocker.

## After the handoff

Use project-local instructions for everyday tasks and update useful knowledge as the project changes. Keep FOUNDATION.md as an optional setup reference, inside or outside the project. Reapply it for substantial environment repair or a change of direction, not every coding session.

## Files and validation status

- **[FOUNDATION.md](./FOUNDATION.md):** The English source guide applied by Codex.
- **README.md:** This bilingual usage guide; the prompts supplement the Foundation.

V2.3 has been exercised in real new-project, existing-code and environment-repair cases. Broader modernization and recovery still need real-project validation. Finalized wording does not certify every scenario or stack.

Feedback is most useful when it describes the starting situation, the environment failure and a reusable improvement. Keep private project details out of public reports.

</details>

<details>
<summary><strong>Türkçe — Tanıtım, senaryolar ve hazır promptlar</strong></summary>

## Nedir?

**Bir kodlama ajanının projende çalışabilmesi için gereken ortamı kurmaya veya onarmaya yönelik tek bir Markdown rehberi.** Hedef projede Codex'e verirsin. Kodu ve amacı keşfetmesine, önemli eksikleri gidermesine, çalışma talimatlarını oluşturmasına, ilgili araçları kontrol etmesine ve günlük işleri projeye özel yönlendirmeye devretmesine yardımcı olur.

*Agentic engineering ortamı*; talimatlar, erişilebilir proje bilgisi, araçlar, doğrulama yolları ve oturumlar arası devamlılığın birleşimidir. Foundation bunları projeye uyarlar; belirli bir teknoloji veya klasör şablonu dayatmaz.

```text
Projeyi incele → Ortamı kur veya onar → Doğrula → Günlük çalışmaya devret
```

**Ortaya çıkması gereken sonuç, kullanılabilir bir çalışma ortamıdır.** Ürün geliştirme sonrasında başlar. Kurulum gerektiğinde genel bir proje iskeleti içerebilir; ancak hazır olmayı kanıtlamak için özellik geliştirmez veya hata çözümünü tamamlamaz.

## Başlamadan önce

1. Codex'te bu rehberin reposunu değil, **üzerinde çalışacağın projeyi** aç. Yeni projeyse hedef dizini kullan.
2. [FOUNDATION.md](./FOUNDATION.md) dosyasını indirip oturuma ekle veya erişilebilir yerel yolunu belirt. Rehber için paket kurulumu gerekmez.
3. Aşağıdan uygun senaryoyu seç. Köşeli parantezleri doldur, geçerli olmayan örnekleri çıkar. Her prompt tek başına kullanılabilir.

Tam bir şartname veya seçilmiş bir sonraki görev gerekmiyor. Bildiklerini belirt, bilinmeyenleri açık bırak. Aşağıdaki örnekler zorunlu teknoloji veya proje yapıları değildir.

## Başlangıç durumunu seç

| Durum | Kullanılacak senaryo |
| :--- | :--- |
| Henüz uygulama kodu yok | **1 · Yeni proje** |
| Kod var, ajan yönlendirmesi yok | **2 · Ortam kurma** |
| Talimatlar var ama güvenilir değil | **3 · Ortam onarma** |
| Sistem yeniden geliştiriliyor veya yön değiştiriyor | **4 · Modernizasyon** |
| Projeyi devraldın, güvenilir bağlam az | **5 · Proje bağlamını kurtarma** |
| Ortam çalışıyor, yeterliliğini kontrol etmek istiyorsun | **6 · Hazırlık kontrolü** |

### 1 · Sıfırdan yeni proje

**Örnek:** Kullanıcıları ve platformu belli olan, henüz kodlanmamış bir randevu uygulaması.

**Adımlar:** Amacı ve bilinen kısıtları belirt → Codex'in kurulum için kritik sorularını yanıtla → geliştirme görevi vermeden önce ortamın devir sonucunu incele.

```text
Eklediğim FOUNDATION.md (v2.3) rehberini yeni bir projeye uygula.
Hedef dizin: [yol]
Amaç ve kullanıcılar: [ör. küçük bir işletmenin randevu yönetimi]
Bilinen kısıtlar: [platform, seçildiyse teknoloji, veri veya teslim kısıtları]
Kararlaştırılmayanlar: [açık önemli seçimler]

Mühendislik çalışmasına başlamak için yeterli en küçük ortamı kur.
Yalnızca kurulumu etkileyen eksik kararları sor. Gerekiyorsa genel bir
proje iskeleti hazırla; ilk ürün özelliğini geliştirme.
Bağlama erişimi ve uygulanabilir çalışma koşullarını doğrula.
Kapsam, kanıt, sınırlamalar ve günlük başlangıç noktasıyla birlikte
READY veya NOT READY sonucu ver.
```

**Beklenen sonuç:** Proje yönü, çalışma talimatları, başlangıç kurulum/doğrulama yolları ve sonraki işler için açık kalan kararlar.

### 2 · Mevcut kod var, agentic ortam yok

**Örnek:** Ekibin kullandığı, kısa bir README'si olan ama çalışma bilgisi belgelenmemiş bir backend.

**Adımlar:** Repoyu ve kısa amacını belirt → Codex'in kodu, yapılandırmayı ve mevcut kontrolleri keşfetmesini sağla → bıraktığı yönlendirmeyi ve çalıştırma sınırlarını incele.

```text
Eklediğim FOUNDATION.md (v2.3) rehberini bu mevcut projeye uygula.
Repo: [yol]
Amaç: [sistem ne yapıyor]
Bilinen çalışma kısıtları: [varsa]

Soru sormadan önce kodu, belgeleri, yapılandırmayı ve mevcut kontrolleri
incele. Eksik proje talimatlarını, bağlam erişimini, doğrulama rehberini
ve bilgi güncelleme düzenini oluştur.
Mevcut yapıyı ve kaydedilmemiş değişiklikleri koru. İlgili mevcut bir
akışı yön bulma örneği olarak kullan; atanmış ürün görevine dönüştürme.
Uygun temel kontrollerden önce komutların yan etkilerini incele.
Kurulum sırasında uygulama hatalarını düzeltme veya iş verisi taşıma.
READY/NOT READY sonucunu, kanıtları, sınırları ve günlük başlangıcı belirt.
```

**Beklenen sonuç:** Talimatlardan ilgili koda ve kontrollere ulaşılabilen bir yol; gözlenen davranış ile kabul edilmiş gereksinimlerin ayrılması.

### 3 · Mevcut agentic ortamı onarma

**Örnek:** AGENTS.md başka bir rehberle çelişiyor, bağlantılar silinmiş dosyalara gidiyor veya her oturum gereksiz miktarda bağlam yüklüyor.

**Adımlar:** Gördüğün belirtileri anlat → Codex'in talimatları kapsam ve kanıtlarıyla karşılaştırmasını sağla → yapılan sınırlı onarımları ve korunan yapıyı incele.

```text
Eklediğim FOUNDATION.md (v2.3) ile bu agentic ortamı onar.
Repo: [yol]
Belirtiler: [ör. çelişen talimatlar, eski yollar, tekrar eden keşif]
Korunacak tercihler: [bilinen çalışma kuralları, varsa]

Mevcut talimatları, bağlam belgelerini, skill'leri ve doğrulama yollarını
incele. Değişiklikten önce somut çelişkileri ve eksikleri belirle.
Yararlı yapıyı ve kullanıcı tercihlerini koru; paralel bir talimat sistemi
oluşturma. Eski yönlendirmeleri açıkça işaretle, yararlı geçmişi koru.
Yalnızca gerekçeli ortam sorunlarını onar; ürün kodunu değiştirme.
Görev bağlamına erişimi ve uygun çalışma koşullarını doğrula.
Onarımları, korunan bilgileri, kanıtları ve kapsamı belirtilmiş READY/NOT READY
sonucunu raporla.
```

**Beklenen sonuç:** Mevcut yapı içinde açık yetki sırası, çalışan referanslar ve tutarlı günlük çalışma rehberi.

### 4 · Yeniden geliştirme veya modernizasyon

**Örnek:** Belirli iş akışlarını koruyarak masaüstü uygulamasını web uygulamasıyla değiştirmek.

**Adımlar:** Mevcut ve hedef konumları belirt → değişim nedenini ve korunacak davranışları açıkla → ortam tamamlandı sayılmadan önce önemli hedef belirsizliklerini çöz.

```text
Eklediğim FOUNDATION.md (v2.3) ile modernizasyon ortamını hazırla.
Mevcut sistem: [yol veya erişilebilir kaynaklar]
Hedef proje: [yol; aynı repo olabilir]
Değişim nedeni: [neden]
Hedef yön: [neler değişmeli]
Korunacaklar: [iş akışları, sözleşmeler veya uyumluluk]
Veri taşıma ve çalışma kısıtları: [bilinen sınırlar veya bilinmeyenler]

Mevcut uygulamayı kabul edilmiş hedef amaçtan ayır.
Her eski davranışın kopyalanacağını veya kaldırılacağını varsayma.
Eksik hedef kararlarını yalnızca ortam hazırlığını engelledikleri
ölçüde çöz. Hedef çalışma rehberini, referans erişimini ve doğrulama
yollarını kur. Yeniden geliştirmeyi veya veri taşımasını başlatma.
Kanıtlar, açık kararlar ve devir bilgisiyle READY/NOT READY sonucu ver.
```

**Beklenen sonuç:** Korunacak/değişecek davranışları açık olan, ilgili eski sistem kanıtlarına erişilebilen hedef çalışma ortamı.

### 5 · Tanımadığın proje veya kayıp bağlam

**Örnek:** Eski belgeleri olan, güvenilir kurulum açıklaması bulunmayan bir repoyu devraldın.

**Adımlar:** Kaynakları ve bildiklerini paylaş → Codex'in asgari güvenilir bağlamı çıkarmasını sağla → doğrulanan bilgileri, belirsizlikleri ve erişim engellerini incele.

```text
Eklediğim FOUNDATION.md (v2.3) ile bu projenin bağlamını kurtar.
Repo: [yol]
Bildiklerim: [kısa bilgiler veya bilinmiyor]
Diğer kaynaklar: [varsa belgeler veya referanslar]

Mühendislik ortamı kurmaya yetecek güvenilir anlayışı oluştur.
Gözlenen bilgileri, çıkarımları ve bilinmeyenleri ayır.
Gereksinim uydurma veya eski belgeleri güncel gerçek kabul etme.
Mevcut çalışmayı koru. En küçük yararlı erişim ve çalışma rehberini
oluştur; temel kontrollerden önce çalıştırma yan etkilerini incele.
Sistemi yeniden tasarlama veya ürün görevine başlama.
Kapsamı belirtilmiş READY/NOT READY, kanıtlar ve kalan bilgi ihtiyacını sun.
```

**Beklenen sonuç:** Uydurulmuş bir şartname yerine güvenilir yönlendirme ve hâlâ bilinmeyenlerin açık kaydı.

### 6 · Hazır ortamın yeterliliğini kontrol etme

**Örnek:** Güncel talimatları ve kontrolleri olan bir projede önemli bir eksik kalıp kalmadığını öğrenmek istiyorsun.

**Adımlar:** Günlük çalışma kapsamını belirt → yalnızca inceleme iste → raporlanan eksiklerin onarımına ayrıca karar ver.

```text
Eklediğim FOUNDATION.md (v2.3) ile bu ortamı değerlendir.
Repo: [yol]
Hedeflenen günlük çalışma kapsamı: [mühendislerin yapabilmesi gerekenler]

Mevcut yönlendirmeyi incele; ilgili bir görevin bağlam ve doğrulama
rotasını takip et. Mevcut izinler içinde yalnızca uygun, zarar vermeyen
temel kontrolleri çalıştır. Proje dosyalarını düzenleme veya yeni bir
talimat yapısı oluşturma. Somut kanıtlar, sınırlar ve varsa gereken
en küçük onarımlarla READY veya NOT READY sonucu ver.
```

**Beklenen sonuç:** Kanıta dayalı hazırlık değerlendirmesi. Yeterli bir ortam için yeni dosya üretmek gerekmez.

## Sonucu nasıl değerlendireceğim?

| Sonuç | Anlamı | Sonraki adımın |
| :--- | :--- | :--- |
| **READY** | Belirtilen mühendislik kapsamı destekleniyor; sınırlar açık. | Projenin kendi talimatlarından günlük göreve başla. |
| **NOT READY** | Belirli bir ortam eksikliği bu kapsamı engelliyor. | Belirtilen önkoşulu veya kararı çöz, etkilenen yeterliliği yeniden değerlendir. |

Kanıt ara: talimatlar bulunabiliyor mu, kod ve bilgi erişilebilir mi, ilgili kontrollerin gerçek sonuçları var mı, sonraki oturum kararları nereye kaydedeceğini biliyor mu? Dosya oluşturmak tek başına başarı değildir. Geçen bir derleme ürün kabulü anlamına gelmez; ileride gerekecek bir entegrasyonun henüz denenmemesi de otomatik olarak kurulum engeli değildir.

## Devirden sonra

Günlük görevlerde projenin kendi talimatlarını kullan, proje değiştikçe yararlı bilgiyi güncelle. FOUNDATION.md dosyasını proje içinde veya dışında isteğe bağlı kurulum referansı olarak tutabilirsin. Her kodlama oturumunda değil, ciddi ortam onarımı veya yön değişikliği gerektiğinde yeniden uygula.

## Dosyalar ve doğrulama durumu

- **[FOUNDATION.md](./FOUNDATION.md):** Codex'in uygulayacağı İngilizce kaynak rehber.
- **README.md:** Bu iki dilli kullanım rehberi; promptlar Foundation'ı tamamlar.

V2.3; yeni proje, mevcut kod ve ortam onarımı senaryolarında gerçek projelerle denendi. Kapsamlı modernizasyon ve proje kurtarma hâlâ gerçek proje doğrulaması bekliyor. Metnin sonlandırılması her senaryo veya teknolojinin doğrulandığı anlamına gelmez.

En yararlı geri bildirim; başlangıç durumunu, ortamın nerede aksadığını ve tekrar kullanılabilir iyileştirmeyi anlatır. Özel proje bilgilerini herkese açık bildirimlerden çıkar.

</details>
