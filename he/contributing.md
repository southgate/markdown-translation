מ: https://github.com/facebook/chef-cookbooks/edit/master/CONTRIBUTING.md

# תרומה לספרי הבישול של השף של פייסבוק

## בדיקת סימון

הנה  ~~כמה ~~ בדיקות מארקדאון בטעם GitHub @southgate.

לאחר מכן: | ok_hand: | זועף: |
---------|----------|----------|
מזל טוב ענק  | פחות ברכות | אין מזל טוב

- [ ] משימה 1
- [ ] משימה 2
- [ ] משימה 3

## תהליך הפיתוח שלנו
מאגר זה מסונכרן ממאגר פנימי. אנחנו בהחלט מקבלים משיכה
מבקש ויטפל במיזוג כראוי.

אנו משתמשים ב-Foodcritic לבדיקת נכונות שף ורובוקופ לסגנון רובי
להסתעף. ערכות החוקים שלנו מסונכרנות הן פנימית והן חיצונית כדי להבטיח
איכות וסגנון קוד עקביים לכולם.

## הסכם רישיון משתתף ("CLA")
על מנת לקבל את בקשת המשיכה שלך, אנחנו צריכים שתגיש CLA. אתה רק צריך
לעשות זאת פעם אחת כדי לעבוד על כל אחד מפרויקטי הקוד הפתוח של פייסבוק.

השלם את ה- CLA שלך כאן: <https://code.facebook.com/cla>

## דרישות מוקדמות
ראשית, תודה על העניין שלך בתרומה, אנו מקדמים בברכה בקשות משיכה!

לפני שליחת בקשת משיכה לריפו זה חשוב לזכור כי
API מונחה תכונות כאן הם מודל שונה מאוד מקהילה אחרת
ספרי בישול. כדי לבנות את המודל הזה, יש דרך ספציפית לספרי בישול
להיכתב.

אנו ממליצים בחום להבטיח שתקרא את [README.md](README.md)
[Philosphy.md](https://github.com/facebook/chef-utils/blob/master/Philosophy.md).
אנו ממליצים גם להגדיר סביבה המשתמשת בהזמנת רשימת הריצה שלנו
(ספרי בישול הליבה הראשון, כל דבר אחר אחרי).

לבסוף, אנא ודא שאתה מבין את הגישה 3 שלבים:

 * `attributes/` קבצים מגדירים API ולעולם אל תיגעו בתכונות של ספר בישול אחר.
 * `recipes/` משאבי כיוונון קבצים (כגון תבניות או שירותים) ושימוש בהם
   API (לקרוא: להגדיר תכונות עבור ספרי בישול אחרים)
 * התכונות נצרכות רק אי פעם ב `runtime`(aka  `converge time`).
   דוגמאות לכך כוללות  `templates`,  `ruby_blocks`או `whyrun_safe_ruby_blocks` 
   `providers`.

## בעיות
אנו משתמשים בבעיות GitHub כדי לעקוב אחר באגים ציבוריים. נא ודא שהתיאור שלך הוא
ברור ויש לו הוראות מספיקות כדי להיות מסוגל לשחזר את הבעיה.

לפייסבוק יש [תוכנית שפע](https://www.facebook.com/whitehat/)כספת
גילוי באגים באבטחה. במקרים אלה, נא לעבור את התהליך
המתואר בדף זה ואינו מגיש בעיה ציבורית.

## שליחת בקשת משיכה

יש לך תיקון או תכונה? מגניב! כאשר אתה שולח את בקשת המשיכה אנו מציעים לך
כוללים פלט מסוים של שף ישים.

אם זהו API (תכונה) חדש, נא ודא שהוא מתועד כראוי
ספר בישול README.

אנו נחזיק את כל התרומות לאותם תקני איכות וסגנון כמו
קוד קיים.


### ספרי בישול חדשים

אנחנו רוצים לשמור על הריפו הזה ממוקד בספרי בישול "ליבה" שמנהלים את הבסיס
Os. אם אתה רוצה לתרום ספר בישול כזה, אנו ממליצים לך להתחיל על ידי
הגשת בעיה תחילה כדי למנוע שכפול מאמץ (ייתכן שיש לנו אחד שאנחנו יכולים
נסה ליצור קוד פתוח, או שאנשים אחרים יכתבו קוד כזה) לפני שיעבדו עליו.

אם אתה רוצה לתרום ספר בישול שלא נופל בקטגוריה זו (למשל.
ניהול דברים בשולחן העבודה או שירותים אחרים), אז אנו מציעים לך להצביע לנו יחסי ציבור
על ריפו שבו אתה רוצה לשמור את זה ואנחנו נשמח לסקור אותו ולהוסיף
מצביע על הריפו שלך ב 
[UNIVERSE.md](https://github.com/facebook/chef-cookbooks/blob/master/UNIVERSE.md)
קובץ, קובץ.

אנו משתמשים `fb_`בקידומת כדי לציין ספרי בישול שמתאימים
מודל זה ומגיעים מן הריפו הזה, אבל אל תהסס לפרסם ספרי בישול במקום אחר
שעוזבים מודל זה ומשתמשים בקידומות אחרות.

## רשיון
על ידי תרומה למאגר זה, אתה מסכים שהתרומות שלך יהיו
מורשה תחת רישיון אפאצ'י 2.0 שלו.
