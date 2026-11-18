# HND Android App - Starter Project

यह Android Studio का शुरुआती प्रोजेक्ट है। ऐप वेबसाइट `https://harappanewsdarpa.com/` को WebView में खोलता है और नीचे Home, Reporter, E-Paper और Video नेविगेशन देता है।

## APK बनाने के लिए
1. Android Studio में `HND_Android_App_Starter` फ़ोल्डर खोलें।
2. Gradle sync पूरा होने दें।
3. Build > Build Bundle(s) / APK(s) > Build APK(s) चुनें।
4. APK `app/build/outputs/apk/debug/` में बनेगा।

## अभी किन चीज़ों की पुष्टि/सेटअप बाकी है
- Reporter Login और E-Paper के वास्तविक URL वेबसाइट के सही पेज मिलने पर `MainActivity.kt` में सेट करें। फिलहाल ये बटन वेबसाइट खोलते हैं।
- वीडियो बटन अभी HND के YouTube खोज परिणाम खोलता है। इसे आधिकारिक YouTube चैनल या वेबसाइट के वीडियो पेज से बदलें।
- असली push notifications के लिए Firebase Cloud Messaging (FCM), Firebase project, `google-services.json`, notification service और server-side push sender चाहिए। केवल ऐप बन जाने से ब्रेकिंग अलर्ट अपने-आप नहीं आएंगे।
- वेबसाइट पर अभी सार्वजनिक रूप से दिखने वाली सामग्री सीमित/placeholder जैसी दिख रही है; ऐप में समाचारों की गुणवत्ता और अपडेट वेबसाइट पर निर्भर होंगे।

## ऐप पहचान
App name: HND - Harappa News Darpan
Application ID: com.harappanewsdarpan.hnd
