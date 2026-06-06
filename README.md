# Habits Tracker - Expenses & Workout Tracker with AI

Web app untuk tracking pengeluaran dan workout dengan AI insights menggunakan Ollama (local AI).

## Fitur MVP

### Expenses Tracker
- ✅ Catat pengeluaran dengan kategori, jumlah, tanggal, dan keterangan
- ✅ Lihat riwayat pengeluaran
- ✅ Analisis pengeluaran per kategori (pie chart)
- ✅ Filter by date range dan kategori
- ✅ AI insights: rekomendasi penghematan berdasarkan pola pengeluaran

### Workout Tracker
- ✅ Catat workout: tipe exercise, durasi, intensitas, kalori terbakar
- ✅ Lihat riwayat workout
- ✅ Progress tracking: weekly stats
- ✅ Filter by exercise type dan date range
- ✅ AI insights: rekomendasi workout dan motivasi berdasarkan progress

## Tech Stack

- **Frontend**: React 18 + TypeScript + Vite
- **Backend**: Express.js + Node.js
- **Database**: MySQL (via Laragon)
- **AI**: Ollama (local, no subscription needed)
- **Styling**: TailwindCSS
- **ORM**: Sequelize

## Prerequisites

- Node.js 18+
- Laragon (MySQL running)
- Ollama installed ([https://ollama.ai](https://ollama.ai))
- Ollama model pulled (e.g., `ollama pull mistral`)

## Quick Start

### 1. Clone Repository
```bash
git clone https://github.com/egapratamaa/habits-tracker.git
cd habits-tracker
```

### 2. Setup Backend
```bash
cd backend
npm install
cp .env.example .env
# Configure .env with MySQL credentials from Laragon
npm run dev
```

### 3. Setup Frontend
```bash
cd frontend
npm install
npm run dev
# Access at http://localhost:5173
```

### 4. Start Ollama (separate terminal)
```bash
ollama serve
# In another terminal: ollama pull mistral
```

## Database Setup
Database setup akan dijelaskan setelah semua file selesai dibuat.

## Ollama Setup
Ollama setup akan dijelaskan setelah semua file selesai dibuat.

## Project Structure
```
habits-tracker/
├── backend/
│   ├── src/
│   │   ├── config/
│   │   ├── controllers/
│   │   ├── models/
│   │   ├── routes/
│   │   ├── services/
│   │   ├── middleware/
│   │   └── server.ts
│   ├── .env.example
│   ├── package.json
│   └── tsconfig.json
├── frontend/
│   ├── src/
│   │   ├── components/
│   │   ├── pages/
│   │   ├── services/
│   │   ├── types/
│   │   └── App.tsx
│   ├── package.json
│   ├── tsconfig.json
│   └── vite.config.ts
└── README.md
```
