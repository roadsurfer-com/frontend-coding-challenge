# 🏕️ Frontend Coding Challenge

## 📜 Introduction

Imagine you own a rental business like **Roadsurfer**. You have a fleet of campervans and rental stations around the globe. Your customers pick up and return campervans at these stations. Your station personnel stay busy handing over and processing the returned vans.

To make your station staff’s lives easier, improve efficiency, and enhance transparency across all departments, you decide to create a **calendar-like dashboard web-app**. This app will display all planned pickups (booking start date) and returns (booking end date) of campervans at every station based on existing bookings.

For simplicity, let’s agree that a booking should always be returned to the same station where it was picked up.

## ⚙️ Setup

- **Framework**: Use a framework of your choice (Vue.js, Angular, React). If you're unsure, we recommend **Vue.js**.
- **Styling**: Feel free to add some styling (simple or sophisticated—it's up to you! 😉). If you're looking for a recommendation, we suggest **TailwindCSS**.
- **Hosting**: Host your code on **GitHub** and publish your web app on **GitHub Pages**. More info: [GitHub Pages](https://pages.github.com/).
- **UX Freedom**: The UX is yours to decide! If the explanation isn't clear enough, feel free to come up with your own interpretation of the task.
- **Mobile-First Design**: Keep the **mobile-first design** principle in mind when creating your web-app layout.

## 🛠️ To Do

### 1. **Create a Reusable Autocomplete Component** 🔍
- Create an **autocomplete** field that performs a search as the user types.
- The field should query a **remote API** to search based on the text entered.
- After the user selects a suggestion, the value should be selected, and an event should notify any interested handlers.

### 2. **Page Layout: Calendar View 📅**
- **Mobile and Desktop Views**: Implement a responsive grid with mobile and desktop views.
- **Week View**: Design a calendar-like week view with **7 tiles**, one for each weekday.
- **Pagination**: Implement pagination to switch between weeks.
- **Station Selector**: Use your **autocomplete component** to select a station (the station where the booking starts or ends). You can fetch the list of stations here: `https://605c94c36d85de00170da8b4.mockapi.io/stations`
- **Bookings Display**: On each day-tile, display bookings that start or end on that day at the selected station.
- **Booking Click**: When a booking is clicked, open a **new view** with the booking details (see below).

### 3. **Booking Detail View 📝**
- **Booking Information**: Retrieve booking details here: `https://605c94c36d85de00170da8b4.mockapi.io/stations/{station-id}/bookings/{booking-id}`
- Display the following booking details:
  - **Customer Name**
  - **Booking Start Date**
  - **Booking End Date**
  - **Booking Duration**
  - **Pickup-Return Station Name**
  - **Action**: Add a button to return to the calendar view.

### 4. **Optional Features 🎯**
- **Reschedule Booking**: Implement a feature allowing a station employee to reschedule the pickup or return date of a booking by drag-and-dropping it. (You can store the changes locally and emulate an API call—output the imaginary API call as text in the console).
- **State Management**: Optionally, introduce **state management** to your application. Choose the level of complexity and which parts of the app will use it.
- **Unit Tests**: Please write **unit tests** for your code! 
