## 📌 About The Project

**FitLog** is a dark-themed workout library designed to help users discover exercises, view detailed workout information, create a daily workout plan, and save workouts for later.

The application provides a clean and responsive interface for browsing workouts and managing a personalized workout routine.

---

## 🚀 Live Demo

🔗 **Live Website:**


---

## ✨ Features

### 🏋️ Workout Library

* Displays workout exercises fetched from an external API.
* Responsive workout card grid.
* Workout images and illustrations.
* Category tags.
* Equipment information.
* Duration, calories, and rating statistics.
* Sort workouts by:

  * Duration
  * Calories
  * Rating

### 📖 Workout Details

* Dedicated detail page for every workout.
* Large workout image.
* Workout description.
* Category tags.
* Key workout specifications.
* Equipment and difficulty information.
* Sets and reps.
* Duration and calories.
* Rating.
* Step-by-step workout instructions.

### 📋 Today's Plan

* Add workouts to today's workout plan.
* Maximum of **5 lifts** per day.
* Live exercise count.
* Total workout duration.
* Total calories.
* View workout details.
* Mark workouts as completed.
* Remove workouts from the plan.

### 🔖 Saved Workouts

* Save workouts for later.
* View saved workouts from the My Plan page.
* Remove saved workouts when no longer needed.

### 🔔 Toast Notifications

Users receive feedback when they:

* Add a workout to today's plan.
* Save a workout.
* Mark a workout as completed.
* Remove a workout.

### 📱 Responsive Design

The website is designed to work across:

* 📱 Mobile
* 📲 Tablet
* 💻 Desktop

The workout grid, navigation, hero section, cards, and detail page adapt to different screen sizes.

### 💾 Local Storage

Workout plan and saved workout data are persisted using `localStorage`, allowing the user's data to survive page reloads.

### ❌ 404 Page

A custom 404 page is included for invalid or unknown routes.

### ⏳ Loading States

Loading animations/states are displayed while workout data is being fetched from the API.

---

## 🛠️ Technologies Used

| Technology             | Purpose                            |
| ---------------------- | ---------------------------------- |
| **Next.js**            | Frontend framework                 |
| **React**              | Building UI components             |
| **Next.js App Router** | Page routing and navigation        |
| **Tailwind CSS**       | Styling and responsive design      |
| **JavaScript**         | Application logic                  |
| **REST API**           | Fetching workout data              |
| **localStorage**       | Persisting plan and saved workouts |
| **Vercel**             | Deployment                         |

---

## 🔌 API

FitLog uses workout data from the following API.

### All Workouts

```text
https://api.abcz.workers.dev/api/fitlog
```

### Single Workout

```text
https://api.abcz.workers.dev/api/fitlog/:id
```

### Alternative API

```text
https://api.api-store.workers.dev/api/fitlog
```

### Alternative Single Workout API

```text
https://api.api-store.workers.dev/api/fitlog/:id
```

---

## 📂 Main Pages

| Route           | Description                   |
| --------------- | ----------------------------- |
| `/`             | Workout Library / Home        |
| `/workout/[id]` | Workout Details               |
| `/my-plan`      | Today's Plan & Saved Workouts |
| `/*`            | Custom 404 Page               |

---

## 🧭 Navigation

The main navigation contains:

* **Workout**
* **My Plan**

The navbar also contains two dynamic counters:

### 🟢 Plan

Shows the number of workouts currently added to **Today's Plan**.

### ⚪ Saved

Shows the number of workouts currently saved for later.

Both counters link to:

```text
/my-plan
```

---

## 🏠 Home Page

The homepage contains:

### Hero Section

**WORKOUT LIBRARY**

> TRAIN WITH INTENT. LOG EVERY SET.

FitLog is a dark, no-nonsense gym companion: pick a lift, lock it into today's plan, and watch the week's work add up.

The **BROWSE WORKOUTS** button smoothly takes the user to the workout library.

### Library

The library displays all workouts received from the API.

Each workout card contains:

* Workout image
* Category
* Workout name
* Equipment
* Duration
* Calories
* Rating

Clicking a workout card opens its detail page.

---

## 📄 Workout Details

Each workout has its own dynamic detail page.

The page contains:

* Workout image
* Workout title
* Description
* Category tags
* Equipment
* Difficulty
* Sets
* Reps
* Duration
* Calories
* Rating
* Instructions

### Actions

**Add to Today's Plan**

Adds the workout to the daily plan.

**Save for Later**

Adds the workout to the Saved section.

Both actions display a toast notification.

---

## 📋 My Plan

The My Plan page contains two tabs:

### Today's Plan

Displays workouts selected for today's routine.

The page includes three live metrics:

```text
Exercises
Minutes
Calories
```

The maximum number of workouts in today's plan is:

```text
5
```

### Saved

Displays workouts saved for later.

---

## ✅ Workout Actions

Each workout in Today's Plan provides:

### View Details

Opens the workout's detail page.

### Mark as Done

Marks the workout as completed and displays a confirmation toast.

### Remove

Removes the workout from Today's Plan and updates the metrics and navbar counter.

---

## 🔍 Sorting

The workout library includes a **Sort By** dropdown.

Available options:

```text
Duration
Calories
Rating
```

The selected option dynamically changes the order of the workout list.

---

## 🎨 Design

The project follows a modern dark gym aesthetic inspired by the provided Figma design.

### Design Characteristics

* Dark background
* High-contrast typography
* Bright accent color
* Bold display headings
* Workout-focused imagery
* Card-based layout
* Responsive navigation
* Minimal and clean interface

---

## 📱 Responsive Layout

FitLog supports different screen sizes.

### Desktop

* Full navigation
* Two-column hero
* 3-column workout grid
* Two-column workout details

### Tablet

* Responsive navigation
* 2-column workout grid
* Adapted spacing and typography

### Mobile

* Mobile-friendly navigation
* Stacked hero section
* Single-column workout cards
* Stacked workout details
* Touch-friendly buttons

---

## ⚡ Performance & User Experience

The application includes:

* API loading state
* Responsive UI
* Dynamic routing
* Toast notifications
* Persistent local data
* Empty states
* 404 page
* Interactive sorting
* Client-side state management

---