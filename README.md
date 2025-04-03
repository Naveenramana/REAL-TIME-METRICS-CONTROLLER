# System Metrics Monitoring Dashboard

A comprehensive system monitoring solution with real-time metrics visualization, alerting, and role-based access control.

## Key Features

- **Real-time Monitoring**: Track CPU, memory, and disk usage with live-updating charts
- **Smart Alerting**: Configurable thresholds trigger visual alarms
- **Role-Based Access**:
  - Admin: Full system control and configuration
  - Operator: Alarm acknowledgment and monitoring
- **Secure Authentication**: SHA-256 hashing for all stored credentials
- **Responsive Design**: Optimized login page and dashboard for all device sizes
- **Data Persistence**: SQLite database storage with CSV export capability
- **Historical Analysis**: View metrics trends over custom time periods

## Technology Stack

**Backend**:
- Java 17
- SparkJava (HTTP server)
- SQLite (Database)
- SHA-256 (Secure password hashing)

**Frontend**:
- React.js
- Chart.js (Data visualization)
- Axios (API communication)
- Bootstrap 5 (Responsive layout)

## Security Features

- All passwords securely hashed using SHA-256 algorithm before storage
- Role-based API endpoint protection
- CORS configuration for frontend-backend communication
- CSRF protection implementation


## Responsive Enhancements

- Mobile-optimized login form with adaptive layout
- Dynamic chart resizing for different screen sizes
- Touch-friendly interface elements
- Responsive data tables with horizontal scrolling on small devices
- Media queries for optimal viewing on:
  - Desktop (≥992px)
  - Tablet (≥768px)
  - Mobile (<768px)

## Installation

1. **Backend and Frontend Setup**:
```bash
cd backend
mvn clean compile
mvn clean install
java -jar target/metrics-api-project2-1.0.0.jar
cd frontend
npm run dev

