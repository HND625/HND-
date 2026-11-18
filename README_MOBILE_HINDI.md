# HND ऐप — मोबाइल से APK बनवाने का तरीका

यह Android ऐप का source project है, APK फाइल नहीं। इस प्रोजेक्ट में GitHub Actions workflow जोड़ा गया है जो GitHub पर डालने के बाद APK बना सकता है।

## केवल मोबाइल से APK बनाने के चरण
1. ZIP को फोन में डाउनलोड करके Extract करें।
2. Chrome में https://github.com खोलें और अपने खाते में साइन इन करें (यदि खाता नहीं है तो बनाएं)।
3. New repository बनाएं, नाम `HND-Android-App` रखें और Public या Private चुनकर Create repository करें।
4. Repository में Add file → Upload files चुनें। ZIP को पहले Extract करें; उसके अंदर की सभी फाइलें और `.github` फ़ोल्डर सहित अपलोड करें। सीधे ZIP फाइल अपलोड न करें।
5. Commit changes करें। GitHub Actions टैब खोलें। `Build HND Android APK` workflow चुनें और जरूरत हो तो `Run workflow` दबाएं।
6. Build पूरा होने पर उस run को खोलें। नीचे Artifacts में `HND-debug-APK` डाउनलोड करें। ZIP को Extract करें; अंदर `app-debug.apk` होगा।
7. APK अपने फोन में खोलकर Android के निर्देशों के अनुसार इंस्टॉल करें।

## ध्यान दें
- यह शुरुआती WebView ऐप है; वेबसाइट के पेज ऐप के भीतर खुलते हैं।
- Reporter और E-Paper के URL वेबसाइट पर सही/उपलब्ध होने चाहिए। अभी दिए गए URL अनुमानित paths हैं।
- असली push notifications के लिए Firebase और वेबसाइट/server पर अलग सेटअप जरूरी है; इस starter में वे सक्रिय नहीं हैं।
- APK debug-signed होगा, Play Store पर प्रकाशित करने के लिए release signing अलग से करनी होगी।
