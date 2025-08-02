# ميسر - شرح المشروع باللهجة السعودية

هالمشروع بس تجربة (ديمو)، يعني مو تطبيق رسمي أو جاهز للاستخدام الفعلي. الهدف منه يوريك كيف ممكن يكون شكل تطبيق تمويل بالعربي، مع واجهة حديثة ودعم للكتابة بالصوت (تحويل الكلام لنص).

---

## وش يشتغل؟

- **التسجيل والدخول:** فيه شاشة ترحيب، تختار نوع الدخول، تحقق من الجوال (مو حقيقي)، وتضبط ملفك الشخصي.
- **الملف الشخصي:** تقدر تعدل بياناتك، تختار تاريخ الميلاد من تقويم، وكل شي ينحفظ بالجهاز.
- **التنقل بين الصفحات:** فيه شريط تحت تقدر تتنقل منه بين الرئيسية، الطلبات، الرسائل، والملف.
- **الرئيسية:** تعرض لك بطاقات ومعلومات (كلها ثابتة، ما فيه بيانات حقيقية).
- **الطلبات:** تقدر تسوي طلب جديد وتستخدم المايك عشان تعبي البيانات بالصوت.
- **تحويل الكلام لنص:**
  - يشتغل في كل خانات الطلب.
  - خانة المبلغ تحوّل الكلام لأرقام (مثلاً تقول "ستة آلاف" يكتبها 6000).
  - تضغط المايك مرة يبدأ يسجل، تضغطه مرة ثانية يوقف ويسوي التحويل.
- **الرسائل:** فيه شات وهمي (مو حقيقي).
- **واجهة حديثة ودعم للعربي بالكامل.**

---

## وش ما يشتغل؟

- **ما فيه تسجيل دخول حقيقي:** التحقق من الجوال كله تمثيل، ما يرسل ولا يستقبل أي رسائل.
- **ما فيه بيانات حقيقية أو سيرفر:** كل شي محفوظ بجهازك، ما فيه تواصل مع أي قاعدة بيانات أو سيرفر.
- **الطلبات والرسائل:** بس شكل، يعني لو حذفت التطبيق أو سويت إعادة تثبيت، كل شي يروح.
- **تحويل الكلام لنص:**
  - يستخدم خدمة AssemblyAI (لازم API Key عشان يشتغل صح، وما هو مدمج تلقائي).
  - أحياناً ما يفهم كل الأرقام أو اللهجات بدقة.
- **بعض الصفحات زي المستندات والإعدادات والمساعدة:** بس أزرار شكل، ما تشتغل.
- **الأمان:** لا تستخدمه لبياناتك الحقيقية أو أي شي مهم.

---

## كيف تجرب البرنامج؟

1. ثبت المتطلبات:
   ```bash
   npm install
   expo install @react-native-community/datetimepicker @react-native-async-storage/async-storage expo-av
   ```
2. شغل التطبيق:
   ```bash
   expo start
   ```
3. امسح الكود بالـ Expo Go على جوالك.

---

---

**ملاحظة:** هالمشروع للعرض والتجربة فقط، مو آمن ولا فيه بيانات حقيقية، ومو متصل بأي سيرفر.
- **Speech-to-Text:**
  - Works for all request fields.
  - Amount field intelligently converts Arabic number words (e.g. "ستة آلاف") to numbers (e.g. 6000).
  - Manual mic toggle (press to start, press again to stop and transcribe).
- **Messages:** Fake chat UI with sample conversations.
- **Modern Arabic RTL UI:** Consistent, RTL-friendly design and green theme.

---

## What is Simulated or Not Working

- **No Real Authentication:** Phone verification and login are simulated—no real SMS or backend.
- **No Real Backend:** All data is local to the app session or AsyncStorage. No cloud sync or server.
- **Requests & Messaging:** Data is not persistent across reinstalls and is not shared between users.
- **Speech-to-Text:**
  - Uses AssemblyAI API for transcription (requires API key, not included by default).
  - May not handle all complex Arabic numbers or dialects perfectly.
- **Document Upload, Settings, Help:** Menu items are placeholders and do not have real functionality.
- **No Production Security:** Not suitable for real user data or deployment.

---

## Notes

- This project is for demonstration and learning purposes only.
- Some UI flows and screens are static or partially implemented.
- You are free to extend, modify, or use this as a base for further development.

---

## Getting Started (for Demo Purposes)

1. Install dependencies:
   ```bash
   npm install
   expo install @react-native-community/datetimepicker @react-native-async-storage/async-storage expo-av
   ```
2. Start the Expo server:
   ```bash
   expo start
   ```
3. Scan the QR code with Expo Go on your device.

---

## Contact

For questions or suggestions, open an issue or contact the project maintainer.
