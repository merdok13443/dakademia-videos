# dakademia-videos

סרטונים מוגמרים של **דקדמיה** (Dakademia), מאוחסנים כאן כדי שלכל סרטון תהיה כתובת ציבורית ישירה ויציבה ש-Buffer יכול להוריד ולפרסם ב-YouTube, Instagram ו-TikTok.

המאגר הזה הוא אחסון בלבד. הקוד, ההנחיות והדמות נמצאים ב-[merdok13443/skills](https://github.com/merdok13443/skills).

## מבנה

```
<course-slug>/
  u<NN>-e<NN>.mp4      # יחידה NN, פרק NN בתוך היחידה
  u<NN>-e<NN>.json     # מטא-דאטה של הפרסום (כותרת, כיתוב, האשטגים, מזהי פוסטים ב-Buffer)
test/                  # קבצי בדיקה של הצינור, לא לפרסום
```

- `course-slug` באנגלית, אותיות קטנות ומקפים (למשל `discrete-math`).
- מספרים תמיד בשתי ספרות: `u01-e03.mp4`.
- קובץ שפורסם לא מוחלף. גרסה מתוקנת מקבלת סיומת: `u01-e03-v2.mp4`.

## כתובות

כל קובץ זמין בשתי כתובות ישירות:

| כתובת | מתי |
|---|---|
| `https://merdok13443.github.io/dakademia-videos/<course-slug>/u01-e03.mp4` | ברירת מחדל (GitHub Pages, נשלח כ-`video/mp4`). מתעדכן כדקה אחרי ה-push. |
| `https://raw.githubusercontent.com/merdok13443/dakademia-videos/main/<course-slug>/u01-e03.mp4` | גיבוי, זמין מיד אחרי ה-push. |

לפני שמעבירים כתובת ל-Buffer בודקים שהיא מחזירה `200` ואת גודל הקובץ הנכון.

## מגבלות

- קובץ עד 100MB (שורט של דקה הוא בערך 5-20MB).
- GitHub ממליץ על מאגר עד כ-1GB ואתר Pages עד 1GB. כשמתקרבים לזה, פותחים מאגר המשך (`dakademia-videos-2`).
