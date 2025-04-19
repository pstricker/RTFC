# RealTimeForeCast (RTFC)

🏌️‍♂️ **RealTimeForeCast** is a real-time web application for tracking stroke play golf tournaments with handicap-adjusted scoring. Built in .NET with Blazor and SignalR, it enables tournament admins to manage players, enter scores, and see leaderboards update live.

---

## 🔧 Tech Stack

- **Frontend**: Blazor WebAssembly + MudBlazor
- **Backend**: ASP.NET Core Web API + SignalR
- **Database**: PostgreSQL (via Entity Framework Core)
- **Authentication**: ASP.NET Identity (admin only)
- **Hosting**: Azure App Service & Azure Database for PostgreSQL

---

## 🎯 Features

- Admin-driven score entry for stroke play tournaments
- Handicap-adjusted scoring (using slope, rating, hole handicaps)
- Real-time leaderboard via SignalR
- Support for multiple tees and custom handicap index per player
- Responsive UI suitable for tablets and desktops

---

## 🚀 Getting Started

### 1. Clone the Repository

```bash
git clone https://github.com/<your-username>/RTFC.git
cd RTFC
```

### 2. Set up the Database

Ensure PostgreSQL is running locally or in the cloud.

Create a `.env` or `appsettings.Development.json` with connection strings:
```json
"ConnectionStrings": {
  "DefaultConnection": "Host=localhost;Database=rtfc;Username=youruser;Password=yourpass"
}
```

Run migrations:

```bash
cd GolfTracker.Api
dotnet ef database update
```

### 3. Run the App

**Backend**:
```bash
cd GolfTracker.Api
dotnet run
```

**Frontend**:
```bash
cd GolfTracker.Web
dotnet run
```

Navigate to `https://localhost:5001` or whatever port Blazor is using.

---

## 📦 Project Structure

```text
RTFC/
├── GolfTracker.Api/         # ASP.NET Core Web API + SignalR
├── GolfTracker.Web/         # Blazor WebAssembly client
├── README.md
```

---

## 🧪 Testing

To run unit tests (coming soon):

```bash
dotnet test
```

---

## 🛠️ Roadmap

See the [RTFC MVP Plan GitHub Project](https://github.com/users/pstricker/projects/3) for feature progress and milestones.

---

## 🤝 Contributing

Contributions are welcome! Open issues or submit pull requests. For larger features, please start with a GitHub Discussion or Proposal.

---

## 📄 License

MIT License. See `LICENSE` file for details.

## 💼 Commercial Use

RealTimeForeCast (RTFC) is available under the MIT License for open-source use.

If you'd like to use RTFC in a commercial product or require extended support, please contact us to discuss a commercial license: [stricker.phil@gmail.com]

[![License: MIT](https://img.shields.io/badge/license-MIT-blue.svg)](LICENSE)
[![Commercial License](https://img.shields.io/badge/license-commercial-yellow.svg)](#-commercial-use)