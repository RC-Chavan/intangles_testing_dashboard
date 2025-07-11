# Integration Testing Coverage Analysis

## Bar Chart - Services Coverage

```mermaid
%%{init: {'theme':'base', 'themeVariables': { 'primaryColor': '#4CAF50', 'primaryTextColor': '#ffffff', 'primaryBorderColor': '#45a049', 'lineColor': '#333', 'secondaryColor': '#FF9800', 'tertiaryColor': '#f4f4f4'}}}%%
xychart-beta
    title "Integration Testing - Services Coverage"
    x-axis ["Total Services", "Covered Services", "Uncovered Services"]
    y-axis "Number of Services" 0 --> 120
    bar [101, 32, 69]
```

## Bar Chart - Specs Coverage

```mermaid
%%{init: {'theme':'base', 'themeVariables': { 'primaryColor': '#2196F3', 'primaryTextColor': '#ffffff', 'primaryBorderColor': '#1976D2', 'lineColor': '#333', 'secondaryColor': '#FF5722', 'tertiaryColor': '#f4f4f4'}}}%%
xychart-beta
    title "Integration Testing - Specs Coverage"
    x-axis ["Total Specs", "Covered Specs", "Uncovered Specs"]
    y-axis "Number of Specs" 0 --> 6000
    bar [5734, 1836, 3898]
```

## Radar Chart - Overall Coverage Metrics

```mermaid
%%{init: {'theme':'base', 'themeVariables': { 'primaryColor': '#9C27B0', 'primaryTextColor': '#ffffff', 'primaryBorderColor': '#7B1FA2', 'lineColor': '#333'}}}%%
quadrantChart
    title Integration Testing Coverage Overview
    x-axis Low Coverage --> High Coverage
    y-axis Services --> Specs
    
    quadrant-1 High Spec Coverage
    quadrant-2 High Service & Spec Coverage
    quadrant-3 Low Coverage
    quadrant-4 High Service Coverage
    
    Services Coverage: [0.33, 0.65]
    Specs Coverage: [0.32, 0.35]
```

## Pie Chart - Services Coverage Distribution

```mermaid
%%{init: {'theme':'base', 'themeVariables': { 'pie1': '#4CAF50', 'pie2': '#FF5722', 'pieOuterStrokeWidth': '2px'}}}%%
pie title Services Coverage Distribution
    "Covered Services (32%)" : 32
    "Uncovered Services (68%)" : 69
```

## Pie Chart - Specs Coverage Distribution

```mermaid
%%{init: {'theme':'base', 'themeVariables': { 'pie1': '#2196F3', 'pie2': '#FF9800', 'pieOuterStrokeWidth': '2px'}}}%%
pie title Specs Coverage Distribution
    "Covered Specs (32%)" : 1836
    "Uncovered Specs (68%)" : 3898
```

## Coverage Summary Table

| Metric | Total | Covered | Coverage % | Status |
|--------|-------|---------|------------|--------|
| **Services** | 101 | 32 | 32.0% | 🟡 Needs Improvement |
| **Specs** | 5,734 | 1,836 | 32.0% | 🟡 Needs Improvement |

## Key Insights

### Services Coverage (32%)
- **Total Services**: 101
- **Covered Services**: 32
- **Gap**: 69 services need integration tests

### Specs Coverage (32%)
- **Total Specs**: 5,734
- **Covered Specs**: 1,836
- **Gap**: 3,898 specs need integration tests

### Priority Areas for Improvement
1. **Critical Services**: Focus on core services like internal-app, external-app, parser
2. **High-Impact Specs**: Prioritize frequently used specifications
3. **Service Dependencies**: Cover services that are dependencies for other services

### Coverage Goals
- **Short-term**: Achieve 50% service coverage (49 services)
- **Medium-term**: Achieve 60% spec coverage (3,441 specs)
- **Long-term**: Achieve 80% overall coverage across both metrics
