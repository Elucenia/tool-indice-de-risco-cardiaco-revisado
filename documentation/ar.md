<!-- ELUCENIA technical documentation · indice-de-risco-cardiaco-revisado · ar · no clinical/professional/rights approval -->

# مؤشر الخطر القلبي المنقح (Lee)

[الشروط والمصادر والأذونات](https://elucenia.org/ar/tools/indice-de-risco-cardiaco-revisado)

## كيفية الاستخدام

استخدم الأداة في البوابة أو افتح index.html عبر خادم HTTP محلي. اختر اللغة، وأكمل الحقول، ثم أجرِ الحساب.

## المدخلات والوحدات

### جراحة عالية الخطورة (داخل الصفاق أو الصدر أو وعائية فوق الأربية)

`cir`

### مرض قلبي إقفاري (احتشاء سابق أو ذبحة أو اختبار إقفار إيجابي أو نترات أو موجة Q بالتخطيط)

`dac`

### قصور القلب (تاريخ مرضي أو وذمة رئوية أو ضيق نفس ليلي انتيابي أو صوت ثالث أو احتقان بالأشعة)

`icc`

### مرض وعائي دماغي (سكتة أو نوبة إقفارية عابرة)

`avc`

### سكري مع استخدام الإنسولين

`insulina`

### كرياتينين قبل الجراحة \> ٢٫٠ mg/dL

`cr`

## إصدار الطريقة

RCRI/لي 1999: 6 عوامل، 0–6؛ لا إعادة معايرة تلقائية

## المعادلة الموثقة

1 نقطة لكل عامل: جراحة عالية الخطورة، مرض قلبي إقفاري، قصور قلب، مرض وعائي دماغي، سكري بالإنسولين، كرياتينين \>2.0 mg/dL.

## الحدود والفئة السكانية

اشتُق RCRI الأصلي لدى أشخاص مستقرين بعمر لا يقل عن 50 سنة خضعوا لجراحة كبرى غير قلبية اختيارية. تخص المعدلات الأتراب التاريخية؛ ولا تشكل معايرة تلقائية للجراحة العاجلة أو الفئات الأخرى أو المستشفى الحالي. يجب أن تتوافق تعريفات العوامل وتفسيرها مع الدليل الإرشادي الساري.

## المراجع

- [Lee TH et al. Derivation and prospective validation of a simple index for prediction of cardiac risk of major noncardiac surgery. Circulation, 1999.](https://doi.org/10.1161/01.CIR.100.10.1043)

- [Duceppe E et al. Canadian Cardiovascular Society guidelines on perioperative cardiac risk assessment and management for patients who undergo noncardiac surgery. Can J Cardiol, 2017.](https://doi.org/10.1016/j.cjca.2016.09.008)

- [Halvorsen S et al. 2022 ESC Guidelines on cardiovascular assessment and management of patients undergoing non-cardiac surgery. Eur Heart J, 2022.](https://doi.org/10.1093/eurheartj/ehac270)

## إعادة إجراء الاختبارات التقنية

شغّل node test.cjs في المجلد الجذري لهذا المستودع لتكرار الحالات الاصطناعية المسجلة. تُحفظ المدخلات والنتائج المتوقعة وحدود التفاوت الأصلية. لا تُعدّ الاختبارات التقنية تحققًا سريريًا.

```sh
node test.cjs
```

يحتوي tool.json على المصادر والإصدار ونطاق المراجعة. يحتفظ examples.json بالمدخلات والنتائج المتوقعة للحالات الاصطناعية؛ ويسجل results.json النتائج التي تم الحصول عليها.

[السجل والمراجع](../tool.json) · [شيفرة JavaScript](../calculator.js) · [حالات مرجعية](../examples.json) · [results.json](../results.json)

## المراجعة وشروط الاستخدام

لم تُجرَ مراجعة سريرية مستقلة.

هذه الواجهة ترجمة أعدّها مؤلفوها، وليست إصدارًا رسميًا أو معتمدًا. لم تُجرَ مراجعة سريرية مستقلة أو مراجعة لغوية مهنية، ولم تُستكمل الموافقة على حقوق استخدام الأدوات.

نتيجة المعادلة أو التصنيف. يعتمد التفسير والتصرف ومدى الانطباق على التقييم المهني والمصدر المحدد.

## الترخيص ونسبة العمل إلى أصحابه

ينطبق Apache-2.0 على كود ELUCENIA فقط. تبقى حقوق الأدوات والمنشورات والترجمات والبيانات لأصحابها المعنيين. احتفظ بملفّي LICENSE وNOTICE.

ELUCENIA · Felipe Guedes · Copyright © 2026
