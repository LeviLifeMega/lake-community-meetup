# Health Declaration Form - Content Plan (Hebrew retreat health waiver)

Standard Israeli fitness/retreat health declaration fields, based on common workshop/ice-bath/breathwork liability forms:

1. פרטים אישיים: שם מלא, ת.ז., טלפון, תאריך לידה, תאריך המילוי
2. הצהרת בריאות כללית (כן/לא לכל סעיף):
   - מחלות לב וכלי דם / יתר לחץ דם
   - בעיות נשימה (אסתמה וכו')
   - סוכרת
   - אפילפסיה / התקפים
   - הריון
   - ניתוחים לאחרונה (פחות מ-6 חודשים)
   - בעיות פסיכיאטריות/פאניקה משמעותיות
   - כל מגבלה רפואית אחרת (שדה טקסט חופשי)
3. סעיף ייעודי לטבילה במים קרים: אזהרה על shock תרמי, התחייבות שלא סובל ממחלת לב לא מאובחנת/לחץ דם לא מאוזן
4. הצהרה משפטית: "הנני מצהיר/ה כי כל הפרטים נכונים, ואני משתתפ/ת מרצוני החופשי ועל אחריותי הבלעדית..." + פטור מאחריות (assumption of risk) כלפי LeviLife והמארגנים
5. חתימה דיגיטלית: canvas לחתימה עם העכבר/אצבע + תאריך אוטומטי
6. שליחה: submit -> שולח מייל ל-office@levilife.com, subject = "<שם הממלא> - הצהרת בריאות רטריט לוילייף 21.8.26"

Implementation: client-side HTML form + signature pad (canvas), on submit convert to formatted email body (mailto: fallback OR serverless form endpoint). Given this is a static GitHub Pages site (no backend), use Formspree or a mailto: link with pre-filled body as pragmatic no-backend solution, OR EmailJS for actual silent email send with signature image attached.
