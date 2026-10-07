# Lab 0 — Prerequisites and Environment Check

<div class="lab-badge lab-badge-blue">Lab 0</div>
<div class="lab-badge lab-badge-green">Prerequisites</div>
<div class="lab-badge lab-badge-teal">10 min</div>

---

## Lab Objectives

By the end of this lab you will be able to:

- [x] Verify access to the IBM Concert platform
- [x] Navigate to the demo environment URL
- [x] Authenticate successfully on the platform
- [x] Confirm the main view loads correctly

---

## 1. Environment Access

### 1.1 Platform URL

Open your browser (Chrome or Firefox) and navigate to the following URL:

```
https://concert.tec.spgi.ibm.com:12443/platform/views/AtG0fxALg1It-Cwf6nsel#
```

!!! warning "SSL Certificate"
    The demo environment uses a self-signed certificate. When the browser shows a security warning:
    
    1. Click **"Advanced"** (Chrome) or **"Advanced Options"** (Firefox)
    2. Select **"Proceed to [URL] (unsafe)"** or **"Accept the risk and continue"**
    
    This behaviour is normal in lab environments.

---

### 1.2 Login Screen

When you access the URL, you will see the IBM Concert login screen:

<div class="screenshot-container" markdown="1">

![IBM Concert login screen](../assets/images/lab0-login.png)

<div class="screenshot-caption" markdown="1">
📸 Figure 1 — IBM Concert authentication screen
</div>
</div>

!!! tip "Reference image"
    The IBM Concert login screen shows the IBM logo at the top, 
    with a centred form containing the **Username** and **Password** fields, 
    and a blue **"Log in"** button.

**Enter the following credentials:**

| Field | Value |
|-------|-------|
| **Username** | `ibmconcert` |
| **Password** | `Passw0rd!` |

1. Type `ibmconcert` in the **Username** field
2. Type `Passw0rd!` in the **Password** field
3. Click the **"Log in"** button or press `Enter`

---

### 1.3 First Access — Main Dashboard

After authenticating successfully, you will be taken to the **IBM Concert main dashboard**:

<div class="screenshot-container" markdown="1">

![IBM Concert main dashboard](../assets/images/lab0-dashboard.png)

<div class="screenshot-caption" markdown="1">
📸 Figure 2 — IBM Concert main view after login
</div>
</div>

!!! success "Successful access"
    If you can see the dashboard with the module cards (**Protect**, **Observe**, **Resilience**, **Optimize**, **Workflows**), access was successful.

---

## 2. Getting Familiar with the Interface

### 2.1 Main Screen Structure

IBM Concert presents a unified interface with the following elements:

```
┌─────────────────────────────────────────────────────────┐
│  IBM Concert          🔔 Alerts    👤 ibmconcert   ⚙️  │
├──────────────────────────────────────────────────────────┤
│  Home | Resilience | Observe | Optimize | Protect | ...  │
├──────────────────────────────────────────────────────────┤
│                                                          │
│   ┌──────────┐  ┌──────────┐  ┌──────────┐             │
│   │ Protect  │  │ Observe  │  │Resilience│             │
│   │  CVEs    │  │  APM     │  │Incidents │             │
│   └──────────┘  └──────────┘  └──────────┘             │
│                                                          │
│   ┌──────────┐  ┌──────────┐                            │
│   │ Optimize │  │Workflows │                            │
│   │Resources │  │  Automat │                            │
│   └──────────┘  └──────────┘                            │
└──────────────────────────────────────────────────────────┘
```

### 2.2 Main Navigation Elements

| Element | Description |
|---------|-------------|
| **Top navigation bar** | Main modules: Home, Resilience, Observe, Optimize, Protect, Workflows, Data Apps |
| **Top bar icons (right)** | Notifications, AI Assistant, user profile and settings |
| **Central area** | Active view of the selected module |
| **Summary panel** | Global KPIs and metrics for the environment |

---

## 3. Environment Verification

Confirm the following elements are visible on the dashboard:

=== "Verification Checklist"

    - [ ] The navigation bar shows all modules
    - [ ] The header shows the user `ibmconcert`
    - [ ] At least one application appears in the inventory
    - [ ] The Protect and Observe modules show sample data
    - [ ] There are no error messages on the main screen

=== "Troubleshooting"

    **Problem**: Page does not load / Connection error
    
    → Verify you are connected to the lab network
    
    → Check that the URL starts with `https://`
    
    **Problem**: Incorrect credentials
    
    → Make sure the password is exactly `Passw0rd!` (capital P and the `0` is zero)
    
    **Problem**: Blank screen after login
    
    → Reload the page with `Ctrl+F5` (Windows) or `Cmd+Shift+R` (Mac)

---

## Summary

!!! success "Lab 0 completed ✅"
    You have successfully verified:
    
    - ✅ Access to the IBM Concert URL
    - ✅ Authentication with the workshop credentials
    - ✅ Main dashboard loading
    - ✅ Concert interface structure
    
    **Next step**: [Lab 1 — Introduction to Concert →](../lab1/index.md)
