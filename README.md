# 🏫 Smart School Management System

> A comprehensive cross-platform school management platform that connects administrators, parents, and canteen staff — with real-time IoT attendance tracking, automated financial controls, and food safety management.

<div align="center">

![Flutter](https://img.shields.io/badge/Flutter-02569B?style=for-the-badge&logo=flutter&logoColor=white)
![Dart](https://img.shields.io/badge/Dart-0175C2?style=for-the-badge&logo=dart&logoColor=white)
![Firebase](https://img.shields.io/badge/Firebase-FFCA28?style=for-the-badge&logo=firebase&logoColor=black)
![Node.js](https://img.shields.io/badge/Node.js-339933?style=for-the-badge&logo=nodedotjs&logoColor=white)
![React](https://img.shields.io/badge/React-20232A?style=for-the-badge&logo=react&logoColor=61DAFB)

![Platform](https://img.shields.io/badge/Platform-iOS%20%7C%20Android%20%7C%20Web-lightgrey?style=flat-square)
![License](https://img.shields.io/badge/License-MIT-green?style=flat-square)
![Status](https://img.shields.io/badge/Status-Production%20Ready-brightgreen?style=flat-square)

</div>

---

## 📖 What Is This?

Managing a school involves dozens of moving parts — tracking whether kids actually showed up, making sure they're not eating something they're allergic to, controlling how much they spend at the canteen, and giving parents real visibility into their child's day.

This system ties all of that together in one platform. A smart bracelet worn by the student automatically logs attendance via IoT sensors. Parents get a daily summary on their phones. The canteen runs on a digital wallet with spending limits set by parents. Admins manage everything from a web dashboard.

**No more manual registers. No more mystery lunches. No more end-of-day surprises for parents.**

---

## ✨ Key Features

### 📱 Mobile App (Flutter — iOS & Android)
- **Dual interface** — separate flows for parents and canteen staff
- **Real-time attendance** — IoT smart bracelet integration auto-logs student check-ins
- **Daily reports** — parents receive automated attendance and spending summaries
- **Canteen wallet** — digital payments with parental spending limits and transaction history
- **Food safety** — allergen detection per meal, meal scheduling for the week ahead
- **Localization** — multi-language support out of the box

### 🖥️ Admin Web Dashboard (React.js)
- Full CRUD for students, staff, and admin accounts
- Attendance overview across all classes
- Financial reporting and transaction monitoring
- Role-based access control

### ⌚ IoT Integration
- Smart bracelets communicate with sensor devices at school entry/exit points
- Attendance is logged instantly — no manual intervention needed
- Edge cases (lost bracelet, sensor offline) are handled gracefully

### 💳 Financial Management
- Parents set daily/weekly spending caps for their child
- Every canteen transaction is recorded and visible in real time
- Automated alerts when a student approaches their limit

---

## 🏗️ Tech Stack

| Layer | Technology |
|---|---|
| Mobile App | Flutter & Dart |
| State Management | BLoC / Cubit |
| Web Dashboard | React.js |
| Backend & APIs | Node.js + Express.js |
| Database & Auth | Firebase (Firestore + Firebase Auth) |
| IoT Communication | REST APIs + sensor firmware |
| Payment | Stripe / PayPal integration |
| Maps | Google Maps API |

---

## 🚀 Getting Started

### Prerequisites

- Flutter SDK `>=3.0.0`
- Node.js `>=18.x`
- Firebase project (Firestore + Authentication enabled)
- Android Studio or Xcode (for mobile builds)

### 1. Clone the repo

```bash
git clone https://github.com/your-username/smart-school-system.git
cd smart-school-system
```

### 2. Set up Firebase

1. Create a project at [console.firebase.google.com](https://console.firebase.google.com)
2. Enable **Firestore** and **Authentication** (Email/Password)
3. Download `google-services.json` (Android) and `GoogleService-Info.plist` (iOS)
4. Place them in the correct directories:
   ```
   android/app/google-services.json
   ios/Runner/GoogleService-Info.plist
   ```

### 3. Run the mobile app

```bash
cd mobile
flutter pub get
flutter run
```

### 4. Run the backend

```bash
cd backend
npm install
cp .env.example .env   # fill in your Firebase credentials and API keys
npm start
```

### 5. Run the admin dashboard

```bash
cd web-dashboard
npm install
npm run dev
```

The dashboard will be available at `http://localhost:3000`.

---

## 📂 Project Structure

```
smart-school-system/
├── mobile/               # Flutter app (parent & canteen interfaces)
│   ├── lib/
│   │   ├── features/     # Feature-based architecture (BLoC)
│   │   ├── core/         # Shared utilities, theme, localization
│   │   └── main.dart
├── web-dashboard/        # React.js admin panel
│   ├── src/
│   │   ├── pages/
│   │   ├── components/
│   │   └── services/     # Firebase & API calls
├── backend/              # Node.js + Express REST API
│   ├── routes/
│   ├── controllers/
│   └── middleware/
└── iot/                  # Firmware docs & sensor integration specs
```

---

## 🔐 Environment Variables

Create a `.env` file in `/backend`:

```env
FIREBASE_PROJECT_ID=your_project_id
FIREBASE_PRIVATE_KEY=your_private_key
FIREBASE_CLIENT_EMAIL=your_client_email
GOOGLE_MAPS_API_KEY=your_maps_key
STRIPE_SECRET_KEY=your_stripe_key
```

---

## 📸 Screenshots

> _Add screenshots of the parent dashboard, canteen interface, and admin panel here._

| Parent Home | Canteen | Admin Dashboard |
|---|---|---|
| _(screenshot)_ | _(screenshot)_ | _(screenshot)_ |

---

## 🤝 Contributing

Contributions are welcome. Here's how:

1. Fork the repository
2. Create a feature branch: `git checkout -b feature/your-feature-name`
3. Commit your changes: `git commit -m 'Add: short description'`
4. Push to your branch: `git push origin feature/your-feature-name`
5. Open a Pull Request — describe what you changed and why

For bugs or feature requests, [open an issue](../../issues) with as much context as possible.

---

## 📬 Contact

**Omar Ali El-Sayed**
Full Stack Developer & Flutter Specialist

- 📧 omaraliabdelaziz250@gmail.com
- 📱 +20 155 112 9273
- 🌍 El-Sharqia, Egypt

---

## 📄 License

This project is licensed under the MIT License — see the [LICENSE](LICENSE) file for details.

---

<div align="center">
  <sub>Built with ❤️ as a graduation project at Zagazig University — Computer Science & Information Technology</sub>
</div>
