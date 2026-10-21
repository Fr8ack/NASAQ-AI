# NASAQ V1.2 — تقرير الاختبارات

**التاريخ:** 20 أكتوبر 2026

| الاختبار | النتيجة | الحدود |
|---|---|---|
| `npm test` | 9/9 PASS | وحدات أمن واسترجاع باستبدالات mocks؛ ليس اتصالًا حقيقيًا |
| Arabic numerals / named surah ref | PASS | اختبار من بيانات اصطناعية موسومة داخل ملف الاختبار فقط، لا ضمن corpus المنتج |
| citation allowlist | PASS | يمنع قبول استشهاد غير مسترجع في نتائج التحليل |
| Reject invented/partial corpus | PASS | لا يسمح باعتبار 43 نصًا قديمًا القرآن كاملًا |
| `npm run verify:corpus` | SAFE STOP | يعلن 0/6236، لا اعتماد مدونة |
| TypeScript parsing | 27/27 PASS | ليس full type-check |
| `npm install --offline` | BLOCKED | `@google/genai` غير مخزن ضمن اعتماديات npm المحلية |
| `npm run lint` | BLOCKED | Vite/client types غير مثبتة |
| `npm run build` | BLOCKED | vite غير مثبت |
| Firebase Emulator / Auth / Rules | NOT RUN | لا تعتمد سلامة إنتاجية |
| Gemini live API | NOT RUN | لا يوجد مفتاح API أو اتصال مثبت |
| Browser / mobile E2E | NOT RUN | لا Chromium / حزمة تشغيل كاملة |

**النتيجة:** أُنجز عمل برمجي مُختبر محدود النطاق. لم يتضح نجاح الموقع عند تشغيله أو نشره؛ ولم يتم إثبات دقة المدونة الكاملة. لا يُسمح بإعلان المشروع مكتملًا.
