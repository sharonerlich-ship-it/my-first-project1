# הוראות העלאה ל-GitHub

## אפשרות 1: דרך GitHub Desktop (הכי קל)

1. הורד והתקן [GitHub Desktop](https://desktop.github.com/)
2. התחבר לחשבון GitHub שלך
3. לחץ על "File" > "Add Local Repository"
4. בחר את התיקייה: `C:\Users\sharo\OneDrive\שולחן העבודה\Cursor projects`
5. לחץ על "Publish repository" כדי להעלות ל-GitHub

## אפשרות 2: דרך האתר של GitHub

1. היכנס ל-[GitHub.com](https://github.com) והתחבר
2. לחץ על הכפתור הירוק "New" או "New repository"
3. תן שם למאגר (למשל: `israeli-stocks-tracker`)
4. בחר "Public" או "Private"
5. **אל תסמן** "Initialize this repository with a README"
6. לחץ על "Create repository"
7. אחרי יצירת המאגר, תראה הוראות - בחר "uploading an existing file"
8. גרור את הקובץ `israeli-stocks-tracker.html` לחלון הדפדפן
9. לחץ על "Commit changes"

## אפשרות 3: דרך Git Command Line

אם Git מותקן במחשב שלך:

```bash
# נווט לתיקייה
cd "C:\Users\sharo\OneDrive\שולחן העבודה\Cursor projects"

# אתחל מאגר Git
git init

# הוסף את הקבצים
git add israeli-stocks-tracker.html

# צור commit
git commit -m "הוספת מעקב מניות ישראליות עם תקופת 5 שנים"

# הוסף את ה-remote של GitHub (החלף YOUR_USERNAME בשם המשתמש שלך)
git remote add origin https://github.com/YOUR_USERNAME/israeli-stocks-tracker.git

# העלה ל-GitHub
git push -u origin main
```

## הערות חשובות

- אם אתה משתמש ב-GitHub Desktop או באתר, אתה לא צריך להתקין Git בנפרד
- ודא שיש לך חשבון GitHub פעיל
- אם המאגר כבר קיים, תוכל פשוט לגרור את הקובץ דרך האתר

