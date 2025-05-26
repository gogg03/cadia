# Cadia - Circadian Rhythm Sleep Optimization App

## Project Overview

Cadia is a self-hosted web application designed to optimize sleep patterns using natural circadian rhythms, solar/lunar cycles, and environmental factors. The app provides personalized sleep recommendations based on location-specific solar time, moon phases, and geomagnetic activity.

## Core Concept

The application moves beyond traditional clock-based sleep scheduling to embrace natural biological rhythms influenced by:
- Solar positioning and natural light cycles
- Lunar phases and gravitational effects
- Schumann resonance (Earth's electromagnetic field)
- Solar activity and geomagnetic conditions
- Individual location and timezone considerations

## Target Users

- Health-conscious individuals seeking natural sleep optimization
- People with irregular sleep schedules
- Users interested in circadian biology and natural rhythms
- Self-hosting enthusiasts who value data privacy

## Key Features

### Phase 1: Core Functionality
1. **Cadia Time Display**
   - Location-based solar time calculation
   - Real-time display of natural time vs. clock time
   - DST compensation and timezone handling

2. **Sleep Recommendations**
   - Current sleep suggestion based on solar position
   - Optimal bedtime and wake time calculations
   - Integration with sunrise/sunset data

3. **Basic Alarms**
   - Wake alarm based on natural light cycles
   - Local notification system
   - Customizable alarm preferences

### Phase 2: Environmental Integration
1. **Lunar Cycle Integration**
   - Moon phase tracking and display
   - Sleep recommendations adjusted for lunar influence
   - Historical correlation with personal sleep patterns

2. **Solar Activity Monitoring**
   - Real-time solar activity data (NOAA)
   - Geomagnetic storm alerts
   - Impact assessment on sleep quality

3. **Schumann Resonance Tracking**
   - Earth's electromagnetic field monitoring
   - Correlation with sleep and wellness patterns
   - Historical data visualization

### Phase 3: Advanced Analytics
1. **Circadian Reports**
   - Daily circadian rhythm analysis
   - Visual sleep pattern tracking
   - Correlation with environmental factors

2. **Sleep Planning**
   - Multi-day sleep optimization
   - Travel and timezone adjustment planning
   - Seasonal adaptation recommendations

3. **Data Storage & Export**
   - Local sleep log database
   - Personal data export capabilities
   - Privacy-focused data handling

## User Experience Design

### Interface Principles
- **Mobile-first design**: Optimized for smartphone usage
- **Dark mode support**: Reduces blue light exposure
- **Minimal UI**: Clean, distraction-free interface
- **Intuitive navigation**: Simple, gesture-based interactions

### Core User Flows

#### Primary Flow: Check Current Sleep Recommendation
1. User opens app
2. App displays current "Cadia Time"
3. Shows immediate sleep recommendation
4. Provides context (solar position, moon phase, etc.)
5. Offers action buttons (set alarm, view details)

#### Secondary Flow: Plan Sleep Schedule
1. User navigates to planning section
2. Selects date range for optimization
3. App calculates optimal sleep windows
4. User reviews and adjusts preferences
5. System sets automated reminders

#### Tertiary Flow: Review Sleep History
1. User accesses history/analytics
2. Views sleep pattern visualizations
3. Correlates with environmental data
4. Identifies optimization opportunities
5. Adjusts future recommendations

### Visual Design
- **Color scheme**: Earth tones with blue accents
- **Typography**: Clean, readable fonts optimized for mobile
- **Icons**: Nature-inspired iconography
- **Animations**: Subtle, purposeful transitions
- **Data visualization**: Clear charts and graphs

## Technical Requirements

### Performance
- App loads in under 2 seconds
- Offline functionality for core features
- Real-time data updates without page refresh
- Responsive design across all device sizes

### Accessibility
- WCAG 2.1 AA compliance
- Screen reader compatibility
- High contrast mode support
- Keyboard navigation support

### Security & Privacy
- All data stored locally by default
- No tracking or analytics
- Optional data export only
- Self-hosted deployment model

## Data Sources & APIs

### External APIs
- **Sunrise/Sunset**: sunrise-sunset.org/api
- **Moon Phases**: api.farmsense.net/v1/moonphases/
- **Timezone/DST**: worldtimeapi.org
- **Solar Activity**: services.swpc.noaa.gov/json/
- **Schumann Resonance**: HeartMath (scraped data)

### Data Processing
- Real-time API integration with fallback caching
- Local data storage for offline functionality
- Automated data refresh cycles
- Error handling for API downtime

## Progressive Web App Features

### Installation
- Add to home screen capability
- Native app-like experience
- Offline functionality
- Background sync for data updates

### Notifications
- Local push notifications for sleep reminders
- Customizable notification preferences
- Respect for device "Do Not Disturb" settings
- Optional geomagnetic event alerts

## Success Metrics

### User Engagement
- Daily active usage
- Sleep recommendation adherence
- Feature utilization rates
- User retention over time

### Health Outcomes
- Self-reported sleep quality improvements
- Sleep pattern consistency
- Reduced time to fall asleep
- Improved wake-up experience

## Future Enhancements

### Phase 4: Extended Features
- Smartwatch integration
- Wearable device data import
- Advanced sleep analytics
- Community features (optional)

### Phase 5: Ecosystem Integration
- Home automation integration
- Smart lighting control
- Temperature optimization
- Sound environment management

## Technical Architecture Notes

This app design integrates with the technical stack defined in [Tech-stack.md](mdc:memory-bank/Tech-stack.md) and follows the implementation timeline in [Implementation-plan.md](mdc:memory-bank/Implementation-plan.md).

Key architectural decisions:
- Self-hosted deployment for privacy
- PWA for cross-platform compatibility
- Local-first data storage
- API-driven environmental data integration
- Docker containerization for portability 