# 💪 FitLog — Workout Library

FitLog is a modern, responsive workout library built with **Next.js** and **Tailwind CSS**. It allows users to browse workouts, view detailed exercise information, create a daily workout plan, and save workouts for later.

🔗 **Live Demo:** https://fit-log-roan-three.vercel.app/

---

## 📌 Project Overview

FitLog is a dark-themed workout companion designed to make workout planning simple and organized.

Users can:

* Browse a workout library
* View detailed information about individual workouts
* Add workouts to today's plan
* Save workouts for later
* Track planned exercises, duration, and calories
* Mark planned workouts as completed
* Remove workouts from their plan
* Sort workouts by duration, calories, or rating
* Access the application on mobile, tablet, and desktop

The workout information is loaded dynamically from the FitLog API.

---

## ✨ Features

### 🏋️ Workout Library

* Displays workouts fetched from the FitLog API
* Responsive workout-card grid
* Workout images and category badges
* Equipment information
* Duration, calories, and rating statistics

### 📋 Today's Plan

* Add workouts to today's workout plan
* Maximum of five workouts can be added
* Live exercise, duration, and calorie metrics
* Remove workouts from the plan
* Mark workouts as completed
* View workout details directly from the plan

### 🔖 Saved Workouts

* Save workouts for later
* Separate Saved tab on the My Plan page
* Live saved-workout counter in the navbar

### 🔍 Workout Details

* Dynamic workout detail pages
* Large workout image
* Workout description
* Category tags
* Equipment and difficulty
* Sets and reps
* Duration and calories
* Rating
* Step-by-step instructions

### 🔄 Sorting

Workouts can be sorted by:

* Duration
* Calories
* Rating

### 🔔 Toast Notifications

Interactive actions provide feedback through toast notifications, including:

* Workout added to plan
* Workout saved
* Workout marked as done
* Workout removed

### 📱 Responsive Design

The interface is designed to work across:

* 📱 Mobile
* 💻 Tablet
* 🖥️ Desktop

### ⚡ Loading & Error States

* Loading animation while workout data is fetched
* Custom 404 page for invalid routes
* Dynamic routes for individual workouts

---

## 🛠️ Technologies Used

| Technology             | Purpose                                      |
| ---------------------- | -------------------------------------------- |
| **Next.js**            | React framework and application architecture |
| **TypeScript**         | Type-safe development                        |
| **React**              | UI development                               |
| **Next.js App Router** | Page and dynamic route handling              |
| **Tailwind CSS**       | Styling and responsive design                |
| **Lucide React**       | UI icons                                     |
| **React Hot Toast**    | Toast notifications                          |
| **FitLog API**         | Workout data source                          |
| **Vercel**             | Deployment                                   |

---

## 🔗 API

### Get All Workouts

```text
https://api.abcz.workers.dev/api/fitlog
```

### Get Single Workout

```text
https://api.abcz.workers.dev/api/fitlog/:id
```

### Alternative API

```text
https://api.api-store.workers.dev/api/fitlog
```

Single workout:

```text
https://api.api-store.workers.dev/api/fitlog/:id
```

---

## 📂 Main Routes

| Route           | Description                     |
| --------------- | ------------------------------- |
| `/`             | Home page and workout library   |
| `/my-plan`      | Today's Plan and Saved workouts |
| `/workout/[id]` | Individual workout details      |
| `404`           | Unknown or invalid routes       |

---

## 🎯 Core User Flow

```text
Home
  ↓
Browse Workouts
  ↓
Select Workout
  ↓
Workout Details
  ↓
┌──────────────────────┐
│ Add to Today's Plan  │
│ Save for Later       │
└──────────────────────┘
          ↓
       My Plan
          ↓
 View / Complete / Remove
```

---

## 📊 Plan Metrics

The **My Plan** page provides a live summary of:

* **Exercises** — number of planned workouts
* **Minutes** — total workout duration
* **Calories** — total estimated calories

These values update when workouts are added or removed.

---

## 🎨 Design

FitLog uses a dark, bold fitness-focused visual style with:

* Strong display typography
* High-contrast UI
* Accent-colored buttons and badges
* Workout imagery
* Responsive layouts
* Clear card-based information hierarchy

---

## 🚀 Getting Started

### 1. Clone the repository

```bash
git clone YOUR_GITHUB_REPOSITORY_URL
```

### 2. Navigate to the project

```bash
cd fit-log
```

### 3. Install dependencies

```bash
npm install
```

### 4. Start the development server

```bash
npm run dev
```

Open:

```text
http://localhost:3000
```

---

## 🏗️ Build for Production

Run:

```bash
npm run build
```

Then start the production server:

```bash
npm start
```

---

## 🌐 Deployment

The project is deployed using **Vercel**.

### Live Website

https://fit-log-roan-three.vercel.app/

---

## 📱 Responsive Support

FitLog is optimized for different screen sizes.

### Mobile

* Responsive navigation
* Stacked hero section
* Single-column workout cards

### Tablet

* Flexible grid layout
