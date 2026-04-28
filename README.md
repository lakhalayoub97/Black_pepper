# Black Pepper Restaurant Website

A modern, responsive website for Black Pepper, an upscale Moroccan restaurant located in Meknès, Morocco.

## Features

- **Home Page**: Hero section with restaurant branding, 4.4-star rating display, and service highlights
- **Menu Page**: Organized menu with categories (Starters, Main Dishes, Drinks, Desserts) with pricing and descriptions
- **About Us**: Restaurant story, values, and what makes Black Pepper special
- **Gallery**: Visual showcase of dishes and restaurant ambiance
- **Reviews**: Customer testimonials and ratings
- **Contact Page**: Location information, contact form, and embedded Google Maps
- **Responsive Design**: Fully optimized for mobile, tablet, and desktop devices
- **Dark Theme**: Elegant dark interface with red and gold accents

## Technologies Used

- **Next.js 16** - React framework with App Router
- **React 19** - UI library
- **TypeScript** - Type safety
- **Tailwind CSS v4** - Utility-first CSS framework
- **Geist Font** - Modern typography

## Installation

### Prerequisites
- Node.js 18+ installed on your machine
- npm or yarn package manager

### Steps

1. **Extract the project**
   ```bash
   # Navigate to the project folder
   cd black-pepper-restaurant
   ```

2. **Install dependencies**
   ```bash
   npm install
   ```

3. **Run the development server**
   ```bash
   npm run dev
   ```

4. **Open in browser**
   - Visit `http://localhost:3000`
   - The site will automatically reload as you make changes

## Project Structure

```
├── app/
│   ├── page.tsx                 # Home page
│   ├── menu/page.tsx            # Menu page
│   ├── about/page.tsx           # About Us page
│   ├── gallery/page.tsx         # Gallery page
│   ├── reviews/page.tsx         # Reviews page
│   ├── contact/page.tsx         # Contact page
│   ├── layout.tsx               # Root layout with metadata
│   └── globals.css              # Global styles and design tokens
├── components/
│   ├── navigation.tsx           # Main navigation bar
│   ├── footer.tsx               # Footer component
│   ├── hero-section.tsx         # Home page hero
│   ├── highlights-section.tsx   # Features/highlights section
│   ├── menu-categories.tsx      # Menu filtering
│   ├── menu-item-card.tsx       # Individual menu item card
│   ├── contact-form.tsx         # Contact form
│   └── ui/                      # shadcn/ui components
├── public/
│   ├── elegant-restaurant-dish.jpg
│   ├── moroccan-.jpg
│   ├── dish-1.jpg
│   ├── dish-2.jpg
│   ├── dish-3.jpg
│   ├── restaurant-interior.jpg
│   ├── ambiance.jpg
│   └── dessert.jpg
├── package.json                 # Project dependencies
└── tsconfig.json               # TypeScript configuration
```

## Customization Guide

### Update Restaurant Information

Edit `app/layout.tsx` to update:
- Restaurant name
- Meta description
- Favicon

### Modify Menu Items

Edit `components/menu-categories.tsx` to:
- Add/remove menu categories
- Update dish names, descriptions, and prices
- Change bestseller badges

### Update Contact Information

Edit `app/contact/page.tsx` to:
- Change phone number, email, address
- Update Google Maps embed code
- Modify business hours

### Change Colors & Theme

Edit `app/globals.css` to modify:
- `--primary` - Main brand color (red)
- `--primary-dark` - Darker red variant
- `--accent` - Gold/accent color
- `--background` - Dark background
- `--foreground` - Text color

### Replace Images

1. Place new images in the `public/` folder
2. Update image paths in components:
   ```tsx
   <img src="/your-image-name.jpg" alt="Description" />
   ```

## Building for Production

```bash
npm run build
```

This creates an optimized production build in the `.next` folder.

## Deploying to Vercel

1. **In v0**: Click **Publish** button in the top right
2. **Or manually**:
   - Push code to GitHub
   - Connect repository to Vercel
   - Vercel automatically deploys on every push

## Available Scripts

- `npm run dev` - Start development server
- `npm run build` - Build for production
- `npm run start` - Start production server
- `npm run lint` - Run ESLint checks

## Browser Support

- Chrome (latest)
- Firefox (latest)
- Safari (latest)
- Edge (latest)

## License

This project is provided as-is for Black Pepper Restaurant.

## Support

For questions or issues:
1. Check the [Next.js documentation](https://nextjs.org/docs)
2. Review [Tailwind CSS docs](https://tailwindcss.com/docs)
3. Visit [React documentation](https://react.dev)

---

Built with ❤️ for Black Pepper Restaurant, Meknès, Morocco
