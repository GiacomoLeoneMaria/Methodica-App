# Methodica - Personal Productivity App

**Methodica** is a complete mobile application for personal productivity management, designed to help users organize events, manage tasks, and balance life's priorities through an intuitive and powerful interface.

## Key Features

The application is built around several integrated modules to offer a comprehensive, 360-degree time management experience.

### **Event & Calendar Management**
- **Full CRUD for Events**: Create, edit, view, and delete events.
- **Multi-View Calendar**: View events in daily (with an hourly timeline), weekly, and monthly modes.
- **All-Day Event Support**: Support for events that last the entire day.
- **Automatic Rescheduling**: Past, uncompleted events can be automatically rescheduled to the current day.
- **Customizable Reminders**: Set multiple notifications for each event (e.g., at the time of the event, 5 minutes before, 1 hour before, etc.).
- **Personalization**: Assign custom icons and colors to each event.

### **Task & Kanban Management**
- **Kanban Board**: Tasks are organized into columns (Backlog, In Progress, Review, Done) for visual workflow management.
- **Task Details**: Each task can have a description, priority (high, medium, low), deadline, icons, sub-tasks, and tags.
- **Advanced Filtering**: The Kanban view can be filtered by "Priority Area," showing only relevant tasks.
- **Daily Notifications**: Daily reminders (morning and evening) for active tasks (In Progress and Review).

### **Priority Square**
- **Life Area Balancing**: Users can define important areas of their life (e.g., Work, Health, Family) and assign a percentage of importance to each.
- **Treemap Visualization**: The areas are displayed as a dynamic square (treemap) that visually represents their "weight."
- **Task/Event Linking**: Tasks and events can be linked to a specific area, helping the user to dedicate time to the right things.

### **Dashboard (Home Screen)**
- **Daily Overview**: Shows a summary of the current day with the date, scheduled events, and active tasks.
- **Daily Progress**: A progress bar shows the percentage of events completed during the day.
- **Quick Access**: Buttons to quickly add new events or tasks.

### **Settings & Customization**
- **Dark/Light/Auto Theme**: The app supports multiple themes that can also automatically adapt to system settings.
- **Notification Management**: Globally enable or disable notifications from the app.
- **Data Management**: Functionality to delete all data, or just events/tasks, to start over.

### **Internationalization (i18n)**
- **Multi-language Support**: The interface is translated into multiple languages (Italian, English, French, German, Spanish) and automatically adapts to the device's language.
- **Date Localization**: Dates and times are formatted correctly based on the detected language.

## Frameworks and Libraries Used

The application was built using **React Native** with the **Expo** framework.

### **Core Framework**
- **React Native**: For cross-platform application development (iOS & Android).
- **Expo**: To simplify development, building, and access to native APIs.

### **Navigation**
- **React Navigation (`@react-navigation/native`, `@react-navigation/bottom-tabs`)**: For managing the tab-based navigation (Tab Navigator) between the main screens.

### **State Management**
- **React Context API**: For managing the application's global state (events, tasks, settings, theme) in a centralized and reactive way through `AppContext` and `ThemeContext`.

### **UI & Components**
- **React Native Core Components**: Base components for building the user interface.
- **`@expo/vector-icons`**: For a large library of customizable icons.
- **`react-native-gesture-handler`**: For managing complex gestures and touch interactions.
- **`react-native-safe-area-context`**: To correctly handle layouts on devices with notches and safe areas.
- **`react-native-calendars`**: Used for the monthly calendar view.
- **`@react-native-community/slider`**: For the slider component used in defining area percentages.
- **`@react-native-community/datetimepicker`**: For native date and time pickers.
- **`expo-linear-gradient`**: To create color gradients in some UI components.

### **Local Storage**
- **`@react-native-async-storage/async-storage`**: For persisting user data (events, tasks, areas, settings) directly on the device.

### **Native APIs & Services**
- **`expo-notifications`**: For complete management of local notifications (requesting permissions, scheduling, cancellation).
- **`expo-splash-screen`**: For programmatic control of the splash screen.
- **`expo-localization`**: To detect the device's language and regional settings.

### **Utilities**
- **`date-fns`**: A modern and powerful library for manipulating and formatting dates and times.
- **`i18next` & `react-i18next`**: For implementing internationalization.
