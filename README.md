# ZenithHR | Enterprise Human Resource Management System (HRM)

A modern, comprehensive, enterprise-level **Human Resource Management System (HRM)** with dedicated **Admin Console**, **HR Operations Panel**, **Department Manager Portal**, and **Employee Self-Service**.

Designed with a premium corporate SaaS aesthetic:
- **Dark navy blue sidebar** (`#0A1128` / `#0F172A`)
- **Primary corporate blue** (`#1765E8`)
- **Secondary accents** (Purple, Emerald, Amber, Rose)
- **Clean white and slate backgrounds** (`#F8FAFC`)
- **Rounded 2xl cards with subtle elevation shadows**
- **Lucide icons & interactive Recharts telemetry**

---

## 🌟 Architecture & Key Features

### 1. Interactive Role-Based Switching
Switch between **4 distinct corporate roles** live from the top navigation bar to experience role-specific permissions and dashboards:
- **Admin (Super Admin)**: Unrestricted system access, user provisioning, permissions matrix, security audit trail, corporate settings.
- **HR Manager (Director of People Operations)**: Employee records, onboarding wizard, attendance timesheets, leave review, payroll processing, salary slip generation, recruitment pipeline.
- **Department Manager (VP of Engineering)**: Team attendance tracking, department leave approvals, performance appraisal reviews.
- **Employee (Staff Member)**: Personal attendance punch clock, leave application, official salary slips, corporate noticeboard.

---

### 2. Full Suite of HRM Modules

1. **Enterprise Dashboard**:
   - Welcome banner with corporate building motif and real-time clock.
   - Key statistics cards: Total Workforce, Present Today, On Leave, Open Vacancies.
   - Interactive Recharts analytics: 6-month Headcount Growth Area Chart, Department Distribution Donut, Weekly Attendance dynamics.
   - Pending Approvals quick-review card with 1-click Approve/Reject.
   - Recent Activities audit stream & Upcoming Events calendar.

2. **Employee Management**:
   - Grid and Data Table views with instant toggle.
   - Live search by Name, Employee ID (`EMP-XXXX`), Email, or Title.
   - Multi-parameter filtering by Department and Employment Status.
   - **Register Employee Modal**: Full legal profile, contact info, emergency contact, compensation tier, and bank routing details.
   - **Personnel Record File Modal**: Detailed overview, salary breakdown, leave entitlement balance, and performance scores.
   - One-click CSV Export.

3. **Departments & Designations**:
   - Department cards with annual budget allocation, headcount, and Department Head details.
   - Designations matrix table with seniority levels (Executive, Lead, Senior, Mid) and salary bands.
   - Add Department and Add Designation modals.

4. **Attendance & Timesheets**:
   - Real-time digital punch clock with live seconds counter.
   - Instant "Clock In / Clock Out" toggle with recorded timestamp.
   - Summary counters: Present, Late arrivals (with grace period enforcement), Half-day, On Leave, Absent.
   - Shift matrix calendar grid.
   - Timesheet records table with work hours and overtime calculation.

5. **Leave Management**:
   - Balance tracking for Annual Leave (20d), Sick Leave (12d), Casual Leave (10d), and Emergency Leave (5d).
   - "Apply for Leave" modal with auto duration calculator and reason.
   - Manager approval workflow with reviewer notes and audit logging.

6. **Payroll & Official Salary Slip Generator**:
   - Summary statistics: Net Disbursed, Statutory Tax Withheld, Benefit Deductions.
   - Salary processing modal: computes Basic, HRA, Conveyance, Medical, Bonuses minus PF and Federal Tax.
   - **Printable & Downloadable Corporate Payslip**:
     - Official company letterhead and registration identifiers.
     - Earnings vs. Deductions comparison table.
     - Net pay highlight.
     - Authorized HR signatory signature line and official company seal.
     - Direct browser print/PDF download button.

7. **Recruitment Pipeline & Hiring Funnel**:
   - Open vacancies list with applicant counter, experience requirements, and salary range.
   - **Interactive Kanban Board**: `Applied` → `Screening` → `Technical Interview` → `HR Interview` → `Offered` → `Hired`.
   - Candidate profile modal with resume preview, interview ratings, notes, and 1-click stage advancement.

8. **Performance Appraisals & KPIs**:
   - 360-degree review evaluations with 5-star ratings.
   - Target goals attainment percentage tracking.
   - Formal evaluation cards with key strengths and areas for development.
   - "Conduct Appraisal" modal.

9. **Announcements & Corporate Agenda**:
   - Noticeboard with priority badges (High, Medium, Normal) and target audience filters.
   - Corporate calendar events & employee milestone celebrations.

10. **Reports & Executive Intelligence**:
    - Workforce Headcount & Diversity trends.
    - Departmental compensation expenditure breakdown.
    - Attendance compliance and recruitment funnel velocity.
    - CSV Export and Print options.

---

### 3. Dedicated Admin Panel

- **User Management**: Provision system credentials, assign system roles, and monitor active sessions.
- **Roles & Permissions Matrix**: Granular RBAC matrix with module-level privilege checkboxes for Admin, HR Manager, Department Manager, and Employee.
- **System Activity Logs**: Complete security audit trail tracking all actions with IP address, timestamp, actor, and severity flag (`info`, `warning`, `critical`).
- **Corporate System Settings**: Legal entity configuration, Federal Tax ID, working hours, grace period, and statutory leave policies.

---

## 🚀 Running the Project

### Prerequisites
- Node.js (v18+)
- npm

### 1. Start Backend API Server
```bash
cd server
npm install
npm start
```
*The Express REST API runs on port `5000` (`http://localhost:5000/api`).*

### 2. Start Frontend Application
```bash
cd client
npm install
npm run dev
```
*The Vite React frontend runs on port `3000` (`http://localhost:3000`).*
