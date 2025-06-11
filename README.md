# Clinical Dashboard Application

## 🏥 Description

Une application complète de tableau de bord clinique avec analyse diagnostique alimentée par IA, gestion des patients et recommandations de médicaments. L'application supporte trois langues : **Français**, **Anglais** et **Arabe** avec support RTL complet.

A comprehensive clinical dashboard application with AI-powered diagnostic analysis, patient management, and medication recommendations. The application supports three languages: **French**, **English**, and **Arabic** with full RTL support.

تطبيق شامل للوحة التحكم الطبية مع التحليل التشخيصي المدعوم بالذكاء الاصطناعي وإدارة المرضى وتوصيات الأدوية. يدعم التطبيق ثلاث لغات: **العربية** و**الإنجليزية** و**الفرنسية** مع دعم كامل للكتابة من اليمين إلى اليسار.

## ✨ Fonctionnalités / Features / الميزات

### Frontend
- 🔐 **Système d'authentification** / Authentication System / نظام المصادقة
- 📊 **Tableau de bord responsive** / Responsive Dashboard / لوحة تحكم متجاوبة
- 👥 **Gestion des patients** / Patient Management / إدارة المرضى
- 🧠 **Outil de diagnostic IA** / AI Diagnostic Tool / أداة التشخيص بالذكاء الاصطناعي
- 💊 **Système de médicaments** / Medication System / نظام الأدوية
- 📋 **Dossiers patients** / Patient Records / سجلات المرضى
- 🌓 **Basculement de thème** / Theme Toggle / تبديل المظهر
- 🌍 **Support multilingue** / Multilingual Support / دعم متعدد اللغات

### Backend (Python Flask)
- 🔌 **API RESTful** / RESTful API / واجهة برمجة تطبيقات RESTful
- 🗄️ **Base de données SQLite** / SQLite Database / قاعدة بيانات SQLite
- 🔒 **Authentification sécurisée** / Secure Authentication / مصادقة آمنة
- 📊 **Utilitaires de base de données** / Database Utilities / أدوات قاعدة البيانات

## 🚀 Installation et Démarrage / Installation & Setup / التثبيت والإعداد

### Prérequis / Prerequisites / المتطلبات المسبقة
- Node.js 18+
- Python 3.8+
- npm ou yarn

### 1. Installation des dépendances / Install Dependencies / تثبيت التبعيات

\`\`\`bash
# Frontend
npm install

# Backend (Python)
pip install flask flask-cors sqlite3
\`\`\`

### 2. Démarrage du Backend / Start Backend / تشغيل الخادم الخلفي

\`\`\`bash
# Initialiser et alimenter la base de données
python scripts/app.py
python scripts/seed_data.py
\`\`\`

### 3. Démarrage du Frontend / Start Frontend / تشغيل الواجهة الأمامية

\`\`\`bash
npm run dev
\`\`\`

### 4. Accès à l'application / Access Application / الوصول للتطبيق

- **URL**: http://localhost:3000
- **Identifiants de test** / Test Credentials / بيانات الاختبار:
  - Email: `doctor@example.com`
  - Mot de passe / Password / كلمة المرور: `password123`

## 🌍 Support des Langues / Language Support / دعم اللغات

L'application supporte trois langues avec basculement en temps réel :

The application supports three languages with real-time switching:

يدعم التطبيق ثلاث لغات مع التبديل في الوقت الفعلي:

- 🇫🇷 **Français** - Interface complète en français
- 🇺🇸 **English** - Full English interface  
- 🇸🇦 **العربية** - واجهة كاملة باللغة العربية مع دعم RTL

### Changement de langue / Language Switching / تغيير اللغة

Cliquez sur l'icône 🌍 dans l'en-tête pour changer de langue.

Click the 🌍 icon in the header to change language.

انقر على أيقونة 🌍 في الرأس لتغيير اللغة.

## 📁 Structure du Projet / Project Structure / هيكل المشروع

\`\`\`
clinical-dashboard/
├── app/                    # Pages Next.js / Next.js Pages / صفحات Next.js
├── components/             # Composants React / React Components / مكونات React
│   ├── language-provider.tsx    # Fournisseur de langue / Language Provider / مزود اللغة
│   ├── language-selector.tsx    # Sélecteur de langue / Language Selector / منتقي اللغة
│   └── ...
├── scripts/               # Scripts Backend Python / Python Backend Scripts / سكريبت الخادم الخلفي
│   ├── app.py            # Serveur API Flask / Flask API Server / خادم Flask API
│   ├── seed_data.py      # Données d'exemple / Sample Data / بيانات العينة
│   └── database_utils.py # Utilitaires DB / DB Utilities / أدوات قاعدة البيانات
└── ...
\`\`\`

## 🔧 API Endpoints

### Authentification / Authentication / المصادقة
- `POST /api/auth/login` - Connexion / Login / تسجيل الدخول
- `POST /api/auth/register` - Inscription / Register / التسجيل
- `POST /api/auth/logout` - Déconnexion / Logout / تسجيل الخروج

### Patients
- `GET /api/patients` - Liste des patients / Patient List / قائمة المرضى
- `POST /api/patients` - Créer patient / Create Patient / إنشاء مريض
- `GET /api/patients/<id>` - Détails patient / Patient Details / تفاصيل المريض

### Diagnostics
- `POST /api/diagnostics/analyze` - Analyse IA / AI Analysis / التحليل بالذكاء الاصطناعي

### Médicaments / Medications / الأدوية
- `GET /api/medications` - Liste médicaments / Medication List / قائمة الأدوية
- `GET /api/patients/<id>/vitals` - Signes vitaux / Vital Signs / العلامات الحيوية

## 🎨 Thèmes / Themes / المظاهر

- 🌞 **Mode clair** / Light Mode / الوضع الفاتح
- 🌙 **Mode sombre** / Dark Mode / الوضع المظلم
- 🔄 **Auto (système)** / Auto (System) / تلقائي (النظام)

## 📱 Support RTL

Support complet pour l'arabe avec :
- Direction de texte de droite à gauche
- Mise en page inversée
- Navigation adaptée
- Polices arabes optimisées

Full Arabic support with:
- Right-to-left text direction
- Mirrored layout
- Adapted navigation
- Optimized Arabic fonts

دعم كامل للعربية مع:
- اتجاه النص من اليمين إلى اليسار
- تخطيط معكوس
- تنقل متكيف
- خطوط عربية محسنة

## 🔒 Sécurité / Security / الأمان

- Hachage des mots de passe / Password hashing / تشفير كلمات المرور
- Sessions sécurisées / Secure sessions / جلسات آمنة
- Validation des données / Data validation / التحقق من البيانات
- Protection CORS / CORS protection / حماية CORS

## 📄 Licence / License / الترخيص

MIT License - Voir LICENSE pour plus de détails.
MIT License - See LICENSE for details.
رخصة MIT - راجع LICENSE للتفاصيل.

## 🤝 Contribution

Les contributions sont les bienvenues ! Veuillez lire CONTRIBUTING.md pour plus de détails.

Contributions are welcome! Please read CONTRIBUTING.md for details.

المساهمات مرحب بها! يرجى قراءة CONTRIBUTING.md للتفاصيل.

## 📞 Support

Pour toute question ou problème, veuillez ouvrir une issue sur GitHub.

For any questions or issues, please open an issue on GitHub.

لأي أسئلة أو مشاكل، يرجى فتح مشكلة على GitHub.
