# Arabic Translation Plan

## Overview
This document outlines the plan for creating an Arabic version of the portfolio website while maintaining all functionality and improving accessibility for Arabic-speaking users.

## File Structure
```
├── index.html         (Original English version)
├── index-ar.html      (New Arabic version)
├── css/
│   ├── style.css     (Original styles)
│   └── style-rtl.css (New RTL styles)
└── js/
    ├── main.js       (Original JavaScript)
    └── main-ar.js    (Arabic version JavaScript)
```

## Technical Implementation

### 1. HTML Changes
- Set `lang="ar"` and `dir="rtl"`
- Add Cairo font from Google Fonts
- Update meta tags and title
- Translate all text content while preserving HTML structure
- Mirror navigation and layout elements

### 2. CSS Modifications (style-rtl.css)
```css
/* Key RTL Changes */
body {
    direction: rtl;
    text-align: right;
    font-family: 'Cairo', sans-serif;
}

/* Mirror margins/paddings */
.ms-* { margin-right: *; margin-left: 0 !important; }
.me-* { margin-left: *; margin-right: 0 !important; }
.ps-* { padding-right: *; padding-left: 0 !important; }
.pe-* { padding-left: *; padding-right: 0 !important; }

/* Mirror Bootstrap grid */
.offset-* { margin-right: auto; margin-left: 0; }
```

### 3. JavaScript Updates (main-ar.js)
- Translate typed text strings
- Update portfolio filters text
- Maintain all animation and interaction functionality

### 4. Font Implementation
```css
@import url('https://fonts.googleapis.com/css2?family=Cairo:wght@400;500;600;700&display=swap');
```

## Content Translation Guidelines
1. Maintain professional tone in Arabic
2. Preserve technical terms where appropriate
3. Adapt CTAs and buttons for Arabic context
4. Keep measurements and numbers in Arabic numerals
5. Mirror iconography and arrows

## Testing Checklist
- [ ] RTL layout verification
- [ ] Arabic font rendering
- [ ] Responsive design in RTL
- [ ] Interactive features
- [ ] Portfolio filters
- [ ] Animations and transitions
- [ ] Contact form validation
- [ ] Cross-browser testing

## Next Steps
1. Create Arabic version files
2. Implement RTL styles
3. Update JavaScript strings
4. Test all functionality
5. Deploy and verify

## Notes
- Preserve all existing functionality
- Maintain consistent branding
- Ensure smooth bilingual user experience