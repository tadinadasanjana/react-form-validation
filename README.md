# React Form Validation App

A comprehensive React form application with validation, password visibility toggle, and multi-step routing using React Router.

## Features

✨ **Form Fields:**
- First Name & Last Name
- Username
- Email
- Password (with show/hide toggle)
- Country Code & Phone Number
- Country & City
- PAN & Aadhaar

🔐 **Validation:**
- Required field validation
- Email format validation
- Password minimum 8 characters
- Phone number must be 10 digits
- PAN format validation (ABCDE1234F)
- Aadhaar must be 12 digits

⚙️ **Features:**
- Real-time form state tracking with `useState`
- Conditional error message rendering
- Submit button disabled until form is valid
- Responsive design for mobile, tablet, and desktop
- Error-highlighted input fields (red border + light red background)
- Redirect to details page on successful submission
- Details page displays all submitted information
- Password masking in details view (shows only last 4 digits)
- Back button to return to form

## Project Structure

```
src/
├── pages/
│   ├── Form.jsx          # Registration form component
│   ├── Form.css          # Form styling
│   ├── Details.jsx       # Details display component
│   └── Details.css       # Details styling
├── utils/
│   └── validation.js     # Validation functions
├── App.jsx               # Main app with routing
├── main.jsx              # React entry point
├── index.css             # Global styles
└── vite.config.js        # Vite configuration
```

## Getting Started

### Prerequisites
- Node.js (v14 or higher)
- npm or yarn

### Installation

```bash
npm install
```

### Running the Application

```bash
npm run dev
```

The app will open at `http://localhost:3000`

### Building for Production

```bash
npm run build
```

## Technologies Used

- **React 18.2** - UI library
- **React Router DOM 6.20** - Client-side routing
- **Vite 5.0** - Build tool
- **CSS3** - Styling with responsive design

## Form Validation Rules

| Field | Rules |
|-------|-------|
| First Name | Required, non-empty |
| Last Name | Required, non-empty |
| Username | Required, non-empty |
| Email | Required, valid email format |
| Password | Required, minimum 8 characters |
| Country Code | Required, non-empty |
| Phone No. | Required, exactly 10 digits |
| Country | Required, must select from dropdown |
| City | Required, non-empty |
| PAN | Required, format: 5 letters + 4 digits + 1 letter (e.g., ABCDE1234F) |
| Aadhaar | Required, exactly 12 digits |

## How It Works

1. **Form Page**: Fill out all required fields
2. **Validation**: Error messages appear below fields with invalid input
3. **Submit Button**: Enabled only when all fields are valid
4. **Submission**: On submit, form data is stored in localStorage
5. **Details Page**: Displays all submitted information with secure password handling
6. **Navigation**: Use back button to return to form

## Responsive Design

The form is fully responsive with:
- Desktop layout: 2-column grid for paired fields
- Tablet layout: Adjusted spacing and font sizes
- Mobile layout: Single column with optimized touch targets

## Browser Compatibility

- Chrome (latest)
- Firefox (latest)
- Safari (latest)
- Edge (latest)

## License

MIT
## 🎥 Demo Video

This video demonstrates:
- Form validation
- Error handling
- Password show/hide
- Submission & navigation

🔗 Demo link: https://drive.google.com/file/d/1h8G_FRe99ysE5HuBshqM7QxiZJa7eU89/view?t=5

