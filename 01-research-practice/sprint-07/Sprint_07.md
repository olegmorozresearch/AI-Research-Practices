# Sprint 7 — Manuscript, Research Release & Scientific Communication

**AI Research Practices · Науково-дослідна практика · Тиждень 7 / 7**

**Результат спринту:** короткий рукопис статті (орієнтовно 5–8 сторінок), тези, перевірений Research Package v1.0 та матеріали для наукового review. **Публікація не є автоматичною дією:** оприлюднення погодженого препринту в Zenodo Community можливе лише після повноцінної перевірки науковим керівником.

**Вхідні артефакти:** Research Problem Statement (Sprint 1), Research Proposal і Literature Review Matrix (Sprint 2), Experimental Protocol (Sprint 3), моделі та відтворюваний код (Sprint 4), Experimental Results (Sprint 5), Results and Discussion та Reproducibility Report (Sprint 6).

**Приклад:** оцінювання стійкості Logistic Regression, Random Forest і Gradient Boosting до гаусівського шуму в тестових ознаках `load_wine`. Гіпотезу, протокол, дані, моделі та отримані результати не змінюємо.

## Маршрут спринту

1. Зіставляємо готові результати з логікою короткої наукової статті.
2. Формуємо **Manuscript v1.0** за єдиним шаблоном DOCX.
3. Показуємо завершений навчальний приклад основних розділів статті.
4. Готуємо **Conference Abstract v1.0** та коротке наукове представлення.
5. Перевіряємо дослідницький пакет: артефакти, походження, відтворюваність, права та метадані.
6. Готуємо пакет до review керівником та, лише після погодження, до оприлюднення.

**Межа етапу:** Sprint 7 завершує дослідження на рівні навчального продукту й передає його на наукову перевірку. Можливі поглиблення, журнальне подання та нові версії результату відносяться до подальшого розвитку дослідження.

## A. Problem Situation — результати є, але чи готова стаття?

У Sprint 6 отримано `Results_and_Discussion_v1.md`, графіки, таблиці й `Reproducibility_Report_v1.md`. Проте це ще не рукопис: бракує назви, анотації, вступу з науковою проблемою, стислого огляду джерел, самодостатнього опису методів, висновків і коректного списку літератури.

**Проблема спринту:** як інтегрувати результати попередніх етапів у коротку статтю, не дописуючи того, чого наш експеримент не встановив, і підготувати перевірюваний Research Release?

**Практичний принцип:** рукопис — аргументований науковий текст; Research Package — артефакти, які дають перевірити походження цього тексту. Вони пов'язані, але не замінюють один одного.

## B1. Essential Theory — архітектура короткої наукової статті

| Розділ | Головне запитання | Звідки беремо матеріал |
|---|---|---|
| Title + Abstract + Keywords | Що досліджено і що встановлено? | Спринти 1, 3, 5–6 |
| Introduction | Яка проблема, прогалина, мета, RQ та H1? | Спринти 1–2 |
| Related Work | Які перевірені праці формують науковий контекст? | Literature Review Matrix (Sprint 2) |
| Materials and Methods | Чи можна відтворити дизайн дослідження? | Protocol + код (Sprint 3–4) |
| Results | Які спостереження і числові свідчення отримано? | Sprint 5–6 |
| Discussion | Що означають результати для RQ та H1? | Sprint 6 |
| Limitations, Open Questions, Future Research | Де межі висновків і що далі? | Sprint 6 |
| Conclusions | Яка стисла відповідь на проблему й науковий внесок? | Sprint 6 |
| References / Availability | Що цитуємо та де перевірити артефакти? | Mendeley + GitHub / майбутній Zenodo record |

**Орієнтовний обсяг:** 5–8 сторінок, але вимоги обраного видання мають пріоритет. Манускрипт створюємо, використовуючи **єдиний DOCX-шаблон**. Для бібліографії використовуємо перевірені записи Mendeley — вигаданих джерел не має бути.

## B2. Essential Theory — логіка Abstract і Conclusions

**Abstract** стисло відображає логіку дослідження: *проблема → мета → метод → конкретні результати → висновок*. Він не вводить нових фактів. **Conclusions** відповідають на RQ, узагальнюють внесок і не дублюють Discussion дослівно.

Розрізняємо:
- **Мета** — що хотіли з'ясувати.
- **Метод** — як організовано перевірку.
- **Результат** — які значення, залежності та відмінності отримано.
- **Внесок** — яке перевірюване знання додало дослідження в установлених межах.

## B3. Essential Theory — від Literature Review до наукового аргументу

Зі Sprint 2 переносимо **тільки перевірені джерела та їхні релевантні твердження**. Для кожної цитованої роботи маємо з'ясувати, яку проблему вона розглядала, який застосувала метод і як саме пов'язана з нашим RQ.

Порівняння з літературою — не формальний перелік результатів: воно показує, який аспект проблеми розглянуто раніше і який аспект перевірено в нашому експерименті. Якщо перевірених посилань ще немає під рукою, ставимо явну позначку **[ПОТРІБНА ЗВІРКА З LITERATURE REVIEW MATRIX]**. Таку позначку необхідно усунути до фінального рукопису.

## B4. Essential Theory — Research Package і Research Release

**Research Package v1.0** — узгоджений набір дослідницьких артефактів для перевірки та відтворення результатів: протокол, вихідний код, конфігурація й залежності, дані або інструкції їх отримання, результати вимірювань, графіки, звіт відтворюваності та реєстр файлів із контрольними сумами. Рукопис, тези, README та відомості про ліцензування включаємо до Research Release v1.0.

**Research Release v1.0** — зафіксована версія наукового продукту, підготовлена для поширення після необхідного review. У межах спринту формуємо пакет і чернетку метаданих; не вигадуємо DOI та не позначаємо непогоджену версію як опубліковану.

**GitHub fork** — робочий простір коду й історії змін.

**DOI та версія Research Release**

Архів оприлюднених версій зберігається на **Zenodo**. Під час першого оприлюднення Research Release створюємо новий запис (*New upload*). У метаданих зазначаємо версію `1.0`. Якщо дослідницький продукт ще не має DOI, Zenodo автоматично присвоїть його після публікації.

Зберігаємо присвоєний DOI як постійний ідентифікатор Research Release v1.0.

Zenodo також підтримує спільний ідентифікатор послідовності версій — *Concept DOI*. Якщо згодом під час переддипломної практики буде підготовлено Research Release v2.0, створюємо його через функцію *New version* попереднього запису. Нова версія отримає окремий DOI, а Concept DOI залишиться спільним для обох версій.

**Авторство:** авторський склад визначається реальним інтелектуальним внеском; саме рецензування керівником не створює автоматичного співавторства. Ліцензію обираємо з урахуванням прав на код, дані, зображення та текст.

## B5. Essential Theory — наукова комунікація та review

Підготовка тексту й його публікація — різні події. Для Sprint 7 послідовність така:

`Manuscript Draft + Abstract → перевірка комплектності → наукове рецензування керівником → виправлення → погоджена версія → Zenodo draft → Submit for review → рішення куратора → оприлюднення`.

Для нашої Zenodo Community неопублікований запис подаємо через **Submit for review**. Подання Research Release v1.0 до Zenodo Community допускається **лише після отримання остаточної позитивної рецензії наукового керівника**. Саме ця рецензія є обов'язковою умовою (тригером) переходу від підготовки дослідницького продукту до його оприлюднення.

Після подання запису його прийняття куратором спільноти може автоматично призвести до публікації в Zenodo.

Формат подання тез конференції чи статті у фаховий журнал залежить від вимог майданчика.

## C1. Guided Research Example — з яких результатів складаємо статтю

Наш навчальний експеримент уже містить потрібні наукові свідчення:

- П'ять рівнів шуму: `σ = 0, 0.1, 0.2, 0.4, 0.6`.
- Три алгоритми, навчені один раз без штучного шуму.
- Для кожного додатного `σ` — п'ять реалізацій шуму зі спільними seed для алгоритмів.
- Результати `Q(m,σ)` (macro-F1), `D(m,σ)` (втрата відносно власної `Q(m,0)`), середні значення та SD.
- Аудит та контрольне повторення 63 оцінювань у Sprint 6.

За `σ=0.6` середня деградація становить **0.0339** (Logistic Regression), **0.0765** (Random Forest) і **0.1227** (Gradient Boosting). Це спостереження має увійти до *Results*, а його значення для H1 — до *Discussion*.

**Вхідний документ:** `Results_and_Discussion_v1_Example.md` зі Sprint 6.

### Організація Research Release v1.0

Для підготовки першої версії дослідницького продукту створюємо в корені робочого каталогу Sprint 7 папку `research_release_v1`.

У цьому каталозі збираємо підготовлені матеріали для наукового рецензування та подальшого оприлюднення:

```text
research_release_v1/
├── Short_Manuscript_v1.docx
├── Conference_Abstract_v1.md
├── README.md
├── LICENSE
└── Review_Request_v1.md
```

- `Short_Manuscript_v1.docx` — рукопис короткої наукової статті.
- `Conference_Abstract_v1.md` — підготовлені конференційні тези.
- `README.md` — опис дослідження, складу Research Package та порядку відтворення результатів.
- `LICENSE` — умови використання матеріалів дослідження.
- `Review_Request_v1.md` — звернення до наукового керівника для проведення остаточного review.

Рукопис і тези формуємо за шаблонами Sprint 7. Для опису Research Package використовуємо результати та артефакти попередніх спринтів.

Після підготовки цих документів у C7 перевіряємо дослідницькі артефакти та створюємо `artifact_manifest.csv`, а в C8 перевіряємо комплектність Research Release перед науковим рецензуванням.

## C2. Guided Research Example — як виглядають Title, Abstract і Keywords

**Title:** *Robustness Profiles of Three Classification Algorithms Under Gaussian Noise in Test Features: A Controlled Case Study*

**Abstract — навчальний зразок**

> We examine how additive Gaussian noise in test features affects the classification performance of Logistic Regression, Random Forest, and Gradient Boosting. Three models are trained without artificial noise using a fixed train/test split of the Wine dataset, and independent Gaussian perturbations are added to standardized test features at four positive noise levels. We evaluate macro-F1, degradation relative to each model's clean reference, and variability across five fixed noise seeds. At the highest studied noise level (σ = 0.6), the mean degradation is 0.0339 for Logistic Regression, 0.0765 for Random Forest, and 0.1227 for Gradient Boosting. The observed degradation profiles differ across the three models, supporting the study hypothesis descriptively. The experiment provides a reproducible comparison of model behavior under the specified perturbation protocol.

**Keywords:** classification robustness; Gaussian noise; macro-F1; logistic regression; random forest; gradient boosting; reproducibility.

**Звернемо увагу:** Abstract містить фактичні числа, не оголошує причинний механізм встановленим і не приписує статистичної значущості непроведеним перевіркам.

## C3. Guided Research Example — Introduction і Related Work

**Introduction — фрагмент готового тексту**

> Reliability under perturbed input data is an important consideration in classification systems. While predictive performance is often reported on unmodified test data, it does not directly describe how a fixed classifier behaves when feature measurements are distorted. This study compares the degradation profiles of three trained classification algorithms under a controlled test-time perturbation. We ask how macro-F1 changes with noise intensity, whether model-specific degradation profiles differ, and how much the results vary across noise realizations. We hypothesize that the three algorithms exhibit different degradation profiles under the same experimental conditions.

**Related Work — структура, яку заповнюємо зі Sprint 2**

1. Дослідження оцінювання стійкості класифікаторів до спотворень ознак — **[перевірені джерела]**.
2. Методики контрольованого введення шуму й оцінювання робастності — **[перевірені джерела]**.
3. Дослідження чутливості конкретних типів моделей — **[перевірені джерела]**.

У навчальному прикладі ці позиції **навмисно не заповнені вигаданими працями**. Перед науковим review студент має внести перевірені бібліографічні посилання та показати, що саме вони підтверджують. Недостатньо просто перерахувати статті.

## C4. Guided Research Example — Methods без повторення всього програмного коду

**Materials and Methods — приклад тексту рукопису**

> We used the `load_wine` classification dataset and a fixed train/test split. Numerical features were standardized using statistics estimated exclusively from the training set. Logistic Regression, Random Forest, and Gradient Boosting were tuned by cross-validation on clean training data using macro-F1; their fitted configurations were then kept fixed. Gaussian noise with zero mean and standard deviation σ was added to the standardized test features for σ ∈ {0.1, 0.2, 0.4, 0.6}. Five prespecified seeds generated noise realizations at each positive σ. Each algorithm was evaluated against the same noise realization for the corresponding (σ, seed) condition. The clean reference was evaluated once per model. We report macro-F1 Q, the corresponding degradation D = Q(m,0) − Q(m,σ), and across-seed mean and sample standard deviation.

У фінальному рукописі уточнюємо **точну процедуру split, добору гіперпараметрів, найменування моделі, зафіксовані конфігурації та версії бібліотек**, використовуючи `Experimental_Protocol`, `Sprint_04` і маніфести. Не переносимо сюди всі комірки коду — для цього є Research Package.

**Рисунок 1:** графік `Q(m,σ)`; **Рисунок 2:** графік `D(m,σ)`; за потреби додаємо рисунки варіативності з Sprint 5.

## C5. Guided Research Example — Results, Discussion, Limitations і Conclusions

**Results (фрагмент):**

> Mean macro-F1 did not increase with increasing noise intensity on the tested grid for any of the three fixed models. At σ = 0.6, the mean macro-F1 was 0.9661 (Logistic Regression), 0.9235 (Random Forest), and 0.8226 (Gradient Boosting). The corresponding mean degradations from model-specific clean references were 0.0339, 0.0765, and 0.1227, respectively. At this noise level, the sample standard deviations of degradation across five realizations were 0.0232, 0.0314, and 0.0307.

**Discussion (фрагмент):**

> The experimental results show that classification quality decreases as the intensity of Gaussian noise in test features increases, although the magnitude of this decrease differs among the three algorithms. Logistic Regression exhibits the smallest degradation, Gradient Boosting the largest, and Random Forest an intermediate response under the investigated conditions.
>
> The degradation profiles demonstrate that the algorithms respond differently to the same levels of input perturbation. Furthermore, the variation observed across five independent noise realizations at each nonzero noise level indicates that the measured degradation also depends on the particular realization of the perturbation.
>
> Taken together, these findings are consistent with the hypothesis that the three algorithms exhibit different degradation profiles under identical experimental conditions. This conclusion is supported by descriptive analysis; the experimental protocol did not specify a separate inferential test of between-model differences.

**Limitations → Open Questions → Future Research:** 

>Переносимо п'ять погоджених обмежень із Sprint 6, формулюємо три відкриті питання та відповідні перспективи, без повторення застережень після кожного абзацу.

**Conclusions — приклад:**

> This controlled experiment documents different degradation profiles for three fixed classifiers under Gaussian perturbations of standardized test features. Logistic Regression showed the smallest mean performance loss and Gradient Boosting the largest at the highest tested noise intensity. Reporting both mean degradation and its across-seed variability helps characterize the observed behavior. The experimental artifacts and reproducibility audit provide a traceable basis for subsequent verification and extensions.

Повний **`Short_Manuscript_v1_Example.md`** у комплекті показує, як ці фрагменти поєднуються в один документ.

## C6. Guided Research Example — тези для наукової комунікації

**Назва тез:** *A Controlled Comparison of Classification Robustness Under Gaussian Test-Feature Noise*

**Тези — навчальний зразок:**

> This study compares the robustness of Logistic Regression, Random Forest, and Gradient Boosting under controlled Gaussian perturbations applied to standardized test features. Using a fixed Wine dataset split, models trained on unperturbed data, five noise seeds, and macro-F1 evaluation, we measure model-specific degradation from clean references. At σ = 0.6, the mean degradation was 0.0339, 0.0765, and 0.1227, respectively. The results reveal distinct descriptive degradation profiles and variability across noise realizations. A documented experimental protocol and reproducibility audit make the analysis traceable.

**Усне представлення (приблизно 60 секунд):** проблема → метод → головний графік → ключовий результат → межа висновку та внесок.

**Важливо:** це універсальний навчальний приклад, а не тези у форматі конкретної конференції. Перед поданням дотримуємося її власних правил обсягу, структури, авторства та оформлення.

## C7. Guided Research Example — перевірка Research Package та створення `artifact_manifest.csv`

У Sprint 4–6 ми зберегли експериментальний протокол, код і конфігурацію, результати вимірювань, графіки, звіт відтворюваності та текст Results and Discussion. Перед підготовкою релізу перевіряємо, чи доступні ці артефакти, і формуємо **один реєстр** `artifact_manifest.csv`.

У словнику `required` зазначено ролі файлів та їхні **прикладові відносні шляхи**. Перед запуском у персональному fork звіряємо шляхи з фактичною структурою власного проєкту; додаємо всі необхідні вихідні дані, код, конфігурації та рисунки. Перевірка для кожного файлу визначає статус, розмір і SHA-256. Відсутні файли залишаються зі статусом `MISSING` — програма не видає неповний пакет за готовий.

Наприкінці цієї ж комірки створюємо машинозчитуваний `research_artifacts/sprint7/artifact_manifest.csv`. 

Це результат **аудиту артефактів**, а не рішення про публікацію.

```python
from pathlib import Path
import csv
import hashlib

# Приклад шляхів. Перед перевіркою свого Research Package звіряємо їх із fork
# і доповнюємо списком усіх файлів, які плануємо включити до релізу.
required = {
    "Experimental Protocol": "research_artifacts/sprint3/Experimental_Protocol.md",
    "Raw measurements": "research_artifacts/sprint5/measurements.csv",
    "Summary": "research_artifacts/sprint5/summary.csv",
    "Reproducibility report": "research_artifacts/sprint6/Reproducibility_Report_v1.md",
    "Results and Discussion": "research_artifacts/sprint6/Results_and_Discussion_v1.md",
    # Додаємо шляхи до вихідного коду, моделей, конфігурацій, даних,
    # графіків та файлів залежностей відповідно до власного Research Package.
}

def sha256_file(path):
    h = hashlib.sha256()
    with path.open("rb") as f:
        for chunk in iter(lambda: f.read(1024 * 1024), b""):
            h.update(chunk)
    return h.hexdigest()

root = Path.cwd()
manifest_rows = []
for role, rel in required.items():
    path = root / rel
    if path.is_file():
        manifest_rows.append((role, rel, "PRESENT", path.stat().st_size, sha256_file(path)))
    else:
        manifest_rows.append((role, rel, "MISSING", "", ""))

manifest_path = root / "research_artifacts/sprint7/artifact_manifest.csv"
manifest_path.parent.mkdir(parents=True, exist_ok=True)
with manifest_path.open("w", encoding="utf-8", newline="") as f:
    writer = csv.writer(f)
    writer.writerow(["role", "relative_path", "status", "size_bytes", "sha256"])
    writer.writerows(manifest_rows)

for role, rel, state, _, _ in manifest_rows:
    print(f"{role:25s} | {state:7s} | {rel}")
print(f"\nНаявні: {sum(row[2] == 'PRESENT' for row in manifest_rows)} / {len(manifest_rows)}")
print("Створено реєстр:", manifest_path.relative_to(root))
```

## C8. Guided Research Example — фінальна перевірка комплекту перед review та Zenodo

У C7 ми перевірили дослідницькі артефакти й записали їхні контрольні суми. Тепер перевіряємо, чи **весь комплект наукового продукту** готовий до передавання науковому керівникові: рукопис, тези, матеріали відтворення, реєстр файлів, опис відтворення, ліцензування та супровідний запит на рецензування.

Наступна комірка читає вже створений `artifact_manifest.csv`, повторно перевіряє наявність зареєстрованих файлів і відповідність їхніх SHA-256, а також перевіряє додаткові документи релізу. Шляхи у словнику `release_files` — **приклад структури персонального проєкту**, який адаптуємо до реального Research Package. Перевірка не створює другого реєстру й не змінює результати експерименту.

Умови допуску до подання на Zenodo Community визначаємо за `Research_Release_v1_Checklist.md`: **остаточна позитивна рецензія керівника обов'язкова**. Автоматична перевірка файлів не замінює наукового рішення. Після погодження готуємо метадані Zenodo: тип публікації, назву, фактичних авторів, анотацію, ключові слова, версію `1.0`, ліцензію та пов'язані ідентифікатори. DOI фіксуємо лише після його фактичного присвоєння.

```python
from pathlib import Path
import csv

root = Path.cwd()
manifest_path = root / "research_artifacts/sprint7/artifact_manifest.csv"
if not manifest_path.is_file():
    raise FileNotFoundError("Спершу виконуємо C7 і створюємо artifact_manifest.csv")

with manifest_path.open(encoding="utf-8", newline="") as f:
    registry = list(csv.DictReader(f))

verified = []
# Перевіряємо не лише наявні рядки реєстру, а й обов'язкові категорії.
# Їх слід внести в required у C7 із реальними шляхами власного fork.
mandatory_roles = {
    "Experimental Protocol", "Raw measurements", "Summary",
    "Reproducibility report", "Results and Discussion",
    "Source code", "Model / model artifact", "Configuration",
    "Data / acquisition instructions", "Dependency specification",
    "Quality figure", "Degradation figure",
}
registered_roles = {entry["role"] for entry in registry}
for role in sorted(mandatory_roles - registered_roles):
    verified.append((f"Не внесено до маніфесту: {role}", False))
for entry in registry:
    target = root / entry["relative_path"]
    verified.append((entry["role"], target.is_file()
                     and entry["status"] == "PRESENT"
                     and sha256_file(target) == entry["sha256"]))

# Приклад структури релізу. Звіряємо і змінюємо шляхи відповідно до власного fork.
release_files = {
    "Manuscript": "research_release_v1/Short_Manuscript_v1.docx",
    "Conference abstract": "research_release_v1/Conference_Abstract_v1.md",
    "Research Package README": "research_release_v1/README.md",
    "License / rights": "research_release_v1/LICENSE",
    "Review request": "research_release_v1/Review_Request_v1.md",
    "Reproducibility manifest": "research_artifacts/sprint7/artifact_manifest.csv",
}
for role, rel in release_files.items():
    verified.append((role, (root / rel).is_file()))

for role, ok in verified:
    print(f"{'PASS' if ok else 'MISSING / MISMATCH':19s} | {role}")
print("\nТехнічна комплектність:", "PASS" if all(ok for _, ok in verified) else "INCOMPLETE")
print("Допуск до Zenodo: лише після остаточної позитивної рецензії керівника.")
```

## Тренувальна вправа 1 — наукове твердження для Abstract

Є фактичне спостереження: за `σ=0.6` середнє `D` становить 0.0339, 0.0765 і 0.1227 для LR, RF і GB відповідно. Оберіть коректне речення для Abstract і коротко поясніть вибір.

**А.** Gradient Boosting завжди найменш стійкий класифікатор.

**Б.** У проведеному експерименті при `σ=0.6` найбільшу середню деградацію продемонстрував Gradient Boosting.

**В.** Gradient Boosting статистично значуще гірший за інші моделі.

## Тренувальна вправа 2 — складання Research Package

У пакеті є `summary.csv`, `measurements.csv`, код і рисунки, але немає `Experimental_Protocol.md`. Чи достатньо такого комплекту для передавання на перевірку відтворюваності? Назвімо відсутній елемент і пояснімо його роль двома реченнями.

## Тренувальна вправа 3 — метадані та публікація

Студент підготував Manuscript v1.0 і натиснув **Save draft** у Zenodo. Чи можна вже вважати роботу опублікованою й додати вигаданий DOI до списку публікацій? Яким є наступний науковий крок у нашому workflow?

## D. Independent Research — завершуємо власний науковий продукт

Працюємо з власними файлами попередніх спринтів і шаблонами комплекту. Зберігаємо результат у персональному GitHub fork. Матеріали надсилаємо на повний review керівнику до будь-якого оприлюднення.

### D1. Manuscript — структура та зв'язність

**Створюємо:** `Short_Manuscript_v1.docx` на основі `Short_Manuscript_v1_Template.docx`.

Переносимо Research Problem / RQ / H1, обґрунтований Literature Review, стислий Experimental Protocol, перевірені Results і Discussion, Limitations, Conclusions, References, Data and Code Availability. **Перевіряємо**, чи Abstract і Conclusions точно відповідають Results та не вводять нових фактів.

**Автори й афіліації:** визначаємо за реальним внеском, не за посадою. Бібліографію додаємо з Mendeley. Поля, які лишилися незаповненими, відмічаємо як `REVISION NEEDED`.

### D2. Scientific Communication — тези й коротка презентація

**Створюємо:** `Conference_Abstract_v1.md` (або формат обраної конференції). У тезах подаємо проблему, метод, один-два перевірені результати, висновок. Узгоджуємо їх із рукописом. Готуємо короткий усний виклад і одну головну ілюстрацію — якщо це передбачає формат заходу.

**Самоперевірка:** чи відповідає формулювання результату реальній таблиці або рисунку? Чи не замінено науковий результат обіцянкою майбутньої роботи?

### D3. Формування Research Package та Research Release v1.0

На цьому етапі формуємо два взаємопов'язані компоненти дослідницького продукту: **Research Package** для перевірки та відтворення результатів і **Research Release v1.0** для наукового рецензування та подальшого оприлюднення.

**1. Research Package — дослідницькі артефакти**

Збираємо та перевіряємо матеріали, необхідні для відтворення дослідження:

- експериментальний протокол;
- перевірений вихідний код, конфігурацію та відомості про версії програмного середовища (`requirements`);
- набори даних або інструкції щодо їх отримання з урахуванням прав використання;
- результати вимірювань, підсумкові таблиці та рисунки;
- `Reproducibility_Report_v1.md`;
- `artifact_manifest.csv` із переліком файлів, результатами перевірки та контрольними сумами SHA-256.

Перевіряємо повноту й цілісність Research Package за процедурою, продемонстрованою в C7.

**2. Research Release v1.0 — комплект для наукової комунікації**

У корені робочого каталогу створюємо папку `research_release_v1/`:

```text
research_release_v1/
├── Short_Manuscript_v1.docx
├── Conference_Abstract_v1.md
├── README.md
├── LICENSE
└── Review_Request_v1.md
```

У цьому каталозі розміщуємо підготовлені рукопис і тези, опис дослідження та його артефактів (`README.md`), інформацію про права використання (`LICENSE`) і звернення до наукового керівника для проведення review.

У `README.md` зазначаємо склад Research Package, розташування дослідницьких артефактів та порядок відтворення результатів. Окремо визначаємо умови доступу до даних і матеріалів третіх сторін.

**3. Перевірка готовності Research Release**

За процедурою C8 перевіряємо:

- комплектність документів у `research_release_v1/`;
- наявність і цілісність артефактів Research Package;
- відповідність рукопису й тез отриманим результатам;
- готовність матеріалів до рецензування за `Research_Release_v1_Checklist.md`.

Після завершення перевірки передаємо Research Release v1.0 науковому керівнику. 

**Подання до Zenodo Community здійснюємо лише після отримання остаточної позитивної рецензії керівника.**

### D4. Фінальна перевірка Research Release та підготовка до оприлюднення

**1. Перевірка Research Package**

Повторно перевіряємо наявність і цілісність дослідницьких артефактів, зареєстрованих у `artifact_manifest.csv`. Звіряємо контрольні суми SHA-256, повноту експериментальних результатів, вихідного коду, конфігурації та документації відтворюваності.

**2. Перевірка Research Release v1.0**

Перевіряємо комплект фінальних документів у каталозі `research_release_v1/`, сформований у D3.

Заповнюємо `Research_Release_v1_Checklist.md`, перевіряючи комплектність матеріалів, авторство, права використання, ліцензію, відповідність метаданих, зафіксований GitHub commit і готовність до наукового рецензування.

**3. Наукове рецензування та підготовка до Zenodo**

Передаємо Research Release v1.0 науковому керівнику для остаточного review. Зауваження опрацьовуємо, виправлення вносимо до рукопису та дослідницьких артефактів і фіксуємо в таблиці опрацювання зауважень керівника, наведеній наприкінці Review_Request_v1_Template.md.

**Лише після отримання остаточної позитивної рецензії керівника** готуємо Zenodo draft і подаємо неопублікований запис до Zenodo Community згідно з правилами спільноти.

У фінальному звіті фіксуємо фактичний статус Research Release:

- `DRAFT` — комплект перебуває на етапі підготовки;
- `UNDER SUPERVISOR REVIEW` — матеріали передано науковому керівнику;
- `APPROVED FOR RELEASE` — отримано остаточне погодження керівника;
- `SUBMITTED TO COMMUNITY` — запис подано до Zenodo Community;
- `PUBLISHED` — Research Release оприлюднено в Zenodo.

DOI зазначаємо лише після його фактичного присвоєння Zenodo.

**Результат власного дослідження за Sprint 7:** `Short_Manuscript_v1.docx`, `Conference_Abstract_v1.md`, перевірений Research Package v1.0, підготовлений Research Release v1.0 та матеріали наукового рецензування.

Поки рецензування триває, статус дослідницького продукту залишається `UNDER SUPERVISOR REVIEW`. Завершення Sprint 7 не означає автоматичного погодження або оприлюднення Research Release.

## E1. Sprint Review — навчальний приклад

- [ ] Назва, Abstract, Methods, Results, Discussion і Conclusions говорять про **один експеримент**.
- [ ] Числові твердження звірені з `Results_and_Discussion_v1_Example.md` зі Sprint 6.
- [ ] Related Work містить лише позначені місця для реально перевірених джерел; вигаданих цитувань немає.
- [ ] Приклад Research Package перевіряє існування файлів і не приховує відсутніх компонентів.
- [ ] Зразок не стверджує, що препринт уже опубліковано або що DOI вже існує.

## E2. Sprint Review — власне дослідження

- [ ] Рукопис оформлено у спільному DOCX-шаблоні; всі потрібні розділи заповнені.
- [ ] Усі RQ і H1 мають обґрунтовану відповідь або коректне зазначення невизначеності.
- [ ] Results ↔ таблиці/рисунки ↔ файли вимірювань узгоджені.
- [ ] Використано перевірені джерела Mendeley; немає плейсхолдерів у версії для публікації.
- [ ] Пакет містить код, протокол, дані/інструкції, результати, маніфест, звіт відтворюваності.
- [ ] Авторство, ліцензії й права на сторонні матеріали перевірені.
- [ ] Отримано або очікуємо документоване рішення наукового керівника.
- [ ] Статус публікації й DOI вказані без припущень.

## E3. Контрольні питання

1. Чим Manuscript відрізняється від Results and Discussion Sprint 6?
2. Які п'ять елементів необхідно відобразити у змістовному Abstract?
3. Чому перевірені джерела Literature Review Matrix не можна замінювати довільними посиланнями?
4. Яку інформацію в Methods треба зазначити, щоб метод був зрозумілим без читання всього коду?
5. Чим Research Package відрізняється від Research Release?
6. Навіщо перевіряти контрольні суми файлів?
7. Чому DOI не є підтвердженням наукової якості чи авторського права?
8. Чим Version DOI відрізняється від Concept DOI?
9. Що означає `Submit for review` для неопублікованого запису в Zenodo Community?
10. Хто приймає рішення про наукову готовність рукопису та як визначається авторство?
11. Які результати Sprint 7 можна вважати досягнутими, якщо рецензування ще не закінчено?

## G. Solutions to Training Exercises — відповіді для самоперевірки

**Вправа 1.** Варіант **Б**: твердження відповідає конкретному результату й не виходить за межі досліджених умов. Варіант А безпідставно узагальнює на всі випадки, В посилається на не виконану статистичну перевірку.

**Вправа 2.** Комплект неповний: бракує Experimental Protocol. Протокол фіксує фактори, умови, метрики та процедури, з якими звіряємо код і результати; самих таблиць для цього недостатньо.

**Вправа 3.** Ні: `Save draft` зберігає неопубліковану чернетку, DOI не вигадуємо. Наступний науковий крок — повний review керівником і внесення виправлень. Лише після погодження готуємо відповідне подання до Zenodo Community.

## Підсумок семитижневої практики

**Проблема → гіпотеза → огляд літератури → протокол → реалізація → основний експеримент → Results and Discussion → Manuscript + Research Package + наукова комунікація.**

Отриманий результат має перевірювану аргументацію, збережені артефакти й документований статус наукового review. Подальший розвиток може включати розширений експеримент, нову версію рукопису, погоджений Zenodo Release та подання до конференції чи журналу — відповідно до наукової готовності й вимог майданчика.
