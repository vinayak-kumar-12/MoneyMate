# 📱 MoneyMate 2.0 Frontend (Mobile App)

> **A Premium Fintech Experience.**  
> Built with React Native and Expo, this application delivers a high-fidelity, futuristic interface for managing GenZ finances.

---

## 🎨 Design System: Electric Obsidian

The frontend uses a custom design system characterized by:
- **Glassmorphism**: Soft blurs and semi-transparent cards.
- **Vibrant Gradients**: Indigo to Sky flows for high energy.
- **Micro-interactions**: Smooth layout transitions powered by Reanimated 3.
- **Context-Aware Cards**: UI elements that change state based on financial activity levels.

---

## 🚀 Key Modules

### 1. Home Dashboard
Quick overview of net balance, active investments, and quick actions for money transfer.

### 2. Activity & Analytics
Deep-dive into spending patterns with real-time donut charts and a detailed banking ledger.

### 3. Message Cabinet
A smart sorting hub that isolates:
- **📦 E-commerce**: Order and delivery tracking.
- **🔐 OTP**: Auto-deleting security codes (15m).
- **🚫 Spam**: Auto-clearing promotional clutter (1h).

### 4. Parental Control
Dedicated monitoring suite for child activity with spend limits and activity badges.

---

## 🛠️ Setup & Running

1. **Install Dependencies**:
   ```bash
   npm install
   ```

2. **Starting the Development Server**:
   ```bash
   npx expo start -c
   ```

3. **Connecting a Device**:
   Open the **Expo Go** app on your phone and scan the QR code displayed in the terminal.

---

## 📂 Internal Directory Structure

- `/src/screens`: Main UI screens (Activity, Home, ParentalControl).
- `/src/context`: State management (Auth, Finance, SMSAnalytics).
- `/src/services`: API interaction layers (Payment, SMSBot, Security).
- `/src/components`: Reusable UI elements (GlassCard, CustomDrawer).
- `/src/constants`: Theme definitions and shared styles.

---

## 🏗️ Technical Dependencies

- **Navigation**: React Navigation (Bottom Tabs + Side Drawer).
- **Animations**: React Native Reanimated.
- **Graphics**: SVG and Expo Linear Gradient.
- **State**: React Context API.
- **Network**: Axios and Socket.io-client.

---

*MoneyMate Framework — Version 2.0.1 Stable*
