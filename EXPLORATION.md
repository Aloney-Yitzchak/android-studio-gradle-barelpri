חקר Android Studio – תשובות התלמיד

שם התלמיד: בראל פריצקר 
תאריך: _______________

חלק א' – סיור ב-Android Studio (30 נקודות)
שאלה 1: תיקיות ראשיות (10 נקודות)

<img width="1000" height="667" alt="image" src="https://github.com/user-attachments/assets/ccaa05ac-7900-4a6c-8d17-5f058393ac7c" />

שמות 3 התיקיות הראשיות:

manifests

java

res

שאלה 2: AndroidManifest.xml (10 נקודות)

<img width="736" height="891" alt="image" src="https://github.com/user-attachments/assets/281c3407-4f07-496f-a4e4-931879c6fdb1" />

מה התפקיד של קובץ זה? (2–3 משפטים)
קובץ AndroidManifest.xml מגדיר מידע בסיסי על האפליקציה.
בקובץ זה מוגדרות ה-Activities של האפליקציה, ההרשאות שלה, ושם החבילה.
בנוסף, הוא קובע איזו Activity תיפתח ראשונה כאשר מפעילים את האפליקציה.

שאלה 3: תיקיית res (10 נקודות)

<img width="191" height="184" alt="image" src="https://github.com/user-attachments/assets/3b162bb9-fde8-4dc0-a26a-c573e1cf60d1" />

3 תיקיות משנה בתוך res:

layout

values

drawable

מה נמצא בכל אחת מהתיקיות האלה?

בתיקיית layout נמצאים קבצי XML שמגדירים את מבנה המסכים של האפליקציה.

בתיקיית values נמצאים קבצים כמו strings.xml שמכילים טקסטים, צבעים וסגנונות.

בתיקיית drawable נמצאות תמונות, אייקונים וקבצי גרפיקה.

חלק ב' – עבודה עם Gradle (40 נקודות)
שאלה 4: build.gradle (Module) (15 נקודות)

<img width="369" height="434" alt="image" src="https://github.com/user-attachments/assets/488a15ca-6d47-41eb-946a-d25a150095d7" />

איזו שורה הוספת בדיוק?

implementation 'com.google.code.gson:gson:2.10.1'

שאלה 5: מה זה Gson? (15 נקודות)

הסבר במילים שלך: מה Gson עושה ולמה זה שימושי?
Gson היא ספרייה של Google שמאפשרת להמיר אובייקטים ב-Java לפורמט JSON ולהפך.
היא שימושית מאוד כאשר האפליקציה מתקשרת עם שרתים ושולחת או מקבלת מידע בצורה מסודרת.

דוגמה לשימוש באפליקציה אמיתית:
באפליקציות כמו WhatsApp או Instagram משתמשים ב-Gson כדי להמיר נתונים שמתקבלים מהשרת (כמו הודעות, משתמשים או פוסטים) לאובייקטים שהאפליקציה יכולה לעבוד איתם.

שאלה 6: Gradle Sync (10 נקודות)

מה קורה כשלוחצים על "Sync Now"?
כאשר לוחצים על Sync Now, Gradle מוריד את ה-dependencies שהוגדרו ומעדכן את הפרויקט בהתאם לשינויים.

מה יקרה אם לא נלחץ על Sync Now אחרי שהוספנו dependency?
הספרייה לא תיטען, והקוד ישתמש במחלקות שלא קיימות, מה שיגרום לשגיאות בקומפילציה.

חלק ג' – ארגון קבצים (30 נקודות)
שאלה 7: strings.xml (10 נקודות)

<img width="1916" height="1071" alt="image" src="https://github.com/user-attachments/assets/4366488c-5787-4a80-8048-287a1f81930b" />

3 ה-strings שהוספתי:

app_name

hello_text

welcome_message

שאלה 8: Layout File חדש (10 נקודות)

איך יצרת layout file חדש? (שלב אחר שלב)

לחצתי קליק ימני על תיקיית layout

בחרתי New

בחרתי Layout Resource File

נתתי שם לקובץ ולחצתי OK

<img width="1919" height="1079" alt="image" src="https://github.com/user-attachments/assets/a2711826-db6a-4761-89b4-968615fe4538" />

שאלה 9: הבנה כללית (10 נקודות)

מה ההבדל בין build.gradle (Project) ל-build.gradle (Module)?
build.gradle (Project) מגדיר הגדרות כלליות לכל הפרויקט,
ואילו build.gradle (Module) מגדיר הגדרות ספציפיות לאפליקציה עצמה כמו dependencies ו-SDK.

למה חשוב להפריד בין קוד (java/) לבין משאבים (res/)?
ההפרדה עוזרת לשמור על סדר בפרויקט, מקלה על תחזוקה, ומאפשרת שינוי עיצוב או טקסטים בלי לגעת בקוד.

שאלות בונוס (10 נקודות)
בונוס 1 (5 נקודות)

Dependency:

implementation 'androidx.recyclerview:recyclerview:1.3.2'


מה הוא עושה:
RecyclerView מאפשר להציג רשימות בצורה יעילה וחלקה, כמו רשימת הודעות או פוסטים.

בונוס 2 (5 נקודות)

מה ההבדל בין minSdk ל-targetSdk?
minSdk מגדיר את גרסת האנדרואיד המינימלית שעליה האפליקציה יכולה לרוץ,
targetSdk מגדיר לאיזו גרסת אנדרואיד האפליקציה מותאמת ומתנהגת לפיה.

סיכום אישי

מה למדת היום שהכי עזר לך להבין את Android Studio?
הבנתי איך בנוי פרויקט Android ואיך Gradle מנהל ספריות והגדרות.

מה היה הכי מאתגר?
להבין את המבנה של Gradle וההבדל בין Project ל-Module.

סיימתי את המשימה! ✅

זמן שלקח לי: ______ דקות
