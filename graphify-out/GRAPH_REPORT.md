# Graph Report - .  (2026-07-22)

## Corpus Check
- Large corpus: 629 files · ~507,865 words. Semantic extraction will be expensive (many Claude tokens). Consider running on a subfolder.

## Summary
- 160 nodes · 46 edges · 117 communities (8 shown, 109 thin omitted)
- Extraction: 74% EXTRACTED · 26% INFERRED · 0% AMBIGUOUS · INFERRED: 12 edges (avg confidence: 0.88)
- Token cost: 191,645 input · 5,789 output

## Community Hubs (Navigation)
- Admissions & Lead Modules
- CRM Roles & Workflows
- Database Tables Schema
- Core App & Authentication
- Permissions System
- Database & Prisma Layer
- CRM User Guides
- Branding & Role Guides
- Erode Branch
- Salem Branch
- Tirupur Branch
- Notification & Automation
- Trainer & Timetable
- Attendance Tracking Module
- Branch Data Model
- Coimbatore Branch
- CEO
- Course Management Module
- Fortune Campus Institute Management System
- runAutoMigrations
- backfillConductorTrainers
- backfillNotificationLinks
- backfillPenaltyAmounts
- runDailyBreakCompliance
- startDailyBreakCompliance
- startDailyLeadReassignment
- sendFeeDueReminder
- startFeeDueReminder
- startMidnightTaskChecker
- checkRecurringBillReminders
- startRecurringBillReminder
- Capability
- CapabilityMeta
- defaultCapabilities
- effectiveCapabilities
- normalizeExtras
- UserForCapabilityCheck
- userHas
- AuthRequest
- AccountabilityThresholds
- AttendanceAuditService
- AuditLogInput
- enrollStudentInBatch
- findOrCreateBatchForEnrollment
- notifyTrainerOfBatchAssignment
- TrainerPlacement
- eachLeaveDay
- reassignTelecallerLeads
- restoreTelecallerLeads
- LmsProgressService
- AutomationWorker
- NotificationService
- recordCompOffIfApplicable
- recordEarlyCheckoutPenalty
- recordLateCheckinPenalty
- runOverdueTaskCheck
- detectMissedSlots
- fmtSlotLabel
- LeaveOverlay
- clearTemplateCache
- getTemplate
- render
- renderTemplate
- saveTemplates
- TemplateKey
- fmtMinutes
- getCheckoutHoursStatus
- getLoggedMinutes
- getRequiredMinutes
- haversineDistance
- generateSessionCode
- ApiResponse
- enforceAppVersion
- BreakCard
- BadgeProps
- ButtonProps
- CalendarProps
- ChartConfig
- TextareaProps
- Toaster
- useIsMobile
- ActiveBreak
- formatRemaining
- useBreakStatus
- AccountabilityThresholds
- AccountabilityThresholdsPayload
- AttendanceAuditLog
- ExpenseRow
- ExpensesListResponse
- ExpensesSummaryResponse
- FeedbackRating
- FeedbackSummary
- WatchlistData
- WatchlistModule
- WatchlistSeverity
- WatchlistSummary
- WatchlistViolation
- Capability
- userHas
- userHasAll
- userHasAny
- cn
- Fortune Innovatives Favicon
- The Chennai Silks Logo
- Code Pixel Logo
- Grasp Clothings Logo
- Heini Logo
- Nittany Logo
- Companies Table
- Incentives Table
- Leads Table
- Notifications Table
- Placements Table
- Portfolios Table
- WhatsApp Logs Table
- Company Controller
- Placement Controller

## God Nodes (most connected - your core abstractions)
1. `Students Table` - 4 edges
2. `Batches Table` - 4 edges
3. `Flexible Permissions Implementation Spec` - 4 edges
4. `CEO User Guide` - 4 edges
5. `Fortune Campus Backend API` - 3 edges
6. `Lead Management Module` - 3 edges
7. `Admission Management Module` - 3 edges
8. `Prisma Schema` - 3 edges
9. `Fortune Campus - User Guides Index` - 3 edges
10. `Student` - 3 edges

## Surprising Connections (you probably didn't know these)
- `Test Students Script` --references--> `Prisma Schema`  [INFERRED]
  test-students.ts → prisma/schema.prisma
- `Fortune Innovatives Logo (Black Background)` --conceptually_related_to--> `CEO User Guide`  [INFERRED]
  frontend/public/logo.jpg → user-guides/1-CEO-Guide.html
- `Fortune Innovatives Logo (White Background)` --conceptually_related_to--> `CEO User Guide`  [INFERRED]
  frontend/src/assets/logo.jpg → user-guides/1-CEO-Guide.html
- `Equal Lead Distribution (FR-15)` --implements--> `Lead Management Module`  [EXTRACTED]
  Phase2_Report.html → fortune-campus/backend/src/modules/leads/lead.controller.ts
- `Student UPI Self-Pay (FR-08)` --shares_data_with--> `Admission Management Module`  [EXTRACTED]
  Phase2_Report.html → fortune-campus/backend/src/modules/admissions/admission.controller.ts

## Import Cycles
- None detected.

## Hyperedges (group relationships)
- **Core Academic Workflow** — course_module, trainer_module, student_module, attendance_module, timetable_module [EXTRACTED 0.95]
- **Lead-to-Student Conversion Pipeline** — lead_module, admission_module, student_module, equal_lead_distribution [EXTRACTED 1.00]
- **System Security & Auth Framework** — auth_module, setup_module, user_model, branch_model [EXTRACTED 0.90]
- **Core Academic Entities** — public_students, public_batches, public_courses, public_trainers, public_attendances [INFERRED 0.85]
- **CRM and Admission Flow** — public_leads, public_admissions, public_students [INFERRED 0.80]
- **Notification Automation Flow** — src_modules_notifications_automation_worker, notification_service [EXTRACTED 0.90]
- **Flexible Permission System** — docs_flexible_permissions_spec, backend_src_lib_permissions, backend_src_middlewares_permission_middleware, prisma_user_model, prisma_capability_grant_log_model [EXTRACTED 1.00]
- **User Role Documentation** — user_guides_1_ceo_guide, user_guides_2_channel_partner_guide, user_guides_3_trainer_guide [EXTRACTED 1.00]
- **Fortune Campus User Roles** — ceo_role, channel_partner_role, trainer_role, student_role, telecaller_role [EXTRACTED 1.00]
- **Lead to Admission Workflow** — telecaller_role, channel_partner_role, trainer_role [INFERRED 0.85]

## Communities (117 total, 109 thin omitted)

### Community 0 - "Admissions & Lead Modules"
Cohesion: 0.29
Nodes (7): Admission Management Module, Equal Lead Distribution (FR-15), Evolution API, WhatsApp Integration Service, Lead Management Module, Student Management Module, Student UPI Self-Pay (FR-08)

### Community 1 - "CRM Roles & Workflows"
Cohesion: 0.29
Nodes (7): Channel Partner, Lead Pipeline (Kanban), Portfolio Submission System, QR Attendance System, Student, Telecaller, Trainer

### Community 2 - "Database Tables Schema"
Cohesion: 0.33
Nodes (7): Admissions Table, Attendances Table, Batches Table, Courses Table, Students Table, Trainers Table, Users Table

### Community 3 - "Core App & Authentication"
Cohesion: 0.40
Nodes (5): Authentication Module, Fortune Campus Backend API, Fortune Campus Frontend, First-Time Setup Module, User Data Model

### Community 4 - "Permissions System"
Cohesion: 0.50
Nodes (5): Permissions Library, Permission Middleware, Flexible Permissions Implementation Spec, Capability Grant Log Model, User Model

### Community 5 - "Database & Prisma Layer"
Cohesion: 0.40
Nodes (5): Supabase PostgreSQL Database, Prisma Schema, Prisma Seed Script, Public Users Table, Test Students Script

### Community 6 - "CRM User Guides"
Cohesion: 0.50
Nodes (5): Fortune Campus CRM, Sirah Digital, Student User Guide, Telecaller User Guide, Fortune Campus - User Guides Index

### Community 7 - "Branding & Role Guides"
Cohesion: 0.40
Nodes (5): Fortune Innovatives Logo (Black Background), Fortune Innovatives Logo (White Background), CEO User Guide, Channel Partner User Guide, Trainer User Guide

## Knowledge Gaps
- **139 isolated node(s):** `runAutoMigrations`, `backfillConductorTrainers`, `backfillNotificationLinks`, `backfillPenaltyAmounts`, `runDailyBreakCompliance` (+134 more)
  These have ≤1 connection - possible missing edges or undocumented components.
- **109 thin communities (<3 nodes) omitted from report** — run `graphify query` to explore isolated nodes.

## Suggested Questions
_Questions this graph is uniquely positioned to answer:_

- **Are the 4 inferred relationships involving `CEO User Guide` (e.g. with `Fortune Innovatives Logo (Black Background)` and `Fortune Innovatives Logo (White Background)`) actually correct?**
  _`CEO User Guide` has 4 INFERRED edges - model-reasoned connections that need verification._
- **What connects `runAutoMigrations`, `backfillConductorTrainers`, `backfillNotificationLinks` to the rest of the system?**
  _139 weakly-connected nodes found - possible documentation gaps or missing edges._