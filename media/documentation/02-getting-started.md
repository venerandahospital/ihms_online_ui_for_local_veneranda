# Getting Started

## Before you begin

You need:

- A supported web browser (Chrome, Edge, or Firefox recommended)
- Your **username** and **password** from your facility administrator
- Network access to the **application server** and **API server** (often on the same LAN)

If the app cannot reach the API, an administrator may need to configure the server connection on first launch.

## Signing in

1. Open the facility login URL (e.g. `/login` or `/login4` depending on deployment).
2. Enter username and password.
3. After successful login, you are directed to the **Overview** hub or your role’s default screen.

**Note:** Branding on the login page (logo, clinic name) may show the facility’s configured name or a default template.

## First-time server connection (IT)

If prompted for API settings:

- Default API path: `/health_care` on port **8080**
- Example local URL: `http://localhost:8080/health_care`
- The active server URL is stored in the browser for subsequent sessions

Administrators should confirm the correct host with your technical team before staff widespread use.

## Main navigation

### Overview sidebar

After login, most modules live under **`/overview`**:

- Collapsible sidebar groups: Dashboard, Clients, OPD, IPD, Lab, Radiology, Pharmacy, Inventory, Finance, HR, Reports, Administration, etc.
- Click a menu item to open that module in the main content area.
- Sidebar can run in **stacked** mode (sidebar shares space with content) or overlay mode — configured under **Business settings**.

### Top header

Available on many screens:

- **Queue** — view current clients in line; open a client visit from the queue
- **Department links** — quick jump to Lab, Scan, Dental, Client visit, etc. (based on your access)
- **Profile / account** — user details, logout
- **Cart / notifications** — where enabled for your role

### Client visit (clinical workspace)

Route: **`/client-visit`**

Usually opened from:

- Queue (client name or clipboard icon)
- Client list or search
- Department workflows that pass client context via session storage

Tabs on the visit screen:

| Tab | Typical use |
|-----|-------------|
| Client bio | Demographics and visit identifiers |
| Initial vitals | Temperature, BP, pulse, SpO₂, etc. |
| Consultations | Clinical notes and consultation forms |
| Procedures | Services and procedures for the visit |
| Treatment | Pharmacy prescribing and treatment chart |
| Finance | Charges and payments for this visit |
| Printouts | Reports and printable documents |

## Queue — quick reference

1. Open **Queue** from the header.
2. Tabs: **Current**, **Discharged today**, **Referred today**.
3. Click the **client name** or the **clipboard icon** to open their visit.
4. Use **Edit** (pencil) to change status, destination module, emergency flag, or notes.

The system loads the existing visit when possible; otherwise it starts from the client’s initial visit context.

## User profile

- Route: **`/user-profile`** or profile modal from Overview
- Update contact details and profile photo where permitted
- Change password when the facility allows self-service password updates

## Roles and what you see

Your **role** in session storage controls:

- Which Overview menu items appear
- Whether you can open dashboards
- Whether you can manage users and access control (typically **admin** or **MD**)

If a menu item is missing, ask an administrator to grant **page access** under **Access control**.

## Subscription

Some routes require an active **subscription**. If modules are blocked, the subscription may be expired — contact administration (**Overview → Subscription**).

## Logging out

Use **Logout** from the account menu. Always log out on shared computers.

## Tips for new users

- Use the queue to avoid searching for clients already in the building.
- Save work on each tab before switching tabs or navigating away.
- Long drug names in pharmacy dropdowns show full text on hover (tooltip).
- Use **Clear field** on prescribing rows before selecting a new item.

## Getting help

1. Read the module guide for your job: pharmacy, inventory, or client care.
2. Report issues to your facility superuser with: screen name, client ID (if applicable), time, and what you clicked.
3. IT staff should refer to **06-technical-guide.md**.

---

*Document 02 — Getting started — HMS documentation v1.0*
