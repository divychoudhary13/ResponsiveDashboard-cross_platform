# Responsive Dashboard App - Lab 4
## Student Information
- **Name:** Divy Choudhary
- **Student ID:** N01728746
- **Course:** CPAN 213
- **Lab:** Lab 4 - Responsive Layouts with Flexbox
- **Date:** September 23, 2025
## Project Description
This responsive dashboard application demonstrates advanced Flexbox layout techniques,
responsive design patterns, and platform-specific styling in React Native.
## Features Implemented
- Responsive grid system with breakpoint detection
- Dashboard widgets with statistics and trends
- Orientation-aware layouts
- Platform-specific styling (iOS/Android)
- Pull-to-refresh functionality
- Performance-optimized StyleSheets
## Technologies Used
- React Native 0.72+
- React Native Orientation Locker
- React Native Vector Icons
- Platform-specific APIs
## Installation
1. Clone the repository
2. Install dependencies: `npm install`
3. Install iOS pods (macOS only): `cd ios && pod install`
4. Run on Android: `npx react-native run-android`
5. Run on iOS: `npx react-native run-ios`

src/
├── components/
│ ├── DashboardHeader.js
│ ├── ResponsiveGrid.js
│ └── widgets/
│ ├── BaseWidget.js
│ └── StatisticWidget.js
├── screens/
│ └── DashboardScreen.js
├── styles/
│ └── theme.js
└── utils/
└── responsive.js


## Responsive Breakpoints
- Small phones: < 350px
- Medium phones: 350-400px
- Large phones: 400-500px
- Tablets: 500-768px
- Large tablets: > 768px


## Grid Columns by Device
- Small: 1 column
- Medium: 2 columns
- Tablet Portrait: 2 columns
- Tablet Landscape: 3-4 columns


## Performance Notes
- All animations run at 60fps
- StyleSheet.create used for all styles
- Memoization applied where necessary
- Native driver enabled for animations


## Screenshots
See `/screenshots` folder for app images on different devices.


## Known Issues
Minor layout shifts may occur on very small screen sizes below 320px.

Occasional flickering when switching device orientation rapidly.

Some third-party icons may not render perfectly on older Android versions.

Pull-to-refresh gesture can be unresponsive on slower devices under heavy load.

Performance may degrade slightly with a very large number of dashboard widgets.


## Future Enhancements
Add dark mode support for improved usability in low-light environments.

Implement user-customizable dashboard widgets and layout preferences.

Enhance accessibility features, including better screen reader support and larger touch targets.

Integrate real-time data updates via WebSocket or push notifications.

Support for landscape mode on phones with adaptive widget resizing.

Add localization and multi-language support.

Improve animations with gesture-based interactions for smoother UX.