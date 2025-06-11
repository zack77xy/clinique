# Guide d'Installation / Installation Guide / دليل التثبيت

## 🚀 Installation Rapide / Quick Installation / التثبيت السريع

### 1. Prérequis / Prerequisites / المتطلبات

Assurez-vous d'avoir installé :
Make sure you have installed:
تأكد من تثبيت:

- **Node.js** (version 18 ou supérieure / version 18 or higher / الإصدار 18 أو أحدث)
- **Python** (version 3.8 ou supérieure / version 3.8 or higher / الإصدار 3.8 أو أحدث)
- **npm** ou **yarn**

### 2. Téléchargement / Download / التحميل

Téléchargez et extrayez le fichier ZIP de l'application.
Download and extract the application ZIP file.
قم بتحميل واستخراج ملف ZIP للتطبيق.

### 3. Installation des Dépendances / Install Dependencies / تثبيت التبعيات

\`\`\`bash
# Naviguez vers le dossier du projet
# Navigate to project folder
# انتقل إلى مجلد المشروع
cd clinical-dashboard

# Installez les dépendances frontend
# Install frontend dependencies
# ثبت تبعيات الواجهة الأمامية
npm install

# Installez les dépendances backend Python
# Install Python backend dependencies
# ثبت تبعيات Python للخادم الخلفي
pip install -r requirements.txt
\`\`\`

### 4. Configuration de la Base de Données / Database Setup / إعداد قاعدة البيانات

\`\`\`bash
# Initialisez et alimentez la base de données
# Initialize and seed the database
# قم بتهيئة وملء قاعدة البيانات
python scripts/seed_data.py
\`\`\`

### 5. Démarrage de l'Application / Start Application / تشغيل التطبيق

#### Terminal 1 - Backend:
\`\`\`bash
python scripts/app.py
\`\`\`

#### Terminal 2 - Frontend:
\`\`\`bash
npm run dev
\`\`\`

### 6. Accès / Access / الوصول

Ouvrez votre navigateur et allez à :
Open your browser and go to:
افتح متصفحك واذهب إلى:

**http://localhost:3000**

### 7. Connexion de Test / Test Login / تسجيل دخول تجريبي

Utilisez ces identifiants pour vous connecter :
Use these credentials to login:
استخدم هذه البيانات لتسجيل الدخول:

- **Email**: doctor@example.com
- **Mot de passe / Password / كلمة المرور**: password123

## 🌍 Changement de Langue / Language Change / تغيير اللغة

1. Cliquez sur l'icône 🌍 dans l'en-tête
2. Sélectionnez votre langue préférée :
   - 🇫🇷 Français
   - 🇺🇸 English  
   - 🇸🇦 العربية

## ✅ Vérification de l'Installation / Installation Verification / التحقق من التثبيت

Si tout fonctionne correctement, vous devriez voir :
If everything works correctly, you should see:
إذا كان كل شيء يعمل بشكل صحيح، يجب أن ترى:

- ✅ Page de connexion avec sélecteur de langue
- ✅ Tableau de bord après connexion
- ✅ Navigation entre les sections
- ✅ Changement de thème (clair/sombre)
- ✅ Support RTL pour l'arabe

## 🔧 Dépannage / Troubleshooting / استكشاف الأخطاء

### Problème : Port déjà utilisé / Port already in use / المنفذ مستخدم بالفعل

\`\`\`bash
# Changez le port pour le frontend
# Change port for frontend
# غير المنفذ للواجهة الأمامية
npm run dev -- -p 3001

# Changez le port pour le backend
# Change port for backend  
# غير المنفذ للخادم الخلفي
# Modifiez app.py ligne: app.run(port=5001)
\`\`\`

### Problème : Erreur de base de données / Database error / خطأ قاعدة البيانات

\`\`\`bash
# Supprimez et recréez la base de données
# Delete and recreate database
# احذف وأعد إنشاء قاعدة البيانات
rm clinical_dashboard.db
python scripts/seed_data.py
\`\`\`

### Problème : Modules Python manquants / Missing Python modules / وحدات Python مفقودة

\`\`\`bash
# Installez les modules individuellement
# Install modules individually
# ثبت الوحدات بشكل فردي
pip install flask
pip install flask-cors
\`\`\`

## 📞 Support

Si vous rencontrez des problèmes :
If you encounter issues:
إذا واجهت مشاكل:

1. Vérifiez que tous les prérequis sont installés
2. Assurez-vous que les ports 3000 et 5000 sont libres
3. Consultez les logs dans les terminaux
4. Redémarrez l'application

Check that all prerequisites are installed
Make sure ports 3000 and 5000 are free
Check logs in terminals
Restart the application

تحقق من تثبيت جميع المتطلبات المسبقة
تأكد من أن المنافذ 3000 و 5000 متاحة
راجع السجلات في الطرفيات
أعد تشغيل التطبيق
