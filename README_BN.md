# CF Chowdhury Fashion Sales Manager — Android project

এটি Android Studio-তে খোলার মতো একটি native Android wrapper project। ভেতরে আগের CF web app-টি asset হিসেবে রাখা হয়েছে। Project target SDK 36 সেট করা আছে।

## APK / AAB তৈরি করার ধাপ
1. কম্পিউটারে Android Studio (সাম্প্রতিক stable version) ইনস্টল করুন।
2. ZIP Extract করে Android Studio-তে `CF-Android-Project` ফোল্ডারটি Open করুন।
3. Gradle sync শেষ হতে দিন; Android SDK Platform 36 ইনস্টল করতে বললে ইনস্টল করুন।
4. ফোনে পরীক্ষা করতে Run চাপুন।
5. Play Store-এর জন্য: **Build → Generate Signed Bundle / APK → Android App Bundle** নির্বাচন করুন। নতুন signing key নিরাপদে সংরক্ষণ করুন। তৈরি হওয়া `.aab` ফাইলটি Play Console-এ upload করতে হয়।

## গুরুত্বপূর্ণ সীমাবদ্ধতা
- এই ফাইলটি Android Studio project source; এখানে প্রস্তুত/সাইন করা APK বা AAB নেই। এই পরিবেশে Android build চালিয়ে যাচাই করা হয়নি।
- বর্তমান web app-এর ডেটা একই অ্যাপ/ডিভাইসের local storage-এ থাকে। Cloud sync/login এখনো যুক্ত নয়। একাধিক ডিভাইসে নিরাপদ cloud data চাইলে Firebase Authentication + Firestore + security rules যুক্ত ও পরীক্ষা করতে হবে।
- Google Play-এ প্রকাশ স্বয়ংক্রিয় নয়। Developer account, app icon, screenshots, privacy policy, Data safety form, content rating এবং Play review লাগতে পারে।
- বাস্তব customer data দেওয়ার আগে backup এবং app behavior পরীক্ষা করুন।
