# नारीFirst — NaariFirst

> *A curated space for ambitious women to connect, grow & celebrate each other.*

![NaariFirst](https://img.shields.io/badge/NaariFirst-Women%20Community-black?style=for-the-badge&labelColor=black&color=C9974A)
![React](https://img.shields.io/badge/React-Frontend-black?style=for-the-badge&logo=react&labelColor=black&color=C9974A)
![C#](https://img.shields.io/badge/C%23-Backend-black?style=for-the-badge&logo=csharp&labelColor=black&color=C9974A)
![ASP.NET Core](https://img.shields.io/badge/ASP.NET_Core-API-black?style=for-the-badge&logo=dotnet&labelColor=black&color=C9974A)
![SQLite](https://img.shields.io/badge/SQLite-Database-black?style=for-the-badge&logo=sqlite&labelColor=black&color=C9974A)

---

## ✦ About

**NaariFirst** is a full-stack women's community platform built for connection, events, and empowerment. Women can request invites, RSVP to exclusive events, and manage their profiles — all within a curated, invite-only space.

Inspired by [@entreprenaari.com](https://instagram.com/entreprenaari.com)

---

## ✦ Features

| Feature | Description |
|---|---|
| 🔐 Auth | JWT-based register & login |
| 🌸 Events | Browse upcoming & past community events |
| 📋 RSVP | Book spots — auto approve or waitlist |
| 👤 Profile | Edit bio, manage notifications, view joined events |
| 🛡️ Admin | Create events, manage RSVPs, view all users |
| 📱 Mobile UI | Designed as a mobile-first app experience |

---

## ✦ Tech Stack

### Frontend
- **React** (JSX)
- **CSS Variables** — Black & Gold design system
- **Playfair Display** + **DM Sans** typography
- Deployed on **Vercel**

### Backend
- **C# ASP.NET Core 8** Web API
- **Entity Framework Core** — SQLite (dev) / PostgreSQL (prod)
- **JWT Authentication** — BCrypt password hashing
- **Swagger UI** — API documentation
- Deployed on **Railway**

---

## ✦ Project Structure

```
NaariFirst/
│
├── frontend/                  # React app
│   ├── src/
│   │   ├── App.jsx            # Main app + all pages
│   │   └── index.js
│   └── package.json
│
└── backend/                   # ASP.NET Core API
    ├── Program.cs             # App startup & config
    ├── Models/
    │   └── Models.cs          # User, Event, Rsvp entities
    ├── DTOs/
    │   └── DTOs.cs            # Request & response shapes
    ├── Controllers/
    │   ├── AuthController.cs
    │   ├── EventsController.cs
    │   ├── RsvpsController.cs
    │   └── UsersController.cs
    └── Services/
        └── Services.cs        # Business logic
```

---

## ✦ API Endpoints

### Auth
```
POST   /api/auth/register       Register new user
POST   /api/auth/login          Login & get JWT token
```

### Events
```
GET    /api/events              Get all upcoming events
GET    /api/events/{id}         Get single event
POST   /api/events              Create event (Admin)
PATCH  /api/events/{id}         Update event (Admin)
DELETE /api/events/{id}         Delete event (Admin)
GET    /api/events/{id}/rsvps   Get event guest list (Admin)
```

### RSVPs
```
POST   /api/rsvps               Submit RSVP
DELETE /api/rsvps/{id}          Cancel RSVP
PATCH  /api/rsvps/{id}/status   Approve/reject RSVP (Admin)
```

### Users
```
GET    /api/users/me            Get my profile
PATCH  /api/users/me            Update my profile
PATCH  /api/users/me/password   Change password
GET    /api/users/me/rsvps      Get my events
DELETE /api/users/me            Delete account
GET    /api/users               Get all users (Admin)
```

---

## ✦ Getting Started

### Prerequisites
- [Visual Studio Community 2022](https://visualstudio.microsoft.com/)
- [.NET 8 SDK](https://dotnet.microsoft.com/download)
- [Node.js LTS](https://nodejs.org/)

---

### Run the Backend

**1. Open Visual Studio → New Project → ASP.NET Core Web API**

**2. Install NuGet packages:**
```bash
dotnet add package Microsoft.EntityFrameworkCore.Sqlite
dotnet add package Microsoft.AspNetCore.Authentication.JwtBearer
dotnet add package BCrypt.Net-Next
dotnet add package Swashbuckle.AspNetCore
```

**3. Add the files into the correct folders**

**4. Press ▶ Run**

**5. Visit Swagger UI:**
```
https://localhost:5000/swagger
```

---

### Run the Frontend

```bash
npx create-react-app naarifirst
cd naarifirst
npm start
```

Replace `src/App.js` with the provided `NaariFirst.jsx` code.

---

### Connect Frontend to Backend

In your React app, add:
```javascript
const API = "https://localhost:5000/api";

const login = async (email, password) => {
  const res = await fetch(`${API}/auth/login`, {
    method: "POST",
    headers: { "Content-Type": "application/json" },
    body: JSON.stringify({ email, password })
  });
  const data = await res.json();
  localStorage.setItem("token", data.token);
};
```

---

## ✦ Deployment

### Backend → Railway
1. Push backend to GitHub
2. Go to [railway.app](https://railway.app)
3. New Project → Deploy from GitHub
4. Select your repo → Railway auto-deploys ✅

### Frontend → Vercel
1. Push frontend to GitHub
2. Go to [vercel.com](https://vercel.com)
3. Import project → Vercel auto-deploys ✅
4. Update API URL to your Railway domain

---

## ✦ Environment Variables

Create an `appsettings.json` in your backend:
```json
{
  "Jwt": {
    "Key": "your_super_secret_key_here_minimum_32_chars"
  },
  "ConnectionStrings": {
    "Default": "Data Source=naarifirst.db"
  }
}
```

---

## ✦ Roadmap

- [x] User authentication (JWT)
- [x] Event listings
- [x] RSVP booking system
- [x] Profile management
- [x] Admin controls
- [ ] Email notifications (SendGrid)
- [ ] Image uploads (Cloudinary)
- [ ] Payment integration (Stripe)
- [ ] React Native mobile app
- [ ] Admin analytics dashboard

---

## ✦ Built By

Built with 🖤 as a full-stack portfolio project.

**Stack:** React · C# · ASP.NET Core · Entity Framework · JWT · SQLite

---

## ✦ License

MIT License — free to use and build upon.

---

*"We exist to lift women up — through community, opportunity, and radical sisterhood."*
*— The NaariFirst Mission*
